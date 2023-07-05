# Comparing `tmp/omnivoreql-0.1.0.tar.gz` & `tmp/omnivoreql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.1.0.tar", last modified: Mon Jul  3 19:16:46 2023, max compression
+gzip compressed data, was "omnivoreql-0.1.1.tar", last modified: Wed Jul  5 21:34:15 2023, max compression
```

## Comparing `omnivoreql-0.1.0.tar` & `omnivoreql-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:16:46.955802 omnivoreql-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-03 19:16:46.951801 omnivoreql-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:16:46.951801 omnivoreql-0.1.0/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/omnivoreql/__init__,py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/omnivoreql/omnivoreql.py
--rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/omnivoreql/schema.gql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:16:46.951801 omnivoreql-0.1.0/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-03 19:16:46.000000 omnivoreql-0.1.0/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 19:16:46.000000 omnivoreql-0.1.0/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:16:46.000000 omnivoreql-0.1.0/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:16:46.000000 omnivoreql-0.1.0/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:16:46.000000 omnivoreql-0.1.0/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:16:46.955802 omnivoreql-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-03 19:16:42.000000 omnivoreql-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:34:15.985662 omnivoreql-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 21:34:15.985662 omnivoreql-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:34:15.985662 omnivoreql-0.1.1/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/omnivoreql/__init__,py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/omnivoreql/omnivoreql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/omnivoreql/schema.gql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:34:15.985662 omnivoreql-0.1.1/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 21:34:15.000000 omnivoreql-0.1.1/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 21:34:15.000000 omnivoreql-0.1.1/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:34:15.000000 omnivoreql-0.1.1/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 21:34:15.000000 omnivoreql-0.1.1/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 21:34:15.000000 omnivoreql-0.1.1/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:34:15.985662 omnivoreql-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 21:34:10.000000 omnivoreql-0.1.1/setup.py
```

### Comparing `omnivoreql-0.1.0/LICENSE` & `omnivoreql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.0/PKG-INFO` & `omnivoreql-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
 Keywords: omnivore api readlater graphql gql client
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OmnivoreQL: Omnivore API client for Python
 
 This is a Python client for the [Omnivore API](https://omnivore.app).
 
 [![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
 [![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
 
+[![Tests](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+
 ## How to use
 
 To use omnivoreql in your Python project, you can follow these steps:
 
 Install the omnivoreql package using pip:
 
 ```bash
```

### Comparing `omnivoreql-0.1.0/README.md` & `omnivoreql-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # OmnivoreQL: Omnivore API client for Python
 
 This is a Python client for the [Omnivore API](https://omnivore.app).
 
 [![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
 [![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
 
+[![Tests](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+
 ## How to use
 
 To use omnivoreql in your Python project, you can follow these steps:
 
 Install the omnivoreql package using pip:
 
 ```bash
```

### Comparing `omnivoreql-0.1.0/omnivoreql/omnivoreql.py` & `omnivoreql-0.1.1/omnivoreql/omnivoreql.py`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.0/omnivoreql/schema.gql` & `omnivoreql-0.1.1/omnivoreql/schema.gql`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.0/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.1.1/omnivoreql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.0
+Version: 0.1.1
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
 Keywords: omnivore api readlater graphql gql client
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OmnivoreQL: Omnivore API client for Python
 
 This is a Python client for the [Omnivore API](https://omnivore.app).
 
 [![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
 [![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
 
+[![Tests](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+
 ## How to use
 
 To use omnivoreql in your Python project, you can follow these steps:
 
 Install the omnivoreql package using pip:
 
 ```bash
```

### Comparing `omnivoreql-0.1.0/setup.py` & `omnivoreql-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import subprocess
 
 def get_latest_git_tag():
     try:
         version = subprocess.check_output(["git", "describe", "--tags", "--abbrev=0"])
         version = version.strip().decode("utf-8")  # Remove trailing newline and decode bytes to string
 
@@ -24,26 +24,28 @@
 
 setup(
     name='omnivoreql',
     version=VERSION,
     description='Omnivore API Client for Python',
     author='Shahriar Yazdipour',
     author_email='git@yazdipour.com',
-    packages=find_packages("omnivoreql"),
+    packages=['omnivoreql'],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="omnivore api readlater graphql gql client",
     platforms="any",
     url="https://github.com/yazdipour/OmnivoreQL",
     project_urls=PROJECT_URLS,
+    include_package_data=True,
+    python_requires=">=3",
     classifiers=[
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         'gql==3.4.1',
         'requests-toolbelt==1.0.0'
-    ],
+    ]
 )
```

