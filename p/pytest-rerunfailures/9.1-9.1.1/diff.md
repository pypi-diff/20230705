# Comparing `tmp/pytest-rerunfailures-9.1.tar.gz` & `tmp/pytest-rerunfailures-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-rerunfailures-9.1.tar", last modified: Wed Aug 26 21:07:44 2020, max compression
+gzip compressed data, was "dist/pytest-rerunfailures-9.1.1.tar", last modified: Tue Sep 29 06:28:33 2020, max compression
```

## Comparing `pytest-rerunfailures-9.1.tar` & `pytest-rerunfailures-9.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2020-08-26 21:07:44.551144 pytest-rerunfailures-9.1/
--rw-r--r--   0 sallner   (1000) users      (100)     5079 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/CHANGES.rst
--rw-r--r--   0 sallner   (1000) users      (100)     1258 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/CONTRIBUTING.rst
--rw-r--r--   0 sallner   (1000) users      (100)      193 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/LICENSE
--rw-r--r--   0 sallner   (1000) users      (100)       59 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/MANIFEST.in
--rw-r--r--   0 sallner   (1000) users      (100)    14000 2020-08-26 21:07:44.551144 pytest-rerunfailures-9.1/PKG-INFO
--rw-r--r--   0 sallner   (1000) users      (100)     4549 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/README.rst
-drwxr-xr-x   0 sallner   (1000) users      (100)        0 2020-08-26 21:07:44.551144 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/
--rw-r--r--   0 sallner   (1000) users      (100)    14000 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/PKG-INFO
--rw-r--r--   0 sallner   (1000) users      (100)      448 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/SOURCES.txt
--rw-r--r--   0 sallner   (1000) users      (100)        1 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/dependency_links.txt
--rw-r--r--   0 sallner   (1000) users      (100)       49 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/entry_points.txt
--rw-r--r--   0 sallner   (1000) users      (100)        1 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/not-zip-safe
--rw-r--r--   0 sallner   (1000) users      (100)       29 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/requires.txt
--rw-r--r--   0 sallner   (1000) users      (100)       21 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/top_level.txt
--rw-r--r--   0 sallner   (1000) users      (100)    10202 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/pytest_rerunfailures.py
--rw-r--r--   0 sallner   (1000) users      (100)      120 2020-08-26 21:07:44.551144 pytest-rerunfailures-9.1/setup.cfg
--rw-r--r--   0 sallner   (1000) users      (100)     1663 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/setup.py
--rw-r--r--   0 sallner   (1000) users      (100)    14704 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/test_pytest_rerunfailures.py
--rw-r--r--   0 sallner   (1000) users      (100)      887 2020-08-26 21:07:44.000000 pytest-rerunfailures-9.1/tox.ini
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2020-09-29 06:28:33.859913 pytest-rerunfailures-9.1.1/
+-rw-r--r--   0 sallner   (1000) users      (100)     5487 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/CHANGES.rst
+-rw-r--r--   0 sallner   (1000) users      (100)     1248 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 sallner   (1000) users      (100)      198 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/LICENSE
+-rw-r--r--   0 sallner   (1000) users      (100)       59 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/MANIFEST.in
+-rw-r--r--   0 sallner   (1000) users      (100)    14540 2020-09-29 06:28:33.859913 pytest-rerunfailures-9.1.1/PKG-INFO
+-rw-r--r--   0 sallner   (1000) users      (100)     4551 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/README.rst
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2020-09-29 06:28:33.859913 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/
+-rw-r--r--   0 sallner   (1000) users      (100)    14540 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/PKG-INFO
+-rw-r--r--   0 sallner   (1000) users      (100)      448 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/SOURCES.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        1 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/dependency_links.txt
+-rw-r--r--   0 sallner   (1000) users      (100)       49 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/entry_points.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        1 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/not-zip-safe
+-rw-r--r--   0 sallner   (1000) users      (100)       29 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/requires.txt
+-rw-r--r--   0 sallner   (1000) users      (100)       21 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/top_level.txt
+-rw-r--r--   0 sallner   (1000) users      (100)    10528 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/pytest_rerunfailures.py
+-rw-r--r--   0 sallner   (1000) users      (100)      120 2020-09-29 06:28:33.859913 pytest-rerunfailures-9.1.1/setup.cfg
+-rw-r--r--   0 sallner   (1000) users      (100)     1665 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/setup.py
+-rw-r--r--   0 sallner   (1000) users      (100)    14915 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/test_pytest_rerunfailures.py
+-rw-r--r--   0 sallner   (1000) users      (100)      948 2020-09-29 06:28:33.000000 pytest-rerunfailures-9.1.1/tox.ini
```

### Comparing `pytest-rerunfailures-9.1/CHANGES.rst` & `pytest-rerunfailures-9.1.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Changelog
 =========
 
