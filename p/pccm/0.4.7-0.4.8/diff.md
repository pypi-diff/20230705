# Comparing `tmp/pccm-0.4.7.tar.gz` & `tmp/pccm-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pccm-0.4.7.tar", last modified: Wed Apr 26 06:01:03 2023, max compression
+gzip compressed data, was "pccm-0.4.8.tar", last modified: Wed Jul  5 02:22:21 2023, max compression
```

## Comparing `pccm-0.4.7.tar` & `pccm-0.4.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.344854 pccm-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 06:00:20.000000 pccm-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 06:01:03.344854 pccm-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 06:00:20.000000 pccm-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.336854 pccm-0.4.7/pccm/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35550 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/inliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/builder/pybind.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/core/
--rw-r--r--   0 runner    (1001) docker     (123)   105155 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/buildmeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/funccode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/inspecttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/core/pycore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/numpylib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/libs/tvten.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/expose_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    51082 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/middlewares/pybind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/source/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/source/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/targets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/targets/cuda_ptx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/pccm/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/test_data/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 06:00:20.000000 pccm-0.4.7/pccm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.336854 pccm-0.4.7/pccm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-26 06:01:03.000000 pccm-0.4.7/pccm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 06:00:20.000000 pccm-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:01:03.344854 pccm-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-26 06:00:20.000000 pccm-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:01:03.340854 pccm-0.4.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-26 06:00:20.000000 pccm-0.4.7/test/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 02:21:39.000000 pccm-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-05 02:22:21.981932 pccm-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 02:21:39.000000 pccm-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35550 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/builder/inliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/builder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/builder/pybind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)   105944 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/buildmeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/funccode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/inspecttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/core/pycore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/libs/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/libs/numpylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/libs/stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/libs/tvten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/middlewares/expose_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51082 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/middlewares/pybind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/pccm/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/source/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/pccm/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/pccm/targets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/targets/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/targets/cuda_ptx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/pccm/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/test_data/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/test_data/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-05 02:21:39.000000 pccm-0.4.8/pccm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.977933 pccm-0.4.8/pccm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 02:22:21.000000 pccm-0.4.8/pccm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 02:21:39.000000 pccm-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 02:22:21.981932 pccm-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-05 02:21:39.000000 pccm-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:22:21.981932 pccm-0.4.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-05 02:21:39.000000 pccm-0.4.8/test/test_core.py
```

### Comparing `pccm-0.4.7/LICENSE` & `pccm-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/PKG-INFO` & `pccm-0.4.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccm
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python C++ Code Manager.
 Home-page: https://github.com/FindDefinition/PCCM
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pccm-0.4.7/pccm/__init__.py` & `pccm-0.4.8/pccm/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/builder/inliner.py` & `pccm-0.4.8/pccm/builder/inliner.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/builder/main.py` & `pccm-0.4.8/pccm/builder/main.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/builder/pybind.py` & `pccm-0.4.8/pccm/builder/pybind.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/__init__.py` & `pccm-0.4.8/pccm/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,23 +336,25 @@
                  inline: bool = False,
                  constexpr: bool = False,
                  attrs: Optional[List[str]] = None,
                  name: Optional[str] = None,
                  macro_guard: Optional[str] = None,
                  impl_loc: str = "",
                  impl_file_suffix: str = ".cc",
-                 header_only: Optional[bool] = None):
+                 header_only: Optional[bool] = None,
+                 extern_c: bool = False):
         super().__init__(inline=inline,
                          constexpr=constexpr,
                          attrs=attrs,
                          name=name,
                          macro_guard=macro_guard,
                          impl_loc=impl_loc,
                          impl_file_suffix=impl_file_suffix,
-                         header_only=header_only)
+                         header_only=header_only,)
+        self.extern_c = extern_c
 
     def get_pre_attrs(self) -> List[str]:
         res = super().get_pre_attrs()  # type: List[str]
         res.append("static")
         return res
 
 
@@ -364,30 +366,35 @@
                  constexpr: bool = False,
                  attrs: Optional[List[str]] = None,
                  name: Optional[str] = None,
                  macro_guard: Optional[str] = None,
                  impl_loc: str = "",
                  impl_file_suffix: str = ".cc",
                  header_only: Optional[bool] = None,
-                 friend: bool = False):
+                 friend: bool = False,
+                 extern_c: bool = False):
         # TODO better handle friend method
         # currently we only support direct friend method
         # declaration.
         super().__init__(inline=inline,
                          constexpr=constexpr,
                          attrs=attrs,
                          name=name,
                          macro_guard=macro_guard,
                          impl_loc=impl_loc,
                          impl_file_suffix=impl_file_suffix,
                          header_only=header_only,
                          friend=friend)
