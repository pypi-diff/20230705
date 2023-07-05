# Comparing `tmp/mdmpy-0.0.15.8.tar.gz` & `tmp/mdmpy-0.0.15.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mdmpy-0.0.15.8.tar", last modified: Mon Feb 11 07:36:42 2019, max compression
+gzip compressed data, was "dist\mdmpy-0.0.15.9.tar", last modified: Thu Feb 14 06:14:57 2019, max compression
```

## Comparing `mdmpy-0.0.15.8.tar` & `mdmpy-0.0.15.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/
--rw-rw-rw-   0        0        0     4636 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/PKG-INFO
--rw-rw-rw-   0        0        0     3453 2019-02-07 06:38:52.000000 mdmpy-0.0.15.8/README.md
--rw-rw-rw-   0        0        0       42 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/setup.cfg
--rw-rw-rw-   0        0        0      938 2019-02-11 07:36:12.000000 mdmpy-0.0.15.8/setup.py
-drwxrwxrwx   0        0        0        0 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/
-drwxrwxrwx   0        0        0        0 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy/
--rw-rw-rw-   0        0        0      165 2019-02-04 02:32:59.000000 mdmpy-0.0.15.8/src/mdmpy/__init__.py
--rw-rw-rw-   0        0        0    14512 2019-02-11 07:28:00.000000 mdmpy-0.0.15.8/src/mdmpy/example1.py
--rw-rw-rw-   0        0        0    12808 2019-02-11 07:35:09.000000 mdmpy-0.0.15.8/src/mdmpy/mdm.py
--rw-rw-rw-   0        0        0     3678 2019-02-11 06:48:20.000000 mdmpy-0.0.15.8/src/mdmpy/util.py
-drwxrwxrwx   0        0        0        0 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/
--rw-rw-rw-   0        0        0     4636 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/src/mdmpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-02-11 07:36:42.000000 mdmpy-0.0.15.8/test/
--rw-rw-rw-   0        0        0      492 2019-01-23 06:13:32.000000 mdmpy-0.0.15.8/test/test_util.py
+drwxrwxrwx   0        0        0        0 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/
+-rw-rw-rw-   0        0        0     5364 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4089 2019-02-14 06:08:33.000000 mdmpy-0.0.15.9/README.md
+-rw-rw-rw-   0        0        0       42 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/setup.cfg
+-rw-rw-rw-   0        0        0      974 2019-02-14 06:14:51.000000 mdmpy-0.0.15.9/setup.py
+drwxrwxrwx   0        0        0        0 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/
+drwxrwxrwx   0        0        0        0 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy/
+-rw-rw-rw-   0        0        0      165 2019-02-04 02:32:59.000000 mdmpy-0.0.15.9/src/mdmpy/__init__.py
+-rw-rw-rw-   0        0        0    15341 2019-02-14 06:10:27.000000 mdmpy-0.0.15.9/src/mdmpy/mdm.py
+-rw-rw-rw-   0        0        0     3676 2019-02-12 07:34:12.000000 mdmpy-0.0.15.9/src/mdmpy/util.py
+drwxrwxrwx   0        0        0        0 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/
+-rw-rw-rw-   0        0        0     5364 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/src/mdmpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-02-14 06:14:57.000000 mdmpy-0.0.15.9/test/
+-rw-rw-rw-   0        0        0      492 2019-01-23 06:13:32.000000 mdmpy-0.0.15.9/test/test_util.py
```

### Comparing `mdmpy-0.0.15.8/PKG-INFO` & `mdmpy-0.0.15.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: mdmpy
-Version: 0.0.15.8
+Version: 0.0.15.9
 Summary: A package that implements Marginal Distribution Models (MDMs)
 Home-page: https://github.com/justanothergithubber/mdmpy
 Author: mdmpy Authors
