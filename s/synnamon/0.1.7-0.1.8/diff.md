# Comparing `tmp/synnamon-0.1.7.tar.gz` & `tmp/synnamon-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnamon-0.1.7.tar", last modified: Fri Jun 30 18:57:14 2023, max compression
+gzip compressed data, was "synnamon-0.1.8.tar", last modified: Wed Jul  5 14:33:58 2023, max compression
```

## Comparing `synnamon-0.1.7.tar` & `synnamon-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.697414 synnamon-0.1.7/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.7/LICENSE.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:57:14.697090 synnamon-0.1.7/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1384 2023-06-30 18:16:35.000000 synnamon-0.1.7/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-06-30 18:57:14.697490 synnamon-0.1.7/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      777 2023-06-30 18:56:00.000000 synnamon-0.1.7/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.681112 synnamon-0.1.7/synnamon/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       62 2023-06-30 18:56:15.000000 synnamon-0.1.7/synnamon/__init__.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.686629 synnamon-0.1.7/synnamon/data/
--rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.7/synnamon/data/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)  9230899 2023-06-30 18:53:58.000000 synnamon-0.1.7/synnamon/data/thesaurus.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      821 2023-06-30 18:55:31.000000 synnamon-0.1.7/synnamon/get_syns.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.685879 synnamon-0.1.7/synnamon.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1860 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      306 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-06-30 18:57:14.000000 synnamon-0.1.7/synnamon.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-06-30 18:57:14.695784 synnamon-0.1.7/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.7/tests/test_get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-05 14:33:58.598765 synnamon-0.1.8/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1101 2023-06-28 16:29:02.000000 synnamon-0.1.8/LICENSE.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-07-05 14:33:58.598463 synnamon-0.1.8/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1386 2023-07-05 14:30:44.000000 synnamon-0.1.8/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-07-05 14:33:58.598837 synnamon-0.1.8/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      823 2023-07-05 14:32:09.000000 synnamon-0.1.8/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-05 14:33:58.569405 synnamon-0.1.8/synnamon/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       62 2023-07-05 14:30:53.000000 synnamon-0.1.8/synnamon/__init__.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-05 14:33:58.574887 synnamon-0.1.8/synnamon/data/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        0 2023-06-30 14:54:31.000000 synnamon-0.1.8/synnamon/data/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20) 20537344 2023-07-05 14:29:14.000000 synnamon-0.1.8/synnamon/data/en_thesaurus.db
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      955 2023-07-05 14:29:05.000000 synnamon-0.1.8/synnamon/get_syns.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-05 14:33:58.574211 synnamon-0.1.8/synnamon.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1862 2023-07-05 14:33:58.000000 synnamon-0.1.8/synnamon.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      309 2023-07-05 14:33:58.000000 synnamon-0.1.8/synnamon.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-05 14:33:58.000000 synnamon-0.1.8/synnamon.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        7 2023-07-05 14:33:58.000000 synnamon-0.1.8/synnamon.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-05 14:33:58.000000 synnamon-0.1.8/synnamon.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-05 14:33:58.597661 synnamon-0.1.8/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1085 2023-06-30 15:07:16.000000 synnamon-0.1.8/tests/test_get_syns.py
```

### Comparing `synnamon-0.1.7/LICENSE.md` & `synnamon-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `synnamon-0.1.7/PKG-INFO` & `synnamon-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
```

### Comparing `synnamon-0.1.7/README.md` & `synnamon-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
```

### Comparing `synnamon-0.1.7/setup.py` & `synnamon-0.1.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="synnamon",
-    version="0.1.7",
+    version="0.1.8",
     description="Pure Python package for getting synonyms for words.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/synnamon",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
@@ -19,9 +19,10 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
     ],
     packages=find_packages(),
     include_package_data=True,
     python_requires='>=3.6',
-    install_requires=['inflex']
+    install_requires=['inflex'],
+    package_data={'synnamon': ['data/*.db']}
 )
```

### Comparing `synnamon-0.1.7/synnamon.egg-info/PKG-INFO` & `synnamon-0.1.8/synnamon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnamon
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pure Python package for getting synonyms for words.
 Home-page: https://github.com/eddiethedean/synnamon
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 
 # Synnamon: Easy to use function for word synonym lookups
 [![PyPI Latest Release](https://img.shields.io/pypi/v/synnamon.svg)](https://pypi.org/project/synnamon/)
 ![Tests](https://github.com/eddiethedean/synnamon/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus json file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
+**Synnamon** is a simple Python package that looks up synonyms using a built in thesaurus shelve file instead of reaching out to web resources (PyDictionary) or using large English lexical databases (nltk WordNet).
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/synnamon
 
 ```sh
 # PyPI
```

### Comparing `synnamon-0.1.7/tests/test_get_syns.py` & `synnamon-0.1.8/tests/test_get_syns.py`

 * *Files identical despite different names*

