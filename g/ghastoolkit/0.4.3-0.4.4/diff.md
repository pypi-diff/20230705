# Comparing `tmp/ghastoolkit-0.4.3.tar.gz` & `tmp/ghastoolkit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.3.tar", last modified: Fri Jun 30 17:52:34 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.4.tar", last modified: Wed Jul  5 10:53:35 2023, max compression
```

## Comparing `ghastoolkit-0.4.3.tar` & `ghastoolkit-0.4.4.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.567422 ghastoolkit-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.567422 ghastoolkit-0.4.3/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.567422 ghastoolkit-0.4.3/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.567422 ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.567422 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-30 17:52:34.000000 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-30 17:52:34.000000 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:52:34.000000 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 17:52:34.000000 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-30 17:52:34.000000 ghastoolkit-0.4.3/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:52:34.571422 ghastoolkit-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-30 17:52:05.000000 ghastoolkit-0.4.3/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.172244 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.168244 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:53:35.000000 ghastoolkit-0.4.4/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:53:35.176245 ghastoolkit-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-05 10:52:59.000000 ghastoolkit-0.4.4/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.3/LICENSE` & `ghastoolkit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/PKG-INFO` & `ghastoolkit-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.3/README.md` & `ghastoolkit-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/pyproject.toml` & `ghastoolkit-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.4/src/ghastoolkit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.4/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.4/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/octokit.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Optional, Union
 from dataclasses import field, is_dataclass
 
 from requests import Session
 from ratelimit import limits, sleep_and_retry
 
 from ghastoolkit.octokit.github import GitHub, Repository
+from ghastoolkit.octokit.graphql import QUERIES
 
 
 # Assume REST requests are being done by a GitHub Token, not
 # a GitHub App which has a higher limit
 # https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=2022-11-28#rate-limiting
 REST_MAX_CALLS = 80  # ~5000 per hour
 
@@ -257,17 +258,16 @@
         self.session = Session()
         self.cursor = ""
         # https://docs.github.com/en/rest/overview/authenticating-to-the-rest-api
         self.session.headers = {
             "Accept": "application/vnd.github.hawkgirl-preview+json",
             "Authorization": f"token {GitHub.token}",
         }
-        self.queries = {}
-
-        self.loadQueries(DEFAULT_GRAPHQL_PATHS)
+        # load in default hardcoded queries
+        self.queries = QUERIES
 
     def query(self, name: str, options: dict[str, Any] = {}) -> dict:
         logger.debug(f"Loading Query by Name :: {name}")
         query_content = self.queries.get(name)
 
         if not query_content:
             raise Exception(f"Failed to load GraphQL query :: {name}")
```

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.4/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.4/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.4/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.4/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.3
+Version: 0.4.4
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.3/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.4/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/ghastoolkit/octokit/clearlydefined.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
 src/ghastoolkit/octokit/secretscanning.py
+src/ghastoolkit/octokit/graphql/__init__.py
 src/ghastoolkit/secretscanning/__init__.py
 src/ghastoolkit/secretscanning/secretalerts.py
 src/ghastoolkit/supplychain/__init__.py
 src/ghastoolkit/supplychain/advisories.py
 src/ghastoolkit/supplychain/dependencies.py
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
```

### Comparing `ghastoolkit-0.4.3/tests/test_codeql_dataext.py` & `ghastoolkit-0.4.4/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_codeqldb.py` & `ghastoolkit-0.4.4/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_codescanning.py` & `ghastoolkit-0.4.4/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_default.py` & `ghastoolkit-0.4.4/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_dependencies.py` & `ghastoolkit-0.4.4/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_depgraph.py` & `ghastoolkit-0.4.4/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_github.py` & `ghastoolkit-0.4.4/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_licenses.py` & `ghastoolkit-0.4.4/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.3/tests/test_octokit.py` & `ghastoolkit-0.4.4/tests/test_secretscanning.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-from dataclasses import dataclass, is_dataclass
 import unittest
 
-from ghastoolkit.octokit.octokit import OctoItem, Octokit, loadOctoItem
 from ghastoolkit.octokit.github import GitHub
+from ghastoolkit.octokit.secretscanning import SecretAlert, SecretScanning
 
 
-class TestOctokit(unittest.TestCase):
+class TestSecretScanning(unittest.TestCase):
     def setUp(self) -> None:
-        GitHub.init(repository="GeekMasher/ghastoolkit@main")
+        GitHub.init("GeekMasher/ghastoolkit")
         return super().setUp()
 
-    def test_route(self):
-        route = Octokit.route(
-            "/repos/{owner}/{repo}/secret-scanning/alerts", GitHub.repository
-        )
-        self.assertEqual(
-            route,
-            "https://api.github.com/repos/GeekMasher/ghastoolkit/secret-scanning/alerts",
-        )
+    def test_secretscanning_default(self):
+        return
 
