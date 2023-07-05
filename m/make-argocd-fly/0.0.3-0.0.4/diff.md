# Comparing `tmp/make_argocd_fly-0.0.3.tar.gz` & `tmp/make_argocd_fly-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_argocd_fly-0.0.3.tar", last modified: Tue Jul  4 20:49:29 2023, max compression
+gzip compressed data, was "make_argocd_fly-0.0.4.tar", last modified: Wed Jul  5 19:56:20 2023, max compression
```

## Comparing `make_argocd_fly-0.0.3.tar` & `make_argocd_fly-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.3/LICENSE
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.3/MANIFEST.in
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      990 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      639 2023-07-04 19:17:22.000000 make_argocd_fly-0.0.3/README.md
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/make_argocd_fly/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.3/make_argocd_fly/__init__.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.3/make_argocd_fly/config.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.3/make_argocd_fly/log_config.yml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.3/make_argocd_fly/pipeline.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.3/make_argocd_fly/resource.py
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.3/make_argocd_fly/utils.py
-drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      990 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/PKG-INFO
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/SOURCES.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/dependency_links.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/entry_points.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/requires.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-04 20:49:29.000000 make_argocd_fly-0.0.3/make_argocd_fly.egg-info/top_level.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)      692 2023-07-04 20:48:54.000000 make_argocd_fly-0.0.3/pyproject.toml
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.3/requirements.txt
--rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-04 20:49:29.396254 make_argocd_fly-0.0.3/setup.cfg
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:56:20.064108 make_argocd_fly-0.0.4/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)    35149 2023-07-04 12:08:38.000000 make_argocd_fly-0.0.4/LICENSE
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       39 2023-07-04 12:31:11.000000 make_argocd_fly-0.0.4/MANIFEST.in
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2654 2023-07-05 19:56:20.054108 make_argocd_fly-0.0.4/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2303 2023-07-05 19:52:03.000000 make_argocd_fly-0.0.4/README.md
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:56:20.054108 make_argocd_fly-0.0.4/make_argocd_fly/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        0 2023-06-29 14:39:57.000000 make_argocd_fly-0.0.4/make_argocd_fly/__init__.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     1284 2023-07-04 11:21:42.000000 make_argocd_fly-0.0.4/make_argocd_fly/config.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      354 2023-06-29 19:14:16.000000 make_argocd_fly-0.0.4/make_argocd_fly/log_config.yml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     5535 2023-07-04 20:47:34.000000 make_argocd_fly-0.0.4/make_argocd_fly/pipeline.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     4243 2023-07-04 20:45:25.000000 make_argocd_fly-0.0.4/make_argocd_fly/resource.py
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      856 2023-07-04 20:39:27.000000 make_argocd_fly-0.0.4/make_argocd_fly/utils.py
+drwxr-xr-x   0 karandash8  (1000) karandash8  (1000)        0 2023-07-05 19:56:20.054108 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)     2654 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/PKG-INFO
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      463 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/SOURCES.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)        1 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/dependency_links.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       66 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/entry_points.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/requires.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       41 2023-07-05 19:56:20.000000 make_argocd_fly-0.0.4/make_argocd_fly.egg-info/top_level.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)      721 2023-07-05 19:56:08.000000 make_argocd_fly-0.0.4/pyproject.toml
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       26 2023-07-01 18:33:32.000000 make_argocd_fly-0.0.4/requirements.txt
+-rw-r--r--   0 karandash8  (1000) karandash8  (1000)       38 2023-07-05 19:56:20.064108 make_argocd_fly-0.0.4/setup.cfg
```

### Comparing `make_argocd_fly-0.0.3/LICENSE` & `make_argocd_fly-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.3/make_argocd_fly/config.py` & `make_argocd_fly-0.0.4/make_argocd_fly/config.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.3/make_argocd_fly/pipeline.py` & `make_argocd_fly-0.0.4/make_argocd_fly/pipeline.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.3/make_argocd_fly/resource.py` & `make_argocd_fly-0.0.4/make_argocd_fly/resource.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.3/make_argocd_fly/utils.py` & `make_argocd_fly-0.0.4/make_argocd_fly/utils.py`

 * *Files identical despite different names*

### Comparing `make_argocd_fly-0.0.3/pyproject.toml` & `make_argocd_fly-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "make_argocd_fly"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Andrei Lapin", email = "karandash8@gmail.com"},
 ]
 description = "A project to generate ArgoCD application resources"
 requires-python = ">=3.10"
 keywords = ["argocd", "kustomize", "jinja2"]
 license = {text = "GPLv3+"}
@@ -20,9 +20,9 @@
 [project.scripts]
 make-argocd-fly = "make_argocd_fly.pipeline:main"
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools.dynamic]
-readme = {file = ["README.md"]}
+readme = {file = ["README.md"], content-type = "text/plain"}
 dependencies = {file = ["requirements.txt"]}
```

