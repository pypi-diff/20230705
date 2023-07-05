# Comparing `tmp/cvxportfolio-0.4.2.tar.gz` & `tmp/cvxportfolio-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.4.2.tar", last modified: Mon Jul  3 18:10:43 2023, max compression
+gzip compressed data, was "cvxportfolio-0.4.3.tar", last modified: Wed Jul  5 16:26:18 2023, max compression
```

## Comparing `cvxportfolio-0.4.2.tar` & `cvxportfolio-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-03 18:10:43.409155 cvxportfolio-0.4.2/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.2/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.2/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-03 18:10:43.408834 cvxportfolio-0.4.2/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     5072 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-03 18:10:43.389904 cvxportfolio-0.4.2/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)     1010 2023-07-03 18:10:28.000000 cvxportfolio-0.4.2/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2155 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    11454 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    17559 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20391 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    15400 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9267 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    22186 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     7094 2023-06-28 16:18:25.000000 cvxportfolio-0.4.2/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     8685 2023-06-28 16:55:55.000000 cvxportfolio-0.4.2/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    14459 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    37997 2023-07-03 18:06:07.000000 cvxportfolio-0.4.2/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-03 18:10:43.406510 cvxportfolio-0.4.2/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-07-03 18:10:28.000000 cvxportfolio-0.4.2/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1635 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.2/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.2/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)    10030 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8469 2023-06-28 16:18:25.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10330 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     7078 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8956 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    22256 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5832 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9194 2023-06-26 16:58:07.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    25311 2023-07-03 17:30:09.000000 cvxportfolio-0.4.2/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.2/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-28 16:18:11.000000 cvxportfolio-0.4.2/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-03 18:10:43.392077 cvxportfolio-0.4.2/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-03 18:10:43.000000 cvxportfolio-0.4.2/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-07-03 18:10:43.000000 cvxportfolio-0.4.2/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-07-03 18:10:43.000000 cvxportfolio-0.4.2/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       65 2023-07-03 18:10:43.000000 cvxportfolio-0.4.2/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-07-03 18:10:43.000000 cvxportfolio-0.4.2/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-07-03 18:10:43.409239 cvxportfolio-0.4.2/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-07-03 18:10:28.000000 cvxportfolio-0.4.2/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.261479 cvxportfolio-0.4.3/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.3/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.3/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-05 16:26:18.261158 cvxportfolio-0.4.3/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     5072 2023-07-03 17:30:09.000000 cvxportfolio-0.4.3/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.248103 cvxportfolio-0.4.3/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)     1018 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2638 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11909 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19207 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20371 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1001 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    15860 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     4167 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22839 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7060 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8648 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14416 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    33741 2023-07-05 16:21:09.000000 cvxportfolio-0.4.3/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.260609 cvxportfolio-0.4.3/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1680 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)    10279 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10139 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7182 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8995 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     3725 2023-07-05 16:17:23.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22397 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5996 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9361 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    25890 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.3/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1325 2023-07-04 14:26:42.000000 cvxportfolio-0.4.3/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-05 16:26:18.250368 cvxportfolio-0.4.3/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)     5442 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1094 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       65 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-07-05 16:26:18.000000 cvxportfolio-0.4.3/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-07-05 16:26:18.261562 cvxportfolio-0.4.3/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-07-05 16:23:56.000000 cvxportfolio-0.4.3/setup.py
```

### Comparing `cvxportfolio-0.4.2/LICENSE` & `cvxportfolio-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.2/PKG-INFO` & `cvxportfolio-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.4.2
+Version: 0.4.3
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
```

### Comparing `cvxportfolio-0.4.2/README.md` & `cvxportfolio-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.2/cvxportfolio/__init__.py` & `cvxportfolio-0.4.3/cvxportfolio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 """Cvxportfolio __init__ module.
 
 This module only republishes the api of a selection of cvxportfolio modules.
 The __all__ attribute of each is used.
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 from .simulator import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
 from .risks import *
-from .returns import *
 from .benchmark import *
 from .result import *
+from .hyperparameters import *
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/benchmark.py` & `cvxportfolio-0.4.3/cvxportfolio/benchmark.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,30 +7,45 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""This module defines benchmark portfolio weights in time that are used, for example,
-by risk terms of optimization-based policies.
+"""This module defines benchmark portfolio weights in time that are used,
+for example, by risk terms of optimization-based policies.
 """
 
 import numpy as np
 import pandas as pd
 
-from .estimator import PolicyEstimator
+from .estimator import PolicyEstimator, DataEstimator
 
-__all__ = ['CashBenchmark', 'UniformBenchmark', 'MarketBenchmark']
+__all__ = ['Benchmark', 'CashBenchmark', 'UniformBenchmark', 'MarketBenchmark']
 
 
 class BaseBenchmark(PolicyEstimator):
     """Base class for cvxportfolio benchmark weights."""
     pass
 
+
+class Benchmark(BaseBenchmark, DataEstimator):
+    """User-provided benchmark.
+    
+    :param benchmark_weights: benchmark weights, either constant in
+        time (pd.Series indexed by assets) or varying in time
+        (pd.DataFrame indexed by time and whose columns are the assets).
+    :type benchmark_weights: pd.Series or pd.DataFrame
+    
+    """
+    
+    def __init__(self, benchmark_weights):
+        DataEstimator.__init__(self, benchmark_weights)
+
+
 class CashBenchmark(BaseBenchmark):
     """Default benchmark weights for cvxportfolio risk models.
     """
 
     def _pre_evaluation(self, universe, backtest_times):
         """Define current_value as a constant."""
         self.current_value = np.zeros(len(universe))
@@ -42,20 +57,20 @@
     """
 
     def _pre_evaluation(self, universe, backtest_times):
         """Define current_value as a constant."""
         self.current_value = np.ones(len(universe))
         self.current_value[-1] = 0.
         self.current_value /= np.sum(self.current_value[:-1])
-   
-     
+
+
 class MarketBenchmark(BaseBenchmark):
     """Portfolio weighted by last year's total volumes.
     """
-    
+
     def _values_in_time(self, past_volumes, **kwargs):
         """Update current_value using past year's volumes."""
-        sumvolumes = past_volumes.loc[past_volumes.index >= (past_volumes.index[-1] - pd.Timedelta('365d'))].mean()
+        sumvolumes = past_volumes.loc[past_volumes.index >= (
+            past_volumes.index[-1] - pd.Timedelta('365d'))].mean()
         result = np.zeros(len(sumvolumes) + 1)
         result[:-1] = sumvolumes / sum(sumvolumes)
         return result
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/constraints.py` & `cvxportfolio-0.4.3/cvxportfolio/constraints.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""This module implements realistic constraints to be used with SinglePeriodOptimization
-and MultiPeriodOptimization policies, or other Cvxpy-based policies.
+"""This module implements realistic constraints to be used with
+SinglePeriodOptimization and MultiPeriodOptimization policies,
+or other Cvxpy-based policies.
 """
 
 
 import cvxpy as cp
 import numpy as np
 
 from .estimator import CvxpyExpressionEstimator, DataEstimator
@@ -57,127 +58,136 @@
     Here we can implement a method to pass benchmark weights
     and make the constraint relative to it rather than to the null
     portfolio.
     """
 
     pass
 
+
 class MarketNeutral(BaseWeightConstraint):
     """Initial implementation of market neutrality.
-    
-    The benchmark portfolio weights are computed here 
+
+    The benchmark portfolio weights are computed here
     (weighting by rolling averages of the market volumes)
     but instead should be their own class (used as well
     by risk models, ...).
     """
-    
+
     def __init__(self):
         self.covarianceforecaster = HistoricalFactorizedCovariance()
-    
+
     def _pre_evaluation(self, universe, backtest_times):
         self.market_vector = cp.Parameter(len(universe)-1)
-    
+
     def _values_in_time(self, t, past_volumes, past_returns, **kwargs):
         tmp = past_volumes.iloc[-250:].mean()
         tmp /= sum(tmp)
-        
-        tmp2 = self.covarianceforecaster.current_value @ (self.covarianceforecaster.current_value.T @ tmp)
+
+        tmp2 = self.covarianceforecaster.current_value @ (
+            self.covarianceforecaster.current_value.T @ tmp)
         # print(tmp2)
         self.market_vector.value = np.array(tmp2)
-        
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         return w_plus[:-1].T @ self.market_vector == 0
-        
-        
+
+
 class TurnoverLimit(BaseTradeConstraint):
     """Turnover limit as a fraction of the portfolio value.
-    
+
     See page 37 of the book.
-    
-    :param delta: constant or changing in time turnover limit 
-    :type delta: float or pd.Series 
+
+    :param delta: constant or changing in time turnover limit
+    :type delta: float or pd.Series
     """
-    
+
     def __init__(self, delta):
         self.delta = DataEstimator(delta, compile_parameter=True)
-        
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         return .5 * cp.norm1(z[:-1]) <= self.delta.parameter
-        
+
 
 class ParticipationRateLimit(BaseTradeConstraint):
     """A limit on maximum trades size as a fraction of market volumes.
-    
 
-    :param volumes: per-stock and per-day market volume estimates, or constant in time
+
+    :param volumes: per-stock and per-day market volume estimates, or constant
+        in time
     :type volumes: pd.Series or pd.DataFrame
-    :param max_fraction_of_volumes: max fraction of market volumes that we're allowed to trade
+    :param max_fraction_of_volumes: max fraction of market volumes that we're
+        allowed to trade
     :type max_fraction_of_volumes: float, pd.Series, pd.DataFrame
     """
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
         self.volumes = DataEstimator(volumes, compile_parameter=True)
         self.max_participation_rate = DataEstimator(
             max_fraction_of_volumes, compile_parameter=True)
         self.portfolio_value = cp.Parameter(nonneg=True)
 
     def _values_in_time(self, current_portfolio_value, **kwargs):
         self.portfolio_value.value = current_portfolio_value
-        
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return cp.multiply(cp.abs(z[:-1]), self.portfolio_value) <= cp.multiply(
-            self.volumes.parameter, self.max_participation_rate.parameter
-        )
+        return cp.multiply(cp.abs(z[:-1]),
+                           self.portfolio_value) <= cp.multiply(self.volumes.parameter,
+                                                                self.max_participation_rate.parameter)
 
 
 class LongOnly(BaseWeightConstraint):
     """A long only constraint.
-    
+
     Imposes that at each point in time the post-trade
     weights are non-negative.
+    
+    :param nocash: if True requires that the cash account is zero.
+    :type nocash: bool
     """
+    
+    def __init__(self, nocash=False):
+        self.nocash = nocash
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return w_plus[:-1] >= 0
+        return [w_plus[:-1] >= 0] + ([w_plus[-1]==0] if self.nocash else [])
 
 
 class NoTrade(BaseTradeConstraint):
     """No-trade condition on name on periods(s)."""
-    
+
     def __init__(self, asset, periods):
         self.asset = asset
         self.periods = periods
-    
+
     def _pre_evaluation(self, universe, backtest_times):
         self.index = universe.get_loc(self.asset)
         self.low = cp.Parameter()
         self.high = cp.Parameter()
-    
+
     def _values_in_time(self, t, **kwargs):
         if t in self.periods:
             self.low.value = 0.
             self.high.value = 0.
         else:
             self.low.value = -100.
             self.high.value = +100.
-    
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        return [z[self.index] >= self.low, 
-            z[self.index] <= self.high] 
-        
+        return [z[self.index] >= self.low,
+                z[self.index] <= self.high]
 
 
 class LeverageLimit(BaseWeightConstraint):
     """A limit on leverage.
-    
+
     Leverage is defined as the :math:`\ell_1` norm of non-cash
     post-trade weights. Here we require that it is smaller than
-    a given value
+    a given value.
 
     :param limit: constant or varying in time leverage limit
     :type limit: float or pd.Series
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
@@ -185,37 +195,37 @@
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return cp.norm(w_plus[:-1], 1) <= self.limit.parameter
 
 
 class MinCashBalance(BaseWeightConstraint):
     """Requires that the cash account is larger than c_min dollars.
-    
-    This uses logic to subtract cash used as margin for the short 
+
+    This uses logic to subtract cash used as margin for the short
     positions that is not documented in the book but is
     equivalent to the book definition's for long-only stock positions.
     """
-    
+
     def __init__(self, c_min):
         self.c_min = DataEstimator(c_min)
         self.rhs = cp.Parameter()
-    
+
     def _values_in_time(self, current_portfolio_value, **kwargs):
         self.rhs.value = self.c_min.current_value/current_portfolio_value
-    
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         # TODO clarify this
         realcash = (w_plus[-1] - 2 * cp.sum(cp.neg(w_plus[:-1])))
         return realcash >= self.rhs
-        
-    
+
+
 class LongCash(MinCashBalance):
     """Requires that cash be non-negative."""
-    
+
     def __init__(self):
         super().__init__(0.)
 
 
 class DollarNeutral(BaseWeightConstraint):
     """Long-short dollar neutral strategy."""
 
@@ -249,97 +259,113 @@
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit.parameter
 
+
 class MinMaxWeightsAtTimes(BaseWeightConstraint):
 
     def __init__(self, limit, times):
         self.base_limit = limit
         self.times = times
-    
+
     def _pre_evaluation(self, universe, backtest_times):
         self.backtest_times = backtest_times
         self.limit = cp.Parameter()
-        
+
     def _values_in_time(self, t, mpo_step, **kwargs):
         tidx = self.backtest_times.get_loc(t)
         nowtidx = tidx + mpo_step
-        if (nowtidx < len(self.backtest_times)) and self.backtest_times[nowtidx] in self.times:
+        if (nowtidx < len(self.backtest_times)) and \
+                (self.backtest_times[nowtidx] in self.times):
             self.limit.value = self.base_limit
         else:
             self.limit.value = 100 * self.sign
 
 
 class MinWeightsAtTimes(MinMaxWeightsAtTimes):
-    
+
     sign = -1.
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit
-        
+
+
 class MaxWeightsAtTimes(MinMaxWeightsAtTimes):
 
     sign = 1.
