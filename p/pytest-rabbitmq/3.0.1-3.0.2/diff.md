# Comparing `tmp/pytest-rabbitmq-3.0.1.tar.gz` & `tmp/pytest-rabbitmq-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-rabbitmq-3.0.1.tar", last modified: Fri Jun 16 09:05:44 2023, max compression
+gzip compressed data, was "pytest-rabbitmq-3.0.2.tar", last modified: Wed Jul  5 07:18:49 2023, max compression
```

## Comparing `pytest-rabbitmq-3.0.1.tar` & `pytest-rabbitmq-3.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.302409 pytest-rabbitmq-3.0.1/pytest_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:31.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:05:44.000000 pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:05:44.306409 pytest-rabbitmq-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.062020 pytest-rabbitmq-3.0.2/pytest_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:18:48.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/setup.cfg
```

### Comparing `pytest-rabbitmq-3.0.1/CHANGES.rst` & `pytest-rabbitmq-3.0.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+3.0.2 (2023-07-05)
+==================
+
+Bugfixes
+--------
+
+- Fixes logdir config option reading. (`#354 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/354>`_)
+- Fixes type hints for specifying ports in Rabbitmq startup process. (`#355 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/355>`_)
+
+
 3.0.1 (2023-06-16)
 ==================
 
 Bugfixes
 --------
 
 - Fixed rabbitmq entrypoint (`#349 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/349>`_)
```

### Comparing `pytest-rabbitmq-3.0.1/CONTRIBUTING.rst` & `pytest-rabbitmq-3.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/COPYING` & `pytest-rabbitmq-3.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/COPYING.lesser` & `pytest-rabbitmq-3.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/PKG-INFO` & `pytest-rabbitmq-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.1
+Version: 3.0.2
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-rabbitmq-3.0.1/README.rst` & `pytest-rabbitmq-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/pyproject.toml` & `pytest-rabbitmq-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-rabbitmq"
-version = "3.0.1"
+version = "3.0.2"
 description = "RabbitMQ process and client fixtures for pytest"
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "rabbitmq", "messsage queue"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -34,15 +34,15 @@
     "pika",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-rabbitmq"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_rabbitmq = "pytest_rabbitmq.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -98,15 +98,15 @@
 showcontent = true
 
 [tool.towncrier.fragment.misc]
 name = "Miscellaneus"
 showcontent = true
 
 [tool.tbump.version]
-current = "3.0.1"
+current = "3.0.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/__init__.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq. If not, see <http://www.gnu.org/licenses/>.
 """Main pytest-rabbitmq module."""
-__version__ = "3.0.1"
+__version__ = "3.0.2"
```

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/__init__.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/client.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/executor.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/executor.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/factories/process.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/process.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,31 +14,55 @@
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq.  If not, see <http://www.gnu.org/licenses/>.
 """RabbitMQ process fixture factory."""
 
 from pathlib import Path
-from typing import Any, Callable, Generator, Optional, TypedDict
+from typing import (
+    Any,
+    Callable,
+    Generator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    TypedDict,
+    Union,
+)
 from warnings import warn
 
 import pytest
 from mirakuru.exceptions import ProcessExitedWithError
 from port_for import get_port
 from pytest import FixtureRequest, TempPathFactory
 
 from pytest_rabbitmq.factories.executor import RabbitMqExecutor
 
+PortType = Union[
+    None,
+    str,
+    int,
+    Tuple[int, int],
+    Set[int],
+    List[str],
+    List[int],
+    List[Tuple[int, int]],
+    List[Set[int]],
+    List[Union[Set[int], Tuple[int, int]]],
+    List[Union[str, int, Tuple[int, int], Set[int]]],
+]
+
 
 class RabbitMQConfig(TypedDict):
     """Pytest RabbitMQ config definition type."""
 
     host: str
-    port: Optional[int]
-    distribution_port: Optional[int]
+    port: PortType
+    distribution_port: PortType
     logsdir: Optional[Path]
     server: str
     ctl: str
     node: str
     plugindir: Path
 
 
@@ -47,32 +71,33 @@
 
     def get_conf_option(option: str) -> Any:
         option_name = "rabbitmq_" + option
         return request.config.getoption(option_name) or request.config.getini(option_name)
 
     port = get_conf_option("port")
     distribution_port = get_conf_option("distribution_port")
+    logsdir = get_conf_option("logsdir")
     config: RabbitMQConfig = {
         "host": get_conf_option("host"),
         "port": int(port) if port else None,
         "distribution_port": int(distribution_port) if distribution_port else None,
-        "logsdir": Path(get_conf_option("logsdir")),
+        "logsdir": Path(logsdir) if logsdir else None,
         "server": get_conf_option("server"),
         "ctl": get_conf_option("ctl"),
         "node": get_conf_option("node"),
         "plugindir": Path(get_conf_option("plugindir")),
     }
     return config
 
 
 def rabbitmq_proc(
     server: Optional[str] = None,
     host: Optional[str] = None,
-    port: Optional[int] = -1,
-    distribution_port: Optional[int] = -1,
+    port: PortType = -1,
+    distribution_port: PortType = -1,
     node: Optional[str] = None,
     ctl: Optional[str] = None,
     logsdir: Optional[Path] = None,
     plugindir: Optional[Path] = None,
 ) -> Callable[[FixtureRequest, TempPathFactory], Generator[RabbitMqExecutor, None, None]]:
     """Fixture factory for RabbitMQ process.
```

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq/plugin.py` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/PKG-INFO` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.1
+Version: 3.0.2
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.1/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pytest-rabbitmq-3.0.1/pytest_rabbitmq.egg-info/SOURCES.txt` & `pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