+9.1.1 (2020-09-29)
+------------------
+
+Compatibility fix.
+++++++++++++++++++
+
+- Ignore ``--result-log`` command line option when used together with ``pytest
+  >= 6.1.0``, as it was removed there. This is a quick fix, use an older
+  version of pytest, if you want to keep this feature for now.
+  (Thanks to `@ntessore`_ for the PR)
+
+- Support up to pytest 6.1.0.
+
+.. _@ntessore: https://github.com/ntessore
+
+
 9.1 (2020-08-26)
 ----------------
 
 Features
 ++++++++
 
 - Add a new flag ``--only-rerun`` to allow for users to rerun only certain
```

### Comparing `pytest-rerunfailures-9.1/CONTRIBUTING.rst` & `pytest-rerunfailures-9.1.1/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,18 @@
    Afterwards ``pre-commit`` will run whenever you commit.
 
    Note that this is automatically done when running ``tox -e linting``.
 
    https://pre-commit.com/ is a framework for managing and maintaining multi-language pre-commit hooks
    to ensure code-style and code formatting is consistent.
 
-#. Install `tox <https://tox.readthedocs.io/en/latest/>`_::
+#. Install `tox <https://tox.readthedocs.io/en/latest/>`_:
 
    Tox is used to run all the tests and will automatically setup virtualenvs
-   to run the tests in. Implicitly http://www.virtualenv.org/en/latest/ is used::
+   to run the tests in. Implicitly https://virtualenv.pypa.io/ is used::
 
     $ pip install tox
     $ tox -e linting,py37
 
 #. Follow **PEP-8** for naming and `black <https://github.com/psf/black>`_ for formatting.
 
 #. Add a line item to the current **unreleased** version in ``CHANGES.rst``, unless the change is trivial.
```

### Comparing `pytest-rerunfailures-9.1/PKG-INFO` & `pytest-rerunfailures-9.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: pytest-rerunfailures
-Version: 9.1
+Version: 9.1.1
 Summary: pytest plugin to re-run tests to eliminate flaky failures
 Home-page: https://github.com/pytest-dev/pytest-rerunfailures
 Author: Leah Klearman
 Author-email: lklrmn@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: .. contents::
         
         pytest-rerunfailures
         ====================
         
-        pytest-rerunfailures is a plugin for `py.test <http://pytest.org>`_ that
+        pytest-rerunfailures is a plugin for `pytest <https://pytest.org>`_ that
         re-runs tests to eliminate intermittent failures.
         
         .. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg
            :target: https://github.com/pytest-dev/pytest-rerunfailures/blob/master/LICENSE
            :alt: License
         .. image:: https://img.shields.io/pypi/v/pytest-rerunfailures.svg
            :target: https://pypi.python.org/pypi/pytest-rerunfailures/
@@ -141,16 +141,16 @@
         * This plugin may *not* be used with class, module, and package level fixtures.
         * This plugin is *not* compatible with pytest-xdist's --looponfail flag.
         * This plugin is *not* compatible with the core --pdb flag.
         
         Resources
         ---------
         
-        - `Issue Tracker <http://github.com/pytest-dev/pytest-rerunfailures/issues>`_
-        - `Code <http://github.com/pytest-dev/pytest-rerunfailures/>`_
+        - `Issue Tracker <https://github.com/pytest-dev/pytest-rerunfailures/issues>`_
+        - `Code <https://github.com/pytest-dev/pytest-rerunfailures/>`_
         
         Development
         -----------
         
         * Test execution count can be retrieved from the ``execution_count`` attribute in test ``item``'s object. Example:
         
           .. code-block:: python
@@ -159,14 +159,30 @@
             def pytest_runtest_makereport(item, call):
                 print(item.execution_count)
         
         
         Changelog
         =========
         
