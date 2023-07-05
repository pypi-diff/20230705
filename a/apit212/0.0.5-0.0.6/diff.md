# Comparing `tmp/apit212-0.0.5.tar.gz` & `tmp/apit212-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-0.0.5.tar", last modified: Wed Jul  5 18:58:23 2023, max compression
+gzip compressed data, was "apit212-0.0.6.tar", last modified: Wed Jul  5 19:46:16 2023, max compression
```

## Comparing `apit212-0.0.5.tar` & `apit212-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 18:58:23.805114 apit212-0.0.5/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     7047 2023-07-05 18:58:23.803746 apit212-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6241 2023-07-05 18:57:42.000000 apit212-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 18:58:23.749653 apit212-0.0.5/apit212/
--rw-rw-rw-   0        0        0    17835 2023-07-05 18:54:10.000000 apit212-0.0.5/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.5/apit212/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-07-05 18:54:15.000000 apit212-0.0.5/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-05 18:54:17.000000 apit212-0.0.5/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:58:23.796190 apit212-0.0.5/apit212.egg-info/
--rw-rw-rw-   0        0        0     7047 2023-07-05 18:58:23.000000 apit212-0.0.5/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-05 18:58:23.000000 apit212-0.0.5/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 18:58:23.000000 apit212-0.0.5/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-05 18:58:23.000000 apit212-0.0.5/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 18:58:23.000000 apit212-0.0.5/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      858 2023-07-05 18:54:27.000000 apit212-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 18:58:23.805114 apit212-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-07-05 18:53:39.000000 apit212-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:46:16.949789 apit212-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7008 2023-07-05 19:46:16.945975 apit212-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6241 2023-07-05 18:57:42.000000 apit212-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 19:46:16.893695 apit212-0.0.6/apit212/
+-rw-rw-rw-   0        0        0    17829 2023-07-05 19:45:11.000000 apit212-0.0.6/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.6/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-0.0.6/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-05 19:45:17.000000 apit212-0.0.6/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-07-05 19:46:16.942394 apit212-0.0.6/apit212.egg-info/
+-rw-rw-rw-   0        0        0     7008 2023-07-05 19:46:16.000000 apit212-0.0.6/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-05 19:46:16.000000 apit212-0.0.6/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 19:46:16.000000 apit212-0.0.6/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-05 19:46:16.000000 apit212-0.0.6/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-05 19:46:16.000000 apit212-0.0.6/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-07-05 19:45:34.000000 apit212-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 19:46:16.949789 apit212-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-07-05 19:45:31.000000 apit212-0.0.6/setup.py
```

### Comparing `apit212-0.0.5/LICENSE` & `apit212-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-0.0.5/PKG-INFO` & `apit212-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
@@ -12,16 +12,14 @@
 Keywords: trading,trading212,api,trade,flock92
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires: requests
 Requires: selenium
-Requires: getpass
-Requires: constant
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
```

### Comparing `apit212-0.0.5/README.md` & `apit212-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apit212-0.0.5/apit212/Apit212.py` & `apit212-0.0.6/apit212/Apit212.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # this unofficial API was created by Flock92 originally made to automate my CFD trading on the trading212 platform
 
 import requests
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from getpass import getpass
-from apit212 import apitconstant
+from apitconstant import *
 from time import sleep
 import logging
 import json
 
 
 class Apit212:
     headers = {}
```

### Comparing `apit212-0.0.5/apit212/apitconstant.py` & `apit212-0.0.6/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.5/apit212/cfdScrape.py` & `apit212-0.0.6/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.5/apit212.egg-info/PKG-INFO` & `apit212-0.0.6/apit212.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
@@ -12,16 +12,14 @@
 Keywords: trading,trading212,api,trade,flock92
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires: requests
 Requires: selenium
-Requires: getpass
-Requires: constant
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
```

### Comparing `apit212-0.0.5/pyproject.toml` & `apit212-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
@@ -25,13 +25,12 @@
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
 ]
 
 dependencies = [
   "selenium>4.7.2",
   "requests>2.28.2",
-  "apitconstant",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Flock92/apit212"
 "Bug Tracker" = "https://github.com/Flock92/apit212/issues"
```

### Comparing `apit212-0.0.5/setup.py` & `apit212-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
-        'getpass',
-        'constant'
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
     description="Unofficial trading212 API",
     long_description=long_description,
     license="MIT",
     keywords="trading api" "python3" "trading212" "API",
```

