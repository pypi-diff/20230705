# Comparing `tmp/pyEasyML-1.0.3.tar.gz` & `tmp/pyEasyML-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEasyML-1.0.3.tar", last modified: Thu Jun  1 20:42:23 2023, max compression
+gzip compressed data, was "pyEasyML-1.0.4.tar", last modified: Wed Jul  5 15:41:31 2023, max compression
```

## Comparing `pyEasyML-1.0.3.tar` & `pyEasyML-1.0.4.tar`

### file list

```diff
@@ -1,73 +1,70 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML/Classification/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5653 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Classifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Factory.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Classification/Models/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/AbstractModel.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/GradientBoostingClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/IsolationForest.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/KMeans.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/KNeighborsClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/LogisticRegression.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/RandomForestClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/SVC.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/XGBClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/Models/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/SearchModelsBestParams.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Classification/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Configs/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Configs/Config.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Configs/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Customize/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      858 2023-06-01 20:39:47.000000 pyEasyML-1.0.3/pyEasyML/Customize/Extension.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      687 2023-06-01 20:34:10.000000 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:33:28.000000 pyEasyML-1.0.3/pyEasyML/Customize/InPlace/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Customize/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Data/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6785 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Data/DataPreprocessing.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Data/FeatureSelection.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Data/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Email/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Email/Email.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Email/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AbstractANN.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/Layers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/NeuralNetworks/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/OutlierDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/OutlierDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Regression/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Regression/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/pyEasyML/Utils/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Utils/ColumnsToID.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Utils/Singleton.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/Utils/Threshold.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.3/pyEasyML/Utils/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.3/pyEasyML/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 17:42:38.000000 pyEasyML-1.0.3/pyEasyML/pyEasyMLcli.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 20:42:23.181947 pyEasyML-1.0.3/pyEasyML.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2049 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/entry_points.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-06-01 20:42:23.000000 pyEasyML-1.0.3/pyEasyML.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-01 20:42:23.185946 pyEasyML-1.0.3/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-06-01 20:41:50.000000 pyEasyML-1.0.3/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Classification/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     7288 2023-06-13 23:48:43.000000 pyEasyML-1.0.4/pyEasyML/Classification/Classifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Factory.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Classification/Models/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/AbstractModel.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/GradientBoostingClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/IsolationForest.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/KMeans.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/KNeighborsClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/LogisticRegression.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/RandomForestClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/SVC.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/XGBClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-06-13 23:22:44.000000 pyEasyML-1.0.4/pyEasyML/Classification/SearchModelsBestParams.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Configs/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Configs/Config.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Configs/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Customize/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2237 2023-07-05 15:38:07.000000 pyEasyML-1.0.4/pyEasyML/Customize/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Customize/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Data/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6304 2023-07-05 15:36:05.000000 pyEasyML-1.0.4/pyEasyML/Data/DataPreprocessing.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Data/FeatureSelection.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Data/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Email/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Email/Email.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Email/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AbstractANN.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/Layers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/OutlierDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/OutlierDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Regression/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Regression/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Utils/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Utils/ColumnsToID.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Utils/Singleton.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Utils/Threshold.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Utils/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/pyEasyMLcli.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1970 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/entry_points.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-07-05 15:41:22.000000 pyEasyML-1.0.4/setup.py
```

### Comparing `pyEasyML-1.0.3/LICENSE` & `pyEasyML-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/PKG-INFO` & `pyEasyML-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Factory.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/AbstractModel.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/AbstractModel.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/GradientBoostingClassifier.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/IsolationForest.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/IsolationForest.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/KMeans.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/KMeans.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/KNeighborsClassifier.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/LogisticRegression.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/RandomForestClassifier.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/SVC.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/SVC.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/Models/XGBClassifier.py` & `pyEasyML-1.0.4/pyEasyML/Classification/Models/XGBClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Classification/SearchModelsBestParams.py` & `pyEasyML-1.0.4/pyEasyML/Classification/SearchModelsBestParams.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Configs/Config.py` & `pyEasyML-1.0.4/pyEasyML/Configs/Config.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Data/DataPreprocessing.py` & `pyEasyML-1.0.4/pyEasyML/Data/DataPreprocessing.py`

 * *Files 23% similar despite different names*

```diff
@@ -70,52 +70,44 @@
             for dataset_path in dataset_paths:
                 dataset = self.read_dataset(dataset_path)
                 datasets.append(dataset)
             
             datasets = tuple(datasets)
             
             dataset = self.concat_datasets(*datasets)
-
-            dataset, = self.clean_dataset(dataset)
             
             dataset.to_parquet(all_data_path)
         
         return dataset
 
     def concat_datasets(self, *datasets:pd.DataFrame) -> pd.DataFrame:
 
         return pd.concat(datasets, ignore_index=True)
 
     def get_train_val_test_datasets(self) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
         raw_dataset = self.read_dataset(self.DATASET_PATH)
-        cleaned_dataset, = self.clean_dataset(raw_dataset)
 
         #Shuffle the dataframe
-        cleaned_dataset = cleaned_dataset.sample(frac=1, random_state=self._config.RANDOM_STATE)
+        raw_dataset = raw_dataset.sample(frac=1, random_state=self._config.RANDOM_STATE)
 
-        len_data = len(cleaned_dataset)
+        len_data = len(raw_dataset)
 
