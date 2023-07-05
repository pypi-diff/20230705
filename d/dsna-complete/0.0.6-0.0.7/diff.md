# Comparing `tmp/dsna_complete-0.0.6.tar.gz` & `tmp/dsna_complete-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.6.tar", last modified: Wed Jul  5 11:24:01 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.7.tar", last modified: Wed Jul  5 11:32:26 2023, max compression
```

## Comparing `dsna_complete-0.0.6.tar` & `dsna_complete-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:24:01.781904 dsna_complete-0.0.6/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:24:01.781952 dsna_complete-0.0.6/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:24:01.781812 dsna_complete-0.0.6/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:24:01.000000 dsna_complete-0.0.6/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:24:01.000000 dsna_complete-0.0.6/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:24:01.000000 dsna_complete-0.0.6/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:24:01.000000 dsna_complete-0.0.6/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:24:01.000000 dsna_complete-0.0.6/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.6/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      379 2023-07-05 11:24:01.782169 dsna_complete-0.0.6/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.6/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:32:26.769135 dsna_complete-0.0.7/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:32:26.769180 dsna_complete-0.0.7/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:32:26.769038 dsna_complete-0.0.7/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      158 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:32:26.000000 dsna_complete-0.0.7/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.7/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      401 2023-07-05 11:32:26.769418 dsna_complete-0.0.7/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.7/setup.py
```

