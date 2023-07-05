# Comparing `tmp/apache-airflow-providers-elasticsearch-4.5.1rc1.tar.gz` & `tmp/apache-airflow-providers-elasticsearch-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-elasticsearch-4.5.1rc1.tar", last modified: Tue Jun 20 11:41:58 2023, max compression
+gzip compressed data, was "apache-airflow-providers-elasticsearch-5.0.0rc1.tar", last modified: Wed Jul  5 07:29:59 2023, max compression
```

## Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1.tar` & `apache-airflow-providers-elasticsearch-5.0.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.308214 apache-airflow-providers-elasticsearch-4.5.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:57.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15999 2023-06-20 11:41:58.309306 apache-airflow-providers-elasticsearch-4.5.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14423 2023-06-20 11:41:57.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.229915 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.230978 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.266842 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-20 11:01:09.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-06-20 11:41:57.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.272499 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5477 2023-06-02 11:31:21.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.281083 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-05 12:50:36.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)    17266 2023-06-02 11:31:21.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/es_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:58.305539 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15999 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      868 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:58.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1992 2023-06-20 11:41:58.311232 apache-airflow-providers-elasticsearch-4.5.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:41:57.000000 apache-airflow-providers-elasticsearch-4.5.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.248184 apache-airflow-providers-elasticsearch-5.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-05 07:29:59.248779 apache-airflow-providers-elasticsearch-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4046 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.153473 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.154748 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.203164 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 07:19:39.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.210183 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6474 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.220252 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    19313 2023-06-29 05:49:30.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:59.245375 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      868 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:59.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-05 07:29:59.250722 apache-airflow-providers-elasticsearch-5.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-07-05 07:29:58.000000 apache-airflow-providers-elasticsearch-5.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/LICENSE` & `apache-airflow-providers-elasticsearch-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/MANIFEST.in` & `apache-airflow-providers-elasticsearch-5.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.5.1"
+__version__ = "5.0.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/get_provider_info.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-elasticsearch",
         "name": "Elasticsearch",
         "description": "`Elasticsearch <https://www.elastic.co/elasticsearch>`__\n",
         "suspended": False,
         "versions": [
+            "5.0.0",
             "4.5.1",
             "4.5.0",
             "4.4.0",
             "4.3.3",
             "4.3.2",
             "4.3.1",
             "4.3.0",
@@ -55,16 +56,14 @@
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
             "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "elasticsearch>7,<7.15.0",
-            "elasticsearch-dbapi",
-            "elasticsearch-dsl>=5.0.0",
         ],
         "integrations": [
             {
                 "integration-name": "Elasticsearch",
                 "external-doc-url": "https://www.elastic.co/elasticsearch",
                 "logo": "/integration-logos/elasticsearch/Elasticsearch.png",
                 "tags": ["software"],
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/hooks/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,61 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from functools import cached_property
 from typing import Any
+from urllib import parse
 
 from elasticsearch import Elasticsearch
-from es.elastic.api import Connection as ESConnection, connect
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.models.connection import Connection as AirflowConnection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 
+def connect(
+    host: str = "localhost",
+    port: int = 9200,
+    user: str | None = None,
+    password: str | None = None,
+    scheme: str = "http",
+    **kwargs: Any,
+) -> ESConnection:
+    return ESConnection(host, port, user, password, scheme, **kwargs)
+
+
+class ESConnection:
+    """wrapper class for elasticsearch.Elasticsearch."""
+
+    def __init__(
+        self,
+        host: str = "localhost",
+        port: int = 9200,
+        user: str | None = None,
+        password: str | None = None,
+        scheme: str = "http",
+        **kwargs: Any,
+    ):
+        self.host = host
+        self.port = port
+        self.user = user
+        self.password = password
+        self.scheme = scheme
+        self.kwargs = kwargs
+        netloc = f"{host}:{port}"
+        self.url = parse.urlunparse((scheme, netloc, "/", None, None, None))
+        if user and password:
+            self.es = Elasticsearch(self.url, http_auth=(user, password), **self.kwargs)
+        else:
+            self.es = Elasticsearch(self.url, **self.kwargs)
+
+
 class ElasticsearchSQLHook(DbApiHook):
     """
     Interact with Elasticsearch through the elasticsearch-dbapi.
 
     This hook uses the Elasticsearch conn_id.
 
     :param elasticsearch_conn_id: The :ref:`ElasticSearch connection id <howto/connection:elasticsearch>`
@@ -100,14 +137,15 @@
 
         return uri
 
 
 class ElasticsearchHook(ElasticsearchSQLHook):
     """
     This class is deprecated and was renamed to ElasticsearchSQLHook.
+
     Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.
     """
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.""",
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/__init__.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/es_json_formatter.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,15 @@
     """Convert a log record to JSON with ISO 8601 date and time format."""
 
     default_time_format = "%Y-%m-%dT%H:%M:%S"
     default_msec_format = "%s.%03d"
     default_tz_format = "%z"
 
     def formatTime(self, record, datefmt=None):
-        """
-        Returns the creation time of the specified LogRecord in ISO 8601 date and time format
-        in the local time zone.
-        """
+        """Return the creation time of the LogRecord in ISO 8601 date/time format in the local time zone."""
         dt = pendulum.from_timestamp(record.created, tz=pendulum.local_timezone())
         if datefmt:
             s = dt.strftime(datefmt)
         else:
             s = dt.strftime(self.default_time_format)
 
         if self.default_msec_format:
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/airflow/providers/elasticsearch/log/es_task_handler.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from time import time
 from typing import TYPE_CHECKING, List, Tuple
 from urllib.parse import quote
 
 # Using `from elasticsearch import *` would break elasticsearch mocking used in unit test.
 import elasticsearch
 import pendulum
-from elasticsearch_dsl import Search
+from elasticsearch.exceptions import ElasticsearchException, NotFoundError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models.dagrun import DagRun
 from airflow.models.taskinstance import TaskInstance
 from airflow.providers.elasticsearch.log.es_json_formatter import ElasticsearchJSONFormatter
 from airflow.utils import timezone
@@ -48,29 +48,61 @@
 
 # Compatibility: Airflow 2.3.3 and up uses this method, which accesses the
 # LogTemplate model to record the log ID template used. If this function does
 # not exist, the task handler should use the log_id_template attribute instead.
 USE_PER_RUN_LOG_ID = hasattr(DagRun, "get_log_template")
 
 
+class Log:
+    """wrapper class to mimic the attributes in Search class used in elasticsearch_dsl.Search."""
+
+    def __init__(self, offset):
+        self.offset = offset
+
+
+class ElasticSearchResponse:
+    """wrapper class to mimic the Search class used in elasticsearch_dsl.Search."""
+
+    def __init__(self, **kwargs):
+        # Store all provided keyword arguments as attributes of this object
+        for key, value in kwargs.items():
+            if key == "log":
+                setattr(self, key, Log(**value))
+            else:
+                setattr(self, key, value)
+
+    def to_dict(self):
+        result = {}
+        for key in self.__dict__.keys():
+            if key == "log":
+                result[key] = self.__dict__[key].__dict__
+            else:
+                result[key] = self.__dict__[key]
+        return result
+
+
 class ElasticsearchTaskHandler(FileTaskHandler, ExternalLoggingMixin, LoggingMixin):
     """
-    ElasticsearchTaskHandler is a python log handler that
-    reads logs from Elasticsearch. Note that Airflow does not handle the indexing
-    of logs into Elasticsearch. Instead, Airflow flushes logs
-    into local files. Additional software setup is required
-    to index the logs into Elasticsearch, such as using
-    Filebeat and Logstash.
+    ElasticsearchTaskHandler is a python log handler that reads logs from Elasticsearch.
+
+    Note that Airflow does not handle the indexing of logs into Elasticsearch. Instead,
+    Airflow flushes logs into local files. Additional software setup is required to index
+    the logs into Elasticsearch, such as using Filebeat and Logstash.
+
     To efficiently query and sort Elasticsearch results, this handler assumes each
     log message has a field `log_id` consists of ti primary keys:
     `log_id = {dag_id}-{task_id}-{execution_date}-{try_number}`
     Log messages with specific log_id are sorted based on `offset`,
     which is a unique integer indicates log message's order.
     Timestamps here are unreliable because multiple log messages
     might have the same timestamp.
+
+    :param base_log_folder: base folder to store logs locally
+    :param log_id_template: log id template
+    :param host: Elasticsearch host name
     """
 
     PAGE = 0
     MAX_LINE_PER_PAGE = 1000
     LOG_NAME = "Elasticsearch"
 
     trigger_should_wrap = True
@@ -88,19 +120,14 @@
         frontend: str = "localhost:5601",
         index_patterns: str | None = conf.get("elasticsearch", "index_patterns", fallback="_all"),
         es_kwargs: dict | None = conf.getsection("elasticsearch_configs"),
         *,
         filename_template: str | None = None,
         log_id_template: str | None = None,
     ):
-        """
-        :param base_log_folder: base folder to store logs locally
-        :param log_id_template: log id template
-        :param host: Elasticsearch host name
-        """
         es_kwargs = es_kwargs or {}
         super().__init__(base_log_folder, filename_template)
         self.closed = False
 
         self.client = elasticsearch.Elasticsearch(host.split(";"), **es_kwargs)  # type: ignore[attr-defined]
 
         if USE_PER_RUN_LOG_ID and log_id_template is not None:
@@ -166,16 +193,15 @@
             try_number=try_number,
             map_index=getattr(ti, "map_index", ""),
         )
 
     @staticmethod
     def _clean_date(value: datetime | None) -> str:
         """
-        Clean up a date value so that it is safe to query in elasticsearch
-        by removing reserved characters.
+        Clean up a date value so that it is safe to query in elasticsearch by removing reserved characters.
 
         https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-query-string-query.html#_reserved_characters
         """
         if value is None:
             return ""
         return value.strftime("%Y_%m_%dT%H_%M_%S_%f")
 
