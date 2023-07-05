# Comparing `tmp/code_var-0.1.1.tar.gz` & `tmp/code_var-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_var-0.1.1.tar", last modified: Thu Sep 29 09:40:34 2022, max compression
+gzip compressed data, was "code_var-0.1.2.tar", last modified: Wed Jul  5 06:36:40 2023, max compression
```

## Comparing `code_var-0.1.1.tar` & `code_var-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2022-09-29 09:40:34.534677 code_var-0.1.1/
--rw-r--r--   0 caolipin   (501) staff       (20)      455 2022-09-29 09:40:34.534545 code_var-0.1.1/PKG-INFO
--rw-r--r--   0 caolipin   (501) staff       (20)      262 2022-09-29 09:33:16.000000 code_var-0.1.1/README.md
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2022-09-29 09:40:34.533495 code_var-0.1.1/code_var/
--rw-r--r--   0 caolipin   (501) staff       (20)        0 2022-09-27 15:00:10.000000 code_var-0.1.1/code_var/__init__.py
--rw-r--r--   0 caolipin   (501) staff       (20)      441 2022-09-28 07:09:17.000000 code_var-0.1.1/code_var/cli.py
-drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2022-09-29 09:40:34.534388 code_var-0.1.1/code_var.egg-info/
--rw-r--r--   0 caolipin   (501) staff       (20)      455 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/PKG-INFO
--rw-r--r--   0 caolipin   (501) staff       (20)      249 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/SOURCES.txt
--rw-r--r--   0 caolipin   (501) staff       (20)        1 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/dependency_links.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       41 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/entry_points.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       41 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/requires.txt
--rw-r--r--   0 caolipin   (501) staff       (20)        9 2022-09-29 09:40:34.000000 code_var-0.1.1/code_var.egg-info/top_level.txt
--rw-r--r--   0 caolipin   (501) staff       (20)       38 2022-09-29 09:40:34.534721 code_var-0.1.1/setup.cfg
--rw-r--r--   0 caolipin   (501) staff       (20)      871 2022-09-29 09:40:30.000000 code_var-0.1.1/setup.py
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.641143 code_var-0.1.2/
+-rw-r--r--   0 caolipin   (501) staff       (20)      451 2023-07-05 06:36:40.640964 code_var-0.1.2/PKG-INFO
+-rw-r--r--   0 caolipin   (501) staff       (20)      261 2023-07-05 06:27:38.000000 code_var-0.1.2/README.md
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.639460 code_var-0.1.2/code_var/
+-rw-r--r--   0 caolipin   (501) staff       (20)        0 2022-09-27 15:00:10.000000 code_var-0.1.2/code_var/__init__.py
+-rw-r--r--   0 caolipin   (501) staff       (20)      441 2023-07-05 06:32:34.000000 code_var-0.1.2/code_var/cli.py
+drwxr-xr-x   0 caolipin   (501) staff       (20)        0 2023-07-05 06:36:40.640578 code_var-0.1.2/code_var.egg-info/
+-rw-r--r--   0 caolipin   (501) staff       (20)      451 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/PKG-INFO
+-rw-r--r--   0 caolipin   (501) staff       (20)      249 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/SOURCES.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)        1 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/dependency_links.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       40 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/entry_points.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       41 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/requires.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)        9 2023-07-05 06:36:40.000000 code_var-0.1.2/code_var.egg-info/top_level.txt
+-rw-r--r--   0 caolipin   (501) staff       (20)       38 2023-07-05 06:36:40.641189 code_var-0.1.2/setup.cfg
+-rw-r--r--   0 caolipin   (501) staff       (20)      867 2023-07-05 06:27:38.000000 code_var-0.1.2/setup.py
```

### Comparing `code_var-0.1.1/setup.py` & `code_var-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     [
         "bs4==0.0.1",
         "requests==2.28.1",
         "typer==0.6.1"
     ]
 
 entry_points = \
-    {'console_scripts': ['var = code_var.cli:run']}
+    {'console_scripts': ['vn = code_var.cli:run']}
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_kwargs = {
     'name': 'code_var',
-    'version': '0.1.1',
-    'description': '"code-var is tools for varname in shell"',
+    'version': '0.1.2',
+    'description': '"code-var is tools for varname in cmd"',
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
-    'author': 'LiPinCao',
+    'author': 'JackCCC',
     'maintainer': None,
     'maintainer_email': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.6.2,<4.0.0',
```

