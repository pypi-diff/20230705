# Comparing `tmp/caishengxiang-0.1.6.tar.gz` & `tmp/caishengxiang-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caishengxiang-0.1.6.tar", last modified: Tue Dec  6 16:26:12 2022, max compression
+gzip compressed data, was "caishengxiang-0.1.7.tar", last modified: Wed Jul  5 16:26:13 2023, max compression
```

## Comparing `caishengxiang-0.1.6.tar` & `caishengxiang-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 16:26:12.415526 caishengxiang-0.1.6/
--rw-rw-rw-   0        0        0      311 2022-12-06 16:26:12.415526 caishengxiang-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-11-15 14:22:37.000000 caishengxiang-0.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-06 16:26:12.403128 caishengxiang-0.1.6/caishengxiang/
--rw-rw-rw-   0        0        0        0 2022-11-15 14:06:58.000000 caishengxiang-0.1.6/caishengxiang/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 16:26:12.413630 caishengxiang-0.1.6/caishengxiang/file_tools/
--rw-rw-rw-   0        0        0        0 2022-11-15 14:06:58.000000 caishengxiang-0.1.6/caishengxiang/file_tools/__init__.py
--rw-rw-rw-   0        0        0      934 2022-11-15 14:06:58.000000 caishengxiang-0.1.6/caishengxiang/file_tools/chmod.py
-drwxrwxrwx   0        0        0        0 2022-12-06 16:26:12.414062 caishengxiang-0.1.6/caishengxiang/logger/
--rw-rw-rw-   0        0        0        0 2022-11-15 14:06:58.000000 caishengxiang-0.1.6/caishengxiang/logger/__init__.py
--rw-rw-rw-   0        0        0     4705 2022-11-15 14:06:58.000000 caishengxiang-0.1.6/caishengxiang/logger/simple_log.py
-drwxrwxrwx   0        0        0        0 2022-12-06 16:26:12.412348 caishengxiang-0.1.6/caishengxiang.egg-info/
--rw-rw-rw-   0        0        0      311 2022-12-06 16:26:12.000000 caishengxiang-0.1.6/caishengxiang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2022-12-06 16:26:12.000000 caishengxiang-0.1.6/caishengxiang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-06 16:26:12.000000 caishengxiang-0.1.6/caishengxiang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-06 15:18:30.000000 caishengxiang-0.1.6/caishengxiang.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2022-12-06 16:26:12.000000 caishengxiang-0.1.6/caishengxiang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-12-06 16:26:12.000000 caishengxiang-0.1.6/caishengxiang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-06 16:26:12.416099 caishengxiang-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1015 2022-12-06 16:21:25.000000 caishengxiang-0.1.6/setup.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.515972 caishengxiang-0.1.7/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      252 2023-07-05 16:26:13.508743 caishengxiang-0.1.7/PKG-INFO
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/README.rst
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.031909 caishengxiang-0.1.7/caishengxiang/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.477960 caishengxiang-0.1.7/caishengxiang/logger/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/logger/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     4705 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/logger/simple_log.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.692122 caishengxiang-0.1.7/caishengxiang/study/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1507 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/classs.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     2012 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/study/dicts.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.749344 caishengxiang-0.1.7/caishengxiang/utils/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.937012 caishengxiang-0.1.7/caishengxiang/utils/file_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/file_tools/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      934 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/file_tools/chmod.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.047161 caishengxiang-0.1.7/caishengxiang/utils/str_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      166 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/str_tools/__init__.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:13.417570 caishengxiang-0.1.7/caishengxiang/utils/time_tools/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/__init__.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1907 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_date.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1170 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/c_dateutil.py
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1606 2023-07-05 15:32:07.000000 caishengxiang-0.1.7/caishengxiang/utils/time_tools/time_type.py
+drwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        0 2023-07-05 16:26:12.315118 caishengxiang-0.1.7/caishengxiang.egg-info/
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      252 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/PKG-INFO
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)      769 2023-07-05 16:26:11.000000 caishengxiang-0.1.7/caishengxiang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        1 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        1 2023-07-05 16:12:31.000000 caishengxiang-0.1.7/caishengxiang.egg-info/not-zip-safe
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)        7 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/requires.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       14 2023-07-05 16:26:10.000000 caishengxiang-0.1.7/caishengxiang.egg-info/top_level.txt
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       39 2023-07-05 16:22:16.000000 caishengxiang-0.1.7/pyproject.toml
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)       38 2023-07-05 16:26:13.518990 caishengxiang-0.1.7/setup.cfg
+-rwxrwxrwx   0 caishengxiang  (1000) caishengxiang  (1000)     1015 2023-07-05 16:26:07.000000 caishengxiang-0.1.7/setup.py
```

### Comparing `caishengxiang-0.1.6/caishengxiang/file_tools/chmod.py` & `caishengxiang-0.1.7/caishengxiang/utils/file_tools/chmod.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.6/caishengxiang/logger/simple_log.py` & `caishengxiang-0.1.7/caishengxiang/logger/simple_log.py`

 * *Files identical despite different names*

### Comparing `caishengxiang-0.1.6/setup.py` & `caishengxiang-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     entry_points={
 
     },
     packages=find_packages(include=['caishengxiang', 'caishengxiang.*']),
     test_sutie='test',
     test_require=test_requirements,
     url='https://github.com/caishengxiang/caishengxiang',
-    version='0.1.6',
+    version='0.1.7',
     zip_safe=False
 )
```