+        self.extern_c = extern_c
 
     def get_pre_attrs(self) -> List[str]:
-        res = super().get_pre_attrs()  # type: List[str]
+        res: List[str] = []
+        if self.extern_c:
+            res.append("extern \"C\"")
+        res.extend(super().get_pre_attrs())
         if self.friend:
             res.append("friend")
         return res
 
 
 class Typedef(object):
     def __init__(self, name: str, content: str):
@@ -515,14 +522,16 @@
 
         self._impl_only_deps: List[Dependency] = []
         self._impl_only_pdeps: List[Dependency] = []
         self._invalid = False
 
         self._type_to_hook: Dict[str, FuncArgAttrHandler] = {}
 
+        self.func_name_override: Optional[str] = None 
+
     def is_template(self) -> bool:
         return len(self._template_arguments) > 0
 
     def make_invalid(self):
         self._invalid = True
         return self
 
@@ -2211,14 +2220,16 @@
                     msg = "your func {}-{}-{} must return a FunctionCode".format(
                         cu.namespace, cu.class_name, v.__name__)
                     raise ValueError(msg)
                 if code_obj.is_invalid():
                     continue
                 func_doc = inspect.getdoc(v)
                 code_obj.func_doc = func_doc
+                if code_obj.func_name_override is not None:
+                    meta.name = code_obj.func_name_override
                 methods.append(FunctionDecl(meta, code_obj))
         return methods
 
     def get_code_units(self) -> List[Class]:
         return self.code_units
 
     def construct_build_meta(self, cus: List[Union[Class, ParameterizedClass]]):
@@ -2285,15 +2296,16 @@
                 header_to_meta[header_key] = meta
         return header_dict, impl_dict, header_to_impls, impl_to_buildmeta, header_to_meta
 
     def code_generation_with_cmake(self,
                         target_name: str,
                         cus: List[Union[Class, ParameterizedClass]],
                         include_root: Optional[Path] = None,
-                        cxx_standard="14"):
+                        cxx_standard="14",
+                        disable_cmake_default_arch: bool = False):
         header_dict = OrderedDict()  # type: Dict[str, CodeSectionHeader]
         impl_dict = OrderedDict()  # type: Dict[str, CodeSectionImpl]
         header_to_impls = OrderedDict()  # type: Dict[str, List[str]]
         impl_to_buildmeta = OrderedDict()  # type: Dict[str, BuildMeta]
         uid_to_meta: Dict[str, BuildMeta] = {}
         header_to_meta: Dict[str, BuildMeta] = {}
         path_to_cmake_content: Dict[str, str] = {}
@@ -2345,14 +2357,19 @@
                 else:
                     cflags_list = compiler_to_cflags.get("g++", []) + global_meta.get_global_cflags().get("g++", [])
                 cflags_stmt = ""
                 if cflags_list:
                     cflags_list_str = "\n".join(["    " + p for p in cflags_list])
                     cflags_stmt = (f"target_compile_options({cu_target_name} PRIVATE "
                     f"$<$<COMPILE_LANGUAGE:CXX>: \n{cflags_list_str}>)")
+                disable_cmake_default_arch_str = ""
+                if disable_cmake_default_arch:
+                    # this only works on cmake >= 3.24
+                    disable_cmake_default_arch_str = f"set_target_properties({cu_target_name} PROPERTIES CUDA_ARCHITECTURES OFF)"
+
                 cmake_static_libs.append(cu_target_name)
                 # TODO why POSITION_INDEPENDENT_CODE (add -dc to nvcc) not working on nvcc?
                 cmakecontents = f"""
 cmake_minimum_required(VERSION 3.20)
 add_library({cu_target_name} OBJECT {' '.join(impl_file_names)})
 # set_target_properties({cu_target_name} PROPERTIES POSITION_INDEPENDENT_CODE ON)
 set_target_properties( {cu_target_name} PROPERTIES CXX_STANDARD {cxx_standard} CUDA_STANDARD {cxx_standard})
@@ -2360,14 +2377,15 @@
 # set_target_properties({cu_target_name} PROPERTIES CUDA_SEPARABLE_COMPILATION ON)
 # set_target_properties({cu_target_name} PROPERTIES CUDA_RESOLVE_DEVICE_SYMBOLS ON)
 
 target_include_directories({cu_target_name} PRIVATE
 {includes_str})
 {cuda_flags}
 {cflags_stmt}
+{disable_cmake_default_arch_str}
                 """
                 path_to_cmake_content[cmakepath] = cmakecontents
                 main_cmake_contents.append(f"add_subdirectory({str(Path(cmakepath).parent)})")
 
             for k in cu_impls_dict.keys():
                 impl_to_buildmeta[k] = meta
             header_to_meta[header_key] = meta
