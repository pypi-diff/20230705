# Comparing `tmp/empyrial-2.0.3.tar.gz` & `tmp/empyrial-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyrial-2.0.3.tar", last modified: Wed Jul  5 00:22:26 2023, max compression
+gzip compressed data, was "empyrial-2.0.4.tar", last modified: Wed Jul  5 01:48:53 2023, max compression
```

## Comparing `empyrial-2.0.3.tar` & `empyrial-2.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:22:26.088117 empyrial-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 00:22:26.088117 empyrial-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 00:22:17.000000 empyrial-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:22:26.088117 empyrial-2.0.3/empyrial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 00:22:26.000000 empyrial-2.0.3/empyrial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 00:22:26.000000 empyrial-2.0.3/empyrial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:22:26.000000 empyrial-2.0.3/empyrial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 00:22:26.000000 empyrial-2.0.3/empyrial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 00:22:26.000000 empyrial-2.0.3/empyrial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:22:26.088117 empyrial-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-05 00:22:17.000000 empyrial-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 01:48:53.542208 empyrial-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 01:48:44.000000 empyrial-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/empyrial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 01:48:53.000000 empyrial-2.0.4/empyrial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:48:53.542208 empyrial-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 01:48:44.000000 empyrial-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:48:53.542208 empyrial-2.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    36808 2023-07-05 01:48:44.000000 empyrial-2.0.4/src/empyrial.py
```

### Comparing `empyrial-2.0.3/PKG-INFO` & `empyrial-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyrial
-Version: 2.0.3
+Version: 2.0.4
 Summary: An Open Source Portfolio Management Framework for Everyone 投资组合管理
 Home-page: https://github.com/ssantoshp/Empyrial
 Author: Santosh Passoubady
 Author-email: santoshpassoubady@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `empyrial-2.0.3/README.md` & `empyrial-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `empyrial-2.0.3/empyrial.egg-info/PKG-INFO` & `empyrial-2.0.4/empyrial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyrial
-Version: 2.0.3
+Version: 2.0.4
 Summary: An Open Source Portfolio Management Framework for Everyone 投资组合管理
 Home-page: https://github.com/ssantoshp/Empyrial
 Author: Santosh Passoubady
 Author-email: santoshpassoubady@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `empyrial-2.0.3/setup.py` & `empyrial-2.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name='empyrial',
-    version='2.0.3',
+    version='2.0.4',
     description='An Open Source Portfolio Management Framework for Everyone 投资组合管理',
-    py_modules=['empyrial'],
+    py_modules=['src/empyrial'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ssantoshp/Empyrial',
     author="Santosh Passoubady",
     author_email="santoshpassoubady@gmail.com",
     license='MIT',
     install_requires=[
```