@@ -205,20 +231,17 @@
         if not metadata:
             metadata = {"offset": 0}
         if "offset" not in metadata:
             metadata["offset"] = 0
 
         offset = metadata["offset"]
         log_id = self._render_log_id(ti, try_number)
-
         logs = self.es_read(log_id, offset, metadata)
         logs_by_host = self._group_logs_by_host(logs)
-
         next_offset = offset if not logs else attrgetter(self.offset_field)(logs[-1])
-
         # Ensure a string here. Large offset numbers will get JSON.parsed incorrectly
         # on the client. Sending as a string prevents this issue.
         # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/MAX_SAFE_INTEGER
         metadata["offset"] = str(next_offset)
 
         # end_of_log_mark may contain characters like '\n' which is needed to
         # have the log uploaded but will not be stored in elasticsearch.
@@ -255,15 +278,14 @@
         # If we hit the end of the log, remove the actual end_of_log message
         # to prevent it from showing in the UI.
         def concat_logs(lines):
             log_range = (len(lines) - 1) if lines[-1].message == self.end_of_log_mark else len(lines)
             return "\n".join(self._format_msg(lines[i]) for i in range(log_range))
 
         message = [(host, concat_logs(hosted_log)) for host, hosted_log in logs_by_host.items()]
-
         return message, metadata
 
     def _format_msg(self, log_line):
         """Format ES Record to match settings.LOG_FORMAT when used with json_format."""
         # Using formatter._style.format makes it future proof i.e.
         # if we change the formatter style from '%' to '{' or '$', this will still work
         if self.json_format:
