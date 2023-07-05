# Comparing `tmp/onboard.client-1.9.2.tar.gz` & `tmp/onboard.client-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboard.client-1.9.2.tar", last modified: Wed Mar 29 17:13:33 2023, max compression
+gzip compressed data, was "onboard.client-1.9.3.tar", last modified: Wed Jul  5 17:11:49 2023, max compression
```

## Comparing `onboard.client-1.9.2.tar` & `onboard.client-1.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-03-29 17:13:33.098313 onboard.client-1.9.2/
--rw-rw-r--   0 john      (1001) john      (1001)    10174 2022-11-08 18:10:09.000000 onboard.client-1.9.2/LICENSE
--rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-03-29 17:13:33.098313 onboard.client-1.9.2/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)     6477 2023-03-08 19:59:24.000000 onboard.client-1.9.2/README.md
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-03-29 17:13:33.094313 onboard.client-1.9.2/onboard/
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-03-29 17:13:33.098313 onboard.client-1.9.2/onboard/client/
--rw-rw-r--   0 john      (1001) john      (1001)      337 2022-11-08 18:10:09.000000 onboard.client-1.9.2/onboard/client/__init__.py
--rw-rw-r--   0 john      (1001) john      (1001)    10308 2023-03-29 16:59:46.000000 onboard.client-1.9.2/onboard/client/client.py
--rw-rw-r--   0 john      (1001) john      (1001)     3375 2022-11-08 18:10:09.000000 onboard.client-1.9.2/onboard/client/dataframes.py
--rw-rw-r--   0 john      (1001) john      (1001)      277 2022-11-08 18:10:09.000000 onboard.client-1.9.2/onboard/client/exceptions.py
--rw-rw-r--   0 john      (1001) john      (1001)     3722 2023-03-08 20:04:47.000000 onboard.client-1.9.2/onboard/client/helpers.py
--rw-rw-r--   0 john      (1001) john      (1001)     5789 2022-11-08 18:10:09.000000 onboard.client-1.9.2/onboard/client/models.py
--rw-rw-r--   0 john      (1001) john      (1001)        0 2022-11-08 18:10:09.000000 onboard.client-1.9.2/onboard/client/py.typed
--rw-rw-r--   0 john      (1001) john      (1001)     2954 2023-03-08 19:20:53.000000 onboard.client-1.9.2/onboard/client/staging.py
--rw-rw-r--   0 john      (1001) john      (1001)     1646 2023-03-08 18:47:59.000000 onboard.client-1.9.2/onboard/client/util.py
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-03-29 17:13:33.094313 onboard.client-1.9.2/onboard.client.egg-info/
--rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-03-29 17:13:33.000000 onboard.client-1.9.2/onboard.client.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      449 2023-03-29 17:13:33.000000 onboard.client-1.9.2/onboard.client.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1001) john      (1001)        1 2023-03-29 17:13:33.000000 onboard.client-1.9.2/onboard.client.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1001) john      (1001)      123 2023-03-29 17:13:33.000000 onboard.client-1.9.2/onboard.client.egg-info/requires.txt
--rw-rw-r--   0 john      (1001) john      (1001)        8 2023-03-29 17:13:33.000000 onboard.client-1.9.2/onboard.client.egg-info/top_level.txt
--rw-rw-r--   0 john      (1001) john      (1001)       38 2023-03-29 17:13:33.098313 onboard.client-1.9.2/setup.cfg
--rw-rw-r--   0 john      (1001) john      (1001)     1319 2023-03-29 17:09:07.000000 onboard.client-1.9.2/setup.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/
+-rw-rw-r--   0 john      (1001) john      (1001)    10174 2022-11-08 18:10:09.000000 onboard.client-1.9.3/LICENSE
+-rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-07-05 17:11:49.882492 onboard.client-1.9.3/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)     6477 2023-03-08 19:59:24.000000 onboard.client-1.9.3/README.md
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard/
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard/client/
+-rw-rw-r--   0 john      (1001) john      (1001)      337 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/__init__.py
+-rw-rw-r--   0 john      (1001) john      (1001)    10308 2023-03-29 16:59:46.000000 onboard.client-1.9.3/onboard/client/client.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3375 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/dataframes.py
+-rw-rw-r--   0 john      (1001) john      (1001)      277 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/exceptions.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3722 2023-03-08 20:04:47.000000 onboard.client-1.9.3/onboard/client/helpers.py
+-rw-rw-r--   0 john      (1001) john      (1001)     5789 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/models.py
+-rw-rw-r--   0 john      (1001) john      (1001)        0 2022-11-08 18:10:09.000000 onboard.client-1.9.3/onboard/client/py.typed
+-rw-rw-r--   0 john      (1001) john      (1001)     2954 2023-03-08 19:20:53.000000 onboard.client-1.9.3/onboard/client/staging.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1646 2023-03-08 18:47:59.000000 onboard.client-1.9.3/onboard/client/util.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2023-07-05 17:11:49.882492 onboard.client-1.9.3/onboard.client.egg-info/
+-rw-rw-r--   0 john      (1001) john      (1001)     7366 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      449 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        1 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1001) john      (1001)      126 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/requires.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        8 2023-07-05 17:11:49.000000 onboard.client-1.9.3/onboard.client.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       38 2023-07-05 17:11:49.882492 onboard.client-1.9.3/setup.cfg
+-rw-rw-r--   0 john      (1001) john      (1001)     1319 2023-07-05 17:03:28.000000 onboard.client-1.9.3/setup.py
```

### Comparing `onboard.client-1.9.2/LICENSE` & `onboard.client-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/PKG-INFO` & `onboard.client-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboard.client
-Version: 1.9.2
+Version: 1.9.3
 Summary: Onboard API SDK
 Home-page: https://github.com/onboard-data/client-py
 Author: Nathan Merritt, John Vines
 Author-email: support@onboarddata.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `onboard.client-1.9.2/README.md` & `onboard.client-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/client.py` & `onboard.client-1.9.3/onboard/client/client.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/dataframes.py` & `onboard.client-1.9.3/onboard/client/dataframes.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/helpers.py` & `onboard.client-1.9.3/onboard/client/helpers.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/models.py` & `onboard.client-1.9.3/onboard/client/models.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/staging.py` & `onboard.client-1.9.3/onboard/client/staging.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard/client/util.py` & `onboard.client-1.9.3/onboard/client/util.py`

 * *Files identical despite different names*

### Comparing `onboard.client-1.9.2/onboard.client.egg-info/PKG-INFO` & `onboard.client-1.9.3/onboard.client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboard.client
-Version: 1.9.2
+Version: 1.9.3
 Summary: Onboard API SDK
 Home-page: https://github.com/onboard-data/client-py
 Author: Nathan Merritt, John Vines
 Author-email: support@onboarddata.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `onboard.client-1.9.2/setup.py` & `onboard.client-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(name='onboard.client',
-      version='1.9.2',
+      version='1.9.3',
       author='Nathan Merritt, John Vines',
       author_email='support@onboarddata.io',
       description='Onboard API SDK',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/onboard-data/client-py',
       packages=['onboard.client'],
```

