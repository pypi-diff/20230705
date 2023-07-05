# Comparing `tmp/meta-example-0.0.5.tar.gz` & `tmp/meta-example-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-example-0.0.5.tar", last modified: Wed Jul  5 11:02:20 2023, max compression
+gzip compressed data, was "dist/meta-example-0.0.6.tar", last modified: Wed Jul  5 11:05:21 2023, max compression
```

## Comparing `meta-example-0.0.5.tar` & `meta-example-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 11:02:20.000000 meta-example-0.0.5/
--rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 11:02:20.000000 meta-example-0.0.5/PKG-INFO
-drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 11:02:20.000000 meta-example-0.0.5/meta_example.egg-info/
--rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 11:02:20.000000 meta-example-0.0.5/meta_example.egg-info/PKG-INFO
--rw-r--r--   0 chaihj15   (501) staff       (20)      152 2023-07-05 11:02:20.000000 meta-example-0.0.5/meta_example.egg-info/SOURCES.txt
--rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 11:02:20.000000 meta-example-0.0.5/meta_example.egg-info/top_level.txt
--rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 11:02:20.000000 meta-example-0.0.5/meta_example.egg-info/dependency_links.txt
--rw-r--r--   0 chaihj15   (501) staff       (20)       88 2023-07-05 11:01:59.000000 meta-example-0.0.5/setup.py
--rw-r--r--   0 chaihj15   (501) staff       (20)       38 2023-07-05 11:02:20.000000 meta-example-0.0.5/setup.cfg
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 11:05:21.000000 meta-example-0.0.6/
+-rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 11:05:21.000000 meta-example-0.0.6/PKG-INFO
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 11:05:21.000000 meta-example-0.0.6/meta_example.egg-info/
+-rw-r--r--   0 chaihj15   (501) staff       (20)      137 2023-07-05 11:05:20.000000 meta-example-0.0.6/meta_example.egg-info/PKG-INFO
+-rw-r--r--   0 chaihj15   (501) staff       (20)      152 2023-07-05 11:05:20.000000 meta-example-0.0.6/meta_example.egg-info/SOURCES.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 11:05:20.000000 meta-example-0.0.6/meta_example.egg-info/top_level.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 11:05:20.000000 meta-example-0.0.6/meta_example.egg-info/dependency_links.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)       88 2023-07-05 11:05:07.000000 meta-example-0.0.6/setup.py
+-rw-r--r--   0 chaihj15   (501) staff       (20)       38 2023-07-05 11:05:21.000000 meta-example-0.0.6/setup.cfg
```