-    
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] <= self.limit
-        
+
 
 class FactorMaxLimit(BaseWeightConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
-    Args:
-        factor_exposure: An (n * r) matrix giving the factor exposure per asset
-        per factor, where n represents # of assets and r represents # of factors
-        limit: A series of list or a single list giving the factor limits
+    :param factor_exposure: DataFrame giving the factor exposure per asset
+        per factor, where the index are the assets and the columns are
+        the factors.
+    :type factor_exposure: pd.DataFrame
+    :param limit: Factor limits, either constant (pd.Series) or varying in time
+        pd.DataFrame.
+    :type limit: pd.Series or pd.DataFrame
     """
 
     def __init__(self, factor_exposure, limit):
-        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.factor_exposure = DataEstimator(
+            factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.parameter.T @ w_plus[:-1] <= self.limit.parameter
+        return (self.factor_exposure.parameter.T @ w_plus[:-1]
+                <= self.limit.parameter)
 
 
 class FactorMinLimit(BaseWeightConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
-    Args:
-        factor_exposure: An (n * r) matrix giving the factor exposure per asset
-        per factor, where n represents # of assets and r represents # of factors
-        limit: A series of list or a single list giving the factor limits
+    :param factor_exposure: DataFrame giving the factor exposure per asset
+        per factor, where the index are the assets and the columns are
+        the factors.
+    :type factor_exposure: pd.DataFrame
+    :param limit: Factor limits, either constant (pd.Series) or varying in time
+        pd.DataFrame.
+    :type limit: pd.Series or pd.DataFrame
     """
 
     def __init__(self, factor_exposure, limit):
-        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.factor_exposure = DataEstimator(
+            factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.parameter.T @ w_plus[:-1] >= self.limit.parameter
+        return (self.factor_exposure.parameter.T @ w_plus[:-1]
+                >= self.limit.parameter)
 
 
 class FixedFactorLoading(BaseWeightConstraint):
     """A constraint to fix portfolio loadings to a set of factors.
 
-    This can be used to impose market neutrality, a certain portfolio-wide alpha, ....
+    This can be used to impose market neutrality, 
+    a certain portfolio-wide alpha, ....
 
     Attributes:
         factor_exposure: An (n * r) matrix giving the factor exposure on each
         factor
         target: A series or number giving the targeted factor loading
     """
 
     def __init__(self, factor_exposure, target):
-        self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
+        self.factor_exposure = DataEstimator(
+            factor_exposure, compile_parameter=True)
         self.target = DataEstimator(target, compile_parameter=True)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return self.factor_exposure.parameter.T @ w_plus[:-1] == self.target.parameter
+        return (self.factor_exposure.parameter.T @ w_plus[:-1]
+                == self.target.parameter)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/costs.py` & `cvxportfolio-0.4.3/cvxportfolio/costs.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,39 +24,43 @@
 import numpy as np
 import pandas as pd
 import copy
 import inspect
 
 from .estimator import CvxpyExpressionEstimator,  DataEstimator
 from .utils import periods_per_year
-__all__ = ["HoldingCost", "TransactionCost", "StocksTransactionCost", "StocksHoldingCost"]
+from .hyperparameters import HyperParameter
+
+__all__ = ["HoldingCost", "TransactionCost",
+           "StocksTransactionCost", "StocksHoldingCost"]
 
 
 class BaseCost(CvxpyExpressionEstimator):
     """Base class for cost objects (and also risks).
 
     Here there is some logic used to implement the algebraic operations.
     See also :class:`CombinedCost`.
     """
-    
+
     def _simulate(self, *args, **kwargs):
         """Simulate cost, used by market simulator.
-        
+
         Look at its invocation in ``MarketSimulator`` for its list of 
         arguments.
-        
+
         Cost classes that are meant to be used in the simulator
         should implement this.
         """
         raise NotImplementedError
 
     def __mul__(self, other):
         """Multiply by constant."""
-        if not np.isscalar(other):
-            raise SyntaxError("You can only multiply cost by a scalar.")
+        if not (np.isscalar(other) or isinstance(other, HyperParameter)):
+            raise SyntaxError("You can only multiply cost by a scalar "
+                              + "or a HyperParameter instance. (Have you instantiated it?)")
         return CombinedCosts([self], [other])
 
     def __add__(self, other):
         """Add cost expression to another cost expression.
 
         Idea is to create a new CombinedCost class that
         implements `_compile_to_cvxpy` and _recursive_values_in_time
@@ -96,142 +100,158 @@
     :param multipliers: floats that multiply the ``costs``
     :type multipliers: list
     """
 
     def __init__(self, costs, multipliers):
         for cost in costs:
             if not isinstance(cost, BaseCost):
-                raise SyntaxError("You can only sum `BaseCost` instances to other `BaseCost` instances.")
+                raise SyntaxError(
+                    "You can only sum cost instances to other cost instances.")
         self.costs = costs
         self.multipliers = multipliers
-        
+
     def __add__(self, other):
         """Add other (combined) cost to self."""
         if isinstance(other, CombinedCosts):
-            return CombinedCosts(self.costs + other.costs, self.multipliers + other.multipliers)
+            return CombinedCosts(self.costs + other.costs,
+                                 self.multipliers + other.multipliers)
         else:
             return CombinedCosts(self.costs + [other], self.multipliers + [1.0])
 
     def __mul__(self, other):
         """Multiply by constant."""
         return CombinedCosts(self.costs, [el * other for el in self.multipliers])
 
     def _recursive_pre_evaluation(self, *args, **kwargs):
         """Iterate over constituent costs."""
         [el._recursive_pre_evaluation(*args, **kwargs) for el in self.costs]
 
     def _recursive_values_in_time(self, **kwargs):
         """Iterate over constituent costs."""
-        [el._recursive_values_in_time(**kwargs) for el in self.costs ]
+        [el._recursive_values_in_time(**kwargs) for el in self.costs]
 
     def _compile_to_cvxpy(self, w_plus, z, portfolio_value):
         """Iterate over constituent costs."""
         self.expression = 0
         for multiplier, cost in zip(self.multipliers, self.costs):
-            self.expression += multiplier * cost._compile_to_cvxpy(w_plus, z, portfolio_value) 
+            self.expression += multiplier * \
+                cost._compile_to_cvxpy(w_plus, z, portfolio_value)
         return self.expression
+        
+    def _collect_hyperparameters(self):
+        return sum([el._collect_hyperparameters() for el in self.costs], []) + \
+            sum([el._collect_hyperparameters() for el in self.multipliers if
+                hasattr(el, '_collect_hyperparameters')], []) 
 
 
 class HoldingCost(BaseCost):
     """This is a generic holding cost model.
-    
+
     Currently it is not meant to be used directly. Look at
     :class:`StocksHoldingCost` for its version specialized to
     the stock market.
     """
 
-    def __init__(self, 
-        spread_on_borrowing_assets_percent=None,
-        spread_on_lending_cash_percent=None,
-        spread_on_borrowing_cash_percent=None,
-        periods_per_year=None,
-        cash_return_on_borrow=False, #TODO revisit this plus spread_on_borrowing_stocks_percent syntax 
-        dividends=None):
-        
+    def __init__(self,
+                 spread_on_borrowing_assets_percent=None,
+                 spread_on_lending_cash_percent=None,
+                 spread_on_borrowing_cash_percent=None,
+                 periods_per_year=None,
+                 # TODO revisit this plus spread_on_borrowing_stocks_percent syntax
+                 cash_return_on_borrow=False,
+                 dividends=None):
+
         self.spread_on_borrowing_assets_percent = None if spread_on_borrowing_assets_percent is None else \
             DataEstimator(spread_on_borrowing_assets_percent)
-        self.dividends = None if dividends is None else DataEstimator(dividends, compile_parameter=True)        
+        self.dividends = None if dividends is None else DataEstimator(
+            dividends, compile_parameter=True)
         self.spread_on_lending_cash_percent = None if spread_on_lending_cash_percent is None else \
-            DataEstimator(spread_on_lending_cash_percent)        
+            DataEstimator(spread_on_lending_cash_percent)
         self.spread_on_borrowing_cash_percent = None if spread_on_borrowing_cash_percent is None else \
             DataEstimator(spread_on_borrowing_cash_percent)
 
         self.periods_per_year = periods_per_year
         self.cash_return_on_borrow = cash_return_on_borrow
-        
+
     def _pre_evaluation(self, universe, backtest_times):
-        
+
         if self.spread_on_borrowing_assets_percent is not None or self.cash_return_on_borrow:
-            self.borrow_cost_stocks = cp.Parameter(len(universe) - 1, nonneg=True)
-        
-        
+            self.borrow_cost_stocks = cp.Parameter(
+                len(universe) - 1, nonneg=True)
+
     def _values_in_time(self, t, past_returns, **kwargs):
         """We use yesterday's value of the cash return here while in the simulator
         we use today's. In the US, updates to the FED rate are published outside
         of trading hours so we might as well use the actual value for today's. The difference
         is very small so for now we do this. 
         """
         ppy = periods_per_year(past_returns.index) if self.periods_per_year is None else \
             self.periods_per_year
-                               
-        cash_return = past_returns.iloc[-1,-1]
+
+        cash_return = past_returns.iloc[-1, -1]
 
         if self.spread_on_borrowing_assets_percent is not None or self.cash_return_on_borrow:
             self.borrow_cost_stocks.value = np.ones(past_returns.shape[1] - 1) * (
-                    cash_return if self.cash_return_on_borrow else 0.) + \
-                self.spread_on_borrowing_assets_percent.current_value / (100 * ppy)
-                
+                cash_return if self.cash_return_on_borrow else 0.) + \
+                self.spread_on_borrowing_assets_percent.current_value / \
+                (100 * ppy)
+
     def _simulate(self, t, h_plus, current_and_past_returns, **kwargs):
-        
+
         ppy = periods_per_year(current_and_past_returns.index) if self.periods_per_year is None else \
             self.periods_per_year
-        
-        cash_return = current_and_past_returns.iloc[-1,-1]        
+
+        cash_return = current_and_past_returns.iloc[-1, -1]
         multiplier = 1 / (100 * ppy)
         result = 0.
         borrowed_stock_positions = np.minimum(h_plus.iloc[:-1], 0.)
-        result += np.sum(((cash_return if self.cash_return_on_borrow else 0.) + 
-            (self.spread_on_borrowing_assets_percent._recursive_values_in_time(t) * multiplier if
-            self.spread_on_borrowing_assets_percent is not None else 0.))
-                 * borrowed_stock_positions)
-        
+        result += np.sum(((cash_return if self.cash_return_on_borrow else 0.) +
+                          (self.spread_on_borrowing_assets_percent._recursive_values_in_time(t) * multiplier if
+                           self.spread_on_borrowing_assets_percent is not None else 0.))
+                         * borrowed_stock_positions)
+
         if self.dividends is not None:
-            result += np.sum(h_plus[:-1] * self.dividends._recursive_values_in_time(t))
-          
+            result += np.sum(h_plus[:-1] *
+                             self.dividends._recursive_values_in_time(t))
+
         # lending_spread = DataEstimator(spread_on_lending_cash_percent)._recursive_values_in_time(t) * multiplier
         # borrowing_spread = DataEstimator(spread_on_borrowing_cash_percent)._recursive_values_in_time(t) * multiplier
 
         # cash_return = current_and_past_returns.iloc[-1,-1]
         real_cash = h_plus.iloc[-1] + sum(np.minimum(h_plus.iloc[:-1], 0.))
 
         if real_cash > 0:
             if self.spread_on_lending_cash_percent is not None:
-                result += real_cash * (max(cash_return - self.spread_on_lending_cash_percent._recursive_values_in_time(t) * multiplier, 0.) - cash_return)
+                result += real_cash * \
+                    (max(cash_return - self.spread_on_lending_cash_percent._recursive_values_in_time(
+                        t) * multiplier, 0.) - cash_return)
         else:
             if self.spread_on_borrowing_cash_percent is not None:
-                result += real_cash * self.spread_on_borrowing_cash_percent._recursive_values_in_time(t) * multiplier
-            
+                result += real_cash * \
+                    self.spread_on_borrowing_cash_percent._recursive_values_in_time(
+                        t) * multiplier
+
         return result
-            
-            
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile cost to cvxpy expression."""
-        
-        expression = 0. 
-        
+
+        expression = 0.
+
         if not (self.spread_on_borrowing_assets_percent is None):
-           expression += cp.multiply(self.borrow_cost_stocks, cp.neg(w_plus)[:-1])
-        
+            expression += cp.multiply(self.borrow_cost_stocks,
+                                      cp.neg(w_plus)[:-1])
+
         if not (self.dividends is None):
             expression -= cp.multiply(self.dividends.parameter, w_plus[:-1])
         assert cp.sum(expression).is_convex()
         return cp.sum(expression)
 
 
-class StocksHoldingCost(HoldingCost):    
+class StocksHoldingCost(HoldingCost):
     """A model for holding cost of stocks.
 
     :param spread_on_borrowing_stocks_percent: spread on top of cash return payed for borrowing assets,
         including cash. If ``None``, the default, it gets from :class:`Backtest` the
         value for the period.
     :type spread_on_borrowing_stocks_percent: float or pd.Series or pd.DataFrame or None
     :param spread_on_lending_cash_percent: spread that subtracts from the cash return for
@@ -246,122 +266,145 @@
     :type dividends: pd.DataFrame or None
     :param periods_per_year: period per year (used in calculation of per-period cost). If None it is calculated
         automatically.
     :type periods_per_year: int or None
     :param cash_return_on_borrow: whether to add (negative of) cash return to borrow cost of assets
     :type cash_return_on_borrow: bool
     """
-    
-    
-    def __init__(self, 
-        spread_on_borrowing_stocks_percent=.5,
-        spread_on_lending_cash_percent=.5,
-        spread_on_borrowing_cash_percent=.5,
-        periods_per_year=None,
-        cash_return_on_borrow=True, #TODO revisit this plus spread_on_borrowing_stocks_percent syntax 
-        dividends=0.):
-        
+
+    def __init__(self,
+                 spread_on_borrowing_stocks_percent=.5,
+                 spread_on_lending_cash_percent=.5,
+                 spread_on_borrowing_cash_percent=.5,
+                 periods_per_year=None,
+                 # TODO revisit this plus spread_on_borrowing_stocks_percent syntax
+                 cash_return_on_borrow=True,
+                 dividends=0.):
+
         super().__init__(
             spread_on_borrowing_assets_percent=spread_on_borrowing_stocks_percent,
             spread_on_lending_cash_percent=spread_on_lending_cash_percent,
             spread_on_borrowing_cash_percent=spread_on_borrowing_cash_percent,
             periods_per_year=periods_per_year,
             cash_return_on_borrow=cash_return_on_borrow,
             dividends=dividends)
 
-    
+
 class TransactionCost(BaseCost):
     """This is a generic model for transaction cost of financial assets.
-    
+
     Currently it is not meant to be used directly. Look at
     :class:`StocksTransactionCost` for its version specialized
     to the stock market.
     """
 
-    def __init__(self, a=None, pershare_cost=None, b=0., window_sigma_est=250, window_volume_est=250, exponent=None):
+    def __init__(self, a=None, pershare_cost=None, b=0., window_sigma_est=None, window_volume_est=None, exponent=None):
 
         self.a = None if a is None else DataEstimator(a)
-        self.pershare_cost = None if pershare_cost is None else DataEstimator(pershare_cost)
+        self.pershare_cost = None if pershare_cost is None else DataEstimator(
+            pershare_cost)
         self.b = None if b is None else DataEstimator(b)
         self.window_sigma_est = window_sigma_est
         self.window_volume_est = window_volume_est
         self.exponent = exponent
-            
+
     def _pre_evaluation(self, universe, backtest_times):
         if self.a is not None or self.pershare_cost is not None:
-            self.first_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
+            self.first_term_multiplier = cp.Parameter(
+                len(universe)-1, nonneg=True)
         if self.b is not None:
-            self.second_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
+            self.second_term_multiplier = cp.Parameter(
+                len(universe)-1, nonneg=True)
 
     def _values_in_time(self, t,  current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
-        
+
         tmp = 0.
-        
+
         if self.a is not None:
-            _ = self.a.current_value 
-            tmp += _ * np.ones(past_returns.shape[1]-1) if np.isscalar(_) else _ 
+            _ = self.a.current_value
+            tmp += _ * \
+                np.ones(past_returns.shape[1]-1) if np.isscalar(_) else _
         if self.pershare_cost is not None:
             if current_prices is None:
-                raise SyntaxError("If you don't provide prices you should set pershare_cost to None")
+                raise SyntaxError(
+                    "If you don't provide prices you should set pershare_cost to None")
             tmp += self.pershare_cost.current_value / current_prices.values
-        
+
         if self.a is not None or self.pershare_cost is not None:
             self.first_term_multiplier.value = tmp
-        
+
         if self.b is not None:
-            
+
+            if (self.window_sigma_est is None) or (self.window_volume_est is None):
+                ppy = periods_per_year(past_returns.index)
+            windowsigma = ppy if (
+                self.window_sigma_est is None) else self.window_sigma_est
+            windowvolume = ppy if (
+                self.window_volume_est is None) else self.window_volume_est
+
             # TODO refactor this with forecast.py logic
-            sigma_est = np.sqrt((past_returns.iloc[-self.window_sigma_est:, :-1]**2).mean()).values
-            volume_est = past_volumes.iloc[-self.window_volume_est:].mean().values
+            sigma_est = np.sqrt(
+                (past_returns.iloc[-windowsigma:, :-1]**2).mean()).values
+            volume_est = past_volumes.iloc[-windowvolume:].mean().values
 
             self.second_term_multiplier.value = self.b.current_value * sigma_est * \
-                (current_portfolio_value / volume_est) ** ((2 if self.exponent is None else self.exponent) - 1)
-                
+                (current_portfolio_value /
+                 volume_est) ** ((2 if self.exponent is None else self.exponent) - 1)
+
     def _simulate(self, t, u, current_and_past_returns, current_and_past_volumes, current_prices, **kwargs):
-        
+
+        if self.window_sigma_est is None:
+            windowsigma = periods_per_year(current_and_past_returns.index)
+        else:
+            windowsigma = self.window_sigma_est
+
         exponent = (1.5 if self.exponent is None else self.exponent)
-        
-        sigma = np.std(current_and_past_returns.iloc[-self.window_sigma_est:, :-1], axis=0)
+
+        sigma = np.std(
+            current_and_past_returns.iloc[-windowsigma:, :-1], axis=0)
 
         result = 0.
         if self.pershare_cost is not None:
             if current_prices is None:
-                raise SyntaxError("If you don't provide prices you should set pershare_cost to None")
-            result += self.pershare_cost._recursive_values_in_time(t) * int(sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
-        
+                raise SyntaxError(
+                    "If you don't provide prices you should set pershare_cost to None")
+            result += self.pershare_cost._recursive_values_in_time(t) * int(
+                sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
+
         if self.a is not None:
-            result += sum(self.a._recursive_values_in_time(t) * np.abs(u.iloc[:-1]))
+            result += sum(self.a._recursive_values_in_time(t)
+                          * np.abs(u.iloc[:-1]))
 
         if self.b is not None:
             if current_and_past_volumes is None:
-                raise SyntaxError("If you don't provide volumes you should set b to None")
+                raise SyntaxError(
+                    "If you don't provide volumes you should set b to None")
             # we add 1 to the volumes to prevent 0 volumes error (trades are cancelled on 0 volumes)
-            result += (np.abs(u.iloc[:-1])**exponent) @ (self.b._recursive_values_in_time(t)  *
-                sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (exponent - 1)))
+            result += (np.abs(u.iloc[:-1])**exponent) @ (self.b._recursive_values_in_time(t) *
+                                                         sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (exponent - 1)))
 
         assert not np.isnan(result)
         assert not np.isinf(result)
 
         return -result
-        
-        
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        
+
         expression = 0
         if self.a is not None or self.pershare_cost is not None:
             expression += cp.abs(z[:-1]).T @ self.first_term_multiplier
             assert expression.is_convex()
         if self.b is not None:
             expression += (cp.abs(z[:-1]) ** (
-                    2 if self.exponent is None else self.exponent)
-                ).T @ self.second_term_multiplier
+                2 if self.exponent is None else self.exponent)
+            ).T @ self.second_term_multiplier
             assert expression.is_convex()
         return expression
-        
-        
+
+
 class StocksTransactionCost(TransactionCost):
     """A model for transaction costs of stocks.
 
     See pages 10-11 in `the book <https://stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf>`_.
     We don't include the short-term alpha term `c` here because it
     can be expressed with a separate `ReturnsForecast` object. 
 
@@ -369,25 +412,29 @@
         (half) the bid-ask spread, or any fee linear in the size of a trade.
     :type a: float or pd.Series or pd.DataFrame
     :param pershare_cost: per-share trade cost, amount of dollars paid for each share traded. 
     :type pershare_cost: float or pd.Series or pd.DataFrame
     :param b: coefficient of the non-linear term of the transaction cost model, which multiplies
         the estimated volatility for each stock (see the book).  
     :type b: float or pd.Series or pd.DataFrame
-    :param window_sigma_est: length of the window for the standard deviation of past returns used to 
-        estimate the volatility :math:`\sigma` of each asset.
-    :type window_sigma_est: int
+    :param window_sigma_est: we use an historical rolling standard deviation to estimate 
+        the average size of the return on a stock on each day, and this multiplies the 
+        second term of the transaction cost model.  See the paper for an explanation of the model. 
+        Here you specify the length of the rolling window to use. If None (the default) it uses
+        a length of 1 year (approximated with the data provided).
+    :type window_sigma_est: int or None
     :param window_volume_est: length of the window for the mean of past volumes used as estimate
         of each period's volume. Has no effect on the simulator version of this which uses
-        the actual volume.
+        the actual volume. If None (the default) it uses a length of 1 year (approximated 
+        with the data provided).
     :type window_volume_est: int
     :param exponent: exponent of the non-linear term, defaults (if set to ``None``) to 1.5 for
         the simulator version, and 2 for the optimization version (because it is more efficient
         numerically and the difference is small, you can change it if you want).
     :type exponent: float or None
     """
-    
-    def __init__(self, a=0., pershare_cost=0.005, b=1.0, window_sigma_est=250, 
-        window_volume_est=250, exponent=1.5):
-        
+
+    def __init__(self, a=0., pershare_cost=0.005, b=1.0, window_sigma_est=None,
+                 window_volume_est=None, exponent=1.5):
+
         super().__init__(a=a, pershare_cost=pershare_cost, b=b, window_sigma_est=window_sigma_est,
-            window_volume_est = window_volume_est, exponent=exponent)
+                         window_volume_est=window_volume_est, exponent=exponent)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/data.py` & `cvxportfolio-0.4.3/cvxportfolio/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 import yfinance as yf
 import pandas as pd
 import numpy as np
 import sqlite3
 
 from .estimator import DataEstimator
 
-__all__ = ["YfinanceTimeSeries", "FredTimeSeries", "FredRateTimeSeries", "BASE_LOCATION"]
+__all__ = ["YfinanceTimeSeries", "FredTimeSeries",
+           "FredRateTimeSeries", "BASE_LOCATION"]
 
 BASE_LOCATION = Path.home() / "cvxportfolio_data"
 
+
 class BaseData:
     """Base class for Cvxportfolio database interface.
 
     Provides a back-end independent way to load and store
     pandas Series and DataFrames where the first index is a
     pandas Timestamp (or numpy datetime64). It also provides
     a systematic way to access external data sources via
@@ -117,34 +119,36 @@
 
     This should not be used directly unless you know what you're doing.
     """
 
     @staticmethod
     def internal_process(data):
         """Manipulate yfinance data for better storing."""
-        
+
         # nan-out nonpositive prices
         data.loc[data["Open"] <= 0, 'Open'] = np.nan
         data.loc[data["Close"] <= 0, "Close"] = np.nan
         data.loc[data["High"] <= 0, "High"] = np.nan
         data.loc[data["Low"] <= 0, "Low"] = np.nan
         data.loc[data["Adj Close"] <= 0, "Adj Close"] = np.nan
-        
+
         # nan-out negative volumes
         data.loc[data["Volume"] < 0, 'Volume'] = np.nan
-        
+
         intraday_logreturn = np.log(data["Close"]) - np.log(data["Open"])
         close_to_close_logreturn = np.log(data["Adj Close"]).diff().shift(-1)
         open_to_open_logreturn = (
-            close_to_close_logreturn + intraday_logreturn - intraday_logreturn.shift(-1)
+            close_to_close_logreturn + intraday_logreturn -
+            intraday_logreturn.shift(-1)
         )
         data["Return"] = np.exp(open_to_open_logreturn) - 1
         del data["Adj Close"]
         # eliminate last period's intraday data
-        data.loc[data.index[-1], ["High", "Low", "Close", "Return", "Volume"]] = np.nan
+        data.loc[data.index[-1], ["High", "Low",
+                                  "Close", "Return", "Volume"]] = np.nan
         return data
 
     def download(self, symbol, current=None, overlap=5, grace_period='5d', **kwargs):
         """Download single stock from Yahoo Finance.
 
         If data was already downloaded we only download
         the most recent missing portion.
@@ -162,15 +166,16 @@
         """
         if (current is None) or (len(current) < overlap):
             updated = yf.download(symbol, progress=False, **kwargs)
             return self.internal_process(updated)
         else:
             if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta(grace_period):
                 return current
-            new = yf.download(symbol, progress=False, start=current.index[-overlap], **kwargs)
+            new = yf.download(symbol, progress=False,
+                              start=current.index[-overlap], **kwargs)
             new = self.internal_process(new)
             return pd.concat([current.iloc[:-overlap], new])
 
     @staticmethod
     def preload(data):
         """Prepare data for use by Cvxportfolio.
 
@@ -178,15 +183,16 @@
         and replace it with 'ValueVolume' which is an estimate
         of the (e.g., US dollar) value of the volume exchanged
         on the day.
         """
         data["ValueVolume"] = data["Volume"] * data["Open"]
         del data["Volume"]
         # remove infty values
-        data.iloc[:, :] = np.nan_to_num(data.values, copy=True, nan=np.nan, posinf=np.nan, neginf=np.nan)
+        data.iloc[:, :] = np.nan_to_num(
+            data.values, copy=True, nan=np.nan, posinf=np.nan, neginf=np.nan)
         # remove extreme values
         # data.loc[data["Return"] < -.99, "Return"] = np.nan
         # data.loc[data["Return"] > .99, "Return"] = np.nan
         return data
 
 
 class BaseDataStore(BaseData):
@@ -241,15 +247,16 @@
             res = self.connection.cursor().execute(f"DROP TABLE '{symbol}'")
             res = self.connection.cursor().execute(
                 f"DROP TABLE '{symbol}___dtypes'")
             self.connection.commit()
 
         if hasattr(data.index, "levels"):
             data.index = data.index.set_names(
-                ["index"] + [f"___level{i}" for i in range(1, len(data.index.levels))]
+                ["index"] +
+                [f"___level{i}" for i in range(1, len(data.index.levels))]
             )
             data = data.reset_index().set_index("index")
         else:
             data.index.name = "index"
 
         data.to_sql(f"{symbol}", self.connection)
         pd.DataFrame(data).dtypes.astype("string").to_sql(
@@ -288,15 +295,14 @@
                 multiindex = [tmp.index.name] + multiindex
                 tmp = tmp.reset_index().set_index(multiindex)
             return tmp.iloc[:, 0] if tmp.shape[1] == 1 else tmp
         except pd.errors.DatabaseError:
             return None
 
 
-
 class PickleStore(BaseDataStore):
     """Pickle data store for pandas Series and DataFrames.
 
     Args:
         base_location (pathlib.Path): filesystem directory where to store files.
 
     """
@@ -322,16 +328,16 @@
         except FileNotFoundError:
             return None
 
     def store(self, symbol, data, **kwargs):
         """Store data locally."""
         self.__create_if_not_existent()
         data.to_pickle(self.location / f"{symbol}.pickle")
-        
-        
+
+
 class LocalDataStore(BaseDataStore):
     """Local data store for pandas Series and DataFrames.
 
     Args:
         base_location (pathlib.Path): filesystem directory where to store files.
 
     """
@@ -400,38 +406,38 @@
             self.location / f"{symbol}___dtypes.csv"
         )
         data.to_csv(self.location / f"{symbol}.csv", **kwargs)
 
 
 class FredBase(BaseData):
     """Base class for FRED data access."""
-    
+
     URL = "https://fred.stlouisfed.org/graph/fredgraph.csv"
-    
+
     def _download(self, symbol):
         return pd.read_csv(self.URL + f'?id={symbol}', index_col=0, parse_dates=[0])[symbol]
 
     def download(self, symbol="DFF", current=None, grace_period='5d'):
         """Download or update pandas Series from FRED. 
-        
+
         If already downloaded don't change data stored locally and only
         add new entries at the end. 
-        
+
         Additionally, we allow for a `grace period`, if the data already downloaded
         has a last entry not older than the grace period, we don't download new data.
         """
         if current is None:
             return self._download(symbol)
         else:
             if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta(grace_period):
                 return current
-                
+
             new = self._download(symbol)
             new = new.loc[new.index > current.index[-1]]
-            
+
             if new.empty:
                 return current
 
             assert new.index[0] > current.index[-1]
             return pd.concat([current, new])
 
 
@@ -448,57 +454,57 @@
 
     """Yahoo Finance data interface using local data store.
 
     Args:
         base_location (pathlib.Path): filesystem directory where to store files.
     """
 
-
     def update_and_load(self, symbol):
         """Update data for symbol and load it."""
         return super().update_and_load(symbol)
 
 
 class FredRate(FredBase, RateBase, SqliteDataStore):
     """Load and store FRED rates like DFF."""
 
     pass
 
 
 class YfinanceTimeSeries(DataEstimator, YfinanceBase, PickleStore):
-    
+
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
-        
-        
+
+
 class FredTimeSeries(DataEstimator, FredBase, PickleStore):
-    
+
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
-    
+
+
 class FredRateTimeSeries(DataEstimator, FredBase, RateBase, PickleStore):
-    
+
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
     def _recursive_pre_evaluation(self, *args, **kwargs):
-        self.data = self.update_and_load(self.symbol)    
-        
+        self.data = self.update_and_load(self.symbol)
+
 
 class TimeSeries(DataEstimator):
     """Class for time series data managed by Cvxportfolio.
 
     Args:
         symbol (str): name of the time series, such as 'AAPL',
             '^VIX', or 'DFF'.
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/errors.py` & `cvxportfolio-0.4.3/cvxportfolio/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     pass
 
 
 class MissingValuesError(DataError):
     """Cvxportfolio tried to access numpy.nan values."""
 
     pass
-    
+
+
 class ForeCastError(DataError):
     """Forecast procedure failed."""
     pass
 
 
 class PortfolioOptimizationError(Exception):
     """Errors with portfolio optimization problems."""
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/estimator.py` & `cvxportfolio-0.4.3/cvxportfolio/estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 This module implements Estimator base classes. Policies, costs, and constraints inherit
 from this.
 """
 
 import numpy as np
 import pandas as pd
 from .errors import MissingValuesError, DataError
+from .hyperparameters import HyperParameter
 import cvxpy as cp
 
 
 class Estimator:
     """Estimator base class.
 
     Policies, costs, and constraints inherit from this. When overloading
@@ -40,43 +41,54 @@
 
         This function is called by Simulator classes on Policy classes
         returning the current trades list. Policy classes, if
         they contain internal estimators, should declare them as attributes
         and call this base function (via `super()`) before
         they do their internal computation. CvxpyExpression estimators
         should instead define this method to update their Cvxpy parameters.
-        
+
         Once we finalize the interface all parameters will be listed here.
         """
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "_recursive_values_in_time"):
                 subestimator._recursive_values_in_time(**kwargs)
         if hasattr(self, "_values_in_time"):
             self.current_value = self._values_in_time(**kwargs)
             return self.current_value
 
 
 class PolicyEstimator(Estimator):
     """Base class for (most) estimators that are part of policy objects."""
     
+    
+    def _collect_hyperparameters(self):
+        """This method finds all hyperparameters defined as part of a policy.
+        """
+        result = []
+        for _, subestimator in self.__dict__.items():
+            if hasattr(subestimator, "_collect_hyperparameters"):
+                result += subestimator._collect_hyperparameters()
+        return result
+            
 
     def _recursive_pre_evaluation(self, universe, backtest_times):
         """Recursively initialize estimator tree for backtest.
 
         :param universe: names of assets to be traded 
         :type universe: pandas.Index
         :param backtest_times: times at which the estimator will be evaluated
         :type backtest_time: pandas.DatetimeIndex
         """
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "_recursive_pre_evaluation"):
-                subestimator._recursive_pre_evaluation(universe, backtest_times)
+                subestimator._recursive_pre_evaluation(
+                    universe, backtest_times)
         if hasattr(self, "_pre_evaluation"):
             self._pre_evaluation(universe, backtest_times)
-    
+
 
 class CvxpyExpressionEstimator(PolicyEstimator):
     """Base class for estimators that are Cvxpy expressions."""
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile term to cvxpy expression.
 
@@ -86,16 +98,16 @@
 
         It can either return a scalar expression, in the case of objective terms,
         or a list of cvxpy constraints, in the case of constraints.
 
         In MultiPeriodOptimization policies this is called separately
         for costs and constraints at different look-ahead steps with
         the corresponding w_plus and z.
-        
-        
+
+
         :param w_plus: post-trade weights 
         :type w_plus: cvxpy.Variable
         :param z: trade weights 
         :type z: cvxpy.Variable
         :param w_plus_minus_w_bm: post-trade weights minus benchmark weights 
         :type w_plus_minus_w_bm: cvxpy.Variable
         """
@@ -121,30 +133,30 @@
         use_last_available_time (bool): if the pandas index exists
             and is a pandas.DateTimeIndex you can instruct self._recursive_values_in_time
             to retrieve the last available value at time t by setting
             this to True. Default is False.
 
     """
 
-    def __init__(self, data, use_last_available_time=False, allow_nans=False, 
-        compile_parameter=False, non_negative=False, positive_semi_definite=False):
+    def __init__(self, data, use_last_available_time=False, allow_nans=False,
+                 compile_parameter=False, non_negative=False, positive_semi_definite=False):
         self.data = data
         self.use_last_available_time = use_last_available_time
         self.allow_nans = allow_nans
         self.compile_parameter = compile_parameter
         self.non_negative = non_negative
-        self.positive_semi_definite =positive_semi_definite
-    
+        self.positive_semi_definite = positive_semi_definite
+
     def _recursive_pre_evaluation(self, universe, backtest_times):
         # super()._recursive_pre_evaluation(universe, backtest_times)
         if self.compile_parameter:
-            value = self.internal__recursive_values_in_time(t=backtest_times[0])
-            self.parameter = cp.Parameter(value.shape if hasattr(value, "shape") else (), 
-                PSD=self.positive_semi_definite, nonneg=self.non_negative)
-            
+            value = self.internal__recursive_values_in_time(
+                t=backtest_times[0])
+            self.parameter = cp.Parameter(value.shape if hasattr(value, "shape") else (),
+                                          PSD=self.positive_semi_definite, nonneg=self.non_negative)
 
     def value_checker(self, result):
         """Ensure that only scalars or arrays without np.nan are returned.
 
         Args:
             result (int, float, or np.array): data produced by self._recursive_values_in_time
 
@@ -164,15 +176,16 @@
             else:
                 return result
 
         if isinstance(result, np.ndarray):
             if np.any(np.isnan(result)) and not self.allow_nans:
                 message = f"{self.__class__.__name__}._recursive_values_in_time result is an array with np.nan's."
                 if hasattr(self.data, 'columns') and len(self.data.columns) == len(result):
-                    message += "Specifically, the problem is with symbol(s): " + str(self.data.columns[np.isnan(result)])
+                    message += "Specifically, the problem is with symbol(s): " + str(
+                        self.data.columns[np.isnan(result)])
                 raise MissingValuesError(message)
             else:
                 return result
 
         raise DataError(
             f"{self.__class__.__name__}._recursive_values_in_time result is not a scalar or array."
         )
@@ -230,17 +243,18 @@
 
         Returns:
             result (float, numpy.array): if you use a callable object make
                 sure that it returns a float or numpy array (and not,
                 for example, a pandas object)
 
         """
-        self.current_value = self.internal__recursive_values_in_time(t, *args, **kwargs)
+        self.current_value = self.internal__recursive_values_in_time(
+            t, *args, **kwargs)
         # we do this because in some cases they never get compiled
-        if hasattr(self, 'parameter'): 
+        if hasattr(self, 'parameter'):
             self.parameter.value = self.current_value
         return self.current_value
 
 
 # class ConstantEstimator(cvxpy.Constant, DataEstimator):
 #     """Cvxpy constant that uses the pre_evalution method to be initialized."""
 #
@@ -311,21 +325,21 @@
 #         value = super().internal__recursive_values_in_time(t=backtest_times[0])
 #         self.parameter = cp.Parameter(
 #             value if hasattr(value, "shape") else (),
 #             PSD=self.positive_semi_definite, nonneg=self.non_negative)
 #
 #     def _recursive_values_in_time(self, t, **kwargs):
 #         self.parameter.value = self.internal__recursive_values_in_time(t, **kwargs)
-        
-        
+
+
 #
 # class ParameterEstimator(DataEstimator):
 #     def __init__(self, *args, **kwargs):
 #         super().__init__(self, *args, compile_parameter=True, **kwargs)
-        
+
 # class ParameterEstimator(cvxpy.Parameter, DataEstimator, PolicyEstimator):
 #     """Data estimator of point-in-time values that contains a Cvxpy Parameter.
 #
 #     Attributes:
 #         parameter (cvxpy.Parameter): the parameter object to use with cvxpy
 #             expressions
 #     Args:
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/forecast.py` & `cvxportfolio-0.4.3/cvxportfolio/forecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,220 +24,226 @@
 import numpy as np
 
 from .estimator import PolicyEstimator
 
 
 def online_cache(_values_in_time):
     """A simple online cache that decorates _values_in_time.
-    
+
     The instance it is used on needs to be hashable (we currently
     use the hash of its __repr__ via dataclass).
     """
-    
+
     def wrapped(self, t, cache=None, **kwargs):
-        
-        if cache is None: # temporary to not change tests
+
+        if cache is None:  # temporary to not change tests
             cache = {}
-            
+
         if not (self in cache):
             cache[self] = {}
-        
+
         if t in cache[self]:
-            logging.debug(f'{self}._values_in_time at time {t} is retrieved from cache.')
+            logging.debug(
+                f'{self}._values_in_time at time {t} is retrieved from cache.')
             result = cache[self][t]
         else:
-            result = _values_in_time(self, t=t, cache=cache, **kwargs)  
-            logging.debug(f'{self}._values_in_time at time {t} is stored in cache.')
+            result = _values_in_time(self, t=t, cache=cache, **kwargs)
+            logging.debug(
+                f'{self}._values_in_time at time {t} is stored in cache.')
             cache[self][t] = result
         return result
-        
+
     return wrapped
 
+
 class BaseForecast(PolicyEstimator):
     """Base class for forecasters."""
-    
+
     # def _recursive_pre_evaluation(self, universe, backtest_times):
     #     self.universe = universe
     #     self.backtest_times = backtest_times
     #
-    
-    
+
     def _agnostic_update(self, t, past_returns):
         """Choose whether to make forecast from scratch or update last one."""
         if (self.last_time is None) or (self.last_time != past_returns.index[-1]):
-            logging.debug(f'{self}._values_in_time at time {t} is computed from scratch.')
+            logging.debug(
+                f'{self}._values_in_time at time {t} is computed from scratch.')
             self._initial_compute(t=t, past_returns=past_returns)
         else:
-            logging.debug(f'{self}._values_in_time at time {t} is updated from previous value.')
+            logging.debug(
+                f'{self}._values_in_time at time {t} is updated from previous value.')
             self._online_update(t=t, past_returns=past_returns)
-            
+
     def _initial_compute(self, t, past_returns):
         """Make forecast from scratch."""
         raise NotImplementedError
 
     def _online_update(self, t, past_returns):
         """Update forecast from period before."""
         raise NotImplementedError
 
+
 @dataclass(unsafe_hash=True)
 class HistoricalMeanReturn(BaseForecast):
     r"""Historical mean returns.
-    
+
     This ignores both the cash returns column and all missing values.
     """
-         
+
     def __post_init__(self):
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
-        
+
     def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
-    
+
     def _values_in_time(self, t, past_returns, cache=None, **kwargs):
         self._agnostic_update(t=t, past_returns=past_returns)
-        return (self.last_sum / self.last_counts).values        
-        
+        return (self.last_sum / self.last_counts).values
+
     def _initial_compute(self, t, past_returns):
         """Make forecast from scratch."""
         self.last_counts = past_returns.iloc[:, :-1].count()
         self.last_sum = past_returns.iloc[:, :-1].sum()
         self.last_time = t
-        
+
     def _online_update(self, t, past_returns):
         """Update forecast from period before."""
         self.last_counts += ~(past_returns.iloc[-1, :-1].isnull())
         self.last_sum += past_returns.iloc[-1, :-1].fillna(0.)
         self.last_time = t
 
-        
+
 class HistoricalMeanError(BaseForecast):
     r"""Historical standard deviations of the mean of non-cash returns.
-    
+
     For a given time series of past returns :math:`r_{t-1}, r_{t-2}, \ldots, r_0` this is
     :math:`\sqrt{\text{Var}[r]/t}`. When there are missing values we ignore them,
     both to compute the variance and the count.
     """
 
     def __init__(self):
         self.varianceforecaster = HistoricalVariance(kelly=False)
-    
+
     def _values_in_time(self, t, past_returns, **kwargs):
         return np.sqrt(self.varianceforecaster.current_value / self.varianceforecaster.last_counts.values)
-        
-        
+
+
 @dataclass(unsafe_hash=True)
 class HistoricalVariance(BaseForecast):
     r"""Historical variances of non-cash returns.
-    
+
     :param kelly: if ``True`` compute :math:`\mathbf{E}[r^2]`, else
         :math:`\mathbf{E}[r^2] - {\mathbf{E}[r]}^2`. The second corresponds
         to the classic definition of variance, while the first is what is obtained
         by Taylor approximation of the Kelly gambling objective. (See page 28 of the book.)
     :type kelly: bool
     """
-    
+
     kelly: bool = True
 
     def __post_init__(self):
         if not self.kelly:
             self.meanforecaster = HistoricalMeanReturn()
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
-        
+
     def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
-    
+
     def _values_in_time(self, t, past_returns, **kwargs):
         self._agnostic_update(t=t, past_returns=past_returns)
         result = (self.last_sum / self.last_counts).values
         if not self.kelly:
             result -= self.meanforecaster.current_value**2
         return result
-        
+
     def _initial_compute(self, t, past_returns):
         self.last_counts = past_returns.iloc[:, :-1].count()
         self.last_sum = (past_returns.iloc[:, :-1]**2).sum()
         self.last_time = t
-        
-    def _online_update(self, t, past_returns): #, last_estimation, last_counts, last_time):
+
+    # , last_estimation, last_counts, last_time):
+    def _online_update(self, t, past_returns):
         self.last_counts += ~(past_returns.iloc[-1, :-1].isnull())
         self.last_sum += past_returns.iloc[-1, :-1].fillna(0.)**2
         self.last_time = t
 
 
 @dataclass(unsafe_hash=True)
 class HistoricalFactorizedCovariance(BaseForecast):
     r"""Historical covariance matrix, sqrt factorized.
-    
+
     :param kelly: if ``True`` compute each :math:` \Sigma_{i,j} \simeq \mathbf{E}[r^{i} r^{j}]`, else
         :math:` \Sigma_{i,j} \simeq \mathbf{E}[r^{i} r^{j}] - \mathbf{E}[r^{i}]\mathbf{E}[r^{j}]` matching
         the behavior of ``pandas.DataFrame.cov(ddof=0)`` (with same logic to handle missing data). 
         The second case corresponds to the classic definition of covariance, while the first is what is obtained
         by Taylor approximation of the Kelly gambling objective. (See page 28 of the book.)
     :type kelly: bool
     """
-    
+
     kelly: bool = True
-    
+
     def __post_init__(self):
         self.last_time = None
-    
+
     def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
-    
+
     @staticmethod
     def _get_count_matrix(past_returns):
         r"""We obtain the matrix of non-null joint counts:
-        
+
         .. math::
-        
+
             \text{Count}\left(r^{i}r^{j} \neq \texttt{nan}\right).
         """
-        tmp = (~past_returns.iloc[:,:-1].isnull()) * 1.
+        tmp = (~past_returns.iloc[:, :-1].isnull()) * 1.
         return tmp.T @ tmp
-    
+
     @staticmethod
     def _get_initial_joint_mean(past_returns):
         r"""Compute precursor of :math:`\Sigma_{i,j} = \mathbf{E}[r^{i}]\mathbf{E}[r^{j}]`.
         """
-        nonnull = (~past_returns.iloc[:,:-1].isnull()) * 1.
-        tmp = nonnull.T @ past_returns.iloc[:,:-1].fillna(0.)
-        return tmp # * tmp.T
+        nonnull = (~past_returns.iloc[:, :-1].isnull()) * 1.
+        tmp = nonnull.T @ past_returns.iloc[:, :-1].fillna(0.)
+        return tmp  # * tmp.T
 
     @staticmethod
     def _factorize(Sigma):
         """Factorize matrix and remove negative eigenvalues."""
         eigval, eigvec = np.linalg.eigh(Sigma)
         eigval = np.maximum(eigval, 0.)
         return eigvec @ np.diag(np.sqrt(eigval))
-        
+
     def _initial_compute(self, t, past_returns):
         self.last_counts_matrix = self._get_count_matrix(past_returns).values
-        filled = past_returns.iloc[:,:-1].fillna(0.).values
+        filled = past_returns.iloc[:, :-1].fillna(0.).values
         self.last_sum_matrix = filled.T @ filled
         if not self.kelly:
             self.joint_mean = self._get_initial_joint_mean(past_returns)
 
         self.last_time = t
-        
+
     def _online_update(self, t, past_returns):
         nonnull = ~(past_returns.iloc[-1, :-1].isnull())
         self.last_counts_matrix += np.outer(nonnull, nonnull)
         last_ret = past_returns.iloc[-1, :-1].fillna(0.)
         self.last_sum_matrix += np.outer(last_ret, last_ret)
         self.last_time = t
         if not self.kelly:
             self.joint_mean += last_ret
 
     @online_cache
     def _values_in_time(self, t, past_returns, **kwargs):
-  
+
         self._agnostic_update(t=t, past_returns=past_returns)
         Sigma = self.last_sum_matrix / self.last_counts_matrix
-        
+
         if not self.kelly:
             tmp = self.joint_mean / self.last_counts_matrix
             Sigma -= tmp.T * tmp
-               
-        return self._factorize(Sigma) 
+
+        return self._factorize(Sigma)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/policies.py` & `cvxportfolio-0.4.3/cvxportfolio/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,25 +197,25 @@
         self.target_weights = DataEstimator(target_weights)
 
     def _recursive_values_in_time(self, t, current_weights, **kwargs):
         """We need to override recursion b/c we catch exception."""
         try:
             super()._recursive_values_in_time(t=t, current_weights=current_weights, **kwargs)
             return pd.Series(self.target_weights.current_value,
-                    current_weights.index) - current_weights
+                             current_weights.index) - current_weights
         except MissingValuesError:
             return pd.Series(0., current_weights.index)
