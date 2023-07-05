# Comparing `tmp/PrSpiders-0.5.2.6.tar.gz` & `tmp/PrSpiders-0.5.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.6.tar", last modified: Wed Jul  5 02:42:45 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.7.tar", last modified: Wed Jul  5 02:49:11 2023, max compression
```

## Comparing `PrSpiders-0.5.2.6.tar` & `PrSpiders-0.5.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.803274 PrSpiders-0.5.2.6/
--rw-rw-rw-   0        0        0     1091 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     5497 2023-07-05 02:42:45.802276 PrSpiders-0.5.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.771359 PrSpiders-0.5.2.6/PrSpider/
--rw-rw-rw-   0        0        0    11427 2023-07-05 02:33:58.000000 PrSpiders-0.5.2.6/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/PrSpider/__init__.py
--rw-rw-rw-   0        0        0     2799 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/PrSpider/log.py
--rw-rw-rw-   0        0        0    11257 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3260 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4881 2023-07-05 02:34:28.000000 PrSpiders-0.5.2.6/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.784326 PrSpiders-0.5.2.6/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5497 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-05 02:42:45.000000 PrSpiders-0.5.2.6/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5136 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.786321 PrSpiders-0.5.2.6/pkg/
--rw-rw-rw-   0        0        0       23 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.793301 PrSpiders-0.5.2.6/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-07-05 02:42:45.800283 PrSpiders-0.5.2.6/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4217 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.6/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-07-05 02:42:45.804272 PrSpiders-0.5.2.6/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-07-05 02:34:28.000000 PrSpiders-0.5.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.292601 PrSpiders-0.5.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     5497 2023-07-05 02:49:11.292601 PrSpiders-0.5.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.261680 PrSpiders-0.5.2.7/PrSpider/
+-rw-rw-rw-   0        0        0    11427 2023-07-05 02:33:58.000000 PrSpiders-0.5.2.7/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2799 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11243 2023-07-05 02:48:51.000000 PrSpiders-0.5.2.7/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3254 2023-07-05 02:48:51.000000 PrSpiders-0.5.2.7/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4881 2023-07-05 02:34:28.000000 PrSpiders-0.5.2.7/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.273651 PrSpiders-0.5.2.7/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5497 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-05 02:49:11.000000 PrSpiders-0.5.2.7/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5136 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.275643 PrSpiders-0.5.2.7/pkg/
+-rw-rw-rw-   0        0        0       23 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.283622 PrSpiders-0.5.2.7/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-07-05 02:49:11.290604 PrSpiders-0.5.2.7/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4217 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-06-19 00:51:50.000000 PrSpiders-0.5.2.7/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 02:49:11.293596 PrSpiders-0.5.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-07-05 02:49:05.000000 PrSpiders-0.5.2.7/setup.py
```

### Comparing `PrSpiders-0.5.2.6/LICENSE.txt` & `PrSpiders-0.5.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/PKG-INFO` & `PrSpiders-0.5.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.6
+Version: 0.5.2.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.6/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2.7/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/PrSpider/log.py` & `PrSpiders-0.5.2.7/PrSpider/log.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/PrSpider/pxpath.py` & `PrSpiders-0.5.2.7/PrSpider/pxpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from urllib.parse import urljoin
 import re, time, copy
 from lxml import etree
 from datetime import timedelta, datetime
 import unicodedata
-from PrSpider.PrSpiders import loguer
+from .log import loguer
 
 
 class Xpath(object):
     def __init__(self, response, encoding="utf-8"):
         if isinstance(response, str):
             self.res = etree.HTML(response)
         else:
```

### Comparing `PrSpiders-0.5.2.6/PrSpider/pyconn.py` & `PrSpiders-0.5.2.7/PrSpider/pyconn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pymysql
-from .PrSpiders import loguer
+from .log import loguer
 
 
 def ErrorTip(func):
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
```

### Comparing `PrSpiders-0.5.2.6/PrSpider/requestXpath.py` & `PrSpiders-0.5.2.7/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/PrSpider/useragent.py` & `PrSpiders-0.5.2.7/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2.7/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.6
+Version: 0.5.2.7
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.6/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2.7/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/README.md` & `PrSpiders-0.5.2.7/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2.7/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/pkg/prspider/start.py` & `PrSpiders-0.5.2.7/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/requestXpath/__init__.py` & `PrSpiders-0.5.2.7/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/requestXpath/pxpath.py` & `PrSpiders-0.5.2.7/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/requestXpath/requestXpath.py` & `PrSpiders-0.5.2.7/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/requestXpath/useragent.py` & `PrSpiders-0.5.2.7/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.6/setup.py` & `PrSpiders-0.5.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.2.6"
+__version__ = "0.5.2.7"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

