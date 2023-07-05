# Comparing `tmp/interval-search-0.5.1.tar.gz` & `tmp/interval-search-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval-search-0.5.1.tar", last modified: Tue Jul  4 05:48:30 2023, max compression
+gzip compressed data, was "interval-search-0.5.2.tar", last modified: Wed Jul  5 09:40:00 2023, max compression
```

## Comparing `interval-search-0.5.1.tar` & `interval-search-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.800614 interval-search-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 05:48:19.000000 interval-search-0.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-04 05:48:19.000000 interval-search-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 05:48:19.000000 interval-search-0.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 05:48:19.000000 interval-search-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 05:48:19.000000 interval-search-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 05:48:30.800614 interval-search-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 05:48:19.000000 interval-search-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-04 05:48:19.000000 interval-search-0.5.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/interval_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 05:48:19.000000 interval-search-0.5.1/interval_search/interval_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.796615 interval-search-0.5.1/interval_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-04 05:48:30.000000 interval-search-0.5.1/interval_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-04 05:48:30.800614 interval-search-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 05:48:19.000000 interval-search-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 05:48:30.800614 interval-search-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_binary_search_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_binary_search_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_curried_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_doubling_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 05:48:19.000000 interval-search-0.5.1/tests/test_interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:40:00.849107 interval-search-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 09:39:48.000000 interval-search-0.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-05 09:39:48.000000 interval-search-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 09:39:48.000000 interval-search-0.5.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 09:39:48.000000 interval-search-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-05 09:39:48.000000 interval-search-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-05 09:40:00.849107 interval-search-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 09:39:48.000000 interval-search-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:40:00.849107 interval-search-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 09:39:48.000000 interval-search-0.5.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:40:00.849107 interval-search-0.5.2/interval_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/curried_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-05 09:39:48.000000 interval-search-0.5.2/interval_search/interval_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:40:00.849107 interval-search-0.5.2/interval_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-05 09:40:00.000000 interval-search-0.5.2/interval_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 09:40:00.000000 interval-search-0.5.2/interval_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:40:00.000000 interval-search-0.5.2/interval_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:40:00.000000 interval-search-0.5.2/interval_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 09:40:00.000000 interval-search-0.5.2/interval_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 09:40:00.849107 interval-search-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 09:39:48.000000 interval-search-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:40:00.849107 interval-search-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_binary_search_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_curried_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_curried_binary_search_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_curried_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_doubling_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-05 09:39:48.000000 interval-search-0.5.2/tests/test_interval_search.py
```

### Comparing `interval-search-0.5.1/CONTRIBUTING.rst` & `interval-search-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/LICENSE` & `interval-search-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/PKG-INFO` & `interval-search-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.5.1
+Version: 0.5.2
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.5.1/README.rst` & `interval-search-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/docs/Makefile` & `interval-search-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/docs/conf.py` & `interval-search-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/docs/installation.rst` & `interval-search-0.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/docs/make.bat` & `interval-search-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/__init__.py` & `interval-search-0.5.2/interval_search/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for interval_search."""
 
 __author__ = """Matthew Andres Moreno"""
 __email__ = 'm.more500@gmail.com'
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 from .binary_search import binary_search
 from .binary_search_iterative import binary_search_iterative
 from .binary_search_recursive import binary_search_recursive
 from .curried_binary_search import curried_binary_search
 from .curried_binary_search_iterative import curried_binary_search_iterative
 from .curried_binary_search_recursive import curried_binary_search_recursive
```

### Comparing `interval-search-0.5.1/interval_search/binary_search_iterative.py` & `interval-search-0.5.2/interval_search/binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/binary_search_recursive.py` & `interval-search-0.5.2/interval_search/binary_search_recursive.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/curried_binary_search_iterative.py` & `interval-search-0.5.2/interval_search/curried_binary_search_iterative.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,32 +49,29 @@
         Returns
         -------
         guess
             The lowest integer value that satisfies the search criteria, and
             None if upper_bound does not satisfy the search criteria or search
             range is empty (i.e., lower_bound > upper_bound).
         """
-
-        # Check if the range is invalid.
-        if lower_bound > upper_bound:
-            return None
-
-        # Loop until lower_bound is greater than upper_bound
-        while lower_bound <= upper_bound:
+        # Loop until lower_bound is greater than or equal to upper_bound
+        while lower_bound < upper_bound:
             # Find the midpoint
             midpoint = (lower_bound + upper_bound) >> 1  # equiv // 2
 
-            # If predicate is satisfied by midpoint, search the left half.
             if predicate(midpoint):
-                upper_bound = midpoint - 1
-            # Otherwise, search the right half.
+                upper_bound = midpoint
             else:
                 lower_bound = midpoint + 1
 
         # If the search ended successfully, lower_bound is the answer.
         # Otherwise, return None.
-        if predicate(lower_bound):
-            return lower_bound
-        else:
+        if lower_bound > upper_bound:
             return None
+        if lower_bound == upper_bound:
+            if predicate(lower_bound):
+                return lower_bound
+            else:
+                return None
+
 
     return binary_search_iterative
```

### Comparing `interval-search-0.5.1/interval_search/curried_binary_search_recursive.py` & `interval-search-0.5.2/interval_search/curried_binary_search_recursive.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/curried_doubling_search.py` & `interval-search-0.5.2/interval_search/curried_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/doubling_search.py` & `interval-search-0.5.2/interval_search/doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search/interval_search.py` & `interval-search-0.5.2/interval_search/interval_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/interval_search.egg-info/PKG-INFO` & `interval-search-0.5.2/interval_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: interval-search
-Version: 0.5.1
+Version: 0.5.2
 Summary: interval-search provides predicate-based binary and doubling search implementations
 Home-page: https://github.com/mmore500/interval-search
 Author: Matthew Andres Moreno
 Author-email: m.more500@gmail.com
 License: MIT license
 Description: ===============
         interval-search
```

### Comparing `interval-search-0.5.1/interval_search.egg-info/SOURCES.txt` & `interval-search-0.5.2/interval_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/setup.py` & `interval-search-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     keywords='interval-search',
     name='interval-search',
     packages=find_packages(include=['interval_search', 'interval_search.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mmore500/interval-search',
-    version='0.5.1',
+    version='0.5.2',
     zip_safe=False,
 )
```

### Comparing `interval-search-0.5.1/tests/test_binary_search.py` & `interval-search-0.5.2/tests/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_binary_search_iterative.py` & `interval-search-0.5.2/tests/test_binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_binary_search_recursive.py` & `interval-search-0.5.2/tests/test_binary_search_recursive.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_curried_binary_search.py` & `interval-search-0.5.2/tests/test_curried_binary_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_curried_binary_search_iterative.py` & `interval-search-0.5.2/tests/test_curried_binary_search_iterative.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_curried_doubling_search.py` & `interval-search-0.5.2/tests/test_curried_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_doubling_search.py` & `interval-search-0.5.2/tests/test_doubling_search.py`

 * *Files identical despite different names*

### Comparing `interval-search-0.5.1/tests/test_interval_search.py` & `interval-search-0.5.2/tests/test_interval_search.py`

 * *Files identical despite different names*