+        9.1.1 (2020-09-29)
+        ------------------
+        
+        Compatibility fix.
+        ++++++++++++++++++
+        
+        - Ignore ``--result-log`` command line option when used together with ``pytest
+          >= 6.1.0``, as it was removed there. This is a quick fix, use an older
+          version of pytest, if you want to keep this feature for now.
+          (Thanks to `@ntessore`_ for the PR)
+        
+        - Support up to pytest 6.1.0.
+        
+        .. _@ntessore: https://github.com/ntessore
+        
+        
         9.1 (2020-08-26)
         ----------------
         
         Features
         ++++++++
         
         - Add a new flag ``--only-rerun`` to allow for users to rerun only certain
```

### Comparing `pytest-rerunfailures-9.1/README.rst` & `pytest-rerunfailures-9.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pytest-rerunfailures
 ====================
 
-pytest-rerunfailures is a plugin for `py.test <http://pytest.org>`_ that
+pytest-rerunfailures is a plugin for `pytest <https://pytest.org>`_ that
 re-runs tests to eliminate intermittent failures.
 
 .. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg
    :target: https://github.com/pytest-dev/pytest-rerunfailures/blob/master/LICENSE
    :alt: License
 .. image:: https://img.shields.io/pypi/v/pytest-rerunfailures.svg
    :target: https://pypi.python.org/pypi/pytest-rerunfailures/
@@ -131,16 +131,16 @@
 * This plugin may *not* be used with class, module, and package level fixtures.
 * This plugin is *not* compatible with pytest-xdist's --looponfail flag.
 * This plugin is *not* compatible with the core --pdb flag.
 
 Resources
 ---------
 
-- `Issue Tracker <http://github.com/pytest-dev/pytest-rerunfailures/issues>`_
-- `Code <http://github.com/pytest-dev/pytest-rerunfailures/>`_
+- `Issue Tracker <https://github.com/pytest-dev/pytest-rerunfailures/issues>`_
+- `Code <https://github.com/pytest-dev/pytest-rerunfailures/>`_
 
 Development
 -----------
 
 * Test execution count can be retrieved from the ``execution_count`` attribute in test ``item``'s object. Example:
 
   .. code-block:: python
```

### Comparing `pytest-rerunfailures-9.1/pytest_rerunfailures.egg-info/PKG-INFO` & `pytest-rerunfailures-9.1.1/pytest_rerunfailures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: pytest-rerunfailures
-Version: 9.1
+Version: 9.1.1
 Summary: pytest plugin to re-run tests to eliminate flaky failures
 Home-page: https://github.com/pytest-dev/pytest-rerunfailures
 Author: Leah Klearman
 Author-email: lklrmn@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: .. contents::
         
         pytest-rerunfailures
         ====================
         
-        pytest-rerunfailures is a plugin for `py.test <http://pytest.org>`_ that
+        pytest-rerunfailures is a plugin for `pytest <https://pytest.org>`_ that
         re-runs tests to eliminate intermittent failures.
         
         .. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg
            :target: https://github.com/pytest-dev/pytest-rerunfailures/blob/master/LICENSE
            :alt: License
         .. image:: https://img.shields.io/pypi/v/pytest-rerunfailures.svg
            :target: https://pypi.python.org/pypi/pytest-rerunfailures/
@@ -141,16 +141,16 @@
         * This plugin may *not* be used with class, module, and package level fixtures.
         * This plugin is *not* compatible with pytest-xdist's --looponfail flag.
         * This plugin is *not* compatible with the core --pdb flag.
         
         Resources
         ---------
         
-        - `Issue Tracker <http://github.com/pytest-dev/pytest-rerunfailures/issues>`_
-        - `Code <http://github.com/pytest-dev/pytest-rerunfailures/>`_
+        - `Issue Tracker <https://github.com/pytest-dev/pytest-rerunfailures/issues>`_
+        - `Code <https://github.com/pytest-dev/pytest-rerunfailures/>`_
         
         Development
         -----------
         
         * Test execution count can be retrieved from the ``execution_count`` attribute in test ``item``'s object. Example:
         
           .. code-block:: python
