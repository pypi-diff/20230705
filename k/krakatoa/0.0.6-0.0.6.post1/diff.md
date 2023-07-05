# Comparing `tmp/krakatoa-0.0.6.tar.gz` & `tmp/krakatoa-0.0.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.6.tar", last modified: Tue Jul  4 17:49:59 2023, max compression
+gzip compressed data, was "krakatoa-0.0.6.post1.tar", last modified: Wed Jul  5 18:18:26 2023, max compression
```

## Comparing `krakatoa-0.0.6.tar` & `krakatoa-0.0.6.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:49:59.703104 krakatoa-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 17:49:48.000000 krakatoa-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 17:49:59.703104 krakatoa-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-04 17:49:48.000000 krakatoa-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:49:59.699104 krakatoa-0.0.6/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:49:59.703104 krakatoa-0.0.6/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:49:59.703104 krakatoa-0.0.6/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-04 17:49:48.000000 krakatoa-0.0.6/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:49:59.699104 krakatoa-0.0.6/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-04 17:49:59.000000 krakatoa-0.0.6/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-04 17:49:59.000000 krakatoa-0.0.6/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:49:59.000000 krakatoa-0.0.6/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 17:49:59.000000 krakatoa-0.0.6/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 17:49:59.000000 krakatoa-0.0.6/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 17:49:59.703104 krakatoa-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 17:49:48.000000 krakatoa-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/future/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/future/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_getmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/krakatoa/models/quick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/krakatoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 18:18:26.000000 krakatoa-0.0.6.post1/krakatoa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 18:18:26.504647 krakatoa-0.0.6.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-05 18:18:12.000000 krakatoa-0.0.6.post1/setup.py
```

### Comparing `krakatoa-0.0.6/LICENSE` & `krakatoa-0.0.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/PKG-INFO` & `krakatoa-0.0.6.post1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6
+Version: 0.0.6.post1
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6/krakatoa/future/analysis.py` & `krakatoa-0.0.6.post1/krakatoa/future/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,54 +138,14 @@
                 try:
                     self.described[col]['dist'] = self.columnDist(col)
                 except:
                     self.described[col]['dist'] = {}
 
         return self.described
 
-    def diagnostic(self):
-        '''
-        Disclaimer!
-
-        This function returns some paremeters like -> 'missing', 'unique', 'target'
-
-        When those returns as False, means that they are not ok and need attention!
-        The True flag, means that there are no missing data, the target is solid or there are no unique columns!
-        '''
-
-        res_diagnostic = {'missing': True, 'unique': True, 'target': True}
-        # Check for missing data
-        null_data = self._nullPercFeatures()
-        null_diagnostic = null_data[null_data['count'] > 0][[
-            'variable', 'count']].to_dict('records')
-
-        if len(null_diagnostic) > 0:
-            null_diagnostic_items = {}
-            for item in null_diagnostic:
-                null_diagnostic_items[item['variable']] = item['count']
-            res_diagnostic['missing'] = False
-            res_diagnostic['missing_data'] = null_diagnostic_items
-
-        # Check for unique data
-        unique_data = self.dataset.nunique()
-        unique_diagnostic = unique_data[unique_data == 1].to_dict()
-
-        if len(unique_diagnostic.keys()) > 1:
-            res_diagnostic['unique'] = False
-            res_diagnostic['unique_data'] = unique_diagnostic
-
-        # Check for valid target
-        if self.target is None:
-            res_diagnostic['target'] = False
-        else:
-            if self.target not in set(self.dataset.columns):
-                res_diagnostic['target'] = False
-
-        return res_diagnostic
-
     def iqrOutliers(self, column: str, method: str = 'midpoint'):
 
         if column in self.numeric_cols:
             Q1 = np.percentile(self.dataset[column], 25, method=method)
             Q2 = np.percentile(self.dataset[column], 50, method=method)
             Q3 = np.percentile(self.dataset[column], 75, method=method)
             Q4 = np.percentile(self.dataset[column], 100, method=method)
@@ -226,14 +186,67 @@
             iqr_outliers = self.iqrOutliers(col, method)
 
             if iqr_outliers['has_outliers']:
                 outliers[col] = iqr_outliers
 
         return outliers
 
+    def diagnostic(self):
+        '''
+        Disclaimer!
+
+        This function returns some paremeters like -> 'missing', 'unique', 'target'
+
+        When those returns as False, means that they are not ok and need attention!
+        The True flag, means that there are no missing data, the target is solid or there are no unique columns!
+        '''
+
+        (rows, cols) = self.dataset.shape
+        res_diagnostic = {'missing': True, 'unique': True,
+                          'target': True, 'outliers': True, 'rows': rows, 'cols': cols}
+        
+        # Check for missing data
+        null_data = self._nullPercFeatures()
+        null_diagnostic = null_data[null_data['count'] > 0][[
+            'variable', 'count']].to_dict('records')
+
+        if len(null_diagnostic) > 0:
+            null_diagnostic_items = {}
+            for item in null_diagnostic:
+                null_diagnostic_items[item['variable']] = item['count']
+            res_diagnostic['missing'] = False
+            res_diagnostic['missing_data'] = null_diagnostic_items
+
+        # Check for unique data
+        unique_data = self.dataset.nunique()
+        unique_diagnostic = unique_data[unique_data == 1].to_dict()
+
+        if len(unique_diagnostic.keys()) > 1:
+            res_diagnostic['unique'] = False
+            res_diagnostic['unique_data'] = unique_diagnostic
+
+        # Check for valid target
+        if self.target is None:
+            res_diagnostic['target'] = False
+        else:
+            if self.target not in set(self.dataset.columns):
+                res_diagnostic['target'] = False
+
+        # Check for outliers
+        for col in self.dataset.columns:
+            try:
+                outliers = self.iqrOutliers(column=col)
+                if outliers['has_outliers']:
+                    res_diagnostic['outliers'] = False
+                    break
+            except:
+                pass
+
+        return res_diagnostic
+
     def columnInfo(self, column: str, get_values: bool = True, get_values_method: str = 'head',
                    get_values_size: int = 10, most_common_size: int = 2):
 
         info = {
             'type': str(),
             'values': list(),
             'stats': dict(),
```

### Comparing `krakatoa-0.0.6/krakatoa/future/evaluate.py` & `krakatoa-0.0.6.post1/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/future/experiment.py` & `krakatoa-0.0.6.post1/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/future/preprocess.py` & `krakatoa-0.0.6.post1/krakatoa/future/preprocess.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/models/_config.py` & `krakatoa-0.0.6.post1/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/models/_getmodels.py` & `krakatoa-0.0.6.post1/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/models/_metrics.py` & `krakatoa-0.0.6.post1/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/models/autotune.py` & `krakatoa-0.0.6.post1/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa/models/quick.py` & `krakatoa-0.0.6.post1/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/krakatoa.egg-info/PKG-INFO` & `krakatoa-0.0.6.post1/krakatoa.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krakatoa
-Version: 0.0.6
+Version: 0.0.6.post1
 Summary: Machine Learning high level package.
 Home-page: https://github.com/aitec-mp/krakatoa
-Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6.tar.gz
+Download-URL: https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz
 Author: Matheus de Prá Andrade
 Author-email: mpandrade@ucs.br
 License: MIT
 Keywords: krakatoa,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `krakatoa-0.0.6/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.6.post1/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.6/setup.py` & `krakatoa-0.0.6.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.6',      
+  version = '0.0.6post1',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
   long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.6post1.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
           'scikit-learn',
           'numpy',
           'pandas',
           'xgboost',
           'seaborn'
```

