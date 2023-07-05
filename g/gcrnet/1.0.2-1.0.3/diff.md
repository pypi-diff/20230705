# Comparing `tmp/gcrnet-1.0.2.tar.gz` & `tmp/gcrnet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gcrnet-1.0.2.tar", last modified: Tue Jul  4 15:26:51 2023, max compression
+gzip compressed data, was "dist\gcrnet-1.0.3.tar", last modified: Wed Jul  5 13:49:58 2023, max compression
```

## Comparing `gcrnet-1.0.2.tar` & `gcrnet-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 15:26:51.577535 gcrnet-1.0.2/
--rw-rw-rw-   0        0        0     1084 2023-06-26 18:33:53.000000 gcrnet-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       88 2023-07-03 12:42:46.000000 gcrnet-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1532 2023-07-04 15:26:51.575559 gcrnet-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-07-04 14:25:43.000000 gcrnet-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 15:26:51.518630 gcrnet-1.0.2/gcrnet/
--rw-rw-rw-   0        0        0       26 2023-07-04 14:12:17.000000 gcrnet-1.0.2/gcrnet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:26:51.572138 gcrnet-1.0.2/gcrnet/__pycache__/
--rw-rw-rw-   0        0        0      191 2023-07-04 15:04:43.000000 gcrnet-1.0.2/gcrnet/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      191 2023-07-04 15:13:21.000000 gcrnet-1.0.2/gcrnet/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1647 2023-06-22 12:49:09.000000 gcrnet-1.0.2/gcrnet/__pycache__/base.cpython-38.pyc
--rw-rw-rw-   0        0        0    17271 2023-06-19 19:48:00.000000 gcrnet-1.0.2/gcrnet/__pycache__/crsdnn.cpython-38.pyc
--rw-rw-rw-   0        0        0    15795 2023-07-04 15:04:43.000000 gcrnet-1.0.2/gcrnet/__pycache__/gcrnet.cpython-38.pyc
--rw-rw-rw-   0        0        0    15807 2023-07-04 15:13:21.000000 gcrnet-1.0.2/gcrnet/__pycache__/gcrnet.cpython-39.pyc
--rw-rw-rw-   0        0        0    12820 2023-06-26 17:14:55.000000 gcrnet-1.0.2/gcrnet/__pycache__/gcrnn.cpython-38.pyc
--rw-rw-rw-   0        0        0     3014 2023-06-17 13:50:02.000000 gcrnet-1.0.2/gcrnet/__pycache__/io.cpython-38.pyc
--rw-rw-rw-   0        0        0     2226 2023-06-19 20:02:12.000000 gcrnet-1.0.2/gcrnet/__pycache__/layers.cpython-38.pyc
--rw-rw-rw-   0        0        0     1555 2023-06-22 14:49:35.000000 gcrnet-1.0.2/gcrnet/__pycache__/losses.cpython-38.pyc
--rw-rw-rw-   0        0        0     4911 2023-06-17 13:50:02.000000 gcrnet-1.0.2/gcrnet/__pycache__/matching.cpython-38.pyc
--rw-rw-rw-   0        0        0     1442 2023-06-22 15:45:30.000000 gcrnet-1.0.2/gcrnet/__pycache__/meter.cpython-38.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-22 15:52:03.000000 gcrnet-1.0.2/gcrnet/__pycache__/meters.cpython-38.pyc
--rw-rw-rw-   0        0        0     1627 2023-07-02 13:48:40.000000 gcrnet-1.0.2/gcrnet/__pycache__/mlp.cpython-38.pyc
--rw-rw-rw-   0        0        0     5659 2023-07-02 13:48:40.000000 gcrnet-1.0.2/gcrnet/__pycache__/models.cpython-38.pyc
--rw-rw-rw-   0        0        0     3803 2023-06-22 14:49:36.000000 gcrnet-1.0.2/gcrnet/__pycache__/penalty.cpython-38.pyc
--rw-rw-rw-   0        0        0     1109 2023-06-06 16:19:54.000000 gcrnet-1.0.2/gcrnet/__pycache__/simulate_data.cpython-38.pyc
--rw-rw-rw-   0        0        0    10786 2023-07-04 15:20:28.000000 gcrnet-1.0.2/gcrnet/__pycache__/utils.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-07-04 15:26:51.573716 gcrnet-1.0.2/gcrnet/datasets/
--rw-rw-rw-   0        0        0        0 2023-06-06 16:19:54.000000 gcrnet-1.0.2/gcrnet/datasets/__init__.py
--rw-rw-rw-   0        0        0    21643 2023-07-03 14:51:59.000000 gcrnet-1.0.2/gcrnet/gcrnet.py
--rw-rw-rw-   0        0        0     1697 2023-06-22 14:44:51.000000 gcrnet-1.0.2/gcrnet/losses.py
--rw-rw-rw-   0        0        0     1347 2023-07-02 13:47:35.000000 gcrnet-1.0.2/gcrnet/mlp.py
--rw-rw-rw-   0        0        0     6649 2023-07-02 13:47:35.000000 gcrnet-1.0.2/gcrnet/models.py
--rw-rw-rw-   0        0        0     3759 2023-06-22 14:48:49.000000 gcrnet-1.0.2/gcrnet/penalty.py
--rw-rw-rw-   0        0        0     9643 2023-07-04 15:18:09.000000 gcrnet-1.0.2/gcrnet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:26:51.527639 gcrnet-1.0.2/gcrnet.egg-info/
--rw-rw-rw-   0        0        0     1532 2023-07-04 15:26:51.000000 gcrnet-1.0.2/gcrnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-07-04 15:26:51.000000 gcrnet-1.0.2/gcrnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 15:26:51.000000 gcrnet-1.0.2/gcrnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-04 15:26:51.000000 gcrnet-1.0.2/gcrnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-04 15:26:51.000000 gcrnet-1.0.2/gcrnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       77 2023-07-03 12:42:46.000000 gcrnet-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 15:26:51.578528 gcrnet-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-07-04 15:26:14.000000 gcrnet-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:49:58.801632 gcrnet-1.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-06-26 18:33:53.000000 gcrnet-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:42:46.000000 gcrnet-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3284 2023-07-05 13:49:58.800130 gcrnet-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3004 2023-07-05 13:45:27.000000 gcrnet-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 13:49:58.733309 gcrnet-1.0.3/gcrnet/
+-rw-rw-rw-   0        0        0       26 2023-07-04 14:12:17.000000 gcrnet-1.0.3/gcrnet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:49:58.795143 gcrnet-1.0.3/gcrnet/__pycache__/
+-rw-rw-rw-   0        0        0      191 2023-07-04 15:04:43.000000 gcrnet-1.0.3/gcrnet/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      191 2023-07-04 15:13:21.000000 gcrnet-1.0.3/gcrnet/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1647 2023-06-22 12:49:09.000000 gcrnet-1.0.3/gcrnet/__pycache__/base.cpython-38.pyc
+-rw-rw-rw-   0        0        0    17271 2023-06-19 19:48:00.000000 gcrnet-1.0.3/gcrnet/__pycache__/crsdnn.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15795 2023-07-04 15:04:43.000000 gcrnet-1.0.3/gcrnet/__pycache__/gcrnet.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15807 2023-07-04 15:13:21.000000 gcrnet-1.0.3/gcrnet/__pycache__/gcrnet.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12820 2023-06-26 17:14:55.000000 gcrnet-1.0.3/gcrnet/__pycache__/gcrnn.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3014 2023-06-17 13:50:02.000000 gcrnet-1.0.3/gcrnet/__pycache__/io.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2226 2023-06-19 20:02:12.000000 gcrnet-1.0.3/gcrnet/__pycache__/layers.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1555 2023-06-22 14:49:35.000000 gcrnet-1.0.3/gcrnet/__pycache__/losses.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4911 2023-06-17 13:50:02.000000 gcrnet-1.0.3/gcrnet/__pycache__/matching.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1442 2023-06-22 15:45:30.000000 gcrnet-1.0.3/gcrnet/__pycache__/meter.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-22 15:52:03.000000 gcrnet-1.0.3/gcrnet/__pycache__/meters.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1627 2023-07-02 13:48:40.000000 gcrnet-1.0.3/gcrnet/__pycache__/mlp.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5659 2023-07-02 13:48:40.000000 gcrnet-1.0.3/gcrnet/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3803 2023-06-22 14:49:36.000000 gcrnet-1.0.3/gcrnet/__pycache__/penalty.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1109 2023-06-06 16:19:54.000000 gcrnet-1.0.3/gcrnet/__pycache__/simulate_data.cpython-38.pyc
+-rw-rw-rw-   0        0        0    10786 2023-07-04 15:20:28.000000 gcrnet-1.0.3/gcrnet/__pycache__/utils.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-07-05 13:49:58.798135 gcrnet-1.0.3/gcrnet/datasets/
+-rw-rw-rw-   0        0        0        0 2023-06-06 16:19:54.000000 gcrnet-1.0.3/gcrnet/datasets/__init__.py
+-rw-rw-rw-   0        0        0    21643 2023-07-03 14:51:59.000000 gcrnet-1.0.3/gcrnet/gcrnet.py
+-rw-rw-rw-   0        0        0     1697 2023-06-22 14:44:51.000000 gcrnet-1.0.3/gcrnet/losses.py
+-rw-rw-rw-   0        0        0     1347 2023-07-02 13:47:35.000000 gcrnet-1.0.3/gcrnet/mlp.py
+-rw-rw-rw-   0        0        0     6649 2023-07-02 13:47:35.000000 gcrnet-1.0.3/gcrnet/models.py
+-rw-rw-rw-   0        0        0     3759 2023-06-22 14:48:49.000000 gcrnet-1.0.3/gcrnet/penalty.py
+-rw-rw-rw-   0        0        0     9643 2023-07-04 15:18:09.000000 gcrnet-1.0.3/gcrnet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:49:58.746295 gcrnet-1.0.3/gcrnet.egg-info/
+-rw-rw-rw-   0        0        0     3284 2023-07-05 13:49:58.000000 gcrnet-1.0.3/gcrnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-07-05 13:49:58.000000 gcrnet-1.0.3/gcrnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:49:58.000000 gcrnet-1.0.3/gcrnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-05 13:49:58.000000 gcrnet-1.0.3/gcrnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 13:49:58.000000 gcrnet-1.0.3/gcrnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       77 2023-07-03 12:42:46.000000 gcrnet-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:49:58.802125 gcrnet-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-07-05 13:49:51.000000 gcrnet-1.0.3/setup.py
```

### Comparing `gcrnet-1.0.2/LICENSE` & `gcrnet-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/base.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/crsdnn.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/crsdnn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/gcrnet.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/gcrnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/gcrnet.cpython-39.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/gcrnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/gcrnn.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/gcrnn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/io.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/io.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/layers.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/layers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/losses.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/losses.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/matching.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/matching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/meter.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/meter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/meters.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/meters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/mlp.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/mlp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/models.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/penalty.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/penalty.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/simulate_data.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/simulate_data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/__pycache__/utils.cpython-38.pyc` & `gcrnet-1.0.3/gcrnet/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/gcrnet.py` & `gcrnet-1.0.3/gcrnet/gcrnet.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/losses.py` & `gcrnet-1.0.3/gcrnet/losses.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/mlp.py` & `gcrnet-1.0.3/gcrnet/mlp.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/models.py` & `gcrnet-1.0.3/gcrnet/models.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/penalty.py` & `gcrnet-1.0.3/gcrnet/penalty.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet/utils.py` & `gcrnet-1.0.3/gcrnet/utils.py`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/gcrnet.egg-info/SOURCES.txt` & `gcrnet-1.0.3/gcrnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcrnet-1.0.2/setup.py` & `gcrnet-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='gcrnet',
-      version='1.0.2',
+      version='1.0.3',
       author="Bin Luo",
       author_email="bin.luo2@duke.edu",
       description="A Python library for sparse-input neural networks using group concave regularization",
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='MIT',
       packages=['gcrnet'],
```

