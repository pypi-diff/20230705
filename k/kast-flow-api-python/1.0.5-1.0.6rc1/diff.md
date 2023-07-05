# Comparing `tmp/kast_flow_api_python-1.0.5.tar.gz` & `tmp/kast_flow_api_python-1.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kast_flow_api_python-1.0.5.tar", max compression
+gzip compressed data, was "kast_flow_api_python-1.0.6rc1.tar", max compression
```

## Comparing `kast_flow_api_python-1.0.5.tar` & `kast_flow_api_python-1.0.6rc1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-27 08:59:44.985066 kast_flow_api_python-1.0.5/kast_flow_api/__init__.py
--rw-r--r--   0        0        0     8970 2023-06-27 08:59:44.960066 kast_flow_api_python-1.0.5/kast_flow_api/v1.py
--rw-r--r--   0        0        0      528 2023-06-27 09:00:05.108127 kast_flow_api_python-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-05 08:45:28.809107 kast_flow_api_python-1.0.6rc1/kast_flow_api/__init__.py
+-rw-r--r--   0        0        0     8970 2023-07-05 08:45:28.783107 kast_flow_api_python-1.0.6rc1/kast_flow_api/v1.py
+-rw-r--r--   0        0        0      537 2023-07-05 08:45:48.563153 kast_flow_api_python-1.0.6rc1/pyproject.toml
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 kast_flow_api_python-1.0.6rc1/PKG-INFO
```

### Comparing `kast_flow_api_python-1.0.5/kast_flow_api/v1.py` & `kast_flow_api_python-1.0.6rc1/kast_flow_api/v1.py`

 * *Files identical despite different names*

### Comparing `kast_flow_api_python-1.0.5/pyproject.toml` & `kast_flow_api_python-1.0.6rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kast-flow-api-python"
-version = "1.0.5"
+version = "1.0.6-preview1"
 description = "kast python api unified processing engine"
 authors = ["kast"]
 packages = [
     { include = "kast_flow_api" }
 ]
 
 [tool.poetry.dependencies]
```