-            
-            
+
+
 class Uniform(FixedWeights):
     """Uniform allocation on non-cash assets."""
-    
+
     def __init__(self):
         pass
-    
+
     def _pre_evaluation(self, universe, backtest_times):
         target_weights = pd.Series(1., universe)
         target_weights.iloc[-1] = 0
         target_weights /= sum(target_weights)
         self.target_weights = DataEstimator(target_weights)
 
 
@@ -268,46 +268,44 @@
         DataFrame indexed by time.
     :type target: pd.Series or pd.DataFrame
     :param tracking_error: we trade to match the target
         weights whenever the 2-norm of our weights minus the
         target is larger than this. Pass a Series if you want to vary it in
         time.
     :type tracking_error: pd.Series or pd.DataFrame
-    
+
     """
 
     def __init__(self, target, tracking_error):
         self.target = DataEstimator(target)
         self.tracking_error = DataEstimator(tracking_error)
 
     def _values_in_time(self, t, current_weights, **kwargs):
         if np.linalg.norm(current_weights - self.target.current_value) > \
-          self.tracking_error.current_value:
+                self.tracking_error.current_value:
             return self.target.current_value - current_weights
         else:
             return pd.Series(0., current_weights.index)
 
 
-
-
 class MultiPeriodOptimization(BaseTradingPolicy):
     r"""Multi Period Optimization policy.
 
     Implements the model developed in Chapter 5, in particular
     at page 49, of the book. You specify the objective terms
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify lists
     of constraints. There are two ways to do it. You either
     define the same objective terms and costraints for each 
     step of the multi-period problem, or you define a different
     objective term and different list of constraints for each step.
     In addition we offer a `terminal_constraint` argument to
     simply impose that at the last step in the optimization the
     post-trade weights match the given weights (see page 51).
-    
+
     When it computes the trajectory of weights for the future
     it only returns the first step (to the Simulator, typically).
     The future steps (planning horizon) are by default not returned.
 
     :param objective: these will be maximized;
         if you pass a single expression of BaseCost it is understood as the 
         same for all steps; if it's a list you must also pass a list of lists
@@ -339,115 +337,129 @@
         so you can choose your own solver and pass
         parameters to it.
     """
 
     def __init__(self, objective, constraints=[], include_cash_return=True, planning_horizon=None, terminal_constraint=None, benchmark=CashBenchmark, **kwargs):
         if hasattr(objective, '__iter__'):
             if not (hasattr(constraints, '__iter__') and len(constraints) and (hasattr(constraints[0], '__iter__') and len(objective) == len(constraints))):
-                raise SyntaxError('If you pass objective as a list, constraints should be a list of lists of the same length.')
+                raise SyntaxError(
+                    'If you pass objective as a list, constraints should be a list of lists of the same length.')
             self.planning_horizon = len(objective)
             self.objective = objective
             self.constraints = constraints
         else:
             if not np.isscalar(planning_horizon):
-                raise SyntaxError('If `objective` and `constraints` are the same for all steps you must specify `planning_horizon`.')
+                raise SyntaxError(
+                    'If `objective` and `constraints` are the same for all steps you must specify `planning_horizon`.')
             self.planning_horizon = planning_horizon
-            self.objective = [copy.deepcopy(objective) for i in range(planning_horizon)] if planning_horizon > 1 else [objective]
-            self.constraints = [copy.deepcopy(constraints) for i in range(planning_horizon)] if planning_horizon > 1 else [constraints]
-        
+            self.objective = [copy.deepcopy(objective) for i in range(
+                planning_horizon)] if planning_horizon > 1 else [objective]
+            self.constraints = [copy.deepcopy(constraints) for i in range(
+                planning_horizon)] if planning_horizon > 1 else [constraints]
+
         self.include_cash_return = include_cash_return
         if self.include_cash_return:
             self.objective = [el + CashReturn() for el in self.objective]
         self.terminal_constraint = terminal_constraint
         self.benchmark = benchmark() if isinstance(benchmark, type) else benchmark
         self.cvxpy_kwargs = kwargs
 
-    def _compile_to_cvxpy(self):#, w_plus, z, value):
+    def _compile_to_cvxpy(self):  # , w_plus, z, value):
         """Compile all cvxpy expressions and the problem."""
         self.cvxpy_objective = [
-            el._compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
+            el._compile_to_cvxpy(
+                self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i])
             for i, el in enumerate(self.objective)]
         self.cvxpy_objective = sum(self.cvxpy_objective)
         assert self.cvxpy_objective.is_dcp()  # dpp=True)
         assert self.cvxpy_objective.is_concave()
         self.cvxpy_constraints = [
-            flatten_heterogeneous_list([constr._compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
-                for constr in el])
+            flatten_heterogeneous_list([constr._compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i])
+                                        for constr in el])
             for i, el in enumerate(self.constraints)]
         self.cvxpy_constraints = sum(self.cvxpy_constraints, [])
         self.cvxpy_constraints += [cp.sum(z) == 0 for z in self.z_at_lags]
         w = self.w_current
         for i in range(self.planning_horizon):
-            self.cvxpy_constraints.append(self.w_plus_at_lags[i] == self.z_at_lags[i] + w)
-            self.cvxpy_constraints.append(self.w_plus_at_lags[i] - self.w_bm == self.w_plus_minus_w_bm_at_lags[i])
+            self.cvxpy_constraints.append(
+                self.w_plus_at_lags[i] == self.z_at_lags[i] + w)
+            self.cvxpy_constraints.append(
+                self.w_plus_at_lags[i] - self.w_bm == self.w_plus_minus_w_bm_at_lags[i])
             w = self.w_plus_at_lags[i]
         if not self.terminal_constraint is None:
             self.cvxpy_constraints.append(w == self.terminal_constraint)
-        self.problem = cp.Problem(cp.Maximize(self.cvxpy_objective), self.cvxpy_constraints)
+        self.problem = cp.Problem(cp.Maximize(
+            self.cvxpy_objective), self.cvxpy_constraints)
         assert self.problem.is_dcp()  # dpp=True)
 
     def _recursive_pre_evaluation(self, universe, backtest_times):
         """No point in using recursive super() method."""
-        
+
         for obj in self.objective:
-            obj._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
+            obj._recursive_pre_evaluation(
+                universe=universe, backtest_times=backtest_times)
         for constr_at_lag in self.constraints:
             for constr in constr_at_lag:
-                constr._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
-        
-        self.benchmark._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
+                constr._recursive_pre_evaluation(
+                    universe=universe, backtest_times=backtest_times)
+
+        self.benchmark._recursive_pre_evaluation(
+            universe=universe, backtest_times=backtest_times)
         self.w_bm = cp.Parameter(len(universe))
 
         # temporary
         # self.w_bm = np.zeros(len(universe))
         # self.w_bm[-1] = 1.
-        
+
         # initialize the problem
         # self.portfolio_value = cp.Parameter(nonneg=True)
         self.w_current = cp.Parameter(len(universe))
-        self.z_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)] 
-        self.w_plus_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
-        self.w_plus_minus_w_bm_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
+        self.z_at_lags = [cp.Variable(len(universe))
+                          for i in range(self.planning_horizon)]
+        self.w_plus_at_lags = [cp.Variable(
+            len(universe)) for i in range(self.planning_horizon)]
+        self.w_plus_minus_w_bm_at_lags = [cp.Variable(
+            len(universe)) for i in range(self.planning_horizon)]
 
         # simulator will overwrite this with cached loaded from disk
         self.cache = {}
 
         # self._compile_to_cvxpy()#self.w_plus, self.z, self.portfolio_value)
-        
 
     def _recursive_values_in_time(self, t, current_weights, current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
         """Update all cvxpy parameters and solve."""
-        
+
         assert current_portfolio_value > 0
         assert np.isclose(sum(current_weights), 1)
-                
+
         for i, obj in enumerate(self.objective):
-            obj._recursive_values_in_time(t=t, current_weights=current_weights, 
-                    current_portfolio_value=current_portfolio_value, 
-                    past_returns=past_returns, past_volumes=past_volumes, 
-                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)     
-                     
+            obj._recursive_values_in_time(t=t, current_weights=current_weights,
+                                          current_portfolio_value=current_portfolio_value,
+                                          past_returns=past_returns, past_volumes=past_volumes,
+                                          current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)
+
         for i, constr_at_lag in enumerate(self.constraints):
             for constr in constr_at_lag:
-                constr._recursive_values_in_time(t=t, current_weights=current_weights, 
-                    current_portfolio_value=current_portfolio_value, 
-                    past_returns=past_returns, past_volumes=past_volumes, 
-                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)   
-                    
-        self.benchmark._recursive_values_in_time(t=t, current_weights=current_weights, 
-                    current_portfolio_value=current_portfolio_value, 
-                    past_returns=past_returns, past_volumes=past_volumes, 
-                    current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs) 
-                    
+                constr._recursive_values_in_time(t=t, current_weights=current_weights,
+                                                 current_portfolio_value=current_portfolio_value,
+                                                 past_returns=past_returns, past_volumes=past_volumes,
+                                                 current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)
+
+        self.benchmark._recursive_values_in_time(t=t, current_weights=current_weights,
+                                                 current_portfolio_value=current_portfolio_value,
+                                                 past_returns=past_returns, past_volumes=past_volumes,
+                                                 current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)
+
         self.w_bm.value = self.benchmark.current_value
         self.w_current.value = current_weights.values
 
         try:
             with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", message='Solution may be inaccurate')
+                warnings.filterwarnings(
+                    "ignore", message='Solution may be inaccurate')
                 self.problem.solve(**self.cvxpy_kwargs)
         except cp.SolverError:
             raise PortfolioOptimizationError(
                 f"Numerical solver for policy {self.__class__.__name__} at time {t} failed;"
                 "try changing it, relaxing some constraints, or dropping some costs.")
         if self.problem.status in ["unbounded", "unbounded_inaccurate"]:
             raise PortfolioOptimizationError(
@@ -455,17 +467,25 @@
             )
         if self.problem.status in ["infeasible", 'infeasible_inaccurate']:
             raise PortfolioOptimizationError(
                 f"Policy {self.__class__.__name__} at time {t} resulted in an infeasible problem."
             )
 
         return pd.Series(self.z_at_lags[0].value, current_weights.index)
+        
+    def _collect_hyperparameters(self):
+        result = []
+        for el in self.objective:
+            result += el._collect_hyperparameters()
+        for el in self.constraints:
+            for constr in el:
+                result += el._collect_hyperparameters()
+        return result
 
 
-    
 class SinglePeriodOptimization(MultiPeriodOptimization):
     r"""Single Period Optimization policy.
 
     Implements the model developed in Chapter 4, in particular
     at page 43, of the book. You specify the objective term
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify a list
@@ -483,11 +503,9 @@
         and ``MarketBenchmark``, which approximates the market-weighted portfolio.
     :type benchmark: BaseBenchmark class or instance
     :param \**kwargs: these will be passed to cvxpy.Problem.solve, so you can choose your own solver and pass
         parameters to it.
     """
 
     def __init__(self, objective, constraints=[], include_cash_return=True, benchmark=CashBenchmark, **kwargs):
-        super().__init__([objective], [constraints], include_cash_return=include_cash_return, 
-            benchmark=benchmark, **kwargs)
-        
-
+        super().__init__([objective], [constraints], include_cash_return=include_cash_return,
+                         benchmark=benchmark, **kwargs)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/result.py` & `cvxportfolio-0.4.3/cvxportfolio/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,36 +21,37 @@
 from .estimator import Estimator
 from .utils import periods_per_year
 import matplotlib.pyplot as plt
 
 __all__ = ['BacktestResult']
 
 
-
 def getFiscalQuarter(dt):
     """Convert a time to a fiscal quarter."""
     year = dt.year
     quarter = (dt.month - 1) // 3 + 1
     return "Q%i %s" % (quarter, year)
-    
-    
+
+
 class BacktestResult(Estimator):
     """Holds the data from a Backtest and producs metrics and plots."""
-    
-    
+
     def __init__(self, universe, backtest_times, costs):
         """Initialization of backtest result."""
-        self.h = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
-        self.u = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
-        self.z = pd.DataFrame(index=backtest_times, columns=universe, dtype=float)
-        self.costs = {cost.__class__.__name__:pd.Series(index=backtest_times, dtype=float) for cost in costs}
+        self.h = pd.DataFrame(index=backtest_times,
+                              columns=universe, dtype=float)
+        self.u = pd.DataFrame(index=backtest_times,
+                              columns=universe, dtype=float)
+        self.z = pd.DataFrame(index=backtest_times,
+                              columns=universe, dtype=float)
+        self.costs = {cost.__class__.__name__: pd.Series(
+            index=backtest_times, dtype=float) for cost in costs}
         self.policy_times = pd.Series(index=backtest_times, dtype=float)
         self.simulator_times = pd.Series(index=backtest_times, dtype=float)
-    
-    
+
     @property
     def PPY(self):
         return periods_per_year(self.h.index)
 
     @property
     def v(self):
         """The value of the portfolio over time."""
@@ -88,25 +89,25 @@
         return pd.Series(
             data=val.values[1:] / val.values[:-1] - 1, index=val.index[:-1]
         )
 
     @property
     def excess_returns(self):
         return self.returns - self.cash_returns
-        
+
     @property
     def growth_rates(self):
         """The growth rate log(v_{t+1}/v_t)"""
         return np.log(self.returns + 1)
-        
+
     @property
     def excess_growth_rates(self):
         """The growth rate log(v_{t+1}/v_t)"""
         return np.log(self.excess_returns + 1)
-    
+
     # @property
     # def annual_growth_rate(self):
     #     """The annualized growth rate PPY/T sum_{t=1}^T log(v_{t+1}/v_t)"""
     #     return self.growth_rates.mean() * self.PPY
     #
     # @property
     # def annual_return(self):
@@ -139,66 +140,64 @@
             * np.mean(self.excess_returns)
             / np.std(self.excess_returns)
         )
 
     @property
     def turnover(self):
         """Turnover ||u_t||_1/(2*v_t)"""
-        return np.abs(self.u.iloc[:,:-1]).sum(axis=1) / (2*self.v.loc[self.u.index])
+        return np.abs(self.u.iloc[:, :-1]).sum(axis=1) / (2*self.v.loc[self.u.index])
 
     @property
     def trading_days(self):
         """The fraction of days with nonzero turnover."""
         return (self.turnover.values > 0).sum() / self.turnover.size
-        
+
     @property
     def drawdown(self):
         return -(1 - (self.v / self.v.cummax()))
-        
+
     def plot(self, show=True, how_many_weights=7):
         """Make plots."""
-        
+
         # value
         self.v.plot(figsize=(12, 5), label='Multi Period Optimization')
         plt.ylabel('USD')
         plt.yscale('log')
         plt.title('Total value of the portfolio in time')
-        
+
         # weights
-        biggest_weights = np.abs(self.w).mean().sort_values().iloc[-how_many_weights:].index
+        biggest_weights = np.abs(self.w).mean(
+        ).sort_values().iloc[-how_many_weights:].index
         self.w[biggest_weights].plot()
         plt.title('Largest weights of the portfolio in time')
-                
+
         if show:
             plt.show()
-        
 
     def __repr__(self):
         data = collections.OrderedDict({
             "Number of periods": self.u.shape[0],
             "Initial timestamp": self.h.index[0],
             "Universe size": self.h.shape[1],
             "Final timestamp": self.h.index[-1],
             "Total profit (PnL)": self.profit,
             "Annualized portfolio return (%)": self.returns.mean() * 100 * self.PPY,
             "Annualized excess return (%)": self.excess_returns.mean() * 100 * self.PPY,
-            "Annualized excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),            
+            "Annualized excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),
             "Sharpe ratio": self.sharpe_ratio,
             "Worst drawdown (%)": self.drawdown.min() * 100,
             "Average drawdown (%)": self.drawdown.mean() * 100,
             "Daily Turnover (%)": self.turnover.mean() * 100,
             "Annualized Turnover (%)": self.turnover.mean() * 100 * self.PPY,
-            
+
             "Average leverage (%)": self.leverage.mean() * 100,
             "Max leverage (%)": self.leverage.max() * 100})
-        
-        data.update(collections.OrderedDict({f'Average of {cost} per period (bp)': (self.costs[cost]/self.v).mean()*1E4 for cost in self.costs}))
-        
+
+        data.update(collections.OrderedDict({f'Average of {cost} per period (bp)': (
+            self.costs[cost]/self.v).mean()*1E4 for cost in self.costs}))
+
         data.update(collections.OrderedDict(
             {"Average policy time (sec)": self.policy_times.mean(),
-            "Average simulator time (sec)": self.simulator_times.mean()
-            }))
+             "Average simulator time (sec)": self.simulator_times.mean()
+             }))
 
         return 'Backtest Result:\n' + pd.Series(data=data).to_string(float_format="{:,.3f}".format)
-        
-
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/returns.py` & `cvxportfolio-0.4.3/cvxportfolio/returns.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 
 from .costs import BaseCost, CombinedCosts
 from .risks import BaseRiskModel
-from .estimator import DataEstimator #, ParameterEstimator
+from .estimator import DataEstimator  # , ParameterEstimator
 from .forecast import HistoricalMeanReturn, HistoricalMeanError
 
 __all__ = [
     "ReturnsForecast",
     "ReturnsForecastError",
     "CashReturn",
 ]
@@ -37,53 +37,52 @@
 
     Use this to define any logic common to return models.
     """
 
 
 class CashReturn(BaseReturnsModel):
     r"""Objective term representing cash return.
-    
+
     The forecast of cash return :math:`{\left(\hat{r}_t\right)}_n` is the observed value
     from last period :math:`{\left({r}_{t-1}\right)}_n`.
-    
+
     This object is included automatically in :class:`SinglePeriodOptimization`
     and :class:`MultiPeriodOptimization` policies. You can change
     this behavior by setting their ``include_cash_return`` to False.
-    
+
     :param short_margin_requirement: fraction of value of a short positions
         that is margined by portfolio cash
     :type short_margin_requirement: float
     """
-    
+
     def __init__(self, cash_returns=None, short_margin_requirement=1.):
-        self.cash_returns = None if cash_returns is None else DataEstimator(cash_returns, 
-            compile_parameter=True, non_negative=True)
+        self.cash_returns = None if cash_returns is None else DataEstimator(cash_returns,
+                                                                            compile_parameter=True, non_negative=True)
         self.short_margin_requirement = short_margin_requirement
-        
+
     def _pre_evaluation(self, universe, backtest_times):
         self.cash_return_parameter = cp.Parameter(nonneg=True) if self.cash_returns is None \
             else self.cash_returns.parameter
-            
+
         # else DataEstimator(self.cash_returns, non_negative=True, compile_parameter=True)
-        
-        
+
     def _values_in_time(self, t, past_returns, **kwargs):
         """Update cash return parameter as last cash return."""
         if self.cash_returns is None:
-            self.cash_return_parameter.value = past_returns.iloc[-1,-1]
-        
+            self.cash_return_parameter.value = past_returns.iloc[-1, -1]
+
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Apply cash return to "real" cash position (without shorts and margins)."""
-        realcash = (w_plus[-1] - (1 + self.short_margin_requirement) * cp.sum(cp.neg(w_plus[:-1])))
+        realcash = (w_plus[-1] - (1 + self.short_margin_requirement)
+                    * cp.sum(cp.neg(w_plus[:-1])))
         result = realcash * self.cash_return_parameter
         assert result.is_concave()
         return result
-        
-    
-    
+
+
 class ReturnsForecast(BaseReturnsModel):
     r"""Returns forecast for non-cash assets, provided by the user or computed from the data.
 
     This class represents the term :math:`\hat{r}_t`,
     the forecast of non-cash assets' returns at time :math:`t`.
     :ref:`Optimization-based policies` use this, typically as the first
     element of their objectives.
@@ -137,31 +136,31 @@
 
     Defines a single period optimization policy where the returns' forecasts
     :math:`\hat{r}_t` are the full average of past returns at each point in time
     and the risk model is the full covariance, also computed from the past returns.
     """
 
     def __init__(self, r_hat=None, decay=1.):
-        
+
         if not r_hat is None:
             self.r_hat = DataEstimator(r_hat)
         else:
             self.r_hat = HistoricalMeanReturn()
         self.decay = decay
-        
+
     def _pre_evaluation(self, universe, backtest_times):
         self.r_hat_parameter = cp.Parameter(len(universe)-1)
-        
+
     def _values_in_time(self, t, past_returns, mpo_step=0, **kwargs):
-        self.r_hat_parameter.value = self.r_hat.current_value * self.decay**(mpo_step)
+        self.r_hat_parameter.value = self.r_hat.current_value * \
+            self.decay**(mpo_step)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Cvxpy expression acts on non-cash assets."""
-        return w_plus[:-1].T @ self.r_hat_parameter 
-        
+        return w_plus[:-1].T @ self.r_hat_parameter
 
 
 class ReturnsForecastError(BaseRiskModel):
     """Simple return forecast error risk with values provided by the user.
 
     Implements the model described in pages 31-32 of the paper. You
     must pass the delta Series (if constant) or DataFrame (if time-varying)
@@ -175,27 +174,22 @@
         or varying in time (if DataFrame), 
         or fitted from the data as the standard deviation
         of the historical mean estimator 
     :type deltas_errors: pd.DataFrame or pd.Series or None
     """
 
     def __init__(self, deltas=None):
-        
+
         if not deltas is None:
             self.deltas = DataEstimator(deltas)
         else:
             self.deltas = HistoricalMeanError()
-            
+
     def _pre_evaluation(self, universe, backtest_times):
         self.deltas_parameter = cp.Parameter(len(universe)-1, nonneg=True)
 
-
     def _values_in_time(self, t, past_returns, **kwargs):
         self.deltas_parameter.value = self.deltas.current_value
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile to cvxpy expression."""
         return cp.abs(w_plus_minus_w_bm[:-1]).T @ self.deltas_parameter
-
-
-
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/risks.py` & `cvxportfolio-0.4.3/cvxportfolio/risks.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .estimator import DataEstimator 
+from .estimator import DataEstimator
 import logging
 import warnings
 
 import scipy.linalg
 
 import cvxpy as cp
 import numpy as np
@@ -33,32 +33,28 @@
     "DiagonalCovariance",
     "FactorModelCovariance",
     "RiskForecastError",
     "WorstCaseRisk",
 ]
 
 
-
-
 class BaseRiskModel(BaseCost):
     pass
 
 
-
-
 class FullCovariance(BaseRiskModel):
     """Quadratic risk model with full covariance matrix.
-    
+
     :param Sigma: DataFrame of covariance matrices
         supplied by the user, or None if fitting from the past data.
         The DataFrame can either represents a single constant covariance matrix
         or one for each point in time.
     :type Sigma: pandas.DataFrame or None
-    
-    
+
+
     """
     # r"""Quadratic risk model with full covariance matrix.
     #
     # This class represents the term :math:`\Sigma_t`, *i.e.,*
     # the :math:`(n-1) \times (n-1)` positive semi-definite matrix
     # which estimates the covariance of the (non-cash) assets' returns.
     # :ref:`Optimization-based policies` use this, as is explained
@@ -114,135 +110,138 @@
 
     def __init__(self, Sigma=None, kelly=True):
 
         if not Sigma is None:
             self.Sigma = DataEstimator(Sigma)
             self.alreadyfactorized = False
         else:
-            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) 
+            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly)
             self.alreadyfactorized = True
-            
+
     def _pre_evaluation(self, universe, backtest_times):
         self.Sigma_sqrt = cp.Parameter((len(universe)-1, len(universe)-1))
 
     def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        
+
         if self.alreadyfactorized:
             self.Sigma_sqrt.value = self.Sigma.current_value
         else:
             Sigma = self.Sigma.current_value
             eigval, eigvec = np.linalg.eigh(Sigma)
             eigval = np.maximum(eigval, 0.)
             self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        self.cvxpy_expression = cp.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
+        self.cvxpy_expression = cp.sum_squares(
+            self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
         return self.cvxpy_expression
 
+
 class RiskForecastError(BaseRiskModel):
     """Risk forecast error. 
-    
+
     Implements the model defined in page 31 of the book. Takes same arguments
     as :class:`DiagonalCovariance`.
-    
+
     :param sigma_squares: per-stock variances, indexed by time if DataFrame.
         If None it will be fitted on past data.
     :type sigma_squares: pd.DataFrame or pd.Series or None
     """
 
     def __init__(self, sigma_squares=None):
         if sigma_squares is None:
-            self.sigma_squares = HistoricalVariance(kelly=True) #None None
+            self.sigma_squares = HistoricalVariance(kelly=True)  # None None
         else:
             self.sigma_squares = DataEstimator(sigma_squares)
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         # self.zeroforcash=True
         # self.kelly=True
-        
+
     def _pre_evaluation(self, universe, backtest_times):
-        self.sigmas_parameter = cp.Parameter(len(universe)-1, nonneg=True)#+self.kelly))
+        self.sigmas_parameter = cp.Parameter(
+            len(universe)-1, nonneg=True)  # +self.kelly))
 
     def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        
+
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
         #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
         #         sigma_squares.iloc[-1] = 0.
         #     sigma_squares = sigma_squares.values
         # else:
         #     sigma_squares = self.sigma_squares.current_value
-            
+
         sigma_squares = self.sigma_squares.current_value
-        
+
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
         return cp.square(cp.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
-                
+
 
 class DiagonalCovariance(BaseRiskModel):
     """Diagonal covariance matrix, user-provided or fit from data.
 
     :param sigma_squares: per-stock variances, indexed by time if DataFrame.
         If None it will be fitted on past data.
     :type sigma_squares: pd.DataFrame or pd.Series or None 
     """
 
     def __init__(self, sigma_squares=None):
         if not sigma_squares is None:
             self.sigma_squares = DataEstimator(sigma_squares)
         else:
-            self.sigma_squares = HistoricalVariance(kelly=True) #None
-        #self.zeroforcash = True
-        #self.kelly = True
+            self.sigma_squares = HistoricalVariance(kelly=True)  # None
+        # self.zeroforcash = True
+        # self.kelly = True
         # self.standard_deviations = ParameterEstimator(standard_deviations)
-        
+
     def _pre_evaluation(self, universe, backtest_times):
-        self.sigmas_parameter = cp.Parameter(len(universe)-1) #+self.kelly))
+        self.sigmas_parameter = cp.Parameter(len(universe)-1)  # +self.kelly))
 
     def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        #super()._recursive_values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
-        
+        # super()._recursive_values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
+
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
         #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
         #         sigma_squares[-1] = 0.
         #     sigma_squares = sigma_squares.values
         # else:
         #     sigma_squares = self.sigma_squares.current_value
-        
+
         sigma_squares = self.sigma_squares.current_value
 
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
         return cp.sum_squares(cp.multiply(w_plus_minus_w_bm[:-1], self.sigmas_parameter))
 
 
 class FactorModelCovariance(BaseRiskModel):
     """Factor model covariance, either user-provided or fitted from the data.
-    
+
     It has the structure
-    
+
     :math:`F F^T + \mathbf{diag}(d)`
-    
+
     where :math:`F` is a *tall* matrix (many more rows than columns) and the vector
     :math:`d` is all non-negative. 
-    
+
     :param F: exposure matrices either constant or varying in time; if so, use a pandas multiindexed
          dataframe. If None it will be fitted.
     :type F: pd.DataFrame or None
     :param d: idyosyncratic variances either constant or varying in time; If None it will be fitted.
     :type d: pd.Series or pd.DataFrame or None
     :param num_factors: number of factors (columns of F), used if fitting the model
     :type num_factors: int    
@@ -261,51 +260,53 @@
     #     forecast_error_kappa (float or pd.Series): uncertainty on the
     #         assets' correlations. See the paper, pages 32-33.
 
     # """
 
     factor_Sigma = None
 
-    def __init__(self, F=None, d=None, num_factors=1, kelly=True):#, normalize=False):
-        self.F = F if F is None else DataEstimator(F, compile_parameter=True) 
-        self.d = d if d is None else DataEstimator(d) 
+    # , normalize=False):
+    def __init__(self, F=None, d=None, num_factors=1, kelly=True):
+        self.F = F if F is None else DataEstimator(F, compile_parameter=True)
+        self.d = d if d is None else DataEstimator(d)
         if (self.F is None) or (self.d is None):
             self.fit = True
-            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) #Sigma
+            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly)  # Sigma
         else:
             self.fit = False
         self.num_factors = num_factors
 
     def _pre_evaluation(self, universe, backtest_times):
         self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
         effective_num_factors = min(self.num_factors, len(universe)-1)
-        self.F_parameter = cp.Parameter((effective_num_factors, len(universe)-1)) if self.F is None else self.F.parameter
-
+        self.F_parameter = cp.Parameter((effective_num_factors, len(
+            universe)-1)) if self.F is None else self.F.parameter
 
     def _values_in_time(self, t, past_returns, **kwargs):
