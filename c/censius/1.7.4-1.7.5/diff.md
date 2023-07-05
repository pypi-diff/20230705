# Comparing `tmp/censius-1.7.4.tar.gz` & `tmp/censius-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.7.4.tar", last modified: Wed Jun 28 11:55:18 2023, max compression
+gzip compressed data, was "censius-1.7.5.tar", last modified: Wed Jul  5 08:16:18 2023, max compression
```

## Comparing `censius-1.7.4.tar` & `censius-1.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.290827 censius-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-28 11:55:18.290827 censius-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-28 11:55:16.000000 censius-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-28 11:55:16.000000 censius-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:55:18.290827 censius-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-28 11:55:16.000000 censius-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.282827 censius-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.286827 censius-1.7.4/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/CensiusParent.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.286827 censius-1.7.4/src/censius/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.290827 censius-1.7.4/src/censius/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/UseCase.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-28 11:55:16.000000 censius-1.7.4/src/censius/nlp/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:55:18.286827 censius-1.7.4/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-28 11:55:18.000000 censius-1.7.4/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-28 11:55:18.000000 censius-1.7.4/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:55:18.000000 censius-1.7.4/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-28 11:55:18.000000 censius-1.7.4/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 11:55:18.000000 censius-1.7.4/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:16:18.746959 censius-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 08:16:15.000000 censius-1.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 08:16:15.000000 censius-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 08:16:18.746959 censius-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 08:16:15.000000 censius-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.734959 censius-1.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.738959 censius-1.7.5/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/CensiusParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-05 08:16:16.000000 censius-1.7.5/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/src/censius/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.746959 censius-1.7.5/src/censius/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/UseCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-05 08:16:15.000000 censius-1.7.5/src/censius/nlp/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:16:18.742959 censius-1.7.5/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 08:16:18.000000 censius-1.7.5/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.7.4/PKG-INFO` & `censius-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.4
+Version: 1.7.5
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.4/setup.py` & `censius-1.7.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.7.4",
+    version="1.7.5",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
     packages=["censius", "censius.nlp", "censius.ml"],
     install_requires=["requests", "jsonschema", "pandas", "numpy"],
```

### Comparing `censius-1.7.4/src/censius/CensiusParent.py` & `censius-1.7.5/src/censius/CensiusParent.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/ml/CensiusClient.py` & `censius-1.7.5/src/censius/ml/CensiusClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,16 @@
         response = requests.request(
             "POST",
             REGISTER_DATASET_URL(self.project_id),
             headers=headers,
             data=payload,
             files=files,
         )
-        os.remove(os.getcwd() + "/" + file_name)
+        if os.name != 'nt': 
+            os.remove(os.getcwd() + "/" + file_name)
 
         return response.json()
 
     ## Will be deprecated
     def process_model(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=process_model_schema)
```

### Comparing `censius-1.7.4/src/censius/ml/constants.py` & `censius-1.7.5/src/censius/ml/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/ml/schemas.py` & `censius-1.7.5/src/censius/ml/schemas.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/ml/utils.py` & `censius-1.7.5/src/censius/ml/utils.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/nlp/CensiusClient.py` & `censius-1.7.5/src/censius/nlp/CensiusClient.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/nlp/constants.py` & `censius-1.7.5/src/censius/nlp/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius/nlp/schema.py` & `censius-1.7.5/src/censius/nlp/schema.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.4/src/censius.egg-info/PKG-INFO` & `censius-1.7.5/src/censius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.4
+Version: 1.7.5
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.4/src/censius.egg-info/SOURCES.txt` & `censius-1.7.5/src/censius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

