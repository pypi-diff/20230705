# Comparing `tmp/astro_run_dag-0.2.5.tar.gz` & `tmp/astro_run_dag-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_run_dag-0.2.5.tar", max compression
+gzip compressed data, was "astro_run_dag-0.2.6.tar", max compression
```

## Comparing `astro_run_dag-0.2.5.tar` & `astro_run_dag-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       29 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/README.md
--rw-r--r--   0        0        0     1989 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      137 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/__init__.py
--rw-r--r--   0        0        0     3249 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/__main__.py
--rw-r--r--   0        0        0        0 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/utils/__init__.py
--rw-r--r--   0        0        0      244 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/utils/exceptions.py
--rw-r--r--   0        0        0     3149 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/utils/get_dag.py
--rw-r--r--   0        0        0     1814 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/utils/parse_settings_file.py
--rw-r--r--   0        0        0     8199 2022-11-21 22:43:18.733744 astro_run_dag-0.2.5/run_dag/utils/run_dag.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 astro_run_dag-0.2.5/setup.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 astro_run_dag-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/README.md
+-rw-r--r--   0        0        0     2672 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/__init__.py
+-rw-r--r--   0        0        0     3412 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/utils/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/utils/exceptions.py
+-rw-r--r--   0        0        0     3149 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/utils/get_dag.py
+-rw-r--r--   0        0        0     1780 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/utils/parse_settings_file.py
+-rw-r--r--   0        0        0     8572 2023-07-05 21:13:25.687349 astro_run_dag-0.2.6/run_dag/utils/run_dag.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 astro_run_dag-0.2.6/PKG-INFO
```

### Comparing `astro_run_dag-0.2.5/pyproject.toml` & `astro_run_dag-0.2.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astro-run-dag"
-version = "0.2.5"
+version = "0.2.6"
 description = "Run Airflow DAGs with just python"
 authors = [
     "Astronomer <humans@astronomer.io>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["python", "transform", "analyst", "DAG", "airflow", "astronomer"]
@@ -16,55 +16,83 @@
     "Framework :: Apache Airflow",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 include=[
    { path = 'include', format = 'wheel' }
 ]
-
-[project.urls]
-Home = "https://astronomer.io/"
-Source = "https://github.com/astronomer/astro-sdk/sql-cli"
+homepage = "https://astronomer.io/"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = "^3.7"
 typer = {extras = ["all"], version = "^0.6.1"}
 apache-airflow = ">2.0"
 python-dotenv = "^0.21.0"
-astro-sdk-python = {version = "^1.2.2"}
 
 [tool.poetry.scripts]
 run_dag = "run_dag.__main__:app"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
+astro-sdk-python = {version = "^1.6.1", python = ">=3.7.1,<3.11"}
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 mypy = "^0.982"
 types-pyyaml = ">5.4.1"
+pydantic = "<2.0"
 
 [tool.poetry.group.type_check]
 optional = true
 
 [tool.poetry.group.type_check.dependencies]
 mypy = "^0.982"
 types-pyyaml = ">5.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-src_paths = ["run_dag", "tests"]
+[tool.black]
+line-length = 110
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+
+[tool.ruff]
+line-length = 110
+# Enable Pyflakes `E` and `F` codes by default.
+extend-select = [
+    "W",    # pycodestyle warnings
+    "I",    # isort
+    "C90",  # Complexity
+#    "B",    # flake8-bugbear
+    "C4",    # flake8-comprehensions
+#    "ANN",  # flake8-annotations
+    "ISC",  # flake8-implicit-str-concat
+    "T10",  # flake8-debugger
+    "A",    # flake8-builtins
+    "UP",   # pyupgrade
+]
+
+# Remove this in future
+extend-ignore = ["A002", "C901", "E402", "E501", "ISC001", "ISC003", "UP030"]
+
+target-version = "py37"
+fix = true
+
+[tool.ruff.mccabe]
+max-complexity = 6
+
+[tool.ruff.isort]
+combine-as-imports = true
 
 [tool.mypy]
 color_output = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 files = ["run_dag"]
```

### Comparing `astro_run_dag-0.2.5/run_dag/__main__.py` & `astro_run_dag-0.2.6/run_dag/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# This is a sample Python script.
-
-# Press ⌃R to execute it or replace it with your code.
-# Press Double ⇧ to search everywhere for classes, files, tool windows, actions, and settings.
 import logging
 import warnings
+from datetime import datetime
 
 import typer
 from airflow.models.dagbag import DagBag
 from airflow.utils.cli import process_subdir
 from dotenv import load_dotenv
 from rich import print as rprint
 from typer import Exit
@@ -15,17 +12,15 @@
 from run_dag.utils.exceptions import ConnectionFailed
 from run_dag.utils.get_dag import get_dag
 from run_dag.utils.parse_settings_file import parse_settings_file
 from run_dag.utils.run_dag import run_dag
 
 warnings.filterwarnings(action="ignore")
 load_dotenv()
-app = typer.Typer(
-    add_completion=False, context_settings={"help_option_names": ["-h", "--help"]}
-)
+app = typer.Typer(add_completion=False, context_settings={"help_option_names": ["-h", "--help"]})
 
 
 airflow_logger = logging.getLogger("airflow")
 airflow_logger.setLevel(logging.CRITICAL)
 airflow_logger.propagate = False
 
 
@@ -57,34 +52,42 @@
         help="path to a file containing a list of connection objects",
     ),
     variables_file_path: str = typer.Argument(
         default=None,
         show_default=False,
         help="path to a file containing a list of variable objects",
     ),
