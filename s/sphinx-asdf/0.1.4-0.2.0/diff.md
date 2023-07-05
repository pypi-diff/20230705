# Comparing `tmp/sphinx-asdf-0.1.4.tar.gz` & `tmp/sphinx-asdf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-asdf-0.1.4.tar", last modified: Fri Jul  8 16:47:50 2022, max compression
+gzip compressed data, was "sphinx-asdf-0.2.0.tar", last modified: Wed Jul  5 19:25:00 2023, max compression
```

## Comparing `sphinx-asdf-0.1.4.tar` & `sphinx-asdf-0.2.0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.300073 sphinx-asdf-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/.github/workflows/sphinx_asdf_ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-07-08 16:47:50.300073 sphinx-asdf-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/bandit.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-07-08 16:47:50.300073 sphinx-asdf-0.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       81 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/sphinx_asdf/
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/asdf2rst.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/connections.py
--rw-r--r--   0 runner    (1001) docker     (121)    16501 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/directives.py
--rw-r--r--   0 runner    (1001) docker     (121)     5210 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/md2rst.py
--rw-r--r--   0 runner    (1001) docker     (121)     5229 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/sphinx_asdf/static/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/logo.ico
--rw-r--r--   0 runner    (1001) docker     (121)    10668 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    16762 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/sphinx_asdf.css
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/static/sphinx_asdf.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/sphinx_asdf/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/sphinx_asdf/templates/schema.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7092 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-08 16:47:50.000000 sphinx-asdf-0.1.4/sphinx_asdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/schemas/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/schemas/core/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/schemas/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-basic-generation/schemas/foo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-global-config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/schemas/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/schemas/core/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/schemas/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-config/a/b/c/schemas/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-config/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-config/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.296073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/contents.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.292073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.300073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/c/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/c/bar.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 16:47:50.300073 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/c/core/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/c/core/baz.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/roots/test-global-prefix/schemas/a/b/c/foo.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tests/test_sphinx_asdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-07-08 16:47:40.000000 sphinx-asdf-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.github/workflows/sphinx_asdf_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 19:25:00.220387 sphinx-asdf-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/sphinx_asdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/asdf2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/md2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/sphinx_asdf/templates/schema.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 19:25:00.000000 sphinx-asdf-0.2.0/sphinx_asdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-basic-generation/schemas/foo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.208387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/a/b/c/schemas/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-config/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/contents.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.212387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/bar.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:25:00.216387 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/core/baz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/roots/test-global-prefix/schemas/a/b/c/foo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tests/test_sphinx_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-05 19:24:49.000000 sphinx-asdf-0.2.0/tox.ini
```

### Comparing `sphinx-asdf-0.1.4/.github/workflows/publish-to-pypi.yml` & `sphinx-asdf-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/.github/workflows/sphinx_asdf_ci.yml` & `sphinx-asdf-0.2.0/.github/workflows/sphinx_asdf_ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: CI
 
 on:
   push:
     branches:
-      - master
+      - main
     tags:
       - "*"
   pull_request:
     branches:
 
 jobs:
   tox_pytest:
```

### Comparing `sphinx-asdf-0.1.4/.pre-commit-config.yaml` & `sphinx-asdf-0.2.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 repos:
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-yaml
     args: ["--unsafe"]
   - id: debug-statements
   - id: end-of-file-fixer
   - id: trailing-whitespace
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.34.0
+  rev: v3.8.0
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
     - id: flake8
 
 - repo: https://github.com/PyCQA/bandit
-  rev: 1.7.4
+  rev: 1.7.5
   hooks:
     - id: bandit
       args: ["-c", "bandit.yaml"]
```

### Comparing `sphinx-asdf-0.1.4/CONTRIBUTING.md` & `sphinx-asdf-0.2.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Please open a new issue or new pull request for bugs, feedback, or new features
 you would like to see. If there is an issue you would like to work on, please
 leave a comment and we will be happy to assist. New contributions and
 contributors are very welcome!
 
