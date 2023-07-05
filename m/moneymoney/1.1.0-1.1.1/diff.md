# Comparing `tmp/moneymoney-1.1.0.tar.gz` & `tmp/moneymoney-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneymoney-1.1.0.tar", last modified: Sun Apr  9 16:44:12 2023, max compression
+gzip compressed data, was "moneymoney-1.1.1.tar", last modified: Wed Jul  5 14:43:57 2023, max compression
```

## Comparing `moneymoney-1.1.0.tar` & `moneymoney-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.575771 moneymoney-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 16:43:59.000000 moneymoney-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 16:43:59.000000 moneymoney-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-09 16:44:12.575771 moneymoney-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-09 16:43:59.000000 moneymoney-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.571771 moneymoney-1.1.0/moneymoney/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/currency_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/money.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-09 16:43:59.000000 moneymoney-1.1.0/moneymoney/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:44:12.575771 moneymoney-1.1.0/moneymoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:44:12.000000 moneymoney-1.1.0/moneymoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-09 16:43:59.000000 moneymoney-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-09 16:44:12.575771 moneymoney-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:43:57.506716 moneymoney-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 14:43:44.000000 moneymoney-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 14:43:44.000000 moneymoney-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-05 14:43:57.506716 moneymoney-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-05 14:43:44.000000 moneymoney-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:43:57.506716 moneymoney-1.1.1/moneymoney/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:43:44.000000 moneymoney-1.1.1/moneymoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 14:43:44.000000 moneymoney-1.1.1/moneymoney/currency_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 14:43:44.000000 moneymoney-1.1.1/moneymoney/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-05 14:43:44.000000 moneymoney-1.1.1/moneymoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-05 14:43:44.000000 moneymoney-1.1.1/moneymoney/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:43:57.506716 moneymoney-1.1.1/moneymoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-05 14:43:57.000000 moneymoney-1.1.1/moneymoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-05 14:43:57.000000 moneymoney-1.1.1/moneymoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:43:57.000000 moneymoney-1.1.1/moneymoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-05 14:43:57.000000 moneymoney-1.1.1/moneymoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 14:43:57.000000 moneymoney-1.1.1/moneymoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-05 14:43:44.000000 moneymoney-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 14:43:57.506716 moneymoney-1.1.1/setup.cfg
```

### Comparing `moneymoney-1.1.0/LICENSE` & `moneymoney-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moneymoney-1.1.0/moneymoney/money.py` & `moneymoney-1.1.1/moneymoney/money.py`

 * *Files identical despite different names*

### Comparing `moneymoney-1.1.0/pyproject.toml` & `moneymoney-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
 ]
 # Make sure this matches the keywords in GitHub
 keywords = ["currency", "python", "money", "finance"]
-version = "1.1.0"
+version = "1.1.1"
 # Minumum supported version
 # If supporting newer versions, update ->  CI and classifiers
 # If minimum supported version changes, update -> CI, coverage, lint, release and classifiers.
 requires-python = ">=3.9.0"
 
 # Always try to be compatible with these versions and above
 dependencies = []
```

