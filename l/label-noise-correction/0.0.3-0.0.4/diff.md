# Comparing `tmp/label_noise_correction-0.0.3.tar.gz` & `tmp/label_noise_correction-0.0.4.tar.gz`

## Comparing `label_noise_correction-0.0.3.tar` & `label_noise_correction-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/__init__.py
--rwxr-xr-x   0        0        0     2893 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/be.py
--rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/cc.py
--rwxr-xr-x   0        0        0     5831 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/fair_obnc.py
--rwxr-xr-x   0        0        0     3935 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/hlnc.py
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/labelcorrection.py
--rwxr-xr-x   0        0        0     1809 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/obnc.py
--rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/pl.py
--rwxr-xr-x   0        0        0     4076 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/src/label_noise_correction/stc.py
--rwxr-xr-x   0        0        0     3238 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/.gitignore
--rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     3501 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/README.md
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 label_noise_correction-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/__init__.py
+-rwxr-xr-x   0        0        0     2893 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/be.py
+-rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/cc.py
+-rwxr-xr-x   0        0        0     4887 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/fair_obnc.py
+-rwxr-xr-x   0        0        0     3935 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/hlnc.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/labelcorrection.py
+-rwxr-xr-x   0        0        0     1809 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/obnc.py
+-rwxr-xr-x   0        0        0     1699 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/pl.py
+-rwxr-xr-x   0        0        0     4076 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/src/label_noise_correction/stc.py
+-rwxr-xr-x   0        0        0     3238 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1099 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0     3501 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/README.md
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 label_noise_correction-0.0.4/PKG-INFO
```

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/be.py` & `label_noise_correction-0.0.4/src/label_noise_correction/be.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/cc.py` & `label_noise_correction-0.0.4/src/label_noise_correction/cc.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/fair_obnc.py` & `label_noise_correction-0.0.4/src/label_noise_correction/fair_obnc.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,108 +46,87 @@
     m : float
         Proportion of labels to correct
     sensitive_attr : str
         Name of sensitive attribute
     prob : float
         Probability of correcting a label that does not contribute to balancing label distribution across sensitive groups
     """
-    def __init__(self, m:float, sensitive_attr:str, prob:float):
+    def __init__(self, m:float, sensitive_attr:str):
         super().__init__('Fair-OBNC-dp', m)
         self.sensitive_attr = sensitive_attr
-        self.prob = prob
 
     def dem_par_diff(self, X, y, attr):
         p_y1_g1 = len(y.loc[(X[attr] == 1) & (y == 1)]) / len(y.loc[X[attr] == 1])
         p_y1_g0 = len(y.loc[(X[attr] == 0) & (y == 1)]) / len(y.loc[X[attr] == 0])
 
         return p_y1_g1 - p_y1_g0
+    
+    def fair_correction(self, X, y, y_pred, margins):
+        y_corrected = y.copy()
+
+        n = int(self.m*len(margins))
+        corrected = 0
+
+        for i in margins.index:
+            dem_par = self.dem_par_diff(X, y, self.sensitive_attr)
+            if X.loc[i, self.sensitive_attr] == 0 and y.loc[i] == int(dem_par < 0):
+                y_corrected.loc[i] = y_pred.loc[i]
+                corrected += 1
+            elif X.loc[i, self.sensitive_attr] == 1 and y.loc[i] == int(dem_par > 0):
+                y_corrected.loc[i] = y_pred.loc[i]
+                corrected += 1
+            elif dem_par == 0:
+                y_corrected.loc[i] = y_pred.loc[i]
+                corrected += 1
+            
+            if corrected == n:
+                break
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
         y_corrected = y.copy()
 
         bagging = BaggingClassifier(n_estimators=100, random_state=42).fit(X, y)
         y_pred = pd.Series(bagging.predict(X), index=y.index)
 
         margins = self.calculate_margins(X.loc[y != y_pred], y.loc[y != y_pred], bagging).apply(lambda x: abs(x)).sort_values(ascending=False)
 
-        dem_par = self.dem_par_diff(X, y, self.sensitive_attr)
-        n = int(self.m*len(margins))
-
-        if dem_par == 0:
-            y_corrected.loc[margins.index[:n]] = [(1 - y.loc[i]) for i in margins.index[:n]]
-
-        else:
-            corrected = 0
-            for i in margins.index:
-                if X.loc[i, self.sensitive_attr] == 0:
-                    if y.loc[i] == int(dem_par < 0) or np.random.random() < self.prob:
-                        y_corrected.loc[i] = y_pred.loc[i]
-                        corrected += 1
-                else:
-                    if y.loc[i] == int(dem_par > 0) or np.random.random() < self.prob:
-                        y_corrected.loc[i] =  y_pred.loc[i]
-                        corrected += 1
-                
-                if corrected == n:
-                    break
+        y_corrected = self.fair_correction(X, y, y_pred, margins)
 
         return y_corrected
     
     def log_params(self):
         mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
         mlflow.log_param('sensitive_attr', self.sensitive_attr)
-        mlflow.log_param('prob', self.prob)
 
 class FairOBNC(FairOBNCOptimizeDemographicParity):
     """
     Fair Ordering-Based Correction algorithm (Fair-OBNC)
 
     Attributes
     ----------
     m : float
         Proportion of labels to correct
     sensitive_attr : str
         Name of sensitive attribute
     prob : float
         Probability of correcting a label that does not contribute to balancing label distribution across sensitive groups
     """
-    def __init__(self, m:float, sensitive_attr:str, prob:float):
-        super().__init__('Fair-OBNC', m, sensitive_attr, prob)
+    def __init__(self, m:float, sensitive_attr:str):
+        super().__init__('Fair-OBNC', m, sensitive_attr)
 
     def correct(self, X:pd.DataFrame, y:pd.Series):
-        y_corrected = y.copy()
         X_fair = X.drop(columns=self.sensitive_attr)
 
         bagging = BaggingClassifier(n_estimators=100, random_state=42).fit(X_fair, y)
         y_pred = pd.Series(bagging.predict(X_fair), index=y.index)
 
         margins = self.calculate_margins(X_fair.loc[y != y_pred], y.loc[y != y_pred], bagging).apply(lambda x: abs(x)).sort_values(ascending=False)
 
-        dem_par = self.dem_par_diff(X, y, self.sensitive_attr)
-        n = int(self.m*len(margins))
-
-        if dem_par == 0:
-            y_corrected.loc[margins.index[:n]] = [(1 - y.loc[i]) for i in margins.index[:n]]
-
-        else:
-            corrected = 0
-            for i in margins.index:
-                if X.loc[i, self.sensitive_attr] == 0:
-                    if y.loc[i] == int(dem_par < 0) or np.random.random() < self.prob:
-                        y_corrected.loc[i] = y_pred.loc[i]
-                        corrected += 1
-                else:
-                    if y.loc[i] == int(dem_par > 0) or np.random.random() < self.prob:
-                        y_corrected.loc[i] =  y_pred.loc[i]
-                        corrected += 1
-                
-                if corrected == n:
-                    break
+        y_corrected = self.fair_correction(X, y, y_pred, margins)
 
         return y_corrected
     
     def log_params(self):
         mlflow.log_param('correction_alg', self.name)
         mlflow.log_param('m', self.m)
-        mlflow.log_param('sensitive_attr', self.sensitive_attr)
-        mlflow.log_param('prob', self.prob)
+        mlflow.log_param('sensitive_attr', self.sensitive_attr)
```

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/hlnc.py` & `label_noise_correction-0.0.4/src/label_noise_correction/hlnc.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/labelcorrection.py` & `label_noise_correction-0.0.4/src/label_noise_correction/labelcorrection.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/obnc.py` & `label_noise_correction-0.0.4/src/label_noise_correction/obnc.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/pl.py` & `label_noise_correction-0.0.4/src/label_noise_correction/pl.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/src/label_noise_correction/stc.py` & `label_noise_correction-0.0.4/src/label_noise_correction/stc.py`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/.gitignore` & `label_noise_correction-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/LICENSE` & `label_noise_correction-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/README.md` & `label_noise_correction-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `label_noise_correction-0.0.3/pyproject.toml` & `label_noise_correction-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "label_noise_correction"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Inês Silva", email="inesoliveiraesilva@gmail.com" },
 ]
 description = "Label Noise Correction Methods"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `label_noise_correction-0.0.3/PKG-INFO` & `label_noise_correction-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: label_noise_correction
-Version: 0.0.3
+Version: 0.0.4
 Summary: Label Noise Correction Methods
 Project-URL: Homepage, https://github.com/reluzita/label-noise-correction
 Author-email: Inês Silva <inesoliveiraesilva@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