@@ -159,14 +159,30 @@
             def pytest_runtest_makereport(item, call):
                 print(item.execution_count)
         
         
         Changelog
         =========
         
+        9.1.1 (2020-09-29)
+        ------------------
+        
+        Compatibility fix.
+        ++++++++++++++++++
+        
+        - Ignore ``--result-log`` command line option when used together with ``pytest
+          >= 6.1.0``, as it was removed there. This is a quick fix, use an older
+          version of pytest, if you want to keep this feature for now.
+          (Thanks to `@ntessore`_ for the PR)
+        
+        - Support up to pytest 6.1.0.
+        
+        .. _@ntessore: https://github.com/ntessore
+        
+        
         9.1 (2020-08-26)
         ----------------
         
         Features
         ++++++++
         
         - Add a new flag ``--only-rerun`` to allow for users to rerun only certain
```

### Comparing `pytest-rerunfailures-9.1/pytest_rerunfailures.py` & `pytest-rerunfailures-9.1.1/pytest_rerunfailures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import re
 import time
 import warnings
 
 import pkg_resources
 import pytest
-from _pytest.resultlog import ResultLog
 from _pytest.runner import runtestprotocol
 
 PYTEST_GTE_54 = pkg_resources.parse_version(
     pytest.__version__
 ) >= pkg_resources.parse_version("5.4")
 
+PYTEST_GTE_61 = pkg_resources.parse_version(
+    pytest.__version__
+) >= pkg_resources.parse_version("6.1")
+
 
 def works_with_current_xdist():
     """Returns compatibility with installed pytest-xdist version.
 
     When running tests in parallel using pytest-xdist < 1.20.0, the first
     report that is logged will finish and terminate the current node rather
     rerunning the test. Thus we must skip logging of intermediate results under
@@ -68,35 +71,39 @@
         "flaky(reruns=1, reruns_delay=0): mark test to re-run up "
         "to 'reruns' times. Add a delay of 'reruns_delay' seconds "
         "between re-runs.",
     )
 
 
 def _get_resultlog(config):
-    if PYTEST_GTE_54:
+    if PYTEST_GTE_61:
+        return None
+    elif PYTEST_GTE_54:
         # hack
         from _pytest.resultlog import resultlog_key
 
         return config._store.get(resultlog_key, default=None)
     else:
         return getattr(config, "_resultlog", None)
 
 
 def _set_resultlog(config, resultlog):
-    if PYTEST_GTE_54:
+    if PYTEST_GTE_61:
+        pass
+    elif PYTEST_GTE_54:
         # hack
         from _pytest.resultlog import resultlog_key
 
         config._store[resultlog_key] = resultlog
     else:
         config._resultlog = resultlog
 
 
 # making sure the options make sense
-# should run before / at the begining of pytest_cmdline_main
+# should run before / at the beginning of pytest_cmdline_main
 def check_options(config):
     val = config.getvalue
     if not val("collectonly"):
         if config.option.reruns != 0:
             if config.option.usepdb:  # a core option
                 raise pytest.UsageError("--reruns incompatible with --pdb")
 
@@ -295,36 +302,39 @@
     rerun = terminalreporter.stats.get("rerun")
     if rerun:
         for rep in rerun:
             pos = rep.nodeid
             lines.append("RERUN {}".format(pos))
 
 
-class RerunResultLog(ResultLog):
-    def __init__(self, config, logfile):
-        ResultLog.__init__(self, config, logfile)
-
-    def pytest_runtest_logreport(self, report):
-        """
-        Adds support for rerun report fix for issue:
-        https://github.com/pytest-dev/pytest-rerunfailures/issues/28
-        """
-        if report.when != "call" and report.passed:
-            return
-        res = self.config.hook.pytest_report_teststatus(report=report)
-        code = res[1]
-        if code == "x":
-            longrepr = str(report.longrepr)
-        elif code == "X":
-            longrepr = ""
-        elif report.passed:
-            longrepr = ""
-        elif report.failed:
-            longrepr = str(report.longrepr)
-        elif report.skipped:
-            longrepr = str(report.longrepr[2])
-        elif report.outcome == "rerun":
-            longrepr = str(report.longrepr)
-        else:
-            longrepr = str(report.longrepr)
+if not PYTEST_GTE_61:
+    from _pytest.resultlog import ResultLog
+
+    class RerunResultLog(ResultLog):
+        def __init__(self, config, logfile):
+            ResultLog.__init__(self, config, logfile)
+
+        def pytest_runtest_logreport(self, report):
+            """
+            Adds support for rerun report fix for issue:
+            https://github.com/pytest-dev/pytest-rerunfailures/issues/28
+            """
+            if report.when != "call" and report.passed:
+                return
+            res = self.config.hook.pytest_report_teststatus(report=report)
+            code = res[1]
+            if code == "x":
+                longrepr = str(report.longrepr)
+            elif code == "X":
+                longrepr = ""
+            elif report.passed:
+                longrepr = ""
+            elif report.failed:
+                longrepr = str(report.longrepr)
+            elif report.skipped:
+                longrepr = str(report.longrepr[2])
+            elif report.outcome == "rerun":
+                longrepr = str(report.longrepr)
+            else:
+                longrepr = str(report.longrepr)
 
-        self.log_outcome(report, code, longrepr)
+            self.log_outcome(report, code, longrepr)
```

### Comparing `pytest-rerunfailures-9.1/setup.py` & `pytest-rerunfailures-9.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.rst") as readme, open("CHANGES.rst") as changelog:
     long_description = ".. contents::\n\n" + readme.read() + "\n\n" + changelog.read()
 
 setup(
     name="pytest-rerunfailures",
-    version="9.1",
+    version="9.1.1",
     description="pytest plugin to re-run tests to eliminate flaky failures",
     long_description=long_description,
     author="Leah Klearman",
     author_email="lklrmn@gmail.com",
     url="https://github.com/pytest-dev/pytest-rerunfailures",
     py_modules=["pytest_rerunfailures"],
     entry_points={"pytest11": ["rerunfailures = pytest_rerunfailures"]},
```

### Comparing `pytest-rerunfailures-9.1/test_pytest_rerunfailures.py` & `pytest-rerunfailures-9.1.1/test_pytest_rerunfailures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import random
 import time
 from unittest import mock
 
+import pkg_resources
 import pytest
 
 
 pytest_plugins = "pytester"
 
+PYTEST_GTE_61 = pkg_resources.parse_version(
+    pytest.__version__
+) >= pkg_resources.parse_version("6.1")
+
 
 def temporary_failure(count=1):
     return """
             import py
             path = py.path.local(__file__).dirpath().ensure('test.res')
             count = path.read() or 1
             if int(count) <= {0}:
