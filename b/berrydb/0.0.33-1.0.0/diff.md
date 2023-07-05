# Comparing `tmp/berrydb-0.0.33.tar.gz` & `tmp/berrydb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berrydb-0.0.33.tar", last modified: Wed Jul  5 07:22:17 2023, max compression
+gzip compressed data, was "berrydb-1.0.0.tar", last modified: Wed Jul  5 05:03:26 2023, max compression
```

## Comparing `berrydb-0.0.33.tar` & `berrydb-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-05 07:22:17.354635 berrydb-0.0.33/
--rw-rw-r--   0 akash     (1000) akash     (1000)      556 2023-07-05 07:22:17.354635 berrydb-0.0.33/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      167 2023-07-05 05:51:47.000000 berrydb-0.0.33/README.md
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-05 07:22:17.354635 berrydb-0.0.33/berrydb.egg-info/
--rw-rw-r--   0 akash     (1000) akash     (1000)      556 2023-07-05 07:22:17.000000 berrydb-0.0.33/berrydb.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      172 2023-07-05 07:22:17.000000 berrydb-0.0.33/berrydb.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-05 07:22:17.000000 berrydb-0.0.33/berrydb.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-07-05 07:22:17.000000 berrydb-0.0.33/berrydb.egg-info/requires.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-05 07:22:17.000000 berrydb-0.0.33/berrydb.egg-info/top_level.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-07-05 07:22:17.354635 berrydb-0.0.33/setup.cfg
--rw-rw-r--   0 akash     (1000) akash     (1000)      507 2023-07-05 06:56:25.000000 berrydb-0.0.33/setup.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-05 05:03:26.452297 berrydb-1.0.0/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      206 2023-07-05 05:03:26.452297 berrydb-1.0.0/PKG-INFO
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2023-07-05 05:03:26.452297 berrydb-1.0.0/berrydb.egg-info/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      206 2023-07-05 05:03:26.000000 berrydb-1.0.0/berrydb.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      162 2023-07-05 05:03:26.000000 berrydb-1.0.0/berrydb.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-05 05:03:26.000000 berrydb-1.0.0/berrydb.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        9 2023-07-05 05:03:26.000000 berrydb-1.0.0/berrydb.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2023-07-05 05:03:26.000000 berrydb-1.0.0/berrydb.egg-info/top_level.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       38 2023-07-05 05:03:26.452297 berrydb-1.0.0/setup.cfg
+-rw-rw-r--   0 akash     (1000) akash     (1000)      265 2023-07-05 05:01:22.000000 berrydb-1.0.0/setup.py
```

