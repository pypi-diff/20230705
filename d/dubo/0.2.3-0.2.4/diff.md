# Comparing `tmp/dubo-0.2.3.tar.gz` & `tmp/dubo-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubo-0.2.3.tar", max compression
+gzip compressed data, was "dubo-0.2.4.tar", max compression
```

## Comparing `dubo-0.2.3.tar` & `dubo-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.3/LICENSE
--rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.3/README.md
--rw-r--r--   0        0        0      194 2023-01-05 10:20:42.201716 dubo-0.2.3/dubo/__init__.py
--rw-r--r--   0        0        0      119 2023-01-09 02:17:46.409227 dubo-0.2.3/dubo/__version__.py
--rw-r--r--   0        0        0     3311 2023-01-09 02:08:50.349001 dubo-0.2.3/dubo/ask_dubo.py
--rw-r--r--   0        0        0      358 2023-01-09 02:08:50.349275 dubo-0.2.3/dubo/config.py
--rw-r--r--   0        0        0      556 2023-01-09 02:18:02.979890 dubo-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 dubo-0.2.3/setup.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 dubo-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.4/LICENSE
+-rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.4/README.md
+-rw-r--r--   0        0        0      194 2023-01-05 10:20:42.201716 dubo-0.2.4/dubo/__init__.py
+-rw-r--r--   0        0        0      119 2023-07-05 20:05:03.562011 dubo-0.2.4/dubo/__version__.py
+-rw-r--r--   0        0        0     3311 2023-07-05 20:08:11.607878 dubo-0.2.4/dubo/ask_dubo.py
+-rw-r--r--   0        0        0      336 2023-07-05 20:04:00.514700 dubo-0.2.4/dubo/config.py
+-rw-r--r--   0        0        0      556 2023-07-05 20:18:48.836736 dubo-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 dubo-0.2.4/setup.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 dubo-0.2.4/PKG-INFO
```

### Comparing `dubo-0.2.3/LICENSE` & `dubo-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dubo-0.2.3/dubo/ask_dubo.py` & `dubo-0.2.4/dubo/ask_dubo.py`

 * *Files identical despite different names*

### Comparing `dubo-0.2.3/pyproject.toml` & `dubo-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dubo"
-version = "0.2.3"
+version = "0.2.4"
 description = "Analytics made simple"
 authors = ["Andrew Duberstein <ajduberstein@gmail.com>", "Andrew Duberstein <duber@mercator.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dubo-0.2.3/setup.py` & `dubo-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dubo',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'Analytics made simple',
     'long_description': 'dubo\n====\n\ndubo is a client for running LLMs against DataFrames and other 2D data.\n\nIt is currently in an alpha release and not yet ready for use in production pipelines.\n',
     'author': 'Andrew Duberstein',
     'author_email': 'ajduberstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dubo-0.2.3/PKG-INFO` & `dubo-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dubo
-Version: 0.2.3
+Version: 0.2.4
 Summary: Analytics made simple
 License: MIT
 Author: Andrew Duberstein
 Author-email: ajduberstein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

