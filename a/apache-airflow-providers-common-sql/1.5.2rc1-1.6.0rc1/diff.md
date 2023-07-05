# Comparing `tmp/apache-airflow-providers-common-sql-1.5.2rc1.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-common-sql-1.5.2rc1.tar", last modified: Tue Jun 20 11:41:45 2023, max compression
+gzip compressed data, was "apache-airflow-providers-common-sql-1.6.0rc1.tar", last modified: Wed Jul  5 07:29:52 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.5.2rc1.tar` & `apache-airflow-providers-common-sql-1.6.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.301147 apache-airflow-providers-common-sql-1.5.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.5.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:44.000000 apache-airflow-providers-common-sql-1.5.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.5.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10837 2023-06-20 11:41:45.302237 apache-airflow-providers-common-sql-1.5.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9274 2023-06-20 11:41:44.000000 apache-airflow-providers-common-sql-1.5.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.205910 apache-airflow-providers-common-sql-1.5.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.206905 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.207999 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.241758 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-06-20 11:41:44.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.250908 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21736 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.257158 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44504 2023-06-02 11:31:21.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.263533 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:45.298495 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10837 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:45.000000 apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-common-sql-1.5.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 11:41:45.304206 apache-airflow-providers-common-sql-1.5.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1690 2023-06-20 11:41:44.000000 apache-airflow-providers-common-sql-1.5.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.932599 apache-airflow-providers-common-sql-1.6.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-05 07:29:52.933230 apache-airflow-providers-common-sql-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.846572 apache-airflow-providers-common-sql-1.6.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.847607 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.848699 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.885380 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 07:19:39.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.891800 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23794 2023-06-29 14:43:21.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.898281 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46803 2023-06-29 14:43:21.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.904996 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 07:29:52.929896 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 07:29:52.000000 apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-common-sql-1.6.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-05 07:29:52.935124 apache-airflow-providers-common-sql-1.6.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-05 07:29:51.000000 apache-airflow-providers-common-sql-1.6.0rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/LICENSE` & `apache-airflow-providers-common-sql-1.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/MANIFEST.in` & `apache-airflow-providers-common-sql-1.6.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.5.2"
+__version__ = "1.6.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-sql",
         "name": "Common SQL",
         "description": "`Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__\n",
         "suspended": False,
         "versions": [
+            "1.6.0",
             "1.5.2",
             "1.5.1",
             "1.5.0",
             "1.4.0",
             "1.3.4",
             "1.3.3",
             "1.3.2",
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from contextlib import closing
 from datetime import datetime
-from typing import Any, Callable, Iterable, Mapping, Protocol, Sequence, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, Protocol, Sequence, cast
+from urllib.parse import urlparse
 
 import sqlparse
 from packaging.version import Version
 from sqlalchemy import create_engine
 
 from airflow import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.version import version
 
+if TYPE_CHECKING:
+    from airflow.providers.openlineage.extractors import OperatorLineage
+    from airflow.providers.openlineage.sqlparser import DatabaseInfo
+
 
 def return_single_query_results(sql: str | Iterable[str], return_last: bool, split_statements: bool):
     """
     Determines when results of single query only should be returned.
 
     For compatibility reasons, the behaviour of the DBAPIHook is somewhat confusing.
     In some cases, when multiple queries are run, the return value will be an iterable (list) of results
@@ -251,16 +256,15 @@
         """
         Splits string into multiple SQL expressions.
 
         :param sql: SQL string potentially consisting of multiple expressions
         :return: list of individual expressions
         """
         splits = sqlparse.split(sqlparse.format(sql, strip_comments=True))
-        statements: list[str] = list(filter(None, splits))
-        return statements
+        return [s for s in splits if s]
 
     @property
     def last_description(self) -> Sequence[Sequence] | None:
         if not self.descriptions:
             return None
         return self.descriptions[-1]
 
@@ -511,7 +515,56 @@
                 status = True
                 message = "Connection successfully tested"
         except Exception as e:
             status = False
             message = str(e)
 
         return status, message
+
+    def get_openlineage_database_info(self, connection) -> DatabaseInfo | None:
+        """
+        Returns database specific information needed to generate and parse lineage metadata.
+
+        This includes information helpful for constructing information schema query
+        and creating correct namespace.
+
+        :param connection: Airflow connection to reduce calls of `get_connection` method
+        """
+
+    def get_openlineage_database_dialect(self, connection) -> str:
+        """
+        Returns database dialect used for SQL parsing.
+
+        For a list of supported dialects check: https://openlineage.io/docs/development/sql#sql-dialects
+        """
+        return "generic"
+
+    def get_openlineage_default_schema(self) -> str:
+        """
+        Returns default schema specific to database.
+
+        .. seealso::
+            - :class:`airflow.providers.openlineage.sqlparser.SQLParser`
+        """
+        return self.__schema or "public"
+
+    def get_openlineage_database_specific_lineage(self, task_instance) -> OperatorLineage | None:
+        """
+        Returns additional database specific lineage, e.g. query execution information.
+
+        This method is called only on completion of the task.
+
+        :param task_instance: this may be used to retrieve additional information
+            that is collected during runtime of the task
+        """
+
+    @staticmethod
+    def get_openlineage_authority_part(connection) -> str:
+        """
+        This method serves as common method for several hooks to get authority part from Airflow Connection.
+
+        The authority represents the hostname and port of the connection
+        and conforms OpenLineage naming convention for a number of databases (e.g. MySQL, Postgres, Trino).
+        """
+        parsed = urlparse(connection.get_uri())
+        authority = f"{parsed.hostname}:{parsed.port}"
+        return authority
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, NoReturn, Sequence, SupportsAbs
 
 from airflow.exceptions import AirflowException, AirflowFailException
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator, SkipMixin
 from airflow.providers.common.sql.hooks.sql import DbApiHook, fetch_all_handler, return_single_query_results
+from airflow.utils.helpers import merge_dicts
 
 if TYPE_CHECKING:
+    from airflow.providers.openlineage.extractors import OperatorLineage
     from airflow.utils.context import Context
 
 
 def _convert_to_float_if_possible(s: str) -> float | str:
     try:
         return float(s)
     except (ValueError, TypeError):
@@ -286,18 +288,76 @@
         return self._process_output(output, hook.descriptions)
 
     def prepare_template(self) -> None:
         """Parse template file for attribute parameters."""
         if isinstance(self.parameters, str):
             self.parameters = ast.literal_eval(self.parameters)
 
+    def get_openlineage_facets_on_start(self) -> OperatorLineage | None:
+        try:
+            from airflow.providers.openlineage.sqlparser import SQLParser
+        except ImportError:
+            return None
+
+        hook = self.get_db_hook()
+
+        connection = hook.get_connection(getattr(hook, hook.conn_name_attr))
+        try:
+            database_info = hook.get_openlineage_database_info(connection)
+        except AttributeError:
+            self.log.debug("%s has no database info provided", hook)
+            database_info = None
+
+        if database_info is None:
+            return None
+
+        try:
+            sql_parser = SQLParser(
+                dialect=hook.get_openlineage_database_dialect(connection),
+                default_schema=hook.get_openlineage_default_schema(),
+            )
+        except AttributeError:
+            self.log.debug("%s failed to get database dialect", hook)
+            return None
+
+        operator_lineage = sql_parser.generate_openlineage_metadata_from_sql(
+            sql=self.sql, hook=hook, database_info=database_info, database=self.database
+        )
+
+        return operator_lineage
+
+    def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage | None:
+        operator_lineage = self.get_openlineage_facets_on_start() or OperatorLineage()
+
+        try:
+            from airflow.providers.openlineage.extractors import OperatorLineage
+        except ImportError:
+            return operator_lineage
+
+        hook = self.get_db_hook()
+        try:
+            database_specific_lineage = hook.get_openlineage_database_specific_lineage(task_instance)
+        except AttributeError:
+            database_specific_lineage = None
+
+        if database_specific_lineage is None:
+            return operator_lineage
+
+        return OperatorLineage(
+            inputs=operator_lineage.inputs + database_specific_lineage.inputs,
+            outputs=operator_lineage.outputs + database_specific_lineage.outputs,
+            run_facets=merge_dicts(operator_lineage.run_facets, database_specific_lineage.run_facets),
+            job_facets=merge_dicts(operator_lineage.job_facets, database_specific_lineage.job_facets),
+        )
+
 
 class SQLColumnCheckOperator(BaseSQLOperator):
     """
     Performs one or more of the templated checks in the column_checks dictionary.
+
     Checks are performed on a per-column basis specified by the column_mapping.
 
     Each check can take one or more of the following options:
 
     * ``equal_to``: an exact value to equal, cannot be used with other comparison options
     * ``greater_than``: value that result should be strictly greater than
     * ``less_than``: value that results should be strictly less than
@@ -536,14 +596,15 @@
                 "'less than or equal to', use geq_to or leq_to."
             )
 
 
 class SQLTableCheckOperator(BaseSQLOperator):
     """
     Performs one or more of the checks provided in the checks dictionary.
+
     Checks should be written to return a boolean result.
 
     :param table: the table to run checks on
     :param checks: the dictionary of checks, where check names are followed by a dictionary containing at
         least a check statement, and optionally a partition clause, e.g.:
 
         .. code-block:: python
@@ -646,18 +707,19 @@
             )
             for check_name, value in self.checks.items()
         )
 
 
 class SQLCheckOperator(BaseSQLOperator):
     """
