# Comparing `tmp/dexcolor-0.1.2.tar.gz` & `tmp/dexcolor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexcolor-0.1.2.tar", last modified: Sat Jul  1 14:16:38 2023, max compression
+gzip compressed data, was "dexcolor-0.2.0.tar", last modified: Wed Jul  5 13:32:18 2023, max compression
```

## Comparing `dexcolor-0.1.2.tar` & `dexcolor-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 14:16:38.395317 dexcolor-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-06-27 17:24:27.000000 dexcolor-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4115 2023-07-01 14:16:38.395317 dexcolor-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3541 2023-06-28 15:06:59.000000 dexcolor-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 14:16:38.363095 dexcolor-0.1.2/dexcolor/
--rw-rw-rw-   0        0        0      130 2023-06-28 09:54:49.000000 dexcolor-0.1.2/dexcolor/__init__.py
--rw-rw-rw-   0        0        0     4167 2023-06-27 13:05:05.000000 dexcolor-0.1.2/dexcolor/background.py
--rw-rw-rw-   0        0        0     7117 2023-06-27 13:00:01.000000 dexcolor-0.1.2/dexcolor/dex.py
--rw-rw-rw-   0        0        0     2984 2023-06-28 10:14:06.000000 dexcolor-0.1.2/dexcolor/rt.py
--rw-rw-rw-   0        0        0     1682 2023-06-27 12:37:02.000000 dexcolor-0.1.2/dexcolor/styles.py
-drwxrwxrwx   0        0        0        0 2023-07-01 14:16:38.385681 dexcolor-0.1.2/dexcolor.egg-info/
--rw-rw-rw-   0        0        0     4115 2023-07-01 14:16:38.000000 dexcolor-0.1.2/dexcolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-01 14:16:38.000000 dexcolor-0.1.2/dexcolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:16:38.000000 dexcolor-0.1.2/dexcolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-01 14:16:38.000000 dexcolor-0.1.2/dexcolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      646 2023-07-01 14:14:15.000000 dexcolor-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 14:16:38.395317 dexcolor-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 13:32:18.433608 dexcolor-0.2.0/
+-rw-rw-rw-   0        0        0     1085 2023-07-05 13:15:38.000000 dexcolor-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3344 2023-07-05 13:32:18.431244 dexcolor-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2722 2023-07-05 12:37:42.000000 dexcolor-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 13:32:18.390864 dexcolor-0.2.0/dexcolor/
+-rw-rw-rw-   0        0        0     3903 2023-07-05 08:51:54.000000 dexcolor-0.2.0/dexcolor/Ansi.py
+-rw-rw-rw-   0        0        0      130 2023-07-05 08:38:31.000000 dexcolor-0.2.0/dexcolor/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-07-05 08:35:11.000000 dexcolor-0.2.0/dexcolor/ansitowin32.py
+-rw-rw-rw-   0        0        0     1325 2023-07-05 08:53:12.000000 dexcolor-0.2.0/dexcolor/initialize.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:32:18.429249 dexcolor-0.2.0/dexcolor/tests/
+-rw-rw-rw-   0        0        0     1329 2023-07-05 13:09:49.000000 dexcolor-0.2.0/dexcolor/tests/test_dexcolor.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:32:18.423159 dexcolor-0.2.0/dexcolor.egg-info/
+-rw-rw-rw-   0        0        0     3344 2023-07-05 13:32:18.000000 dexcolor-0.2.0/dexcolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-07-05 13:32:18.000000 dexcolor-0.2.0/dexcolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:32:18.000000 dexcolor-0.2.0/dexcolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 13:32:18.000000 dexcolor-0.2.0/dexcolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2023-07-05 12:37:06.000000 dexcolor-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:32:18.433608 dexcolor-0.2.0/setup.cfg
```

### Comparing `dexcolor-0.1.2/LICENSE` & `dexcolor-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Terong33
+Copyright (c) 2017 Terong333
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dexcolor-0.1.2/pyproject.toml` & `dexcolor-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dexcolor"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Terong333", email="thisterong33@proton.me" },
 ]
-description = "Terminal colored text."
+description = "A Python package for adding color and style to terminal text output"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Terminals",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Terong33/dexcolor"
-"PyPI_page" = "https://pypi.org/project/dexcolor/"
+"Homepage" = "https://github.com/Terong33/dexcolor/"
+"PyPI_page" = "https://pypi.org/project/dexcolor/"
```