-Author-email: 3600019+justanothergithubber@users.noreply.github.com
+Author-email: mdmpyatgithub@gmail.com
 License: UNKNOWN
 Description: # MDM Py
         
         [![Documentation Status](https://readthedocs.org/projects/mdmpy/badge/?version=latest)](https://mdmpy.readthedocs.io/en/latest/?badge=latest)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/c13f603535364a7ba5a6a18ea6756a64)](https://app.codacy.com/app/justanothergithubber/mdmpy?utm_source=github.com&utm_medium=referral&utm_content=justanothergithubber/mdmpy&utm_campaign=Badge_Grade_Dashboard)
         [![PyPI version](https://badge.fury.io/py/mdmpy.svg)](https://badge.fury.io/py/mdmpy)
+        [![Project Status: WIP â€“ Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
         
         This package is a `Python` implementation of [Marginal Distribution Models](https://pubsonline.informs.org/doi/10.1287/mnsc.2014.1906) (MDMs), which can be used in Discrete Choice Modelling.
         
-        ## Install
+        ## Documentation
+        Documentation is kindly hosted by [Read The Docs](https://mdmpy.readthedocs.io/ "mdmpy Documentation").
         
+        ## Install
         This package is uploaded to [PyPI](https://pypi.org/ "Python Package Index"). Hence, 
         
         ```bat
         pip install mdmpy
         ```
         
         should work.
@@ -86,12 +89,19 @@
         ## Todo
         
         1.  Add documentation and more meaningful comments
             *   Add more type hints, especially those involving Python builtins
         
         2.  Add tests.
         
+        3.  Put `pandas` into `extras_require` of `setup.py`, and remove the dependency. 
+            *   Input of `MDM` class will become a `NumPy` array rather than a dataframe.
+        
+            *   Dataframe conversion will be turned into a utility function,
+            likely using try-except block for imports
+        
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdmpy-0.0.15.8/README.md` & `mdmpy-0.0.15.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # MDM Py
 
 [![Documentation Status](https://readthedocs.org/projects/mdmpy/badge/?version=latest)](https://mdmpy.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/c13f603535364a7ba5a6a18ea6756a64)](https://app.codacy.com/app/justanothergithubber/mdmpy?utm_source=github.com&utm_medium=referral&utm_content=justanothergithubber/mdmpy&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI version](https://badge.fury.io/py/mdmpy.svg)](https://badge.fury.io/py/mdmpy)
+[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 
 This package is a `Python` implementation of [Marginal Distribution Models](https://pubsonline.informs.org/doi/10.1287/mnsc.2014.1906) (MDMs), which can be used in Discrete Choice Modelling.
 
-## Install
+## Documentation
+Documentation is kindly hosted by [Read The Docs](https://mdmpy.readthedocs.io/ "mdmpy Documentation").
 
+## Install
 This package is uploaded to [PyPI](https://pypi.org/ "Python Package Index"). Hence, 
 
 ```bat
 pip install mdmpy
 ```
 
 should work.
@@ -77,7 +80,13 @@
 
 ## Todo
 
 1.  Add documentation and more meaningful comments
     *   Add more type hints, especially those involving Python builtins
 
 2.  Add tests.
+
+3.  Put `pandas` into `extras_require` of `setup.py`, and remove the dependency. 
+    *   Input of `MDM` class will become a `NumPy` array rather than a dataframe.
+
+    *   Dataframe conversion will be turned into a utility function,
+    likely using try-except block for imports
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdmpy-0.0.15.8/setup.py` & `mdmpy-0.0.15.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mdmpy",
-    version="0.0.15.8",
+    version="0.0.15.9",
     author="mdmpy Authors",
-    author_email="3600019+justanothergithubber@users.noreply.github.com",
+    author_email="mdmpyatgithub@gmail.com",
     description="A package that implements Marginal Distribution Models (MDMs)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/justanothergithubber/mdmpy",
-    packages=["mdmpy"],
+    packages=setuptools.find_packages('src'),
     package_dir={'':'src'},
     classifiers=[
+        "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
     'pandas',
     'numpy',
```

### Comparing `mdmpy-0.0.15.8/src/mdmpy/example1.py` & `mdmpy-0.0.15.9/src/mdmpy/mdm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,20 @@
+"""
+This module contains the main class, MDM, in this package.
 
-import os
-os.environ["PATH"] = "D:/Downloads/Software (General Use)/SUTD/Solvers/IPOPT/Ipopt64-3.12.11/bin/" + os.pathsep + os.environ["PATH"]
-import csv
+Within the class are methods related to solving for the Maximum
+Likelihood Estimate (MLE) of coefficients. Two methods are used
+to initialise a model using pyomo, which can then be passed onto
+a solver to be solved. Another way to solve for the coefficients
+is to use a gradient ascent.
+"""
 import math
-import requests
-import pandas as pd
 import numpy as np
-import scipy.stats as stats
 import pyomo.environ as aml
-import util
-
-url = "http://pages.stern.nyu.edu/~wgreene/Text/Edition7/TableF18-2.csv"
-
-df = pd.DataFrame(index=np.arange(0, 840), columns=np.arange(0,7))
-with requests.Session() as s:
-    download = s.get(url)
-
-
-    cr = csv.reader(download.content.decode().splitlines())
-    next(cr)
-    for ix, row in enumerate(cr):
-        df.loc[ix] = [int(x) for x in row]
-
-# mdm0 = mdmpy.MDM(df,   # input dataframe
-#                  0,    # the choice is index 0
-#                  4,    # there are 4 possible choices
-#                  [2,3] # we will use columns index 2 and 3 (3rd and 4th column, Python indices start from 0)
-#                  )
-# mdm0.model_init()
-# mdm0.model_solve("ipopt")
-# beta0 = [mdm0.m.beta[idx].value for idx in mdm0.m.beta]
-# print(beta0)
-# ll0 = mdm0.ll(beta0)
-# print(ll0)
-
+from . import util
 
 class MDM:
     """
     The main class of the package. This models the Marginal Distribution
     Models (MDM)
     """
     def __init__(self,
@@ -97,125 +74,170 @@
                     x_ik = x_i[k]
                     f_arg_ik = cor_lamb - sum(x*y for x, y in zip(input_beta, x_ik))
                     loglik += math.log(1-self._cdf(f_arg_ik))
                 else:
                     pass
         return loglik
 
-    def __loglikexpr(self, heteroscedastic=False, lag_f=None):
+    def __loglikexpr(self, heteroscedastic=False, ASC=False, lag_f=None):
         ### TODO - refactor the double summation over I and K, which is repeated
         if lag_f is None:
-            lag_f=lambda arg: aml.log(1-self._cdf(arg))
+            lag_f = lambda arg: aml.log(1-self._cdf(arg))
+        ### TODO Figure out best way to write out the different cases
         if heteroscedastic:
-            return sum(sum(
-                        self._Z[i][k]*self.m.alpha[k]*lag_f(
-                            self.m.lambda_[i]-sum(
-                                self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+            if ASC:
+                return sum(sum(
+                    self._Z[i][k]*self.m.alpha[k]*lag_f(
+                        self.m.lambda_[i]-sum(
+                            self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+                                -self.m.ASC[k]
                                     ) for k in self.m.K) for i in self.m.I)
+            else:
+                return sum(sum(
+                    self._Z[i][k]*self.m.alpha[k]*lag_f(
+                        self.m.lambda_[i]-sum(
+                            self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+                                ) for k in self.m.K) for i in self.m.I)
         else:
-            return sum(sum(
-                        self._Z[i][k]*lag_f(
-                            self.m.lambda_[i]-sum(
-                                self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+            if ASC:
+                return sum(sum(
+                    self._Z[i][k]*lag_f(
+                        self.m.lambda_[i]-sum(
+                            self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+                                -self.m.ASC[k]
                                     ) for k in self.m.K) for i in self.m.I)
+            else:
+                return sum(sum(
+                    self._Z[i][k]*lag_f(
+                        self.m.lambda_[i]-sum(
+                            self.m.beta[l]*self._X[i][k][l] for l in self.m.L)
+                                ) for k in self.m.K) for i in self.m.I)
+
+    def model_init(self,
+                   heteroscedastic=False,
+                   alpha_to_be_fixed=0,
+                   alpha_cons_limits=(0, 1),
+                   use_ASCs=False,
+                   ASC_fixed_to_zero=None,
+                   model_seed=None,
+                   v=0):
+        """
+        This method initializes the pyomo model as an instance
+        attribute m. Values can later be taken directly from m.
 
-    def model_init(self, heteroscedastic=False, model_seed=None):
-        """"This method initializes the pyomo model as an instance
-        attribute m. Values can later be taken directly from m."""
+        The various keyword arguments of this method are used to customise
+        the resulting model. They include alternative-specific constants
+        (ASCs) which act as y-intercepts depending on which choice was made.
+
+        Another keyword argument is involved in deciding whether the model
+        will handle heteroscedasticity.
+        """
         self.m = aml.ConcreteModel()
         # Model Sets
         self.m.K = aml.Set(initialize=range(self._num_choices))
         self.m.L = aml.Set(initialize=range(self._num_attr))
         self.m.I = aml.Set(initialize=range(self._num_indiv))
 
 
         ### Model Variables ###
         # Initialize at some certain seed
         # For checking if convexity gives numerical stability
         if model_seed:
             np.random.seed(model_seed)
-            numpy_stan_exp = np.random.standard_exponential
-            self.m.beta = aml.Var(self.m.L, initialize=lambda _: numpy_stan_exp()) # 1 arg required for initialize
-            self.m.lambda_ = aml.Var(self.m.I, initialize=lambda _: numpy_stan_exp())
-            ### TODO - Delete OR add verbosity flag to determine if these should be printed
-            print([self.m.beta[h].value for h in self.m.L])
-            print([self.m.lambda_[g].value for g in self.m.I])
+            np_stan_exp = np.random.standard_exponential
+            self.m.beta = aml.Var(self.m.L, initialize=lambda _: np_stan_exp()) # 1 arg required for initialize
+            self.m.lambda_ = aml.Var(self.m.I, initialize=lambda _: np_stan_exp())
+            if use_ASCs:
+                self.m.ASC = aml.Var(self.m.K, initialize=lambda _: np_stan_exp())
+            if v >= 1:
+                print([self.m.beta[q].value for q in self.m.L])
+                print([self.m.lambda_[q].value for q in self.m.I])
+                if use_ASCs:
+                    print([self.m.ASC[q].value for q in self.m.K])
         else:
             self.m.beta = aml.Var(self.m.L)
             self.m.lambda_ = aml.Var(self.m.I)
+            if use_ASCs:
+                self.m.ASC = aml.Var(self.m.K)
+                if ASC_fixed_to_zero:
+                    self.m.ASCConstr = aml.Constraint(self.m.ASC[ASC_fixed_to_zero] == 0)
 
-        # Handling heteroscedascity
+        # Variable for handling heteroscedascity
         if heteroscedastic:
             # known heteroscedasticity
             if isinstance(heteroscedastic, list):
                 self.m.alpha = {idx:v for idx, v in enumerate(heteroscedastic)}
             # else, unknown heteroscedasticity
             else:
-                self.m.alpha = aml.Var(self.m.K, domain=aml.PositiveReals)
+                self.m.alpha = aml.Var(self.m.K, domain=aml.NonNegativeReals)
 #                 self.m.AlphaSumCons = aml.Constraint(expr=sum(self.m.alpha[k] for k in self.m.K)==num_choices)
-                self.m.FixOneAlphaC = aml.Constraint(expr=self.m.alpha[0] == 1)
+                self.m.FixOneAlphaC = aml.Constraint(expr=self.m.alpha[alpha_to_be_fixed] == 1)
 
-                def _tol_cons(model, k, ALPHA_TOL=0.3):
-                    return model.alpha[k] >= ALPHA_TOL
+                def _alpha_cons(model, k):
+                    # alpha_cons_limits is a keyword argument to model_init
+                    return (alpha_cons_limits[0], model.alpha[k], alpha_cons_limits[1])
 
-                self.m.AlphaTol = aml.Constraint(self.m.K, rule=_tol_cons)
+                self.m.AlphaTol = aml.Constraint(self.m.K, rule=_alpha_cons)
 
         # Objective Function
         ### TODO Hardcode in the other common distributions, especially
         ### Those with a region which is simultaneously reliability function
         ### convex and logconcave, which guarantees concave objective
         ### This hardcoding should simplify the algebraic expression
         ### for the solver, and hence allow to see more
         ###### Dists under consideration:
         ###### Hyperbolic secant - region: non-negative numbers AKA above median
+        ###### Extreme Value - region: non-negative numbers AKA above median
         ###### ... distributions with suitable unbounded regions
         ###### ... satisfying tail convex+tail logconcave
         if heteroscedastic:
             if self._cdf == util.exp_cdf:
                 O_expr = self.__loglikexpr(heteroscedastic=True, lag_f=lambda arg: -arg)
+            elif self._cdf == util.exp_cdf and use_ASCs:
+                O_expr = self.__loglikexpr(heteroscedastic=True, ASC=True, lag_f=lambda arg: -arg)
             else:
                 O_expr = self.__loglikexpr(heteroscedastic=True)
 
         else:
             # Model CDF simplifications
             if self._cdf == util.exp_cdf:
                 O_expr = self.__loglikexpr(lag_f=lambda arg: -arg)
-            ### seems bugged ###
-            if self._cdf == util.gumbel_cdf:
+            elif self._cdf == util.gumbel_cdf:
                 O_expr = self.__loglikexpr(lag_f=lambda arg: aml.log(1-aml.exp(-aml.exp(-arg))))
-            ### seems bugged ###
+            elif use_ASCs:
+                O_expr = self.__loglikexpr(ASC=True)
             else:
                 O_expr = self.__loglikexpr()
 
         # Model Objective
         self.m.O = aml.Objective(expr=O_expr, sense=aml.maximize)
 
         # Lagrangian Constraints (for each individual)
+        def _lag_cons_helper(model, i, lhs_sum_expr=None):
+            if lhs_sum_expr is None:
+                lhs_sum_expr = (1-self._cdf(model.lambda_[i]-sum(
+                                    model.beta[l]*self._X[i][k][l] for l in model.L)))
+            return sum(lhs_sum_expr for k in model.K) <= 1
         # MEM
+        if heteroscedastic and use_ASCs and self._cdf == util.exp_cdf:
+            sum_expr = aml.exp(model.alpha[k]*(sum(
+                            model.beta[l]*self._X[i][k][l] for l in model.L)-model.lambda_[i]))
+
+        ### TODO Figure out best way to write out the different cases
         if heteroscedastic and self._cdf == util.exp_cdf:
-            def _lag_cons(model, i):
-                return sum(aml.exp(model.alpha[k]*(sum(
-                    model.beta[l]*self._X[i][k][l] for l in model.L)-model.lambda_[i])) for k in model.K) <= 1
+            sum_expr = aml.exp(model.alpha[k]*(sum(
+                            model.beta[l]*self._X[i][k][l] for l in model.L)-model.lambda_[i]))
         elif self._cdf == util.exp_cdf:
-            def _lag_cons(model, i):
-                return sum(aml.exp(sum(
-                    model.beta[l]*self._X[i][k][l] for l in model.L)-model.lambda_[i]) for k in model.K) <= 1
-        ### seems bugged ###
+            sum_expr = aml.exp(sum(model.beta[l]*self._X[i][k][l] for l in model.L)-model.lambda_[i])
         elif self._cdf == util.gumbel_cdf:
-            def _lag_cons(model, i):
-                return sum(1-aml.exp(-aml.exp(
-                            (model.lambda_[i]-sum(
-                                model.beta[l]*self._X[i][k][l] for l in model.L))
-                                    )) for k in model.K) <= 1
-        ### seems bugged ###
+            sum_expr = 1-aml.exp(-aml.exp(
+                            sum(model.beta[l]*self._X[i][k][l] for l in model.L)-(model.lambda_[i])))
         else:
-            def _lag_cons(model, i):
-                return sum(1-self._cdf(model.lambda_[i]-sum(
-                    model.beta[l]*self._X[i][k][l] for l in model.L)) for k in model.K) <= 1
-        self.m.C = aml.Constraint(self.m.I, rule=_lag_cons)
+            sum_expr = None
+        self.m.C = aml.Constraint(self.m.I, rule=_lag_cons_helper(lhs_sum_expr=sum_expr))
 
         # Scale restriction - not required
         # but might help solver not get lost and diverge
         def _beta_size_cons(model, l):
             return (-20, model.beta[l], 20)
         self.m.BetaSizeCon = aml.Constraint(self.m.L, rule=_beta_size_cons)
 
@@ -257,62 +279,37 @@
 
     def grad_desc(self,
                   initial_beta,
                   max_steps: int = 50,
                   grad_mult=1,
                   eps: float = 10**-7,
                   verbosity=0):
-        """Starts a gradient-descent based method using the CDF and PDF.
+        """
+        Starts a gradient-descent based method using the CDF and PDF.
         Requires a starting beta iterate.
 
-        TODO : to add f_arg_min which will be pass onto the gradient
+        TODO: to add f_arg_min which will be pass onto the gradient
         calculators and use grad_lambda_beta to move towards
         a convex region, which is above f_arg_min
+
+        TODO: Add some sort of linesearch method. That is, a method
+        that uses a direction and tries varies stepsizes to check
+        what happens to the loglikelihood with those stepsizes
+        and uses some rules or heuristics to decide which
+        stepsize to choose
         """
         last_log_lik = self.ll(initial_beta)
         beta_iterate = initial_beta #initialize
         for num_step in range(max_steps):
             grad, corr_lambs = self._calc_grad_ll_beta(beta_iterate)
-            print(grad)
             beta_iterate = beta_iterate + grad_mult*(grad/(num_step+1))
-            # once no more big gains are made, stop
             cur_ll = self.ll(beta_iterate, corr_lambs=corr_lambs)
             if verbosity == 1:
                 print(cur_ll)
             if math.isnan(cur_ll):
                 print("An Error occurred in calculating Loglikelihood")
                 break # no point continuing when LL has is nan
+            # once no more big gains are made, stop
             if abs(last_log_lik-cur_ll) < eps:
                 break
             last_log_lik = cur_ll
         return beta_iterate
-
-
-mdm2 = MDM(df,   # input dataframe
-                 0,    # the choice is index 0
-                 4,    # there are 4 possible choices
-                 [1, 2, 3, 4], # we will use columns index 2 and 3 (3rd and 4th column, Python indices start from 0)
-                 input_cdf=util.gumbel_cdf)
-mdm2.model_init()
-mdm2.add_conv()
-mdm2.model_solve("ipopt")
-beta2 = [mdm2.m.beta[idx].value for idx in mdm2.m.beta]
-print(beta2)
-ll2 = mdm2.ll(beta2)
-print(ll2)
-
-mdm1 = MDM(df,   # input dataframe
-                 0,    # the choice is index 0
-                 4,    # there are 4 possible choices
-                 [1, 2, 3, 4] # now instead we use all 4 choice-specific-data columns
-                 )
-mdm1._cdf = stats.expon.cdf
-mdm1._pdf = stats.expon.pdf
-mdm1.grad_desc([0.01, 0.01, 0.01, 0.01],
-               grad_mult=0.01,
-               verbosity=1)
-# mdm1.model_init()
-# mdm1.model_solve("ipopt")
-# beta1 = [mdm1.m.beta[idx].value for idx in mdm1.m.beta]
-# print(beta1)
-# ll1 = mdm1.ll(beta1)
-# print(ll1)
```

### Comparing `mdmpy-0.0.15.8/src/mdmpy/util.py` & `mdmpy-0.0.15.9/src/mdmpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """Exponential Cumulative Distribution Function (CDF), with default parameter 1"""
     return 1-aml.exp(-lambda_*x)
 
 def exp_pdf(x, lambda_: float = 1):
     """Exponential Probability Density Function (PDF), with default parameter 1"""
     return lambda_*aml.exp(-lambda_*x)
 
-# in general, lambda = 1
+# in general, beta = 1
 def gumbel_cdf(x, beta: float = 1):
     """Gumbel Cumulative Distribution Function (CDF), with default parameter 1"""
     return aml.exp(-aml.exp(-x/beta))
 
 def gumbel_pdf(x, beta: float = 1):
     """Gumbel Probability Density Function (PDF), with default parameter 1"""
     return 1/beta * aml.exp(-((x/beta)+aml.exp(-(x/beta))))
```

### Comparing `mdmpy-0.0.15.8/src/mdmpy.egg-info/PKG-INFO` & `mdmpy-0.0.15.9/src/mdmpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: mdmpy
-Version: 0.0.15.8
+Version: 0.0.15.9
 Summary: A package that implements Marginal Distribution Models (MDMs)
 Home-page: https://github.com/justanothergithubber/mdmpy
 Author: mdmpy Authors
-Author-email: 3600019+justanothergithubber@users.noreply.github.com
+Author-email: mdmpyatgithub@gmail.com
 License: UNKNOWN
 Description: # MDM Py
         
         [![Documentation Status](https://readthedocs.org/projects/mdmpy/badge/?version=latest)](https://mdmpy.readthedocs.io/en/latest/?badge=latest)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/c13f603535364a7ba5a6a18ea6756a64)](https://app.codacy.com/app/justanothergithubber/mdmpy?utm_source=github.com&utm_medium=referral&utm_content=justanothergithubber/mdmpy&utm_campaign=Badge_Grade_Dashboard)
         [![PyPI version](https://badge.fury.io/py/mdmpy.svg)](https://badge.fury.io/py/mdmpy)
+        [![Project Status: WIP â€“ Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
         
         This package is a `Python` implementation of [Marginal Distribution Models](https://pubsonline.informs.org/doi/10.1287/mnsc.2014.1906) (MDMs), which can be used in Discrete Choice Modelling.
         
-        ## Install
+        ## Documentation
+        Documentation is kindly hosted by [Read The Docs](https://mdmpy.readthedocs.io/ "mdmpy Documentation").
         
+        ## Install
         This package is uploaded to [PyPI](https://pypi.org/ "Python Package Index"). Hence, 
         
         ```bat
         pip install mdmpy
         ```
         
         should work.
@@ -86,12 +89,19 @@
         ## Todo
         
         1.  Add documentation and more meaningful comments
             *   Add more type hints, especially those involving Python builtins
         
         2.  Add tests.
         
+        3.  Put `pandas` into `extras_require` of `setup.py`, and remove the dependency. 
+            *   Input of `MDM` class will become a `NumPy` array rather than a dataframe.
+        
+            *   Dataframe conversion will be turned into a utility function,
+            likely using try-except block for imports
+        
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

