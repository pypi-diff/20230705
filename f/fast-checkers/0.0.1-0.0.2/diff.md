# Comparing `tmp/fast-checkers-0.0.1.tar.gz` & `tmp/fast-checkers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.0.1.tar", last modified: Tue Jul  4 22:05:41 2023, max compression
+gzip compressed data, was "fast-checkers-0.0.2.tar", last modified: Tue Jul  4 22:18:46 2023, max compression
```

## Comparing `fast-checkers-0.0.1.tar` & `fast-checkers-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/american_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/base_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/checkers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/fast_checkers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-04 22:05:41.000000 fast-checkers-0.0.1/fast_checkers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 22:05:41.000000 fast-checkers-0.0.1/fast_checkers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:05:41.000000 fast-checkers-0.0.1/fast_checkers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 22:05:41.000000 fast-checkers-0.0.1/fast_checkers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:05:41.354358 fast-checkers-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-04 22:05:31.000000 fast-checkers-0.0.1/test/test_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/american_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/base_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/checkers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/fast_checkers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 22:18:46.000000 fast-checkers-0.0.2/fast_checkers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:18:46.825040 fast-checkers-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-04 22:18:36.000000 fast-checkers-0.0.2/test/test_board.py
```

### Comparing `fast-checkers-0.0.1/checkers/__init__.py` & `fast-checkers-0.0.2/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.1/checkers/american_board.py` & `fast-checkers-0.0.2/checkers/american_board.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.1/checkers/base_board.py` & `fast-checkers-0.0.2/checkers/base_board.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.1/checkers/main.py` & `fast-checkers-0.0.2/checkers/main.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.1/checkers/models.py` & `fast-checkers-0.0.2/checkers/models.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.0.1/test/test_board.py` & `fast-checkers-0.0.2/test/test_board.py`

 * *Files identical despite different names*

