# Comparing `tmp/sam_ml-py-0.7.3.tar.gz` & `tmp/sam_ml-py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.7.3.tar", last modified: Thu Jun 29 12:57:14 2023, max compression
+gzip compressed data, was "sam_ml-py-0.8.0.tar", last modified: Wed Jul  5 08:58:33 2023, max compression
```

## Comparing `sam_ml-py-0.7.3.tar` & `sam_ml-py-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.145703 sam_ml-py-0.7.3/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.145703 sam_ml-py-0.7.3/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.145703 sam_ml-py-0.7.3/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 12:57:14.000000 sam_ml-py-0.7.3/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 12:57:14.000000 sam_ml-py-0.7.3/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:57:14.000000 sam_ml-py-0.7.3/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-29 12:57:14.000000 sam_ml-py-0.7.3/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 12:57:14.000000 sam_ml-py-0.7.3/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:14.153704 sam_ml-py-0.7.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-29 12:57:02.000000 sam_ml-py-0.7.3/test/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.778266 sam_ml-py-0.8.0/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.778266 sam_ml-py-0.8.0/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.782266 sam_ml-py-0.8.0/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.786266 sam_ml-py-0.8.0/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 08:58:33.000000 sam_ml-py-0.8.0/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:33.790266 sam_ml-py-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-05 08:58:23.000000 sam_ml-py-0.8.0/test/test_models.py
```

### Comparing `sam_ml-py-0.7.3/LICENSE` & `sam_ml-py-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/PKG-INFO` & `sam_ml-py-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.7.3
+Version: 0.8.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: with_swig
 License-File: LICENSE
 
 # SAM_ML
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
-## getting started
+## getting started (with SMAC3 library)
 
 0. pre-installations *(needed for [smac](https://github.com/automl/SMAC3) library)*
 
 You need to install `swig` for the *smag* library that is used for hyperparameter tuning.
 
 Linux *(see [smac installation guide](https://automl.github.io/SMAC3/main/1_installation.html))*:
 
@@ -29,14 +30,24 @@
 
 MacOS (with [homebrew](https://formulae.brew.sh/formula/swig)):
 
 ```
 brew install swig
 ```
 
+Windows (see [swigwin](https://www.swig.org/download.html))
+
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
+
+```
+pip install sam-ml-py[with_swig]
+```
+
+## getting started (without SMAC3 library)
+
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.7.3/README.md` & `sam_ml-py-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SAM_ML
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
-## getting started
+## getting started (with SMAC3 library)
 
 0. pre-installations *(needed for [smac](https://github.com/automl/SMAC3) library)*
 
 You need to install `swig` for the *smag* library that is used for hyperparameter tuning.
 
 Linux *(see [smac installation guide](https://automl.github.io/SMAC3/main/1_installation.html))*:
 
@@ -18,14 +18,24 @@
 
 MacOS (with [homebrew](https://formulae.brew.sh/formula/swig)):
 
 ```
 brew install swig
 ```
 
+Windows (see [swigwin](https://www.swig.org/download.html))
+
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
+
+```
+pip install sam-ml-py[with_swig]
+```
+
+## getting started (without SMAC3 library)
+
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.7.3/sam_ml/data/embeddings.py` & `sam_ml-py-0.8.0/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/data/feature_selection.py` & `sam_ml-py-0.8.0/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/data/sampling.py` & `sam_ml-py-0.8.0/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/data/scaler.py` & `sam_ml-py-0.8.0/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.8.0/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/AdaBoostClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 from ConfigSpace import Beta, Categorical, ConfigurationSpace, Float, Integer
 from sklearn.base import ClassifierMixin
-from sklearn.ensemble import (
-    AdaBoostClassifier,
-    GradientBoostingClassifier,
-    RandomForestClassifier,
-)
-from sklearn.linear_model import LogisticRegression
-from sklearn.svm import SVC
+from sklearn.ensemble import AdaBoostClassifier, RandomForestClassifier
 from sklearn.tree import DecisionTreeClassifier
 
 from .main_classifier import Classifier
 
 
 class ABC(Classifier):
     """ AdaBoostClassifier Wrapper class """
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/BaggingClassifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import warnings
 
 from ConfigSpace import Beta, Categorical, ConfigurationSpace, Float, Integer
 from sklearn.base import ClassifierMixin
-from sklearn.ensemble import (
-    BaggingClassifier,
-    GradientBoostingClassifier,
-    RandomForestClassifier,
-)
-from sklearn.linear_model import LogisticRegression
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.svm import SVC
+from sklearn.ensemble import BaggingClassifier, RandomForestClassifier
 from sklearn.tree import DecisionTreeClassifier
 
+from sam_ml.config import get_n_jobs
+
 from .main_classifier import Classifier
 
 warnings. filterwarnings('ignore')
 
 
 class BC(Classifier):
     """ BaggingClassifier Wrapper class """
 
     def __init__(
         self,
         model_name: str = "BaggingClassifier",
         random_state: int = 42,
-        n_jobs: int = -1,
+        n_jobs: int = get_n_jobs(),
         estimator: ClassifierMixin = DecisionTreeClassifier(max_depth=1),
         **kwargs,
     ):
         """
         @param (important one):
             estimator: base estimator from which the boosted ensemble is built (default: DecisionTreeClassifier with max_depth=1)
             n_estimator: number of boosting stages to perform
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.8.0/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.8.0/sam_ml/models/ClassifierTest.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/ExtraTreesClassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
 from sklearn.ensemble import ExtraTreesClassifier
 
+from sam_ml.config import get_n_jobs
+
 from .main_classifier import Classifier
 
 
 class ETC(Classifier):
     """ ExtraTreesClassifier Wrapper class """
 
     def __init__(
         self,
         model_name: str = "ExtraTreesClassifier",
-        n_jobs: int = -1,
+        n_jobs: int = get_n_jobs(),
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
             n_estimators: Number of trees
             max_depth: Maximum number of levels in tree
@@ -42,15 +44,15 @@
             "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
             "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
             "bootstrap": Categorical("bootstrap", [True, False], default=False),
             "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         
-        # workaround for now -> Problems with Normal distribution (in smac_search)
+        # workaround for now -> Problems with Normal distribution (in smac_search) (04/07/2023)
         self.smac_grid = ConfigurationSpace(
             seed=42,
             space={
             "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
             "max_depth": Integer("max_depth", (3, 15), default=5),
             "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.8.0/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/GaussianProcessClassifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ConfigSpace import Categorical, ConfigurationSpace, Integer
 from sklearn.gaussian_process import GaussianProcessClassifier
 
+from sam_ml.config import get_n_jobs
+
 from .main_classifier import Classifier
 
 
 class GPC(Classifier):
     """ GaussianProcessClassifier Wrapper class """
 
     def __init__(
         self,
         model_name: str = "GaussianProcessClassifier",
-        n_jobs: int = -1,
+        n_jobs: int = get_n_jobs(),
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
             multi_class: specifies how multi-class classification problems are handled
             max_iter_predict: the maximum number of iterations in Newton's method for approximating the posterior during predict
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.8.0/sam_ml/models/GradientBoostingMachine.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
             "subsample": Float("subsample", (0.7, 1), default=1),
             "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
             "loss": Categorical("loss", ["log_loss", "deviance"], default="log_loss"),
             "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
             })
         
-        # workaround for now -> Problems with Normal distribution (in smac_search)
+        # workaround for now -> Problems with Normal distribution (in smac_search) (04/07/2023)
         self.smac_grid = ConfigurationSpace(
             seed=42,
             space={
             "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
             "max_depth": Integer("max_depth", (1, 15), default=3),
             "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.8.0/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import numpy as np
 from ConfigSpace import Categorical, ConfigurationSpace, Float, InCondition
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 
 from .main_classifier import Classifier
 
+np.seterr(divide = 'ignore')
 
 class LDA(Classifier):
     """ LinearDiscriminantAnalysis Wrapper class """
 
     def __init__(
         self,
         model_name: str = "LinearDiscriminantAnalysis",
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.8.0/sam_ml/models/LogisticRegression.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,8 +51,17 @@
         solver_and_penalty = ForbiddenAndConjunction(
             ForbiddenEqualsClause(grid["penalty"], "elasticnet"),
             ForbiddenInClause(grid["solver"], ["newton-cg", "lbfgs", "liblinear", "sag"]),
         )
         l1_ratio_cond = EqualsCondition(grid["l1_ratio"], grid["penalty"], "elasticnet")
         grid.add_forbidden_clause(solver_and_penalty)
         grid.add_condition(l1_ratio_cond)
+
+        # workaround for now -> Problems with EqualsCondition (KeyError: 'l1_ratio') (04/07/2023)
+        self.smac_grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "solver": Categorical("solver", ["newton-cg", "lbfgs", "liblinear", "sag", "saga"], default="lbfgs"),
+            "penalty": Categorical("penalty", ["l2"], default="l2"),
+            "C": Float("C", (0.01, 100), log=True, default=1),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.8.0/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/RandomForestClassifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
 from sklearn.ensemble import RandomForestClassifier
 
+from sam_ml.config import get_n_jobs
+
 from .main_classifier import Classifier
 
 
 class RFC(Classifier):
     """ RandomForestClassifier Wrapper class """
 
     def __init__(
         self,
         model_name: str = "RandomForestClassifier",
-        n_jobs: int = -1, 
+        n_jobs: int = get_n_jobs(), 
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
             n_estimators: Number of trees in random forest
             max_depth: Maximum number of levels in tree
@@ -42,15 +44,15 @@
             "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
             "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
             "bootstrap": Categorical("bootstrap", [True, False], default=True),
             "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         
-        # workaround for now -> Problems with Normal distribution (in smac_search)
+        # workaround for now -> Problems with Normal distribution (in smac_search) (04/07/2023)
         self.smac_grid = ConfigurationSpace(
             seed=42,
             space={
             "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
             "max_depth": Integer("max_depth", (3, 15), default=5),
             "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
             "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.8.0/sam_ml/models/XGBoostClassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ConfigSpace import ConfigurationSpace, Float, Integer, Normal
 from xgboost import XGBClassifier
 
+from sam_ml.config import get_n_jobs
+
 from .main_classifier import Classifier
 
 
 class XGBC(Classifier):
     """ SupportVectorClassifier Wrapper class """
 
     def __init__(
         self,
         model_name: str = "XGBClassifier",
-        n_jobs: str = -1,
+        n_jobs: str = get_n_jobs(),
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
             random_state: random_state for model
             n_jobs: how many cores shall be used (-1 means all)
@@ -34,15 +36,15 @@
             'reg_lambda' : Float('reg_lambda', (0, 1), default=1),
             'colsample_bytree' : Float('colsample_bytree', (0.5, 1), default=1),
             'min_child_weight' : Integer('min_child_weight', (0, 10), default=1),
             'n_estimators': Integer("n_estimators", bounds=(50, 750), distribution=Normal(150, 100), default=100),
             "learning_rate": Float("learning_rate", bounds=(0.001, 0.30), log=True, default=0.1),
             })
         
-        # workaround for now -> Problems with Normal distribution (in smac_search)
+        # workaround for now -> Problems with Normal distribution (in smac_search) (04/07/2023)
         self.smac_grid = ConfigurationSpace(
             seed=42,
             space={
             "max_depth": Integer("max_depth", (3, 10), default=6),
             "gamma": Float('gamma', (0, 9), default=0),
             'reg_alpha' : Integer('reg_alpha', (0, 180), default=0),
             'reg_lambda' : Float('reg_lambda', (0, 1), default=1),
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/__init__.py` & `sam_ml-py-0.8.0/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/main_classifier.py` & `sam_ml-py-0.8.0/sam_ml/models/main_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import sys
+import warnings
 from datetime import timedelta
 from statistics import mean
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from ConfigSpace import Configuration, ConfigurationSpace
@@ -10,24 +13,34 @@
     accuracy_score,
     classification_report,
     make_scorer,
     precision_score,
     recall_score,
 )
 from sklearn.model_selection import cross_validate
-from smac import HyperparameterOptimizationFacade, Scenario
 from tqdm.auto import tqdm
 
-from sam_ml.config import setup_logger
+from sam_ml.config import get_n_jobs, setup_logger
 
 from .main_model import Model
 from .scorer import l_scoring, s_scoring
 
+SMAC_INSTALLED: bool
+try:
+    from smac import HyperparameterOptimizationFacade, Scenario
+    SMAC_INSTALLED = True
+except:
+    SMAC_INSTALLED = False
+
 logger = setup_logger(__name__)
 
+if not sys.warnoptions:
+    warnings.simplefilter("ignore")
+    os.environ["PYTHONWARNINGS"] = "ignore" # Also affects subprocesses
+
 
 class Classifier(Model):
     """ Classifier parent class """
 
     def __init__(self, model_object = None, model_name: str = "classifier", model_type: str = "Classifier", grid: ConfigurationSpace = ConfigurationSpace()):
         """
         @params:
@@ -248,15 +261,15 @@
         cv_scores = cross_validate(
             self,
             X,
             y,
             scoring=scorer,
             cv=cv_num,
             return_train_score=True,
-            n_jobs=-1,
+            n_jobs=get_n_jobs(),
         )
 
         pd_scores = pd.DataFrame(cv_scores).transpose()
         pd_scores["average"] = pd_scores.mean(numeric_only=True, axis=1)
 
         score = pd_scores["average"]
         self.cv_scores = {
@@ -425,17 +438,20 @@
             
             walltime_limit: the maximum time in seconds that SMAC is allowed to run
 
             log_level: 10 - DEBUG, 20 - INFO, 30 - WARNING, 40 - ERROR, 50 - CRITICAL (SMAC3 library log levels)
 
         @return: ConfigSpace.Configuration with best hyperparameters (can be used like dict)
         """
+        if not SMAC_INSTALLED:
+            raise ImportError("SMAC3 library is not installed -> follow instructions in Repo to install SMAC3 (https://github.com/Priapos1004/SAM_ML)")
+
         logger.debug("starting smac_search")
-        # NormalInteger in grid are not supported (using workaround for now)
-        if self.model_type in ("RFC", "ETC", "GBM", "XGBC"):
+        # NormalInteger and EqualsCondition in grid are not supported (using workaround for now) (04/07/2023)
+        if self.model_type in ("RFC", "ETC", "GBM", "XGBC", "LR"):
             grid = self.smac_grid
         else:
             grid = self.grid
 
         scenario = Scenario(
             grid,
             n_trials=n_trails,
```

### Comparing `sam_ml-py-0.7.3/sam_ml/models/main_model.py` & `sam_ml-py-0.8.0/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.8.0/sam_ml/models/main_pipeline.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml/models/scorer.py` & `sam_ml-py-0.8.0/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.3/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.8.0/sam_ml_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.7.3
+Version: 0.8.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: with_swig
 License-File: LICENSE
 
 # SAM_ML
 
 [![PyPI version](https://badge.fury.io/py/sam-ml-py.svg)](https://badge.fury.io/py/sam-ml-py)
 
 a library created by Samuel Brinkmann
 
-## getting started
+## getting started (with SMAC3 library)
 
 0. pre-installations *(needed for [smac](https://github.com/automl/SMAC3) library)*
 
 You need to install `swig` for the *smag* library that is used for hyperparameter tuning.
 
 Linux *(see [smac installation guide](https://automl.github.io/SMAC3/main/1_installation.html))*:
 
@@ -29,14 +30,24 @@
 
 MacOS (with [homebrew](https://formulae.brew.sh/formula/swig)):
 
 ```
 brew install swig
 ```
 
+Windows (see [swigwin](https://www.swig.org/download.html))
+
+1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
+
+```
+pip install sam-ml-py[with_swig]
+```
+
+## getting started (without SMAC3 library)
+
 1. install the package to your activated virtual environment *(python version 3.10 and higher is needed)*
 
 ```
 pip install sam-ml-py
 ```
 
 2. now you can import the package, e.g.:
```

### Comparing `sam_ml-py-0.7.3/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.8.0/sam_ml_py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 sam_ml/__init__.py
 sam_ml/config/__init__.py
+sam_ml/config/global_variables.py
 sam_ml/config/logging.py
 sam_ml/data/__init__.py
 sam_ml/data/embeddings.py
 sam_ml/data/feature_selection.py
 sam_ml/data/sampling.py
 sam_ml/data/scaler.py
 sam_ml/data/synthetic_data.py
```

### Comparing `sam_ml-py-0.7.3/setup.py` & `sam_ml-py-0.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.7.3",
+    version="0.8.0",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
     install_requires=[
-        "scikit-learn",
+        "scikit-learn<1.3", # version 1.3 has some issues currently (04/07/2023)
         "pandas",
         "matplotlib",
         "numpy",
         "imbalanced-learn",
         "pygame",
         "ipywidgets",
         "tqdm",
         "statsmodels",
         "sentence-transformers",
         "xgboost",
         "ConfigSpace", # for hyperparameter tuning spaces
-        "smac", # for hyperparameter tuning
     ],
-    extras_require={"test": ["pytest", "pylint!=2.5.0", "isort", "refurb", "black"],},
+    extras_require={"test": ["pytest", "pylint", "isort", "refurb", "black"],
+                    "with_swig": ["smac"]},
     author="Samuel Brinkmann",
     license="MIT",
-    tests_require=["pytest==4.4.1"],
+    tests_require=["pytest"],
     setup_requires=["pytest-runner"],
 )
```

