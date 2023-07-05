# Comparing `tmp/deephaven-plugin-matplotlib-0.1.1.tar.gz` & `tmp/deephaven-plugin-matplotlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-matplotlib-0.1.1.tar", last modified: Tue Nov 22 14:46:22 2022, max compression
+gzip compressed data, was "deephaven-plugin-matplotlib-0.1.2.tar", last modified: Wed Jul  5 19:50:24 2023, max compression
```

## Comparing `deephaven-plugin-matplotlib-0.1.1.tar` & `deephaven-plugin-matplotlib-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/deephaven.mplstyle
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-11-22 14:46:13.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/figure_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:46:22.986690 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-22 14:46:22.000000 deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4327 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.527347 deephaven-plugin-matplotlib-0.1.2/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.527347 deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     5728 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/deephaven.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (122)     3336 2023-07-05 19:50:13.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/figure_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 19:50:24.531348 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-05 19:50:24.000000 deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-matplotlib-0.1.1/LICENSE` & `deephaven-plugin-matplotlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-matplotlib-0.1.1/PKG-INFO` & `deephaven-plugin-matplotlib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-matplotlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Deephaven Plugin for matplotlib
 Home-page: https://github.com/deephaven/deephaven-plugin-matplotlib
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-matplotlib
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-matplotlib/issues
 Keywords: deephaven,plugin,matplotlib
@@ -126,20 +126,23 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin matplotlib
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
```

### Comparing `deephaven-plugin-matplotlib-0.1.1/README.md` & `deephaven-plugin-matplotlib-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,20 +106,23 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin matplotlib
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
```

### Comparing `deephaven-plugin-matplotlib-0.1.1/setup.cfg` & `deephaven-plugin-matplotlib-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/__init__.py` & `deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from deephaven.plugin import Registration
 from deephaven.table_listener import listen
 from importlib import resources
 import matplotlib.pyplot as plt
 from matplotlib.animation import Animation
 import itertools
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 def _init_theme():
     # Set the Deephaven style globally.
     # We use the savefig function to export the Figure, and that uses the Figure's properties for colours rather than temporary styling.
     # The Figure's properties are set on creation time of the Figure, rather than when the Figure is exported
     # We do not have hooks into when a user creates a new Figure, so we set the theme globally ahead of time
     # https://github.com/matplotlib/matplotlib/issues/6592/
@@ -153,9 +153,9 @@
         # to get the update information
         self._last_update = update
         return super()._step(*args)
 
     def _draw_frame(self, framedata):
         data = {}
         for column in self._columns:
-            data[column] = dhnp.to_numpy(self._table, [column])
+            data[column] = dhnp.to_numpy(self._table, [column])[:, 0]
         self._func(data, self._last_update, *self._args)
```

### Comparing `deephaven-plugin-matplotlib-0.1.1/src/deephaven/plugin/matplotlib/figure_type.py` & `deephaven-plugin-matplotlib-0.1.2/src/deephaven/plugin/matplotlib/figure_type.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO` & `deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-matplotlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Deephaven Plugin for matplotlib
 Home-page: https://github.com/deephaven/deephaven-plugin-matplotlib
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-matplotlib
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-matplotlib/issues
 Keywords: deephaven,plugin,matplotlib
@@ -126,20 +126,23 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin matplotlib
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
```

### Comparing `deephaven-plugin-matplotlib-0.1.1/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt` & `deephaven-plugin-matplotlib-0.1.2/src/deephaven_plugin_matplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