@@ -275,47 +297,58 @@
                 pass
 
         # Just a safe-guard to preserve backwards-compatibility
         return log_line.message
 
     def es_read(self, log_id: str, offset: str, metadata: dict) -> list:
         """
-        Returns the logs matching log_id in Elasticsearch and next offset.
-        Returns '' if no log is found or there was an error.
+        Return the logs matching log_id in Elasticsearch and next offset or ''.
 
         :param log_id: the log_id of the log to read.
         :param offset: the offset start to read log from.
         :param metadata: log metadata, used for steaming log download.
         """
         # Offset is the unique key for sorting logs given log_id.
-        search = (
-            Search(index=self.index_patterns, using=self.client)
-            .query("match_phrase", log_id=log_id)
-            .sort(self.offset_field)
-        )
+        query = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"match_phrase": {"log_id": log_id}},
+                        {"range": {self.offset_field: {"gt": int(offset)}}},
+                    ]
+                }
+            },
+            "sort": [{self.offset_field: {"order": "asc"}}],
+        }
 
-        search = search.filter("range", **{self.offset_field: {"gt": int(offset)}})
-        max_log_line = search.count()
-        if "download_logs" in metadata and metadata["download_logs"] and "max_offset" not in metadata:
-            try:
-                if max_log_line > 0:
-                    metadata["max_offset"] = attrgetter(self.offset_field)(
-                        search[max_log_line - 1].execute()[-1]
-                    )
-                else:
-                    metadata["max_offset"] = 0
-            except Exception:
-                self.log.exception("Could not get current log size with log_id: %s", log_id)
+        try:
+            max_log_line = self.client.count(index=self.index_patterns, body=query)["count"]
+        except NotFoundError as e:
+            self.log.exception("The target index pattern %s does not exist", self.index_patterns)
+            raise e
+        except ElasticsearchException as e:
+            self.log.exception("Could not get current log size with log_id: %s", log_id)
+            raise e
 
         logs = []
         if max_log_line != 0:
             try:
