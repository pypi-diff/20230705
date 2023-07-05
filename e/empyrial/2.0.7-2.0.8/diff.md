# Comparing `tmp/empyrial-2.0.7.tar.gz` & `tmp/empyrial-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.7.tar", last modified: Wed Jul  5 02:46:51 2023, max compression
+gzip compressed data, was "empyrial-2.0.8.tar", last modified: Wed Jul  5 02:58:05 2023, max compression
```

## Comparing `empyrial-2.0.7.tar` & `empyrial-2.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:46:51.622385 empyrial-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:46:11.000000 empyrial-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 02:46:11.000000 empyrial-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-05 02:46:51.622385 empyrial-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.618385 empyrial-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/src/empyrial/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:46:11.000000 empyrial-2.0.7/src/empyrial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:46:11.000000 empyrial-2.0.7/src/empyrial/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/src/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:58:05.808254 empyrial-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:57:23.000000 empyrial-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 02:57:23.000000 empyrial-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 02:58:05.812254 empyrial-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/empyrial/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 02:57:23.000000 empyrial-2.0.8/src/empyrial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:57:23.000000 empyrial-2.0.8/src/empyrial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/top_level.txt
```

### Comparing `empyrial-2.0.7/README.md` & `empyrial-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `empyrial-2.0.7/setup.cfg` & `empyrial-2.0.8/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 [metadata]
 name = empyrial
-version = 2.0.7
+version = 2.0.8
 description = An Open Source Portfolio Management Framework for Everyone 投资组合管理
 url = https://github.com/ssantoshp/Empyrial
 long_description_content_type = text/markdown
 long_descript = # Empyrial
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Developers
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.0
+install_requires = 
+	numpy
+	matplotlib
+	datetime
+	empyrical
+	quantstats
+	yfinance
+	ipython
+	fpdf
+	pyportfolioopt
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	gha_python_packaging_demo =empyrial.main:entry_point
```

### Comparing `empyrial-2.0.7/src/empyrial/main.py` & `empyrial-2.0.8/src/empyrial/main.py`

 * *Files identical despite different names*

