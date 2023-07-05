# Comparing `tmp/pyEasyML-1.0.4.tar.gz` & `tmp/pyEasyML-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEasyML-1.0.4.tar", last modified: Wed Jul  5 15:41:31 2023, max compression
+gzip compressed data, was "pyEasyML-1.0.5.tar", last modified: Wed Jul  5 16:02:37 2023, max compression
```

## Comparing `pyEasyML-1.0.4.tar` & `pyEasyML-1.0.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Classification/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     7288 2023-06-13 23:48:43.000000 pyEasyML-1.0.4/pyEasyML/Classification/Classifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Factory.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Classification/Models/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/AbstractModel.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/GradientBoostingClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/IsolationForest.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/KMeans.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/KNeighborsClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/LogisticRegression.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/RandomForestClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/SVC.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/XGBClassifier.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/Models/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-06-13 23:22:44.000000 pyEasyML-1.0.4/pyEasyML/Classification/SearchModelsBestParams.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Classification/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML/Configs/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Configs/Config.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Configs/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Customize/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2237 2023-07-05 15:38:07.000000 pyEasyML-1.0.4/pyEasyML/Customize/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Customize/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Data/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6304 2023-07-05 15:36:05.000000 pyEasyML-1.0.4/pyEasyML/Data/DataPreprocessing.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Data/FeatureSelection.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Data/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Email/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Email/Email.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Email/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AbstractANN.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/Layers.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/NeuralNetworks/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/OutlierDetection/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/OutlierDetection/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Regression/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Regression/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/pyEasyML/Utils/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Utils/ColumnsToID.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Utils/Singleton.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/Utils/Threshold.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.4/pyEasyML/Utils/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.4/pyEasyML/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 17:42:38.000000 pyEasyML-1.0.4/pyEasyML/pyEasyMLcli.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 15:41:31.744323 pyEasyML-1.0.4/pyEasyML.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1970 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/entry_points.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-07-05 15:41:31.000000 pyEasyML-1.0.4/pyEasyML.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-07-05 15:41:31.748323 pyEasyML-1.0.4/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-07-05 15:41:22.000000 pyEasyML-1.0.4/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.504143 pyEasyML-1.0.5/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1083 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      344 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Classification/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     7288 2023-06-13 23:48:43.000000 pyEasyML-1.0.5/pyEasyML/Classification/Classifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1609 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Factory.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Classification/Models/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4031 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/AbstractModel.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      896 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/GradientBoostingClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3629 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/IsolationForest.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1153 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/KMeans.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      827 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/KNeighborsClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      817 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/LogisticRegression.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      778 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/RandomForestClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      623 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/SVC.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      844 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/XGBClassifier.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/Models/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1675 2023-06-13 23:22:44.000000 pyEasyML-1.0.5/pyEasyML/Classification/SearchModelsBestParams.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Classification/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Configs/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2666 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/pyEasyML/Configs/Config.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Configs/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Customize/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2237 2023-07-05 15:38:07.000000 pyEasyML-1.0.5/pyEasyML/Customize/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/pyEasyML/Customize/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Data/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6859 2023-07-05 16:02:11.000000 pyEasyML-1.0.5/pyEasyML/Data/DataPreprocessing.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     3692 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Data/FeatureSelection.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Data/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Email/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2802 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Email/Email.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Email/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2159 2023-05-31 04:12:00.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AbstractANN.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     5595 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1163 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      941 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     6614 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      383 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/ConvolutionalLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      783 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2092 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/Layers.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/NeuralNetworks/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/OutlierDetection/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/OutlierDetection/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Regression/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      326 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Regression/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML/Utils/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2623 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/pyEasyML/Utils/ColumnsToID.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Utils/Singleton.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2979 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/pyEasyML/Utils/Threshold.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-05-31 00:12:33.000000 pyEasyML-1.0.5/pyEasyML/Utils/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1282 2023-06-01 13:39:31.000000 pyEasyML-1.0.5/pyEasyML/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2727 2023-06-01 17:42:38.000000 pyEasyML-1.0.5/pyEasyML/pyEasyMLcli.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-05 16:02:37.500143 pyEasyML-1.0.5/pyEasyML.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      743 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1970 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       54 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/entry_points.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       46 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        9 2023-07-05 16:02:37.000000 pyEasyML-1.0.5/pyEasyML.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-07-05 16:02:37.504143 pyEasyML-1.0.5/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1192 2023-07-05 16:02:27.000000 pyEasyML-1.0.5/setup.py
```

### Comparing `pyEasyML-1.0.4/LICENSE` & `pyEasyML-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/PKG-INFO` & `pyEasyML-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Classifier.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Classifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Factory.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/AbstractModel.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/AbstractModel.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/GradientBoostingClassifier.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/GradientBoostingClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/IsolationForest.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/IsolationForest.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/KMeans.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/KMeans.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/KNeighborsClassifier.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/LogisticRegression.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/RandomForestClassifier.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/SVC.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/SVC.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/Models/XGBClassifier.py` & `pyEasyML-1.0.5/pyEasyML/Classification/Models/XGBClassifier.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Classification/SearchModelsBestParams.py` & `pyEasyML-1.0.5/pyEasyML/Classification/SearchModelsBestParams.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Configs/Config.py` & `pyEasyML-1.0.5/pyEasyML/Configs/Config.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Customize/Extension.py` & `pyEasyML-1.0.5/pyEasyML/Customize/Extension.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Data/DataPreprocessing.py` & `pyEasyML-1.0.5/pyEasyML/Data/DataPreprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,27 @@
             return pd.read_parquet(path)
         elif file_extension == ".xlsx":
             return pd.read_excel(path)
         # Add more conditions for other file formats if needed
         else:
             raise ValueError("Unsupported file extension: " + file_extension)    
 
