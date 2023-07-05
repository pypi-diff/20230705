# Comparing `tmp/python-bvk-0.2.0.tar.gz` & `tmp/python-bvk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bvk-0.2.0.tar", last modified: Tue Dec 14 22:03:42 2021, max compression
+gzip compressed data, was "python-bvk-0.2.1.tar", last modified: Wed Jul  5 09:53:10 2023, max compression
```

## Comparing `python-bvk-0.2.0.tar` & `python-bvk-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 22:03:42.230290 python-bvk-0.2.0/
--rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.2.0/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     3442 2021-12-14 22:03:42.230290 python-bvk-0.2.0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.2.0/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 22:03:42.229290 python-bvk-0.2.0/bvk/
--rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.2.0/bvk/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.2.0/bvk/items.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3263 2020-08-07 19:27:30.000000 python-bvk-0.2.0/bvk/settings.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 22:03:42.229290 python-bvk-0.2.0/bvk/spiders/
--rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.2.0/bvk/spiders/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     5029 2021-12-14 21:51:07.000000 python-bvk-0.2.0/bvk/spiders/water_consumption.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2021-12-14 22:03:42.230290 python-bvk-0.2.0/python_bvk.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     3442 2021-12-14 22:03:42.000000 python-bvk-0.2.0/python_bvk.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      297 2021-12-14 22:03:42.000000 python-bvk-0.2.0/python_bvk.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-12-14 22:03:42.000000 python-bvk-0.2.0/python_bvk.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)      566 2021-12-14 22:03:42.000000 python-bvk-0.2.0/python_bvk.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        4 2021-12-14 22:03:42.000000 python-bvk-0.2.0/python_bvk.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2021-12-14 22:03:42.230290 python-bvk-0.2.0/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)      850 2021-12-14 22:03:18.000000 python-bvk-0.2.0/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.060830 python-bvk-0.2.1/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.2.1/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2023-07-05 09:53:10.060830 python-bvk-0.2.1/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.2.1/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.058830 python-bvk-0.2.1/bvk/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.2.1/bvk/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.2.1/bvk/items.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3263 2020-08-07 19:27:30.000000 python-bvk-0.2.1/bvk/settings.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.059830 python-bvk-0.2.1/bvk/spiders/
+-rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.2.1/bvk/spiders/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     5029 2021-12-14 21:51:07.000000 python-bvk-0.2.1/bvk/spiders/water_consumption.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.059830 python-bvk-0.2.1/python_bvk.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      297 2023-07-05 09:53:10.000000 python-bvk-0.2.1/python_bvk.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        4 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-07-05 09:53:10.060830 python-bvk-0.2.1/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)      785 2023-07-05 09:47:48.000000 python-bvk-0.2.1/setup.py
```

### Comparing `python-bvk-0.2.0/LICENSE` & `python-bvk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/PKG-INFO` & `python-bvk-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-bvk
@@ -104,9 +102,7 @@
 scraping the BVK customer portal to get the data. If BVK comes to think you are
 abusing the website they may block your IP address and/or account.
 
 
 # License
 
 See [LICENSE](./LICENSE).
-
-
```

### Comparing `python-bvk-0.2.0/README.md` & `python-bvk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/bvk/__init__.py` & `python-bvk-0.2.1/bvk/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/bvk/items.py` & `python-bvk-0.2.1/bvk/items.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/bvk/settings.py` & `python-bvk-0.2.1/bvk/settings.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/bvk/spiders/water_consumption.py` & `python-bvk-0.2.1/bvk/spiders/water_consumption.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.0/python_bvk.egg-info/PKG-INFO` & `python-bvk-0.2.1/python_bvk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-bvk
@@ -104,9 +102,7 @@
 scraping the BVK customer portal to get the data. If BVK comes to think you are
 abusing the website they may block your IP address and/or account.
 
 
 # License
 
 See [LICENSE](./LICENSE).
-
-
```

### Comparing `python-bvk-0.2.0/setup.py` & `python-bvk-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open("requirements.txt") as fh:
-    install_requires = [line for line in fh if line and line[0] not in "#-"]
+install_requires = ["scrapy", "python-dateutil"]
 
 setuptools.setup(
     name="python-bvk",
-    version="0.2.0",
+    version="0.2.1",
     author="Dan Keder",
     author_email="dan.keder@protonmail.com",
     description="Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dankeder/python-bvk",
     packages=setuptools.find_packages(),
```

