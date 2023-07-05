# Comparing `tmp/modelLab-0.3.tar.gz` & `tmp/modelLab-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelLab-0.3.tar", last modified: Wed Jul  5 16:13:00 2023, max compression
+gzip compressed data, was "modelLab-0.3.1.tar", last modified: Wed Jul  5 16:46:09 2023, max compression
```

## Comparing `modelLab-0.3.tar` & `modelLab-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:13:00.535422 modelLab-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 16:12:43.000000 modelLab-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-05 16:13:00.535422 modelLab-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-05 16:12:43.000000 modelLab-0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:13:00.535422 modelLab-0.3/modelLab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:13:00.535422 modelLab-0.3/modelLab/Classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Classification/classification_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:13:00.535422 modelLab-0.3/modelLab/Regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/Regression/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 16:12:43.000000 modelLab-0.3/modelLab/initial_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:13:00.535422 modelLab-0.3/modelLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-05 16:13:00.000000 modelLab-0.3/modelLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:13:00.000000 modelLab-0.3/modelLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:13:00.000000 modelLab-0.3/modelLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:13:00.000000 modelLab-0.3/modelLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:13:00.000000 modelLab-0.3/modelLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:13:00.535422 modelLab-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-05 16:12:43.000000 modelLab-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 16:45:53.000000 modelLab-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-05 16:46:09.462054 modelLab-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-05 16:45:53.000000 modelLab-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/Classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/classification_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/Regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/initial_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:46:09.462054 modelLab-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-05 16:45:53.000000 modelLab-0.3.1/setup.py
```

### Comparing `modelLab-0.3/LICENSE` & `modelLab-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/PKG-INFO` & `modelLab-0.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-Metadata-Version: 2.1
-Name: modelLab
-Version: 0.3
-Summary: A lib for automating model training process of choosing best model that works for you data
-Home-page: https://github.com/Abhishekkaddipudi/modelLab
-Author: Abhishek Kaddipudi
-Author-email: abhishekkaddipudi007@gmail.com
-Keywords: automl,model,modelbuilder,modelLab
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-
 .. -*- mode: rst -*-
 
 |Version|_ |PythonVersion|_
 
 
 .. |PythonVersion| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue
 .. _PythonVersion: https://pypi.org/project/modelLab/
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. _Mail: mailto:abhishekkaddipudi123@gmail.com
+
+.. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
+.. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
+
+
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
 PURPOSE OF THE PACKAGE
@@ -459,7 +448,13 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+
+Contributor and Author
+======================
+|Mail|_ |Linkedin|_
+
+   [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3/README.rst` & `modelLab-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,46 @@
+Metadata-Version: 2.1
+Name: modelLab
+Version: 0.3.1
+Summary: A lib for automating model training process of choosing best model that works for you data
+Home-page: https://github.com/Abhishekkaddipudi/modelLab
+Author: Abhishek Kaddipudi
+Author-email: abhishekkaddipudi007@gmail.com
+Keywords: automl,model,modelbuilder,modelLab
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+
 .. -*- mode: rst -*-
 
 |Version|_ |PythonVersion|_
 
 
 .. |PythonVersion| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue
 .. _PythonVersion: https://pypi.org/project/modelLab/
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. _Mail: mailto:abhishekkaddipudi123@gmail.com
+
+.. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
+.. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
+
+
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
 PURPOSE OF THE PACKAGE
@@ -441,7 +466,13 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+
+Contributor and Author
+======================
+|Mail|_ |Linkedin|_
+
+   [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3/modelLab/Classification/__init__.py` & `modelLab-0.3.1/modelLab/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/Classification/classification.py` & `modelLab-0.3.1/modelLab/Classification/classification.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/Classification/classification_metrics.py` & `modelLab-0.3.1/modelLab/Classification/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/Regression/__init__.py` & `modelLab-0.3.1/modelLab/Regression/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/Regression/regression.py` & `modelLab-0.3.1/modelLab/Regression/regression.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/Regression/regression_metrics.py` & `modelLab-0.3.1/modelLab/Regression/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/__init__.py` & `modelLab-0.3.1/modelLab/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab/initial_checks.py` & `modelLab-0.3.1/modelLab/initial_checks.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3/modelLab.egg-info/PKG-INFO` & `modelLab-0.3.1/modelLab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelLab
-Version: 0.3
+Version: 0.3.1
 Summary: A lib for automating model training process of choosing best model that works for you data
 Home-page: https://github.com/Abhishekkaddipudi/modelLab
 Author: Abhishek Kaddipudi
 Author-email: abhishekkaddipudi007@gmail.com
 Keywords: automl,model,modelbuilder,modelLab
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -26,14 +26,21 @@
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. _Mail: mailto:abhishekkaddipudi123@gmail.com
+
+.. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
+.. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
+
+
 **modelLab** is a comprehensive library of machine learning models
 designed to facilitate regression or classification tasks on a given
 dataset. It encompasses a diverse range of models and provides a
 comprehensive evaluation of each model's performance, delivering a
 comprehensive set of metrics in a Python dictionary.
 
 PURPOSE OF THE PACKAGE
@@ -459,7 +466,13 @@
    >>> from sklearn.linear_model import LogisticRegression
    >>> from modelLab import classifier
    >>> X, y = make_classification(n_samples=100, n_features=10, random_state=42)
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
+
+Contributor and Author
+======================
+|Mail|_ |Linkedin|_
+
+   [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3/setup.py` & `modelLab-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 import os
 
 REQUIREMENT_FILE_NAME="requirements.txt"
 Project_Name="modelLab"
-Version="0.3"
+Version="0.3.1"
 AUTHOR="Abhishek Kaddipudi"
 DESCRIPTION="A lib for automating model training process of choosing best model that works for you data"
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

