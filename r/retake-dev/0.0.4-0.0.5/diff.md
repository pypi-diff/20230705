# Comparing `tmp/retake_dev-0.0.4.tar.gz` & `tmp/retake_dev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake_dev-0.0.4.tar", last modified: Tue Jul  4 18:34:28 2023, max compression
+gzip compressed data, was "retake_dev-0.0.5.tar", last modified: Tue Jul  4 18:39:15 2023, max compression
```

## Comparing `retake_dev-0.0.4.tar` & `retake_dev-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,35 @@
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.320221 retake_dev-0.0.4/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:34:28.320106 retake_dev-0.0.4/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     1454 2023-07-03 18:27:36.000000 retake_dev-0.0.4/README.md
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.317884 retake_dev-0.0.4/cdc/
--rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.4/cdc/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     3052 2023-07-04 17:10:36.000000 retake_dev-0.0.4/cdc/consumer_postgres.py
--rw-r--r--   0 mingying   (501) staff       (20)    16136 2023-07-03 18:27:36.000000 retake_dev-0.0.4/cdc/pgoutput.py
--rw-r--r--   0 mingying   (501) staff       (20)      691 2023-07-04 17:12:53.000000 retake_dev-0.0.4/cdc/run.py
--rw-r--r--   0 mingying   (501) staff       (20)     3872 2023-07-04 17:12:53.000000 retake_dev-0.0.4/cdc/source_postgres.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.318873 retake_dev-0.0.4/client/
--rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/__init__.py
--rw-r--r--   0 mingying   (501) staff       (20)     1914 2023-07-04 18:10:57.000000 retake_dev-0.0.4/client/collection.py
--rw-r--r--   0 mingying   (501) staff       (20)      235 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/embedding.py
--rw-r--r--   0 mingying   (501) staff       (20)      384 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/source.py
--rw-r--r--   0 mingying   (501) staff       (20)      752 2023-07-04 18:01:08.000000 retake_dev-0.0.4/client/transform.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319085 retake_dev-0.0.4/core/
--rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.4/core/__init__.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319178 retake_dev-0.0.4/interface/
--rw-r--r--   0 mingying   (501) staff       (20)      214 2023-07-03 18:27:13.000000 retake_dev-0.0.4/interface/__init__.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319917 retake_dev-0.0.4/retake_dev.egg-info/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)      405 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/SOURCES.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/dependency_links.txt
--rw-r--r--   0 mingying   (501) staff       (20)       32 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/requires.txt
--rw-r--r--   0 mingying   (501) staff       (20)       26 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/top_level.txt
--rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 18:34:28.320259 retake_dev-0.0.4/setup.cfg
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.285340 retake_dev-0.0.5/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:39:15.285236 retake_dev-0.0.5/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     1454 2023-07-03 18:27:36.000000 retake_dev-0.0.5/README.md
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.282104 retake_dev-0.0.5/cdc/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.5/cdc/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3052 2023-07-04 17:10:36.000000 retake_dev-0.0.5/cdc/consumer_postgres.py
+-rw-r--r--   0 mingying   (501) staff       (20)    16136 2023-07-03 18:27:36.000000 retake_dev-0.0.5/cdc/pgoutput.py
+-rw-r--r--   0 mingying   (501) staff       (20)      691 2023-07-04 17:12:53.000000 retake_dev-0.0.5/cdc/run.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3872 2023-07-04 17:12:53.000000 retake_dev-0.0.5/cdc/source_postgres.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.283105 retake_dev-0.0.5/client/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:13.000000 retake_dev-0.0.5/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1914 2023-07-04 18:10:57.000000 retake_dev-0.0.5/client/collection.py
+-rw-r--r--   0 mingying   (501) staff       (20)      235 2023-07-03 18:27:13.000000 retake_dev-0.0.5/client/embedding.py
+-rw-r--r--   0 mingying   (501) staff       (20)      384 2023-07-03 18:27:13.000000 retake_dev-0.0.5/client/source.py
+-rw-r--r--   0 mingying   (501) staff       (20)      752 2023-07-04 18:01:08.000000 retake_dev-0.0.5/client/transform.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.283328 retake_dev-0.0.5/core/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.5/core/__init__.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.283537 retake_dev-0.0.5/core/extract/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-04 18:36:59.000000 retake_dev-0.0.5/core/extract/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1491 2023-07-04 18:04:32.000000 retake_dev-0.0.5/core/extract/postgres.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.283911 retake_dev-0.0.5/core/load/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-04 18:37:03.000000 retake_dev-0.0.5/core/load/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      315 2023-07-03 18:27:36.000000 retake_dev-0.0.5/core/load/opensearch.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.284246 retake_dev-0.0.5/core/transform/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-04 18:37:08.000000 retake_dev-0.0.5/core/transform/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)      263 2023-07-03 18:27:36.000000 retake_dev-0.0.5/core/transform/embedding.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.284485 retake_dev-0.0.5/interface/
+-rw-r--r--   0 mingying   (501) staff       (20)      214 2023-07-03 18:27:13.000000 retake_dev-0.0.5/interface/__init__.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:39:15.285083 retake_dev-0.0.5/retake_dev.egg-info/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:39:15.000000 retake_dev-0.0.5/retake_dev.egg-info/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)      556 2023-07-04 18:39:15.000000 retake_dev-0.0.5/retake_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 18:39:15.000000 retake_dev-0.0.5/retake_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       32 2023-07-04 18:39:15.000000 retake_dev-0.0.5/retake_dev.egg-info/requires.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       26 2023-07-04 18:39:15.000000 retake_dev-0.0.5/retake_dev.egg-info/top_level.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 18:39:15.285379 retake_dev-0.0.5/setup.cfg
```

### Comparing `retake_dev-0.0.4/README.md` & `retake_dev-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/cdc/consumer_postgres.py` & `retake_dev-0.0.5/cdc/consumer_postgres.py`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/cdc/pgoutput.py` & `retake_dev-0.0.5/cdc/pgoutput.py`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/cdc/run.py` & `retake_dev-0.0.5/cdc/run.py`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/cdc/source_postgres.py` & `retake_dev-0.0.5/cdc/source_postgres.py`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/client/collection.py` & `retake_dev-0.0.5/client/collection.py`

 * *Files identical despite different names*

### Comparing `retake_dev-0.0.4/client/transform.py` & `retake_dev-0.0.5/client/transform.py`

 * *Files identical despite different names*