-
-                logs = search[self.MAX_LINE_PER_PAGE * self.PAGE : self.MAX_LINE_PER_PAGE].execute()
-            except Exception:
+                res = self.client.search(
+                    index=self.index_patterns,
+                    body=query,
+                    size=self.MAX_LINE_PER_PAGE,
+                    from_=self.MAX_LINE_PER_PAGE * self.PAGE,
+                )
+                logs = [
+                    ElasticSearchResponse(
+                        **unwrap_response(response),
+                    )
+                    for response in res["hits"]["hits"]
+                ]
+            except elasticsearch.exceptions.ElasticsearchException:
                 self.log.exception("Could not read log with log_id: %s", log_id)
 
         return logs
 
     def emit(self, record):
         if self.handler:
             setattr(record, self.offset_field, int(time() * (10**9)))
@@ -425,7 +458,37 @@
 
     :meta private:
     """
     try:
         return attrgetter(item)(obj)
     except AttributeError:
         return default
+
+
+def unwrap_response(res):
+    source = res["_source"]
+    transformed = {
+        "log_id": source.get("log_id"),
+        "message": source.get("message"),
+        "meta": {
+            "id": res.get("_id"),
+            "index": res.get("_index"),
+            "version": res.get("_version"),
+            "headers": res.get("_headers"),
+        },
+    }
+    if "offset" in source:
+        transformed["offset"] = source["offset"]
+    if "asctime" in source:
+        transformed["asctime"] = source["asctime"]
+    if "filename" in source:
+        transformed["filename"] = source["filename"]
+    if "host" in source:
+        transformed["host"] = source["host"]
+    if "levelname" in source:
+        transformed["levelname"] = source["levelname"]
+    if "lineno" in source:
+        transformed["lineno"] = source["lineno"]
+    if "log" in source:
+        transformed["log"] = source["log"]
+
+    return transformed
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt` & `apache-airflow-providers-elasticsearch-5.0.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/pyproject.toml` & `apache-airflow-providers-elasticsearch-5.0.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/setup.cfg` & `apache-airflow-providers-elasticsearch-5.0.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/5.0.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -44,16 +45,14 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.4.0.dev0
-	elasticsearch-dbapi
-	elasticsearch-dsl>=5.0.0
 	elasticsearch>7,<7.15.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.elasticsearch.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-elasticsearch-4.5.1rc1/setup.py` & `apache-airflow-providers-elasticsearch-5.0.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-elasticsearch package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.5.1"
+version = "5.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-elasticsearch setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