-        
+
         if self.fit:
             Sigmasqrt = self.Sigma.current_value
             # numpy eigendecomposition has largest eigenvalues last
             self.F_parameter.value = Sigmasqrt[:, -self.num_factors:].T
             d = np.sum(Sigmasqrt[:, :-self.num_factors]**2, axis=1)
         else:
             d = self.d.current_value
         self.idyosync_sqrt_parameter.value = np.sqrt(d)
 
-
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        self.expression = cp.sum_squares(cp.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
+        self.expression = cp.sum_squares(cp.multiply(
+            self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert self.expression.is_dcp(dpp=True)
 
-        self.expression += cp.sum_squares(self.F_parameter @ w_plus_minus_w_bm[:-1])
+        self.expression += cp.sum_squares(self.F_parameter @
+                                          w_plus_minus_w_bm[:-1])
         assert self.expression.is_dcp(dpp=True)
 
         return self.expression
-        
+
 
 class WorstCaseRisk(BaseRiskModel):
     """Select the most restrictive risk model for each value of the allocation vector.
 
     Given a list of risk models, penalize the portfolio allocation by the
     one with highest risk value at the solution point. If uncertain about
     which risk model to use this procedure can be an easy solution.
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/simulator.py` & `cvxportfolio-0.4.3/cvxportfolio/simulator.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,261 +42,281 @@
 PPY = 252
 __all__ = ['StockMarketSimulator', 'MarketSimulator']
 
 
 def _mp_init(l):
     global LOCK
     LOCK = l
-    
-    
+
+
 def _hash_universe(universe):
     return hashlib.sha256(bytes(str(tuple(universe)), 'utf-8')).hexdigest()
-     
-        
+
+
 def _load_cache(universe, trading_frequency, base_location):
     """Load cache from disk."""
-    folder = base_location/f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
+    folder = base_location / \
+        f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
     if 'LOCK' in globals():
         logging.debug(f'Acquiring cache lock from process {os.getpid()}')
         LOCK.acquire()
     try:
         with open(folder/'cache.pkl', 'rb') as f:
-            logging.info(f'Loading cache for universe = {universe} and trading_frequency = {trading_frequency}')
+            logging.info(
+                f'Loading cache for universe = {universe} and trading_frequency = {trading_frequency}')
             return pickle.load(f)
     except FileNotFoundError:
         logging.info(f'Cache not found!')
         return {}
     finally:
         if 'LOCK' in globals():
             logging.debug(f'Releasing cache lock from process {os.getpid()}')
             LOCK.release()
-    
-    
+
+
 def _store_cache(cache, universe, trading_frequency, base_location):
     """Store cache to disk."""
-    folder = base_location/f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
+    folder = base_location / \
+        f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
     if 'LOCK' in globals():
         logging.debug(f'Acquiring cache lock from process {os.getpid()}')
         LOCK.acquire()
     folder.mkdir(exist_ok=True)
     with open(folder/'cache.pkl', 'wb') as f:
-        logging.info(f'Storing cache for universe = {universe} and trading_frequency = {trading_frequency}')
+        logging.info(
+            f'Storing cache for universe = {universe} and trading_frequency = {trading_frequency}')
         pickle.dump(cache, f)
     if 'LOCK' in globals():
         logging.debug(f'Releasing cache lock from process {os.getpid()}')
         LOCK.release()
- 
 
-        
+
 class MarketData:
     """Prepare, hold, and serve market data. 
-    
+
     Not meant to be accessed by user. Most of its initialization
     is documented in MarketSimulator.    
     """
-    
-    def __init__(self, 
-        universe = [], 
-        returns=None,
-        volumes=None,
-        prices=None, 
-        datasource='YFinance',
-        cash_key='USDOLLAR',
-        base_location=BASE_LOCATION, 
-        min_history=pd.Timedelta('365.24d'),
-        max_contiguous_missing='365d', # TODO change logic for this (it's now this to not drop quarterly data)
-        trading_frequency=None,  
-        **kwargs,
-    ):
-        
+
+    def __init__(self,
+                 universe=[],
+                 returns=None,
+                 volumes=None,
+                 prices=None,
+                 datasource='YFinance',
+                 cash_key='USDOLLAR',
+                 base_location=BASE_LOCATION,
+                 min_history=pd.Timedelta('365.24d'),
+                 # TODO change logic for this (it's now this to not drop quarterly data)
+                 max_contiguous_missing='365d',
+                 trading_frequency=None,
+                 copy_dataframes=True,
+                 **kwargs,
+                 ):
+
         # drop duplicates and ensure ordering
         universe = sorted(set(universe))
-        
+
         self.base_location = Path(base_location)
         self.min_history_timedelta = min_history
         self.max_contiguous_missing = max_contiguous_missing
         self.cash_key = cash_key
-        
+
         if len(universe):
             self._get_market_data(universe, datasource)
             self._add_cash_column(self.cash_key)
             self._remove_missing_recent()
         else:
             if returns is None:
-                raise SyntaxError("If you don't specify a universe you should pass `returns`.")
-            # if not returns.shape[1] == volumes.shape[1] + 1:
-            #     raise SyntaxError(
-            #         "In `returns` you must include the cash returns as the last column (and not in `volumes`).")
-            self.returns = returns
-            self.volumes = volumes
-            self.prices = prices
+                raise SyntaxError(
+                    "If you don't specify a universe you should pass `returns`.")
+            self.returns = pd.DataFrame(returns, copy=copy)
+            self.volumes = volumes if volumes is None else \
+                pd.DataFrame(volumes, copy=copy)
+            self.prices = prices if prices is None else \
+                pd.DataFrame(prices, copy=copy)
             if cash_key != returns.columns[-1]:
                 self._add_cash_column(cash_key)
-                            
+
         if trading_frequency:
             self._downsample(trading_frequency)
-        
+
         self._set_read_only()
         self._check_sizes()
-    
-    
+
     def _reduce_universe(self, reduced_universe):
         assert reduced_universe[-1] == self.cash_key
-        logging.debug(f'Preparing MarketData with reduced_universe {reduced_universe}')
+        logging.debug(
+            f'Preparing MarketData with reduced_universe {reduced_universe}')
         return MarketData(
             returns=self.returns[reduced_universe],
-            volumes=self.volumes[reduced_universe[:-1]] if not (self.volumes is None) else None,
-            prices=self.prices[reduced_universe[:-1]] if not (self.prices is None) else None,
-            cash_key = self.cash_key)
-    
+            volumes=self.volumes[reduced_universe[:-1]
+                                 ] if not (self.volumes is None) else None,
+            prices=self.prices[reduced_universe[:-1]
+                               ] if not (self.prices is None) else None,
+            cash_key=self.cash_key,
+            copy_dataframes=False)
+
     @property
     def min_history(self):
         """Min. history expressed in periods."""
         return int(np.round(self.PPY * (self.min_history_timedelta / pd.Timedelta('365.24d'))))
-        
+
     @property
     def universe(self):
         return self.returns.columns
-        
-    sampling_intervals = {'weekly': 'W-MON', 'monthly':'MS', 'quarterly':'QS', 'annual':'AS'}
-        
+
+    sampling_intervals = {'weekly': 'W-MON',
+                          'monthly': 'MS', 'quarterly': 'QS', 'annual': 'AS'}
+
     def _downsample(self, interval):
         """_downsample market data."""
         if not interval in self.sampling_intervals:
-            raise SyntaxError('Unsopported trading interval for down-sampling.')
+            raise SyntaxError(
+                'Unsopported trading interval for down-sampling.')
         interval = self.sampling_intervals[interval]
-        self.returns = np.exp(np.log(1+self.returns).resample(interval, closed='left', label='left').sum(False, 1))-1
+        self.returns = np.exp(np.log(
+            1+self.returns).resample(interval, closed='left', label='left').sum(False, 1))-1
         if self.volumes is not None:
-            self.volumes = self.volumes.resample(interval, closed='left', label='left').sum(False, 1)
+            self.volumes = self.volumes.resample(
+                interval, closed='left', label='left').sum(False, 1)
         if self.prices is not None:
-            self.prices = self.prices.resample(interval, closed='left', label='left').first()
-        
+            self.prices = self.prices.resample(
+                interval, closed='left', label='left').first()
+
     @property
     def PPY(self):
         "Periods per year, assumes returns are about equally spaced."
         return periods_per_year(self.returns.index)
-        
-    
+
     def _check_sizes(self):
-        
-        if (not self.volumes is None) and (not (self.volumes.shape[1] == self.returns.shape[1] - 1) \
-            or not all(self.volumes.columns == self.returns.columns[:-1])):
-            raise SyntaxError('Volumes should have same columns as returns, minus cash_key.')
-        
-        if (not self.prices is None) and (not (self.prices.shape[1] == self.returns.shape[1] - 1) \
-            or not all(self.prices.columns == self.returns.columns[:-1])):
-            raise SyntaxError('Prices should have same columns as returns, minus cash_key.')            
-        
-        
+
+        if (not self.volumes is None) and (not (self.volumes.shape[1] == self.returns.shape[1] - 1)
+                                           or not all(self.volumes.columns == self.returns.columns[:-1])):
+            raise SyntaxError(
+                'Volumes should have same columns as returns, minus cash_key.')
+
+        if (not self.prices is None) and (not (self.prices.shape[1] == self.returns.shape[1] - 1)
+                                          or not all(self.prices.columns == self.returns.columns[:-1])):
+            raise SyntaxError(
+                'Prices should have same columns as returns, minus cash_key.')
+
     def _serve_data_policy(self, t):
         """Give data to policy at time t."""
         tidx = self.returns.index.get_loc(t)
         past_returns = pd.DataFrame(self.returns.iloc[:tidx])
         if not self.volumes is None:
             tidx = self.volumes.index.get_loc(t)
-            past_volumes = pd.DataFrame(self.volumes.iloc[:tidx]) 
+            past_volumes = pd.DataFrame(self.volumes.iloc[:tidx])
         else:
             past_volumes = None
-        current_prices = pd.Series(self.prices.loc[t]) if not self.prices is None else None
-        
+        current_prices = pd.Series(
+            self.prices.loc[t]) if not self.prices is None else None
+
         return past_returns, past_volumes, current_prices
-        
-    
+
     def _serve_data_simulator(self, t):
         """Give data to simulator at time t."""
         tidx = self.returns.index.get_loc(t)
         current_and_past_returns = pd.DataFrame(self.returns.iloc[:tidx+1])
         if not self.volumes is None:
             tidx = self.volumes.index.get_loc(t)
             current_and_past_volumes = pd.DataFrame(self.volumes.iloc[:tidx+1])
         else:
             current_and_past_volumes = None
-        current_prices = pd.Series(self.prices.loc[t]) if not self.prices is None else None
-        
+        current_prices = pd.Series(
+            self.prices.loc[t]) if not self.prices is None else None
+
         return current_and_past_returns, current_and_past_volumes, current_prices
-        
-        
+
     def _set_read_only(self):
         """Set numpy array contained in dataframe to read only.
-        
+
         This is enough to prevent direct assignement to the resulting 
         dataframe. However it could still be accidentally corrupted by assigning
         to columns or indices that are not present in the original.
         We avoid that case as well by returning a wrapped dataframe (which doesn't
         copy data on creation) in _serve_data_policy and _serve_data_simulator.
         """
-        
+
         def ro(df):
             data = df.values
             data.flags.writeable = False
             return pd.DataFrame(data, index=df.index, columns=df.columns)
-            
+
         self.returns = ro(self.returns)
-        
+
         if not self.prices is None:
             self.prices = ro(self.prices)
-            
+
         if not self.volumes is None:
             self.volumes = ro(self.volumes)
-            
+
     def _add_cash_column(self, cash_key):
-        
+
         if not cash_key == 'USDOLLAR':
-            raise NotImplementedError('Currently the only data pipeline built is for USDOLLAR cash')
-            
+            raise NotImplementedError(
+                'Currently the only data pipeline built is for USDOLLAR cash')
+
         data = FredTimeSeries('DFF', base_location=self.base_location)
         data._recursive_pre_evaluation()
-        self.returns[cash_key] = resample_returns(data.data / 100, periods=self.PPY)
-        self.returns[cash_key] = self.returns[cash_key].fillna(method='ffill')        
-    
+        self.returns[cash_key] = resample_returns(
+            data.data / 100, periods=self.PPY)
+        self.returns[cash_key] = self.returns[cash_key].fillna(method='ffill')
+
     DATASOURCES = {'YFinance': YfinanceTimeSeries, 'FRED': FredTimeSeries}
-    
+
     def _get_market_data(self, universe, datasource):
         database_accesses = {}
         print('Updating data')
-        
+
         for stock in universe:
-            logging.debug(f'Getting data for {stock} with {self.DATASOURCES[datasource]}.')
+            logging.debug(
+                f'Getting data for {stock} with {self.DATASOURCES[datasource]}.')
             print('.')
             database_accesses[stock] = self.DATASOURCES[datasource](
                 stock, base_location=self.base_location)
             database_accesses[stock]._recursive_pre_evaluation()
-            
+
         if datasource == 'YFinance':
-            self.returns = pd.DataFrame({stock: database_accesses[stock].data['Return'] for stock in universe})
-            self.volumes = pd.DataFrame({stock: database_accesses[stock].data['ValueVolume'] for stock in universe})
-            self.prices = pd.DataFrame({stock: database_accesses[stock].data['Open'] for stock in universe})
-        else: # only FRED for indexes
-            self.prices = pd.DataFrame({stock: database_accesses[stock].data for stock in universe}) # open prices
+            self.returns = pd.DataFrame(
+                {stock: database_accesses[stock].data['Return'] for stock in universe})
+            self.volumes = pd.DataFrame(
+                {stock: database_accesses[stock].data['ValueVolume'] for stock in universe})
+            self.prices = pd.DataFrame(
+                {stock: database_accesses[stock].data['Open'] for stock in universe})
+        else:  # only FRED for indexes
+            self.prices = pd.DataFrame(
+                {stock: database_accesses[stock].data for stock in universe})  # open prices
             self.returns = 1 - self.prices / self.prices.shift(-1)
-            self.volumes = None            
-        
+            self.volumes = None
+
     def _remove_missing_recent(self):
         """Clean recent data.
-        
+
         Yfinance has some issues with most recent data; 
         we remove recent days if there are NaNs.
         """
-        
+
         if self.prices.iloc[-5:].isnull().any().any():
-            logging.debug('Removing some recent lines because there are missing values.')
+            logging.debug(
+                'Removing some recent lines because there are missing values.')
             drop_at = self.prices.iloc[-5:].isnull().any(axis=1).idxmax()
             logging.debug(f'Dropping at index {drop_at}')
-            self.returns = self.returns.loc[self.returns.index<drop_at]
+            self.returns = self.returns.loc[self.returns.index < drop_at]
             if self.prices is not None:
-                self.prices = self.prices.loc[self.prices.index<drop_at]
+                self.prices = self.prices.loc[self.prices.index < drop_at]
             if self.volumes is not None:
-                self.volumes = self.volumes.loc[self.volumes.index<drop_at]
-        
+                self.volumes = self.volumes.loc[self.volumes.index < drop_at]
+
         # for consistency we must also nan-out the last row of returns and volumes
         self.returns.iloc[-1] = np.nan
         if self.volumes is not None:
             self.volumes.iloc[-1] = np.nan
-        
-        
+
     def _get_backtest_times(self, start_time=None, end_time=None, include_end=True):
         """Get trading calendar from market data."""
         result = self.returns.index
         result = result[result >= self._earliest_backtest_start]
         if start_time:
             result = result[result >= start_time]
         if end_time:
@@ -304,370 +324,331 @@
         if not include_end:
             result = result[:-1]
         return result
 
     @property
     def _break_timestamps(self):
         """List of timestamps at which a backtest should be broken.
-        
+
         An asset enters into a backtest after having non-NaN returns
         for self.min_history periods and exits after having NaN returns
         for self.max_contiguous_missing. Defaults values are 252 and 10 
         respectively.
         """
         self.entry_dates = defaultdict(list)
         self.exit_dates = defaultdict(list)
         for asset in self.returns.columns[:-1]:
             single_asset_returns = self.returns[asset].dropna()
-            if len(single_asset_returns) > self.min_history: 
-                self.entry_dates[single_asset_returns.index[self.min_history]].append(asset)
+            if len(single_asset_returns) > self.min_history:
+                self.entry_dates[single_asset_returns.index[self.min_history]].append(
+                    asset)
                 exit_date = single_asset_returns.index[-1]
                 if (self.returns.index[-1] - exit_date) >= pd.Timedelta(self.max_contiguous_missing):
-                    self.exit_dates[exit_date].append(asset) 
+                    self.exit_dates[exit_date].append(asset)
 
         _ = sorted(set(self.exit_dates) | set(self.entry_dates))
         logging.debug(f'computing break timestamps {_}')
         return _
-        
-    @property    
+
+    @property
     def _limited_universes(self):
         """Valid universes for each section, minus cash.
-        
+
         A backtest is broken into multiple ones that start at each key
         of this, have the universe specified by this, and end
         at the next startpoint.  
         """
         result = OrderedDict()
         uni = []
         for ts in self._break_timestamps:
             uni += self.entry_dates[ts]
             uni = [el for el in uni if not el in self.exit_dates[ts]]
             result[ts] = tuple(sorted(uni))
         return result
-    
+
     @property
     def _earliest_backtest_start(self):
         """Earliest date at which we can start a backtest."""
-        return self.returns.iloc[:,:-1].dropna(how='all').index[self.min_history]
-        
-        
+        return self.returns.iloc[:, :-1].dropna(how='all').index[self.min_history]
+
     def _get_limited_backtests(self, start_time, end_time):
         """Get start/end times and universes of constituent backtests.
-        
+
         Each one has constant universe with assets' that meet the
         ``min_history`` requirement and has not disappeared from the
         dataset.
         """
-                
+
         full_backtest_times = self._get_backtest_times(start_time, end_time)
         brkt = np.array(self._break_timestamps)
 
-        def get_valid_universe_and_its_expiration_for(time):    
+        def get_valid_universe_and_its_expiration_for(time):
             try:
-                return self._limited_universes[brkt[brkt<=time][-1]], \
-                    brkt[brkt>time][0] if len(brkt[brkt>time]) else full_backtest_times[-1]
+                return self._limited_universes[brkt[brkt <= time][-1]], \
+                    brkt[brkt > time][0] if len(
+                        brkt[brkt > time]) else full_backtest_times[-1]
             except IndexError:
-                raise DataError('There are no assets that meet the required min_history.')
-        
+                raise DataError(
+                    'There are no assets that meet the required min_history.')
+
         result = []
         start = full_backtest_times[0]
         while True:
-            
-            universe, expiration = get_valid_universe_and_its_expiration_for(start)
+
+            universe, expiration = get_valid_universe_and_its_expiration_for(
+                start)
             if expiration > full_backtest_times[-1]:
                 expiration = full_backtest_times[-1]
             result.append({
                 'start_time': start,
                 'end_time': expiration,
                 'universe': list(universe) + [self.cash_key]})
-            
+
             if expiration == full_backtest_times[-1]:
                 return result
 
             start = expiration
-        
 
-    # :param spreads: historical bid-ask spreads expressed as (ask-bid)/bid. Default is None,
-    #     equivalent to 0.0. Practical spreads are negligible on US liquid stocks.
-    # :type spreads: pandas.DataFrame
-    #
-    # :param window_sigma_estimate: we use an historical rolling standard deviation to estimate the average
-    #     size of the return on a stock on each day, and this multiplies the second term of the transaction cost model.
-    #     See the paper for an explanation of the model. Here you specify the length of the rolling window to use,
-    #     default is 252 (typical number of trading days in a year).
-    # :type window_sigma_estimate: int
-    
 
 class MarketSimulator:
     """This class is a generic financial market simulator.
-    
+
     It is (currently) not meant to be used directly. Look at
     :class:`StockMarketSimulator` for its version specialized
     to the stock market.
     """
 
-
     def __init__(self, universe=[], returns=None, volumes=None,
-                 prices=None, costs=[], round_trades=False, 
+                 prices=None, costs=[], round_trades=False,
                  min_history=pd.Timedelta('365d'),
                  datasource='YFinance',
                  cash_key="USDOLLAR", base_location=BASE_LOCATION,
                  trading_frequency=None, **kwargs):
         """Initialize the Simulator and download data if necessary."""
         self.base_location = Path(base_location)
         
+        self.enable_caching = not len(universe)
+
         self.market_data = MarketData(
             universe=universe, returns=returns,
             volumes=volumes, prices=prices,
             cash_key=cash_key, base_location=base_location,
             trading_frequency=trading_frequency,
             min_history=min_history,
             datasource=datasource,
             **kwargs)
-            
+
         self.trading_frequency = trading_frequency
-                
+
         if not len(universe) and prices is None:
             if round_trades:
                 raise SyntaxError(
-                    "If you don't specify prices you can't request `round_trades`.")
+                    "If you don't specify prices you can't request "
+                    + "`round_trades`.")
 
-        self.round_trades = round_trades        
+        self.round_trades = round_trades
         self.costs = [el() if isinstance(el, type) else el for el in costs]
         # self.lock = Lock()
        # self.kwargs = kwargs
 
-        
     @staticmethod
     def _round_trade_vector(u, current_prices):
         """Round dollar trade vector u.
         """
         result = pd.Series(u, copy=True)
         result[:-1] = np.round(u[:-1] / current_prices) * current_prices
         result[-1] = -sum(result[:-1])
         return result
 
-
     def _simulate(self, t, h, policy, **kwargs):
         """Get next portfolio and statistics used by Backtest for reporting.
 
         The signature of this method differs from other estimators
-        because we pass the policy directly to it, and the past returns and past volumes
-        are computed by it.
+        because we pass the policy directly to it, and the past returns 
+        and past volumes are computed by it.
         """
-        
+
         # translate to weights
         current_portfolio_value = sum(h)
         current_weights = h / current_portfolio_value
 
-        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
+        past_returns, past_volumes, current_prices = \
+            self.market_data._serve_data_policy(t)
 
         # evaluate the policy
         s = time.time()
-        z = policy._recursive_values_in_time(t=t, current_weights=current_weights, current_portfolio_value=current_portfolio_value, 
-            past_returns=past_returns, past_volumes=past_volumes, current_prices=current_prices, **kwargs)
+        z = policy._recursive_values_in_time(
+            t=t, current_weights=current_weights,
+            current_portfolio_value=current_portfolio_value,
+            past_returns=past_returns, past_volumes=past_volumes,
+            current_prices=current_prices, **kwargs)
+
         policy_time = time.time() - s
-        
+
         # for safety recompute cash
         z[-1] = -sum(z[:-1])
         assert sum(z) == 0.
-        
+
         # trades in dollars
         u = z * current_portfolio_value
-        
+
         # get data for simulator
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = \
+            self.market_data._serve_data_simulator(t)
 
-        # zero out trades on stock that weren't trading on that day 
+        # zero out trades on stock that weren't trading on that day
         if not (current_and_past_volumes is None):
             current_volumes = current_and_past_volumes.iloc[-1]
             non_tradable_stocks = current_volumes[current_volumes <= 0].index
             u[non_tradable_stocks] = 0.
 
         # round trades
         if self.round_trades:
             u = self._round_trade_vector(u, current_prices)
-            
+
         # for safety recompute cash
         u[-1] = -sum(u[:-1])
         assert sum(u) == 0.
 
         # compute post-trade holdings (including cash balance)
         h_plus = h + u
 
         # evaluate cost functions
-        realized_costs = {cost.__class__.__name__: cost._simulate(t=t, u=u,  h_plus=h_plus, 
-            current_and_past_volumes=current_and_past_volumes, 
+        realized_costs = {cost.__class__.__name__: cost._simulate(
+            t=t, u=u,  h_plus=h_plus,
+            current_and_past_volumes=current_and_past_volumes,
             current_and_past_returns=current_and_past_returns,
             current_prices=current_prices,
             periods_per_year=self.market_data.PPY,
-            windowsigma=self.market_data.PPY, #**self.kwargs
-            ) for cost in self.costs}
-        
+            windowsigma=self.market_data.PPY) for cost in self.costs}
+
         # initialize tomorrow's holdings
         h_next = pd.Series(h_plus, copy=True)
-        
+
         # credit costs to cash account
         h_next[-1] = h_plus[-1] + sum(realized_costs.values())
 
         # multiply positions by market returns
         current_returns = current_and_past_returns.iloc[-1]
         h_next *= (1 + current_returns)
-            
-        return h_next, z, u, realized_costs, policy_time
-        
-    def _initialize_policy(self, policy, start_time, end_time):
-        """Initialize the policy object.
-        """
-        policy._recursive_pre_evaluation(universe = self.market_data.universe,
-                             backtest_times = self.market_data._get_backtest_times(start_time, end_time, include_end=False))
-
-        # if policy initialized a cache, rewrite it with loaded one
-        #if hasattr(policy, 'cache'):
-        #    policy.cache = _load_cache(universe=self.market_data.universe, trading_frequency = self.trading_frequency,
-        #        base_location=self.base_location)
 
+        return h_next, z, u, realized_costs, policy_time
 
-    def _single_backtest(self, policy, start_time, end_time, h, universe=None#, backtest_times=None
-    ):
+    def _single_backtest(self, policy, start_time, end_time, h, universe=None):
         if universe is None:
             universe = self.market_data.universe
-        #if backtest_times is None:
-        backtest_times = self.market_data._get_backtest_times(start_time, end_time, include_end=False)
-
-        # self._initialize_policy(policy, start_time, end_time)
+        backtest_times = self.market_data._get_backtest_times(
+            start_time, end_time, include_end=False)
 
         if hasattr(policy, '_compile_to_cvxpy'):
             policy._compile_to_cvxpy()
 
         result = BacktestResult(universe, backtest_times, self.costs)
 
         # this is the main loop of a backtest
         for t in backtest_times:
             result.h.loc[t] = h
-            # print(t, h)
             s = time.time()
             h, result.z.loc[t], result.u.loc[t], realized_costs, \
-                    result.policy_times.loc[t] = self._simulate(t=t, h=h, policy=policy)
+                result.policy_times.loc[t] = self._simulate(
+                    t=t, h=h, policy=policy)
             for cost in realized_costs:
                 result.costs[cost].loc[t] = realized_costs[cost]
-            result.simulator_times.loc[t] = time.time() - s - result.policy_times.loc[t]
+            result.simulator_times.loc[t] = time.time(
+            ) - s - result.policy_times.loc[t]
 
         result.h.loc[pd.Timestamp(end_time)] = h
 
-        # TODO fix this
-        result.cash_returns = self.market_data.returns.iloc[:,-1].loc[result.u.index]
-
-        #if hasattr(policy, 'cache'):
-        #    _store_cache(cache=policy.cache, universe=universe,
-        #    trading_frequency = self.trading_frequency, base_location=self.base_location)
+        result.cash_returns = \
+            self.market_data.returns.iloc[:, -1].loc[result.u.index]
 
         return result
 
-    def _concatenated_backtests(self, policy, start_time, end_time, h):#, lock): #, caches_before=None):
-        constituent_backtests_params = self.market_data._get_limited_backtests(start_time, end_time)
+    def _concatenated_backtests(self, policy, start_time, end_time, h):
+        constituent_backtests_params = self.market_data._get_limited_backtests(
+            start_time, end_time)
         results = []
-        caches_after = {}
         orig_md = self.market_data
         orig_policy = policy
         for el in constituent_backtests_params:
             logging.info(f"current universe: {el['universe']}")
             logging.info(f"interval: {el['start_time']}, {el['end_time']}")
             self.market_data = orig_md._reduce_universe(el['universe'])
-            
+
             # TODO improve
             if len(el['universe']) > len(h):
                 tmp = pd.Series(0, el['universe'])
                 tmp[h.index] = h
                 h = tmp
             else:
                 h = h[el['universe']]
 
             policy = copy.deepcopy(orig_policy)
-            policy._recursive_pre_evaluation(universe = el['universe'],
-                backtest_times = self.market_data._get_backtest_times(el['start_time'], el['end_time'], include_end=True))
-            
-            if hasattr(policy, 'cache'):
+            policy._recursive_pre_evaluation(
+                universe=el['universe'],
+                backtest_times=self.market_data._get_backtest_times(
+                    el['start_time'], el['end_time'], include_end=True)
+            )
+
+            # if policy uses a cache load it from disk
+            if hasattr(policy, 'cache') and self.enable_caching:
                 logging.info('Trying to load cache from disk...')
-                policy.cache = _load_cache(universe=el['universe'], 
-                    trading_frequency = self.trading_frequency, 
-                    base_location=self.base_location)#,
-                    #lock=lock)
-            
-            # if hasattr(policy, 'cache') and tuple(el['universe']) in caches_before:
-            #     logging.info('Attaching cache loaded from disk to policy')
-            #     policy.cache = caches_before[tuple(el['universe'])]
+                policy.cache = _load_cache(
+                    universe=el['universe'],
+                    trading_frequency=self.trading_frequency,
+                    base_location=self.base_location)
 
-            results.append(self._single_backtest(policy, el['start_time'], el['end_time'], h, el['universe']))
+            results.append(self._single_backtest(
+                policy, el['start_time'], el['end_time'], h, el['universe']))
 
             h = results[-1].h.iloc[-1]
-            
-            if hasattr(policy, 'cache'):
+
+            # if policy used a cache write it to disk
+            if hasattr(policy, 'cache') and self.enable_caching:
                 logging.info('Storing cache from policy to disk...')
-                _store_cache(cache=policy.cache, universe=el['universe'], 
-                    trading_frequency=self.trading_frequency, 
-                    base_location=self.base_location)#,
-                    #lock=lock)
-                # logging.info('Extracting cache from policy to return to main process')
-                # caches_after[tuple(el['universe'])] = policy.cache
-        
-        self.market_data = orig_md
-        
-        return self._concatenate_backtest_results(results) #, caches_after
+                _store_cache(cache=policy.cache, universe=el['universe'],
+                             trading_frequency=self.trading_frequency,
+                             base_location=self.base_location)
 
+        self.market_data = orig_md
 
-    # def _store_caches(self, caches_after):
-    #     """Store caches after backtest"""
-    #     for k in caches_after:
-    #         _store_cache(cache=caches_after[k], universe=list(k), trading_frequency=self.trading_frequency,
-    #             base_location=self.base_location)
-    #
-    #
-    # def _load_caches(self, start_time, end_time):
-    #     """Load caches before backtest"""
-    #     caches_before = {}
-    #     constituent_backtests_params = self.market_data._get_limited_backtests(start_time, end_time)
-    #     for el in constituent_backtests_params:
-    #         caches_before[tuple(el['universe'])] = _load_cache(universe=el['universe'],
-    #             trading_frequency = self.trading_frequency, base_location=self.base_location)
-    #     return caches_before
+        return self._concatenate_backtest_results(results)
 
-        
     def _concatenate_backtest_results(self, results):
-        
+
         res = BacktestResult.__new__(BacktestResult)
         res.costs = {}
-        
-        res.h = pd.concat([el.h.iloc[:-1] if i < len(results) -1 else el.h for i, el in enumerate(results)])
+
+        res.h = pd.concat([el.h.iloc[:-1] if i < len(results) -
+                          1 else el.h for i, el in enumerate(results)])
         for attr in ['cash_returns', 'u', 'z', 'simulator_times', 'policy_times']:
-            res.__setattr__(attr, pd.concat([el.__getattribute__(attr) for el in results]) )
-            
+            res.__setattr__(attr, pd.concat(
+                [el.__getattribute__(attr) for el in results]))
+
         # pandas concat can misalign the columns ordering
         ck = self.market_data.cash_key
         sortcol = sorted([el for el in res.u.columns if not el == ck]) + [ck]
         res.u = res.u[sortcol]
         res.z = res.z[sortcol]
         res.h = res.h[sortcol]
         for k in results[0].costs:
             res.costs[k] = pd.concat([el.costs[k] for el in results])
 
         return res
-        
-    
+
     @staticmethod
-    def _worker(policy, simulator, start_time, end_time, h):#, lock): #, caches_before):
-        return simulator._concatenated_backtests(policy, start_time, end_time, h)#, lock) #, caches_before)
+    def _worker(policy, simulator, start_time, end_time, h):
+        return simulator._concatenated_backtests(policy, start_time, end_time, h)
 
-        
-    def backtest(self, policy, start_time=None, end_time=None, initial_value = 1E6, h=None):
+    def backtest(self, policy, start_time=None, end_time=None, initial_value=1E6, h=None):
         """Backtest trading policy.
-        
+
         The default initial portfolio is all cash, or you can pass any portfolio with
         the `h` argument.
-        
+
         :param policy: trading policy
         :type policy: cvx.BaseTradingPolicy
         :param start_time: start time of the backtest; if market it close, the first trading day
              after it is selected
         :type start_time: str or datetime 
         :param end_time: end time of the backtest; if market it close, the last trading day
              before it is selected
@@ -675,28 +656,28 @@
         :param initial_value: initial value in dollar of the portfolio, if not specifying
             ``h`` it is assumed the initial portfolio is all cash; if ``h`` is specified 
             this is ignored
         :type initial_value: float
         :param h: initial portfolio ``h`` expressed in dollar positions. If ``None`` 
             an initial portfolio of ``initial_value`` in cash is used.
         :type h: pd.Series or None
-        
+
         :returns result: instance of :class:`BacktestResult` which has all relevant backtest
             data and logic to compute metrics, generate plots, ...
         :rtype result: cvx.BacktestResult
         """
-        return self.backtest_many([policy], start_time = start_time, end_time = end_time, 
-                             initial_value = initial_value, h=None if h is None else [h], parallel=False)[0]
-                                    
-    def backtest_many(self, policies, start_time=None, end_time=None, initial_value = 1E6, h=None, parallel=True):
+        return self.backtest_many([policy], start_time=start_time, end_time=end_time,
+                                  initial_value=initial_value, h=None if h is None else [h], parallel=False)[0]
+
+    def backtest_many(self, policies, start_time=None, end_time=None, initial_value=1E6, h=None, parallel=True):
         """Backtest many trading policies.
-        
+
         The default initial portfolio is all cash, or you can pass any portfolio with
         the `h` argument, or a list of those.
-        
+
         :param policies: trading policies
         :type policy: list of cvx.BaseTradingPolicy:
         :param start_time: start time of the backtests; if market it close, the first trading day
              after it is selected. Currently it is not possible to specify different start times
             for different policies, so the same is used for all.
         :type start_time: str or datetime 
         :param end_time: end time of the backtests; if market it close, the last trading day
@@ -711,63 +692,58 @@
             is specified, ``initial_value`` is ignored, otherwise the same portfolio of 
             ``initial_value`` all in cash is used as starting point for all backtests.
         :type h: list or pd.Series or None
         :param parallel: whether to run in parallel. If runnning in parallel you **must be careful 
             at how you use this method**. If you use this in a script, you *should* define the MarketSimulator
             *in* the `if __name__ == '__main__:'` clause, and call this method there as well.
         :type parallel: bool
-        
+
         :returns result: list of instances of :class:`BacktestResult` which have all relevant backtest
             data and logic to compute metrics, generate plots, ...
         :rtype result: list of cvx.BacktestResult
         """
-        
+
         if not hasattr(policies, '__len__'):
             raise SyntaxError('You should pass a list of policies.')
-        
+
         if not hasattr(h, '__len__'):
             h = [h] * len(policies)
-            
+
         if not (len(policies) == len(h)):
-            raise SyntaxError('If passing lists of policies and initial portfolios they must have the same length.')
-        
-            
-        backtest_times_inclusive = self.market_data._get_backtest_times(start_time, end_time, include_end=True)
+            raise SyntaxError(
+                'If passing lists of policies and initial portfolios they must have the same length.')
+
+        backtest_times_inclusive = self.market_data._get_backtest_times(
+            start_time, end_time, include_end=True)
         start_time = backtest_times_inclusive[0]
         end_time = backtest_times_inclusive[-1]
-        
+
         # initialize policies and get initial portfolios
-        for i in range(len(policies)):        
+        for i in range(len(policies)):
             if h[i] is None:
                 h[i] = pd.Series(0., self.market_data.universe)
                 h[i][-1] = initial_value
-                
-        # caches_before = self._load_caches(start_time=start_time, end_time=end_time)
-        
+
         n = len(policies)
-        lock = Lock()
-        zip_args = zip(policies, [self] * n, [start_time] * n, [end_time] * n, h)#, [lock]*n) #, [caches_before]*n)
-        
-        # decide if run in parallel or not
-        if (not parallel) or len(policies)==1: 
+
+        zip_args = zip(policies, [self] * n,
+                       [start_time] * n, [end_time] * n, h)
+
+        if (not parallel) or len(policies) == 1:
             result = list(starmap(self._worker, zip_args))
         else:
             with Pool(initializer=_mp_init, initargs=(Lock(),)) as p:
-                result = p.starmap(self._worker, zip_args)   
+                result = p.starmap(self._worker, zip_args)
 
-        # for el in result:
-        #     self._store_caches(el[1])
-        
-        # return [el[0] for el in result]
         return [el for el in result]
-        
+
 
 class StockMarketSimulator(MarketSimulator):
     """This class implements a simulator of the stock market.
-    
+
     We strive to make the parameters here as accurate as possible. The following is
     accurate as of 2023 using numbers obtained on the public website of a
     `large US-based broker <https://www.interactivebrokers.com/>`_.
 
     :param universe: list of `Yahoo Finance <https://finance.yahoo.com/>`_ tickers on which to
         simulate performance of the trading strategy. If left unspecified you should at least
         pass `returns` and `volumes`. If you define a different market data access interface
@@ -806,55 +782,20 @@
         The default interface (Yahoo finance) provides daily trading data, 
         and so that is the default frequency for trades. With this argument you can set instead 
         the trading frequency to ``"weekly"``, which trades every Monday (or the first
         non-holiday trading day of each week), ``"monthly"``, which trades every first of the month (ditto), 
         ``"quarterly"``, and ``"annual"``. 
     :type trading_frequency: str or None
     """
-    
-    
+
     def __init__(self, universe=[],
-        returns=None, volumes=None, prices=None,
-        costs=[StocksTransactionCost, StocksHoldingCost],
-        round_trades=True, min_history=pd.Timedelta('365d'),
-        cash_key="USDOLLAR", base_location=BASE_LOCATION,
-        trading_frequency=None, **kwargs):
-        
-        super().__init__(universe=universe,
-            returns=returns, volumes=volumes, prices=prices,
-            costs=costs, round_trades=round_trades, min_history=min_history,
-            cash_key=cash_key, base_location=base_location,
-            trading_frequency=trading_frequency, **kwargs)
+                 returns=None, volumes=None, prices=None,
+                 costs=[StocksTransactionCost, StocksHoldingCost],
+                 round_trades=True, min_history=pd.Timedelta('365d'),
+                 cash_key="USDOLLAR", base_location=BASE_LOCATION,
+                 trading_frequency=None, **kwargs):
 
-# def _do_single_backtest(policy, start_time, end_time, simulator, cache):
-#     """This function can run on remote process/machine."""
-#
-#     universe = simulator.market_data.universe
-#     backtest_times = simulator.market_data._get_backtest_times(start_time, end_time)
-#
-#     policy._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
-#     if hasattr(policy, 'cache'):
-#         policy.cache = cache
-#     if hasattr(policy, '_compile_to_cvxpy'):
-#         policy._compile_to_cvxpy()
-#
-#     result = BacktestResult(universe, backtest_times, simulator.costs)
-#
-#     # this is the main loop of a backtest
-#     for t in backtest_times:
-#         result.h.loc[t] = h
-#         s = time.time()
-#         h, result.z.loc[t], result.u.loc[t], realized_costs, \
-#                 result.policy_times.loc[t] = simulator.simulate(t=t, h=h, policy=policy)
-#         for cost in realized_costs:
-#             result.costs[cost].loc[t] = realized_costs[cost]
-#         result.simulator_times.loc[t] = time.time() - s - result.policy_times.loc[t]
-#
-#     result.h.loc[pd.Timestamp(end_time)] = h
-#
-#     # TODO fix this
-#     result.cash_returns = simulator.market_data.returns.iloc[:,-1].loc[result.u.index]
-#
-#     return result, policy.cache
-#
-    
-    
+        super().__init__(universe=universe,
+                         returns=returns, volumes=volumes, prices=prices,
+                         costs=costs, round_trades=round_trades, min_history=min_history,
+                         cash_key=cash_key, base_location=base_location,
+                         trading_frequency=trading_frequency, **kwargs)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/base.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,22 +18,26 @@
 import numpy as np
 import pandas as pd
 import cvxpy as cp
 import cvxportfolio as cvx
 
 
 class BaseTestClass(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
-        cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
-        cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
+        cls.sigma = pd.read_csv(
+            Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.volumes = pd.read_csv(
+            Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-    
+
     def boilerplate(self, model):
-        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
+        return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.4.3/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.4.3/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,78 +18,91 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import cvxpy as cp
 import cvxportfolio as cvx
 
+def listvalue(li):
+    return all([el.value() for el in li])
+
 
 class TestConstraints(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
-        cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
-        cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
+        cls.sigma = pd.read_csv(
+            Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.volumes = pd.read_csv(
+            Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-        
+
     def build_constraint(self, constraint, t=None):
         """Initialize constraint, build expression, and point it to given time."""
-        constraint._recursive_pre_evaluation(self.returns.columns, self.returns.index)
-        cvxpy_expression = constraint._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        constraint._recursive_values_in_time(t=pd.Timestamp("2020-01-01") if t is None else t, current_portfolio_value=1000)
+        constraint._recursive_pre_evaluation(
+            self.returns.columns, self.returns.index)
+        cvxpy_expression = constraint._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        constraint._recursive_values_in_time(t=pd.Timestamp(
+            "2020-01-01") if t is None else t, current_portfolio_value=1000)
         return cvxpy_expression
-        
+
     def test_long_only(self):
         model = cvx.LongOnly()
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N)
-        self.assertTrue(cons.value())
+        self.assertTrue(listvalue(cons))
         self.w_plus.value = -np.ones(self.N)
-        self.assertFalse(cons.value())
-        
-    
+        self.assertFalse(listvalue(cons))
+        model = cvx.LongOnly(nocash=True)
+        cons = self.build_constraint(model)
+        self.w_plus.value = np.ones(self.N)
+        self.assertFalse(listvalue(cons))
+
     def test_long_cash(self):
         model = cvx.LongCash()
         cons = self.build_constraint(model)
-        self.w_plus.value = np.ones( self.N)
+        self.w_plus.value = np.ones(self.N)
         self.assertTrue(cons.value())
-        tmp = np.ones( self.N)
+        tmp = np.ones(self.N)
         tmp[-1] = -1
         self.w_plus.value = tmp
         self.assertTrue(cons.is_dcp())
         self.assertFalse(cons.value())
-        
+
     def test_min_cash(self):
-        model = cvx.MinCashBalance(10000) # USD
+        model = cvx.MinCashBalance(10000)  # USD
         cons = self.build_constraint(model)
-        self.w_plus.value = np.zeros( self.N)
+        self.w_plus.value = np.zeros(self.N)
         self.w_plus.value[-1] = 1
-        model._recursive_values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=10001)
+        model._recursive_values_in_time(t=pd.Timestamp(
+            "2020-01-01"), current_portfolio_value=10001)
         self.assertTrue(cons.value())
-        model._recursive_values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=9999)
-        self.assertFalse(cons.value())        
-        
+        model._recursive_values_in_time(t=pd.Timestamp(
+            "2020-01-01"), current_portfolio_value=9999)
+        self.assertFalse(cons.value())
 
     def test_dollar_neutral(self):
         model = cvx.DollarNeutral()
         cons = self.build_constraint(model)
-        tmpvalue = np.zeros( self.N)
+        tmpvalue = np.zeros(self.N)
         tmpvalue[-1] = 1 - sum(tmpvalue[:-1])
         self.w_plus.value = tmpvalue
         self.assertTrue(cons.value())
         tmpvalue = np.ones(self.N)
         tmpvalue[-1] = 1 - sum(tmpvalue[:-1])
         self.w_plus.value = tmpvalue
         self.assertFalse(cons.value())
-        
+
     def test_leverage_limit(self):
         model = cvx.LeverageLimit(2)
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertTrue(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
@@ -99,28 +112,28 @@
         model = cvx.LeverageLimit(7)
         cons = self.build_constraint(model)
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-    
+
     def test_leverage_limit_in_time(self):
         limits = pd.Series(index=self.returns.index, data=2)
         limits.iloc[1] = 7
         model = cvx.LeverageLimit(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
-        
+
     def test_max_weights(self):
         model = cvx.MaxWeights(2)
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertTrue(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
@@ -146,15 +159,15 @@
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
-        
+
     def test_min_weights(self):
         model = cvx.MinWeights(2)
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
@@ -179,50 +192,51 @@
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
         model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
 
     def test_factor_max_limit(self):
-        
-        model = cvx.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
+
+        model = cvx.FactorMaxLimit(
+            np.ones((self.N - 1, 2)), np.array([0.5, 1]))
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertFalse(cons.value())
-        
 
         model = cvx.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
-        cons = self.build_constraint(model,self.returns.index[1])
+        cons = self.build_constraint(model, self.returns.index[1])
 
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
 
     def test_factor_min_limit(self):
-        
-        model = cvx.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
+
+        model = cvx.FactorMinLimit(
+            np.ones((self.N - 1, 2)), np.array([0.5, 1]))
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
-        
+
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-        
+
         model = cvx.FactorMinLimit(np.ones((self.N - 1, 2)), np.array([4, 4]))
         cons = self.build_constraint(model, self.returns.index[1])
         # cons = model.weight_expr(t, self.w_plus, None, None)[0]
         tmp = np.zeros(self.N)
         tmp[0] = 4
         # tmp[1] = -3
         self.w_plus.value = tmp
@@ -235,46 +249,49 @@
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertFalse(cons.value())
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-        
+
     def test_turnover_limit(self):
         model = cvx.TurnoverLimit(0.1)
         cons = self.build_constraint(model)
         self.z.value = np.zeros(self.N)
         self.z.value[-1] = -sum(self.z.value[:-1])
         self.assertTrue(cons.value())
-        
+
         self.z.value[1] = 0.2
         self.z.value[-1] = -sum(self.z.value[:-1])
         self.assertTrue(cons.value())
-        
+
         self.z.value[2] = -0.01
         self.z.value[-1] = -sum(self.z.value[:-1])
         self.assertFalse(cons.value())
 
-        
     def test_participation_rate(self):
         """Test trading constraints."""
 
         t = self.returns.index[1]
 
         # avg daily value limits.
         value = 1e6
-        model = cvx.ParticipationRateLimit(self.volumes, max_fraction_of_volumes=0.1)
-        model._recursive_pre_evaluation(self.returns.columns, self.returns.index)
-        cons = model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model = cvx.ParticipationRateLimit(
+            self.volumes, max_fraction_of_volumes=0.1)
+        model._recursive_pre_evaluation(
+            self.returns.columns, self.returns.index)
+        cons = model._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
         model._recursive_values_in_time(t=t, current_portfolio_value=value)
         print(model.portfolio_value.value)
         # cons = model.weight_expr(t, None, z, value)[0]
         tmp = np.zeros(self.N)
         tmp[:-1] = self.volumes.loc[t].values / value * 0.05
         self.z.value = tmp
         self.assertTrue(cons.value())
         self.z.value = -100 * self.z.value  # -100*np.ones(n)
         self.assertFalse(cons.value())
 
+
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_costs.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,171 +23,188 @@
 
 from cvxportfolio.costs import *
 from cvxportfolio.returns import *
 from cvxportfolio.risks import *
 # from cvxportfolio.legacy import LegacyReturnsForecast #, MultipleReturnsForecasts
 
 
-
 class TestCosts(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
-        cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.volumes = pd.read_csv(
+            Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cvx.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cvx.Variable(cls.returns.shape[1])
         cls.z = cvx.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-        
-        
+
     def test_cost_algebra(self):
         # n = len(self.returns.columns)
         # wplus = cvx.Variable(n)
         self.w_plus_minus_w_bm.value = np.random.uniform(size=self.N)
         self.w_plus_minus_w_bm.value /= sum(self.w_plus_minus_w_bm.value)
         t = self.returns.index[1]
 
         cost1 = DiagonalCovariance()
-        cost2 = FullCovariance(self.returns.iloc[:, :-1].T @ self.returns.iloc[:, :-1] / len(self.returns))
+        cost2 = FullCovariance(
+            self.returns.iloc[:, :-1].T @ self.returns.iloc[:, :-1] / len(self.returns))
         cost3 = cost1 + cost2
 
-        cost3._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        expr1 = cost1._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        expr2 = cost2._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        cost3._recursive_values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
+        cost3._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
+        expr3 = cost3._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr1 = cost1._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr2 = cost2._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cost3._recursive_values_in_time(
+            t=t, past_returns=self.returns.loc[self.returns.index < t])
         self.assertTrue(expr3.value == expr1.value + expr2.value)
 
         cost4 = cost1 * 2
-        expr4 = cost4._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr4 = cost4._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue(expr4.value == expr1.value * 2)
 
         cost3 = cost1 - cost2
-        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr3 = cost3._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue(expr3.value == expr1.value - expr2.value)
 
         cost3 = -cost1 + 2 * cost2
-        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        self.assertTrue( expr3.value == -expr1.value + 2 * expr2.value)
+        expr3 = cost3._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        self.assertTrue(expr3.value == -expr1.value + 2 * expr2.value)
 
         cost3 = -cost1 + 2 * (cost2 + cost1)
-        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        self.assertTrue( np.isclose(expr3.value, -expr1.value + 2 * (expr2.value + expr1.value)))
+        expr3 = cost3._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        self.assertTrue(np.isclose(expr3.value, -expr1.value +
+                        2 * (expr2.value + expr1.value)))
 
         cost3 = cost1 - 2 * (cost2 + cost1)
-        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        self.assertTrue( expr3.value == expr1.value - 2 * (expr2.value + expr1.value))
-        
+        expr3 = cost3._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        self.assertTrue(expr3.value == expr1.value -
+                        2 * (expr2.value + expr1.value))
+
     def test_hcost(self):
         """Test holding cost model."""
-        dividends = pd.Series(np.random.randn(self.N-1), self.returns.columns[:-1])
+        dividends = pd.Series(np.random.randn(self.N-1),
+                              self.returns.columns[:-1])
         dividends *= 0.
         hcost = StocksHoldingCost(spread_on_borrowing_stocks_percent=.5,
-                            dividends=dividends)
-        
-        t = 100 # this is picked so that periods_per_year evaluates to 252
-        hcost._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expression = hcost._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        hcost._recursive_values_in_time(t=self.returns.index[t], past_returns=self.returns.iloc[:t])
+                                  dividends=dividends)
+
+        t = 100  # this is picked so that periods_per_year evaluates to 252
+        hcost._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
+        expression = hcost._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        hcost._recursive_values_in_time(
+            t=self.returns.index[t], past_returns=self.returns.iloc[:t])
         cash_ret = self.returns.iloc[t-1][-1]
-        
+
         for i in range(10):
             self.w_plus.value = np.random.randn(self.N)
             self.w_plus.value[-1] = 1 - np.sum(self.w_plus.value[:-1])
-        
+
             print(expression.value)
 
-            print( -np.sum(np.minimum(self.w_plus.value[:-1], 0.)) * (cash_ret + .5/(100 * 252)))
-            print( - self.w_plus.value[:-1].T @ dividends)
+            print(-np.sum(np.minimum(self.w_plus.value[:-1], 0.)) * (
+                cash_ret + .5/(100 * 252)))
+            print(- self.w_plus.value[:-1].T @ dividends)
             print(-np.sum(np.minimum(self.w_plus.value[:-1], 0.)) * (cash_ret + 0.5/(100 * 252))
-               - self.w_plus.value[:-1].T @ dividends)
+                  - self.w_plus.value[:-1].T @ dividends)
 
             self.assertTrue(np.isclose(expression.value,
-                -np.sum(np.minimum(self.w_plus.value[:-1], 0.)) * (cash_ret + 0.5/(100 * 252))
-                #+ np.abs(self.w_plus.value[-1])* 0.5/(100 * 252)
-               - self.w_plus.value[:-1].T @ dividends
-            ))
-
+                                       -np.sum(np.minimum(self.w_plus.value[:-1], 0.)) * (cash_ret + 0.5/(100 * 252))
+                                       # + np.abs(self.w_plus.value[-1])* 0.5/(100 * 252)
+                                       - self.w_plus.value[:-1].T @ dividends
+                                       ))
 
     def test_tcost(self):
         """Test tcost model."""
         value = 1e6
-        
-        pershare_cost = pd.Series([0., 0.005, 0.], [self.returns.index[12], self.returns.index[23], self.returns.index[34]])
-        b = pd.Series([0., 0., 1.], [self.returns.index[12], self.returns.index[23], self.returns.index[34]])
-        
+
+        pershare_cost = pd.Series([0., 0.005, 0.], [
+                                  self.returns.index[12], self.returns.index[23], self.returns.index[34]])
+        b = pd.Series([0., 0., 1.], [self.returns.index[12],
+                      self.returns.index[23], self.returns.index[34]])
+
         tcost = StocksTransactionCost(
             a=0.001/2, pershare_cost=pershare_cost, b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
-        
+
         t = self.returns.index[12]
-        
-        tcost._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expression = tcost._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        
+
+        tcost._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
+        expression = tcost._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+
         # only spread
-        
-        tcost._recursive_values_in_time(t=self.returns.index[12], 
-            current_portfolio_value = value,
-            past_returns=self.returns.iloc[:12], 
-            past_volumes=self.volumes.iloc[:12],
-            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
-        
-        
+
+        tcost._recursive_values_in_time(t=self.returns.index[12],
+                                        current_portfolio_value=value,
+                                        past_returns=self.returns.iloc[:12],
+                                        past_volumes=self.volumes.iloc[:12],
+                                        current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
+
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
-        
+
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         print(est_tcost_lin)
         print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
-        
-        
+
         # spread and fixed cost
-        
-        prices = pd.Series(np.random.uniform(1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1])
-        
-        tcost._recursive_values_in_time(t=self.returns.index[23], 
-            current_portfolio_value = value,
-            past_returns=self.returns.iloc[:23], 
-            past_volumes=self.volumes.iloc[:23],
-            current_prices=prices)
-        
-        
+
+        prices = pd.Series(np.random.uniform(
+            1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1])
+
+        tcost._recursive_values_in_time(t=self.returns.index[23],
+                                        current_portfolio_value=value,
+                                        past_returns=self.returns.iloc[:23],
+                                        past_volumes=self.volumes.iloc[:23],
+                                        current_prices=prices)
+
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
-        
+
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         est_tcost_lin += np.abs(self.z.value[:-1]) @ (0.005 / prices)
         print(est_tcost_lin)
         print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
-        
+
         # spread and nonlin cost
-        
-        tcost._recursive_values_in_time(t=self.returns.index[34], 
-            current_portfolio_value = value,
-            past_returns=self.returns.iloc[:34], 
-            past_volumes=self.volumes.iloc[:34],
-            current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
-        
-        
+
+        tcost._recursive_values_in_time(t=self.returns.index[34],
+                                        current_portfolio_value=value,
+                                        past_returns=self.returns.iloc[:34],
+                                        past_volumes=self.volumes.iloc[:34],
+                                        current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
+
         self.z.value = np.random.randn(self.returns.shape[1])
         self.z.value[-1] = -np.sum(self.z.value[:-1])
-        
+
         est_tcost_lin = sum(np.abs(self.z.value[:-1]) * 0.0005)
         volumes_est = self.volumes.iloc[:34].mean().values
         sigmas_est = np.sqrt((self.returns.iloc[:34, :-1]**2).mean()).values
-        est_tcost_nonnlin = (np.abs(self.z.value[:-1])**(3/2)) @ (sigmas_est * np.sqrt(value / volumes_est))
+        est_tcost_nonnlin = (
+            np.abs(self.z.value[:-1])**(3/2)) @ (sigmas_est * np.sqrt(value / volumes_est))
         print(est_tcost_lin)
         print(est_tcost_nonnlin)
         print(expression.value)
-        self.assertTrue(np.isclose(expression.value, est_tcost_lin+est_tcost_nonnlin))
-        
-        
+        self.assertTrue(np.isclose(expression.value,
+                        est_tcost_lin+est_tcost_nonnlin))
+
 
 if __name__ == '__main__':
     unittest.main()
-        
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit tests for the data interfaces."""
 
 import unittest
-import shutil, tempfile
+import shutil
+import tempfile
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.data import (
     YfinanceBase,
@@ -30,150 +31,141 @@
     SqliteDataStore,
     TimeSeries,
     PickleStore,
 )
 
 
 class TestData(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Initialize data directory."""
         cls.datadir = Path(tempfile.mkdtemp())
         print('created', cls.datadir)
-        
+
     @classmethod
     def tearDownClass(cls):
         """Remove data directory."""
         print('removing', cls.datadir)
         shutil.rmtree(cls.datadir)
-        
-        
+
     def test_time_series(self):
         ts = TimeSeries("ZM", base_location=self.datadir)
         assert not hasattr(ts, "data")
         ts._recursive_pre_evaluation()
         assert np.all(
-            ts._recursive_values_in_time(pd.Timestamp("2023-04-11"), "foo", bar=None)
+            ts._recursive_values_in_time(
+                pd.Timestamp("2023-04-11"), "foo", bar=None)
             == ts.data.loc["2023-04-11"]
         )
-        
+
     def test_yfinance_download(self):
         """Test YfinanceBase."""
 
         data = YfinanceBase().download("AAPL", start="2023-04-01", end="2023-04-15")
         print(data)
         print(data.loc["2023-04-10"]["Return"])
-        print(data.loc["2023-04-11", "Open"] / data.loc["2023-04-10", "Open"] - 1)
+        print(data.loc["2023-04-11", "Open"] /
+              data.loc["2023-04-10", "Open"] - 1)
         self.assertTrue(np.isclose(
             data.loc["2023-04-10", "Return"],
-            data.loc["2023-04-11", "Open"] / data.loc["2023-04-10", "Open"] - 1,
+            data.loc["2023-04-11", "Open"] /
+            data.loc["2023-04-10", "Open"] - 1,
         ))
         self.assertTrue(np.isnan(data.iloc[-1]["Close"]))
-    
-    
-    
+
     def test_fred(self):
         store = FredRate(self.datadir)
         data = store.update_and_load("DFF")
         print(data)
         self.assertTrue(np.isclose((1 + data["2023-04-10"]) **
-                          store.trading_days, 1 + 4.83 / 100))
-                          
-                          
+                                   store.trading_days, 1 + 4.83 / 100))
+
     def test_fred_base(self):
         data = FredBase().download("DFF")
         self.assertTrue(data["2023-04-06"] == 4.83)
         self.assertTrue(data.index[0] == pd.Timestamp("1954-07-01"))
         print(data)
         olddata = data.iloc[:-123]
         newdata = FredBase().download("DFF", olddata)
         self.assertTrue(np.all(data == newdata))
-        
 
-        
-        
     def test_yfinance(self):
         """Test yfinance ability to store and retrieve."""
 
         store = Yfinance(self.datadir)
         data = store.update_and_load("ZM")
 
         print(data)
 
         self.assertTrue(np.isclose(
             data.loc["2023-04-05", "Return"],
-            data.loc["2023-04-06", "Open"] / data.loc["2023-04-05", "Open"] - 1,
+            data.loc["2023-04-06", "Open"] /
+            data.loc["2023-04-05", "Open"] - 1,
         ))
 
         data1 = store.update_and_load("ZM")
         print(data1)
 
         self.assertTrue(np.isnan(data1.iloc[-1]["Close"]))
 
         print((data1.iloc[: len(data) - 1].Return -
               data.iloc[:-1].Return).describe().T)
 
         self.assertTrue(np.allclose(
             data1.loc[data.index[:-1]].Return, data.iloc[:-1].Return))
-    
-    
-
 
     def test_sqlite3_store_series(self):
         """Test storing and retrieving of a Series with datetime index."""
         self.base_test_series(SqliteDataStore, self.datadir)
 
     def test_local_store_series(self):
         """Test storing and retrieving of a Series with datetime index."""
         self.base_test_series(LocalDataStore, self.datadir)
-  
+
     def test_pickle_store_series(self):
         """Test storing and retrieving of a Series with datetime index."""
         self.base_test_series(PickleStore, self.datadir)
-  
-    
+
     def test_sqlite3_store_dataframe(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
         self.base_test_dataframe(SqliteDataStore, self.datadir)
 
-
     def test_local_store_dataframe(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
         self.base_test_dataframe(LocalDataStore, self.datadir)
-    
+
     def test_pickle_store_dataframe(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
         self.base_test_dataframe(PickleStore, self.datadir)
-    
 
     def test_local_store_multiindex(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
         self.base_test_multiindex(LocalDataStore, self.datadir)
 
-
     def test_sqlite3_store_multiindex(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
         self.base_test_multiindex(SqliteDataStore, self.datadir)
 
     def test_pickle_store_multiindex(self):
         """Test storing and retrieving of a DataFrame with datetime index."""
-        self.base_test_multiindex(PickleStore, self.datadir)  
+        self.base_test_multiindex(PickleStore, self.datadir)
 
     def base_test_series(self, storeclass, *args, **kwargs):
         """Test storing and retrieving of a Series with datetime index."""
         store = storeclass(*args, **kwargs)
         for data in [
             pd.Series(
                 0.0,
                 pd.date_range(
                     "2020-01-01",
                     "2020-01-10"),
                 name="prova1"),
-            pd.Series(3, pd.date_range("2020-01-01", "2020-01-10"), name="prova2"),
+            pd.Series(3, pd.date_range("2020-01-01",
+                      "2020-01-10"), name="prova2"),
             pd.Series(
                 "ciao", pd.date_range("2020-01-01", "2020-01-02", freq="H"), name="prova3"
             ),
             # test datetime conversion
             pd.Series(
                 pd.date_range("2022-01-01", "2022-01-02", freq="H"),
                 pd.date_range("2020-01-01", "2020-01-02", freq="H"),
@@ -199,16 +191,15 @@
 
             self.assertTrue(data.name == data1.name)
             self.assertTrue(all(data == data1))
             self.assertTrue(all(data.index == data1.index))
             self.assertTrue(data.dtypes == data1.dtypes)
 
         self.assertTrue(store.load("blahblah") is None)
-        
-        
+
     def base_test_dataframe(self, storeclass, *args, **kwargs):
         """Test storing and retrieving of a DataFrame with datetime index."""
         store = storeclass(*args, **kwargs)
         index = pd.date_range("2020-01-01", "2020-01-02", freq="H")
         data = {
             "one": range(len(index)),
             "two": np.arange(len(index)) / 19.0,
@@ -227,15 +218,15 @@
         print(data1)
         print(data1.index.dtype)
         print(data1.dtypes)
 
         self.assertTrue(all(data == data1))
         self.assertTrue(all(data.index == data1.index))
         self.assertTrue(all(data.dtypes == data1.dtypes))
-            
+
     def base_test_multiindex(self, storeclass, *args, **kwargs):
         """Test storing and retrieving of a Series or DataFrame with multi-index."""
         store = storeclass(*args, **kwargs)
 
         # second level is object
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
@@ -300,41 +291,14 @@
 
         print(data1.index)
         print(data1)
         print(data1.index.dtype)
         print(data1.dtypes)
 
         self.assertTrue(all(data == data1))
-        self.assertTrue( all(data.index == data1.index))
-        self.assertTrue( all(data.index.dtypes == data1.index.dtypes))
-        self.assertTrue( all(data.dtypes == data1.dtypes))
-        
-if __name__ == '__main__':
-    unittest.main()
-        
-
-
-
-
-
-
-
-
-
-
-
-                      
-                      
-
-
-
-
-
-
-
-
-
-
-
-
+        self.assertTrue(all(data.index == data1.index))
+        self.assertTrue(all(data.index.dtypes == data1.index.dtypes))
+        self.assertTrue(all(data.dtypes == data1.dtypes))
 
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,162 +14,166 @@
 
 """Unit tests for the data and parameter estimator objects."""
 
 import numpy as np
 import pandas as pd
 import unittest
 
-from cvxportfolio.estimator import DataEstimator #, ParameterEstimator
+from cvxportfolio.estimator import DataEstimator  # , ParameterEstimator
 from cvxportfolio.errors import MissingValuesError, DataError
 
 
 class PlaceholderCallable:
     def __init__(self, value):
         self.value = value
 
     def _recursive_values_in_time(self, t, **kwargs):
         return self.value
 
+
 class TestEstimators(unittest.TestCase):
-        
-        
+
     def test_callable(self):
         estimator = DataEstimator(PlaceholderCallable(1.0))
         time = pd.Timestamp("2022-01-01")
         self.assertEqual(estimator._recursive_values_in_time(time), 1.0)
 
         estimator = DataEstimator(PlaceholderCallable(np.nan))
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time(t=time)
 
         data = np.arange(10.0)
         estimator = DataEstimator(PlaceholderCallable(data))
-        self.assertTrue(np.all(estimator._recursive_values_in_time(t=time) == data))
+        self.assertTrue(
+            np.all(estimator._recursive_values_in_time(t=time) == data))
 
         data[1] = np.nan
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time(time)
 
-
     def test_scalar(self):
         time = pd.Timestamp("2022-01-01")
 
         estimator = DataEstimator(1.0)
         self.assertTrue(estimator._recursive_values_in_time(t=time) == 1.0)
         estimator = DataEstimator(1)
         self.assertTrue(estimator._recursive_values_in_time(t=time) == 1.0)
 
         estimator = DataEstimator(np.nan)
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time(t=time)
 
-
     def test_array(self):
         time = pd.Timestamp("2022-01-01")
         data = np.arange(10.0)
 
         estimator = DataEstimator(data)
-        self.assertTrue(np.all(estimator._recursive_values_in_time(t=time) == data))
+        self.assertTrue(
+            np.all(estimator._recursive_values_in_time(t=time) == data))
 
         data[1] = np.nan
         estimator = DataEstimator(data)
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time(t=time)
 
-
     def test_series_dataframe_notime(self):
         time = pd.Timestamp("2022-01-01")
         data = pd.Series(np.arange(10.0))
         estimator = DataEstimator(data)
-        self.assertTrue(np.all(estimator._recursive_values_in_time(t=time) == data.values))
+        self.assertTrue(
+            np.all(estimator._recursive_values_in_time(t=time) == data.values))
 
         data = pd.DataFrame(np.random.randn(3, 3))
         estimator = DataEstimator(data)
-        self.assertTrue(np.all(estimator._recursive_values_in_time(t=time) == data.values))
-
+        self.assertTrue(
+            np.all(estimator._recursive_values_in_time(t=time) == data.values))
 
     def test_series_timeindex(self):
         index = pd.date_range("2022-01-01", "2022-01-30")
         print(index)
         data = pd.Series(np.arange(len(index)), index)
         estimator = DataEstimator(data)
 
         print(estimator._recursive_values_in_time("2022-01-05"))
-        self.assertTrue(estimator._recursive_values_in_time("2022-01-05") == data.loc["2022-01-05"])
+        self.assertTrue(estimator._recursive_values_in_time(
+            "2022-01-05") == data.loc["2022-01-05"])
 
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2022-02-05")
 
         estimator = DataEstimator(data, use_last_available_time=True)
-        self.assertTrue(estimator._recursive_values_in_time("2022-02-05") == data.iloc[-1])
+        self.assertTrue(estimator._recursive_values_in_time(
+            "2022-02-05") == data.iloc[-1])
 
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2021-02-05")
 
         data["2022-01-05"] = np.nan
         estimator = DataEstimator(data)
-        self.assertTrue(estimator._recursive_values_in_time("2022-01-04") == data.loc["2022-01-04"])
+        self.assertTrue(estimator._recursive_values_in_time(
+            "2022-01-04") == data.loc["2022-01-04"])
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2022-01-05")
 
-
     def test_dataframe_timeindex(self):
         index = pd.date_range("2022-01-01", "2022-01-30")
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         estimator = DataEstimator(data)
 
         print(estimator._recursive_values_in_time("2022-01-05"))
         self.assertTrue(np.all(estimator._recursive_values_in_time(
             "2022-01-05") == data.loc["2022-01-05"]))
 
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2021-01-05")
 
         estimator = DataEstimator(data, use_last_available_time=True)
-        self.assertTrue(np.all(estimator._recursive_values_in_time("2022-02-05") == data.iloc[-1]))
+        self.assertTrue(
+            np.all(estimator._recursive_values_in_time("2022-02-05") == data.iloc[-1]))
 
         data.loc["2022-01-05", 3] = np.nan
         estimator = DataEstimator(data, use_last_available_time=True)
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2021-01-05")
 
-
     def test_dataframe_multindex(self):
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         print(data.index)
         estimator = DataEstimator(data)
-        self.assertTrue( np.all(estimator._recursive_values_in_time(
+        self.assertTrue(np.all(estimator._recursive_values_in_time(
             "2022-01-05") == data.loc["2022-01-05"]))
 
         estimator = DataEstimator(data, use_last_available_time=True)
-        self.assertTrue( np.all(estimator._recursive_values_in_time(
+        self.assertTrue(np.all(estimator._recursive_values_in_time(
             "2022-02-05") == data.loc["2022-01-30"]))
-        self.assertTrue( np.all(estimator._recursive_values_in_time(
+        self.assertTrue(np.all(estimator._recursive_values_in_time(
             "2022-01-05") == data.loc["2022-01-05"]))
         with self.assertRaises(MissingValuesError):
             estimator._recursive_values_in_time("2020-01-05")
 
         index = pd.MultiIndex.from_product([second_level, timeindex])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         estimator = DataEstimator(data)
-        assert np.all(estimator._recursive_values_in_time("2020-01-05") == data.values)
-
+        assert np.all(estimator._recursive_values_in_time(
+            "2020-01-05") == data.values)
 
     def test_parameter_estimator(self):
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
         estimator = DataEstimator(data, compile_parameter=True)
-        self.assertTrue( not hasattr(estimator, "parameter"))
-        estimator._recursive_pre_evaluation(universe=None, backtest_times=timeindex)
+        self.assertTrue(not hasattr(estimator, "parameter"))
+        estimator._recursive_pre_evaluation(
+            universe=None, backtest_times=timeindex)
         # assert hasattr(estimator, 'parameter')
-        self.assertTrue( hasattr(estimator, "parameter"))
+        self.assertTrue(hasattr(estimator, "parameter"))
         estimator._recursive_values_in_time("2022-01-05")
-        self.assertTrue( np.all(estimator.parameter.value == data.loc["2022-01-05"]))
-        
+        self.assertTrue(
+            np.all(estimator.parameter.value == data.loc["2022-01-05"]))
+
+
 if __name__ == '__main__':
     unittest.main()
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_forecast.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,190 +21,197 @@
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 
 
 from cvxportfolio.forecast import HistoricalMeanReturn, HistoricalMeanError, HistoricalVariance, HistoricalFactorizedCovariance
 
+
 class TestEstimators(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-    
+
     # def boilerplate(self, model):
     #     model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
     #     return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-         
-    
+
     def test_mean_update(self):
-        forecaster = HistoricalMeanReturn()#lastforcash=True)
-        
+        forecaster = HistoricalMeanReturn()  # lastforcash=True)
+
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
-        
-        for tidx in [50,51,52,55,56,57]:
+
+        for tidx in [50, 51, 52, 55, 56, 57]:
             t = returns.index[tidx]
-            past_returns = returns.loc[returns.index<t]
-            mean = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
+            past_returns = returns.loc[returns.index < t]
+            mean = forecaster._recursive_values_in_time(
+                t=t, past_returns=past_returns)
             # print(mean)
             # self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
-            self.assertTrue(np.allclose(mean, past_returns.iloc[:,:-1].mean()))
-        
-    
+            self.assertTrue(np.allclose(
+                mean, past_returns.iloc[:, :-1].mean()))
+
     def test_variance_update(self):
         forecaster = HistoricalVariance(kelly=False)
-        
+
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
-        
-        for tidx in [50,51,52,55,56,57]:
+
+        for tidx in [50, 51, 52, 55, 56, 57]:
             t = returns.index[tidx]
-            past_returns = returns.loc[returns.index<t]
-            var = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
+            past_returns = returns.loc[returns.index < t]
+            var = forecaster._recursive_values_in_time(
+                t=t, past_returns=past_returns)
             print(var)
-            #self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
-            self.assertTrue(np.allclose(var, past_returns.var(ddof=0)[:-1]))    
-            
+            # self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
+            self.assertTrue(np.allclose(var, past_returns.var(ddof=0)[:-1]))
+
     def test_meanerror_update(self):
         forecaster = HistoricalMeanError()
-        
+
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
-        
-        for tidx in [50,51,52,55,56,57]:
+
+        for tidx in [50, 51, 52, 55, 56, 57]:
             t = returns.index[tidx]
-            past_returns = returns.loc[returns.index<t]
-            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
+            past_returns = returns.loc[returns.index < t]
+            val = forecaster._recursive_values_in_time(
+                t=t, past_returns=past_returns)
             print(val)
-            #self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
-            self.assertTrue(np.allclose(val, past_returns.std(ddof=0)[:-1] / np.sqrt(past_returns.count()[:-1]) ))  
-            
+            # self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
+            self.assertTrue(np.allclose(val, past_returns.std(ddof=0)[
+                            :-1] / np.sqrt(past_returns.count()[:-1])))
+
     def test_counts_matrix(self):
-        forecaster = HistoricalFactorizedCovariance()#kelly=True)
+        forecaster = HistoricalFactorizedCovariance()  # kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
-        
+
         count_matrix = forecaster._get_count_matrix(returns)
-        
-        for indexes in [(1,2), (4,5), (1,5), (7, 18), (7,24), (1,15), (13,22)]:
+
+        for indexes in [(1, 2), (4, 5), (1, 5), (7, 18), (7, 24), (1, 15), (13, 22)]:
             print(count_matrix.iloc[indexes[0], indexes[1]])
-            print(len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna()))
+            print(len((returns.iloc[:, indexes[0]] *
+                  returns.iloc[:, indexes[1]]).dropna()))
             self.assertTrue(np.isclose(count_matrix.iloc[indexes[0], indexes[1]],
-                len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna())))
-                
+                                       len((returns.iloc[:, indexes[0]] * returns.iloc[:, indexes[1]]).dropna())))
+
     def test_sum_matrix(self):
-        forecaster = HistoricalFactorizedCovariance()#kelly=True)
+        forecaster = HistoricalFactorizedCovariance()  # kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
-        
-        forecaster._recursive_values_in_time(t=pd.Timestamp('2022-01-01'), past_returns=returns)
-         
+
+        forecaster._recursive_values_in_time(
+            t=pd.Timestamp('2022-01-01'), past_returns=returns)
+
         sum_matrix = forecaster.last_sum_matrix
-        
-        for indexes in [(1,2), (4,5), (1,5), (7, 18), (7,24), (1,15), (13,22)]:
+
+        for indexes in [(1, 2), (4, 5), (1, 5), (7, 18), (7, 24), (1, 15), (13, 22)]:
             print()
             print(sum_matrix[indexes[0], indexes[1]])
-            print( (returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).sum())
+            print((returns.iloc[:, indexes[0]] *
+                  returns.iloc[:, indexes[1]]).sum())
             self.assertTrue(np.isclose(
                 sum_matrix[indexes[0], indexes[1]],
-                (returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).sum()
-                ))
-        
+                (returns.iloc[:, indexes[0]] *
+                 returns.iloc[:, indexes[1]]).sum()
+            ))
+
     def test_covariance_update(self):
         """Test covariance forecast estimator."""
-        
+
         forecaster = HistoricalFactorizedCovariance()
-        
+
         returns = pd.DataFrame(self.returns.iloc[:, :4], copy=True)
         returns.iloc[:20, 1] = np.nan
         returns.iloc[10:30, 0] = np.nan
         returns.iloc[25:40, 2] = np.nan
-        
+
         def compute_Sigma(rets):
-            res = np.zeros((3,3))
-            res[0,0] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 0])
-            res[1,1] = np.nanmean(rets.iloc[:, 1] * rets.iloc[:, 1])
-            res[2,2] = np.nanmean(rets.iloc[:, 2] * rets.iloc[:, 2])
-            res[0,1] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 1])
-            res[0,2] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 2])
-            res[1,2] = np.nanmean(rets.iloc[:, 1] * rets.iloc[:, 2])
-            res[1,0] = res[0,1]
-            res[2,0] = res[0,2]
-            res[2,1] = res[1,2]
+            res = np.zeros((3, 3))
+            res[0, 0] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 0])
+            res[1, 1] = np.nanmean(rets.iloc[:, 1] * rets.iloc[:, 1])
+            res[2, 2] = np.nanmean(rets.iloc[:, 2] * rets.iloc[:, 2])
+            res[0, 1] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 1])
+            res[0, 2] = np.nanmean(rets.iloc[:, 0] * rets.iloc[:, 2])
+            res[1, 2] = np.nanmean(rets.iloc[:, 1] * rets.iloc[:, 2])
+            res[1, 0] = res[0, 1]
+            res[2, 0] = res[0, 2]
+            res[2, 1] = res[1, 2]
             return res
-        
-        for tidx in [50,51,52,55,56,57]:
+
+        for tidx in [50, 51, 52, 55, 56, 57]:
             t = returns.index[tidx]
-            past_returns = returns.loc[returns.index<t]
-            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
+            past_returns = returns.loc[returns.index < t]
+            val = forecaster._recursive_values_in_time(
+                t=t, past_returns=past_returns)
             Sigma = val @ val.T
             self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
 
     def test_covariance_update_nokelly(self):
         """Test covariance forecast estimator.
-        
+
         NOTE: due to a bug in pandas we can't test against pandas.DataFrame.cov, 
         see https://github.com/pandas-dev/pandas/issues/45814 . In fact with the
         current bug in pandas 
         ``past_returns.iloc[:,:-1].cov(ddof=0)`` returns ``past_returns.iloc[:,:-1].cov(ddof=1)``
         whenever there are missing values.
         """
-        
+
         forecaster = HistoricalFactorizedCovariance(kelly=False)
-        
+
         returns = pd.DataFrame(self.returns.iloc[:, :4], copy=True)
         returns.iloc[:20, 1] = np.nan
         returns.iloc[10:30, 0] = np.nan
         returns.iloc[25:40, 2] = np.nan
-        
+
         def cov_ij(i, j, rets):
             i_nanmasker = np.zeros(len(rets))
             i_nanmasker[rets.iloc[:, i].isnull()] = np.nan
             i_nanmasker[~(rets.iloc[:, i].isnull())] = 1.
             j_nanmasker = np.zeros(len(rets))
             j_nanmasker[rets.iloc[:, j].isnull()] = np.nan
             j_nanmasker[~(rets.iloc[:, j].isnull())] = 1.
             print(i_nanmasker, j_nanmasker)
             return np.nanmean(rets.iloc[:, i] * rets.iloc[:, j]) - np.nanmean(rets.iloc[:, i] * j_nanmasker) * np.nanmean(rets.iloc[:, j] * i_nanmasker)
-        
+
         def compute_Sigma(rets):
-            res = np.zeros((3,3))
-            res[0,0] = cov_ij(0,0, rets)
-            res[1,1] = cov_ij(1,1, rets)
-            res[2,2] = cov_ij(2,2, rets)
-            res[0,1] = cov_ij(0,1, rets)
-            res[0,2] = cov_ij(0,2, rets)
-            res[1,2] = cov_ij(1,2, rets)
-            res[1,0] = res[0,1]
-            res[2,0] = res[0,2]
-            res[2,1] = res[1,2]
+            res = np.zeros((3, 3))
+            res[0, 0] = cov_ij(0, 0, rets)
+            res[1, 1] = cov_ij(1, 1, rets)
+            res[2, 2] = cov_ij(2, 2, rets)
+            res[0, 1] = cov_ij(0, 1, rets)
+            res[0, 2] = cov_ij(0, 2, rets)
+            res[1, 2] = cov_ij(1, 2, rets)
+            res[1, 0] = res[0, 1]
+            res[2, 0] = res[0, 2]
+            res[2, 1] = res[1, 2]
             return res
-        
-        
-        for tidx in [50,51,52,55,56,57]:
+
+        for tidx in [50, 51, 52, 55, 56, 57]:
             t = returns.index[tidx]
-            past_returns = returns.loc[returns.index<t]
-            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
+            past_returns = returns.loc[returns.index < t]
+            val = forecaster._recursive_values_in_time(
+                t=t, past_returns=past_returns)
             Sigma = val @ val.T
 
             self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
             # pandasSigma = past_returns.iloc[:,:-1].cov(ddof=0)
             # self.assertTrue(np.allclose(Sigma, pandasSigma))
-            self.assertTrue(np.allclose(np.diag(Sigma), past_returns.iloc[:,:-1].var(ddof=0)))
+            self.assertTrue(np.allclose(
+                np.diag(Sigma), past_returns.iloc[:, :-1].var(ddof=0)))
+
 
-            
-        
-        
-    
 if __name__ == '__main__':
     unittest.main()
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_policies.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,33 +28,34 @@
 from cvxportfolio.risks import *
 from cvxportfolio.costs import *
 from cvxportfolio.constraints import *
 from cvxportfolio.errors import *
 
 
 class TestPolicies(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
-        cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.volumes = pd.read_csv(
+            Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
 
     def test_hold(self):
         hold = Hold()
         w = pd.Series(0.5, ["AAPL", "CASH"])
         self.assertTrue(np.all(
             hold._recursive_values_in_time(current_weights=w).values == np.zeros(2)))
-            
-            
+
     def test_rank_and_long_short(self):
         hold = Hold()
         w = pd.Series(0.25, ["AAPL", "TSLA", "GOOGL", "CASH"])
         signal = pd.Series([1, 2, 3], ["AAPL", "TSLA", "GOOGL"])
         num_long = 1
         num_short = 1
         target_leverage = 3.0
@@ -64,17 +65,17 @@
             num_short=num_short,
             target_leverage=target_leverage,
         )
         z = rls._recursive_values_in_time(t=None, current_weights=w)
         print(z)
         wplus = w + z
         self.assertTrue(wplus["CASH"] == 1)
-        self.assertTrue( wplus["TSLA"] == 0)
-        self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
-        self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
+        self.assertTrue(wplus["TSLA"] == 0)
+        self.assertTrue(wplus["AAPL"] == -wplus["GOOGL"])
+        self.assertTrue(np.abs(wplus[:-1]).sum() == 3)
 
         index = pd.date_range("2020-01-01", "2020-01-03")
         signal = pd.DataFrame(
             {
                 "AAPL": pd.Series([1, 1.9, 3], index),
                 "TSLA": pd.Series([3, 2.1, 1], index),
                 "GOOGL": pd.Series([4, 4, 4], index),
@@ -85,78 +86,79 @@
             num_long=num_long,
             num_short=num_short,
             target_leverage=target_leverage,
         )
         z1 = rls._recursive_values_in_time(t=index[0], current_weights=w)
         print(z1)
         wplus = w + z1
-        self.assertTrue( wplus["CASH"] == 1)
-        self.assertTrue( wplus["TSLA"] == 0)
-        self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
-        self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
+        self.assertTrue(wplus["CASH"] == 1)
+        self.assertTrue(wplus["TSLA"] == 0)
+        self.assertTrue(wplus["AAPL"] == -wplus["GOOGL"])
+        self.assertTrue(np.abs(wplus[:-1]).sum() == 3)
         z2 = rls._recursive_values_in_time(t=index[1], current_weights=w)
         print(z2)
         wplus = w + z2
-        self.assertTrue( wplus["CASH"] == 1)
-        self.assertTrue( wplus["TSLA"] == 0)
-        self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
-        self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
+        self.assertTrue(wplus["CASH"] == 1)
+        self.assertTrue(wplus["TSLA"] == 0)
+        self.assertTrue(wplus["AAPL"] == -wplus["GOOGL"])
+        self.assertTrue(np.abs(wplus[:-1]).sum() == 3)
         z3 = rls._recursive_values_in_time(t=index[2], current_weights=w)
         wplus = w + z3
-        self.assertTrue( wplus["CASH"] == 1)
-        self.assertTrue( wplus["AAPL"] == 0)
-        self.assertTrue( wplus["TSLA"] == -wplus["GOOGL"])
-        self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
+        self.assertTrue(wplus["CASH"] == 1)
+        self.assertTrue(wplus["AAPL"] == 0)
+        self.assertTrue(wplus["TSLA"] == -wplus["GOOGL"])
+        self.assertTrue(np.abs(wplus[:-1]).sum() == 3)
         print(z3)
 
-
     def test_proportional_trade(self):
-    
+
         a = pd.Series(1., self.returns.columns)
         a[-1] = 1 - sum(a[:-1])
         b = pd.Series(-1., self.returns.columns)
         b[-1] = 1 - sum(b[:-1])
 
         targets = pd.DataFrame({self.returns.index[3]: a,
                                 self.returns.index[15]: b
                                 }).T
         policy = ProportionalTradeToTargets(targets)
 
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
             self.returns.columns)
         start_portfolio[-1] = 1 - sum(start_portfolio[:-1])
         for t in self.returns.index[:17]:
             print(t)
             print(start_portfolio)
-        
-            trade = policy._recursive_values_in_time(t=t, current_weights=start_portfolio)
+
+            trade = policy._recursive_values_in_time(
+                t=t, current_weights=start_portfolio)
             start_portfolio += trade
-        
+
             if t in targets.index:
                 self.assertTrue(np.all(start_portfolio == targets.loc[t]))
 
-        self.assertTrue( np.all(trade == 0.))
-        
+        self.assertTrue(np.all(trade == 0.))
+
     def test_sell_all(self):
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
             self.returns.columns)
         policy = SellAll()
         t = pd.Timestamp('2022-01-01')
-        trade = policy._recursive_values_in_time(t=t, current_weights=start_portfolio)
+        trade = policy._recursive_values_in_time(
+            t=t, current_weights=start_portfolio)
         allcash = np.zeros(len(start_portfolio))
         allcash[-1] = 1
         assert isinstance(trade, pd.Series)
         assert np.allclose(allcash, start_portfolio + trade)
 
-
     def test_fixed_trade(self):
         fixed_trades = pd.DataFrame(
             np.random.randn(
                 len(self.returns),
                 self.returns.shape[1]),
             index=self.returns.index,
             columns=self.returns.columns)
@@ -167,15 +169,14 @@
             0., self.returns.columns))
         self.assertTrue(np.all(trade == fixed_trades.loc[t]))
 
         t = pd.Timestamp('1900-01-01')
         trade = policy._recursive_values_in_time(t=t, current_weights=trade)
         self.assertTrue(np.all(trade == 0.))
 
-
     def test_fixed_weights(self):
         fixed_weights = pd.DataFrame(
             np.random.randn(
                 len(self.returns),
                 self.returns.shape[1]),
             index=self.returns.index,
             columns=self.returns.columns)
@@ -183,166 +184,177 @@
         policy = FixedWeights(fixed_weights)
         t = self.returns.index[123]
         trade = policy._recursive_values_in_time(t=t, current_weights=pd.Series(
             0., self.returns.columns))
         self.assertTrue(np.all(trade == fixed_weights.loc[t]))
 
         t = self.returns.index[111]
-        trade = policy._recursive_values_in_time(t=t, current_weights=fixed_weights.iloc[110])
-        self.assertTrue( np.allclose(trade + fixed_weights.iloc[110], fixed_weights.loc[t]))
+        trade = policy._recursive_values_in_time(
+            t=t, current_weights=fixed_weights.iloc[110])
+        self.assertTrue(np.allclose(
+            trade + fixed_weights.iloc[110], fixed_weights.loc[t]))
 
         t = pd.Timestamp('1900-01-01')
         trade = policy._recursive_values_in_time(t=t, current_weights=trade)
-        self.assertTrue( np.all(trade == 0.))
-
+        self.assertTrue(np.all(trade == 0.))
 
     def test_periodic_rebalance(self):
 
-        target = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
+        target = pd.Series(np.random.uniform(
+            size=self.returns.shape[1]), self.returns.columns)
         target /= sum(target)
-        rebalancing_times = pd.date_range(start=self.returns.index[0], end=self.returns.index[-1], 
-            freq='7d')
+        rebalancing_times = pd.date_range(start=self.returns.index[0], end=self.returns.index[-1],
+                                          freq='7d')
 
         policy = PeriodicRebalance(target, rebalancing_times=rebalancing_times)
-        init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
+        init = pd.Series(np.random.randn(
+            self.returns.shape[1]), self.returns.columns)
 
-        trade = policy._recursive_values_in_time(t=rebalancing_times[0], current_weights=init)
+        trade = policy._recursive_values_in_time(
+            t=rebalancing_times[0], current_weights=init)
         self.assertTrue(np.allclose(trade + init, target))
 
         trade = policy._recursive_values_in_time(t=rebalancing_times[0] + pd.Timedelta('1d'),
-            current_weights=init)
+                                                 current_weights=init)
         self.assertTrue(np.allclose(trade, 0))
 
     def test_uniform(self):
         pol = Uniform()
         pol._recursive_pre_evaluation(self.returns.columns, self.returns.index)
-        
-        init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
-        trade = pol._recursive_values_in_time(t=self.returns.index[123], current_weights=init)
-        self.assertTrue(np.allclose((trade + init)[:-1], 
-            np.ones(self.returns.shape[1]-1)/(self.returns.shape[1]-1)))
-        
+
+        init = pd.Series(np.random.randn(
+            self.returns.shape[1]), self.returns.columns)
+        trade = pol._recursive_values_in_time(
+            t=self.returns.index[123], current_weights=init)
+        self.assertTrue(np.allclose((trade + init)[:-1],
+                                    np.ones(self.returns.shape[1]-1)/(self.returns.shape[1]-1)))
 
     def test_proportional_rebalance(self):
 
-        target = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
+        target = pd.Series(np.random.uniform(
+            size=self.returns.shape[1]), self.returns.columns)
         target /= sum(target)
         target_matching_times = self.returns.index[::3]
 
-        policy = ProportionalRebalance(target, target_matching_times=target_matching_times)
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy = ProportionalRebalance(
+            target, target_matching_times=target_matching_times)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
 
-        init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
+        init = pd.Series(np.random.randn(
+            self.returns.shape[1]), self.returns.columns)
 
-        trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
+        trade = policy._recursive_values_in_time(
+            t=self.returns.index[1], current_weights=init)
         init += trade
-        trade2 = policy._recursive_values_in_time(t=self.returns.index[2], current_weights=init)
+        trade2 = policy._recursive_values_in_time(
+            t=self.returns.index[2], current_weights=init)
         self.assertTrue(np.allclose(trade, trade2))
         self.assertTrue(np.allclose(trade + trade2 + init, target))
-    
+
     def test_adaptive_rebalance(self):
         np.random.seed(0)
         target = pd.Series(
             np.random.uniform(
                 size=self.returns.shape[1]),
             self.returns.columns)
         target /= sum(target)
         target = pd.DataFrame({ind: target for ind in self.returns.index}).T
 
-        init = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
+        init = pd.Series(np.random.uniform(
+            size=self.returns.shape[1]), self.returns.columns)
         init /= sum(init)
 
         for tracking_error in [0.01, .02, .05, .1]:
             policy = AdaptiveRebalance(target, tracking_error=tracking_error)
-            trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
+            trade = policy._recursive_values_in_time(
+                t=self.returns.index[1], current_weights=init)
             self.assertTrue(np.allclose(init + trade, target.iloc[0]))
 
         for tracking_error in [.2, .5]:
             policy = AdaptiveRebalance(target, tracking_error=tracking_error)
-            trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
+            trade = policy._recursive_values_in_time(
+                t=self.returns.index[1], current_weights=init)
             self.assertTrue(np.allclose(trade, 0.))
 
-
     def test_single_period_optimization(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance(kelly=False)
         tcost = TransactionCost(a=1E-3/2, pershare_cost=0., b=None, exponent=2)
-        
+
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
-            -tcost
-            #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
-            ,
+            # - TcostModel(half_spread=5 * 1E-4)  # , power=2)
+            - tcost,
             constraints=[LongOnly(), LeverageLimit(1)],
             include_cash_return=False,
             # verbose=True,
             solver='ECOS')
-            
 
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         policy._compile_to_cvxpy()
-        
+
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         result = policy._recursive_values_in_time(
             t=self.returns.index[121],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:121],
             past_volumes=self.volumes.iloc[:121],
             current_prices=pd.Series(1., self.volumes.columns))
-            
-       
 
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
         print(cvxportfolio_result)
-        
+
         # print(np.linalg.eigh(self.returns.iloc[:121, :-1].cov().values)[0])
 
         # REPLICATE WITH CVXPY
-        
-        COV = self.returns.iloc[:121, :-1].cov(ddof=0).values #+ np.outer(self.returns.iloc[:121, :-1].mean(), self.returns.iloc[:121, :-1].mean())
+
+        # + np.outer(self.returns.iloc[:121, :-1].mean(), self.returns.iloc[:121, :-1].mean())
+        COV = self.returns.iloc[:121, :-1].cov(ddof=0).values
         w = cp.Variable(self.N)
         cp.Problem(cp.Maximize(w[:-1].T @ self.returns.iloc[:121, :-1].mean().values -
-                                 2 * cp.quad_form(w[:-1], COV) -
-                                 5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])
-                                 ),
-                    [w >= 0, w <= 1, sum(w) == 1]
-                    ).solve(solver='ECOS')
+                               2 * cp.quad_form(w[:-1], COV) -
+                               5 * 1E-4 * cp.sum(cp.abs(w - curw)[:-1])
+                               ),
+                   [w >= 0, w <= 1, sum(w) == 1]
+                   ).solve(solver='ECOS')
 
         cvxpy_result = pd.Series(w.value - curw, self.returns.columns)
 
         print(cvxpy_result)
-        
+
         print(cvxportfolio_result - cvxpy_result)
-        self.assertTrue(np.allclose(cvxportfolio_result - cvxpy_result, 0., atol=1e-5))
-    
-    
-    
+        self.assertTrue(np.allclose(
+            cvxportfolio_result - cvxpy_result, 0., atol=1e-5))
+
     def test_single_period_optimization_solve_twice(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
-        
+
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
             - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1)],
             # verbose=True,
             solver='ECOS')
 
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         policy._compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         result = policy._recursive_values_in_time(
             t=self.returns.index[134],
@@ -367,100 +379,97 @@
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:134],
             past_volumes=self.volumes.iloc[:134],
             current_prices=pd.Series(1., self.volumes.columns))
 
         self.assertTrue(np.allclose(result2, 0., atol=1e-7))
-        
-        
+
     def test_single_period_optimization_infeasible(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
         policy = SinglePeriodOptimization(
             return_forecast
             - 2 * risk_forecast
             - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1), MaxWeights(-1)],
             # verbose=True,
             solver='ECOS')
 
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         policy._compile_to_cvxpy()
 
-
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
             result = policy._recursive_values_in_time(
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
                 current_prices=pd.Series(1., self.volumes.columns))
-            
+
     def test_single_period_optimization_unbounded(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance()
         policy = SinglePeriodOptimization(
-            return_forecast
-            #- 2 * risk_forecast
-            #- TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
+            return_forecast            # - 2 * risk_forecast
+            # - TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
-            constraints=[LongOnly(), #LeverageLimit(1), MaxWeights(-1)
-        ],
+            constraints=[LongOnly(),  # LeverageLimit(1), MaxWeights(-1)
+                         ],
             # verbose=True,
             solver='ECOS')
 
-        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         policy._compile_to_cvxpy()
 
-
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
             result = policy._recursive_values_in_time(
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
                 current_prices=pd.Series(1., self.volumes.columns))
-     
+
     def test_multi_period_optimization2(self):
         """Test that MPO1 and MPO2 and MPO5 return same if no tcost, and diff if tcost"""
 
         results = []
-        for planning_horizon in [1,2,5]:
+        for planning_horizon in [1, 2, 5]:
             return_forecast = ReturnsForecast()
             risk_forecast = FullCovariance()
             policy = MultiPeriodOptimization(
                 return_forecast
-                - 10 * risk_forecast
-                #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
-                ,
+                # - TcostModel(half_spread=5 * 1E-4)  # , power=2)
+                - 10 * risk_forecast,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._recursive_pre_evaluation(
+                universe=self.returns.columns, backtest_times=self.returns.index)
             policy._compile_to_cvxpy()
 
-
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             results.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
@@ -472,31 +481,31 @@
 
         self.assertTrue(np.allclose(results[0], results[1], atol=1e-4))
         self.assertTrue(np.allclose(results[1], results[2], atol=1e-4))
 
         # with tcost
 
         results = []
-        for planning_horizon in [1,2,5]:
+        for planning_horizon in [1, 2, 5]:
             return_forecast = ReturnsForecast()
             risk_forecast = FullCovariance()
             policy = MultiPeriodOptimization(
                 return_forecast
                 - 10 * risk_forecast
-                - TransactionCost(a=25 * 1E-4, pershare_cost=0., b=0.)
-                #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
-                ,
+                # - TcostModel(half_spread=5 * 1E-4)  # , power=2)
+                - TransactionCost(a=25 * 1E-4, pershare_cost=0., b=0.),
                 constraints=[LongOnly(), LeverageLimit(1)],
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._recursive_pre_evaluation(
+                universe=self.returns.columns, backtest_times=self.returns.index)
             policy._compile_to_cvxpy()
-            
+
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             results.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
@@ -504,70 +513,69 @@
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
                 current_prices=pd.Series(1., self.volumes.columns)))
 
         self.assertFalse(np.allclose(results[0], results[1], atol=1e-4))
         self.assertFalse(np.allclose(results[1], results[2], atol=1e-4))
-        
+
     def test_multi_period_optimization_syntax(self):
         with self.assertRaises(SyntaxError):
             MultiPeriodOptimization([ReturnsForecast()], [])
         with self.assertRaises(SyntaxError):
-            MultiPeriodOptimization([ReturnsForecast()], [[],[]])
+            MultiPeriodOptimization([ReturnsForecast()], [[], []])
         with self.assertRaises(SyntaxError):
             MultiPeriodOptimization([ReturnsForecast()], None)
         with self.assertRaises(SyntaxError):
             MultiPeriodOptimization(ReturnsForecast())
-        MultiPeriodOptimization(ReturnsForecast(), planning_horizon = 1)
-        
+        MultiPeriodOptimization(ReturnsForecast(), planning_horizon=1)
+
     def test_multi_period_optimization3(self):
         """Check that terminal constraint brings closer to benchmark."""
-    
+
         np.random.seed(0)
         benchmark = np.random.uniform(size=self.returns.shape[1])
         benchmark /= sum(benchmark)
         benchmark = pd.Series(benchmark, self.returns.columns)
-    
+
         diff_to_benchmarks = []
-        for planning_horizon in [1,2,5]:
+        for planning_horizon in [1, 2, 5]:
 
             return_forecast = ReturnsForecast()
             risk_forecast = FullCovariance()
             policy = MultiPeriodOptimization(
                 return_forecast
                 - 10 * risk_forecast
-                - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
-                ,
+                # , power=2)
+                - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.),
                 constraints=[LongOnly(), LeverageLimit(1)],
-                #verbose=True,
+                # verbose=True,
                 terminal_constraint=benchmark,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._recursive_pre_evaluation(
+                universe=self.returns.columns, backtest_times=self.returns.index)
             policy._compile_to_cvxpy()
-            
+
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
             diff_to_benchmarks.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
                 current_prices=pd.Series(1., self.volumes.columns)) + curw - benchmark)
-                                        
+
         self.assertTrue(np.isclose(np.linalg.norm(diff_to_benchmarks[0]), 0.))
-        self.assertTrue(np.linalg.norm(diff_to_benchmarks[0]) < np.linalg.norm(diff_to_benchmarks[1]))
-        self.assertTrue(np.linalg.norm(diff_to_benchmarks[1]) < np.linalg.norm(diff_to_benchmarks[2]))
-    
-    
+        self.assertTrue(np.linalg.norm(
+            diff_to_benchmarks[0]) < np.linalg.norm(diff_to_benchmarks[1]))
+        self.assertTrue(np.linalg.norm(
+            diff_to_benchmarks[1]) < np.linalg.norm(diff_to_benchmarks[2]))
+
+
 if __name__ == '__main__':
     unittest.main()
-        
-    
-    
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_returns.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,102 +19,110 @@
 
 import cvxpy as cp
 import numpy as np
 import pandas as pd
 import numpy as np
 
 
-
 from cvxportfolio.returns import *
 
+
 class TestReturns(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-        
+
     def boilerplate(self, model):
         """Initialize objects, compile cvxpy expression."""
-        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        model._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        
-        
+
     def test_cash_returns(self):
         "Test CashReturn object with last return as forecast."
         cash_model = CashReturn()
         cvxpy_expression = self.boilerplate(cash_model)
         self.w_plus.value = np.random.randn(self.N)
-        cash_model._recursive_values_in_time(t=None, past_returns=self.returns.iloc[:123])
+        cash_model._recursive_values_in_time(
+            t=None, past_returns=self.returns.iloc[:123])
         cr = self.returns.iloc[122, -1]
-        self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
-        
+        self.assertTrue(cvxpy_expression.value == cr * (
+            self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
+
     def test_cash_returns_provided(self):
         "Test CashReturn object with provided cash returns."
-        cash_model = CashReturn(self.returns.iloc[:,-1])
+        cash_model = CashReturn(self.returns.iloc[:, -1])
         cvxpy_expression = self.boilerplate(cash_model)
         self.w_plus.value = np.random.randn(self.N)
-        cash_model._recursive_values_in_time(t=self.returns.index[123], past_returns=None)
+        cash_model._recursive_values_in_time(
+            t=self.returns.index[123], past_returns=None)
         cr = self.returns.iloc[123, -1]
-        self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
-        
+        self.assertTrue(cvxpy_expression.value == cr * (
+            self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
+
     def test_returns_forecast(self):
         "Test ReturnsForecast object with provided assets' returns."
-        alpha_model = ReturnsForecast(self.returns.iloc[:,:-1])
+        alpha_model = ReturnsForecast(self.returns.iloc[:, :-1])
         cvxpy_expression = self.boilerplate(alpha_model)
-        alpha_model._recursive_values_in_time(t=self.returns.index[123], past_returns=None)
+        alpha_model._recursive_values_in_time(
+            t=self.returns.index[123], past_returns=None)
         self.w_plus.value = np.random.randn(self.N)
         print(cvxpy_expression.value)
-        print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1]) 
-        #+ ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1]))
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus[:-1].value @ self.returns.iloc[123][:-1]))
-                #+ ((self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1])))
-        
-        
+        print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1])
+        # + ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1]))
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+                        self.w_plus[:-1].value @ self.returns.iloc[123][:-1]))
+        # + ((self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1])))
+
     def test_full_returns_forecast(self):
         "Test ReturnsForecast object with historical mean forecasts."
         alpha_model = ReturnsForecast()
         cvxpy_expression = self.boilerplate(alpha_model)
         t = self.returns.index[123]
-        alpha_model._recursive_values_in_time(t=t, past_returns = self.returns.loc[self.returns.index<t])
+        alpha_model._recursive_values_in_time(
+            t=t, past_returns=self.returns.loc[self.returns.index < t])
         self.w_plus.value = np.random.uniform(size=self.N)
         self.w_plus.value /= sum(self.w_plus.value)
-        myforecast = self.returns.iloc[:, :-1].loc[self.returns.index < t].mean()
+        myforecast = self.returns.iloc[:, :-
+                                       1].loc[self.returns.index < t].mean()
         # myforecast.iloc[-1] = self.returns.iloc[122, -1]
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus.value[:-1] @ myforecast))
-        
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+                        self.w_plus.value[:-1] @ myforecast))
+
     def test_returns_forecast_error(self):
         "Test ReturnsForecastError object with provided values."
-        delta = self.returns.iloc[:, :-1].std(ddof=0) / np.sqrt(len(self.returns))
+        delta = self.returns.iloc[:, :-
+                                  1].std(ddof=0) / np.sqrt(len(self.returns))
         # delta.iloc[-1] = 0
         error_risk = ReturnsForecastError(delta)
         cvxpy_expression = self.boilerplate(error_risk)
         error_risk._recursive_values_in_time(t='ciao', past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
-        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta))
-
+        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(
+            self.w_plus_minus_w_bm.value[:-1]) @ delta))
 
     def test_full_returns_forecast_error(self):
         "Test ReturnsForecastError object with as forecast the std of the mean estimator."
         error_risk = ReturnsForecastError()
         cvxpy_expression = self.boilerplate(error_risk)
         t = self.returns.index[123]
         past_returns = self.returns.loc[self.returns.index < t]
-        error_risk._recursive_values_in_time(t=t, past_returns = past_returns)
+        error_risk._recursive_values_in_time(t=t, past_returns=past_returns)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         delta = past_returns.std(ddof=0) / np.sqrt(past_returns.count())
         print(cvxpy_expression.value)
         print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
-        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
-    
-    
+        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(
+            self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
+
 
 if __name__ == '__main__':
     unittest.main()
-
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_risks.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,224 +21,231 @@
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.risks import *
 
 USED_RETURNS = 10
 
+
 class TestRisks(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0]).iloc[:, :USED_RETURNS]
+        cls.returns = pd.read_csv(Path(
+            __file__).parent / "returns.csv", index_col=0, parse_dates=[0]).iloc[:, :USED_RETURNS]
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-        
+
     def boilerplate(self, model):
-        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        model._recursive_pre_evaluation(
+            universe=self.returns.columns, backtest_times=self.returns.index)
         return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
 
-
     def test_full_sigma(self):
-        historical_covariances = self.returns.iloc[:, :-1].rolling(50).cov(ddof=0).dropna()
+        historical_covariances = self.returns.iloc[:,
+                                                   :-1].rolling(50).cov(ddof=0).dropna()
         risk_model = FullCovariance(historical_covariances)
-        
+
         cvxpy_expression = self.boilerplate(risk_model)
 
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_covariances.index[123][0]
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model._recursive_values_in_time(t=t, past_returns='Hello!')
 
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
-                          historical_covariances.loc[t] @ self.w_plus_minus_w_bm.value[:-1]))
-                               
+                                   historical_covariances.loc[t] @ self.w_plus_minus_w_bm.value[:-1]))
+
     def test_full_estimated_sigma(self):
 
         risk_model = FullCovariance()
-        
+
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         # N = returns.shape[1]
         # returns.iloc[:, -1] = 0.
 
         # w_plus = cp.Variable(N)
         # risk_model._recursive_pre_evaluation(
         #     returns.iloc[:, :], None, start_time=returns.index[50], end_time=None)
         # cvxpy_expression = risk_model._compile_to_cvxpy(w_plus, None, None)
-        
+
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
-        should_be = past.iloc[:,:-1].T @ past.iloc[:,:-1] / len(past)
-        
-        self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
-        
+        should_be = past.iloc[:, :-1].T @ past.iloc[:, :-1] / len(past)
+
+        self.w_plus_minus_w_bm.value = np.random.randn(self.N)
+
         risk_model._recursive_values_in_time(t=t, past_returns=past)
         print(cvxpy_expression.value)
-        
-        print(self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1])
-        
+
+        print(self.w_plus_minus_w_bm.value[:-1] @
+              should_be @ self.w_plus_minus_w_bm.value[:-1])
+
         self.assertTrue(np.isclose(cvxpy_expression.value,
-                          self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1]))
-                          
+                                   self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1]))
+
     def test_diagonal_covariance(self):
 
         # N = returns.shape[1]
         # returns.iloc[:, -1] = 0.
 
-        historical_variances = self.returns.iloc[:,:-1].rolling(50).var().shift(1).dropna()
+        historical_variances = self.returns.iloc[:,
+                                                 :-1].rolling(50).var().shift(1).dropna()
         risk_model = DiagonalCovariance(historical_variances)
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
-        self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
+        self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model._recursive_values_in_time(t=t, past_returns='hello')
 
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
-                          np.diag(historical_variances.loc[t]) @ self.w_plus_minus_w_bm.value[:-1]))
+                                   np.diag(historical_variances.loc[t]) @ self.w_plus_minus_w_bm.value[:-1]))
 
     def test_full_diagonal_covariance(self):
 
         risk_model = DiagonalCovariance()
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
         should_be = (past**2).mean()
         should_be.iloc[-1] = 0.
-        
+
         risk_model._recursive_values_in_time(t=t, past_returns=past)
-        self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
-        
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
-                          np.diag(should_be) @ self.w_plus_minus_w_bm.value))
+        self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
+        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
+                                   np.diag(should_be) @ self.w_plus_minus_w_bm.value))
 
     def test_forecast_error(self):
 
-        historical_variances = (self.returns.iloc[:, :-1]**2).rolling(50).mean().shift(1).dropna()
-        
+        historical_variances = (
+            self.returns.iloc[:, :-1]**2).rolling(50).mean().shift(1).dropna()
+
         risk_model = RiskForecastError(historical_variances)
         cvxpy_expression = self.boilerplate(risk_model)
-        
+
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
-        
-        self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
+
+        self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model._recursive_values_in_time(t=t, past_returns='hello')
 
         print(cvxpy_expression.value)
-        print((np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2)
-        self.assertTrue(np.isclose(cvxpy_expression.value, 
-        
-        (np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2
-        
-        ))
+        print((np.abs(
+            self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2)
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+
+                                   (np.abs(
+                                       self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2
+
+                                   ))
 
     def test_full_forecast_error(self):
 
         risk_model = RiskForecastError()
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = pd.Timestamp('2014-06-02')
-        
+
         past = self.returns.loc[self.returns.index < t]
         should_be = (past**2).mean()
         should_be.iloc[-1] = 0.
 
         risk_model._recursive_values_in_time(t=t, past_returns=past)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
-        self.assertTrue(np.isclose(cvxpy_expression.value, 
-        
-        (np.abs(self.w_plus_minus_w_bm.value) @ np.sqrt(should_be))**2
-        
-        ))
-        
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+
+                                   (np.abs(self.w_plus_minus_w_bm.value)
+                                    @ np.sqrt(should_be))**2
+
+                                   ))
+
     def test_low_rank_covariance(self):
-        
-        F = pd.DataFrame(np.random.randn(2, self.N-1), columns=self.returns.columns[:-1])
-        d = pd.Series(np.random.uniform(size=(self.N-1)), self.returns.columns[:-1])
+
+        F = pd.DataFrame(np.random.randn(2, self.N-1),
+                         columns=self.returns.columns[:-1])
+        d = pd.Series(np.random.uniform(size=(self.N-1)),
+                      self.returns.columns[:-1])
         risk_model = FactorModelCovariance(F=F, d=d)
-        
+
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
-        
-        risk_model._recursive_values_in_time(t=self.returns.index[12], past_returns='hello')
+
+        risk_model._recursive_values_in_time(
+            t=self.returns.index[12], past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
-        
-        self.assertTrue(np.isclose(cvxpy_expression.value, 
-            self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] + \
-                ((F @ self.w_plus_minus_w_bm.value[:-1])**2).sum()))
-                
+
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+                                   self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] +
+                                   ((F @ self.w_plus_minus_w_bm.value[:-1])**2).sum()))
+
     def test_estimated_low_rank_covariance(self):
-        
-        risk_model = FactorModelCovariance()#normalize=False)
-        
+
+        risk_model = FactorModelCovariance()  # normalize=False)
+
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
-        
+
         t = pd.Timestamp('2014-06-02')
-        
+
         past = self.returns.loc[self.returns.index < t]
-        
+
         FS = past.T @ past / len(past)
         FS.iloc[:, -1] = 0.
         FS.iloc[-1, :] = 0.
         eigval, eigvec = np.linalg.eigh(FS)
         F = np.sqrt(eigval[-1]) * eigvec[:, -1]
         d = np.diag(FS) - F**2
-        
+
         risk_model._recursive_values_in_time(t=t, past_returns=past)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
-        
+
         self.assertTrue(np.isclose(cvxpy_expression.value,
-            self.w_plus_minus_w_bm.value @ np.diag(d) @ self.w_plus_minus_w_bm.value + \
-                ((F @ self.w_plus_minus_w_bm.value)**2).sum()))
-                
-                
-                
+                                   self.w_plus_minus_w_bm.value @ np.diag(d) @ self.w_plus_minus_w_bm.value +
+                                   ((F @ self.w_plus_minus_w_bm.value)**2).sum()))
+
     def test_worst_case_risk(self):
 
         risk_model0 = FullCovariance()
         risk_model1 = DiagonalCovariance()
         worst_case = WorstCaseRisk([risk_model0, risk_model1])
-        
+
         cvxpy_expression = self.boilerplate(worst_case)
 
         assert cvxpy_expression.is_convex()
 
-        cvxpy_expression0 = risk_model0._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        cvxpy_expression1 = risk_model1._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cvxpy_expression0 = risk_model0._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cvxpy_expression1 = risk_model1._compile_to_cvxpy(
+            self.w_plus, self.z, self.w_plus_minus_w_bm)
 
         self.w_plus_minus_w_bm.value = np.ones(self.N)
 
         t = pd.Timestamp('2014-06-02')
-        
-        worst_case._recursive_values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
+
+        worst_case._recursive_values_in_time(
+            t=t, past_returns=self.returns.loc[self.returns.index < t])
 
         print(cvxpy_expression.value)
         print(cvxpy_expression0.value)
         print(cvxpy_expression1.value)
         assert (cvxpy_expression.value == cvxpy_expression0.value)
         assert (cvxpy_expression.value > cvxpy_expression1.value)
-        
-
 
 
 if __name__ == '__main__':
     unittest.main()
-
-
-
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.4.3/cvxportfolio/tests/test_simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,536 +26,568 @@
 
 from cvxportfolio.simulator import StockMarketSimulator, MarketSimulator, MarketData
 from cvxportfolio.estimator import DataEstimator
 
 from copy import deepcopy
 import cvxportfolio as cvx
 
+
 class TestSimulator(unittest.TestCase):
-    
+
     @classmethod
     def setUpClass(cls):
         """Initialize data directory."""
         cls.datadir = Path(tempfile.mkdtemp())
         print('created', cls.datadir)
-        
-        cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
-        cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
-        cls.prices = pd.DataFrame(np.random.uniform(10, 200, size=cls.volumes.shape), 
-            index=cls.volumes.index, columns=cls.volumes.columns)
+
+        cls.returns = pd.read_csv(
+            Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
+        cls.volumes = pd.read_csv(
+            Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
+        cls.prices = pd.DataFrame(np.random.uniform(10, 200, size=cls.volumes.shape),
+                                  index=cls.volumes.index, columns=cls.volumes.columns)
         cls.market_data = MarketData(returns=cls.returns, volumes=cls.volumes, prices=cls.prices, cash_key='cash',
-             base_location=cls.datadir)
+                                     base_location=cls.datadir)
         cls.universe = cls.returns.columns
-        
+
     @classmethod
     def tearDownClass(cls):
         """Remove data directory."""
         print('removing', cls.datadir)
         shutil.rmtree(cls.datadir)
-        
+
     def test_market_data__downsample(self):
         "Test downsampling of market data."
         md = MarketData(['AAPL', 'GOOG'])
-        
-        
+
         idx = md.returns.index
-    
-        freqs = ['weekly', 'monthly', 'quarterly'] # not doing annual because XXXX-01-01 is holiday
+
+        # not doing annual because XXXX-01-01 is holiday
+        freqs = ['weekly', 'monthly', 'quarterly']
         testdays = ['2023-05-01', '2023-05-01', '2022-04-01']
-        periods = [['2023-05-01', '2023-05-02', '2023-05-03', '2023-05-04', '2023-05-05'], 
-                    idx[(idx >= '2023-05-01') & (idx < '2023-06-01')],
-                idx[(idx >= '2022-04-01') & (idx < '2022-07-01')]  ]
-        
+        periods = [['2023-05-01', '2023-05-02', '2023-05-03', '2023-05-04', '2023-05-05'],
+                   idx[(idx >= '2023-05-01') & (idx < '2023-06-01')],
+                   idx[(idx >= '2022-04-01') & (idx < '2022-07-01')]]
+
         for i in range(len(freqs)):
-            
+
             new_md = deepcopy(md)
-        
+
             new_md._downsample(freqs[i])
             print(new_md.returns)
             self.assertTrue(np.isnan(new_md.returns.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.volumes.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.prices.GOOG.iloc[0]))
-            
+
             if freqs[i] == 'weekly':
-                self.assertTrue(all(new_md.returns.index.weekday==0))
-                
+                self.assertTrue(all(new_md.returns.index.weekday == 0))
+
             if freqs[i] == 'monthly':
-                self.assertTrue(all(new_md.returns.index.day==1))
-            
-            self.assertTrue(all(md.prices.loc[testdays[i]] == new_md.prices.loc[testdays[i]]))
-            self.assertTrue(np.allclose(md.volumes.loc[periods[i]].sum(), new_md.volumes.loc[testdays[i]]))
-            self.assertTrue(np.allclose((1 + md.returns.loc[periods[i]]).prod(), 1 + new_md.returns.loc[testdays[i]]))
+                self.assertTrue(all(new_md.returns.index.day == 1))
+
+            self.assertTrue(
+                all(md.prices.loc[testdays[i]] == new_md.prices.loc[testdays[i]]))
+            self.assertTrue(np.allclose(
+                md.volumes.loc[periods[i]].sum(), new_md.volumes.loc[testdays[i]]))
+            self.assertTrue(np.allclose(
+                (1 + md.returns.loc[periods[i]]).prod(), 1 + new_md.returns.loc[testdays[i]]))
 
-    
     def test_market_data_methods1(self):
         t = self.returns.index[10]
-        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
+        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(
+            t)
         self.assertTrue(past_returns.index[-1] < t)
         self.assertTrue(past_volumes.index[-1] < t)
         self.assertTrue(past_volumes.index[-1] == past_returns.index[-1])
         print(current_prices.name)
         print(t)
         self.assertTrue(current_prices.name == t)
-        
+
     def test_market_data_methods2(self):
         t = self.returns.index[10]
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(
+            t)
         self.assertTrue(current_and_past_returns.index[-1] == t)
         self.assertTrue(current_and_past_volumes.index[-1] == t)
         print(current_prices.name)
         print(t)
         self.assertTrue(current_prices.name == t)
-        
+
     def test_break_timestamp(self):
-        md = MarketData(['AAPL', 'ZM', 'TSLA'], min_history=pd.Timedelta('365d'), base_location=self.datadir)
+        md = MarketData(['AAPL', 'ZM', 'TSLA'], min_history=pd.Timedelta(
+            '365d'), base_location=self.datadir)
         self.assertTrue(pd.Timestamp('2020-04-20') in md._break_timestamps)
         # self.assertTrue(len(md.break_up_backtest('2000-01-01')) == 3)
-        self.assertTrue(md._limited_universes[pd.Timestamp('2011-06-28')] == ('AAPL', 'TSLA'))
-        
-        
+        self.assertTrue(md._limited_universes[pd.Timestamp(
+            '2011-06-28')] == ('AAPL', 'TSLA'))
+
     def test_market_data_object_safety(self):
         t = self.returns.index[10]
-        
-        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
-        
+
+        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(
+            t)
+
         with self.assertRaises(ValueError):
-            past_returns.iloc[-2,-2] = 2.
-            
+            past_returns.iloc[-2, -2] = 2.
+
         with self.assertRaises(ValueError):
-            past_volumes.iloc[-1,-1] = 2.
-            
+            past_volumes.iloc[-1, -1] = 2.
+
         obj2 = deepcopy(self.market_data)
         obj2._set_read_only()
-        
+
         past_returns, past_volumes, current_prices = obj2._serve_data_policy(t)
-        
+
         with self.assertRaises(ValueError):
             current_prices.iloc[-1] = 2.
-            
+
         current_prices.loc['BABA'] = 3.
-        
+
         past_returns, past_volumes, current_prices = obj2._serve_data_policy(t)
-        
-        self.assertFalse( 'BABA' in current_prices.index)
-        
+
+        self.assertFalse('BABA' in current_prices.index)
+
     def test_market_data_initializations(self):
-        
+
         used_returns = self.returns.iloc[:, :-1]
         t = self.returns.index[20]
-        
-        with_download_fred = MarketData(returns=used_returns, volumes=self.volumes, prices=self.prices, 
-            cash_key='USDOLLAR', base_location=self.datadir)
-        
+
+        with_download_fred = MarketData(returns=used_returns, volumes=self.volumes, prices=self.prices,
+                                        cash_key='USDOLLAR', base_location=self.datadir)
+
         without_prices = MarketData(returns=used_returns, volumes=self.volumes, cash_key='USDOLLAR',
-             base_location=self.datadir)
-        past_returns, past_volumes, current_prices = without_prices._serve_data_policy(t)
+                                    base_location=self.datadir)
+        past_returns, past_volumes, current_prices = without_prices._serve_data_policy(
+            t)
         self.assertTrue(current_prices is None)
-        
-        without_volumes = MarketData(returns=used_returns, cash_key='USDOLLAR', base_location=self.datadir)
-        current_and_past_returns, current_and_past_volumes, current_prices = without_volumes._serve_data_simulator(t)
+
+        without_volumes = MarketData(
+            returns=used_returns, cash_key='USDOLLAR', base_location=self.datadir)
+        current_and_past_returns, current_and_past_volumes, current_prices = without_volumes._serve_data_simulator(
+            t)
         self.assertTrue(current_and_past_volumes is None)
-        
+
         with self.assertRaises(SyntaxError):
-            MarketData(returns=self.returns, volumes=self.volumes, prices=self.prices.iloc[:, :-1], cash_key='cash', 
-                base_location=self.datadir)
-             
-        with self.assertRaises(SyntaxError):
-            MarketData(returns=self.returns, volumes=self.volumes.iloc[:,:-3], prices=self.prices, cash_key='cash', 
-                base_location=self.datadir)
-             
-        with self.assertRaises(SyntaxError):
-            used_prices = pd.DataFrame(self.prices, index=self.prices.index, columns=self.prices.columns[::-1])
-            MarketData(returns=self.returns, volumes=self.volumes, prices=used_prices, cash_key='cash', 
-                base_location=self.datadir)
- 
-        with self.assertRaises(SyntaxError):
-            used_volumes = pd.DataFrame(self.volumes, index=self.volumes.index, columns=self.volumes.columns[::-1])
-            MarketData(returns=self.returns, volumes=used_volumes, prices=self.prices, cash_key='cash', 
-                base_location=self.datadir)    
-    
+            MarketData(returns=self.returns, volumes=self.volumes, prices=self.prices.iloc[:, :-1], cash_key='cash',
+                       base_location=self.datadir)
+
+        with self.assertRaises(SyntaxError):
+            MarketData(returns=self.returns, volumes=self.volumes.iloc[:, :-3], prices=self.prices, cash_key='cash',
+                       base_location=self.datadir)
+
+        with self.assertRaises(SyntaxError):
+            used_prices = pd.DataFrame(
+                self.prices, index=self.prices.index, columns=self.prices.columns[::-1])
+            MarketData(returns=self.returns, volumes=self.volumes, prices=used_prices, cash_key='cash',
+                       base_location=self.datadir)
+
+        with self.assertRaises(SyntaxError):
+            used_volumes = pd.DataFrame(
+                self.volumes, index=self.volumes.index, columns=self.volumes.columns[::-1])
+            MarketData(returns=self.returns, volumes=used_volumes, prices=self.prices, cash_key='cash',
+                       base_location=self.datadir)
+
     def test_market_data_full(self):
-        
+
         md = MarketData(['AAPL', 'ZM'], base_location=self.datadir)
         assert np.all(md.universe == ['AAPL', 'ZM', 'USDOLLAR'])
-        
+
         t = md.returns.index[-40]
-        
+
         past_returns, past_volumes, current_prices = md._serve_data_policy(t)
         self.assertFalse(past_volumes is None)
         self.assertFalse(current_prices is None)
-        
-    
+
     def test_simulator_raises(self):
 
         with self.assertRaises(SyntaxError):
             simulator = MarketSimulator()
 
         with self.assertRaises(SyntaxError):
-            simulator = StockMarketSimulator(returns=pd.DataFrame([[0.]], index=[pd.Timestamp.today()], columns=['USDOLLAR']))
+            simulator = StockMarketSimulator(returns=pd.DataFrame(
+                [[0.]], index=[pd.Timestamp.today()], columns=['USDOLLAR']))
 
         with self.assertRaises(SyntaxError):
-            simulator = MarketSimulator(volumes=pd.DataFrame([[0.]], index=[pd.Timestamp.today()]))
+            simulator = MarketSimulator(volumes=pd.DataFrame(
+                [[0.]], index=[pd.Timestamp.today()]))
 
         with self.assertRaises(SyntaxError):
             simulator = MarketSimulator(returns=pd.DataFrame(
                 [[0.]], columns=['USDOLLAR'], index=[pd.Timestamp.today()]), volumes=pd.DataFrame([[0.]]))
 
         # not raises
         simulator = MarketSimulator(returns=pd.DataFrame([[0., 0.]], columns=['A', 'USDOLLAR']), volumes=pd.DataFrame(
             [[0.]], columns=['A']), per_share_fixed_cost=0., round_trades=False)
 
         with self.assertRaises(SyntaxError):
             simulator = MarketSimulator(returns=pd.DataFrame(
                 [[0., 0.]], index=[pd.Timestamp.today()], columns=['X', 'USDOLLAR']), volumes=pd.DataFrame([[0.]]), per_share_fixed_cost=0.)
 
-            
     def test_prepare_data(self):
         simulator = MarketSimulator(['ZM', 'META'], base_location=self.datadir)
         self.assertTrue(simulator.market_data.returns.shape[1] == 3)
-        self.assertTrue( simulator.market_data.prices.shape[1] == 2)
-        self.assertTrue( simulator.market_data.volumes.shape[1] == 2)
+        self.assertTrue(simulator.market_data.prices.shape[1] == 2)
+        self.assertTrue(simulator.market_data.volumes.shape[1] == 2)
         # self.assertTrue( simulator.sigma_estimate.data.shape[1] == 2)
-        self.assertTrue( np.isnan(simulator.market_data.returns.iloc[-1, 0]))
-        self.assertTrue( np.isnan(simulator.market_data.volumes.iloc[-1, 1]))
-        self.assertTrue( not np.isnan(simulator.market_data.prices.iloc[-1, 0]))
-        self.assertTrue( simulator.market_data.returns.index[-1] == simulator.market_data.volumes.index[-1])
-        self.assertTrue( simulator.market_data.returns.index[-1] == simulator.market_data.prices.index[-1])
+        self.assertTrue(np.isnan(simulator.market_data.returns.iloc[-1, 0]))
+        self.assertTrue(np.isnan(simulator.market_data.volumes.iloc[-1, 1]))
+        self.assertTrue(not np.isnan(simulator.market_data.prices.iloc[-1, 0]))
+        self.assertTrue(
+            simulator.market_data.returns.index[-1] == simulator.market_data.volumes.index[-1])
+        self.assertTrue(
+            simulator.market_data.returns.index[-1] == simulator.market_data.prices.index[-1])
 
-            
-        
     def test_cash_holding_cost(self):
-        
+
         t = self.returns.index[-40]
-        
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
-        
+
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(
+            t)
+
         cash_return = self.returns.loc[t, 'cash']
-        
+
         hcost = cvx.StocksHoldingCost(
-            #spread_on_lending_cash_percent=0.,
-            #spread_on_borrowing_cash_percent=0.,
+            # spread_on_lending_cash_percent=0.,
+            # spread_on_borrowing_cash_percent=0.,
             dividends=0.,
             periods_per_year=252,
             spread_on_borrowing_stocks_percent=0.,
             cash_return_on_borrow=False)
-        
+
         for i in range(10):
             np.random.seed(i)
             h_plus = np.random.randn(self.returns.shape[1])*1000
             h_plus = pd.Series(h_plus, self.returns.columns)
             h_plus[-1] = 1000 - sum(h_plus[:-1])
-            
-            sim_cash_hcost = hcost._simulate(t, h_plus=h_plus, current_and_past_returns=current_and_past_returns)
 
-            real_cash_position = h_plus[-1] + sum(np.minimum(h_plus[:-1],0.))
+            sim_cash_hcost = hcost._simulate(
+                t, h_plus=h_plus, current_and_past_returns=current_and_past_returns)
+
+            real_cash_position = h_plus[-1] + sum(np.minimum(h_plus[:-1], 0.))
             if real_cash_position > 0:
-                cash_hcost = real_cash_position * (np.maximum(cash_return - 0.005/252, 0.) - cash_return)
+                cash_hcost = real_cash_position * \
+                    (np.maximum(cash_return - 0.005/252, 0.) - cash_return)
             if real_cash_position < 0:
                 cash_hcost = real_cash_position * (0.005/252)
 
             self.assertTrue(np.isclose(cash_hcost, sim_cash_hcost))
 
-
     def test_stocks_holding_cost(self):
-                
+
         t = self.returns.index[-20]
-        
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
-        
+
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(
+            t)
+
         cash_return = self.returns.loc[t, 'cash']
-        
-        ## stock holding cost
+
+        # stock holding cost
         for i in range(10):
             np.random.seed(i)
             h_plus = np.random.randn(4)*10000
             h_plus[3] = 10000 - sum(h_plus[:-1])
             h_plus = pd.Series(h_plus)
-            
+
             dividends = np.random.uniform(size=len(h_plus)-1) * 1E-4
-            
+
             hcost = cvx.StocksHoldingCost(
                 spread_on_lending_cash_percent=0.,
                 spread_on_borrowing_cash_percent=0.,
                 dividends=dividends, periods_per_year=252)
-            
-            
-            sim_hcost = hcost._simulate(t=t, h_plus = h_plus, current_and_past_returns=current_and_past_returns)
-            
+
+            sim_hcost = hcost._simulate(
+                t=t, h_plus=h_plus, current_and_past_returns=current_and_past_returns)
+
             total_borrow_cost = cash_return + (0.005)/252
-            hcost = -total_borrow_cost * sum(-np.minimum(h_plus,0.)[:-1])
+            hcost = -total_borrow_cost * sum(-np.minimum(h_plus, 0.)[:-1])
             hcost += dividends @ h_plus[:-1]
-            
+
             self.assertTrue(np.isclose(hcost, sim_hcost))
-    
-    
+
     def test_transaction_cost_syntax(self):
-                
+
         t = self.returns.index[-20]
-        
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
-        
+
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(
+            t)
+
         u = pd.Series(np.ones(len(current_prices)+1), self.universe)
-        
+
         tcost = cvx.StocksTransactionCost()
         # syntax checks
         with self.assertRaises(SyntaxError):
-            tcost._simulate(t, u=u, current_prices=None, 
-                            current_and_past_volumes=current_and_past_volumes, 
+            tcost._simulate(t, u=u, current_prices=None,
+                            current_and_past_volumes=current_and_past_volumes,
                             current_and_past_returns=current_and_past_returns)
-        
+
         tcost = cvx.TransactionCost(pershare_cost=None,)
-        tcost._simulate(t, u=u, current_prices=None, 
-                        current_and_past_volumes=current_and_past_volumes, 
+        tcost._simulate(t, u=u, current_prices=None,
+                        current_and_past_volumes=current_and_past_volumes,
                         current_and_past_returns=current_and_past_returns)
-        
-        tcost = cvx.TransactionCost()           
+
+        tcost = cvx.TransactionCost()
         with self.assertRaises(SyntaxError):
-            tcost._simulate(t, u=u, current_prices=current_prices, 
-                            current_and_past_volumes=None, 
+            tcost._simulate(t, u=u, current_prices=current_prices,
+                            current_and_past_volumes=None,
                             current_and_past_returns=current_and_past_returns)
-        
+
         tcost = cvx.TransactionCost(b=None)
-        tcost._simulate(t, u=u, current_prices=current_prices, 
-                        current_and_past_volumes=None, 
+        tcost._simulate(t, u=u, current_prices=current_prices,
+                        current_and_past_volumes=None,
                         current_and_past_returns=current_and_past_returns)
-        
-        
+
     def test_transaction_cost(self):
-        
+
         t = self.returns.index[-5]
-        
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
+
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(
+            t)
         print(current_prices)
-                
+
         n = len(current_prices)
-        
+
         for i in range(10):
             np.random.seed(i)
             spreads = np.random.uniform(size=n)*1E-3
             u = np.random.uniform(size=n+1)*1E4
             u[-1] = -sum(u[:-1])
             u = pd.Series(u, self.universe)
             u = MarketSimulator._round_trade_vector(u, current_prices)
-            
-            tcost = cvx.StocksTransactionCost(a = spreads/2)
-                        
-            sim_cost = tcost._simulate(t, u=u, current_prices=current_prices, 
-                            current_and_past_volumes=current_and_past_volumes, 
-                            current_and_past_returns=current_and_past_returns)
+
+            tcost = cvx.StocksTransactionCost(a=spreads/2)
+
+            sim_cost = tcost._simulate(t, u=u, current_prices=current_prices,
+                                       current_and_past_volumes=current_and_past_volumes,
+                                       current_and_past_returns=current_and_past_returns)
 
             shares = sum(np.abs(u[:-1] / current_prices))
             tcost = -0.005 * shares
             # print(tcost, sim_cost)
             tcost -= np.abs(u.iloc[:-1]) @ spreads / 2
             # print(self.returns.loc[self.returns.index <= t].iloc[-252:, :-1].std())
-            tcost -= sum((np.abs(u.iloc[:-1])**1.5) * self.returns.loc[self.returns.index <= t].iloc[-252:, :-1].std(ddof=0) / np.sqrt(self.volumes.loc[t]))
+            tcost -= sum((np.abs(u.iloc[:-1])**1.5) * self.returns.loc[self.returns.index <=
+                         t].iloc[-252:, :-1].std(ddof=0) / np.sqrt(self.volumes.loc[t]))
             # sim_tcost = simulator.transaction_costs(u)
             #
             print(tcost, sim_cost)
             self.assertTrue(np.isclose(tcost, sim_cost))
-        
 
-             
     def test_methods(self):
-        simulator = MarketSimulator(['ZM', 'META', 'AAPL'], base_location=self.datadir)
-    
-        for t in [pd.Timestamp('2023-04-13')]:#, pd.Timestamp('2022-04-11')]: # can't because sigma requires 1000 days
-            #super(simulator.__class__, simulator)._recursive_values_in_time(t=t)
-            
-            ## round trade
-    
+        simulator = MarketSimulator(
+            ['ZM', 'META', 'AAPL'], base_location=self.datadir)
+
+        # , pd.Timestamp('2022-04-11')]: # can't because sigma requires 1000 days
+        for t in [pd.Timestamp('2023-04-13')]:
+            # super(simulator.__class__, simulator)._recursive_values_in_time(t=t)
+
+            # round trade
+
             for i in range(10):
                 np.random.seed(i)
                 tmp = np.random.uniform(size=4)*1000
                 tmp[3] = -sum(tmp[:3])
                 u = pd.Series(tmp, simulator.market_data.universe)
-                rounded = simulator._round_trade_vector(u, simulator.market_data.prices.loc[t])
+                rounded = simulator._round_trade_vector(
+                    u, simulator.market_data.prices.loc[t])
                 self.assertTrue(sum(rounded) == 0)
-                self.assertTrue(np.linalg.norm(rounded[:-1] - u[:-1]) < \
-                    np.linalg.norm(simulator.market_data.prices.loc[t]/2))
-        
+                self.assertTrue(np.linalg.norm(rounded[:-1] - u[:-1]) <
+                                np.linalg.norm(simulator.market_data.prices.loc[t]/2))
+
                 print(u)
-        
-                
+
     def test__simulate_policy(self):
-        simulator = StockMarketSimulator(['META', 'AAPL'], base_location=self.datadir)
-    
+        simulator = StockMarketSimulator(
+            ['META', 'AAPL'], base_location=self.datadir)
 
         start_time = '2023-03-10'
         end_time = '2023-04-20'
-    
-        ## hold
+
+        # hold
         policy = cvx.Hold()
         for i in range(10):
             np.random.seed(i)
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.market_data.universe)
             h = pd.Series(h0, copy=True)
-            simulator._initialize_policy(policy, start_time, end_time)
+
+            policy._recursive_pre_evaluation(
+                universe=simulator.market_data.universe,
+                backtest_times=simulator.market_data._get_backtest_times(
+                    start_time, end_time, include_end=False)
+            )
+
             for t in simulator.market_data.returns.index[(simulator.market_data.returns.index >= start_time) & (simulator.market_data.returns.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, costs, timer = simulator._simulate(t=t, h=h, policy=policy)
+                h, z, u, costs, timer = simulator._simulate(
+                    t=t, h=h, policy=policy)
                 tcost, hcost = costs['StocksTransactionCost'], costs['StocksHoldingCost']
                 assert tcost == 0.
-                #if np.all(h0[:2] > 0):
+                # if np.all(h0[:2] > 0):
                 #    assert hcost == 0.
-                assert np.isclose((oldcash + hcost) * (1+simulator.market_data.returns.loc[t, 'USDOLLAR']), h[-1])
-            
-            simh = h0[:-1] * simulator.market_data.prices.loc[pd.Timestamp(end_time) + pd.Timedelta('1d')] / simulator.market_data.prices.loc[start_time]
+                assert np.isclose(
+                    (oldcash + hcost) * (1+simulator.market_data.returns.loc[t, 'USDOLLAR']), h[-1])
+
+            simh = h0[:-1] * simulator.market_data.prices.loc[pd.Timestamp(
+                end_time) + pd.Timedelta('1d')] / simulator.market_data.prices.loc[start_time]
             self.assertTrue(np.allclose(simh, h[:-1]))
-        
-        ## proportional_trade
+
+        # proportional_trade
         policy = cvx.ProportionalTradeToTargets(
-        targets = pd.DataFrame({pd.Timestamp(end_time) + pd.Timedelta('1d'):  pd.Series([0, 0, 1], simulator.market_data.returns.columns)}).T)
-        
+            targets=pd.DataFrame({pd.Timestamp(end_time) + pd.Timedelta('1d'):  pd.Series([0, 0, 1], simulator.market_data.returns.columns)}).T)
+
         for i in range(10):
             np.random.seed(i)
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.market_data.returns.columns)
             h = pd.Series(h0, copy=True)
-            simulator._initialize_policy(policy, start_time, end_time)
+            policy._recursive_pre_evaluation(
+                universe=simulator.market_data.universe,
+                backtest_times=simulator.market_data._get_backtest_times(
+                    start_time, end_time, include_end=False)
+            )
+
             for t in simulator.market_data.returns.index[(simulator.market_data.returns.index >= start_time) & (simulator.market_data.returns.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, costs, timer = simulator._simulate(t=t, h=h, policy=policy)
+                h, z, u, costs, timer = simulator._simulate(
+                    t=t, h=h, policy=policy)
                 tcost, hcost = costs['StocksTransactionCost'], costs['StocksHoldingCost']
                 print(h)
                 # print(tcost, stock_hcost, cash_hcost)
-            
-            self.assertTrue(np.all(np.abs(h[:-1]) < simulator.market_data.prices.loc[end_time]))
-            
+
+            self.assertTrue(
+                np.all(np.abs(h[:-1]) < simulator.market_data.prices.loc[end_time]))
+
     def test_backtest(self):
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
-            cvx.ReturnsForecastError() -
-            .5 * cvx.FullCovariance(),
-            [#cvx.LongOnly(),
+                                           cvx.ReturnsForecastError() -
+                                           .5 * cvx.FullCovariance(),
+                                           [  # cvx.LongOnly(),
             cvx.LeverageLimit(1)], verbose=True)
-        sim = cvx.MarketSimulator(['AAPL', 'MSFT'],#', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
-         base_location=self.datadir)
-        result = sim.backtest(pol, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
-        
+        sim = cvx.MarketSimulator(['AAPL', 'MSFT'],  # ', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
+                                  base_location=self.datadir)
+        result = sim.backtest(pol, pd.Timestamp(
+            '2023-01-01'), pd.Timestamp('2023-04-20'))
+
         print(result)
-        
+
     def test_backtest_concatenation(self):
         sim = cvx.MarketSimulator(['AAPL', 'ZM'])
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
-            cvx.ReturnsForecastError() -
-            .5 * cvx.FullCovariance(),
-            [#cvx.LongOnly(),
+                                           cvx.ReturnsForecastError() -
+                                           .5 * cvx.FullCovariance(),
+                                           [  # cvx.LongOnly(),
             cvx.LeverageLimit(1)], verbose=True)
-        
-        result = sim.backtest(pol, pd.Timestamp('2020-04-01'), pd.Timestamp('2020-05-01')) # zoom enters in mid-april
+
+        result = sim.backtest(pol, pd.Timestamp(
+            '2020-04-01'), pd.Timestamp('2020-05-01'))  # zoom enters in mid-april
         ridx = result.w.index
         self.assertTrue(result.w['ZM'].isnull().sum() > 5)
         self.assertTrue(result.w['AAPL'].isnull().sum() < 2)
         self.assertTrue(len(ridx) == len(set(ridx)))
         self.assertTrue(len(ridx) == len(sim.market_data.returns.loc[
-            (sim.market_data.returns.index>=ridx[0]) & (sim.market_data.returns.index<=ridx[-1]) ]))
+            (sim.market_data.returns.index >= ridx[0]) & (sim.market_data.returns.index <= ridx[-1])]))
         print(result)
-            
+
     def test_multiple_backtest(self):
-        
+
         pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() -
-            cvx.ReturnsForecastError() -
-            .5 * cvx.FullCovariance(),
-            [#cvx.LongOnly(),
+                                           cvx.ReturnsForecastError() -
+                                           .5 * cvx.FullCovariance(),
+                                           [  # cvx.LongOnly(),
             cvx.LeverageLimit(1)], verbose=True)
-            
+
         pol1 = cvx.Uniform()
-        
-        sim = cvx.MarketSimulator(['AAPL', 'MSFT'],#', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
-         base_location=self.datadir)
-         
-        with self.assertRaises(SyntaxError):
-            result = sim.backtest_many([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'), h=['hello'])
-            
-        result =  sim.backtest(pol1, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
-        
-        result2, result3 =  sim.backtest_many([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
-        
+
+        sim = cvx.MarketSimulator(['AAPL', 'MSFT'],  # ', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
+                                  base_location=self.datadir)
+
+        with self.assertRaises(SyntaxError):
+            result = sim.backtest_many([pol, pol1], pd.Timestamp(
+                '2023-01-01'), pd.Timestamp('2023-04-20'), h=['hello'])
+
+        result = sim.backtest(pol1, pd.Timestamp(
+            '2023-01-01'), pd.Timestamp('2023-04-20'))
+
+        result2, result3 = sim.backtest_many(
+            [pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
+
         self.assertTrue(np.all(result.h == result3.h))
-        
-    
+
     def test_multiple_backtest2(self):
         """Test re-use of a worker process"""
         cpus = multiprocessing.cpu_count()
-        
+
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'], base_location=self.datadir)
         pols = [cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)])
-            for i in range(cpus*2)]
-        results = sim.backtest_many(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
+                for i in range(cpus*2)]
+        results = sim.backtest_many(pols, pd.Timestamp(
+            '2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
         sharpes = [result.sharpe_ratio for result in results]
         self.assertTrue(len(set(sharpes)) == 1)
-        
-        
+
     def test_multiple_backtest3(self):
         """Test benchmarks."""
-        
-        
+
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'], base_location=self.datadir)
         pols = [
-            cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)]),
-            cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.UniformBenchmark),
-            cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.MarketBenchmark),
-                ]
-        results = sim.backtest_many(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
+            cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
+            ) - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)]),
+            cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
+            ) - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.UniformBenchmark),
+            cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
+            ) - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.MarketBenchmark),
+        ]
+        results = sim.backtest_many(pols, pd.Timestamp(
+            '2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
         print(np.linalg.norm(results[0].w.sum()[:2] - .5))
         print(np.linalg.norm(results[1].w.sum()[:2] - .5))
         print(np.linalg.norm(results[2].w.sum()[:2] - .5))
-        self.assertTrue( np.linalg.norm(results[1].w.sum()[:2] - .5) < np.linalg.norm(results[0].w.sum()[:2] - .5) )
-        self.assertTrue( np.linalg.norm(results[1].w.sum()[:2] - .5) < np.linalg.norm(results[2].w.sum()[:2] - .5) )
-        
+        self.assertTrue(np.linalg.norm(results[1].w.sum()[
+                        :2] - .5) < np.linalg.norm(results[0].w.sum()[:2] - .5))
+        self.assertTrue(np.linalg.norm(results[1].w.sum()[
+                        :2] - .5) < np.linalg.norm(results[2].w.sum()[:2] - .5))
+
     def test_multiple_backtest4(self):
         """Test _downsample and offline cache."""
-        
+
         time_first = 0.
         results_first = []
         for downsampling in ['weekly', 'monthly', 'quarterly', 'annual']:
-            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE', 'ZM', 'META'], base_location=self.datadir, trading_frequency=downsampling)
-            pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
+            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE', 'ZM', 'META'],
+                                      base_location=self.datadir, trading_frequency=downsampling)
+            pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
+            ) - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
             s = time.time()
             results_first.append(sim.backtest(pol, pd.Timestamp('2021-12-01')))
-            time_first += time.time() - s 
-            
+            time_first += time.time() - s
+
         time_second = 0.
         results_second = []
         for downsampling in ['weekly', 'monthly', 'quarterly', 'annual']:
-            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE', 'ZM', 'META'], base_location=self.datadir, trading_frequency=downsampling)
-            pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
+            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE', 'ZM', 'META'],
+                                      base_location=self.datadir, trading_frequency=downsampling)
+            pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast(
+            ) - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
             s = time.time()
-            results_second.append(sim.backtest(pol, pd.Timestamp('2021-12-01')))
+            results_second.append(sim.backtest(
+                pol, pd.Timestamp('2021-12-01')))
             time_second += time.time() - s
-        
+
         # example is too small to see speed difference w/ cache
         # sadly we have to drop this test element
         # self.assertTrue(time_second < time_first)
         print(time_second, time_first)
-        [self.assertTrue(np.isclose(results_first[i].sharpe_ratio, results_second[i].sharpe_ratio)) for i in range(len(results_first))]
-            
-            
+        [self.assertTrue(np.isclose(results_first[i].sharpe_ratio,
+                         results_second[i].sharpe_ratio)) for i in range(len(results_first))]
+
     def test_plot_result(self):
         """Test plot method of result."""
-        sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE', 'ZM', 'META'], base_location=self.datadir)
-        sim.backtest(cvx.Uniform(), pd.Timestamp('2023-01-01')).plot(show=False)
-         
-         
-                
-if __name__ == '__main__':
-    unittest.main()
-        
-
-
-
-
-    
+        sim = cvx.MarketSimulator(
+            ['AAPL', 'MSFT', 'GE', 'ZM', 'META'], base_location=self.datadir)
+        sim.backtest(cvx.Uniform(), pd.Timestamp(
+            '2023-01-01')).plot(show=False)
 
 
-
-
-
-         
-
-        
-
-            
-    
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.4.3/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.2/cvxportfolio/utils.py` & `cvxportfolio-0.4.3/cvxportfolio/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pandas as pd
 import numpy as np
 
-__all__ = ['periods_per_year', 'resample_returns', 'flatten_heterogeneous_list']
+__all__ = ['periods_per_year', 'resample_returns',
+           'flatten_heterogeneous_list']
+
 
 def periods_per_year(idx):
     """Given a datetime pandas index return the periods per year."""
-    return int(np.round(len(idx) / ((idx[-1] - idx[0]) / pd.Timedelta('365.24d'))))
-    
+    return int(np.round(len(idx) / ((idx[-1] - idx[0]) /
+                                    pd.Timedelta('365.24d'))))
+
+
 def resample_returns(returns, periods):
     """Resample returns expressed over number of periods to single period."""
     return np.exp(np.log(1 + returns) / periods) - 1
 
-def flatten_heterogeneous_list(l):
+
+def flatten_heterogeneous_list(li):
     """[1, 2, 3, [4, 5]] -> [1, 2, 3, 4, 5]"""
-    return sum(([el] if not hasattr(el, '__iter__') 
-        else el for el in l), [])
+    return sum(([el] if not hasattr(el, '__iter__')
+                else el for el in li), [])
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-0.4.3/cvxportfolio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.4.2
+Version: 0.4.3
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
```

### Comparing `cvxportfolio-0.4.2/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.4.3/cvxportfolio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 cvxportfolio/benchmark.py
 cvxportfolio/constraints.py
 cvxportfolio/costs.py
 cvxportfolio/data.py
 cvxportfolio/errors.py
 cvxportfolio/estimator.py
 cvxportfolio/forecast.py
+cvxportfolio/hyperparameters.py
 cvxportfolio/policies.py
 cvxportfolio/result.py
 cvxportfolio/returns.py
 cvxportfolio/risks.py
 cvxportfolio/simulator.py
 cvxportfolio/utils.py
 cvxportfolio.egg-info/PKG-INFO
@@ -26,12 +27,13 @@
 cvxportfolio/tests/returns.csv
 cvxportfolio/tests/sigmas.csv
 cvxportfolio/tests/test_constraints.py
 cvxportfolio/tests/test_costs.py
 cvxportfolio/tests/test_data.py
 cvxportfolio/tests/test_estimator.py
 cvxportfolio/tests/test_forecast.py
+cvxportfolio/tests/test_hyperparameters.py
 cvxportfolio/tests/test_policies.py
 cvxportfolio/tests/test_returns.py
 cvxportfolio/tests/test_risks.py
 cvxportfolio/tests/test_simulator.py
 cvxportfolio/tests/volumes.csv
```

### Comparing `cvxportfolio-0.4.2/setup.py` & `cvxportfolio-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_descr = ''.join(f.readlines())
 
 setup(
     name='cvxportfolio',
-    version='0.4.2',
+    version='0.4.3',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
```

