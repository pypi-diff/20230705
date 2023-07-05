# Comparing `tmp/modelLab-0.1.tar.gz` & `tmp/modelLab-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelLab-0.1.tar", last modified: Wed Jul  5 16:01:03 2023, max compression
+gzip compressed data, was "modelLab-0.2.tar", last modified: Wed Jul  5 15:38:55 2023, max compression
```

## Comparing `modelLab-0.1.tar` & `modelLab-0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:01:03.989707 modelLab-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 16:00:49.000000 modelLab-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-05 16:01:03.989707 modelLab-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-05 16:00:49.000000 modelLab-0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:01:03.989707 modelLab-0.1/modelLab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:01:03.989707 modelLab-0.1/modelLab/Classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Classification/classification_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:01:03.989707 modelLab-0.1/modelLab/Regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/Regression/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 16:00:49.000000 modelLab-0.1/modelLab/initial_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:01:03.989707 modelLab-0.1/modelLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-05 16:01:03.000000 modelLab-0.1/modelLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:01:03.000000 modelLab-0.1/modelLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:01:03.000000 modelLab-0.1/modelLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:01:03.000000 modelLab-0.1/modelLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:01:03.000000 modelLab-0.1/modelLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:01:03.989707 modelLab-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-05 16:00:49.000000 modelLab-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:38:55.535530 modelLab-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 15:38:37.000000 modelLab-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-07-05 15:38:55.535530 modelLab-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-05 15:38:37.000000 modelLab-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:38:55.531530 modelLab-0.2/modelLab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:38:55.535530 modelLab-0.2/modelLab/Classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Classification/classification_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:38:55.535530 modelLab-0.2/modelLab/Regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/Regression/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 15:38:37.000000 modelLab-0.2/modelLab/initial_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:38:55.531530 modelLab-0.2/modelLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-07-05 15:38:55.000000 modelLab-0.2/modelLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 15:38:55.000000 modelLab-0.2/modelLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:38:55.000000 modelLab-0.2/modelLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 15:38:55.000000 modelLab-0.2/modelLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 15:38:55.000000 modelLab-0.2/modelLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:38:55.535530 modelLab-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-05 15:38:37.000000 modelLab-0.2/setup.py
```

### Comparing `modelLab-0.1/LICENSE` & `modelLab-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/PKG-INFO` & `modelLab-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 Metadata-Version: 2.1
 Name: modelLab
-Version: 0.1
+Version: 0.2
 Summary: A lib for automating model training process of choosing best model that works for you data
 Home-page: https://github.com/Abhishekkaddipudi/modelLab
 Author: Abhishek Kaddipudi
 Author-email: abhishekkaddipudi007@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
-.. -*- mode: rst -*-
-
-|Version|_ |PythonVersion|_
-
-
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue
-.. _PythonVersion: https://pypi.org/project/modelLab/
-
-.. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
-.. _Version: https://github.com/Abhishekkaddipudi/modelLab
-
-.. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
-.. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
+|Unit Test| —
 
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
@@ -458,7 +446,9 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+.. |Unit Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelLab-0.1/README.rst` & `modelLab-0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-.. -*- mode: rst -*-
-
-|Version|_ |PythonVersion|_
-
-
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue
-.. _PythonVersion: https://pypi.org/project/modelLab/
-
-.. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
-.. _Version: https://github.com/Abhishekkaddipudi/modelLab
-
-.. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
-.. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
+|Unit Test| —
 
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
@@ -441,7 +429,9 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+.. |Unit Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelLab-0.1/modelLab/Classification/__init__.py` & `modelLab-0.2/modelLab/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/Classification/classification.py` & `modelLab-0.2/modelLab/Classification/classification.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/Classification/classification_metrics.py` & `modelLab-0.2/modelLab/Classification/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/Regression/__init__.py` & `modelLab-0.2/modelLab/Regression/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/Regression/regression.py` & `modelLab-0.2/modelLab/Regression/regression.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/Regression/regression_metrics.py` & `modelLab-0.2/modelLab/Regression/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/__init__.py` & `modelLab-0.2/modelLab/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab/initial_checks.py` & `modelLab-0.2/modelLab/initial_checks.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.1/modelLab.egg-info/PKG-INFO` & `modelLab-0.2/modelLab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 Metadata-Version: 2.1
 Name: modelLab
-Version: 0.1
+Version: 0.2
 Summary: A lib for automating model training process of choosing best model that works for you data
 Home-page: https://github.com/Abhishekkaddipudi/modelLab
 Author: Abhishek Kaddipudi
 Author-email: abhishekkaddipudi007@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
-.. -*- mode: rst -*-
-
-|Version|_ |PythonVersion|_
-
-
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue
-.. _PythonVersion: https://pypi.org/project/modelLab/
-
-.. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
-.. _Version: https://github.com/Abhishekkaddipudi/modelLab
-
-.. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
-.. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
+|Unit Test| —
 
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
@@ -458,7 +446,9 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+.. |Unit Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `modelLab-0.1/setup.py` & `modelLab-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 import os
 
 REQUIREMENT_FILE_NAME="requirements.txt"
 Project_Name="modelLab"
-Version="0.1"
+Version="0.2"
 AUTHOR="Abhishek Kaddipudi"
 DESCRIPTION="A lib for automating model training process of choosing best model that works for you data"
 CLASSIFIERS = [
     'Development Status :: 1 - Planning',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

