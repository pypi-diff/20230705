# Comparing `tmp/SupervisedDiscretization-0.0.2.tar.gz` & `tmp/SupervisedDiscretization-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SupervisedDiscretization-0.0.2.tar", last modified: Fri Jun 16 17:33:53 2023, max compression
+gzip compressed data, was "SupervisedDiscretization-0.0.3.tar", last modified: Wed Jul  5 10:21:44 2023, max compression
```

## Comparing `SupervisedDiscretization-0.0.2.tar` & `SupervisedDiscretization-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/
--rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4542 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4167 2023-05-19 14:37:51.000000 SupervisedDiscretization-0.0.2/README.md
--rw-rw-rw-   0        0        0      541 2023-06-16 17:33:06.000000 SupervisedDiscretization-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.825221 SupervisedDiscretization-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.840933 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/
-drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.860057 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/
--rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
--rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
--rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
--rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2028 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
--rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/__init__.py
--rw-rw-rw-   0        0        0     6512 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/discretizer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:33:53.856504 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/
--rw-rw-rw-   0        0        0     4542 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-16 17:33:53.000000 SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4542 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4167 2023-05-19 14:37:51.000000 SupervisedDiscretization-0.0.3/README.md
+-rw-rw-rw-   0        0        0      541 2023-07-05 10:16:39.000000 SupervisedDiscretization-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.167443 SupervisedDiscretization-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.168359 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.233645 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/
+-rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
+-rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
+-rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
+-rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
+-rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/__init__.py
+-rw-rw-rw-   0        0        0     7211 2023-07-05 10:05:12.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/discretizer.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.189595 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/
+-rw-rw-rw-   0        0        0     4542 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/top_level.txt
```

### Comparing `SupervisedDiscretization-0.0.2/LICENSE` & `SupervisedDiscretization-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/PKG-INFO` & `SupervisedDiscretization-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedDiscretization
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Cecilia Salvatore <cecilia.salvatore@uniroma2.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.2 Author-
+Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.3 Author-
 email: Cecilia Salvatore
 salvatore@uniroma2.it> Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # supervised-discretization This repository
 contains the code for the paper Supervised_Feature_Compression_based_on
 Counterfactual_Analysis ## Installation * The MILP problem for computing the
```

### Comparing `SupervisedDiscretization-0.0.2/README.md` & `SupervisedDiscretization-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/pyproject.toml` & `SupervisedDiscretization-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "scikit-learn",
     "gurobipy"
 ]
 build-backend = "setuptools.build_meta"
 [tool.setuptools]
 [project]
 name = "SupervisedDiscretization"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Cecilia Salvatore", email="cecilia.salvatore@uniroma2.it" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization/discretizer.py` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/discretizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,33 @@
     def getAllThresholds(self, x, c):
         tao_c = pd.DataFrame(columns=['Feature','Threshold'])
         x_c = np.sort(np.unique((x[c])))
         tao_c['Threshold'] = x_c[:-1] + (x_c[1:] - x_c[:-1]) / 2
         tao_c['Feature'] = c
         return tao_c
 
+
+class BucketDiscretizer(Discretizer):
+    def fit(self, x, y):
+        self.tao = pd.DataFrame(columns=['Feature','Threshold'])
+        for i in x.columns:
+            self.tao = pd.concat((self.tao,self.getAllThresholds(x, y, i)))
+
+    def getAllThresholds(self, x, y, c):
+        tao_c = pd.DataFrame(columns=['Feature','Threshold'])
+        x_c, i_c = np.unique(x[c], return_index=True)
+        i_c = i_c[np.argsort(x_c)]
+        x_c = x[c].iloc[i_c].to_numpy()
+        y_c = y.iloc[i_c].to_numpy()
+        t = x_c[:-1] + (x_c[1:] - x_c[:-1]) / 2
+        mask = (y_c[1:] - y_c[:-1]) != 0
+        tao_c['Threshold'] = t[mask]
+        tao_c['Feature'] = c
+        return tao_c
+
 class FCCA(Discretizer):
     def __init__(self, estimator, p0=0.5, p1=1, lambda0=0.1, lambda1=1, lambda2=0.0, compress=True, timelimit=1*60, verbose=True):
         super().__init__()
         self.estimator = estimator
         self.p0 = p0
         self.p1 = p1
         self.lambda0 = lambda0
```

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/PKG-INFO` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedDiscretization
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Cecilia Salvatore <cecilia.salvatore@uniroma2.it>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.2 Author-
+Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.3 Author-
 email: Cecilia Salvatore
 salvatore@uniroma2.it> Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # supervised-discretization This repository
 contains the code for the paper Supervised_Feature_Compression_based_on
 Counterfactual_Analysis ## Installation * The MILP problem for computing the
```

### Comparing `SupervisedDiscretization-0.0.2/src/SupervisedDiscretization.egg-info/SOURCES.txt` & `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

