# Comparing `tmp/empyrial-2.0.4.tar.gz` & `tmp/empyrial-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.4.tar", last modified: Wed Jul  5 01:48:53 2023, max compression
+gzip compressed data, was "empyrial-2.0.5.tar", last modified: Wed Jul  5 02:05:00 2023, max compression
```

## Comparing `empyrial-2.0.4.tar` & `empyrial-2.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 01:48:53.542208 empyrial-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 01:48:44.000000 empyrial-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:48:53.542208 empyrial-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 01:48:44.000000 empyrial-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 01:48:44.000000 empyrial-2.0.4/src/empyrial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.770971 empyrial-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 02:05:00.766971 empyrial-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 02:04:53.000000 empyrial-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.766971 empyrial-2.0.5/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-05 02:05:00.000000 empyrial-2.0.5/empyrial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 02:05:00.770971 empyrial-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 02:04:53.000000 empyrial-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:05:00.766971 empyrial-2.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 02:04:53.000000 empyrial-2.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 02:04:53.000000 empyrial-2.0.5/src/empyrial.py
```

### Comparing `empyrial-2.0.4/PKG-INFO` & `empyrial-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyrial
-Version: 2.0.4
+Version: 2.0.5
 Summary: An Open Source Portfolio Management Framework for Everyone 投资组合管理
 Home-page: https://github.com/ssantoshp/Empyrial
 Author: Santosh Passoubady
 Author-email: santoshpassoubady@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `empyrial-2.0.4/README.md` & `empyrial-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `empyrial-2.0.4/empyrial.egg-info/PKG-INFO` & `empyrial-2.0.5/empyrial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyrial
-Version: 2.0.4
+Version: 2.0.5
 Summary: An Open Source Portfolio Management Framework for Everyone 投资组合管理
 Home-page: https://github.com/ssantoshp/Empyrial
 Author: Santosh Passoubady
 Author-email: santoshpassoubady@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `empyrial-2.0.4/setup.py` & `empyrial-2.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name='empyrial',
-    version='2.0.4',
+    version='2.0.5',
     description='An Open Source Portfolio Management Framework for Everyone 投资组合管理',
-    py_modules=['src/empyrial'],
+    py_modules=['src.empyrial'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ssantoshp/Empyrial',
     author="Santosh Passoubady",
     author_email="santoshpassoubady@gmail.com",
     license='MIT',
     install_requires=[
```

### Comparing `empyrial-2.0.4/src/empyrial.py` & `empyrial-2.0.5/src/empyrial.py`

 * *Files identical despite different names*

