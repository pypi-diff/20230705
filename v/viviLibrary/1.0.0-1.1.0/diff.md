# Comparing `tmp/viviLibrary-1.0.0.tar.gz` & `tmp/viviLibrary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viviLibrary-1.0.0.tar", last modified: Wed Jul  5 14:56:07 2023, max compression
+gzip compressed data, was "viviLibrary-1.1.0.tar", last modified: Wed Jul  5 17:11:52 2023, max compression
```

## Comparing `viviLibrary-1.0.0.tar` & `viviLibrary-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:56:07.408929 viviLibrary-1.0.0/
--rw-rw-rw-   0        0        0      123 2023-07-05 14:56:07.407618 viviLibrary-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-07-05 14:23:17.000000 viviLibrary-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 14:56:07.408929 viviLibrary-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      236 2023-07-05 14:54:44.000000 viviLibrary-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:56:07.405492 viviLibrary-1.0.0/viviLibrary.egg-info/
--rw-rw-rw-   0        0        0      123 2023-07-05 14:56:07.000000 viviLibrary-1.0.0/viviLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-07-05 14:56:07.000000 viviLibrary-1.0.0/viviLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:56:07.000000 viviLibrary-1.0.0/viviLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:56:07.000000 viviLibrary-1.0.0/viviLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 17:11:52.351939 viviLibrary-1.1.0/
+-rw-rw-rw-   0        0        0      123 2023-07-05 17:11:52.350340 viviLibrary-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2023-07-05 14:23:17.000000 viviLibrary-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 17:11:52.351939 viviLibrary-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      236 2023-07-05 17:11:45.000000 viviLibrary-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 17:11:52.346702 viviLibrary-1.1.0/viviLibrary.egg-info/
+-rw-rw-rw-   0        0        0      123 2023-07-05 17:11:52.000000 viviLibrary-1.1.0/viviLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-07-05 17:11:52.000000 viviLibrary-1.1.0/viviLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 17:11:52.000000 viviLibrary-1.1.0/viviLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 17:11:52.000000 viviLibrary-1.1.0/viviLibrary.egg-info/top_level.txt
```

### Comparing `viviLibrary-1.0.0/README.md` & `viviLibrary-1.1.0/README.md`

 * *Files identical despite different names*

