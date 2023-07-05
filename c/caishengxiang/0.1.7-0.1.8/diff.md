# Comparing `tmp/caishengxiang-0.1.7.tar.gz` & `tmp/caishengxiang-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caishengxiang-0.1.7.tar", last modified: Wed Jul  5 16:26:13 2023, max compression
+gzip compressed data, was "caishengxiang-0.1.8.tar", last modified: Wed Jul  5 16:58:59 2023, max compression
```

## Comparing `caishengxiang-0.1.7.tar` & `caishengxiang-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.515972 caishengxiang-0.1.7/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      252 2023-07-05 16:26:13.508743 caishengxiang-0.1.7/PKG-INFO
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/README.rst
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.031909 caishengxiang-0.1.7/caishengxiang/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/__init__.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.477960 caishengxiang-0.1.7/caishengxiang/logger/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/logger/__init__.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     4705 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/logger/simple_log.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.692122 caishengxiang-0.1.7/caishengxiang/study/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/__init__.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1507 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/classs.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     2012 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/dicts.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.749344 caishengxiang-0.1.7/caishengxiang/utils/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/__init__.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.937012 caishengxiang-0.1.7/caishengxiang/utils/file_tools/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/file_tools/__init__.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      934 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/file_tools/chmod.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.047161 caishengxiang-0.1.7/caishengxiang/utils/str_tools/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/str_tools/__init__.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.417570 caishengxiang-0.1.7/caishengxiang/utils/time_tools/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/__init__.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1907 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_date.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1170 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_dateutil.py
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1606 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/time_type.py
-drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.315118 caishengxiang-0.1.7/caishengxiang.egg-info/
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      252 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/PKG-INFO
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      769 2023-07-05 16:26:11.000000 caishengxiang-0.1.7/caishengxiang.egg-info/SOURCES.txt
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        1 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/dependency_links.txt
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        1 2023-07-05 16:12:31.000000 caishengxiang-0.1.7/caishengxiang.egg-info/not-zip-safe
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        7 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/requires.txt
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       14 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/top_level.txt
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       39 2023-07-05 16:22:16.000000 caishengxiang-0.1.7/pyproject.toml
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       38 2023-07-05 16:26:13.518990 caishengxiang-0.1.7/setup.cfg
--rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1015 2023-07-05 16:26:07.000000 caishengxiang-0.1.7/setup.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:59.478664 caishengxiang-0.1.8/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      862 2023-07-05 16:58:59.471657 caishengxiang-0.1.8/PKG-INFO
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      568 2023-07-05 15:33:12.000000 caishengxiang-0.1.8/README.md
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/README.rst
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.113261 caishengxiang-0.1.8/caishengxiang/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       62 2023-07-05 16:37:05.000000 caishengxiang-0.1.8/caishengxiang/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.527435 caishengxiang-0.1.8/caishengxiang/logger/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/logger/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     4705 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/logger/simple_log.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.722344 caishengxiang-0.1.8/caishengxiang/study/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/study/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1507 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/study/classs.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     2012 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/study/dicts.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.766495 caishengxiang-0.1.8/caishengxiang/utils/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.929347 caishengxiang-0.1.8/caishengxiang/utils/file_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/file_tools/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      934 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/file_tools/chmod.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:59.021097 caishengxiang-0.1.8/caishengxiang/utils/str_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/str_tools/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:59.383817 caishengxiang-0.1.8/caishengxiang/utils/time_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/time_tools/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1907 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/time_tools/c_date.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1170 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/time_tools/c_dateutil.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1606 2023-07-05 15:32:07.000000 caishengxiang-0.1.8/caishengxiang/utils/time_tools/time_type.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:58:58.424350 caishengxiang-0.1.8/caishengxiang.egg-info/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      862 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/PKG-INFO
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      774 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        1 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       50 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/entry_points.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       42 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/requires.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       14 2023-07-05 16:58:57.000000 caishengxiang-0.1.8/caishengxiang.egg-info/top_level.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      726 2023-07-05 16:48:06.000000 caishengxiang-0.1.8/pyproject.toml
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       38 2023-07-05 16:58:59.481199 caishengxiang-0.1.8/setup.cfg
```

### Comparing `caishengxiang-0.1.7/caishengxiang/logger/simple_log.py` & `caishengxiang-0.1.8/caishengxiang/logger/simple_log.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/study/classs.py` & `caishengxiang-0.1.8/caishengxiang/study/classs.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/study/dicts.py` & `caishengxiang-0.1.8/caishengxiang/study/dicts.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/utils/file_tools/chmod.py` & `caishengxiang-0.1.8/caishengxiang/utils/file_tools/chmod.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_date.py` & `caishengxiang-0.1.8/caishengxiang/utils/time_tools/c_date.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_dateutil.py` & `caishengxiang-0.1.8/caishengxiang/utils/time_tools/c_dateutil.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang/utils/time_tools/time_type.py` & `caishengxiang-0.1.8/caishengxiang/utils/time_tools/time_type.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.7/caishengxiang.egg-info/SOURCES.txt` & `caishengxiang-0.1.8/caishengxiang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+README.md
 README.rst
 pyproject.toml
-setup.py
 caishengxiang/__init__.py
 caishengxiang.egg-info/PKG-INFO
 caishengxiang.egg-info/SOURCES.txt
 caishengxiang.egg-info/dependency_links.txt
-caishengxiang.egg-info/not-zip-safe
+caishengxiang.egg-info/entry_points.txt
 caishengxiang.egg-info/requires.txt
 caishengxiang.egg-info/top_level.txt
 caishengxiang/logger/__init__.py
 caishengxiang/logger/simple_log.py
 caishengxiang/study/__init__.py
 caishengxiang/study/classs.py
 caishengxiang/study/dicts.py
```

