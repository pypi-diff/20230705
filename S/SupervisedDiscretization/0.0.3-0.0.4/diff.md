# Comparing `tmp/SupervisedDiscretization-0.0.3.tar.gz` & `tmp/SupervisedDiscretization-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SupervisedDiscretization-0.0.3.tar", last modified: Wed Jul  5 10:21:44 2023, max compression
+gzip compressed data, was "SupervisedDiscretization-0.0.4.tar", last modified: Wed Jul  5 10:35:02 2023, max compression
```

## Comparing `SupervisedDiscretization-0.0.3.tar` & `SupervisedDiscretization-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/
--rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4542 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4167 2023-05-19 14:37:51.000000 SupervisedDiscretization-0.0.3/README.md
--rw-rw-rw-   0        0        0      541 2023-07-05 10:16:39.000000 SupervisedDiscretization-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 10:21:44.235659 SupervisedDiscretization-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.167443 SupervisedDiscretization-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.168359 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/
-drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.233645 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/
--rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
--rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
--rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
--rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2028 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
--rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/__init__.py
--rw-rw-rw-   0        0        0     7211 2023-07-05 10:05:12.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/discretizer.py
-drwxrwxrwx   0        0        0        0 2023-07-05 10:21:44.189595 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/
--rw-rw-rw-   0        0        0     4542 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-05 10:21:44.000000 SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:02.275553 SupervisedDiscretization-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-05-19 11:29:35.000000 SupervisedDiscretization-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4542 2023-07-05 10:35:02.275553 SupervisedDiscretization-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4167 2023-05-19 14:37:51.000000 SupervisedDiscretization-0.0.4/README.md
+-rw-rw-rw-   0        0        0      541 2023-07-05 10:33:45.000000 SupervisedDiscretization-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:35:02.275553 SupervisedDiscretization-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:02.243739 SupervisedDiscretization-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:02.259840 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:02.275553 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/
+-rw-rw-rw-   0        0        0     1372 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py
+-rw-rw-rw-   0        0        0     1016 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py
+-rw-rw-rw-   0        0        0     1323 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py
+-rw-rw-rw-   0        0        0     2322 2023-05-19 13:43:06.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:39:05.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-06-16 17:23:57.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py
+-rw-rw-rw-   0        0        0     2660 2023-05-19 13:31:57.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 13:24:30.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/__init__.py
+-rw-rw-rw-   0        0        0     7221 2023-07-05 10:33:45.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/discretizer.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:35:02.275553 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/
+-rw-rw-rw-   0        0        0     4542 2023-07-05 10:35:02.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2023-07-05 10:35:02.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:35:02.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-05 10:35:02.000000 SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/top_level.txt
```

### Comparing `SupervisedDiscretization-0.0.3/LICENSE` & `SupervisedDiscretization-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/PKG-INFO` & `SupervisedDiscretization-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedDiscretization
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.3 Author-
+Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.4 Author-
 email: Cecilia Salvatore
 salvatore@uniroma2.it> Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # supervised-discretization This repository
 contains the code for the paper Supervised_Feature_Compression_based_on
 Counterfactual_Analysis ## Installation * The MILP problem for computing the
```

### Comparing `SupervisedDiscretization-0.0.3/README.md` & `SupervisedDiscretization-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/pyproject.toml` & `SupervisedDiscretization-0.0.4/pyproject.toml`

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
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Cecilia Salvatore", email="cecilia.salvatore@uniroma2.it" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/GradientBoostingSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/RandomForestSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/SVCSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/TreeEnsembleSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/counterfactualExplanations.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/CounterfactualAnalysis/gurobiSolver.py`

 * *Files identical despite different names*

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization/discretizer.py` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization/discretizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             self.tao = pd.concat((self.tao,self.getAllThresholds(x, y, i)))
 
     def getAllThresholds(self, x, y, c):
         tao_c = pd.DataFrame(columns=['Feature','Threshold'])
         x_c, i_c = np.unique(x[c], return_index=True)
         i_c = i_c[np.argsort(x_c)]
         x_c = x[c].iloc[i_c].to_numpy()
-        y_c = y.iloc[i_c].to_numpy()
+        y_c = y.iloc[i_c].to_numpy().flatten()
         t = x_c[:-1] + (x_c[1:] - x_c[:-1]) / 2
         mask = (y_c[1:] - y_c[:-1]) != 0
         tao_c['Threshold'] = t[mask]
         tao_c['Feature'] = c
         return tao_c
 
 class FCCA(Discretizer):
```

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/PKG-INFO` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedDiscretization
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.3 Author-
+Metadata-Version: 2.1 Name: SupervisedDiscretization Version: 0.0.4 Author-
 email: Cecilia Salvatore
 salvatore@uniroma2.it> Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # supervised-discretization This repository
 contains the code for the paper Supervised_Feature_Compression_based_on
 Counterfactual_Analysis ## Installation * The MILP problem for computing the
```

### Comparing `SupervisedDiscretization-0.0.3/src/SupervisedDiscretization.egg-info/SOURCES.txt` & `SupervisedDiscretization-0.0.4/src/SupervisedDiscretization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