-The main development work is done on the "master" branch. The "stable" branch is
+The main development work is done on the "main" branch. The "stable" branch is
 protected and used for official releases. The rest of the branches are for
 release maintenance and should not be used normally. Unless otherwise told by a
-maintainer, pull request should be made and submitted to the "master" branch.
+maintainer, pull request should be made and submitted to the "main" branch.
 
 New to github or open source projects? If you are unsure about where to start or
 haven't used github before, please feel free to contact the package maintainers.
 
 Feedback and feature requests? Is there something missing you would like to see?
 Please open an issue or send an email to the maintainers. This package follows
 the Spacetelescope `Code of Conduct<CODE_OF_CONDUCT.md>`_ strives to provide a
```

### Comparing `sphinx-asdf-0.1.4/LICENSE` & `sphinx-asdf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/PKG-INFO` & `sphinx-asdf-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sphinx-asdf
-Version: 0.1.4
+Version: 0.2.0
 Summary: Sphinx plugin for generating documentation from ASDF schemas
 Home-page: https://github.com/spacetelescope/sphinx-asdf
 Author: The ASDF Developers
 License: BSD-3-Clause
 Provides: sphinx_asdf
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Provides-Extra: tests
 License-File: LICENSE
 
 sphinx-asdf
 ===========
 
 .. image:: https://github.com/asdf-format/sphinx-asdf/workflows/CI/badge.svg
@@ -23,15 +23,15 @@
 Installation
 ------------
 
 To install the latest release on PyPI::
 
     $ pip install sphinx-asdf
 
-The latest development version is available from the ``master`` branch `on
+The latest development version is available from the ``main`` branch `on
 github`_. To clone the project:
 
 ::
 
     $ git clone https://github.com/asdf-format/sphinx-asdf
 
 To install:
```

### Comparing `sphinx-asdf-0.1.4/README.rst` & `sphinx-asdf-0.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Installation
 ------------
 
 To install the latest release on PyPI::
 
     $ pip install sphinx-asdf
 
-The latest development version is available from the ``master`` branch `on
+The latest development version is available from the ``main`` branch `on
 github`_. To clone the project:
 
 ::
 
     $ git clone https://github.com/asdf-format/sphinx-asdf
 
 To install:
```

### Comparing `sphinx-asdf-0.1.4/setup.cfg` & `sphinx-asdf-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,26 @@
 description = Sphinx plugin for generating documentation from ASDF schemas
 long_description = file: README.rst
 url = https://github.com/spacetelescope/sphinx-asdf
 github_project = spacetelescope/sphinx-asdf
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.9
 include_package_data = True
 setup_requires = setuptools_scm
 install_requires = 
 	asdf
 	astropy>=5.0.4
 	docutils
-	graphviz
-	matplotlib
-	myst-parser
-	mistune~=0.8.4
+	mistune>=3
 	sphinx
 	sphinx-astropy
 	sphinx_bootstrap_theme
 	sphinx-rtd-theme
-	sphinx-inline-tabs
 	toml
 
 [options.extras_require]
 tests = 
 	pytest
 
 [flake8]
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/__init__.py` & `sphinx-asdf-0.2.0/sphinx_asdf/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     update_app_config,
 )
 from .directives import AsdfAutoschemas, AsdfSchema, schema_def
 from .nodes import add_asdf_nodes
 
 
 def setup(app):
-
     # Describes a path relative to the sphinx source directory
     app.add_config_value("asdf_schema_path", "schemas", "env")
     app.add_config_value("asdf_schema_standard_prefix", "", "env")
     app.add_config_value("asdf_schema_reference_mappings", [], "env")
 
     app.add_directive("asdf-autoschemas", AsdfAutoschemas)
     app.add_directive("asdf-schema", AsdfSchema)
