# Comparing `tmp/empyrial-2.0.5.tar.gz` & `tmp/empyrial-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.5.tar", last modified: Wed Jul  5 02:05:00 2023, max compression
+gzip compressed data, was "empyrial-2.0.7.tar", last modified: Wed Jul  5 02:46:51 2023, max compression
```

## Comparing `empyrial-2.0.5.tar` & `empyrial-2.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.770971 empyrial-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 02:05:00.766971 empyrial-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:04:53.000000 empyrial-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.766971 empyrial-2.0.5/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 02:05:00.770971 empyrial-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 02:04:53.000000 empyrial-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.766971 empyrial-2.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 02:04:53.000000 empyrial-2.0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:04:53.000000 empyrial-2.0.5/src/empyrial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:46:51.622385 empyrial-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:46:11.000000 empyrial-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 02:46:11.000000 empyrial-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-05 02:46:51.622385 empyrial-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.618385 empyrial-2.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/src/empyrial/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:46:11.000000 empyrial-2.0.7/src/empyrial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:46:11.000000 empyrial-2.0.7/src/empyrial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:46:51.622385 empyrial-2.0.7/src/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 02:46:51.000000 empyrial-2.0.7/src/empyrial.egg-info/top_level.txt
```

### Comparing `empyrial-2.0.5/PKG-INFO` & `empyrial-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: empyrial
-Version: 2.0.5
-Summary: An Open Source Portfolio Management Framework for Everyone 投资组合管理
-Home-page: https://github.com/ssantoshp/Empyrial
-Author: Santosh Passoubady
-Author-email: santoshpassoubady@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-
 
 # By Investors, For Investors.
 <br><br><br><br>
 <div align="center">
 <img src="https://user-images.githubusercontent.com/61618641/120909011-98f8a180-c670-11eb-8844-2d423ba3fa9c.png"/>
 <br><br><br><br><br><br>
```

### Comparing `empyrial-2.0.5/src/empyrial.py` & `empyrial-2.0.7/src/empyrial/main.py`

 * *Files identical despite different names*

