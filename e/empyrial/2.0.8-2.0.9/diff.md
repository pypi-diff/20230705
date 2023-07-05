# Comparing `tmp/empyrial-2.0.8.tar.gz` & `tmp/empyrial-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.8.tar", last modified: Wed Jul  5 02:58:05 2023, max compression
+gzip compressed data, was "empyrial-2.0.9.tar", last modified: Wed Jul  5 03:04:05 2023, max compression
```

## Comparing `empyrial-2.0.8.tar` & `empyrial-2.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:58:05.808254 empyrial-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:57:23.000000 empyrial-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 02:57:23.000000 empyrial-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 02:58:05.812254 empyrial-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/empyrial/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 02:57:23.000000 empyrial-2.0.8/src/empyrial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:57:23.000000 empyrial-2.0.8/src/empyrial/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:58:05.808254 empyrial-2.0.8/src/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 02:58:05.000000 empyrial-2.0.8/src/empyrial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 03:04:05.947246 empyrial-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 03:03:19.000000 empyrial-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 03:03:19.000000 empyrial-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 03:04:05.947246 empyrial-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/empyrial/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 03:03:19.000000 empyrial-2.0.9/src/empyrial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 03:03:19.000000 empyrial-2.0.9/src/empyrial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:04:05.947246 empyrial-2.0.9/src/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 03:04:05.000000 empyrial-2.0.9/src/empyrial.egg-info/top_level.txt
```

### Comparing `empyrial-2.0.8/README.md` & `empyrial-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `empyrial-2.0.8/setup.cfg` & `empyrial-2.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = empyrial
-version = 2.0.8
+version = 2.0.9
 description = An Open Source Portfolio Management Framework for Everyone 投资组合管理
 url = https://github.com/ssantoshp/Empyrial
 long_description_content_type = text/markdown
 long_descript = # Empyrial
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
```

### Comparing `empyrial-2.0.8/src/empyrial/main.py` & `empyrial-2.0.9/src/empyrial/main.py`

 * *Files identical despite different names*

