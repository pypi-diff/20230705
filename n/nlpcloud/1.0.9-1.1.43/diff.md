# Comparing `tmp/nlpcloud-1.0.9.tar.gz` & `tmp/nlpcloud-1.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpcloud-1.0.9.tar", last modified: Tue Apr 27 14:32:13 2021, max compression
+gzip compressed data, was "nlpcloud-1.1.43.tar", last modified: Wed Jul  5 06:26:03 2023, max compression
```

## Comparing `nlpcloud-1.0.9.tar` & `nlpcloud-1.1.43.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      792 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4529 2021-04-27 14:32:00.000000 nlpcloud-1.0.9/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/nlpcloud/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2756 2021-04-27 14:31:18.000000 nlpcloud-1.0.9/nlpcloud/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/nlpcloud.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      792 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      167 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2021-04-27 14:32:12.000000 nlpcloud-1.0.9/nlpcloud.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2021-04-27 14:32:13.368677 nlpcloud-1.0.9/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      855 2021-04-27 14:30:53.000000 nlpcloud-1.0.9/setup.py
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1053 2021-01-19 13:02:30.000000 nlpcloud-1.1.43/LICENSE
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/PKG-INFO
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    16934 2023-06-05 09:52:34.000000 nlpcloud-1.1.43/README.md
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/nlpcloud/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)    13808 2023-06-27 09:40:51.000000 nlpcloud-1.1.43/nlpcloud/__init__.py
+drwxrwxr-x   0 juliensalinas  (1000) juliensalinas  (1000)        0 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/nlpcloud.egg-info/
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)     1109 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/PKG-INFO
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)      206 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        1 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/requires.txt
+-rw-r--r--   0 juliensalinas  (1000) juliensalinas  (1000)        9 2023-07-05 06:26:03.000000 nlpcloud-1.1.43/nlpcloud.egg-info/top_level.txt
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)       38 2023-07-05 06:26:03.449042 nlpcloud-1.1.43/setup.cfg
+-rw-rw-r--   0 juliensalinas  (1000) juliensalinas  (1000)     1257 2023-07-05 06:25:23.000000 nlpcloud-1.1.43/setup.py
```