+    execution_date: datetime = typer.Option(
+        default=None,
+        show_default=False,
+        help="execution date for the dagrun. Defaults to now",
+    ),
+    verbose: bool = typer.Option(
+        default=False,
+        help="print out the logs of the dag run",
+    ),
 ) -> None:
-
     import_errors = DagBag(process_subdir(str(dag_file))).import_errors
     if import_errors:
         all_errors = "\n\n".join(list(import_errors.values()))
-        rprint(
-            f"[bold red]DAG failed to render[/bold red]\n errors found:\n\n {all_errors}"
-        )
+        rprint(f"[bold red]DAG failed to render[/bold red]\n errors found:\n\n {all_errors}")
         raise Exit(code=1)
     dag = get_dag(dag_id=dag_id, subdir=dag_file, include_examples=False)
     connections, variables = None, None
     if settings_file_path:
         connections, variables = parse_settings_file(settings_file_path)
     try:
         dr = run_dag(
             dag,
+            execution_date=execution_date,
             conn_file_path=connections_file_path,
             variable_file_path=variables_file_path,
             connections=connections,
             variables=variables,
+            verbose=verbose,
         )
     except ConnectionFailed as connection_failed:
         rprint(
             f"  [bold red]{connection_failed}[/bold red] using connection [bold]{connection_failed.conn_id}[/bold]"
         )
         raise Exit(code=1)
     except Exception as exception:
```

### Comparing `astro_run_dag-0.2.5/run_dag/utils/get_dag.py` & `astro_run_dag-0.2.6/run_dag/utils/get_dag.py`

 * *Files identical despite different names*

### Comparing `astro_run_dag-0.2.5/run_dag/utils/parse_settings_file.py` & `astro_run_dag-0.2.6/run_dag/utils/parse_settings_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 from airflow.models.variable import Variable
 
 
 def _get_connections(yaml_dict: Dict[str, Any]) -> Dict[str, Connection]:
     connections = {}
     for i in yaml_dict["connections"]:
         parsed_yaml_dict = {
-            (k.replace("conn_", "") if k not in ["conn_id", "conn_type"] else k): v
-            for k, v in i.items()
+            (k.replace("conn_", "") if k not in ["conn_id", "conn_type"] else k): v for k, v in i.items()
         }
         connections[parsed_yaml_dict["conn_id"]] = Connection(**parsed_yaml_dict)
     return connections
 
 
 def _get_variables(yaml_dict: Dict[str, Any]) -> Dict[str, Variable]:
     variables = {}
     for i in yaml_dict["variables"]:
-        variables[i["variable_name"]] = Variable(
-            key=i["variable_name"], val=i["variable_value"]
-        )
+        variables[i["variable_name"]] = Variable(key=i["variable_name"], val=i["variable_value"])
     return variables
 
 
 def parse_settings_file(
     file_path: str,
 ) -> Tuple[Dict[str, Connection], Dict[str, Variable]]:
     """
```

### Comparing `astro_run_dag-0.2.5/run_dag/utils/run_dag.py` & `astro_run_dag-0.2.6/run_dag/utils/run_dag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-import sys
+import typing
 import warnings
 from datetime import datetime
 from typing import Any
 
 from airflow.models.connection import Connection
 from airflow.models.dag import DAG
 from airflow.models.dagrun import DagRun
@@ -13,18 +13,19 @@
 from airflow.models.variable import Variable
 from airflow.secrets.local_filesystem import LocalFilesystemBackend
 from airflow.utils import timezone
 from airflow.utils.session import NEW_SESSION, provide_session
 from airflow.utils.state import DagRunState, State
 from airflow.utils.types import DagRunType
 from rich import print as pprint
+from rich.console import Console
+from rich.logging import RichHandler
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm.session import Session
 
-from astro.sql.operators.cleanup import AstroCleanupException
 from run_dag.utils.exceptions import ConnectionFailed
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 
 
 class AstroFilesystemBackend(LocalFilesystemBackend):
@@ -72,21 +73,23 @@
 
     :param dag: The Airflow DAG we will run
     :param execution_date: execution date for the DAG run
     :param run_conf: configuration to pass to newly created dagrun
     :param conn_file_path: file path to a connection file in either yaml or json
     :param variable_file_path: file path to a variable file in either yaml or json
     :param session: database connection (optional)
+    :param verbose: whether to print out the logs of the tasks
 
     :return: the dag run object
     """
