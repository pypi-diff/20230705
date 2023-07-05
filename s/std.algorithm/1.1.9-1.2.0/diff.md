# Comparing `tmp/std.algorithm-1.1.9.tar.gz` & `tmp/std.algorithm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.9.tar", last modified: Wed Jul  5 05:20:51 2023, max compression
+gzip compressed data, was "std.algorithm-1.2.0.tar", last modified: Wed Jul  5 05:26:24 2023, max compression
```

## Comparing `std.algorithm-1.1.9.tar` & `std.algorithm-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.656270 std.algorithm-1.1.9/
--rw-rw-rw-   0        0        0     1186 2023-07-05 05:20:51.657269 std.algorithm-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      805 2023-07-05 05:15:57.000000 std.algorithm-1.1.9/README.md
--rw-rw-rw-   0        0        0      312 2023-07-05 05:20:51.658269 std.algorithm-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      598 2023-07-05 03:44:38.000000 std.algorithm-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.622336 std.algorithm-1.1.9/std/
--rw-rw-rw-   0        0        0    15074 2023-06-29 01:01:53.000000 std.algorithm-1.1.9/std/MySQL.py
--rw-rw-rw-   0        0        0    21080 2023-06-24 23:12:40.000000 std.algorithm-1.1.9/std/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.588637 std.algorithm-1.1.9/std/assets/
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.588637 std.algorithm-1.1.9/std/assets/cn/
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.628332 std.algorithm-1.1.9/std/assets/cn/segment/
--rw-rw-rw-   0        0        0  5809716 2022-08-12 09:27:37.000000 std.algorithm-1.1.9/std/assets/cn/segment/vocab.csv
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.590635 std.algorithm-1.1.9/std/assets/jp/
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.637328 std.algorithm-1.1.9/std/assets/jp/segment/
--rw-rw-rw-   0        0        0   974268 2021-07-12 00:31:55.000000 std.algorithm-1.1.9/std/assets/jp/segment/vocab.csv
--rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.9/std/combinatorics.py
--rw-rw-rw-   0        0        0    16008 2023-07-05 03:38:56.000000 std.algorithm-1.1.9/std/cpp.py
--rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.9/std/data.py
--rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/error.py
--rw-rw-rw-   0        0        0     8575 2023-06-13 06:00:00.000000 std.algorithm-1.1.9/std/file.py
--rw-rw-rw-   0        0        0     1822 2023-06-29 00:59:34.000000 std.algorithm-1.1.9/std/http.py
--rw-rw-rw-   0        0        0    40303 2023-06-19 00:45:15.000000 std.algorithm-1.1.9/std/keras.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.644323 std.algorithm-1.1.9/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.9/std/lib/eigen.dll
--rw-rw-rw-   0        0        0  1821816 2023-07-05 04:59:41.000000 std.algorithm-1.1.9/std/lib/libeigen.so
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.649322 std.algorithm-1.1.9/std/nlp/
--rw-rw-rw-   0        0        0      976 2023-07-05 03:24:35.000000 std.algorithm-1.1.9/std/nlp/__init__.py
--rw-rw-rw-   0        0        0    12833 2023-07-05 03:24:56.000000 std.algorithm-1.1.9/std/nlp/ner.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.656270 std.algorithm-1.1.9/std/nlp/segment/
--rw-rw-rw-   0        0        0        0 2023-07-05 03:49:19.000000 std.algorithm-1.1.9/std/nlp/segment/__init__.py
--rw-rw-rw-   0        0        0     5960 2023-07-05 03:33:09.000000 std.algorithm-1.1.9/std/nlp/segment/cn.py
--rw-rw-rw-   0        0        0     2896 2022-12-12 01:11:49.000000 std.algorithm-1.1.9/std/nlp/segment/en.py
--rw-rw-rw-   0        0        0     6731 2023-07-05 03:42:31.000000 std.algorithm-1.1.9/std/nlp/segment/jp.py
--rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.9/std/regexp.py
--rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.9/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.9/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.9/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.9/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:20:51.627333 std.algorithm-1.1.9/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0     1186 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-05 05:20:51.000000 std.algorithm-1.1.9/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.913973 std.algorithm-1.2.0/
+-rw-rw-rw-   0        0        0     1186 2023-07-05 05:26:24.914973 std.algorithm-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      805 2023-07-05 05:15:57.000000 std.algorithm-1.2.0/README.md
+-rw-rw-rw-   0        0        0      312 2023-07-05 05:26:24.915972 std.algorithm-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      598 2023-07-05 03:44:38.000000 std.algorithm-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.881328 std.algorithm-1.2.0/std/
+-rw-rw-rw-   0        0        0    15074 2023-06-29 01:01:53.000000 std.algorithm-1.2.0/std/MySQL.py
+-rw-rw-rw-   0        0        0    21080 2023-06-24 23:12:40.000000 std.algorithm-1.2.0/std/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.834699 std.algorithm-1.2.0/std/assets/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.833701 std.algorithm-1.2.0/std/assets/cn/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.887932 std.algorithm-1.2.0/std/assets/cn/segment/
+-rw-rw-rw-   0        0        0  5809716 2022-08-12 09:27:37.000000 std.algorithm-1.2.0/std/assets/cn/segment/vocab.csv
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.836697 std.algorithm-1.2.0/std/assets/jp/
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.896927 std.algorithm-1.2.0/std/assets/jp/segment/
+-rw-rw-rw-   0        0        0   974268 2021-07-12 00:31:55.000000 std.algorithm-1.2.0/std/assets/jp/segment/vocab.csv
+-rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.2.0/std/combinatorics.py
+-rw-rw-rw-   0        0        0    16005 2023-07-05 05:25:50.000000 std.algorithm-1.2.0/std/cpp.py
+-rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.2.0/std/data.py
+-rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.2.0/std/error.py
+-rw-rw-rw-   0        0        0     8575 2023-06-13 06:00:00.000000 std.algorithm-1.2.0/std/file.py
+-rw-rw-rw-   0        0        0     1822 2023-06-29 00:59:34.000000 std.algorithm-1.2.0/std/http.py
+-rw-rw-rw-   0        0        0    40303 2023-06-19 00:45:15.000000 std.algorithm-1.2.0/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.903922 std.algorithm-1.2.0/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.2.0/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0  1821816 2023-07-05 04:59:41.000000 std.algorithm-1.2.0/std/lib/libeigen.so
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.908920 std.algorithm-1.2.0/std/nlp/
+-rw-rw-rw-   0        0        0      976 2023-07-05 03:24:35.000000 std.algorithm-1.2.0/std/nlp/__init__.py
+-rw-rw-rw-   0        0        0    12833 2023-07-05 03:24:56.000000 std.algorithm-1.2.0/std/nlp/ner.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.912974 std.algorithm-1.2.0/std/nlp/segment/
+-rw-rw-rw-   0        0        0        0 2023-07-05 03:49:19.000000 std.algorithm-1.2.0/std/nlp/segment/__init__.py
+-rw-rw-rw-   0        0        0     5960 2023-07-05 03:33:09.000000 std.algorithm-1.2.0/std/nlp/segment/cn.py
+-rw-rw-rw-   0        0        0     2896 2022-12-12 01:11:49.000000 std.algorithm-1.2.0/std/nlp/segment/en.py
+-rw-rw-rw-   0        0        0     6731 2023-07-05 03:42:31.000000 std.algorithm-1.2.0/std/nlp/segment/jp.py
+-rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.2.0/std/regexp.py
+-rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.2.0/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.2.0/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.2.0/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.2.0/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.2.0/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-07-05 05:26:24.886927 std.algorithm-1.2.0/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0     1186 2023-07-05 05:26:24.000000 std.algorithm-1.2.0/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-05 05:26:24.000000 std.algorithm-1.2.0/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 05:26:24.000000 std.algorithm-1.2.0/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 05:26:24.000000 std.algorithm-1.2.0/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-05 05:26:24.000000 std.algorithm-1.2.0/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.9/PKG-INFO` & `std.algorithm-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: std.algorithm
-Version: 1.1.9
+Version: 1.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Cosmos
 Author-email: 744984949@qq.com
 License: MIT
 Description: # std
