# Comparing `tmp/code_var-0.1.2.tar.gz` & `tmp/code_var-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_var-0.1.2.tar", last modified: Wed Jul  5 06:36:40 2023, max compression
+gzip compressed data, was "code_var-0.1.3.tar", last modified: Wed Jul  5 06:40:10 2023, max compression
```

## Comparing `code_var-0.1.2.tar` & `code_var-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.641143 code_var-0.1.2/
--rw-r--r--   0 caolipin   (501) staff       (20)      451 2023-07-05 06:36:40.640964 code_var-0.1.2/PKG-INFO
--rw-r--r--   0 caolipin   (501) staff       (20)      261 2023-07-05 06:27:38.000000 code_var-0.1.2/README.md
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.639460 code_var-0.1.2/code_var/
--rw-r--r--   0 caolipin   (501) staff       (20)        0 2022-09-27 15:00:10.000000 code_var-0.1.2/code_var/__init__.py
--rw-r--r--   0 caolipin   (501) staff       (20)      441 2023-07-05 06:32:34.000000 code_var-0.1.2/code_var/cli.py
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.640578 code_var-0.1.2/code_var.egg-info/
--rw-r--r--   0 caolipin   (501) staff       (20)      451 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/PKG-INFO
--rw-r--r--   0 caolipin   (501) staff       (20)      249 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/SOURCES.txt
--rw-r--r--   0 caolipin   (501) staff       (20)        1 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/dependency_links.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       40 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/entry_points.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       41 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/requires.txt
--rw-r--r--   0 caolipin   (501) staff       (20)        9 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/top_level.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       38 2023-07-05 06:36:40.641189 code_var-0.1.2/setup.cfg
--rw-r--r--   0 caolipin   (501) staff       (20)      867 2023-07-05 06:27:38.000000 code_var-0.1.2/setup.py
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:40:10.474638 code_var-0.1.3/
+-rw-r--r--   0 caolipin   (501) staff       (20)      450 2023-07-05 06:40:10.474485 code_var-0.1.3/PKG-INFO
+-rw-r--r--   0 caolipin   (501) staff       (20)      260 2023-07-05 06:38:28.000000 code_var-0.1.3/README.md
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:40:10.473436 code_var-0.1.3/code_var/
+-rw-r--r--   0 caolipin   (501) staff       (20)        0 2022-09-27 15:00:10.000000 code_var-0.1.3/code_var/__init__.py
+-rw-r--r--   0 caolipin   (501) staff       (20)      441 2023-07-05 06:32:34.000000 code_var-0.1.3/code_var/cli.py
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:40:10.474314 code_var-0.1.3/code_var.egg-info/
+-rw-r--r--   0 caolipin   (501) staff       (20)      450 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/PKG-INFO
+-rw-r--r--   0 caolipin   (501) staff       (20)      249 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/SOURCES.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)        1 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/dependency_links.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       40 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/entry_points.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       41 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/requires.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)        9 2023-07-05 06:40:10.000000 code_var-0.1.3/code_var.egg-info/top_level.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       38 2023-07-05 06:40:10.474720 code_var-0.1.3/setup.cfg
+-rw-r--r--   0 caolipin   (501) staff       (20)      867 2023-07-05 06:39:48.000000 code_var-0.1.3/setup.py
```

### Comparing `code_var-0.1.2/setup.py` & `code_var-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     {'console_scripts': ['vn = code_var.cli:run']}
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_kwargs = {
     'name': 'code_var',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '"code-var is tools for varname in cmd"',
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     'author': 'JackCCC',
     'maintainer': None,
     'maintainer_email': None,
     'packages': packages,
```

