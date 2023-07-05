# Comparing `tmp/ou_tm351_jl_extensions-0.2.0.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.0.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.1.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.0.tar` & `ou_tm351_jl_extensions-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/LICENSE
--rw-r--r--   0        0        0      467 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/README.md
--rw-r--r--   0        0        0     2388 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      938 2023-06-22 17:41:34.079741 ou_tm351_jl_extensions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1370 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/README.md
+-rw-r--r--   0        0        0     2388 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      938 2023-07-05 00:48:01.501932 ou_tm351_jl_extensions-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.1/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.0/LICENSE` & `ou_tm351_jl_extensions-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.0/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.1/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.0/pyproject.toml` & `ou_tm351_jl_extensions-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 jupyterlab = "^4.0.1"
 jupyterlab-ou-brand-extension = "^0.2.0"
 jupyterlab-cell-status-extension = "^0.1.3"
-jupyterlab-myst = "^1.1.3"
+jupyterlab-myst = "^2.0.0"
 jupyterlab-empinken-extension = "^0.4.0"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^5.0.0"
 jupyterlab-git = "^0.41.0"
 jupytext = "^1.14.5"
 jupyter-archive = "^3.3.4"
 #jupyterlab-spellchecker = "^0.7.3"
```

