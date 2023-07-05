# Comparing `tmp/flypp-5.2.1.tar.gz` & `tmp/flypp-5.2.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flypp-5.2.1.tar", last modified: Tue Jul  4 10:18:07 2023, max compression
+gzip compressed data, was "flypp-5.2.1.2.1.tar", last modified: Wed Jul  5 14:28:16 2023, max compression
```

## Comparing `flypp-5.2.1.tar` & `flypp-5.2.1.2.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 10:18:07.263113 flypp-5.2.1/
--rw-rw-rw-   0        0        0     1085 2023-07-04 09:14:29.000000 flypp-5.2.1/LICENSE
--rw-rw-rw-   0        0        0      900 2023-07-04 10:18:07.262113 flypp-5.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-07-04 09:14:50.000000 flypp-5.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-04 10:18:07.246655 flypp-5.2.1/flypp/
--rw-rw-rw-   0        0        0        0 2023-07-04 09:13:33.000000 flypp-5.2.1/flypp/__init__.py
--rw-rw-rw-   0        0        0       83 2023-07-04 09:55:54.000000 flypp-5.2.1/flypp/main.py
-drwxrwxrwx   0        0        0        0 2023-07-04 10:18:07.261106 flypp-5.2.1/flypp.egg-info/
--rw-rw-rw-   0        0        0      900 2023-07-04 10:18:06.000000 flypp-5.2.1/flypp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-07-04 10:18:07.000000 flypp-5.2.1/flypp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 10:18:06.000000 flypp-5.2.1/flypp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 10:18:06.000000 flypp-5.2.1/flypp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 10:18:06.000000 flypp-5.2.1/flypp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 10:18:07.263113 flypp-5.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-07-04 10:17:50.000000 flypp-5.2.1/setup.py
+drwxr-xr-x   0 r3pwnx     (501) staff       (20)        0 2023-07-05 14:28:16.061032 flypp-5.2.1.2.1/
+-rw-r--r--   0 r3pwnx     (501) staff       (20)     1085 2023-07-04 09:14:29.000000 flypp-5.2.1.2.1/LICENSE
+-rw-r--r--   0 r3pwnx     (501) staff       (20)       23 2023-07-05 14:26:26.000000 flypp-5.2.1.2.1/MANIFEST.in
+-rw-r--r--   0 r3pwnx     (501) staff       (20)      886 2023-07-05 14:28:16.060912 flypp-5.2.1.2.1/PKG-INFO
+-rw-r--r--   0 r3pwnx     (501) staff       (20)       10 2023-07-04 09:14:50.000000 flypp-5.2.1.2.1/README.rst
+drwxr-xr-x   0 r3pwnx     (501) staff       (20)        0 2023-07-05 14:28:16.060171 flypp-5.2.1.2.1/flypp/
+-rw-r--r--   0 r3pwnx     (501) staff       (20)        0 2023-07-04 09:13:33.000000 flypp-5.2.1.2.1/flypp/__init__.py
+-rw-r--r--   0 r3pwnx     (501) staff       (20)     1361 2023-07-04 15:50:52.000000 flypp-5.2.1.2.1/flypp/egg.py
+-rw-r--r--   0 r3pwnx     (501) staff       (20)   684177 2023-07-04 15:00:57.000000 flypp-5.2.1.2.1/flypp/flypp.gif
+-rw-r--r--   0 r3pwnx     (501) staff       (20)      131 2023-07-04 15:53:33.000000 flypp-5.2.1.2.1/flypp/main.py
+drwxr-xr-x   0 r3pwnx     (501) staff       (20)        0 2023-07-05 14:28:16.060739 flypp-5.2.1.2.1/flypp.egg-info/
+-rw-r--r--   0 r3pwnx     (501) staff       (20)      886 2023-07-05 14:28:16.000000 flypp-5.2.1.2.1/flypp.egg-info/PKG-INFO
+-rw-r--r--   0 r3pwnx     (501) staff       (20)      248 2023-07-05 14:28:16.000000 flypp-5.2.1.2.1/flypp.egg-info/SOURCES.txt
+-rw-r--r--   0 r3pwnx     (501) staff       (20)        1 2023-07-05 14:28:16.000000 flypp-5.2.1.2.1/flypp.egg-info/dependency_links.txt
+-rw-r--r--   0 r3pwnx     (501) staff       (20)       69 2023-07-05 14:28:16.000000 flypp-5.2.1.2.1/flypp.egg-info/entry_points.txt
+-rw-r--r--   0 r3pwnx     (501) staff       (20)        6 2023-07-05 14:28:16.000000 flypp-5.2.1.2.1/flypp.egg-info/top_level.txt
+-rw-r--r--   0 r3pwnx     (501) staff       (20)       38 2023-07-05 14:28:16.061078 flypp-5.2.1.2.1/setup.cfg
+-rw-r--r--   0 r3pwnx     (501) staff       (20)     1323 2023-07-05 14:28:10.000000 flypp-5.2.1.2.1/setup.py
```

### Comparing `flypp-5.2.1/LICENSE` & `flypp-5.2.1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flypp-5.2.1/PKG-INFO` & `flypp-5.2.1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1
-Name: flypp
-Version: 5.2.1
-Summary: fast fetch
-Home-page: 
-Author: flypp
-Author-email: flypp@noexists.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
-
-fast fetch
+Metadata-Version: 2.1
+Name: flypp
+Version: 5.2.1.2.1
+Summary: fast fetch
+Home-page: UNKNOWN
+Author: flypp
+Author-email: flypp@noexists.com
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+fast fetch
+
```

### Comparing `flypp-5.2.1/flypp.egg-info/PKG-INFO` & `flypp-5.2.1.2.1/flypp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1
-Name: flypp
-Version: 5.2.1
-Summary: fast fetch
-Home-page: 
-Author: flypp
-Author-email: flypp@noexists.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
-
-fast fetch
+Metadata-Version: 2.1
+Name: flypp
+Version: 5.2.1.2.1
+Summary: fast fetch
+Home-page: UNKNOWN
+Author: flypp
+Author-email: flypp@noexists.com
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+fast fetch
+
```

### Comparing `flypp-5.2.1/setup.py` & `flypp-5.2.1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
   long_description = f.read()
 setup(name='flypp',  # 包名
-      version='5.2.1',  # 版本号
+      version='5.2.1.2.1',  # 版本号
       description='fast fetch',
       long_description=long_description,
       author='flypp',
       author_email='flypp@noexists.com',
       url='',
       install_requires=[],
       license='MIT License',
@@ -26,10 +26,10 @@
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
           'Topic :: Software Development :: Libraries'
       ],
   entry_points = {
-    'console_scripts': ['flypp=flypp.main:main'],
+    'console_scripts': ['flypp=flypp.main:main', 'ppegg=flypp.egg:run_egg'],
   },
 )
```

