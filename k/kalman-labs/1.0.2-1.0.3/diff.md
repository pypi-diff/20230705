# Comparing `tmp/kalman-labs-1.0.2.tar.gz` & `tmp/kalman-labs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalman-labs-1.0.2.tar", last modified: Wed Jul  5 17:03:44 2023, max compression
+gzip compressed data, was "kalman-labs-1.0.3.tar", last modified: Wed Jul  5 17:55:46 2023, max compression
```

## Comparing `kalman-labs-1.0.2.tar` & `kalman-labs-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.089027 kalman-labs-1.0.2/
--rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.2/LICENSE
--rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:03:44.088891 kalman-labs-1.0.2/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.2/README.md
--rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-05 17:03:44.089083 kalman-labs-1.0.2/setup.cfg
--rw-r--r--   0 serverport   (501) staff       (20)      513 2023-07-05 17:03:14.000000 kalman-labs-1.0.2/setup.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.086496 kalman-labs-1.0.2/signal_processing_packages/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.086664 kalman-labs-1.0.2/signal_processing_packages/src/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.087702 kalman-labs-1.0.2/signal_processing_packages/src/kalman/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/__init__.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.088026 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/__init__.py
--rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/extract_features.py
--rw-r--r--   0 serverport   (501) staff       (20)    15256 2023-07-05 16:56:03.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/deep_learning_training.py
--rw-r--r--   0 serverport   (501) staff       (20)     7404 2023-07-05 13:10:25.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/machine_learning_training.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.088639 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/
--rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
--rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
--rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
--rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.965111 kalman-labs-1.0.3/
+-rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.3/LICENSE
+-rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:55:46.964989 kalman-labs-1.0.3/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.3/README.md
+-rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-05 17:55:46.965153 kalman-labs-1.0.3/setup.cfg
+-rw-r--r--   0 serverport   (501) staff       (20)      513 2023-07-05 17:55:35.000000 kalman-labs-1.0.3/setup.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.962641 kalman-labs-1.0.3/signal_processing_packages/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.962800 kalman-labs-1.0.3/signal_processing_packages/src/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.963840 kalman-labs-1.0.3/signal_processing_packages/src/kalman/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman/__init__.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.964206 kalman-labs-1.0.3/signal_processing_packages/src/kalman/audio_features/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman/audio_features/__init__.py
+-rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman/audio_features/extract_features.py
+-rw-r--r--   0 serverport   (501) staff       (20)    15473 2023-07-05 17:50:33.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman/deep_learning_training.py
+-rw-r--r--   0 serverport   (501) staff       (20)     7633 2023-07-05 17:42:30.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman/machine_learning_training.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:55:46.964822 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/
+-rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:55:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-05 17:55:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-05 17:55:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
+-rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-05 17:55:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-05 17:55:46.000000 kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
```

### Comparing `kalman-labs-1.0.2/LICENSE` & `kalman-labs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.2/setup.py` & `kalman-labs-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kalman-labs',
-    version='1.0.2',
+    version='1.0.3',
     author='Aditya',
     author_email='aditya@kalman.in',
     description='The Global Kalman Package',
     packages=find_packages('signal_processing_packages/src'),
     package_dir={'': 'signal_processing_packages/src'},
     install_requires=[
         'numpy',
```

### Comparing `kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/extract_features.py` & `kalman-labs-1.0.3/signal_processing_packages/src/kalman/audio_features/extract_features.py`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.2/signal_processing_packages/src/kalman/deep_learning_training.py` & `kalman-labs-1.0.3/signal_processing_packages/src/kalman/deep_learning_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
-from signal_processing_packages.src.kalman.audio_features.extract_features import generate_feature_file
+from audio_features.extract_features import generate_feature_file
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import precision_score, recall_score
 from imblearn.over_sampling import SMOTE, ADASYN
 from imblearn.under_sampling import NearMiss
 
 import tensorflow as tf
 import keras
 from keras.models import Model
 from keras.layers import Input, Dense, Dropout, Reshape, Conv2D, ConvLSTM1D, AveragePooling2D, BatchNormalization, \
     Activation, Flatten, LSTM, Bidirectional
 from keras.utils import to_categorical
 
 
-def train_ml_model(ml_model, folder_path=None, x_train=None, y_train=None, x_val=None, y_val=None, scaler=None,
+def train_dl_model(dl_model, folder_path=None, x_train=None, y_train=None, x_val=None, y_val=None, scaler=None,
                    label_folder_map=None, testing=True, val_size=0.3, oversampling=None, undersampling=False,
                    batch_size=48, epochs=100):
     oversampler = None
     try:
         if folder_path is not None:
             assert x_train is None and y_train is None, "x_train and y_train must be None when folder_path is given"
             audio_df, label_name_dict = generate_feature_file(folder_path, scaler, label_folder_map)
@@ -30,25 +30,31 @@
                 raise ValueError("Both oversampling and undersampling cannot be enabled at the same time")
             if oversampling == "smote":
                 oversampler = SMOTE()
             elif oversampling == "adasyn":
                 oversampler = ADASYN()
             x_train, y_train = oversampler.fit_resample(x_train, y_train)
 
+            if x_val is not None and y_val is not None:
+                x_val, y_val = oversampler.fit_resample(x_val, y_val)
+
         if undersampling:
             if oversampling is not None:
                 raise ValueError("Both oversampling and undersampling cannot be enabled at the same time")
             undersampler = NearMiss(version=1, n_neighbors=3)
             x_train, y_train = undersampler.fit_resample(x_train, y_train)
 
+            if x_val is not None and y_val is not None:
+                x_val, y_val = undersampler.fit_resample(x_val, y_val)
+
         if x_val is None and y_val is None:
             x_train, x_val, y_train, y_val = train_test_split(x_train, y_train, test_size=val_size,
                                                               random_state=42)
 
-        results = train_model(ml_model, x_train, y_train, x_val, y_val, testing, batch_size, epochs)
+        results = train_model(dl_model, x_train, y_train, x_val, y_val, testing, batch_size, epochs)
         return results
 
     except Exception as e:
         return None, str(e)
 
 
 def train_model(dl_model, x_train, y_train, x_val, y_val, testing, batch_size, epochs):
```

### Comparing `kalman-labs-1.0.2/signal_processing_packages/src/kalman/machine_learning_training.py` & `kalman-labs-1.0.3/signal_processing_packages/src/kalman/machine_learning_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from signal_processing_packages.src.kalman.audio_features.extract_features import generate_feature_file
+from audio_features.extract_features import generate_feature_file
 from sklearn.model_selection import train_test_split, cross_val_score
 from sklearn.metrics import classification_report
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier, AdaBoostClassifier
 from sklearn.neural_network import MLPClassifier
@@ -27,20 +27,26 @@
                 raise ValueError("Both oversampling and undersampling cannot be enabled at the same time")
             if oversampling == "smote":
                 oversampler = SMOTE()
             elif oversampling == "adasyn":
                 oversampler = ADASYN()
             x_train, y_train = oversampler.fit_resample(x_train, y_train)
 
+            if x_test is not None and y_test is not None:
+                x_test, y_test = oversampler.fit_resample(x_test, y_test)
+
         if undersampling:
             if oversampling is not None:
                 raise ValueError("Both oversampling and undersampling cannot be enabled at the same time")
             undersampler = NearMiss(version=1, n_neighbors=3)
             x_train, y_train = undersampler.fit_resample(x_train, y_train)
 
+            if x_test is not None and y_test is not None:
+                x_test, y_test = undersampler.fit_resample(x_test, y_test)
+
         if testing:
             if folder_path is None:
                 assert x_train is not None and y_train is not None, "x_train and y_train must be provided when " \
                                                                     "testing is True and folder_path is None"
                 if x_test is None and y_test is None:
                     x_train, x_test, y_train, y_test = train_test_split(x_train, y_train, test_size=test_size,
                                                                         random_state=42)
```

### Comparing `kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt` & `kalman-labs-1.0.3/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

