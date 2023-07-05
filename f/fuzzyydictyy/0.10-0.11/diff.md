# Comparing `tmp/fuzzyydictyy-0.10.tar.gz` & `tmp/fuzzyydictyy-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzyydictyy-0.10.tar", last modified: Wed Jul  5 01:49:47 2023, max compression
+gzip compressed data, was "fuzzyydictyy-0.11.tar", last modified: Wed Jul  5 01:51:39 2023, max compression
```

## Comparing `fuzzyydictyy-0.10.tar` & `fuzzyydictyy-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:49:47.154382 fuzzyydictyy-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-05 01:49:40.000000 fuzzyydictyy-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      107 2023-07-05 01:49:36.000000 fuzzyydictyy-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2614 2023-07-05 01:49:47.154382 fuzzyydictyy-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2012 2023-07-05 01:46:45.000000 fuzzyydictyy-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 01:49:47.150369 fuzzyydictyy-0.10/fuzzyydictyy/
--rw-rw-rw-   0        0        0     2012 2023-07-05 01:46:45.000000 fuzzyydictyy-0.10/fuzzyydictyy/README.MD
--rw-rw-rw-   0        0        0     2864 2023-07-05 01:47:37.000000 fuzzyydictyy-0.10/fuzzyydictyy/__init__.py
--rw-rw-rw-   0        0        0        9 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy/requirements.txt
--rw-rw-rw-   0        0        0     1207 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-05 01:49:47.153361 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/
--rw-rw-rw-   0        0        0     2614 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-05 01:49:47.000000 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/fuzzyydictyy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-05 01:49:47.154382 fuzzyydictyy-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-05 01:49:46.000000 fuzzyydictyy-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-05 01:51:27.000000 fuzzyydictyy-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      107 2023-07-05 01:51:24.000000 fuzzyydictyy-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2618 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-07-05 01:50:38.000000 fuzzyydictyy-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.233399 fuzzyydictyy-0.11/fuzzyydictyy/
+-rw-rw-rw-   0        0        0     2016 2023-07-05 01:50:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/README.MD
+-rw-rw-rw-   0        0        0     2864 2023-07-05 01:47:37.000000 fuzzyydictyy-0.11/fuzzyydictyy/__init__.py
+-rw-rw-rw-   0        0        0        9 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/requirements.txt
+-rw-rw-rw-   0        0        0     1207 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/
+-rw-rw-rw-   0        0        0     2618 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-07-05 01:51:39.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-05 01:51:39.238387 fuzzyydictyy-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/setup.py
```

### Comparing `fuzzyydictyy-0.10/LICENSE.rst` & `fuzzyydictyy-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.10/PKG-INFO` & `fuzzyydictyy-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyydictyy
-Version: 0.10
+Version: 0.11
 Summary: Dict with fuzzy key matching 
 Home-page: https://github.com/hansalemaos/fuzzyydictyy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: fuzzy,dict
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # Dict with fuzzy key matching 
 
-## pip install fuzzdict 
+## pip install fuzzyydictyy 
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 
 
 ### Approximate Key Lookups: 
 
 The fuzzy matching capability allows users to retrieve values even if the exact key is not available. This can be beneficial when dealing with user input, search queries, or data with potential typos or variations.
```

### Comparing `fuzzyydictyy-0.10/README.md` & `fuzzyydictyy-0.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dict with fuzzy key matching 
 
-## pip install fuzzdict 
+## pip install fuzzyydictyy 
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 
 
 ### Approximate Key Lookups: 
 
 The fuzzy matching capability allows users to retrieve values even if the exact key is not available. This can be beneficial when dealing with user input, search queries, or data with potential typos or variations.
```

### Comparing `fuzzyydictyy-0.10/fuzzyydictyy/README.MD` & `fuzzyydictyy-0.11/fuzzyydictyy/README.MD`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dict with fuzzy key matching 
 
-## pip install fuzzdict 
+## pip install fuzzyydictyy 
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 
 
 ### Approximate Key Lookups: 
 
 The fuzzy matching capability allows users to retrieve values even if the exact key is not available. This can be beneficial when dealing with user input, search queries, or data with potential typos or variations.
```

### Comparing `fuzzyydictyy-0.10/fuzzyydictyy/__init__.py` & `fuzzyydictyy-0.11/fuzzyydictyy/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.10/fuzzyydictyy/thirdparty.json` & `fuzzyydictyy-0.11/fuzzyydictyy/thirdparty.json`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.10/fuzzyydictyy.egg-info/PKG-INFO` & `fuzzyydictyy-0.11/fuzzyydictyy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyydictyy
-Version: 0.10
+Version: 0.11
 Summary: Dict with fuzzy key matching 
 Home-page: https://github.com/hansalemaos/fuzzyydictyy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: fuzzy,dict
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # Dict with fuzzy key matching 
 
-## pip install fuzzdict 
+## pip install fuzzyydictyy 
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda 
 
 
 ### Approximate Key Lookups: 
 
 The fuzzy matching capability allows users to retrieve values even if the exact key is not available. This can be beneficial when dealing with user input, search queries, or data with potential typos or variations.
```

### Comparing `fuzzyydictyy-0.10/setup.py` & `fuzzyydictyy-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Dict with fuzzy key matching '''
 
 # Setting up
 setup(
     name="fuzzyydictyy",
     version=VERSION,
     license='MIT',
```

