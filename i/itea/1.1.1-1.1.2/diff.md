# Comparing `tmp/itea-1.1.1.tar.gz` & `tmp/itea-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itea-1.1.1.tar", last modified: Thu Jul  7 11:12:55 2022, max compression
+gzip compressed data, was "itea-1.1.2.tar", last modified: Wed Jul  5 13:17:24 2023, max compression
```

## Comparing `itea-1.1.1.tar` & `itea-1.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     1524 2021-06-13 21:30:49.000000 itea-1.1.1/LICENSE
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1755 2022-07-07 11:12:55.000000 itea-1.1.1/PKG-INFO
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     9592 2022-01-25 21:15:16.000000 itea-1.1.1/README.md
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      597 2021-06-01 18:40:11.000000 itea-1.1.1/itea/__init__.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/_base/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    19067 2022-07-05 16:32:15.000000 itea-1.1.1/itea/_base/_BaseITEA.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    13019 2022-07-06 13:26:34.000000 itea-1.1.1/itea/_base/_BaseITExpr.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      526 2021-06-13 23:13:52.000000 itea-1.1.1/itea/_base/__init__.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/_manipulators/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      487 2021-05-31 21:16:17.000000 itea-1.1.1/itea/_manipulators/__init__.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     1318 2021-06-25 17:17:22.000000 itea-1.1.1/itea/_manipulators/generator.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     5012 2021-06-05 14:21:02.000000 itea-1.1.1/itea/_manipulators/mutation.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     1047 2021-06-05 14:22:28.000000 itea-1.1.1/itea/_manipulators/sanitizer.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     2904 2021-06-25 13:12:44.000000 itea-1.1.1/itea/_manipulators/simplifier.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/classification/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    11012 2021-11-26 19:34:06.000000 itea-1.1.1/itea/classification/_ITEA_classifier.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    17414 2022-07-06 12:42:56.000000 itea-1.1.1/itea/classification/_ITExpr_classifier.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      959 2021-06-13 23:42:42.000000 itea-1.1.1/itea/classification/__init__.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/inspection/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    28175 2021-11-26 18:43:24.000000 itea-1.1.1/itea/inspection/_ITEA_summarizer.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)    48164 2022-07-06 13:14:37.000000 itea-1.1.1/itea/inspection/_ITExpr_explainer.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     9298 2021-06-25 17:21:04.000000 itea-1.1.1/itea/inspection/_ITExpr_inspector.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     5721 2021-06-13 23:55:38.000000 itea-1.1.1/itea/inspection/_ITExpr_texifier.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     2109 2021-06-13 23:47:24.000000 itea-1.1.1/itea/inspection/__init__.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea/regression/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     8451 2021-11-26 19:33:46.000000 itea-1.1.1/itea/regression/_ITEA_regressor.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     9115 2022-07-05 15:41:12.000000 itea-1.1.1/itea/regression/_ITExpr_regressor.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      932 2021-06-13 23:38:20.000000 itea-1.1.1/itea/regression/__init__.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     1755 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/PKG-INFO
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      968 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/SOURCES.txt
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)        1 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/dependency_links.txt
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)      139 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/requires.txt
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)       11 2022-07-07 11:12:55.000000 itea-1.1.1/itea.egg-info/top_level.txt
--rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       38 2022-07-07 11:12:55.000000 itea-1.1.1/setup.cfg
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     1587 2022-07-07 11:12:50.000000 itea-1.1.1/setup.py
-drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2022-07-07 11:12:55.000000 itea-1.1.1/tests/
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)        0 2021-06-16 23:59:29.000000 itea-1.1.1/tests/__init__.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     5935 2021-07-19 15:51:41.000000 itea-1.1.1/tests/test_BaseITEA.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     6619 2021-11-26 15:04:19.000000 itea-1.1.1/tests/test_BaseITExpr.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     8014 2022-07-05 16:03:14.000000 itea-1.1.1/tests/test_classifier.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     3897 2021-06-25 13:26:10.000000 itea-1.1.1/tests/test_manipulators.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     4909 2021-06-13 13:31:25.000000 itea-1.1.1/tests/test_mutations.py
--rwxrwxrwx   0 guilherme  (1000) guilherme  (1000)     8439 2022-07-05 16:03:31.000000 itea-1.1.1/tests/test_regressor.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.714665 itea-1.1.2/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1524 2021-06-13 21:30:49.000000 itea-1.1.2/LICENSE
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1911 2023-07-05 13:17:24.714665 itea-1.1.2/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    10797 2023-07-04 15:47:22.000000 itea-1.1.2/README.md
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      597 2021-06-01 18:40:11.000000 itea-1.1.2/itea/__init__.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/_base/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    19067 2022-07-05 16:32:15.000000 itea-1.1.2/itea/_base/_BaseITEA.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    13019 2022-07-06 13:26:34.000000 itea-1.1.2/itea/_base/_BaseITExpr.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      526 2021-06-13 23:13:52.000000 itea-1.1.2/itea/_base/__init__.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/_manipulators/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      487 2021-05-31 21:16:17.000000 itea-1.1.2/itea/_manipulators/__init__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1318 2021-06-25 17:17:22.000000 itea-1.1.2/itea/_manipulators/generator.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     5012 2021-06-05 14:21:02.000000 itea-1.1.2/itea/_manipulators/mutation.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1047 2021-06-05 14:22:28.000000 itea-1.1.2/itea/_manipulators/sanitizer.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     2904 2021-06-25 13:12:44.000000 itea-1.1.2/itea/_manipulators/simplifier.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/classification/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    11012 2021-11-26 19:34:06.000000 itea-1.1.2/itea/classification/_ITEA_classifier.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    17411 2023-07-02 17:23:15.000000 itea-1.1.2/itea/classification/_ITExpr_classifier.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      959 2021-06-13 23:42:42.000000 itea-1.1.2/itea/classification/__init__.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/inspection/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    28175 2021-11-26 18:43:24.000000 itea-1.1.2/itea/inspection/_ITEA_summarizer.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)    48164 2022-07-06 13:14:37.000000 itea-1.1.2/itea/inspection/_ITExpr_explainer.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     9298 2021-06-25 17:21:04.000000 itea-1.1.2/itea/inspection/_ITExpr_inspector.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     5721 2021-06-13 23:55:38.000000 itea-1.1.2/itea/inspection/_ITExpr_texifier.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     2109 2023-07-02 18:27:43.000000 itea-1.1.2/itea/inspection/__init__.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea/regression/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     8451 2021-11-26 19:33:46.000000 itea-1.1.2/itea/regression/_ITEA_regressor.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     9115 2022-07-05 15:41:12.000000 itea-1.1.2/itea/regression/_ITExpr_regressor.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      932 2021-06-13 23:38:20.000000 itea-1.1.2/itea/regression/__init__.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.710665 itea-1.1.2/itea.egg-info/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1911 2023-07-05 13:17:24.000000 itea-1.1.2/itea.egg-info/PKG-INFO
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)      968 2023-07-05 13:17:24.000000 itea-1.1.2/itea.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        1 2023-07-05 13:17:24.000000 itea-1.1.2/itea.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       60 2023-07-05 13:17:24.000000 itea-1.1.2/itea.egg-info/requires.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       11 2023-07-05 13:17:24.000000 itea-1.1.2/itea.egg-info/top_level.txt
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)       38 2023-07-05 13:17:24.714665 itea-1.1.2/setup.cfg
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     1357 2023-07-05 13:09:06.000000 itea-1.1.2/setup.py
+drwxrwxr-x   0 guilherme  (1000) guilherme  (1000)        0 2023-07-05 13:17:24.714665 itea-1.1.2/tests/
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)        0 2021-06-16 23:59:29.000000 itea-1.1.2/tests/__init__.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     5935 2021-07-19 15:51:41.000000 itea-1.1.2/tests/test_BaseITEA.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     6610 2023-07-02 17:24:25.000000 itea-1.1.2/tests/test_BaseITExpr.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     8002 2023-07-02 17:33:00.000000 itea-1.1.2/tests/test_classifier.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     3897 2021-06-25 13:26:10.000000 itea-1.1.2/tests/test_manipulators.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     4909 2021-06-13 13:31:25.000000 itea-1.1.2/tests/test_mutations.py
+-rw-rw-r--   0 guilherme  (1000) guilherme  (1000)     8430 2023-07-02 17:24:30.000000 itea-1.1.2/tests/test_regressor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `itea-1.1.1/LICENSE` & `itea-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/PKG-INFO` & `itea-1.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: itea
-Version: 1.1.1
+Version: 1.1.2
 Summary: Interaction-Transformation Evolutionary Algorithm for Symbolic Regression.
-Home-page: UNKNOWN
 Author: Guilherme Aldeia
 Author-email: guilherme.aldeia@ufabc.edu.br
 License: BSD-3-Clause
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # itea-python
 
 <img src="https://galdeia.github.io/itea-python/_static/itea-logo.png" alt="drawing" width="300"/><br>
@@ -34,13 +32,13 @@
 model-specific explainer based on the Partial Effects to help users get a
 better understanding of the resulting expressions.
 
 This implementation is based on the scikit-learn package and the implementations
 of the estimators follow their guidelines.
 
 
+> **OBS:** There also exists a [high-performing Haskell implementation (that comes with a python wrapper)](https://github.com/folivetti/ITEA) by [@folivetti](https://github.com/folivetti/ITEA).
+
 ## Documentation
 
 Documentation is available at [readthedocs](https://itea-python.readthedocs.io/en/latest).
 
-
-
```

