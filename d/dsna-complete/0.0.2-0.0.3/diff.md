# Comparing `tmp/dsna_complete-0.0.2.tar.gz` & `tmp/dsna_complete-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.2.tar", last modified: Mon Jul  3 12:43:18 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.3.tar", last modified: Wed Jul  5 07:46:32 2023, max compression
```

## Comparing `dsna_complete-0.0.2.tar` & `dsna_complete-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.812575 dsna_complete-0.0.2/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:43:18.812630 dsna_complete-0.0.2/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.811417 dsna_complete-0.0.2/automl/
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.2/automl/__init__.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     1726 2023-06-08 03:05:14.000000 dsna_complete-0.0.2/automl/generate.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     9436 2023-07-03 12:40:48.000000 dsna_complete-0.0.2/automl/process.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     2739 2023-07-03 12:37:42.000000 dsna_complete-0.0.2/automl/test.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)    19852 2023-07-03 12:06:17.000000 dsna_complete-0.0.2/automl/train.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.809969 dsna_complete-0.0.2/base/
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.811776 dsna_complete-0.0.2/base/utils/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     3339 2023-07-03 11:35:14.000000 dsna_complete-0.0.2/base/utils/servant.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-03 12:43:18.812476 dsna_complete-0.0.2/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      326 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       17 2023-07-03 12:43:18.000000 dsna_complete-0.0.2/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.2/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      386 2023-07-03 12:43:18.812866 dsna_complete-0.0.2/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.2/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.999175 dsna_complete-0.0.3/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-05 07:46:31.999261 dsna_complete-0.0.3/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.996493 dsna_complete-0.0.3/automl/
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.3/automl/__init__.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.996592 dsna_complete-0.0.3/automl/preservice/
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.997330 dsna_complete-0.0.3/automl/preservice/VIP/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)     3461 2023-07-05 07:01:10.000000 dsna_complete-0.0.3/automl/preservice/VIP/eda.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)     6035 2023-07-05 07:29:39.000000 dsna_complete-0.0.3/automl/preservice/VIP/test.py
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)    19917 2023-07-05 07:16:53.000000 dsna_complete-0.0.3/automl/preservice/VIP/train.py
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)     1059 2023-07-05 07:29:48.000000 dsna_complete-0.0.3/automl/preservice/conclude.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.997866 dsna_complete-0.0.3/automl/utils/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)     3439 2023-07-05 07:01:33.000000 dsna_complete-0.0.3/automl/utils/operate.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.995946 dsna_complete-0.0.3/base/
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.998106 dsna_complete-0.0.3/base/utils/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)     3335 2023-07-05 07:06:34.000000 dsna_complete-0.0.3/base/utils/servant.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.999072 dsna_complete-0.0.3/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      402 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       17 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.3/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      371 2023-07-05 07:46:31.999563 dsna_complete-0.0.3/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.3/setup.py
```

### Comparing `dsna_complete-0.0.2/automl/generate.py` & `dsna_complete-0.0.3/automl/preservice/VIP/eda.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import string
 from math import ceil
+import string
 
-class Generate:
+class CreateRange:
 
-    def generate_numerical_ranges(self, numeric_variable, thresholds_list):
+    def create_numerical_ranges(self, numeric_variable, thresholds_list):
         ''' Create a list of ranges for numeric variable you want to categorize
 
             Parameters
             ----------
             numeric_variable: Series
                         Column of a DataFrame that contains numerical values that you want to categorize
             thresholds_list: List
@@ -20,15 +20,15 @@
             numerical_ranges_list.append(range(start, threshold))
             start = threshold
 
         numerical_ranges_list.append(range(threshold, final))
 
         return numerical_ranges_list
 
-    def generate_categorical_ranges(self, interval,start,finish):
+    def create_categorical_ranges(self, interval,start,finish):
         ''' Create a list of ranges for categorcial variable you want to categorzie
 
             Parameters
             ----------
             interval: int
                 Count of intervals to create
             start: int -- float
@@ -46,8 +46,61 @@
                 categorical_ranges_list.append(range(start, start+ diff))
             else:
                 categorical_ranges_list.append(range(start, ceil(1.5 * (start+diff))))
 
             start += diff
 
         return categorical_ranges_list
