# Comparing `tmp/common-pyutil-0.8.6.tar.gz` & `tmp/common-pyutil-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-pyutil-0.8.6.tar", max compression
+gzip compressed data, was "common-pyutil-0.8.7.tar", max compression
```

## Comparing `common-pyutil-0.8.6.tar` & `common-pyutil-0.8.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2021-10-31 18:50:10.780585 common-pyutil-0.8.6/LICENSE.md
--rw-r--r--   0        0        0      563 2021-11-12 13:24:48.487758 common-pyutil-0.8.6/README.md
--rw-r--r--   0        0        0       22 2023-04-17 02:55:22.633110 common-pyutil-0.8.6/common_pyutil/__init__.py
--rw-r--r--   0        0        0      219 2021-11-12 13:24:48.488758 common-pyutil-0.8.6/common_pyutil/contexts.py
--rw-r--r--   0        0        0     2086 2021-10-31 18:50:06.586667 common-pyutil-0.8.6/common_pyutil/decorators.py
--rw-r--r--   0        0        0    15900 2023-04-14 10:37:51.995391 common-pyutil-0.8.6/common_pyutil/functional.py
--rw-r--r--   0        0        0      860 2021-10-31 18:50:06.596667 common-pyutil-0.8.6/common_pyutil/io.py
--rw-r--r--   0        0        0     6816 2021-10-31 18:50:06.577667 common-pyutil-0.8.6/common_pyutil/log.py
--rw-r--r--   0        0        0     1543 2022-11-26 16:51:57.704616 common-pyutil-0.8.6/common_pyutil/monitor.py
--rw-r--r--   0        0        0     6165 2022-06-09 20:05:34.150703 common-pyutil-0.8.6/common_pyutil/net.py
--rw-r--r--   0        0        0     1686 2023-01-11 14:33:05.379827 common-pyutil-0.8.6/common_pyutil/proc.py
--rw-r--r--   0        0        0        0 2021-10-31 18:50:05.672685 common-pyutil-0.8.6/common_pyutil/py.typed
--rw-r--r--   0        0        0     2592 2021-11-12 13:24:48.490758 common-pyutil-0.8.6/common_pyutil/structures.py
--rw-r--r--   0        0        0     8552 2023-04-13 00:12:02.441705 common-pyutil-0.8.6/common_pyutil/system.py
--rw-r--r--   0        0        0     1476 2022-02-06 10:37:09.214421 common-pyutil-0.8.6/common_pyutil/venv.py
--rw-r--r--   0        0        0     1109 2023-04-17 02:55:22.511112 common-pyutil-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     1370 2023-04-17 02:56:46.788309 common-pyutil-0.8.6/setup.py
--rw-r--r--   0        0        0     1662 2023-04-17 02:56:46.788537 common-pyutil-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2021-10-31 18:50:10.780585 common-pyutil-0.8.7/LICENSE.md
+-rw-r--r--   0        0        0      563 2021-11-12 13:24:48.487758 common-pyutil-0.8.7/README.md
+-rw-r--r--   0        0        0       22 2023-07-05 08:28:50.041365 common-pyutil-0.8.7/common_pyutil/__init__.py
+-rw-r--r--   0        0        0      219 2021-11-12 13:24:48.488758 common-pyutil-0.8.7/common_pyutil/contexts.py
+-rw-r--r--   0        0        0     2086 2021-10-31 18:50:06.586667 common-pyutil-0.8.7/common_pyutil/decorators.py
+-rw-r--r--   0        0        0    15900 2023-04-14 10:37:51.995391 common-pyutil-0.8.7/common_pyutil/functional.py
+-rw-r--r--   0        0        0      860 2021-10-31 18:50:06.596667 common-pyutil-0.8.7/common_pyutil/io.py
+-rw-r--r--   0        0        0     6812 2023-05-21 15:55:02.884820 common-pyutil-0.8.7/common_pyutil/log.py
+-rw-r--r--   0        0        0     1759 2023-05-15 03:40:21.789897 common-pyutil-0.8.7/common_pyutil/monitor.py
+-rw-r--r--   0        0        0     6165 2022-06-09 20:05:34.150703 common-pyutil-0.8.7/common_pyutil/net.py
+-rw-r--r--   0        0        0     1686 2023-01-11 14:33:05.379827 common-pyutil-0.8.7/common_pyutil/proc.py
+-rw-r--r--   0        0        0        0 2021-10-31 18:50:05.672685 common-pyutil-0.8.7/common_pyutil/py.typed
+-rw-r--r--   0        0        0     2592 2021-11-12 13:24:48.490758 common-pyutil-0.8.7/common_pyutil/structures.py
+-rw-r--r--   0        0        0     8552 2023-04-13 00:12:02.441705 common-pyutil-0.8.7/common_pyutil/system.py
+-rw-r--r--   0        0        0     1476 2022-02-06 10:37:09.214421 common-pyutil-0.8.7/common_pyutil/venv.py
+-rw-r--r--   0        0        0     1109 2023-07-05 08:28:49.917367 common-pyutil-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     1370 2023-07-05 08:29:50.472004 common-pyutil-0.8.7/setup.py
+-rw-r--r--   0        0        0     1662 2023-07-05 08:29:50.472232 common-pyutil-0.8.7/PKG-INFO
```

### Comparing `common-pyutil-0.8.6/LICENSE.md` & `common-pyutil-0.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/README.md` & `common-pyutil-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/decorators.py` & `common-pyutil-0.8.7/common_pyutil/decorators.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/functional.py` & `common-pyutil-0.8.7/common_pyutil/functional.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/io.py` & `common-pyutil-0.8.7/common_pyutil/io.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/log.py` & `common-pyutil-0.8.7/common_pyutil/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,16 @@
         fmt: Logger format
         no_file_logger: Don't create a file logger
         no_stream_logger: Don't create a stream logger
 
     Returns:
         A tuple of filename and the logger instance
     """
-    if not datefmt:
-        datefmt = '%Y/%m/%d %I:%M:%S %p'
-    if not fmt:
-        '%(asctime)s %(message)s'
+    datefmt = datefmt or '%Y/%m/%d %I:%M:%S %p'
+    fmt = fmt or '[%(levelname)s] %(asctime)s %(message)s'
     logger = logging.getLogger(logger_name)
     formatter = logging.Formatter(datefmt=datefmt, fmt=fmt)
     if not no_file_logger and logdir and log_file_name:
         if not os.path.exists(logdir):
             os.mkdir(logdir)
         if not log_file_name.endswith('.log'):
             log_file_name += '.log'
```

### Comparing `common-pyutil-0.8.6/common_pyutil/monitor.py` & `common-pyutil-0.8.7/common_pyutil/monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,42 @@
 
         with timer:             # doesn't reset
             do_something_else
 
         print(timer.time)
         timer.clear()           # now reset
     """
