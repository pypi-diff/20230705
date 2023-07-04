# Comparing `tmp/fetch_features-0.2.8.tar.gz` & `tmp/fetch_features-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch_features-0.2.8.tar", last modified: Sat Jun  3 21:34:55 2023, max compression
+gzip compressed data, was "fetch_features-0.2.9.tar", last modified: Tue Jul  4 21:59:07 2023, max compression
```

## Comparing `fetch_features-0.2.8.tar` & `fetch_features-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.372066 fetch_features-0.2.8/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.8/LICENSE.md
--rw-r--r--   0 msp        (501) staff       (20)     3259 2023-06-03 21:34:55.371508 fetch_features-0.2.8/PKG-INFO
--rwxr-xr-x   0 msp        (501) staff       (20)     2533 2023-05-28 22:29:31.000000 fetch_features-0.2.8/README.md
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.357366 fetch_features-0.2.8/images/
--rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.8/images/fetch_features_gui.png
--rw-r--r--   0 msp        (501) staff       (20)     1159 2023-06-03 01:07:37.000000 fetch_features-0.2.8/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-06-03 21:34:55.372233 fetch_features-0.2.8/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.353469 fetch_features-0.2.8/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.363245 fetch_features-0.2.8/src/fetch_features.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     3259 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      463 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       57 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)      162 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        8 2023-06-03 21:34:55.000000 fetch_features-0.2.8/src/fetch_features.egg-info/top_level.txt
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-06-03 21:34:55.369835 fetch_features-0.2.8/src/fetcher/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.8/src/fetcher/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)     1239 2023-06-03 21:19:35.000000 fetch_features-0.2.8/src/fetcher/__main__.py
--rwx------   0 msp        (501) staff       (20)    18653 2023-06-03 21:21:01.000000 fetch_features-0.2.8/src/fetcher/access_genbank.py
--rw-r--r--   0 msp        (501) staff       (20)    17556 2023-06-03 21:18:22.000000 fetch_features-0.2.8/src/fetcher/gui.py
--rw-r--r--   0 msp        (501) staff       (20)    10902 2023-06-02 17:44:42.000000 fetch_features-0.2.8/src/fetcher/user_input.py
--rwx------   0 msp        (501) staff       (20)    27324 2023-06-01 03:19:25.000000 fetch_features-0.2.8/src/fetcher/utils.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-04 21:59:07.962396 fetch_features-0.2.9/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-04-07 00:12:37.000000 fetch_features-0.2.9/LICENSE.md
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-07-04 21:59:07.961880 fetch_features-0.2.9/PKG-INFO
+-rwxr-xr-x   0 msp        (501) staff       (20)     2533 2023-05-28 22:29:31.000000 fetch_features-0.2.9/README.md
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-04 21:59:07.946675 fetch_features-0.2.9/images/
+-rw-r--r--   0 msp        (501) staff       (20)   340268 2023-04-30 01:32:33.000000 fetch_features-0.2.9/images/fetch_features_gui.png
+-rw-r--r--   0 msp        (501) staff       (20)     1159 2023-07-04 21:27:00.000000 fetch_features-0.2.9/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-04 21:59:07.962517 fetch_features-0.2.9/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-04 21:59:07.943702 fetch_features-0.2.9/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-04 21:59:07.953406 fetch_features-0.2.9/src/fetch_features.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     3259 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      463 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       57 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)      162 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        8 2023-07-04 21:59:07.000000 fetch_features-0.2.9/src/fetch_features.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-04 21:59:07.960013 fetch_features-0.2.9/src/fetcher/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-05-04 15:38:40.000000 fetch_features-0.2.9/src/fetcher/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)     1239 2023-06-03 21:19:35.000000 fetch_features-0.2.9/src/fetcher/__main__.py
+-rwx------   0 msp        (501) staff       (20)    18653 2023-06-03 21:21:01.000000 fetch_features-0.2.9/src/fetcher/access_genbank.py
+-rw-r--r--   0 msp        (501) staff       (20)    17556 2023-06-03 21:18:22.000000 fetch_features-0.2.9/src/fetcher/gui.py
+-rw-r--r--   0 msp        (501) staff       (20)    10521 2023-07-04 21:36:43.000000 fetch_features-0.2.9/src/fetcher/user_input.py
+-rwx------   0 msp        (501) staff       (20)    27324 2023-06-01 03:19:25.000000 fetch_features-0.2.9/src/fetcher/utils.py
```

### Comparing `fetch_features-0.2.8/LICENSE.md` & `fetch_features-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/PKG-INFO` & `fetch_features-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch_features
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fetch_features-0.2.8/README.md` & `fetch_features-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/images/fetch_features_gui.png` & `fetch_features-0.2.9/images/fetch_features_gui.png`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/pyproject.toml` & `fetch_features-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fetch_features"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Fetch features from a list of accession or BioSample numbers."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `fetch_features-0.2.8/src/fetch_features.egg-info/PKG-INFO` & `fetch_features-0.2.9/src/fetch_features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetch-features
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fetch features from a list of accession or BioSample numbers.
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/fetch_features
 Keywords: unique identifier,accession number,BioSample number,GenBank,sequence features
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fetch_features-0.2.8/src/fetcher/__main__.py` & `fetch_features-0.2.9/src/fetcher/__main__.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/src/fetcher/access_genbank.py` & `fetch_features-0.2.9/src/fetcher/access_genbank.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/src/fetcher/gui.py` & `fetch_features-0.2.9/src/fetcher/gui.py`

 * *Files identical despite different names*

### Comparing `fetch_features-0.2.8/src/fetcher/user_input.py` & `fetch_features-0.2.9/src/fetcher/user_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,40 +11,33 @@
 from pathlib import Path
 import re
 from typing import Union
 import pkg_resources
 
 # Description message.
 description_msg = r"""
-  __      _       _        __            _
- / _| ___| |_ ___| |__    / _| ___  __ _| |_ _   _ _ __ ___  ___
-| |_ / _ \ __/ __| '_ \  | |_ / _ \/ _` | __| | | | '__/ _ \/ __|
-|  _|  __/ || (__| | | | |  _|  __/ (_| | |_| |_| | | |  __/\__ \
-|_|  \___|\__\___|_| |_| |_|  \___|\__,_|\__|\__,_|_|  \___||___/
-
 Fetch features from a list of accession or BioSample numbers.
 """
 
 # Epilog message for command line help.
 epilog_msg = r"""
 Usage examples:
 1. The simplest command. The output is in the current working directory.
-$ fetcher -i path/to/list.txt -t accession -e email@address.com
+fetch_features -i path/list.txt -t accession -e your@email.com
 
 2. In this example, the output is in your Documents.
-$ fetcher -i path/to/list.txt -t accession -e email@address.com -o ~/Documents
+fetch_features -i path/list.txt -t accession -e your@email.com -o ~/Documents
 
 3. If you prefer the GUI version.
-$ fetcher --gui
+fetch_features --gui
 """
 
 
 class UserInput:
     """Class to save user input via the commmand line."""
-    # TODO: include a `type` option for the type of identifiers in the list.
 
     def __init__(
             self,
             infile: Union[Path, None] = None,
             extention_infile: Union[str, None] = None,
             uid_type: Union[str, None] = None,
             email: Union[str, None] = None,
```

### Comparing `fetch_features-0.2.8/src/fetcher/utils.py` & `fetch_features-0.2.9/src/fetcher/utils.py`

 * *Files identical despite different names*

