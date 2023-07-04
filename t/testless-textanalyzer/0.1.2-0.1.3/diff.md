# Comparing `tmp/testless_textanalyzer-0.1.2.tar.gz` & `tmp/testless_textanalyzer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.2.tar", last modified: Fri Jun 30 18:23:40 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.3.tar", last modified: Tue Jul  4 23:29:37 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.2.tar` & `testless_textanalyzer-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 18:23:40.601628 testless_textanalyzer-0.1.2/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-06-30 18:23:40.601628 testless_textanalyzer-0.1.2/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-06-30 18:23:40.601628 testless_textanalyzer-0.1.2/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      633 2023-06-30 18:22:18.000000 testless_textanalyzer-0.1.2/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 18:23:40.597628 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-06-30 18:23:40.000000 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      406 2023-06-30 18:23:40.000000 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-06-30 18:23:40.000000 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       48 2023-06-30 18:23:40.000000 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-06-30 18:23:40.000000 testless_textanalyzer-0.1.2/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 18:23:40.597628 testless_textanalyzer-0.1.2/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.2/textanalyzer/__init__.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-06-30 18:23:40.601628 testless_textanalyzer-0.1.2/textanalyzer/testless_textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.2/textanalyzer/testless_textanalyzer/__init__.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.2/textanalyzer/testless_textanalyzer/feature_set.py
--rw-rw-r--   0 yousif    (1000) yousif    (1000)     3818 2023-06-30 12:42:38.000000 testless_textanalyzer-0.1.2/textanalyzer/testless_textanalyzer/text_analyzer.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      633 2023-07-04 23:28:58.000000 testless_textanalyzer-0.1.3/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.052926 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      542 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       48 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:29:36.000000 testless_textanalyzer-0.1.3/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.3/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:29:37.056926 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        4 2023-06-26 23:28:42.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/__init__.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     5931 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     7344 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/crf_utils.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     8650 2023-07-04 19:03:02.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2246 2023-06-26 21:34:30.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature_set.py
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)     2644 2023-07-04 17:44:09.000000 testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/text_analyzer.py
```

### Comparing `testless_textanalyzer-0.1.2/setup.py` & `testless_textanalyzer-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.2',
+  version='0.1.3',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
   long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
```

### Comparing `testless_textanalyzer-0.1.2/textanalyzer/testless_textanalyzer/feature_set.py` & `testless_textanalyzer-0.1.3/textanalyzer/testless_textanalyzer/feature_set.py`

 * *Files identical despite different names*