-        train_val_dataset = cleaned_dataset[:int(len_data*0.8)]
-        test_dataset = cleaned_dataset[int(len_data*0.8):]
+        train_val_dataset = raw_dataset[:int(len_data*0.8)]
+        test_dataset = raw_dataset[int(len_data*0.8):]
 
         return train_val_dataset, test_dataset
 
-    def clean_dataset(self, *dfs:pd.DataFrame) -> tuple[pd.DataFrame, ...]:
+    def clean_dataset(self, *dfs:tuple[pd.DataFrame]) -> tuple[pd.DataFrame, ...]:
         # CLEAN THE DATASET HERE.
-        aux_list = []
-        for df in dfs:
-            df = df.apply(pd.to_numeric, errors='coerce')
-            df = df.select_dtypes(include=['number'])
-            df = self.handle_missing_values(df)
-            aux_list.append(df)
-        dfs = tuple(aux_list)
 
         return dfs
 
     def handle_missing_values(self, dataset:pd.DataFrame) -> pd.DataFrame:
+        # HANDLE MISSING VALUES HERE.
+        
         X = dataset.columns.to_list()
         for x in X:
             if dataset[x].isna().all():
                 dataset.drop(labels=[x], axis=1, inplace=True)
             elif dataset[x].isna().any():
                 dataset[x] = dataset[x].fillna(dataset[x].mean())
 
@@ -137,15 +129,15 @@
             X = dataset[columns]
         Y = dataset[target_column]
 
         X_train, X_test, Y_train, Y_test = sklearn.model_selection.train_test_split(
             X.to_numpy(), 
             Y.to_numpy(), 
             test_size=0.3, 
-            #shuffle=True, #Shuffle is already done in the clean_dataset function. 
+            shuffle=True,
             random_state=self._config.RANDOM_STATE
         )
 
         X_train, X_test = self.normalize_data([X_train, X_test], columns)
 
         return X_train, X_test, Y_train, Y_test
 
@@ -168,21 +160,20 @@
         else:
             scaler = self.fit_standard_scaler(columns)
 
         return scaler
 
     def fit_standard_scaler(self, columns:list[str]) -> sklearn.preprocessing.StandardScaler:
         raw_dataset = self.read_dataset(self.DATASET_PATH)
-        cleaned_dataset, = self.clean_dataset(raw_dataset)
 
-        cleaned_dataset = cleaned_dataset[columns]
-        cleaned_dataset = cleaned_dataset.to_numpy()
+        raw_dataset = raw_dataset[columns]
+        raw_dataset = raw_dataset.to_numpy()
 
         scaler = sklearn.preprocessing.StandardScaler()
-        scaler.fit(cleaned_dataset)
+        scaler.fit(raw_dataset)
 
         columns_id_str = self._columns_to_id.convert_columns_to_id(*columns)
         path = os.path.join(self._config.get_normalization_model_path(), f'scaler_{columns_id_str}.sav')
         pickle.dump(scaler, open(path, 'wb'))
 
         return scaler
```

### Comparing `pyEasyML-1.0.3/pyEasyML/Data/FeatureSelection.py` & `pyEasyML-1.0.4/pyEasyML/Data/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Email/Email.py` & `pyEasyML-1.0.4/pyEasyML/Email/Email.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AbstractANN.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AbstractANN.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/NeuralNetworks/Layers/Layers.py` & `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/Layers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Utils/ColumnsToID.py` & `pyEasyML-1.0.4/pyEasyML/Utils/ColumnsToID.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Utils/Singleton.py` & `pyEasyML-1.0.4/pyEasyML/Utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/Utils/Threshold.py` & `pyEasyML-1.0.4/pyEasyML/Utils/Threshold.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/__init__.py` & `pyEasyML-1.0.4/pyEasyML/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML/pyEasyMLcli.py` & `pyEasyML-1.0.4/pyEasyML/pyEasyMLcli.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.3/pyEasyML.egg-info/PKG-INFO` & `pyEasyML-1.0.4/pyEasyML.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.3/pyEasyML.egg-info/SOURCES.txt` & `pyEasyML-1.0.4/pyEasyML.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 pyEasyML/Classification/Models/SVC.py
 pyEasyML/Classification/Models/XGBClassifier.py
 pyEasyML/Classification/Models/__init__.py
 pyEasyML/Configs/Config.py
 pyEasyML/Configs/__init__.py
 pyEasyML/Customize/Extension.py
 pyEasyML/Customize/__init__.py
-pyEasyML/Customize/InPlace/Extension.py
-pyEasyML/Customize/InPlace/__init__.py
 pyEasyML/Data/DataPreprocessing.py
 pyEasyML/Data/FeatureSelection.py
 pyEasyML/Data/__init__.py
 pyEasyML/Email/Email.py
 pyEasyML/Email/__init__.py
 pyEasyML/NeuralNetworks/AbstractANN.py
 pyEasyML/NeuralNetworks/__init__.py
```

### Comparing `pyEasyML-1.0.3/setup.py` & `pyEasyML-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'A python machine learning framework.'
 LONG_DESCRIPTION = 'A framework made to aid in the development of end-to-end machine learning projects, with data preprocessing, ml models, feature selection, hyperparameter tuning and much more.'
 
 # Setting up
 setup(
     name="pyEasyML",
     version=VERSION,
```