```

### Comparing `std.algorithm-1.1.9/README.md` & `std.algorithm-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/setup.py` & `std.algorithm-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/MySQL.py` & `std.algorithm-1.2.0/std/MySQL.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/__init__.py` & `std.algorithm-1.2.0/std/__init__.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/assets/cn/segment/vocab.csv` & `std.algorithm-1.2.0/std/assets/cn/segment/vocab.csv`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/assets/jp/segment/vocab.csv` & `std.algorithm-1.2.0/std/assets/jp/segment/vocab.csv`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/combinatorics.py` & `std.algorithm-1.2.0/std/combinatorics.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/cpp.py` & `std.algorithm-1.2.0/std/cpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ctypes import *
 import std
 import numpy as np
 import os
 
-ctypes2numpy = {"?": np.bool,
+ctypes2numpy = {"?": bool,
           "c": np.char,
           "b": np.byte,
           "B": np.ubyte,
           "f": np.float32,
           "d": np.double,
           "g": np.longdouble,
           "h": np.short,
```

### Comparing `std.algorithm-1.1.9/std/data.py` & `std.algorithm-1.2.0/std/data.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/file.py` & `std.algorithm-1.2.0/std/file.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/http.py` & `std.algorithm-1.2.0/std/http.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/keras.py` & `std.algorithm-1.2.0/std/keras.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/lib/eigen.dll` & `std.algorithm-1.2.0/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/lib/libeigen.so` & `std.algorithm-1.2.0/std/lib/libeigen.so`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/nlp/__init__.py` & `std.algorithm-1.2.0/std/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/nlp/ner.py` & `std.algorithm-1.2.0/std/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/nlp/segment/cn.py` & `std.algorithm-1.2.0/std/nlp/segment/cn.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/nlp/segment/en.py` & `std.algorithm-1.2.0/std/nlp/segment/en.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/nlp/segment/jp.py` & `std.algorithm-1.2.0/std/nlp/segment/jp.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/search.py` & `std.algorithm-1.2.0/std/search.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/sets.py` & `std.algorithm-1.2.0/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/tree.py` & `std.algorithm-1.2.0/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std/xml.py` & `std.algorithm-1.2.0/std/xml.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.9/std.algorithm.egg-info/PKG-INFO` & `std.algorithm-1.2.0/std.algorithm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: std.algorithm
-Version: 1.1.9
+Version: 1.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Cosmos
 Author-email: 744984949@qq.com
 License: MIT
 Description: # std
```

### Comparing `std.algorithm-1.1.9/std.algorithm.egg-info/SOURCES.txt` & `std.algorithm-1.2.0/std.algorithm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

