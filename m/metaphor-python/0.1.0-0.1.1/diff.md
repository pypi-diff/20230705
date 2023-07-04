# Comparing `tmp/metaphor-python-0.1.0.tar.gz` & `tmp/metaphor-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.0.tar", last modified: Tue Jul  4 22:57:24 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.1.tar", last modified: Tue Jul  4 23:05:14 2023, max compression
```

## Comparing `metaphor-python-0.1.0.tar` & `metaphor-python-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 22:57:24.817810 metaphor-python-0.1.0/
--rw-r--r--   0 jwang      (501) staff       (20)      655 2023-07-04 22:57:24.817674 metaphor-python-0.1.0/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)       81 2023-07-04 22:56:54.000000 metaphor-python-0.1.0/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 22:57:24.816949 metaphor-python-0.1.0/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 22:55:15.000000 metaphor-python-0.1.0/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     2976 2023-07-04 22:54:36.000000 metaphor-python-0.1.0/metaphor_python/metaphor.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 22:57:24.817494 metaphor-python-0.1.0/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      655 2023-07-04 22:57:24.000000 metaphor-python-0.1.0/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      268 2023-07-04 22:57:24.000000 metaphor-python-0.1.0/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-04 22:57:24.000000 metaphor-python-0.1.0/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-04 22:57:24.000000 metaphor-python-0.1.0/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-04 22:57:24.000000 metaphor-python-0.1.0/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-04 22:57:24.817853 metaphor-python-0.1.0/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-04 22:55:57.000000 metaphor-python-0.1.0/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 23:05:14.983500 metaphor-python-0.1.1/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-04 23:05:14.983362 metaphor-python-0.1.1/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)       81 2023-07-04 22:56:54.000000 metaphor-python-0.1.1/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 23:05:14.982531 metaphor-python-0.1.1/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.1/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     2976 2023-07-04 22:54:36.000000 metaphor-python-0.1.1/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-04 23:05:14.983181 metaphor-python-0.1.1/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-04 23:05:14.983543 metaphor-python-0.1.1/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-04 23:05:14.000000 metaphor-python-0.1.1/setup.py
```

### Comparing `metaphor-python-0.1.0/PKG-INFO` & `metaphor-python-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-
-UNKNOWN
-
```

### Comparing `metaphor-python-0.1.0/metaphor_python/metaphor.py` & `metaphor-python-0.1.1/metaphor_python/api.py`

 * *Files identical despite different names*

### Comparing `metaphor-python-0.1.0/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.1/metaphor_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-
-UNKNOWN
-
```

