# Comparing `tmp/agixtsdk-0.0.7.tar.gz` & `tmp/agixtsdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixtsdk-0.0.7.tar", last modified: Sat Jul  1 05:25:04 2023, max compression
+gzip compressed data, was "agixtsdk-0.0.8.tar", last modified: Wed Jul  5 15:31:20 2023, max compression
```

## Comparing `agixtsdk-0.0.7.tar` & `agixtsdk-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.786227 agixtsdk-0.0.7/agixtsdk/
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/agixtsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/agixtsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 05:25:04.000000 agixtsdk-0.0.7/agixtsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 05:25:04.790227 agixtsdk-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-01 05:24:52.000000 agixtsdk-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.283160 agixtsdk-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/agixtsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/agixtsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:31:20.279160 agixtsdk-0.0.8/agixtsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:31:20.000000 agixtsdk-0.0.8/agixtsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:31:20.283160 agixtsdk-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 15:31:10.000000 agixtsdk-0.0.8/setup.py
```

### Comparing `agixtsdk-0.0.7/LICENSE` & `agixtsdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `agixtsdk-0.0.7/PKG-INFO` & `agixtsdk-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1
-Name: agixtsdk
-Version: 0.0.7
-Summary: The AGiXT SDK for Python.
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AGiXT SDK for Python
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
 [![Logo](https://josh-xt.github.io/AGiXT/images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 This repository is for the [AGiXT](https://github.com/Josh-XT/AGiXT) SDK for Python.
 
 ## Installation
 ```bash
 pip install agixtsdk
 ```
 
 ## Usage
+
+```python
+from agixtsdk import AGiXTSDK
+
+base_uri = "http://localhost:7437"
+api_key = "your_agixt_api_key"
+
+ApiClient = AGiXTSDK(base_uri=base_uri, api_key=api_key)
+```
+
 Check out the AGiXT [Examples and Tests Notebook](https://github.com/Josh-XT/AGiXT/blob/main/tests/tests.ipynb) for examples of how to use the AGiXT SDK for Python.
 
 ## More Documentation
 Want to know more about AGiXT?  Check out our [documentation](https://josh-xt.github.io/AGiXT/) or [GitHub](https://github.com/Josh-XT/AGiXT) page.
```

### Comparing `agixtsdk-0.0.7/README.md` & `agixtsdk-0.0.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,38 @@
+Metadata-Version: 2.1
+Name: agixtsdk
+Version: 0.0.8
+Summary: The AGiXT SDK for Python.
+Author: Josh XT
+Author-email: josh@devxt.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AGiXT SDK for Python
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
 [![Logo](https://josh-xt.github.io/AGiXT/images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 This repository is for the [AGiXT](https://github.com/Josh-XT/AGiXT) SDK for Python.
 
 ## Installation
 ```bash
 pip install agixtsdk
 ```
 
 ## Usage
+
+```python
+from agixtsdk import AGiXTSDK
+
+base_uri = "http://localhost:7437"
+api_key = "your_agixt_api_key"
+
+ApiClient = AGiXTSDK(base_uri=base_uri, api_key=api_key)
+```
+
 Check out the AGiXT [Examples and Tests Notebook](https://github.com/Josh-XT/AGiXT/blob/main/tests/tests.ipynb) for examples of how to use the AGiXT SDK for Python.
 
 ## More Documentation
 Want to know more about AGiXT?  Check out our [documentation](https://josh-xt.github.io/AGiXT/) or [GitHub](https://github.com/Josh-XT/AGiXT) page.
```

### Comparing `agixtsdk-0.0.7/agixtsdk.egg-info/PKG-INFO` & `agixtsdk-0.0.8/agixtsdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixtsdk
-Version: 0.0.7
+Version: 0.0.8
 Summary: The AGiXT SDK for Python.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,11 +18,21 @@
 
 ## Installation
 ```bash
 pip install agixtsdk
 ```
 
 ## Usage
+
+```python
+from agixtsdk import AGiXTSDK
+
+base_uri = "http://localhost:7437"
+api_key = "your_agixt_api_key"
+
+ApiClient = AGiXTSDK(base_uri=base_uri, api_key=api_key)
+```
+
 Check out the AGiXT [Examples and Tests Notebook](https://github.com/Josh-XT/AGiXT/blob/main/tests/tests.ipynb) for examples of how to use the AGiXT SDK for Python.
 
 ## More Documentation
 Want to know more about AGiXT?  Check out our [documentation](https://josh-xt.github.io/AGiXT/) or [GitHub](https://github.com/Josh-XT/AGiXT) page.
```

### Comparing `agixtsdk-0.0.7/setup.py` & `agixtsdk-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="agixtsdk",
-    version="0.0.7",
+    version="0.0.8",
     description="The AGiXT SDK for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