@@ -274,14 +279,15 @@
             def test_pass():
                 pass"""
     )
     result = testdir.runpytest("--reruns", "1")
     assert_outcomes(result, passed=0, error=1, rerun=1)
 
 
+@pytest.mark.skipif(PYTEST_GTE_61, reason="--result-log removed in pytest>=6.1")
 def test_rerun_with_resultslog(testdir):
     testdir.makepyfile(
         """
         def test_fail():
             assert False"""
     )
```

### Comparing `pytest-rerunfailures-9.1/tox.ini` & `pytest-rerunfailures-9.1.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Tox (https://tox.readthedocs.io/en/latest/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
-# test suite on all supported python versions. To use it, "pip install tox"
+# test suite on all supported Python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [flake8]
 # NOTE: This is kept in line with Black
 #       See: https://black.readthedocs.io/en/stable/the_black_code_style.html#line-length
 max-line-length = 88
 
 [tox]
 envlist =
     linting
-    py{35,36,37,38,py3}-pytest{50,51,52,53,54}
+    py{35,36,37,38,py3}-pytest{50,51,52,53,54,60,61}
 minversion = 3.17.1
 
 [testenv]
-commands = py.test test_pytest_rerunfailures.py {posargs}
+commands = pytest test_pytest_rerunfailures.py {posargs}
 deps =
     pytest50: pytest==5.0.*
     pytest51: pytest==5.1.*
     pytest52: pytest==5.2.*
     pytest53: pytest==5.3.*
     pytest54: pytest==5.4.*
+    pytest60: pytest==6.0.*
+    pytest61: pytest==6.1.*
 
 [testenv:linting]
 basepython = python3
 commands = pre-commit run --all-files --show-diff-on-failure {posargs:}
 deps = pre-commit>=1.11.0
 skip_install = True
```