-    
+    
+class Categorize:
+    
+    def __init__(self):
+        self.letters = string.ascii_letters
+    
+    def categorize_numerical_variable(self, df_series, numerical_ranges_list):
+        ''' Returns a dictionary of categories with corresponding ranges 
+        
+            Parameters
+            ----------
+            df_series: Series
+                    Numerical variable series
+            numerical_ranges_list: List
+                    List of ranges for numerical values
+        '''
+        
+        letters = self.letters[:len(numerical_ranges_list)]
+        range_dict = dict(zip(letters, numerical_ranges_list))
+        category_dict = {}
+
+        for key, value in range_dict.items():
+            for data in  df_series.values:
+                if int(data) in value:
+                    category_dict[data] = key
+
+        return category_dict
+    
+    def categorize_categorical_variable(self, grouped_data, categorical_ranges_list):
+        ''' Returns a dictionary of categories with corresponding ranges 
+
+            Parameters
+            ----------
+            grouped_data: Series
+                    Series acquired after using groupby method
+            categorical_ranges_list: List
+                    List of ranges for categorical values
+        '''
+
+        letters = string.ascii_letters[:len(categorical_ranges_list)]
+        range_dict = dict(zip(letters, categorical_ranges_list))
+        category_dict = {}
+        for name, data in enumerate(grouped_data):
+            for key, value in range_dict.items():
+                if int(data) in value:
+                    category_dict[grouped_data.index[name]] = key
+
+        return category_dict
+    
+class DetectOutlier:
+    pass
+
+class AnalyzeError:
+    pass
```

### Comparing `dsna_complete-0.0.2/automl/train.py` & `dsna_complete-0.0.3/automl/preservice/VIP/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 from sklearn.model_selection import train_test_split
 
 import tensorflow as tf
 from tensorflow.keras.layers import Dense, Input
 from tensorflow.keras import Sequential
 
 
-from automl.process import Format, Preprocess
-from base.utils.servant import BaseFormat
+from automl.utils.operate import Process
+from automl.preservice.conclude import Preprocess
+from base.utils.servant import Format
 
 import pmdarima as pm
 from pmdarima import model_selection
 from prophet import Prophet
 
 import gc
 
-class Create:
+class CreateModel:
     
     def create_regression_model(self, algorithm, parameters = {}):
         """
         Create a regression model
 
         Parameters
         ----------
@@ -240,23 +241,23 @@
         if algorithm == 'AAR' : ts_model = pm.auto_arima(data, **parameters)
 
         if algorithm == 'PRH': ts_model = Prophet(**parameters)
         
         return ts_model
     
 
-class Include(Create, Format, Preprocess, BaseFormat):
+class IncludeModel(CreateModel, Process, Preprocess, Format):
 
     def include_feature_selection(self, model, key, model_object, X_train, X_test, y_train):
         """
         Apply feature selection on train and test values
         """
         selector_model = model[1] 
         selector_name = selector_model['feature_selection'][0]
-        selector_algorithm = self.format_algorithm_string(selector_name)
+        selector_algorithm = self.format_string_with_num(selector_name)
         selector_parameters = selector_model['feature_selection'][1]
 
         print(f'Selecting features with {selector_name} for {key}')
         feature_selector = self.create_feature_selection_model(model_object, selector_algorithm, selector_parameters)
 
         X_train_selected = feature_selector.fit_transform(X_train, y_train)
         X_test_selected = feature_selector.transform(X_test)
@@ -265,15 +266,15 @@
     
     def include_dimensionality_reduction(self, model, key, X_train, X_test, y_train):
         """
         Apply dimensionality reduction on train and test values
         """
         dimensionality_reduction_model = model[1] 
         dimensionality_reduction_name = dimensionality_reduction_model['dimensionality_reduction'][0]
-        dimensionality_reduction_algorithm = self.format_algorithm_string(dimensionality_reduction_name)
+        dimensionality_reduction_algorithm = self.format_string_with_num(dimensionality_reduction_name)
         dimensionality_reduction_parameters = dimensionality_reduction_model['dimensionality_reduction'][1]
         
 
         print(f'Reducing dimensions with {dimensionality_reduction_name} for {key}')
         
         dimensionality_reducer = self.create_dimensionality_reduction_model(dimensionality_reduction_algorithm, dimensionality_reduction_parameters)
         
@@ -288,15 +289,15 @@
             
         X_train_reduced = dimensionality_reducer.fit_transform(X_train)
         X_test_reduced = dimensionality_reducer.transform(X_test)
         
         return X_train_reduced, X_test_reduced, dimensionality_reduction_name
     
     
-class Build(Include):
+class BuildModel(IncludeModel):
     
     def __init__(self, test_dict, feature_selection=False, dimensionality_reduction=False):
         
         self.test_dict = test_dict
         self.test_dict['predictions'] = {}
         self.test_dict['models'] = {}
         self.test_dict['X_test'] = {}
@@ -318,16 +319,16 @@
             Name of the variable that model is going to predict
         """      
         for key, data in self.test_dict['data'].items():
             for model in models_list:
                 
                 X_train, X_test, y_train, y_test = self.preprocess_test_data(data, dependent_variable)
                 