-    execution_date = execution_date or timezone.utcnow()
-    dag.log.debug(
-        "Clearing existing task instances for execution date %s", execution_date
-    )
+    execution_date = timezone.coerce_datetime(execution_date) or timezone.utcnow()
+    execution_date = typing.cast(datetime, execution_date)
+    dag.log.debug("Clearing existing task instances for execution date %s", execution_date)
+    if execution_date < dag.start_date:
+        raise ValueError(f"Execution date {execution_date} is before dag start date {dag.start_date}")
     dag.clear(
         start_date=execution_date,
         end_date=execution_date,
         dag_run_state=False,  # type: ignore
         session=session,
     )
     dag.log.debug("Getting dagrun for dag %s", dag.dag_id)
@@ -118,42 +121,39 @@
     # than creating a BackfillJob and allows us to surface logs to the user
     while dr.state == State.RUNNING:
         schedulable_tis, _ = dr.update_state(session=session)
         for ti in schedulable_tis:
             if verbose:
                 add_logger_if_needed(dag, ti)
             ti.task = tasks[ti.task_id]
-            _run_task(ti, session=session)
+            _run_task(ti, session=session, verbose=verbose)
     if conn_file_path or variable_file_path or connections:
         # Remove the local variables we have added to the secrets_backend_list
         secrets_backend_list.pop(0)  # noqa
     return dr
 
 
 def add_logger_if_needed(dag: DAG, ti: TaskInstance) -> None:
     """
     Add a formatted logger to the taskinstance so all logs are surfaced to the command line instead
     of into a task file. Since this is a local test run, it is much better for the user to see logs
     in the command line, rather than needing to search for a log file.
 
     :param ti: The taskinstance that will receive a logger
     """
-    logging_format = logging.Formatter(
-        "[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s"
-    )
-    handler = logging.StreamHandler(sys.stdout)
+    handler = RichHandler()
     handler.level = logging.DEBUG
-    handler.setFormatter(logging_format)
+
     # only add log handler once
-    if not any(isinstance(h, logging.StreamHandler) for h in ti.log.handlers):
-        dag.log.debug("Adding Streamhandler to taskinstance %s", ti.task_id)
+    if not any(isinstance(h, RichHandler) for h in ti.log.handlers):
+        dag.log.debug("Adding RichHandler to taskinstance %s", ti.task_id)
         ti.log.addHandler(handler)
 
 
-def _run_task(ti: TaskInstance, session: Session) -> None:
+def _run_task(ti: TaskInstance, session: Session, verbose: bool = False) -> None:
     """
     Run a single task instance, and push result to Xcom for downstream tasks. Bypasses a lot of
     extra steps used in `task.run` to keep our local running as fast as possible
     This function is only meant for the `dag.test` function as a helper function.
 
     :param ti: TaskInstance to run
     """
@@ -161,31 +161,39 @@
         pprint(
             f"Running task [bold yellow]{ti.task_id}[/bold yellow][{ti.map_index}]...",
             end=" ",
         )
     else:
         pprint(f"Running [bold yellow]{ti.task_id}[/bold yellow]...", end=" ")
 
+    console = Console()
+    if verbose:
+        pprint()
+        console.rule("[bold red]🧾 Task Logs")
+
     try:
         warnings.filterwarnings(action="ignore")
         ti._run_raw_task(session=session)  # skipcq: PYL-W0212
         session.flush()
         session.commit()
-        pprint("[bold green]SUCCESS[/bold green]")
+        if verbose:
+            console.rule()
+        pprint("[bold green]SUCCESS[/bold green] ✅")
     except OperationalError as operational_exception:
         pprint("[bold red]FAILED[/bold red]")
         orig_exception = operational_exception.orig
         orig_message = orig_exception.args[0]
-        raise ConnectionFailed(
-            orig_message, conn_id=ti.task.conn_id
-        ) from orig_exception
-    except AstroCleanupException:
-        pprint("aql.cleanup async, continuing")
-    except Exception:
-        pprint("[bold red]FAILED[/bold red]")
+        raise ConnectionFailed(orig_message, conn_id=ti.task.conn_id) from orig_exception
+    except Exception as e:
+        if e.__class__.__name__ == "AstroCleanupException":
+            pprint("aql.cleanup async, continuing")
+            return
+        if verbose:
+            console.rule()
+        pprint("[bold red]FAILED[/bold red] ❌")
         raise
 
 
 def _get_or_create_dagrun(
     dag: DAG,
     conf: dict[Any, Any] | None,
     start_date: datetime,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

