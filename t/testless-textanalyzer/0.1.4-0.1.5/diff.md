# Comparing `tmp/testless_textanalyzer-0.1.4.tar.gz` & `tmp/testless_textanalyzer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.4.tar", last modified: Tue Jul  4 23:32:54 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.5.tar", last modified: Tue Jul  4 23:49:46 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.4.tar` & `testless_textanalyzer-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-04 23:32:44.000000 testless_textanalyzer-0.1.4/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      542 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.4/textanalyzer/__init__.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/__init__.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     5931 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     7344 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf_utils.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature_set.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2644 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/text_analyzer.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:49:46.197623 testless_textanalyzer-0.1.5/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:49:46.197623 testless_textanalyzer-0.1.5/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:49:46.197623 testless_textanalyzer-0.1.5/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-04 23:49:00.000000 testless_textanalyzer-0.1.5/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:49:46.193622 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:49:45.000000 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      492 2023-07-04 23:49:45.000000 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:49:45.000000 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-04 23:49:45.000000 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:49:45.000000 testless_textanalyzer-0.1.5/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:49:46.193622 testless_textanalyzer-0.1.5/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.5/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:49:46.197623 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/__init__.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     6036 2023-07-04 23:48:46.000000 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/crf.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     7379 2023-07-04 23:49:28.000000 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/crf_utils.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/feature.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2679 2023-07-04 23:48:29.000000 testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/text_analyzer.py
```

### Comparing `testless_textanalyzer-0.1.4/setup.py` & `testless_textanalyzer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.4',
+  version='0.1.5',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
   long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
```

### Comparing `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf.py` & `testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/crf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from utils.read_data import read_data
-from feature import FeatureSet, STARTING_TOKEN_INDEX
+from textanalyzer.testless_textanalyzer.utils.read_data import read_data
+from textanalyzer.testless_textanalyzer.feature import FeatureSet, STARTING_TOKEN_INDEX
 import numpy as np
 from scipy.optimize import fmin_l_bfgs_b
-from crf_utils import calculate_log_likelihood, _gradient, _generate_potential_table
+from textanalyzer.testless_textanalyzer.crf_utils import calculate_log_likelihood, _gradient, _generate_potential_table
 from tqdm import tqdm
 
 import time
 import datetime
 import pickle
 import os
```

### Comparing `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf_utils.py` & `testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/crf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from feature import  STARTING_TOKEN_INDEX
+from textanalyzer.testless_textanalyzer.feature import  STARTING_TOKEN_INDEX
 
 
 SCALING_THR = 1e250
 
 GRADIENT = None
 
 def _generate_potential_table(params, num_labels, feature_set, X, inference=True):
```

### Comparing `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature.py` & `testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/feature.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/text_analyzer.py` & `testless_textanalyzer-0.1.5/textanalyzer/testless_textanalyzer/text_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import nltk
 import re
-from crf import LinearChainCRF
+from textanalyzer.testless_textanalyzer.crf import LinearChainCRF
 
 class TextAnalyzer():
     def __init__(self, path_to_model):
         self.crf = LinearChainCRF()
         self.crf.load(path_to_model)
```