+    def save_dataset(self, dataset:pd.DataFrame, path:str) -> None:
+        file_extension = os.path.splitext(path)[1].lower()
+    
+        if file_extension == ".csv":
+            dataset.to_csv(path, index=False)
+        elif file_extension == ".parquet":
+            dataset.to_parquet(path, index=False)
+        elif file_extension == ".xlsx":
+            dataset.to_excel(path, index=False)
+        # Add more conditions for other file formats if needed
+        else:
+            raise ValueError("Unsupported file extension: " + file_extension)   
+
     def read_all_data(self) -> pd.DataFrame:
         all_data_path = glob.glob(os.path.join(self._DATA_FOLDER_PATH, "all_data.*"))[0]
 
         if exists(all_data_path):
             print("Reading all_data.")
             return self.read_dataset(all_data_path)
         else:
```

### Comparing `pyEasyML-1.0.4/pyEasyML/Data/FeatureSelection.py` & `pyEasyML-1.0.5/pyEasyML/Data/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Email/Email.py` & `pyEasyML-1.0.5/pyEasyML/Email/Email.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AbstractANN.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AbstractANN.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/AnomalyDetector.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/AnomalyDetection/Factory.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/ConvolutionalAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Autoencoders/DeepAutoencoder.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/DeepAutoencoderLayers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/NeuralNetworks/Layers/Layers.py` & `pyEasyML-1.0.5/pyEasyML/NeuralNetworks/Layers/Layers.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Utils/ColumnsToID.py` & `pyEasyML-1.0.5/pyEasyML/Utils/ColumnsToID.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Utils/Singleton.py` & `pyEasyML-1.0.5/pyEasyML/Utils/Singleton.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/Utils/Threshold.py` & `pyEasyML-1.0.5/pyEasyML/Utils/Threshold.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/__init__.py` & `pyEasyML-1.0.5/pyEasyML/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML/pyEasyMLcli.py` & `pyEasyML-1.0.5/pyEasyML/pyEasyMLcli.py`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/pyEasyML.egg-info/PKG-INFO` & `pyEasyML-1.0.5/pyEasyML.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEasyML
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python machine learning framework.
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,AI,Machine Learning,Neural Networks
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyEasyML-1.0.4/pyEasyML.egg-info/SOURCES.txt` & `pyEasyML-1.0.5/pyEasyML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyEasyML-1.0.4/setup.py` & `pyEasyML-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'A python machine learning framework.'
 LONG_DESCRIPTION = 'A framework made to aid in the development of end-to-end machine learning projects, with data preprocessing, ml models, feature selection, hyperparameter tuning and much more.'
 
 # Setting up
 setup(
     name="pyEasyML",
     version=VERSION,
```

