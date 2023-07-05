# Comparing `tmp/hlagenie-0.0.2.tar.gz` & `tmp/hlagenie-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlagenie-0.0.2.tar", last modified: Wed Jul  5 18:03:47 2023, max compression
+gzip compressed data, was "hlagenie-0.0.3.tar", last modified: Wed Jul  5 19:42:39 2023, max compression
```

## Comparing `hlagenie-0.0.2.tar` & `hlagenie-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 nomad     (1000) nomad     (1000)        0 2023-07-05 18:03:47.168063 hlagenie-0.0.2/
--rw-r--r--   0 nomad     (1000) nomad     (1000)    35149 2023-06-23 00:09:54.000000 hlagenie-0.0.2/LICENSE
--rw-r--r--   0 nomad     (1000) nomad     (1000)      281 2023-07-05 17:37:50.000000 hlagenie-0.0.2/MANIFEST.in
--rw-r--r--   0 nomad     (1000) nomad     (1000)     1570 2023-07-05 18:03:47.168063 hlagenie-0.0.2/PKG-INFO
--rw-r--r--   0 nomad     (1000) nomad     (1000)      908 2023-07-05 17:31:06.000000 hlagenie-0.0.2/README.md
-drwxr-xr-x   0 nomad     (1000) nomad     (1000)        0 2023-07-05 18:03:47.168063 hlagenie-0.0.2/hlagenie/
--rw-r--r--   0 nomad     (1000) nomad     (1000)      443 2023-07-05 17:49:32.000000 hlagenie-0.0.2/hlagenie/__init__.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)      127 2023-07-04 18:19:47.000000 hlagenie-0.0.2/hlagenie/configs.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     7364 2023-07-05 00:24:20.000000 hlagenie-0.0.2/hlagenie/data_repository.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     9550 2023-07-05 00:03:43.000000 hlagenie-0.0.2/hlagenie/db.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     6220 2023-07-05 00:31:18.000000 hlagenie-0.0.2/hlagenie/genie.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     1358 2023-07-04 19:15:14.000000 hlagenie-0.0.2/hlagenie/load.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     2795 2023-07-05 00:24:16.000000 hlagenie-0.0.2/hlagenie/misc.py
--rw-r--r--   0 nomad     (1000) nomad     (1000)     2481 2023-06-30 19:41:22.000000 hlagenie-0.0.2/hlagenie/smart_sort.py
-drwxr-xr-x   0 nomad     (1000) nomad     (1000)        0 2023-07-05 18:03:47.168063 hlagenie-0.0.2/hlagenie.egg-info/
--rw-r--r--   0 nomad     (1000) nomad     (1000)     1570 2023-07-05 18:03:47.000000 hlagenie-0.0.2/hlagenie.egg-info/PKG-INFO
--rw-r--r--   0 nomad     (1000) nomad     (1000)      437 2023-07-05 18:03:47.000000 hlagenie-0.0.2/hlagenie.egg-info/SOURCES.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)        1 2023-07-05 18:03:47.000000 hlagenie-0.0.2/hlagenie.egg-info/dependency_links.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)        1 2023-07-05 17:19:56.000000 hlagenie-0.0.2/hlagenie.egg-info/not-zip-safe
--rw-r--r--   0 nomad     (1000) nomad     (1000)       72 2023-07-05 18:03:47.000000 hlagenie-0.0.2/hlagenie.egg-info/requires.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)        9 2023-07-05 18:03:47.000000 hlagenie-0.0.2/hlagenie.egg-info/top_level.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)       45 2023-07-05 00:38:46.000000 hlagenie-0.0.2/requirements-tests.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)       72 2023-07-05 17:58:42.000000 hlagenie-0.0.2/requirements.txt
--rw-r--r--   0 nomad     (1000) nomad     (1000)      418 2023-07-05 18:03:47.168063 hlagenie-0.0.2/setup.cfg
--rw-r--r--   0 nomad     (1000) nomad     (1000)     1297 2023-07-05 17:49:32.000000 hlagenie-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.149740 hlagenie-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 19:42:29.000000 hlagenie-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-05 19:42:29.000000 hlagenie-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-05 19:42:39.149740 hlagenie-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-05 19:42:29.000000 hlagenie-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.145740 hlagenie-0.0.3/hlagenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/genie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-05 19:42:29.000000 hlagenie-0.0.3/hlagenie/smart_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:42:39.149740 hlagenie-0.0.3/hlagenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:42:38.000000 hlagenie-0.0.3/hlagenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 19:42:39.000000 hlagenie-0.0.3/hlagenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 19:42:29.000000 hlagenie-0.0.3/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 19:42:29.000000 hlagenie-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 19:42:39.149740 hlagenie-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-05 19:42:29.000000 hlagenie-0.0.3/setup.py
```

### Comparing `hlagenie-0.0.2/LICENSE` & `hlagenie-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/data_repository.py` & `hlagenie-0.0.3/hlagenie/data_repository.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/db.py` & `hlagenie-0.0.3/hlagenie/db.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/genie.py` & `hlagenie-0.0.3/hlagenie/genie.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/load.py` & `hlagenie-0.0.3/hlagenie/load.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/misc.py` & `hlagenie-0.0.3/hlagenie/misc.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/hlagenie/smart_sort.py` & `hlagenie-0.0.3/hlagenie/smart_sort.py`

 * *Files identical despite different names*

### Comparing `hlagenie-0.0.2/setup.py` & `hlagenie-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="hlagenie",
-    version="0.0.2",
+    version="0.0.3",
     description="Sequence handing for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Giovanni Biagini",
     author_email="dbiagini@tulane.edu",
     url="https://github.com/gbiagini/hlagenie",
     packages=[
```