```

### Comparing `pccm-0.4.7/pccm/core/codegen.py` & `pccm-0.4.8/pccm/core/codegen.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/funccode.py` & `pccm-0.4.8/pccm/core/funccode.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/inspecttools.py` & `pccm-0.4.8/pccm/core/inspecttools.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/markers.py` & `pccm-0.4.8/pccm/core/markers.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/parsers.py` & `pccm-0.4.8/pccm/core/parsers.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/core/pycore.py` & `pccm-0.4.8/pccm/core/pycore.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/extension.py` & `pccm-0.4.8/pccm/extension.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/graph/__init__.py` & `pccm-0.4.8/pccm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/libs/numpylib.py` & `pccm-0.4.8/pccm/libs/numpylib.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/libs/stl.py` & `pccm-0.4.8/pccm/libs/stl.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/libs/tvten.py` & `pccm-0.4.8/pccm/libs/tvten.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/middlewares/__init__.py` & `pccm-0.4.8/pccm/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/middlewares/expose_main.py` & `pccm-0.4.8/pccm/middlewares/expose_main.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/middlewares/pybind.py` & `pccm-0.4.8/pccm/middlewares/pybind.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/source/__init__.py` & `pccm-0.4.8/pccm/source/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/source/core.py` & `pccm-0.4.8/pccm/source/core.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/stubs/__init__.py` & `pccm-0.4.8/pccm/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/targets/cuda.py` & `pccm-0.4.8/pccm/targets/cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
                          inline: bool = False,
                          attrs: Optional[List[str]] = None,
                          macro_guard: Optional[str] = None,
                          impl_loc: str = "",
                          impl_file_suffix: str = ".cu",
                          launch_bounds: Optional[Tuple[int, int]] = None,
                          header_only: Optional[bool] = None,
+                         extern_c: bool = False,
                          name=None):
     if attrs is None:
         attrs = []
     cuda_global_attrs = attrs + ["__global__"]
     if launch_bounds is not None:
         cuda_global_attrs.append("__launch_bounds__({}, {})".format(
             launch_bounds[0], launch_bounds[1]))
@@ -60,15 +61,16 @@
                             inline=inline,
                             constexpr=False,
                             macro_guard=macro_guard,
                             impl_loc=impl_loc,
                             impl_file_suffix=impl_file_suffix,
                             attrs=cuda_global_attrs,
                             header_only=header_only,
-                            is_global=True)
+                            is_global=True,
+                            extern_c=extern_c)
 
 
 def member_function(func=None,
                     host: bool = False,
                     device: bool = False,
                     inline: bool = False,
                     forceinline: bool = False,
@@ -150,14 +152,15 @@
                       constexpr: bool = False,
                       attrs: Optional[List[str]] = None,
                       macro_guard: Optional[str] = None,
                       impl_loc: str = "",
                       impl_file_suffix: str = ".cu",
                       header_only: Optional[bool] = None,
                       is_global: bool = False,
+                      extern_c: bool = False,
                       name=None):
     if forceinline or inline:
         assert forceinline is not inline, "can't set both inline and forceinline"
     cuda_global_attrs = []
     if forceinline:
         cuda_global_attrs.append("__forceinline__")
     if host:
@@ -173,15 +176,16 @@
     meta = meta_cls(name=name,
                     inline=inline,
                     constexpr=constexpr,
                     attrs=attrs,
                     macro_guard=macro_guard,
                     impl_loc=impl_loc,
                     impl_file_suffix=impl_file_suffix,
-                    header_only=header_only)
+                    header_only=header_only,
+                    extern_c=extern_c)
     return markers.meta_decorator(func, meta)
 
 
 def constructor(func=None,
                 host: bool = False,
                 device: bool = False,
                 inline: bool = False,
```

### Comparing `pccm-0.4.7/pccm/targets/cuda_ptx.py` & `pccm-0.4.8/pccm/targets/cuda_ptx.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/test_data/__init__.py` & `pccm-0.4.8/pccm/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/test_data/example.py` & `pccm-0.4.8/pccm/test_data/example.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/test_data/mod.py` & `pccm-0.4.8/pccm/test_data/mod.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm/utils.py` & `pccm-0.4.8/pccm/utils.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/pccm.egg-info/PKG-INFO` & `pccm-0.4.8/pccm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pccm
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python C++ Code Manager.
 Home-page: https://github.com/FindDefinition/PCCM
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pccm-0.4.7/pccm.egg-info/SOURCES.txt` & `pccm-0.4.8/pccm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/setup.py` & `pccm-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `pccm-0.4.7/test/test_core.py` & `pccm-0.4.8/test/test_core.py`

 * *Files identical despite different names*