@@ -33,10 +32,9 @@
     app.connect("html-page-context", handle_page_context)
     app.connect("doctree-read", add_labels_to_nodes)
     app.connect("build-finished", on_build_finished)
 
     static_dir = os.path.join(os.path.dirname(__file__), "static")
 
     app.config._raw_config.setdefault("html_static_path", []).append(static_dir)
-    app.add_css_file("custom.css")
 
     return dict(version="0.1.1", parallel_read_safe=True, parallel_write_safe=True)
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/asdf2rst.py` & `sphinx-asdf-0.2.0/sphinx_asdf/asdf2rst.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             kwargs = dict()
             # Use the ignore_unrecognized_tag parameter as a proxy for both options
             kwargs["ignore_unrecognized_tag"] = "ignore_unrecognized_tag" in self.arguments
             kwargs["ignore_missing_extensions"] = "ignore_unrecognized_tag" in self.arguments
 
             if show_bocks:
                 with asdf.open(filename, **kwargs) as ff:
-                    for i, block in enumerate(ff.blocks.internal_blocks):
+                    for i, block in enumerate(ff._blocks.internal_blocks):
                         data = codecs.encode(block.data.tobytes(), "hex")
                         if len(data) > 40:
                             data = data[:40] + b"..."
                         allocated = block._allocated
                         size = block._size
                         data_size = block._data_size
                         flags = block._flags
@@ -123,18 +123,18 @@
                         code += "\n"
 
                         literal = nodes.literal_block(code, code)
                         literal["language"] = "yaml"
                         set_source_info(self, literal)
                         parts.append(literal)
 
-                    internal_blocks = list(ff.blocks.internal_blocks)
+                    internal_blocks = list(ff._blocks.internal_blocks)
                     if len(internal_blocks) and internal_blocks[-1].array_storage != "streamed":
                         buff = io.BytesIO()
-                        ff.blocks.write_block_index(buff, ff)
+                        ff._blocks.write_block_index(buff, ff)
                         block_index = buff.getvalue().decode("utf-8")
                         literal = nodes.literal_block(block_index, block_index)
                         literal["language"] = "yaml"
                         set_source_info(self, literal)
                         parts.append(literal)
 
         finally:
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/conf.py` & `sphinx-asdf-0.2.0/sphinx_asdf/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 
 static_dir = os.path.join(os.path.dirname(__file__), "static")
 html_logo = f"{static_dir}/logo.png"
 html_favicon = f"{static_dir}/logo.ico"
 latex_logo = f"{static_dir}/logo.pdf"
 
 sys.path.insert(0, os.path.join(os.path.abspath(os.path.dirname("__file__")), "sphinxext"))
-extensions += ["sphinx_asdf", "sphinx_inline_tabs", "myst_parser"]
+extensions += ["sphinx_asdf"]
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/connections.py` & `sphinx-asdf-0.2.0/sphinx_asdf/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import posixpath
 import warnings
 
+import sphinx.builders
 from docutils import nodes
-from sphinx.io import read_doc
 from sphinx.util import rst
 from sphinx.util.docutils import sphinx_domains
 from sphinx.util.fileutil import copy_asset
 
 from .directives import schema_def
 from .nodes import schema_doc
 
@@ -18,21 +18,22 @@
 def find_autoasdf_directives(env, filename):
     if filename.endswith(".md"):
         return []
 
     docname = env.path2doc(filename)
     env.prepare_settings(docname)
     with sphinx_domains(env), rst.default_role(docname, env.config.default_role):
-        doctree = read_doc(env.app, env, env.doc2path(docname))
+        builder = sphinx.builders.text.TextBuilder(env.app, env)
+        builder.read_doc(docname)
+        doctree = env.get_and_resolve_doctree(docname, builder)
 
-    return doctree.traverse(schema_def)
+    return doctree.findall(schema_def)
 
 
 def find_autoschema_references(app, genfiles):
-
     # We set this environment variable to indicate that the AsdfSchemas
     # directive should be parsed as a simple list of schema references
     # rather than as the toctree that will be generated when the documentation
     # is actually built.
     app.env.autoasdf_generate = True
 
     logger = logging.getLogger("sphinx")
