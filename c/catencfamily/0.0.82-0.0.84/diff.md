# Comparing `tmp/catencfamily-0.0.82.tar.gz` & `tmp/catencfamily-0.0.84.tar.gz`

## Comparing `catencfamily-0.0.82.tar` & `catencfamily-0.0.84.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.82/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89750 2020-02-02 00:00:00.000000 catencfamily-0.0.82/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    43737 2020-02-02 00:00:00.000000 catencfamily-0.0.82/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.82/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.82/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.82/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.84/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89886 2020-02-02 00:00:00.000000 catencfamily-0.0.84/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    45236 2020-02-02 00:00:00.000000 catencfamily-0.0.84/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.84/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.84/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.84/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.84/PKG-INFO
```

### Comparing `catencfamily-0.0.82/src/catencfamily/encoders.py` & `catencfamily-0.0.84/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 29th June, 2023
+# 5th July, 2023
 """
 References:
 Coding standard:
     https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
     
 Developing sklearn estimators:
     https://scikit-learn.org/stable/developers/develop.html 
@@ -1784,17 +1784,20 @@
             # level; so take an average level-wise. Resulting grouped dataframe 
             # has cat col as index, but sorted.
             #-----
             # Expt:29th June, 2023
             r = t.copy()
             r['target'] = target
             #-----
-            r = r.groupby(by = [key], sort = True).mean()
+            yu = list(r[key])
+            r = r.groupby(by = yu, sort = True).mean()
+            #r = r.groupby(by = [key], sort = True).mean()
             # Get also index ('app') as one of the columns
-            r.reset_index(inplace = True)  
+            r.reset_index(inplace = True)
+            r=r.rename(columns = {'index' : key})
             if take_mean:
                 # Our vector dataframe is now ready
                 vec[key] = r
             else:
                 vec[key] = t
                 # Add target col also
                 vec[key]['target'] = target
```

### Comparing `catencfamily-0.0.82/src/catencfamily/utils.py` & `catencfamily-0.0.84/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-# 23th June, 2023
+# 4th July, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
+from sklear.cluster import KMeans
+from sklearn.mixture import GaussianMixture
 from sklearn.feature_selection import  mutual_info_classif
 import networkx as nx
 import itertools
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pathlib import Path
+import gc
 
 
 
 
 def xgImptFeatures(model, df_columns, filename = None, master=None):
     """
     Given an xgboost classifier model & data col
@@ -1338,11 +1341,62 @@
     """
     print(f"Datashape before processing: {df.shape}")
     df = df.loc[:, (df != df.iloc[0]).any()] 
     print(f"Datashape after processing: {df.shape}")
     return df
 
 
+
+def featureEngKmeans(train, test, n_clusters,step_size, km = True, gmm = True, random_state = 42):
+    """
+    Parameters
+    ----------
+    train : DataFrame
+    test : DataFrame
+    n_clusters : int; Number of clusters
+    step_size : int; No of cat_cols
+    km : boolean; Should features be generated through KMeans
+         Defaul.
+    gmm : boolean; Should features be generated through GMM
+    random_state : int;  The default is 42.
+
+    Returns
+    -------
+    tr : DataFrame
+    te : DataFrame
+    """
+    
+    if (not km and not gmm):
+        return train,test
+    
+    tr = train.copy()
+    te = test.copy()
+    label_tr = []
+    label_te = []
+    for i in range(0,tr.shape[1],step_size):
+      print("Current index: ", i)
+      if km:
+        km = KMeans(n_clusters = n_clusters,random_state = random_state)
+        _= km.fit_transform(tr.iloc[:, i:i+step_size].values.astype(np.float))
+        label_tr.append(km.labels_)
+        label_te.append(km.predict(te.iloc[:,i:i+step_size]))
+
+      if gmm:
+        gmm = GaussianMixture(n_components = n_clusters, random_state = random_state)
+        gmm.fit(tr) 
+        label_tr.append(gmm.predict(tr))
+        label_te.append(gmm.predict(te))
+
+      _=gc.collect()
+
+    for i in range(len(label_tr)):
+      tr['clu'+str(i)] = label_tr[i]
+      te['clu' + str(i)] = label_te[i] 
+
+    return tr,te
+
+
+
 ################### That's all folks #######################
```

### Comparing `catencfamily-0.0.82/LICENSE` & `catencfamily-0.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.82/README.md` & `catencfamily-0.0.84/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.82/pyproject.toml` & `catencfamily-0.0.84/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.82"
+version = "0.0.84"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.82/PKG-INFO` & `catencfamily-0.0.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.82
+Version: 0.0.84
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

