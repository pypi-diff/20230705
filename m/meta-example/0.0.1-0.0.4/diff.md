# Comparing `tmp/meta_example-0.0.1.tar.gz` & `tmp/meta-example-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\meta_example-0.0.1.tar", last modified: Tue Mar  7 08:36:41 2023, max compression
+gzip compressed data, was "dist/meta-example-0.0.4.tar", last modified: Wed Jul  5 09:31:46 2023, max compression
```

## Comparing `meta_example-0.0.1.tar` & `meta-example-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 08:36:41.000000 meta_example-0.0.1/
--rw-rw-rw-   0        0        0      225 2023-03-07 08:36:41.000000 meta_example-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-07 08:36:41.000000 meta_example-0.0.1/meta_example.egg-info/
--rw-rw-rw-   0        0        0      225 2023-03-07 08:36:41.000000 meta_example-0.0.1/meta_example.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-03-07 08:36:41.000000 meta_example-0.0.1/meta_example.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 08:36:41.000000 meta_example-0.0.1/meta_example.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 08:36:41.000000 meta_example-0.0.1/meta_example.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 08:36:41.000000 meta_example-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      112 2023-03-07 08:36:38.000000 meta_example-0.0.1/setup.py
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 09:31:46.000000 meta-example-0.0.4/
+-rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 09:31:46.000000 meta-example-0.0.4/PKG-INFO
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 09:31:46.000000 meta-example-0.0.4/meta_example.egg-info/
+-rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 09:31:46.000000 meta-example-0.0.4/meta_example.egg-info/PKG-INFO
+-rw-r--r--   0 chaihj15   (501) staff       (20)      152 2023-07-05 09:31:46.000000 meta-example-0.0.4/meta_example.egg-info/SOURCES.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 09:31:46.000000 meta-example-0.0.4/meta_example.egg-info/top_level.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 09:31:46.000000 meta-example-0.0.4/meta_example.egg-info/dependency_links.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)       88 2023-07-05 09:30:35.000000 meta-example-0.0.4/setup.py
+-rw-r--r--   0 chaihj15   (501) staff       (20)       38 2023-07-05 09:31:46.000000 meta-example-0.0.4/setup.cfg
```