@@ -51,15 +52,14 @@
     # Unset this variable now that we're done.
     app.env.autoasdf_generate = False
 
     return list(schemas)
 
 
 def create_schema_docs(app, schemas):
-
     for schema in schemas:
         schema_name = schema.children[0].astext()
         standard_prefix = schema.standard_prefix or app.env.config.asdf_schema_standard_prefix
         output_dir = posixpath.join(app.srcdir, "generated", standard_prefix)
         doc_path = posixpath.join(output_dir, schema_name + ".rst")
 
         if posixpath.exists(doc_path):
@@ -75,15 +75,14 @@
             if standard_prefix:
                 ff.write(f"    :standard_prefix: {standard_prefix}\n")
             ff.write(f"    :schema_root: {schema.schema_root}\n\n")
             ff.write(f"    {schema_name}\n")
 
 
 def autogenerate_schema_docs(app):
-
     env = app.env
 
     genfiles = [env.doc2path(x, base=None) for x in env.found_docs if posixpath.isfile(env.doc2path(x))]
 
     if not genfiles:
         return
 
@@ -102,30 +101,30 @@
     dist = get_distribution("sphinx_asdf")
     config.html_context["sphinx_asdf_version"] = dist.version
 
 
 def handle_page_context(app, pagename, templatename, ctx, doctree):
     # Use custom template when rendering pages containing schema documentation.
     # This allows us to selectively include bootstrap
-    if doctree is not None and doctree.traverse(schema_doc):
+    if doctree is not None and doctree.findall(schema_doc):
         return os.path.join(TEMPLATE_PATH, "schema.html")
 
 
 def normalize_name(name):
     for char in [".", "_", "/"]:
         name = name.replace(char, "-")
     return name
 
 
 def add_labels_to_nodes(app, document):
     labels = app.env.domaindata["std"]["labels"]
     anonlabels = app.env.domaindata["std"]["anonlabels"]
     basepath = os.path.join("generated", app.env.config.asdf_schema_standard_prefix)
 
-    for node in document.traverse():
+    for node in document.findall():
         if isinstance(node, str) or not (isinstance(node, nodes.Node) and node["ids"]):
             continue
 
         labelid = node["ids"][0]
         docname = app.env.docname
         basename = os.path.relpath(docname, basepath)
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/directives.py` & `sphinx-asdf-0.2.0/sphinx_asdf/directives.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,23 @@
     def __init__(self, *args, **kwargs):
         self.schema_root = kwargs.pop("schema_root", "")
         self.standard_prefix = kwargs.pop("standard_prefix", "")
         super().__init__(*args, **kwargs)
 
 
 class AsdfAutoschemas(SphinxDirective):
-
     required_arguments = 0
     optional_arguments = 2
     has_content = True
     option_spec = {
         "schema_root": directives.path,
         "standard_prefix": directives.unchanged,
     }
 
     def _process_asdf_toctree(self, standard_prefix):
-
         links = []
         for name in self.content:
             if not name:
                 continue
             schema = self.env.path2doc(name.strip() + ".rst")
             link = posixpath.join("generated", standard_prefix, schema)
             links.append((schema, link))
@@ -69,15 +67,14 @@
         tocnode["entries"] = links
         tocnode["maxdepth"] = -1
         tocnode["glob"] = None
 
         return [tocnode]
 
     def run(self):
-
         standard_prefix = self.options.get("standard_prefix", self.env.config.asdf_schema_standard_prefix)
 
         # This is the case when we are actually using Sphinx to generate
         # documentation
         if not getattr(self.env, "autoasdf_generate", False):
             return self._process_asdf_toctree(standard_prefix)
 
@@ -90,24 +87,22 @@
         return [
             schema_def(text=c.strip().split()[0], standard_prefix=standard_prefix, schema_root=schema_root)
             for c in self.content
         ]
 
 
 class AsdfSchema(SphinxDirective):
