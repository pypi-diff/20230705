# Comparing `tmp/testless_textanalyzer-0.1.6.tar.gz` & `tmp/testless_textanalyzer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testless_textanalyzer-0.1.6.tar", last modified: Tue Jul  4 23:52:08 2023, max compression
+gzip compressed data, was "testless_textanalyzer-0.1.7.tar", last modified: Tue Jul  4 23:57:57 2023, max compression
```

## Comparing `testless_textanalyzer-0.1.6.tar` & `testless_textanalyzer-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:52:08.335344 testless_textanalyzer-0.1.6/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:52:08.335344 testless_textanalyzer-0.1.6/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:52:08.335344 testless_textanalyzer-0.1.6/setup.cfg
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-04 23:52:05.000000 testless_textanalyzer-0.1.6/setup.py
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:52:08.335344 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:52:07.000000 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 yousif    (1000) yousif    (1000)      257 2023-07-04 23:52:08.000000 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:52:07.000000 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-04 23:52:07.000000 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/requires.txt
--rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:52:07.000000 testless_textanalyzer-0.1.6/testless_textanalyzer.egg-info/top_level.txt
-drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:52:08.335344 testless_textanalyzer-0.1.6/textanalyzer/
--rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.6/textanalyzer/__init__.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:57:57.459689 testless_textanalyzer-0.1.7/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:57:57.459689 testless_textanalyzer-0.1.7/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       38 2023-07-04 23:57:57.459689 testless_textanalyzer-0.1.7/setup.cfg
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      651 2023-07-04 23:56:52.000000 testless_textanalyzer-0.1.7/setup.py
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:57:57.459689 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      377 2023-07-04 23:57:57.000000 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)      257 2023-07-04 23:57:57.000000 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        1 2023-07-04 23:57:57.000000 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       61 2023-07-04 23:57:57.000000 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/requires.txt
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)       13 2023-07-04 23:57:57.000000 testless_textanalyzer-0.1.7/testless_textanalyzer.egg-info/top_level.txt
+drwxrwxr-x   0 yousif    (1000) yousif    (1000)        0 2023-07-04 23:57:57.459689 testless_textanalyzer-0.1.7/textanalyzer/
+-rw-rw-r--   0 yousif    (1000) yousif    (1000)        0 2023-06-30 12:43:17.000000 testless_textanalyzer-0.1.7/textanalyzer/__init__.py
```

### Comparing `testless_textanalyzer-0.1.6/setup.py` & `testless_textanalyzer-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'testless_textanalyzer' ,
-  version='0.1.6',
+  version='0.1.7',
   description='A text analyzer for test step sentences',
   packages=find_packages(),
   author='Youssef Ahmed',
   include_package_data=True,
   license='MIT',
   long_description="Text analyzer for test step sentences",
   long_description_content_type="text/markdown",
```

