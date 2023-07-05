# Comparing `tmp/dsna_complete-0.0.4.tar.gz` & `tmp/dsna_complete-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.4.tar", last modified: Wed Jul  5 11:08:30 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.5.tar", last modified: Wed Jul  5 11:19:34 2023, max compression
```

## Comparing `dsna_complete-0.0.4.tar` & `dsna_complete-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:08:30.671326 dsna_complete-0.0.4/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:08:30.671369 dsna_complete-0.0.4/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:08:30.671235 dsna_complete-0.0.4/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.4/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      378 2023-07-05 11:08:30.671601 dsna_complete-0.0.4/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.4/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:19:34.838558 dsna_complete-0.0.5/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:19:34.838610 dsna_complete-0.0.5/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:19:34.838456 dsna_complete-0.0.5/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:19:34.000000 dsna_complete-0.0.5/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:19:34.000000 dsna_complete-0.0.5/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:19:34.000000 dsna_complete-0.0.5/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:19:34.000000 dsna_complete-0.0.5/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:19:34.000000 dsna_complete-0.0.5/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.5/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      378 2023-07-05 11:19:34.838860 dsna_complete-0.0.5/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.5/setup.py
```

