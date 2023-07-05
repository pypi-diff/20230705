# Comparing `tmp/medirect-0.8.0.tar.gz` & `tmp/medirect-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/medirect-0.8.0.tar", last modified: Mon Jan  8 18:48:50 2018, max compression
+gzip compressed data, was "dist/medirect-0.9.0.tar", last modified: Mon May  7 20:40:50 2018, max compression
```

## Comparing `medirect-0.8.0.tar` & `medirect-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwx---   0 crosenth (452607616) domain^users (452461057)        0 2018-01-08 18:48:50.000000 medirect-0.8.0/
-drwxrwx---   0 crosenth (452607616) domain^users (452461057)        0 2018-01-08 18:48:50.000000 medirect-0.8.0/medirect/
--rw-rw----   0 crosenth (452607616) domain^users (452461057)     2734 2018-01-04 20:14:43.000000 medirect-0.8.0/medirect/__init__.py
--rwxrwx---   0 crosenth (452607616) domain^users (452461057)     5731 2018-01-05 19:40:56.000000 medirect-0.8.0/medirect/ftract.py
--rwxrwx---   0 crosenth (452607616) domain^users (452461057)     8622 2017-11-14 23:38:50.000000 medirect-0.8.0/medirect/mefetch.py
-drwxrwx---   0 crosenth (452607616) domain^users (452461057)        0 2018-01-08 18:48:50.000000 medirect-0.8.0/medirect.egg-info/
--rw-rw----   0 crosenth (452607616) domain^users (452461057)      713 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/PKG-INFO
--rw-rw----   0 crosenth (452607616) domain^users (452461057)      304 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/SOURCES.txt
--rw-rw----   0 crosenth (452607616) domain^users (452461057)        1 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/dependency_links.txt
--rw-rw----   0 crosenth (452607616) domain^users (452461057)       79 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/entry_points.txt
--rw-rw----   0 crosenth (452607616) domain^users (452461057)       32 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/requires.txt
--rw-rw----   0 crosenth (452607616) domain^users (452461057)        9 2018-01-08 18:48:49.000000 medirect-0.8.0/medirect.egg-info/top_level.txt
-drwxrwx---   0 crosenth (452607616) domain^users (452461057)        0 2018-01-08 18:48:50.000000 medirect-0.8.0/tests/
--rw-rw----   0 crosenth (452607616) domain^users (452461057)     3266 2018-01-05 19:41:23.000000 medirect-0.8.0/tests/test_ftract.py
--rw-rw----   0 crosenth (452607616) domain^users (452461057)     6402 2017-01-24 23:17:10.000000 medirect-0.8.0/README.rst
--rw-rw----   0 crosenth (452607616) domain^users (452461057)       80 2018-01-08 18:48:50.000000 medirect-0.8.0/setup.cfg
--rw-rw----   0 crosenth (452607616) domain^users (452461057)     1106 2018-01-08 18:41:07.000000 medirect-0.8.0/setup.py
--rw-rw----   0 crosenth (452607616) domain^users (452461057)      713 2018-01-08 18:48:50.000000 medirect-0.8.0/PKG-INFO
+drwxrwx---   0 crosenth (47973) g_crosenth (47973)        0 2018-05-07 20:40:50.000000 medirect-0.9.0/
+drwxrwx---   0 crosenth (47973) g_crosenth (47973)        0 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect/
+-rw-rw----   0 crosenth (47973) g_crosenth (47973)     2734 2018-05-07 20:39:39.000000 medirect-0.9.0/medirect/__init__.py
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)     7852 2018-05-07 20:39:39.000000 medirect-0.9.0/medirect/ftract.py
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)     8622 2017-12-05 20:26:57.000000 medirect-0.9.0/medirect/mefetch.py
+drwxrwx---   0 crosenth (47973) g_crosenth (47973)        0 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)      679 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/PKG-INFO
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)      283 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/SOURCES.txt
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)        1 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/dependency_links.txt
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)       79 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/entry_points.txt
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)       32 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/requires.txt
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)        9 2018-05-07 20:40:50.000000 medirect-0.9.0/medirect.egg-info/top_level.txt
+-rw-rw----   0 crosenth (47973) g_crosenth (47973)     6402 2018-05-07 20:39:31.000000 medirect-0.9.0/README.rst
+-rw-rw----   0 crosenth (47973) g_crosenth (47973)      101 2018-05-07 20:40:50.000000 medirect-0.9.0/setup.cfg
+-rwxrwx---   0 crosenth (47973) g_crosenth (47973)     1106 2018-05-07 20:39:39.000000 medirect-0.9.0/setup.py
+-rw-rw----   0 crosenth (47973) g_crosenth (47973)      679 2018-05-07 20:40:50.000000 medirect-0.9.0/PKG-INFO
```

### Comparing `medirect-0.8.0/medirect/__init__.py` & `medirect-0.9.0/medirect/__init__.py`

 * *Files identical despite different names*

### Comparing `medirect-0.8.0/medirect/mefetch.py` & `medirect-0.9.0/medirect/mefetch.py`

 * *Files identical despite different names*

### Comparing `medirect-0.8.0/medirect.egg-info/PKG-INFO` & `medirect-0.9.0/medirect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: medirect
-Version: 0.8.0
+Version: 0.9.0
 Summary: multiprocessed ncbi edirect and ftract
 Home-page: https://github.com/crosenth/medirect
 Author: Chris Rosenthal
 Author-email: crosenth@gmail.com
 License: GPLv3
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Keywords: ncbi,edirect,multiprocessing,entrez,bioinformatics
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `medirect-0.8.0/README.rst` & `medirect-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `medirect-0.8.0/setup.py` & `medirect-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     keywords=['ncbi', 'edirect', 'multiprocessing',
               'entrez', 'bioinformatics'],
     packages=setuptools.find_packages(exclude=['tests']),
     entry_points={
         'console_scripts': [
             'mefetch=medirect.mefetch:run',
             'ftract= medirect.ftract:run']},
-    version='0.8.0',
+    version='0.9.0',
     url='https://github.com/crosenth/medirect',
     license='GPLv3',
     install_requires=['biopython>=1.68', 'retrying>=1.3.3'],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Development Status :: 4 - Beta',
         'Environment :: Console',
```

### Comparing `medirect-0.8.0/PKG-INFO` & `medirect-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: medirect
-Version: 0.8.0
+Version: 0.9.0
 Summary: multiprocessed ncbi edirect and ftract
 Home-page: https://github.com/crosenth/medirect
 Author: Chris Rosenthal
 Author-email: crosenth@gmail.com
 License: GPLv3
-Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Keywords: ncbi,edirect,multiprocessing,entrez,bioinformatics
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

