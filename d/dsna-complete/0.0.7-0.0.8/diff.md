# Comparing `tmp/dsna_complete-0.0.7.tar.gz` & `tmp/dsna_complete-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.7.tar", last modified: Wed Jul  5 11:32:26 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.8.tar", last modified: Wed Jul  5 11:41:35 2023, max compression
```

## Comparing `dsna_complete-0.0.7.tar` & `dsna_complete-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:32:26.769135 dsna_complete-0.0.7/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:32:26.769180 dsna_complete-0.0.7/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:32:26.769038 dsna_complete-0.0.7/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.7/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      401 2023-07-05 11:32:26.769418 dsna_complete-0.0.7/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.7/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.518877 dsna_complete-0.0.8/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:41:35.518918 dsna_complete-0.0.8/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.8/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      438 2023-07-05 11:41:35.519148 dsna_complete-0.0.8/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.8/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.517892 dsna_complete-0.0.8/src/
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:41:35.518788 dsna_complete-0.0.8/src/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      237 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:41:35.000000 dsna_complete-0.0.8/src/dsna_complete.egg-info/top_level.txt
```