-
-@dataclass
-class Example(OctoItem):
-    number: int
-
-
-class TestLoadOctoItem(unittest.TestCase):
-    def test_load(self):
-        item = loadOctoItem(Example, {"number": 5})
-
-        self.assertTrue(isinstance(item, Example))
-        self.assertTrue(is_dataclass(item))
-
-        self.assertEqual(item.number, 5)
+    def test_codescanning_default(self):
+        ss = SecretScanning()
+        self.assertEqual(ss.repository.display(), "GeekMasher/ghastoolkit")
+
+        ss = SecretScanning(GitHub.repository)
+        self.assertEqual(ss.repository.display(), "GeekMasher/ghastoolkit")
+
+        GitHub.init("Sample/Repo")
+        ss = SecretScanning(GitHub.repository)
+        self.assertEqual(ss.repository.display(), "Sample/Repo")
+
+
+class TestSecretAlert(unittest.TestCase):
+    def test_load_alert(self):
+        data = {
+            "number": 23,
+            "created_at": "2020-11-06T18:18:30Z",
+            "state": "open",
+            "secret_type": "mailchimp_api_key",
+            "secret_type_display_name": "Mailchimp API Key",
+            "secret": "ABCDEFG",
+        }
+        alert = SecretAlert(**data)
+        self.assertEqual(alert.number, 23)
+        self.assertEqual(alert.state, "open")
+        self.assertEqual(alert.secret_type, "mailchimp_api_key")
+        self.assertEqual(alert.secret, "ABCDEFG")
```

### Comparing `ghastoolkit-0.4.3/tests/test_secretscanning.py` & `ghastoolkit-0.4.4/tests/test_octokit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,52 @@
+from dataclasses import dataclass, is_dataclass
 import unittest
 
+from ghastoolkit.octokit.octokit import OctoItem, Octokit, GraphQLRequest, loadOctoItem
 from ghastoolkit.octokit.github import GitHub
-from ghastoolkit.octokit.secretscanning import SecretAlert, SecretScanning
 
 
-class TestSecretScanning(unittest.TestCase):
+class TestOctokit(unittest.TestCase):
     def setUp(self) -> None:
-        GitHub.init("GeekMasher/ghastoolkit")
+        GitHub.init(repository="GeekMasher/ghastoolkit@main")
         return super().setUp()
 
-    def test_secretscanning_default(self):
-        return
+    def test_route(self):
+        route = Octokit.route(
+            "/repos/{owner}/{repo}/secret-scanning/alerts", GitHub.repository
+        )
+        self.assertEqual(
+            route,
+            "https://api.github.com/repos/GeekMasher/ghastoolkit/secret-scanning/alerts",
+        )
+
+
+@dataclass
+class Example(OctoItem):
+    number: int
+
+
+class TestLoadOctoItem(unittest.TestCase):
+    def test_load(self):
+        item = loadOctoItem(Example, {"number": 5})
+
+        self.assertTrue(isinstance(item, Example))
+        self.assertTrue(is_dataclass(item))
+
+        self.assertEqual(item.number, 5)
+
+class TestOctokitGraphQL(unittest.TestCase):
+    def setUp(self) -> None:
+        GitHub.init(repository="GeekMasher/ghastoolkit@main")
+        return super().setUp()
+
+    def test_loading_defaults(self):
+        gql = GraphQLRequest()
+        # load 2 default queries
+        self.assertEqual(len(gql.queries.keys()), 2)
+
+        query1 = gql.queries.get("GetDependencyAlerts")
+        self.assertIsNotNone(query1)
+        
+        query2 = gql.queries.get("GetDependencyInfo")
+        self.assertIsNotNone(query2)
 
-    def test_codescanning_default(self):
-        ss = SecretScanning()
-        self.assertEqual(ss.repository.display(), "GeekMasher/ghastoolkit")
-
-        ss = SecretScanning(GitHub.repository)
-        self.assertEqual(ss.repository.display(), "GeekMasher/ghastoolkit")
-
-        GitHub.init("Sample/Repo")
-        ss = SecretScanning(GitHub.repository)
-        self.assertEqual(ss.repository.display(), "Sample/Repo")
-
-
-class TestSecretAlert(unittest.TestCase):
-    def test_load_alert(self):
-        data = {
-            "number": 23,
-            "created_at": "2020-11-06T18:18:30Z",
-            "state": "open",
-            "secret_type": "mailchimp_api_key",
-            "secret_type_display_name": "Mailchimp API Key",
-            "secret": "ABCDEFG",
-        }
-        alert = SecretAlert(**data)
-        self.assertEqual(alert.number, 23)
-        self.assertEqual(alert.state, "open")
-        self.assertEqual(alert.secret_type, "mailchimp_api_key")
-        self.assertEqual(alert.secret, "ABCDEFG")
```