-    Performs checks against a db. The ``SQLCheckOperator`` expects
-    a sql query that will return a single row. Each value on that
-    first row is evaluated using python ``bool`` casting. If any of the
-    values return ``False`` the check is failed and errors out.
+    Performs checks against a db.
+
+    The ``SQLCheckOperator`` expects a sql query that will return a single row.
+    Each value on that first row is evaluated using python ``bool`` casting.
+    If any of the values return ``False`` the check is failed and errors out.
 
     Note that Python bool casting evals the following as ``False``:
 
     * ``False``
     * ``0``
     * Empty string (``""``)
     * Empty list (``[]``)
@@ -804,16 +866,15 @@
             ]
 
         return [record == numeric_pass_value_conv for record in numeric_records]
 
 
 class SQLIntervalCheckOperator(BaseSQLOperator):
     """
-    Checks that the values of metrics given as SQL expressions are within
-    a certain tolerance of the ones from days_back before.
+    Check that metrics given as SQL expressions are within tolerance of the ones from days_back before.
 
     :param table: the table name
     :param conn_id: the connection ID used to connect to the database.
     :param database: name of database which will overwrite the defined one in connection
     :param days_back: number of days between ds and the ds we want to check
         against. Defaults to 7 days
     :param date_filter_column: The column name for the dates to filter on. Defaults to 'ds'
@@ -942,17 +1003,17 @@
             self._raise_exception(f"The following tests have failed:\n {', '.join(sorted(failed_tests))}")
 
         self.log.info("All tests have passed")
 
 
 class SQLThresholdCheckOperator(BaseSQLOperator):
     """