-                model_name, parameters = self.format_models_list(model[0])
-                algorithm = self.format_algorithm_string(model_name)
+                model_name, parameters = self.process_models_list(model[0])
+                algorithm = self.format_string_with_num(model_name)
                 
                 # Dict names
                 label = key+model_name
                 
                 regressor = self.create_regression_model(algorithm , parameters)
                 
                 if self.feature_selection: 
@@ -367,16 +368,16 @@
             Name of the variable that model is going to predict
         """       
         for key, data in self.test_dict['data'].items():
             for model in models_list:
 
                 X_train, X_test, y_train, y_test = self.preprocess_test_data(data, dependent_variable)
 
-                model_name, parameters = self.format_models_list(model[0])
-                algorithm = self.format_algorithm_string(model_name)
+                model_name, parameters = self.process_models_list(model[0])
+                algorithm = self.format_string_with_num(model_name)
                 
                 # Dict names
                 label = key+model_name
                 
                 classifier = self.create_classification_model(algorithm , parameters)
                 
                 if self.feature_selection: 
@@ -423,22 +424,22 @@
         for key, data in self.test_dict['data'].items():
             
         
             for model in models_list:
                 
                 X_train, X_test, y_train, y_test = self.preprocess_test_data(data, dependent_variable)
                 
-                model_name, layers, compile_parameters, fit_parameters = self.format_models_list(model[0])
-                kind = self.format_algorithm_string(model_name)
+                model_name, layers, compile_parameters, fit_parameters = self.process_models_list(model[0])
+                kind = self.format_string_with_num(model_name)
                 
                 # Dict names
                 label = key+model_name
                 
                 #Create NN 
-                layers = self.format_input_layer(layers, X_train)
+                layers = self.process_input_layer(layers, X_train)
                 nn = self.create_deep_learning_model(layers, compile_parameters)
                                 
                 if self.feature_selection: 
                     X_train_selected, X_test_selected, selector_name = self.include_feature_selection(model, key, nn, X_train, X_test, y_train)
                     X_train = X_train_selected
                     X_test = X_test_selected
                     label += selector_name
@@ -470,38 +471,38 @@
         ----------
         models_list: list
             List of time series models and parameters.
         """   
         for key, data in self.test_dict['data'].items():
             for model in models_list:
 
-                model_name, layers, parameters, test_size = self.format_models_list(model[0])
-                algorithm = self.format_algorithm_string(model_name) 
+                model_name, layers, parameters, test_size = self.process_models_list(model[0])
+                algorithm = self.format_string_with_num(model_name) 
                 
                 #Change columns names if algorithm is Prophet
                 if algorithm == 'PRH':
-                    data = self.format_prophet_data(data)
+                    data = self.process_prophet_data(data)
                     
                 train, test= self.preprocess_time_series_data(data, test_size)
     
                 # Dict names
                 label = key+model_name
                 
                 print(f'Creating time series model {model_name} for {key}')
                 ts_model = self.create_time_series_model(algorithm, data , parameters)
                 print('Model created!')
                 ts_model.fit(train)
                 
                 if algorithm == 'PRH':
                     #Drop y values from test dataframe to make future dataframe for Prophet.
                     predictions = ts_model.predict(test.drop('y', axis=1))
-                    predictions = self.format_prophet_predictions
+                    predictions = self.process_prophet_predictions
                     
                     #Format the test and train tables so index is datetime column
-                    train, test = self.format_prophet_index(train, test)
+                    train, test = self.process_prophet_index(train, test)
                 
                 else:
                     predictions = ts_model.predict(n_periods = test.shape[0])
 
                 self.test_dict['models'][label] = ts_model
                 self.test_dict['predictions'][label] = predictions
                 #Because there is no X - y split in time series, train is labeled as X_test and test is labeled as y_test.
```

### Comparing `dsna_complete-0.0.2/base/utils/servant.py` & `dsna_complete-0.0.3/base/utils/servant.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             order_is_correct = True
 
         else:
             order_is_correct = False
             
         return order_is_correct
 
-class BaseFormat:
+class Format:
     
     def format_passenger_string(self, passenger_string):
         
         formatted_passenger_string = passenger_string.split(',')[0]
         
         return formatted_passenger_string
```

