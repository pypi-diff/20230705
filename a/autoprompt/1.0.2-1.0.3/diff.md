# Comparing `tmp/autoprompt-1.0.2.tar.gz` & `tmp/autoprompt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoprompt-1.0.2.tar", last modified: Wed Jul  5 17:45:25 2023, max compression
+gzip compressed data, was "autoprompt-1.0.3.tar", last modified: Wed Jul  5 17:49:03 2023, max compression
```

## Comparing `autoprompt-1.0.2.tar` & `autoprompt-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 17:45:25.513688 autoprompt-1.0.2/
--rw-rw-rw-   0        0        0      164 2023-07-05 17:45:25.513688 autoprompt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-05 17:44:57.000000 autoprompt-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 17:45:25.498021 autoprompt-1.0.2/autoprompt/
--rw-rw-rw-   0        0        0       45 2023-07-05 17:41:42.000000 autoprompt-1.0.2/autoprompt/__init__.py
--rw-rw-rw-   0        0        0       45 2023-07-05 17:41:34.000000 autoprompt-1.0.2/autoprompt/app.py
-drwxrwxrwx   0        0        0        0 2023-07-05 17:45:25.513688 autoprompt-1.0.2/autoprompt.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-05 17:45:25.000000 autoprompt-1.0.2/autoprompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-05 17:45:25.000000 autoprompt-1.0.2/autoprompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 17:45:25.000000 autoprompt-1.0.2/autoprompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 17:45:25.000000 autoprompt-1.0.2/autoprompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 17:45:25.000000 autoprompt-1.0.2/autoprompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 17:45:25.513688 autoprompt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-07-05 17:44:15.000000 autoprompt-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 17:49:03.892326 autoprompt-1.0.3/
+-rw-rw-rw-   0        0        0      164 2023-07-05 17:49:03.892326 autoprompt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-05 17:44:57.000000 autoprompt-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 17:49:03.871158 autoprompt-1.0.3/autoprompt/
+-rw-rw-rw-   0        0        0       45 2023-07-05 17:41:42.000000 autoprompt-1.0.3/autoprompt/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-07-05 17:41:34.000000 autoprompt-1.0.3/autoprompt/app.py
+drwxrwxrwx   0        0        0        0 2023-07-05 17:49:03.892326 autoprompt-1.0.3/autoprompt.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-05 17:49:03.000000 autoprompt-1.0.3/autoprompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-05 17:49:03.000000 autoprompt-1.0.3/autoprompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 17:49:03.000000 autoprompt-1.0.3/autoprompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-05 17:49:03.000000 autoprompt-1.0.3/autoprompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 17:49:03.000000 autoprompt-1.0.3/autoprompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 17:49:03.892326 autoprompt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      296 2023-07-05 17:48:17.000000 autoprompt-1.0.3/setup.py
```

