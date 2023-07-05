# Comparing `tmp/geodock-1.0.0.tar.gz` & `tmp/geodock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/scratch4/jgray21/lchu11/GeoDock/dist/.tmp-13z5fns6/geodock-1.0.0.tar", last modified: Wed Jul  5 20:34:59 2023, max compression
+gzip compressed data, was "/scratch4/jgray21/lchu11/GeoDock/dist/.tmp-22one397/geodock-1.0.1.tar", last modified: Wed Jul  5 20:50:59 2023, max compression
```

## Comparing `geodock-1.0.0.tar` & `geodock-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1065 2023-06-30 18:18:41.000000 geodock-1.0.0/LICENSE.md
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)       19 2023-07-05 19:31:03.000000 geodock-1.0.0/MANIFEST.in
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:34:59.000000 geodock-1.0.0/PKG-INFO
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      905 2023-07-04 02:59:52.000000 geodock-1.0.0/README.md
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2494 2023-07-05 17:00:05.000000 geodock-1.0.0/geodock/GeoDockRunner.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:34.000000 geodock-1.0.0/geodock/__init__.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock/model/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5221 2023-06-01 18:47:22.000000 geodock-1.0.0/geodock/model/GeoDock.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:17.000000 geodock-1.0.0/geodock/model/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      486 2023-05-17 20:56:02.000000 geodock-1.0.0/geodock/model/interface.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock/model/modules/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 17:15:41.000000 geodock-1.0.0/geodock/model/modules/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7909 2023-06-09 18:56:03.000000 geodock-1.0.0/geodock/model/modules/graph_module.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7183 2023-07-04 03:51:21.000000 geodock-1.0.0/geodock/model/modules/iterative_transformer.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9365 2023-07-04 03:50:32.000000 geodock-1.0.0/geodock/model/modules/structure_module.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock/trainer/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-18 19:22:41.000000 geodock-1.0.0/geodock/trainer/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1013 2023-05-18 19:28:10.000000 geodock-1.0.0/geodock/trainer/run.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3252 2023-05-18 19:29:30.000000 geodock-1.0.0/geodock/trainer/train.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5198 2023-05-18 19:22:42.000000 geodock-1.0.0/geodock/trainer/utils.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/PKG-INFO
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      596 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/SOURCES.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        1 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/dependency_links.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      195 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/requires.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        8 2023-07-05 20:34:59.000000 geodock-1.0.0/geodock.egg-info/top_level.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)       81 2023-07-05 18:52:34.000000 geodock-1.0.0/pyproject.toml
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      550 2023-07-05 20:34:59.000000 geodock-1.0.0/setup.cfg
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:59.000000 geodock-1.0.1/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1065 2023-06-30 18:18:41.000000 geodock-1.0.1/LICENSE.md
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       19 2023-07-05 19:31:03.000000 geodock-1.0.1/MANIFEST.in
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:50:59.000000 geodock-1.0.1/PKG-INFO
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      905 2023-07-04 02:59:52.000000 geodock-1.0.1/README.md
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2494 2023-07-05 17:00:05.000000 geodock-1.0.1/geodock/GeoDockRunner.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:34.000000 geodock-1.0.1/geodock/__init__.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock/model/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5221 2023-06-01 18:47:22.000000 geodock-1.0.1/geodock/model/GeoDock.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:17.000000 geodock-1.0.1/geodock/model/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      486 2023-05-17 20:56:02.000000 geodock-1.0.1/geodock/model/interface.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:59.000000 geodock-1.0.1/geodock/model/modules/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 17:15:41.000000 geodock-1.0.1/geodock/model/modules/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7909 2023-06-09 18:56:03.000000 geodock-1.0.1/geodock/model/modules/graph_module.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7183 2023-07-04 03:51:21.000000 geodock-1.0.1/geodock/model/modules/iterative_transformer.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9365 2023-07-04 03:50:32.000000 geodock-1.0.1/geodock/model/modules/structure_module.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:59.000000 geodock-1.0.1/geodock/trainer/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-18 19:22:41.000000 geodock-1.0.1/geodock/trainer/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1013 2023-05-18 19:28:10.000000 geodock-1.0.1/geodock/trainer/run.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3252 2023-05-18 19:29:30.000000 geodock-1.0.1/geodock/trainer/train.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5198 2023-05-18 19:22:42.000000 geodock-1.0.1/geodock/trainer/utils.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/PKG-INFO
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      596 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/SOURCES.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        1 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/dependency_links.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       84 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/requires.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        8 2023-07-05 20:50:58.000000 geodock-1.0.1/geodock.egg-info/top_level.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       81 2023-07-05 18:52:34.000000 geodock-1.0.1/pyproject.toml
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      434 2023-07-05 20:50:59.000000 geodock-1.0.1/setup.cfg
```

### Comparing `geodock-1.0.0/LICENSE.md` & `geodock-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/PKG-INFO` & `geodock-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodock
-Version: 1.0.0
+Version: 1.0.1
 Author: Lee-Shin Chu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GeoDock
```

### Comparing `geodock-1.0.0/README.md` & `geodock-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/GeoDockRunner.py` & `geodock-1.0.1/geodock/GeoDockRunner.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/model/GeoDock.py` & `geodock-1.0.1/geodock/model/GeoDock.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/model/modules/graph_module.py` & `geodock-1.0.1/geodock/model/modules/graph_module.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/model/modules/iterative_transformer.py` & `geodock-1.0.1/geodock/model/modules/iterative_transformer.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/model/modules/structure_module.py` & `geodock-1.0.1/geodock/model/modules/structure_module.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/trainer/run.py` & `geodock-1.0.1/geodock/trainer/run.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/trainer/train.py` & `geodock-1.0.1/geodock/trainer/train.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock/trainer/utils.py` & `geodock-1.0.1/geodock/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.0/geodock.egg-info/PKG-INFO` & `geodock-1.0.1/geodock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodock
-Version: 1.0.0
+Version: 1.0.1
 Author: Lee-Shin Chu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GeoDock
```

### Comparing `geodock-1.0.0/geodock.egg-info/SOURCES.txt` & `geodock-1.0.1/geodock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

