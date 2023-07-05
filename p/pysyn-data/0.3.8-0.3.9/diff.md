# Comparing `tmp/pysyn-data-0.3.8.tar.gz` & `tmp/pysyn-data-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysyn-data-0.3.8.tar", last modified: Wed Jul  5 09:27:13 2023, max compression
+gzip compressed data, was "pysyn-data-0.3.9.tar", last modified: Wed Jul  5 09:35:05 2023, max compression
```

## Comparing `pysyn-data-0.3.8.tar` & `pysyn-data-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:27:13.653574 pysyn-data-0.3.8/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1194 2023-07-05 09:27:13.653574 pysyn-data-0.3.8/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1663 2023-07-05 09:27:00.000000 pysyn-data-0.3.8/README.md
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn-data-0.3.8/README.rst
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:27:13.653574 pysyn-data-0.3.8/pysyn_data/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn-data-0.3.8/pysyn_data/__init__.py
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:27:13.653574 pysyn-data-0.3.8/pysyn_data.egg-info/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1194 2023-07-05 09:27:13.000000 pysyn-data-0.3.8/pysyn_data.egg-info/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-07-05 09:27:13.000000 pysyn-data-0.3.8/pysyn_data.egg-info/SOURCES.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-07-05 09:27:13.000000 pysyn-data-0.3.8/pysyn_data.egg-info/dependency_links.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-07-05 09:27:13.000000 pysyn-data-0.3.8/pysyn_data.egg-info/top_level.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-07-05 09:27:13.653574 pysyn-data-0.3.8/setup.cfg
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1612 2023-07-05 09:26:44.000000 pysyn-data-0.3.8/setup.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:35:05.236118 pysyn-data-0.3.9/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1194 2023-07-05 09:35:05.236118 pysyn-data-0.3.9/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1664 2023-07-05 09:34:56.000000 pysyn-data-0.3.9/README.md
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn-data-0.3.9/README.rst
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:35:05.236118 pysyn-data-0.3.9/pysyn_data/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn-data-0.3.9/pysyn_data/__init__.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:35:05.236118 pysyn-data-0.3.9/pysyn_data.egg-info/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1194 2023-07-05 09:35:05.000000 pysyn-data-0.3.9/pysyn_data.egg-info/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-07-05 09:35:05.000000 pysyn-data-0.3.9/pysyn_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-07-05 09:35:05.000000 pysyn-data-0.3.9/pysyn_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-07-05 09:35:05.000000 pysyn-data-0.3.9/pysyn_data.egg-info/top_level.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-07-05 09:35:05.236118 pysyn-data-0.3.9/setup.cfg
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1612 2023-07-05 09:34:57.000000 pysyn-data-0.3.9/setup.py
```

### Comparing `pysyn-data-0.3.8/PKG-INFO` & `pysyn-data-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyn-data
-Version: 0.3.8
+Version: 0.3.9
 Summary: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.
 Author: Raghav-Ritesh-Tavlab
 Author-email: raghav.20.rb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pysyn-data-0.3.8/README.md` & `pysyn-data-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## pysyn-data Package
 This package is for generating synthetic data using 4 machine learning models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi. Link will be updated for the same.
 
-#### Package Intallation
+#### Package Installation
 For installing the pysyn-data package the following command has to be run:
 ```
 pip install pysyn-data
 ```
 
 #### Functions Usage
```

### Comparing `pysyn-data-0.3.8/README.rst` & `pysyn-data-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `pysyn-data-0.3.8/pysyn_data/__init__.py` & `pysyn-data-0.3.9/pysyn_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pysyn-data-0.3.8/pysyn_data.egg-info/PKG-INFO` & `pysyn-data-0.3.9/pysyn_data.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyn-data
-Version: 0.3.8
+Version: 0.3.9
 Summary: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.
 Author: Raghav-Ritesh-Tavlab
 Author-email: raghav.20.rb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pysyn-data-0.3.8/setup.py` & `pysyn-data-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.3.8'
+VERSION = '0.3.9'
 DESCRIPTION = 'This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.'
 LONG_DESCRIPTION = 'This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi.'
 
 # Setting up
 setup(
     name="pysyn-data",
     version=VERSION,
```

