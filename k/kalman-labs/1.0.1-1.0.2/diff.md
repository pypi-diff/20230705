# Comparing `tmp/kalman-labs-1.0.1.tar.gz` & `tmp/kalman-labs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalman-labs-1.0.1.tar", last modified: Mon Jul  3 11:33:53 2023, max compression
+gzip compressed data, was "kalman-labs-1.0.2.tar", last modified: Wed Jul  5 17:03:44 2023, max compression
```

## Comparing `kalman-labs-1.0.1.tar` & `kalman-labs-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.594690 kalman-labs-1.0.1/
--rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.1/LICENSE
--rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-03 11:33:53.594561 kalman-labs-1.0.1/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.1/README.md
--rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-03 11:33:53.594739 kalman-labs-1.0.1/setup.cfg
--rw-r--r--   0 serverport   (501) staff       (20)      405 2023-07-03 11:33:47.000000 kalman-labs-1.0.1/setup.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.592320 kalman-labs-1.0.1/signal_processing_packages/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.592535 kalman-labs-1.0.1/signal_processing_packages/src/
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.593308 kalman-labs-1.0.1/signal_processing_packages/src/kalman/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman/__init__.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.593477 kalman-labs-1.0.1/signal_processing_packages/src/kalman/audio_features/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman/audio_features/__init__.py
--rw-r--r--   0 serverport   (501) staff       (20)     1644 2023-07-03 11:28:43.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman/audio_features/extract_features.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.593747 kalman-labs-1.0.1/signal_processing_packages/src/kalman/machine_learning_training/
--rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:10:12.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman/machine_learning_training/__init__.py
--rw-r--r--   0 serverport   (501) staff       (20)     1030 2023-07-03 07:29:24.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman/machine_learning_training/ml_training_script.py
-drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-03 11:33:53.594393 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/
--rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-03 11:33:53.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
--rw-r--r--   0 serverport   (501) staff       (20)      705 2023-07-03 11:33:53.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
--rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-03 11:33:53.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
--rw-r--r--   0 serverport   (501) staff       (20)       21 2023-07-03 11:33:53.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
--rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-03 11:33:53.000000 kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.089027 kalman-labs-1.0.2/
+-rw-r--r--   0 serverport   (501) staff       (20)     1067 2023-04-17 18:12:27.000000 kalman-labs-1.0.2/LICENSE
+-rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:03:44.088891 kalman-labs-1.0.2/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)       48 2023-04-17 18:12:27.000000 kalman-labs-1.0.2/README.md
+-rw-r--r--   0 serverport   (501) staff       (20)       38 2023-07-05 17:03:44.089083 kalman-labs-1.0.2/setup.cfg
+-rw-r--r--   0 serverport   (501) staff       (20)      513 2023-07-05 17:03:14.000000 kalman-labs-1.0.2/setup.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.086496 kalman-labs-1.0.2/signal_processing_packages/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.086664 kalman-labs-1.0.2/signal_processing_packages/src/
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.087702 kalman-labs-1.0.2/signal_processing_packages/src/kalman/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-05-13 14:42:55.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/__init__.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.088026 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/
+-rw-r--r--   0 serverport   (501) staff       (20)        0 2023-04-17 19:01:55.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/__init__.py
+-rw-r--r--   0 serverport   (501) staff       (20)     3598 2023-07-03 17:29:46.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/audio_features/extract_features.py
+-rw-r--r--   0 serverport   (501) staff       (20)    15256 2023-07-05 16:56:03.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/deep_learning_training.py
+-rw-r--r--   0 serverport   (501) staff       (20)     7404 2023-07-05 13:10:25.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman/machine_learning_training.py
+drwxr-xr-x   0 serverport   (501) staff       (20)        0 2023-07-05 17:03:44.088639 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/
+-rw-r--r--   0 serverport   (501) staff       (20)      158 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
+-rw-r--r--   0 serverport   (501) staff       (20)      674 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        1 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
+-rw-r--r--   0 serverport   (501) staff       (20)       76 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/requires.txt
+-rw-r--r--   0 serverport   (501) staff       (20)        7 2023-07-05 17:03:44.000000 kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
```

### Comparing `kalman-labs-1.0.1/LICENSE` & `kalman-labs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kalman-labs-1.0.1/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt` & `kalman-labs-1.0.2/signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 setup.py
 signal_processing_packages/src/kalman/__init__.py
+signal_processing_packages/src/kalman/deep_learning_training.py
+signal_processing_packages/src/kalman/machine_learning_training.py
 signal_processing_packages/src/kalman/audio_features/__init__.py
 signal_processing_packages/src/kalman/audio_features/extract_features.py
-signal_processing_packages/src/kalman/machine_learning_training/__init__.py
-signal_processing_packages/src/kalman/machine_learning_training/ml_training_script.py
 signal_processing_packages/src/kalman_labs.egg-info/PKG-INFO
 signal_processing_packages/src/kalman_labs.egg-info/SOURCES.txt
 signal_processing_packages/src/kalman_labs.egg-info/dependency_links.txt
 signal_processing_packages/src/kalman_labs.egg-info/requires.txt
 signal_processing_packages/src/kalman_labs.egg-info/top_level.txt
```

