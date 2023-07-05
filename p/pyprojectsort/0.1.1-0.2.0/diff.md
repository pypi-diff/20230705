# Comparing `tmp/pyprojectsort-0.1.1.tar.gz` & `tmp/pyprojectsort-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectsort-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprojectsort-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprojectsort-0.1.1.tar` & `pyprojectsort-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1938 2023-06-26 20:17:28.006407 pyprojectsort-0.1.1/README.md
--rw-r--r--   0        0        0     2079 2023-06-26 20:17:38.010333 pyprojectsort-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      203 2023-06-26 20:17:28.006407 pyprojectsort-0.1.1/pyprojectsort/__init__.py
--rw-r--r--   0        0        0      197 2023-06-26 20:17:28.006407 pyprojectsort-0.1.1/pyprojectsort/__version__.py
--rw-r--r--   0        0        0      816 2023-06-26 20:17:28.006407 pyprojectsort-0.1.1/pyprojectsort/main.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 pyprojectsort-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3098 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/README.md
+-rw-r--r--   0        0        0     2034 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/pyprojectsort/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/pyprojectsort/__main__.py
+-rw-r--r--   0        0        0      197 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/pyprojectsort/__version__.py
+-rw-r--r--   0        0        0     3038 2023-07-05 18:55:50.374415 pyprojectsort-0.2.0/pyprojectsort/main.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 pyprojectsort-0.2.0/PKG-INFO
```

### Comparing `pyprojectsort-0.1.1/pyproject.toml` & `pyprojectsort-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 
 [project]
 authors = [
     { name = "Kieran Ryan" },
 ]
 name = "pyprojectsort"
-description = "Autoformatter for pyproject.toml files"
+description = "Formatter for pyproject.toml files"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
@@ -28,42 +28,39 @@
     "version",
 ]
 
 [project.scripts]
 pyprojectsort = "pyprojectsort.main:main"
 
 [project.urls]
-Documentation = "https://kieran-ryan.github.io/python-package-template/"
-Source = "https://github.com/kieran-ryan/python-package-template"
-Tracker = "https://github.com/kieran-ryan/python-package-template/issues"
+Documentation = "https://kieran-ryan.github.io/pyprojectsort/"
+Source = "https://github.com/kieran-ryan/pyprojectsort"
+Tracker = "https://github.com/kieran-ryan/pyprojectsort/issues"
 
 [tool.flit.module]
 name = "pyprojectsort"
 
 [tool.bandit]
 exclude_dirs = [
     "tests",
     "venv",
 ]
 
-[tool.black]
-preview = true
-
 [tool.coverage.html]
 directory = "docs/coverage"
 
 [tool.coverage.run]
 branch = true
 omit = [
     "*/tests/*",
     "*/venv/*",
 ]
 
 [tool.coverage.report]
-fail_under = 90.0
+fail_under = 75.0
 show_missing = true
 
 [tool.coverage.xml]
 output = "docs/coverage/coverage.xml"
 
 [tool.isort]
 profile = "black"
@@ -82,32 +79,34 @@
 ]
 ignore = [
     "ANN",
     "ARG",
     "DTZ005",
     "D203",
     "D213",
+    "FIX002",
     "G004",
     "INP001",
     "S101",
     "T201",
+    "TD003",
 ]
 
 [tool.ruff.isort]
 required-imports = [
     "from __future__ import annotations",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.mypy]
 mypy_path = "pyprojectsort"
 files = "."
-exclude = "__init__.py|setup.py|docs|tests|venv"
+exclude = "__init__.py|docs|tests|venv"
 
 [tool.pylint]
 recursive = true
 ignore = [
     "docs",
     "tests",
     "venv",
```

