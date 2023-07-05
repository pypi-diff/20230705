# Comparing `tmp/MEGNetSparse-0.0.1.tar.gz` & `tmp/MEGNetSparse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGNetSparse-0.0.1.tar", last modified: Tue Jul  4 18:29:07 2023, max compression
+gzip compressed data, was "MEGNetSparse-0.0.2.tar", last modified: Wed Jul  5 16:15:01 2023, max compression
```

## Comparing `MEGNetSparse-0.0.1.tar` & `MEGNetSparse-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-04 18:29:08.761250 MEGNetSparse-0.0.1/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       22 2023-06-20 14:41:44.000000 MEGNetSparse-0.0.1/.gitignore
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-04 18:29:08.113698 MEGNetSparse-0.0.1/MEGNetSparse/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.1/MEGNetSparse/__init__.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-06-27 20:57:11.000000 MEGNetSparse-0.0.1/MEGNetSparse/dense2sparse.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.1/MEGNetSparse/eos.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.1/MEGNetSparse/layers.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.1/MEGNetSparse/model.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.1/MEGNetSparse/struct2graph.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     7461 2023-06-28 00:30:39.000000 MEGNetSparse-0.0.1/MEGNetSparse/trainer.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.1/MEGNetSparse/utils.py
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-04 18:29:08.266232 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      273 2023-07-04 18:29:06.000000 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      604 2023-07-04 18:29:07.000000 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/SOURCES.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-04 18:29:06.000000 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/dependency_links.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       11 2023-07-04 18:29:07.000000 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/requires.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-04 18:29:07.000000 MEGNetSparse-0.0.1/MEGNetSparse.egg-info/top_level.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      273 2023-07-04 18:29:08.756181 MEGNetSparse-0.0.1/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       21 2023-06-03 13:54:47.000000 MEGNetSparse-0.0.1/README.md
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-04 18:29:08.508177 MEGNetSparse-0.0.1/examples/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.1/examples/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.1/examples/MoS2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.1/examples/WSe2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.1/examples/descriptors.csv
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.1/examples/example.ipynb
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.1/examples/initial_structures.csv
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-04 18:29:08.699755 MEGNetSparse-0.0.1/examples/pilot/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.1/examples/pilot/data.pickle.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.1/examples/pilot/targets.csv.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      406 2023-07-03 18:54:47.000000 MEGNetSparse-0.0.1/pyproject.toml
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-04 18:29:08.763300 MEGNetSparse-0.0.1/setup.cfg
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 16:15:02.253929 MEGNetSparse-0.0.2/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       31 2023-07-05 12:55:20.000000 MEGNetSparse-0.0.2/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.2/LICENSE
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 16:15:01.832054 MEGNetSparse-0.0.2/MEGNetSparse/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.2/MEGNetSparse/__init__.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-06-27 20:57:11.000000 MEGNetSparse-0.0.2/MEGNetSparse/dense2sparse.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.2/MEGNetSparse/eos.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.2/MEGNetSparse/layers.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.2/MEGNetSparse/model.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.2/MEGNetSparse/struct2graph.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     7461 2023-06-28 00:30:39.000000 MEGNetSparse-0.0.2/MEGNetSparse/trainer.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.2/MEGNetSparse/utils.py
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 16:15:01.957054 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 16:15:01.000000 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      612 2023-07-05 16:15:01.000000 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-05 16:15:01.000000 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-05 16:15:01.000000 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/requires.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-05 16:15:01.000000 MEGNetSparse-0.0.2/MEGNetSparse.egg-info/top_level.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 16:15:02.253929 MEGNetSparse-0.0.2/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.2/README.md
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 16:15:02.144553 MEGNetSparse-0.0.2/examples/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.2/examples/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.2/examples/MoS2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.2/examples/WSe2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.2/examples/descriptors.csv
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.2/examples/example.ipynb
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.2/examples/initial_structures.csv
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 16:15:02.222679 MEGNetSparse-0.0.2/examples/pilot/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.2/examples/pilot/data.pickle.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.2/examples/pilot/targets.csv.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-05 14:01:52.000000 MEGNetSparse-0.0.2/pyproject.toml
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 16:15:02.253929 MEGNetSparse-0.0.2/setup.cfg
```

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/dense2sparse.py` & `MEGNetSparse-0.0.2/MEGNetSparse/dense2sparse.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/eos.py` & `MEGNetSparse-0.0.2/MEGNetSparse/eos.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/layers.py` & `MEGNetSparse-0.0.2/MEGNetSparse/layers.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/model.py` & `MEGNetSparse-0.0.2/MEGNetSparse/model.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/struct2graph.py` & `MEGNetSparse-0.0.2/MEGNetSparse/struct2graph.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/trainer.py` & `MEGNetSparse-0.0.2/MEGNetSparse/trainer.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse/utils.py` & `MEGNetSparse-0.0.2/MEGNetSparse/utils.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/MEGNetSparse.egg-info/SOURCES.txt` & `MEGNetSparse-0.0.2/MEGNetSparse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 README.md
 pyproject.toml
 MEGNetSparse/__init__.py
 MEGNetSparse/dense2sparse.py
 MEGNetSparse/eos.py
 MEGNetSparse/layers.py
 MEGNetSparse/model.py
```

### Comparing `MEGNetSparse-0.0.1/examples/MoS2.cif` & `MEGNetSparse-0.0.2/examples/MoS2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/examples/WSe2.cif` & `MEGNetSparse-0.0.2/examples/WSe2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/examples/descriptors.csv` & `MEGNetSparse-0.0.2/examples/descriptors.csv`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/examples/example.ipynb` & `MEGNetSparse-0.0.2/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/examples/pilot/data.pickle.gz` & `MEGNetSparse-0.0.2/examples/pilot/data.pickle.gz`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.1/examples/pilot/targets.csv.gz` & `MEGNetSparse-0.0.2/examples/pilot/targets.csv.gz`

 * *Files identical despite different names*

