# Comparing `tmp/dsna_complete-0.0.8.tar.gz` & `tmp/dsna_complete-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.8.tar", last modified: Wed Jul  5 11:41:35 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.9.tar", last modified: Wed Jul  5 11:52:17 2023, max compression
```

## Comparing `dsna_complete-0.0.8.tar` & `dsna_complete-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.518877 dsna_complete-0.0.8/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:41:35.518918 dsna_complete-0.0.8/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.8/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      438 2023-07-05 11:41:35.519148 dsna_complete-0.0.8/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.8/setup.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.517892 dsna_complete-0.0.8/src/
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.518788 dsna_complete-0.0.8/src/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      237 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/top_level.txt
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:17.288324 dsna_complete-0.0.9/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:52:17.288368 dsna_complete-0.0.9/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:17.287490 dsna_complete-0.0.9/dsna_complete/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:50:47.000000 dsna_complete-0.0.9/dsna_complete/__init__.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:17.288161 dsna_complete-0.0.9/dsna_complete/automl/
+-rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.9/dsna_complete/automl/__init__.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:17.288256 dsna_complete-0.0.9/dsna_complete/base/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:05.000000 dsna_complete-0.0.9/dsna_complete/base/__ init__.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:52:17.288046 dsna_complete-0.0.9/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:52:17.000000 dsna_complete-0.0.9/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      308 2023-07-05 11:52:17.000000 dsna_complete-0.0.9/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:52:17.000000 dsna_complete-0.0.9/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:52:17.000000 dsna_complete-0.0.9/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       14 2023-07-05 11:52:17.000000 dsna_complete-0.0.9/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.9/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      431 2023-07-05 11:52:17.288591 dsna_complete-0.0.9/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.9/setup.py
```

