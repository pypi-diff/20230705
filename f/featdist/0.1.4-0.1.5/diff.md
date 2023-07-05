# Comparing `tmp/featdist-0.1.4.tar.gz` & `tmp/featdist-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featdist-0.1.4.tar", last modified: Wed Jan 11 08:01:20 2023, max compression
+gzip compressed data, was "featdist-0.1.5.tar", last modified: Wed Jul  5 07:36:40 2023, max compression
```

## Comparing `featdist-0.1.4.tar` & `featdist-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:01:20.070071 featdist-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-11 08:01:08.000000 featdist-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-11 08:01:20.070071 featdist-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-11 08:01:08.000000 featdist-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:01:20.070071 featdist-0.1.4/featdist/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-11 08:01:08.000000 featdist-0.1.4/featdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-01-11 08:01:08.000000 featdist-0.1.4/featdist/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:01:20.070071 featdist-0.1.4/featdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-11 08:01:20.000000 featdist-0.1.4/featdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-11 08:01:20.000000 featdist-0.1.4/featdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 08:01:20.000000 featdist-0.1.4/featdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-11 08:01:20.000000 featdist-0.1.4/featdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-11 08:01:20.000000 featdist-0.1.4/featdist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 08:01:20.070071 featdist-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-01-11 08:01:08.000000 featdist-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 07:36:26.000000 featdist-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 07:36:40.052848 featdist-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-05 07:36:26.000000 featdist-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/featdist/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 07:36:26.000000 featdist-0.1.5/featdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-07-05 07:36:26.000000 featdist-0.1.5/featdist/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/featdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:36:40.052848 featdist-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-05 07:36:26.000000 featdist-0.1.5/setup.py
```

### Comparing `featdist-0.1.4/LICENSE` & `featdist-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `featdist-0.1.4/PKG-INFO` & `featdist-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featdist
-Version: 0.1.4
+Version: 0.1.5
 Summary: Train test target distribution function for machine learning
 Home-page: https://github.com/Hasan-Basri-Akcay/featdist
 Author: Hasan Basri Akcay
 Author-email: hasan.basri.akcay@gmail.com
 Keywords: python,data science,data analysis,exploratory data analysis,distribution,beginner
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

### Comparing `featdist-0.1.4/README.md` & `featdist-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `featdist-0.1.4/featdist/base.py` & `featdist-0.1.5/featdist/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,12 +353,13 @@
     except:
         return 0
 
 
 def _find_trend_changes(data):
     data_diff = data.diff()
     data_diff = data_diff > 0
+    data_diff = data_diff.values
     counts = 0
     for index in range(1,len(data_diff)-1):
         if data_diff[index] != data_diff[index+1]:
             counts+=1
-    return counts
+    return counts
```

### Comparing `featdist-0.1.4/featdist.egg-info/PKG-INFO` & `featdist-0.1.5/featdist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featdist
-Version: 0.1.4
+Version: 0.1.5
 Summary: Train test target distribution function for machine learning
 Home-page: https://github.com/Hasan-Basri-Akcay/featdist
 Author: Hasan Basri Akcay
 Author-email: hasan.basri.akcay@gmail.com
 Keywords: python,data science,data analysis,exploratory data analysis,distribution,beginner
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

### Comparing `featdist-0.1.4/setup.py` & `featdist-0.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="featdist",
-    version="v0.1.4",
+    version="v0.1.5",
     author="Hasan Basri Akcay",
     author_email="hasan.basri.akcay@gmail.com",
     description="Train test target distribution function for machine learning",
     long_description=(
         "Featdist (Train Test Target Distribution) helps with feature understanding, "
         "calculating feature importances, feature comparison, feature debugging, and "
         "leakage detection"
```