-
     has_content = True
     optional_arguments = 2
     option_spec = {
         "schema_root": directives.path,
         "standard_prefix": directives.unchanged,
     }
 
     def run(self):
-
         self.envconfig = self.state.document.settings.env.config
         self.schema_name = self.content[0]
         schema_dir = self.options.get("schema_root", self.envconfig.asdf_schema_path)
         standard_prefix = self.options.get("standard_prefix", self.envconfig.asdf_schema_standard_prefix)
         srcdir = self.state.document.settings.env.srcdir
 
         schema_file = posixpath.join(srcdir, schema_dir, standard_prefix, self.schema_name) + ".yaml"
@@ -195,15 +190,14 @@
 
         if not schema_id.endswith(".html"):
             schema_id += ".html"
 
         return schema_id
 
     def _create_reference(self, refname, shorten=False):
-
         if "#" in refname:
             schema_id, fragment = refname.split("#")
         else:
             schema_id = refname
             fragment = ""
 
         if schema_id:
@@ -377,15 +371,14 @@
             combiner_list.append(schema_combiner_item(None, *[properties]))
 
         container_node.append(combiner_list)
         container_node["ids"] = [path]
         return schema_properties(None, *[container_node], id=path)
 
     def _create_property_node(self, name, tree, required, path=""):
-
         description = tree.get("description", "")
 
         if "$ref" in tree:
             typ, ref = self._create_reference(tree.get("$ref"), shorten=True)
         elif "tag" in tree:
             _tag = tree.get("tag")
             typ, ref = self._create_reference(_tag, shorten=True)
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/nodes.py` & `sphinx-asdf-0.2.0/sphinx_asdf/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,10 +196,9 @@
 ]
 
 
 __all__ = [klass.__name__ for klass in custom_nodes] + ["add_asdf_nodes"]
 
 
 def add_asdf_nodes(app):
-
     for node in custom_nodes:
         app.add_node(node, html=(node.visit_html, node.depart_html))
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/static/logo.ico` & `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.ico`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/static/logo.pdf` & `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/static/logo.png` & `sphinx-asdf-0.2.0/sphinx_asdf/static/logo.png`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/static/sphinx_asdf.css` & `sphinx-asdf-0.2.0/sphinx_asdf/static/sphinx_asdf.css`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf/templates/schema.html` & `sphinx-asdf-0.2.0/sphinx_asdf/templates/schema.html`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf.egg-info/PKG-INFO` & `sphinx-asdf-0.2.0/sphinx_asdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sphinx-asdf
-Version: 0.1.4
+Version: 0.2.0
 Summary: Sphinx plugin for generating documentation from ASDF schemas
 Home-page: https://github.com/spacetelescope/sphinx-asdf
 Author: The ASDF Developers
 License: BSD-3-Clause
 Provides: sphinx_asdf
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Provides-Extra: tests
 License-File: LICENSE
 
 sphinx-asdf
 ===========
 
 .. image:: https://github.com/asdf-format/sphinx-asdf/workflows/CI/badge.svg
@@ -23,15 +23,15 @@
 Installation
 ------------
 
 To install the latest release on PyPI::
 
     $ pip install sphinx-asdf
 
-The latest development version is available from the ``master`` branch `on
+The latest development version is available from the ``main`` branch `on
 github`_. To clone the project:
 
 ::
 
     $ git clone https://github.com/asdf-format/sphinx-asdf
 
 To install:
```

### Comparing `sphinx-asdf-0.1.4/sphinx_asdf.egg-info/SOURCES.txt` & `sphinx-asdf-0.2.0/sphinx_asdf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 sphinx_asdf/md2rst.py
 sphinx_asdf/nodes.py
 sphinx_asdf.egg-info/PKG-INFO
 sphinx_asdf.egg-info/SOURCES.txt
 sphinx_asdf.egg-info/dependency_links.txt
 sphinx_asdf.egg-info/requires.txt
 sphinx_asdf.egg-info/top_level.txt
