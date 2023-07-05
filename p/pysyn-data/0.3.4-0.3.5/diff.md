# Comparing `tmp/pysyn-data-0.3.4.tar.gz` & `tmp/pysyn-data-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysyn-data-0.3.4.tar", last modified: Sun May 14 19:55:49 2023, max compression
+gzip compressed data, was "dist/pysyn-data-0.3.5.tar", last modified: Wed Jul  5 09:20:45 2023, max compression
```

## Comparing `pysyn-data-0.3.4.tar` & `pysyn-data-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1260 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1725 2023-05-14 19:55:44.000000 pysyn-data-0.3.4/README.md
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn-data-0.3.4/README.rst
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn-data-0.3.4/pysyn_data/__init__.py
-drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data.egg-info/
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1260 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data.egg-info/PKG-INFO
--rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data.egg-info/SOURCES.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data.egg-info/dependency_links.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/pysyn_data.egg-info/top_level.txt
--rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-05-14 19:55:49.000000 pysyn-data-0.3.4/setup.cfg
--rw-rw-r--   0 alokh     (1015) alokh     (1015)     1461 2023-05-14 19:55:35.000000 pysyn-data-0.3.4/setup.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1260 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1632 2023-07-05 09:16:34.000000 pysyn-data-0.3.5/README.md
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1429 2023-03-22 01:49:07.000000 pysyn-data-0.3.5/README.rst
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)    18350 2023-03-22 00:33:31.000000 pysyn-data-0.3.5/pysyn_data/__init__.py
+drwxrwxr-x   0 alokh     (1015) alokh     (1015)        0 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data.egg-info/
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1260 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data.egg-info/PKG-INFO
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)      188 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)        1 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       11 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/pysyn_data.egg-info/top_level.txt
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)       38 2023-07-05 09:20:45.000000 pysyn-data-0.3.5/setup.cfg
+-rw-rw-r--   0 alokh     (1015) alokh     (1015)     1612 2023-07-05 09:20:36.000000 pysyn-data-0.3.5/setup.py
```

### Comparing `pysyn-data-0.3.4/PKG-INFO` & `pysyn-data-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyn-data
-Version: 0.3.4
+Version: 0.3.5
 Summary: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.
 Home-page: UNKNOWN
 Author: Raghav-Ritesh-Tavlab
 Author-email: raghav.20.rb@gmail.com
 License: UNKNOWN
 Description: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi.
 Platform: UNKNOWN
```

### Comparing `pysyn-data-0.3.4/README.md` & `pysyn-data-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 ## pysyn-data Package
-This package is for generating synthetic data using 4 machine learning models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi. This is the [link](http://tavlab.iiitd.edu.in/index.html) to the lab's official webpage.
-
-
+This package is for generating synthetic data using 4 machine learning models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi.
 
 #### Package Intallation
 For installing the pysyn-data package the following command has to be run:
 ```bash
 pip install pysyn-data
 ```
```

### Comparing `pysyn-data-0.3.4/README.rst` & `pysyn-data-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `pysyn-data-0.3.4/pysyn_data/__init__.py` & `pysyn-data-0.3.5/pysyn_data/__init__.py`

 * *Files identical despite different names*

### Comparing `pysyn-data-0.3.4/pysyn_data.egg-info/PKG-INFO` & `pysyn-data-0.3.5/pysyn_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyn-data
-Version: 0.3.4
+Version: 0.3.5
 Summary: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.
 Home-page: UNKNOWN
 Author: Raghav-Ritesh-Tavlab
 Author-email: raghav.20.rb@gmail.com
 License: UNKNOWN
 Description: This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi.
 Platform: UNKNOWN
```

### Comparing `pysyn-data-0.3.4/setup.py` & `pysyn-data-0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 DESCRIPTION = 'This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics.'
 LONG_DESCRIPTION = 'This package is for generating synthetic data using 4 models i.e Conditional Genrative Adveserial Networks(CTGAN), Gaussian Mixture Model (GMM), Prinicipal Component Analysis (PCA) and Bayesian Network (BN). It also informs the user which model will work best based on the input data characterisitics. This package was created in TAVLAB under guidance of Dr. Tavpritesh Sethi (Computational Biology Lab under Dr Tavpritesh Sethi at IIITD) for Clinical Data Synthesis Project at Indraprastha Institute of Information Technology, Delhi.'
 
 # Setting up
 setup(
     name="pysyn-data",
     version=VERSION,
@@ -18,8 +18,15 @@
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
+
+'''
+python3.7 setup.py sdist bdist_wheel
+twine check dist/*
+twine upload --repository-url https://upload.pypi.org/legacy/ --skip-existing dist/*
+
+'''
```

