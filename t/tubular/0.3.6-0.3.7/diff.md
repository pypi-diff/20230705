# Comparing `tmp/tubular-0.3.6.tar.gz` & `tmp/tubular-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubular-0.3.6.tar", last modified: Wed May 24 15:54:28 2023, max compression
+gzip compressed data, was "tubular-0.3.7.tar", last modified: Wed Jul  5 14:01:24 2023, max compression
```

## Comparing `tubular-0.3.6.tar` & `tubular-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-05-24 15:51:27.000000 tubular-0.3.6/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-05-24 15:54:28.985024 tubular-0.3.6/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2023-05-24 15:51:27.000000 tubular-0.3.6/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-05-24 15:54:28.985024 tubular-0.3.6/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1457 2023-05-24 15:51:27.000000 tubular-0.3.6/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.981024 tubular-0.3.6/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14672 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/test_data.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4876 2023-05-24 15:51:27.000000 tubular-0.3.6/tests/test_transformers.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/tubular/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      286 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/_version.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14927 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/base.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20028 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/capping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1985 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/comparison.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41786 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/dates.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13464 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/imputers.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17192 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/mapping.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2002 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/misc.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42279 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/nominal.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    30363 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/numeric.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6024 2023-05-24 15:51:27.000000 tubular-0.3.6/tubular/strings.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-05-24 15:54:28.985024 tubular-0.3.6/tubular.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-05-24 15:54:28.000000 tubular-0.3.6/tubular.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.760365 tubular-0.3.7/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1550 2023-07-05 13:47:51.000000 tubular-0.3.7/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-07-05 14:01:24.760365 tubular-0.3.7/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2023-07-05 13:47:51.000000 tubular-0.3.7/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-07-05 14:01:24.760365 tubular-0.3.7/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1457 2023-07-05 13:47:51.000000 tubular-0.3.7/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.748365 tubular-0.3.7/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14672 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/test_data.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4876 2023-07-05 13:47:51.000000 tubular-0.3.7/tests/test_transformers.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.756365 tubular-0.3.7/tubular/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      286 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       22 2023-07-05 14:00:40.000000 tubular-0.3.7/tubular/_version.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14927 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/base.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    20028 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/capping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1985 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/comparison.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    41786 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/dates.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13464 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/imputers.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17192 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/mapping.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2002 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/misc.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    42271 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/nominal.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    30363 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/numeric.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6024 2023-07-05 13:47:51.000000 tubular-0.3.7/tubular/strings.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-07-05 14:01:24.756365 tubular-0.3.7/tubular.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4335 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      470 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       40 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       14 2023-07-05 14:01:24.000000 tubular-0.3.7/tubular.egg-info/top_level.txt
```

### Comparing `tubular-0.3.6/LICENSE` & `tubular-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/PKG-INFO` & `tubular-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tubular-0.3.6/README.md` & `tubular-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/setup.py` & `tubular-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tests/test_data.py` & `tubular-0.3.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tests/test_transformers.py` & `tubular-0.3.7/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/base.py` & `tubular-0.3.7/tubular/base.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/capping.py` & `tubular-0.3.7/tubular/capping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/comparison.py` & `tubular-0.3.7/tubular/comparison.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/dates.py` & `tubular-0.3.7/tubular/dates.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/imputers.py` & `tubular-0.3.7/tubular/imputers.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/mapping.py` & `tubular-0.3.7/tubular/mapping.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/misc.py` & `tubular-0.3.7/tubular/misc.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/nominal.py` & `tubular-0.3.7/tubular/nominal.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from sklearn.preprocessing import OneHotEncoder
 
 from tubular.base import BaseTransformer
 from tubular.mapping import BaseMappingTransformMixin
 
 
 class BaseNominalTransformer(BaseTransformer):
-    """Base nominal transformer designed inherrited from for nominal transformers.
+    """Base Transformer extension for nominal transformers.
 
     Contains columns_set_or_check method which overrides the columns_set_or_check method in BaseTransformer if given
-    primacy in inheritance. The difference being that NominalColumnSetOrCheckMixin's columns_set_or_check only selects
+    primacy in inheritance. The difference being that BaseNominalTransformer's columns_set_or_check only selects
     object and categorical columns from X, if the columns attribute is not set by the user.
     """
 
     def columns_set_or_check(self, X):
         """Function to check or set columns attribute.
 
         If the columns attribute is None then set it to all object and category columns in X. Otherwise run the
@@ -432,15 +432,15 @@
         Returns
         -------
         X : pd.DataFrame
             Transformed input X with rare levels grouped for into a new rare level.
 
         """
 
-        X = super().transform(X)
+        X = BaseNominalTransformer.transform(self, X)
 
         self.check_is_fitted(["mapping_"])
 
         for c in self.columns:
 
             # for categorical dtypes have to set new category for the impute values first
             # and convert back to the categorical type, other it will convert to object
```

### Comparing `tubular-0.3.6/tubular/numeric.py` & `tubular-0.3.7/tubular/numeric.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular/strings.py` & `tubular-0.3.7/tubular/strings.py`

 * *Files identical despite different names*

### Comparing `tubular-0.3.6/tubular.egg-info/PKG-INFO` & `tubular-0.3.7/tubular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubular
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package to perform pre processing steps for machine learning models
 Author: LV GI Data Science Team
 Author-email: #DataSciencePackages@lv.co.uk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