### Comparing `itea-1.1.1/README.md` & `itea-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 model-specific explainer based on the Partial Effects to help users get a
 better understanding of the resulting expressions.
 
 This implementation is based on the scikit-learn package and the implementations
 of the estimators follow their guidelines.
 
 
+> **OBS:** There also exists a [high-performing Haskell implementation (that comes with a python wrapper)](https://github.com/folivetti/ITEA) by [@folivetti](https://github.com/folivetti/ITEA).
+
 ## Documentation
 
 Documentation is available at [readthedocs](https://itea-python.readthedocs.io/en/latest).
 
 -----
 
 ## Installation
@@ -43,15 +45,35 @@
 Alternatively, you can download the source code at the 
 [itea-python GitHub page](https://github.com/gAldeia/itea-python) and run:
 
 ```shell
 $ pip install .
 ```
 
-> **NOTE:** If pip fails to install the latest version, you will need to update `pip` and `setuptools`, and install an older version of `docutils<0.18` (such as v0.17.1).
+Additionally, you can install it inside a conda environment. First create the environment:
+
+```shell 
+conda create --name itea-python python=3.10
+```
+
+Then activate the environment:
+
+```shell
+conda activate itea-python
+```
+
+and install the `itea` by using one of the options above (`pip install itea` or `pip install .`).
+
+> **NOTE:** to run the **tests**, build **the documentation**, **profile** the code and execute a simple **benchmark**, you may need to install some requirements. If you want to do so, first you need to install itea in a conda environment. Then, inside the environment:
+>
+> ```pip install -r requirements.txt```
+>
+> You will also need to have a \LaTeX compiler and pandoc installed to build the docs.
+>
+> There is a `Makefile` at the root of this repository that contains simple macros to run these commands (or you can simply call `make`) and everything will be executed. There is a dedicated section for each additional highlighted resource at the end of this markdown. 
 
 ## Using the ITEA algorithm
 
 Before jumping into using the library, here are some tips and examples
 that might make it easier to use.
 
 ITEA can be used for regression (with the ``ITEA_regressor`` class) or
@@ -121,15 +143,19 @@
 
 # yields the same result as the previous line
 reg.predict(X_reg)
 ```
 
 The ITEA Package also implements some classes focused on interpretability,
 providing mechanisms to inspect and better understand the returned symbolic
-expressions. We can obtain importance values ​​from expression attributes and
+expressions.
+
+> **NOTE:** in order to generate the reports, you'll need to have a \LaTeX compiler installed locally. You can go with `pdfLaTex` if you don't have any, since it is easy to install.
+
+We can obtain importance values ​​from expression attributes and
 even generate graphs:
 
 ```python
 explainer = ITExpr_explainer(
     itexpr=final_itexpr, tfuncs=reg.tfuncs).fit(X_reg, y_reg)
 
 explainer.plot_feature_importances(
@@ -139,15 +165,17 @@
     barh_kw={'color':'green'}
 )
 ```
 
 ![feature importances plot](https://galdeia.github.io/itea-python/_images/_regression_example_17_0.png)
 
 Explainers do not inherit any scikit interfaces, but implements a similar usage.
-So, the steps to use the explainers are: 1. Instanciate the explainer; 2. Fit;
+So, the steps to use the explainers are:
+1. Instanciate the explainer;
+2. Fit;
 3. Generate the plots.
 
 That said, if you're familiar with scikit's ecosystem of regressors and
 classifiers, you'll have no problem using ITEA and its explainers.
 
 For more examples, see:
 
@@ -258,8 +286,8 @@
         "Explaining Symbolic Regression Predictions," 2020 IEEE Congress on
         Evolutionary Computation (CEC)._
 
 
 ## Contributing
 
 This is still in active development. Feel free to contact the developers with
-suggestions, critics, or questions. You can always raise an issue on GitHub!
+suggestions, critics, or questions. You can always raise an issue on GitHub!
```

### Comparing `itea-1.1.1/itea/__init__.py` & `itea-1.1.2/itea/__init__.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_base/_BaseITEA.py` & `itea-1.1.2/itea/_base/_BaseITEA.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_base/_BaseITExpr.py` & `itea-1.1.2/itea/_base/_BaseITExpr.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_base/__init__.py` & `itea-1.1.2/itea/_base/__init__.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_manipulators/generator.py` & `itea-1.1.2/itea/_manipulators/generator.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_manipulators/mutation.py` & `itea-1.1.2/itea/_manipulators/mutation.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_manipulators/sanitizer.py` & `itea-1.1.2/itea/_manipulators/sanitizer.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/_manipulators/simplifier.py` & `itea-1.1.2/itea/_manipulators/simplifier.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/classification/_ITEA_classifier.py` & `itea-1.1.2/itea/classification/_ITEA_classifier.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/classification/_ITExpr_classifier.py` & `itea-1.1.2/itea/classification/_ITExpr_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             # Estimating as a one vs all classification for each class
             prob_class1 = probs[:, class_id]
             prob_class0 = np.sum(
                 probs[:, [i for i in range(len(self.classes_))
                     if i != class_id]],
                 axis=1)
 
-            V = np.diagflat(np.product([prob_class0, prob_class1], axis=0))
+            V = np.diagflat(np.prod([prob_class0, prob_class1], axis=0))
 
             try:
                 covars[class_id, :, :] = np.linalg.inv(
                     X_design.T @ V @ X_design)
             except np.linalg.LinAlgError as e:
                 # singular matrix, lets use the pseudo inverse
                 covars[class_id, :, :] = np.linalg.pinv(
```

### Comparing `itea-1.1.1/itea/classification/__init__.py` & `itea-1.1.2/itea/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/inspection/_ITEA_summarizer.py` & `itea-1.1.2/itea/inspection/_ITEA_summarizer.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/inspection/_ITExpr_explainer.py` & `itea-1.1.2/itea/inspection/_ITExpr_explainer.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/inspection/_ITExpr_inspector.py` & `itea-1.1.2/itea/inspection/_ITExpr_inspector.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/inspection/_ITExpr_texifier.py` & `itea-1.1.2/itea/inspection/_ITExpr_texifier.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/inspection/__init__.py` & `itea-1.1.2/itea/inspection/__init__.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/regression/_ITEA_regressor.py` & `itea-1.1.2/itea/regression/_ITEA_regressor.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/regression/_ITExpr_regressor.py` & `itea-1.1.2/itea/regression/_ITExpr_regressor.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea/regression/__init__.py` & `itea-1.1.2/itea/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/itea.egg-info/PKG-INFO` & `itea-1.1.2/itea.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: itea
-Version: 1.1.1
+Version: 1.1.2
 Summary: Interaction-Transformation Evolutionary Algorithm for Symbolic Regression.
-Home-page: UNKNOWN
 Author: Guilherme Aldeia
 Author-email: guilherme.aldeia@ufabc.edu.br
 License: BSD-3-Clause
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # itea-python
 
 <img src="https://galdeia.github.io/itea-python/_static/itea-logo.png" alt="drawing" width="300"/><br>
@@ -34,13 +32,13 @@
 model-specific explainer based on the Partial Effects to help users get a
 better understanding of the resulting expressions.
 
 This implementation is based on the scikit-learn package and the implementations
 of the estimators follow their guidelines.
 
 
+> **OBS:** There also exists a [high-performing Haskell implementation (that comes with a python wrapper)](https://github.com/folivetti/ITEA) by [@folivetti](https://github.com/folivetti/ITEA).
+
 ## Documentation
 
 Documentation is available at [readthedocs](https://itea-python.readthedocs.io/en/latest).
 
-
-
```

### Comparing `itea-1.1.1/itea.egg-info/SOURCES.txt` & `itea-1.1.2/itea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/setup.py` & `itea-1.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,43 @@
 from setuptools import find_packages, setup
 
 description = open('README.md', encoding='utf-8').read()
 
 setup(
     name             = "itea",
     packages         = find_packages(),
-    version          = "1.1.1",
+    version          = "1.1.2",
     description      = ("Interaction-Transformation Evolutionary Algorithm "
                         "for Symbolic Regression."),
     # Only the "introduction" in README (text below the horizontal rule)
     long_description = description[:description.find('-----')],
     long_description_content_type = 'text/markdown',
     author           = "Guilherme Aldeia",
-    author_email="guilherme.aldeia@ufabc.edu.br",
+    author_email     = "guilherme.aldeia@ufabc.edu.br",
     license          = "BSD-3-Clause",
     install_requires = [
-        "numpy>=1.18.2",
-        "scikit-learn>=0.23.1",
-        "matplotlib>=3.2.2",
-        "pandas>=1.1.0",
-        "jax>=0.2.13",
-        "jaxlib>=0.1.67",
-        "scipy>=1.5.2",
-        "pylatex==1.4.1",
-        "docutils==0.17.1"
+        # ITEA core
+        "numpy",        # >=1.18.2
+        "scikit-learn", # >=1.0.0
+        "jax[cpu]",
+        "scipy",        # >=1.5.2
+
+        # ITEA summarizer
+        "matplotlib",   # >=3.2.2
+        "pandas",       # >=1.1.0
+        "pylatex"       # >=1.4.1
     ],
     package_data = {'examples' : ['examples']},
     include_package_data = True,
     python_requires = '>=3.7',
     setup_requires  = [
-        "wheel",
-        "pytest-runner",
-        "coverage",
-        "coverage-badge",
-
-        #required to build the docs
-        "Jinja2==2.11",  
-        "nbsphinx"
+        "setuptools",
+        "wheel"
     ],
 
     # Aditional packages not included in install requires
     tests_require   = [
-        # Used in tests
-        "pytest",
-        "pytest-html",
-
-        # Used in profiling
-        "snakeviz",
-
-        # Used in benchmarking
-        "filelock"
-        ],
+        "pytest-runner",
+        "pytest"
+    ],
     test_suite = "tests",
 )
```

### Comparing `itea-1.1.1/tests/test_BaseITEA.py` & `itea-1.1.2/tests/test_BaseITEA.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/tests/test_BaseITExpr.py` & `itea-1.1.2/tests/test_BaseITExpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 def test_linear_BaseITExpr_eval(linear_baseITExpr, sample_data):
 
     X, _ = sample_data
 
     # it should be the same matrix, since _eval returns a matrix where each
     # column is one it term, and the it expression is a linear combination
     # of the features, using onli the identity function as transformation func
-    assert np.array_equal(linear_baseITExpr._eval(X), X) 
+    assert np.allclose(linear_baseITExpr._eval(X), X) 
 
 
 def test_linear_BaseITExpr_complexity(linear_baseITExpr):
     # calculated by hand, the expected complexity is 26, the number of nodes
     # needed to recreate the it expression as a symbolic expression
 
     assert linear_baseITExpr.complexity() == 26
@@ -135,15 +135,15 @@
         for c_idx in range(expected_gradients.shape[0]):
             for x_idx in range(expected_gradients.shape[2]): # number of variables
                 expected_gradients[c_idx, :, x_idx] = np.divide(
                     np.exp(predictions)[:, c_idx] * expected_gradients[c_idx, :, x_idx],
                     np.power(np.exp(predictions)[:, c_idx] + 1.0, 2)
                 )
 
-    assert np.array_equal(
+    assert np.allclose(
         linear_baseITExpr.gradient(
             X,
             tfuncs_dx = {'id': lambda x: np.ones_like(x)},
             logit = logit
         ),
         expected_gradients
     )
@@ -174,15 +174,15 @@
         for c_idx in range(expected_gradients.shape[0]):
             for x_idx in range(expected_gradients.shape[2]): # number of variables
                 expected_gradients[c_idx, :, x_idx] = np.divide(
                     np.exp(predictions)[:, c_idx] * expected_gradients[c_idx, :, x_idx],
                     np.power(np.exp(predictions)[:, c_idx] + 1.0, 2)
                 )
 
-    assert np.array_equal(
+    assert np.allclose(
         nonlinear_baseITExpr.gradient(
             X,
             tfuncs_dx = {'id': lambda x: np.ones_like(x)},
             logit = logit
         ),
         expected_gradients
     )
```

### Comparing `itea-1.1.1/tests/test_classifier.py` & `itea-1.1.2/tests/test_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     with pytest.raises(NotFittedError):
         linear_ITExpr.predict_proba(X)
 
     linear_ITExpr.fit(X, y)
 
     assert np.array(linear_ITExpr.coef_).ndim == 2
     assert np.array(linear_ITExpr.intercept_).ndim == 1
-    assert np.array_equal(linear_ITExpr.classes_,  [0, 1, 2])
+    assert np.allclose(linear_ITExpr.classes_,  [0, 1, 2])
 
     # Shoudnt raise an error anymore    
     linear_ITExpr.predict(X)
 
     # The ITExpr is exactly the same original expresison. must have almost
     # perfect results.
     assert np.isclose(linear_ITExpr._fitness, 1.0)
@@ -134,17 +134,17 @@
         multi_class='multinomial',
         penalty='none',
         random_state=42
     ).fit(X, y)
 
     # They should give the exact same coefficients and intercept, with same
     # shapes and vales, and even have the score() function with same return val
-    assert np.array_equal(itexpr_clf.coef_, scikit_clf.coef_)
-    assert np.array_equal(itexpr_clf.intercept_, scikit_clf.intercept_)
-    assert np.array_equal(itexpr_clf.score(X, y), scikit_clf.score(X, y))
+    assert np.allclose(itexpr_clf.coef_, scikit_clf.coef_)
+    assert np.allclose(itexpr_clf.intercept_, scikit_clf.intercept_)
+    assert np.allclose(itexpr_clf.score(X, y), scikit_clf.score(X, y))
 
 
 def test_linear_ITExpr_predict(
     linear_ITExpr, classification_toy_data):
 
     X, y = classification_toy_data
```

### Comparing `itea-1.1.1/tests/test_manipulators.py` & `itea-1.1.2/tests/test_manipulators.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/tests/test_mutations.py` & `itea-1.1.2/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `itea-1.1.1/tests/test_regressor.py` & `itea-1.1.2/tests/test_regressor.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,17 +127,17 @@
     # Fitting the linear model, which will correspond to a linear regression
     itexpr_reg = linear_ITExpr.fit(X, y)
     
     scikit_reg = LinearRegression().fit(X, y)
 
     # They should give the exact same coefficients and intercept, with same
     # shapes and vales, and even have the score() function with same return val
-    assert np.array_equal(itexpr_reg.coef_, scikit_reg.coef_)
-    assert np.array_equal(itexpr_reg.intercept_, scikit_reg.intercept_)
-    assert np.array_equal(itexpr_reg.score(X, y), scikit_reg.score(X, y))
+    assert np.allclose(itexpr_reg.coef_, scikit_reg.coef_)
+    assert np.allclose(itexpr_reg.intercept_, scikit_reg.intercept_)
+    assert np.allclose(itexpr_reg.score(X, y), scikit_reg.score(X, y))
     
 
 
 def test_linear_ITExpr_predict(
     linear_ITExpr, regression_toy_data):
 
     X, y, coef = regression_toy_data
```

