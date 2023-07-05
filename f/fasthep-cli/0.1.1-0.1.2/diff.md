# Comparing `tmp/fasthep_cli-0.1.1.tar.gz` & `tmp/fasthep_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasthep_cli-0.1.1.tar", last modified: Wed Nov 30 20:13:32 2022, max compression
+gzip compressed data, was "fasthep_cli-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fasthep_cli-0.1.1.tar` & `fasthep_cli-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1425 2022-11-30 20:13:25.929086 fasthep_cli-0.1.1/README.md
--rw-r--r--   0        0        0     2705 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      235 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/__init__.py
--rw-r--r--   0        0        0      438 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/_carpenter.py
--rw-r--r--   0        0        0     1227 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/_download.py
--rw-r--r--   0        0        0     1297 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/_plotter.py
--rw-r--r--   0        0        0      849 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/_software.py
--rw-r--r--   0        0        0     4838 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/main.py
--rw-r--r--   0        0        0        0 2022-11-30 20:13:25.933086 fasthep_cli-0.1.1/src/fasthep_cli/py.typed
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 fasthep_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1425 2023-07-05 19:00:16.959376 fasthep_cli-0.1.2/README.md
+-rw-r--r--   0        0        0     2705 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/__init__.py
+-rw-r--r--   0        0        0     1227 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/_download.py
+-rw-r--r--   0        0        0     1297 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/_plotter.py
+-rw-r--r--   0        0        0     1221 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/_software.py
+-rw-r--r--   0        0        0     6513 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/logo.py
+-rw-r--r--   0        0        0     4306 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:00:16.963376 fasthep_cli-0.1.2/src/fasthep_cli/py.typed
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 fasthep_cli-0.1.2/PKG-INFO
```

### Comparing `fasthep_cli-0.1.1/README.md` & `fasthep_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fasthep_cli-0.1.1/pyproject.toml` & `fasthep_cli-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fasthep_cli-0.1.1/src/fasthep_cli/_download.py` & `fasthep_cli-0.1.2/src/fasthep_cli/_download.py`

 * *Files identical despite different names*

### Comparing `fasthep_cli-0.1.1/src/fasthep_cli/_plotter.py` & `fasthep_cli-0.1.2/src/fasthep_cli/_plotter.py`

 * *Files identical despite different names*

### Comparing `fasthep_cli-0.1.1/PKG-INFO` & `fasthep_cli-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasthep_cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command line interface for the FAST-HEP tools (one to rule them all)
 Author-email: Luke Kreczko <fast-hep@cern.ch>
 Maintainer-email: The FAST-HEP maintainers <fast-hep@cern.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
```

