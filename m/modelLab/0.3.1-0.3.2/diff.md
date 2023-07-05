# Comparing `tmp/modelLab-0.3.1.tar.gz` & `tmp/modelLab-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelLab-0.3.1.tar", last modified: Wed Jul  5 16:46:09 2023, max compression
+gzip compressed data, was "modelLab-0.3.2.tar", last modified: Wed Jul  5 16:53:49 2023, max compression
```

## Comparing `modelLab-0.3.1.tar` & `modelLab-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 16:45:53.000000 modelLab-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-05 16:46:09.462054 modelLab-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-07-05 16:45:53.000000 modelLab-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/Classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Classification/classification_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab/Regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/Regression/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 16:45:53.000000 modelLab-0.3.1/modelLab/initial_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:46:09.462054 modelLab-0.3.1/modelLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:46:09.000000 modelLab-0.3.1/modelLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:46:09.462054 modelLab-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-05 16:45:53.000000 modelLab-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:53:49.247401 modelLab-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 16:53:34.000000 modelLab-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-05 16:53:49.243401 modelLab-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-05 16:53:34.000000 modelLab-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:53:49.243401 modelLab-0.3.2/modelLab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:53:49.243401 modelLab-0.3.2/modelLab/Classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Classification/classification_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:53:49.243401 modelLab-0.3.2/modelLab/Regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/Regression/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 16:53:34.000000 modelLab-0.3.2/modelLab/initial_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:53:49.243401 modelLab-0.3.2/modelLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-07-05 16:53:49.000000 modelLab-0.3.2/modelLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:53:49.000000 modelLab-0.3.2/modelLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:53:49.000000 modelLab-0.3.2/modelLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:53:49.000000 modelLab-0.3.2/modelLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:53:49.000000 modelLab-0.3.2/modelLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:53:49.247401 modelLab-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-05 16:53:34.000000 modelLab-0.3.2/setup.py
```

### Comparing `modelLab-0.3.1/LICENSE` & `modelLab-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/PKG-INFO` & `modelLab-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelLab
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lib for automating model training process of choosing best model that works for you data
 Home-page: https://github.com/Abhishekkaddipudi/modelLab
 Author: Abhishek Kaddipudi
 Author-email: abhishekkaddipudi007@gmail.com
 Keywords: automl,model,modelbuilder,modelLab
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
-.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=mail
 .. _Mail: mailto:abhishekkaddipudi123@gmail.com
 
 .. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
 .. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
 
 
 **modelLab** is a comprehensive library of machine learning models
@@ -469,10 +469,10 @@
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
 
 Contributor and Author
 ======================
-|Mail|_ |Linkedin|_
+|Mail|_   |Linkedin|_
 
    [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3.1/README.rst` & `modelLab-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
-.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=mail
 .. _Mail: mailto:abhishekkaddipudi123@gmail.com
 
 .. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
 .. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
 
 
 **modelLab** is a comprehensive library of machine learning models
@@ -451,10 +451,10 @@
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
 
 Contributor and Author
 ======================
-|Mail|_ |Linkedin|_
+|Mail|_   |Linkedin|_
 
    [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3.1/modelLab/Classification/__init__.py` & `modelLab-0.3.2/modelLab/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/Classification/classification.py` & `modelLab-0.3.2/modelLab/Classification/classification.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/Classification/classification_metrics.py` & `modelLab-0.3.2/modelLab/Classification/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/Regression/__init__.py` & `modelLab-0.3.2/modelLab/Regression/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/Regression/regression.py` & `modelLab-0.3.2/modelLab/Regression/regression.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/Regression/regression_metrics.py` & `modelLab-0.3.2/modelLab/Regression/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/__init__.py` & `modelLab-0.3.2/modelLab/__init__.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab/initial_checks.py` & `modelLab-0.3.2/modelLab/initial_checks.py`

 * *Files identical despite different names*

### Comparing `modelLab-0.3.1/modelLab.egg-info/PKG-INFO` & `modelLab-0.3.2/modelLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelLab
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lib for automating model training process of choosing best model that works for you data
 Home-page: https://github.com/Abhishekkaddipudi/modelLab
 Author: Abhishek Kaddipudi
 Author-email: abhishekkaddipudi007@gmail.com
 Keywords: automl,model,modelbuilder,modelLab
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 .. |Version| image:: https://img.shields.io/badge/Version-V0.1-blue
 .. _Version: https://github.com/Abhishekkaddipudi/modelLab
 
 .. |Unit_Test| image:: https://github.com/Abhishekkaddipudi/modelLab/actions/workflows/main.yml/badge.svg
 .. _Unit_Test: https://github.com/Abhishekkaddipudi/modelLab
 
-.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=Gmail
+.. |Mail| image:: https://img.shields.io/badge/MailID-lightgrey?style=for-the-badge&logo=mail
 .. _Mail: mailto:abhishekkaddipudi123@gmail.com
 
 .. |Linkedin| image:: https://img.shields.io/badge/Linkedin-darkblue?style=for-the-badge&logo=Linkedin
 .. _Linkedin: https://www.linkedin.com/in/abhishek-kaddipudi-0b5183253/
 
 
 **modelLab** is a comprehensive library of machine learning models
@@ -469,10 +469,10 @@
    >>> models = {'Logistic Regression': LogisticRegression()}  
    >>> classifier(X, y, models=models, verbose=False, rets=True)
    defaultdict(<class 'dict'>, {'Logistic Regression': {'Accuracy': 0.95, 'Precision': 0.9545454545454545, 'Recall': 0.95, 'F1 Score': 0.949874686716792}})
 
 
 Contributor and Author
 ======================
-|Mail|_ |Linkedin|_
+|Mail|_   |Linkedin|_
 
    [**Abhishek Kaddipudi**]
```

### Comparing `modelLab-0.3.1/setup.py` & `modelLab-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 import os
 
 REQUIREMENT_FILE_NAME="requirements.txt"
 Project_Name="modelLab"
-Version="0.3.1"
+Version="0.3.2"
 AUTHOR="Abhishek Kaddipudi"
 DESCRIPTION="A lib for automating model training process of choosing best model that works for you data"
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

