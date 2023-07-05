# Comparing `tmp/dsna_complete-0.0.3.tar.gz` & `tmp/dsna_complete-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsna_complete-0.0.3.tar", last modified: Wed Jul  5 07:46:32 2023, max compression
+gzip compressed data, was "dsna_complete-0.0.4.tar", last modified: Wed Jul  5 11:08:30 2023, max compression
```

## Comparing `dsna_complete-0.0.3.tar` & `dsna_complete-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,11 @@
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.999175 dsna_complete-0.0.3/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-05 07:46:31.999261 dsna_complete-0.0.3/PKG-INFO
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.996493 dsna_complete-0.0.3/automl/
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)        0 2023-06-08 03:05:14.000000 dsna_complete-0.0.3/automl/__init__.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.996592 dsna_complete-0.0.3/automl/preservice/
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.997330 dsna_complete-0.0.3/automl/preservice/VIP/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     3461 2023-07-05 07:01:10.000000 dsna_complete-0.0.3/automl/preservice/VIP/eda.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)     6035 2023-07-05 07:29:39.000000 dsna_complete-0.0.3/automl/preservice/VIP/test.py
--rw-rw-r--   0 enisbaskapan   (501) staff       (20)    19917 2023-07-05 07:16:53.000000 dsna_complete-0.0.3/automl/preservice/VIP/train.py
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     1059 2023-07-05 07:29:48.000000 dsna_complete-0.0.3/automl/preservice/conclude.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.997866 dsna_complete-0.0.3/automl/utils/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     3439 2023-07-05 07:01:33.000000 dsna_complete-0.0.3/automl/utils/operate.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.995946 dsna_complete-0.0.3/base/
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.998106 dsna_complete-0.0.3/base/utils/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)     3335 2023-07-05 07:06:34.000000 dsna_complete-0.0.3/base/utils/servant.py
-drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 07:46:31.999072 dsna_complete-0.0.3/dsna_complete.egg-info/
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      141 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/PKG-INFO
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      402 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/SOURCES.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/dependency_links.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/requires.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       17 2023-07-05 07:46:31.000000 dsna_complete-0.0.3/dsna_complete.egg-info/top_level.txt
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.3/pyproject.toml
--rw-r--r--   0 enisbaskapan   (501) staff       (20)      371 2023-07-05 07:46:31.999563 dsna_complete-0.0.3/setup.cfg
--rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.3/setup.py
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:08:30.671326 dsna_complete-0.0.4/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:08:30.671369 dsna_complete-0.0.4/PKG-INFO
+drwxr-xr-x   0 enisbaskapan   (501) staff       (20)        0 2023-07-05 11:08:30.671235 dsna_complete-0.0.4/dsna_complete.egg-info/
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      157 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/PKG-INFO
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      217 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/SOURCES.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/dependency_links.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      126 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/requires.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)        1 2023-07-05 11:08:30.000000 dsna_complete-0.0.4/dsna_complete.egg-info/top_level.txt
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       80 2023-06-15 10:49:00.000000 dsna_complete-0.0.4/pyproject.toml
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)      378 2023-07-05 11:08:30.671601 dsna_complete-0.0.4/setup.cfg
+-rw-r--r--   0 enisbaskapan   (501) staff       (20)       37 2023-06-15 13:11:52.000000 dsna_complete-0.0.4/setup.py
```