-    Performs a value check using sql code against a minimum threshold
-    and a maximum threshold. Thresholds can be in the form of a numeric
-    value OR a sql statement that results a numeric.
+    Performs a value check using sql code against a minimum threshold and a maximum threshold.
+
+    Thresholds can be in the form of a numeric value OR a sql statement that results a numeric.
 
     :param sql: the sql to be executed. (templated)
     :param conn_id: the connection ID used to connect to the database.
     :param database: name of database which overwrite the defined one in connection
     :param min_threshold: numerical value or min threshold sql to be executed (templated)
     :param max_threshold: numerical value or max threshold sql to be executed (templated)
     """
@@ -1024,14 +1085,15 @@
             self._raise_exception(error_msg)
 
         self.log.info("Test %s Successful.", self.task_id)
 
     def push(self, meta_data):
         """
         Optional: Send data check info and metadata to an external database.
+
         Default functionality will log metadata.
         """
         info = "\n".join(f"""{key}: {item}""" for key, item in meta_data.items())
         self.log.info("Log from %s:\n%s", self.dag_id, info)
 
 
 class BranchSQLOperator(BaseSQLOperator, SkipMixin):
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.6.0rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.6.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/pyproject.toml` & `apache-airflow-providers-common-sql-1.6.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/setup.cfg` & `apache-airflow-providers-common-sql-1.6.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-common-sql-1.5.2rc1/setup.py` & `apache-airflow-providers-common-sql-1.6.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-common-sql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.5.2"
+version = "1.6.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-common-sql setup."""
     setup(
         version=version,
-        extras_require={"pandas": ["pandas>=0.17.1"]},
+        extras_require={
+            "openlineage": ["apache-airflow-providers-openlineage"],
+            "pandas": ["pandas>=0.17.1"],
+        },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.common.sql",
                 "airflow.providers.common.sql.*",
                 "airflow.providers.common.sql_vendor",
                 "airflow.providers.common.sql_vendor.*",
             ],
```