-    def __init__(self, accumulate=False):
-        self._accumulate = accumulate
+    def __init__(self, accumulate: bool = False):
+        self._accumulate: bool = accumulate
         self._time = 0
 
     def __enter__(self):
         self._start = time.time()
 
     def __exit__(self, *args):
+        self._last = time.time() - self._start
         if self.accumulate:
-            self._time += time.time() - self._start
+            self._time += self._last
         else:
-            self._time = time.time() - self._start
+            self._time = self._last
 
     def clear(self):
         "Clear the timer instance"
         self._time = 0
 
     @property
+    def last(self) -> float:
+        """Return the last measured time
+
+        Same as :attr:`time` if :attr:`accumulate` is false
+
+        """
+        return self._last
+
+    @property
     def time(self) -> float:
         "Return the time"
         return self._time
 
     @property
     def accumulate(self) -> bool:
         "Are we accumulating the times?"
```

### Comparing `common-pyutil-0.8.6/common_pyutil/net.py` & `common-pyutil-0.8.7/common_pyutil/net.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/proc.py` & `common-pyutil-0.8.7/common_pyutil/proc.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/structures.py` & `common-pyutil-0.8.7/common_pyutil/structures.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/system.py` & `common-pyutil-0.8.7/common_pyutil/system.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/common_pyutil/venv.py` & `common-pyutil-0.8.7/common_pyutil/venv.py`

 * *Files identical despite different names*

### Comparing `common-pyutil-0.8.6/pyproject.toml` & `common-pyutil-0.8.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common-pyutil"
-version = "0.8.6"
+version = "0.8.7"
 description = "Some common python utility functions"
 authors = ["Akshay <atavist13@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/akshaybadola/common-pyutil"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `common-pyutil-0.8.6/setup.py` & `common-pyutil-0.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['file-magic>=0.4.0,<0.5.0', 'requests>=2.26.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['test = pytest:main']}
 
 setup_kwargs = {
     'name': 'common-pyutil',
-    'version': '0.8.6',
+    'version': '0.8.7',
     'description': 'Some common python utility functions',
     'long_description': "# common-pyutil\nBunch of common utility functions I've used in various projects. This package\nprovides a uniform interface to them.\n\n# Features\n\n- Pure python stdlib with no external dependencies (except [requests](https://github.com/psf/requests))\n- Bunch of useful modules like:\n  1. A simple hierarchical argument parser.\n  2. Functional programming library.\n  3. A `Timer` context for easy monitoring\n  4. A `Tag` decorator for function tagging\n  5. A logging module to get generate a logger with sensible defaults.\n  6. A `Get` class with progress tracking.\n",
     'author': 'Akshay',
     'author_email': 'atavist13@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/akshaybadola/common-pyutil',
```

### Comparing `common-pyutil-0.8.6/PKG-INFO` & `common-pyutil-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-pyutil
-Version: 0.8.6
+Version: 0.8.7
 Summary: Some common python utility functions
 Home-page: https://github.com/akshaybadola/common-pyutil
 License: MIT
 Keywords: utilities,functional
 Author: Akshay
 Author-email: atavist13@gmail.com
 Requires-Python: >=3.7,<4.0
```

