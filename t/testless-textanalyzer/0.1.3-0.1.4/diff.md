# Comparing `tmp/testless_textanalyzer-0.1.3.tar.gz` & `tmp/testless_textanalyzer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.3.tar", last modified: Tue Jul  4 23:29:37 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.4.tar", last modified: Tue Jul  4 23:32:54 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.3.tar` & `testless_textanalyzer-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      633 2023-07-04 23:28:58.000000 testless_textanalyzer-0.1.3/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.052926 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      542 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       48 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.3/textanalyzer/__init__.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/__init__.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     5931 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     7344 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf_utils.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature_set.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2644 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/text_analyzer.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-04 23:32:44.000000 testless_textanalyzer-0.1.4/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      542 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:32:53.000000 testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.4/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:32:54.154845 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/__init__.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     5931 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     7344 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf_utils.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature_set.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2644 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/text_analyzer.py
```

### Comparing `testless_textanalyzer-0.1.3/setup.py` & `testless_textanalyzer-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.3',
+  version='0.1.4',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
   long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
   classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
   ],
-  install_requires=["nltk>=3.8" , "numpy>=1.21.5" , "sklearn_crfsuite>=0.3.6"],
+  install_requires=["nltk>=3.8" , "numpy>=1.21.5" , "sklearn_crfsuite>=0.3.6", "scipy >= 1.7.1"],
 )
```

### Comparing `testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/SOURCES.txt` & `testless_textanalyzer-0.1.4/testless_textanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf.py` & `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf_utils.py` & `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/crf_utils.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature.py` & `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature_set.py` & `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/feature_set.py`

 * *Files identical despite different names*

### Comparing `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/text_analyzer.py` & `testless_textanalyzer-0.1.4/textanalyzer/testless_textanalyzer/text_analyzer.py`

 * *Files identical despite different names*