-sphinx_asdf/static/custom.css
 sphinx_asdf/static/logo.ico
 sphinx_asdf/static/logo.pdf
 sphinx_asdf/static/logo.png
 sphinx_asdf/static/sphinx_asdf.css
 sphinx_asdf/static/sphinx_asdf.js
 sphinx_asdf/templates/schema.html
 tests/conftest.py
```

### Comparing `sphinx-asdf-0.1.4/tests/coveragerc` & `sphinx-asdf-0.2.0/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `sphinx-asdf-0.1.4/tests/test_sphinx_asdf.py` & `sphinx-asdf-0.2.0/tests/test_sphinx_asdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,12 +88,12 @@
     app.builder.build_all()
 
     # Test each of the generated schema documents
     for name in ["foo", "bar", "core/baz"]:
         doctree_path = app.doctreedir / "generated" / f"{name}.doctree"
         doc = pickle.loads(doctree_path.read_bytes())
 
-        title = list(doc.traverse(nodes.title))[0]
+        title = list(doc.findall(nodes.title))[0]
         assert title.astext() == name
 
-        schema_top = list(doc.traverse(sa_nodes.schema_doc))
+        schema_top = list(doc.findall(sa_nodes.schema_doc))
         assert len(schema_top) > 0
```

### Comparing `sphinx-asdf-0.1.4/tox.ini` & `sphinx-asdf-0.2.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -5,81 +5,81 @@
 commands=
     pytest {posargs}
 
 [testenv:asdf-standard]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/asdf-format/asdf-standard
-    pip install asdf-standard[docs]
+    pip install ./asdf-standard[docs]
     sphinx-build asdf-standard/docs/source asdf-standard/docs/build
 
 [testenv:asdf]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/asdf-format/asdf
-    pip install asdf[docs]
+    pip install ./asdf[docs]
     sphinx-build asdf/docs asdf/docs/build
 
 [testenv:asdf-transform-schemas]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/asdf-format/asdf-transform-schemas
-    pip install asdf-transform-schemas[docs]
+    pip install ./asdf-transform-schemas[docs]
     sphinx-build asdf-transform-schemas/docs asdf-transform-schemas/docs/build
 
 [testenv:asdf-coordinates-schemas]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/asdf-format/asdf-coordinates-schemas
-    pip install asdf-coordinates-schemas[docs]
+    pip install ./asdf-coordinates-schemas[docs]
     sphinx-build asdf-coordinates-schemas/docs asdf-coordinates-schemas/docs/build
 
 [testenv:asdf-wcs-schemas]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/asdf-format/asdf-wcs-schemas
-    pip install asdf-wcs-schemas[docs]
+    pip install ./asdf-wcs-schemas[docs]
     sphinx-build asdf-wcs-schemas/docs asdf-wcs-schemas/docs/build
 
 [testenv:asdf-astropy]
 changedir={envtmpdir}
 deps=
     sphinx
-whitelist_externals=
+allowlist_externals=
     git
 commands=
     git clone https://github.com/astropy/asdf-astropy
-    pip install asdf-astropy[docs]
+    pip install ./asdf-astropy[docs]
     sphinx-build asdf-astropy/docs asdf-astropy/docs/build
 
 [testenv:twine]
 deps=
     twine
 commands=
-    twine check {distdir}/*
+    twine check {work_dir}/{package_env}/dist/*
 
 [testenv:checkdocs]
 deps=
     collective.checkdocs
     pygments
 commands=
     python setup.py checkdocs
@@ -98,8 +98,7 @@
     sphinx
     codecov
     coverage
 commands=
     coverage run --source=sphinx_asdf --rcfile={toxinidir}/tests/coveragerc -m pytest
     coverage report -m
     codecov -e TOXENV
-passenv= TOXENV CI TRAVIS TRAVIS_* CODECOV_*
```

