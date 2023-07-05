# Comparing `tmp/altob-0.1.1.tar.gz` & `tmp/altob-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altob-0.1.1.tar", last modified: Wed Jul  5 19:24:58 2023, max compression
+gzip compressed data, was "altob-1.0.0.tar", last modified: Wed Jul  5 19:27:00 2023, max compression
```

## Comparing `altob-0.1.1.tar` & `altob-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:24:58.633745 altob-0.1.1/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4095 2023-07-05 19:24:58.629745 altob-0.1.1/PKG-INFO
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3828 2023-07-05 19:23:49.000000 altob-0.1.1/README.md
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:24:58.629745 altob-0.1.1/altob/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1156 2023-03-29 20:26:21.000000 altob-0.1.1/altob/__init__.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     5512 2023-03-29 20:26:21.000000 altob-0.1.1/altob/amplicon_coverage.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8616 2023-06-20 15:43:27.000000 altob-0.1.1/altob/analyze.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1303 2023-06-30 20:39:20.000000 altob-0.1.1/altob/artic_amplicons.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      279 2023-02-13 20:37:46.000000 altob-0.1.1/altob/cmds.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       73 2023-02-13 20:37:46.000000 altob-0.1.1/altob/command_line.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      546 2023-02-13 20:37:46.000000 altob-0.1.1/altob/consensus.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      922 2023-06-30 20:39:20.000000 altob-0.1.1/altob/constellations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     2719 2023-02-13 20:37:46.000000 altob-0.1.1/altob/convert_mutations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)    16961 2023-06-20 15:42:57.000000 altob-0.1.1/altob/lineages.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4522 2023-06-15 19:27:59.000000 altob-0.1.1/altob/make_clades.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8138 2023-06-30 20:39:20.000000 altob-0.1.1/altob/mutations.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     7114 2023-06-09 20:17:59.000000 altob-0.1.1/altob/precompute.py
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6413 2023-06-30 20:39:20.000000 altob-0.1.1/altob/tobrfv.py
-drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:24:58.629745 altob-0.1.1/altob.egg-info/
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4095 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/PKG-INFO
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      481 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/SOURCES.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        1 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/dependency_links.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       50 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/entry_points.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       70 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/requires.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        6 2023-07-05 19:24:58.000000 altob-0.1.1/altob.egg-info/top_level.txt
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       38 2023-07-05 19:24:58.633745 altob-0.1.1/setup.cfg
--rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      753 2023-02-13 20:37:46.000000 altob-0.1.1/setup.py
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:27:00.815581 altob-1.0.0/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4160 2023-07-05 19:27:00.815581 altob-1.0.0/PKG-INFO
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     3828 2023-07-05 19:23:49.000000 altob-1.0.0/README.md
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:27:00.811581 altob-1.0.0/altob/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1156 2023-03-29 20:26:21.000000 altob-1.0.0/altob/__init__.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     5512 2023-03-29 20:26:21.000000 altob-1.0.0/altob/amplicon_coverage.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8616 2023-06-20 15:43:27.000000 altob-1.0.0/altob/analyze.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     1303 2023-06-30 20:39:20.000000 altob-1.0.0/altob/artic_amplicons.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      279 2023-02-13 20:37:46.000000 altob-1.0.0/altob/cmds.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       73 2023-02-13 20:37:46.000000 altob-1.0.0/altob/command_line.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      546 2023-02-13 20:37:46.000000 altob-1.0.0/altob/consensus.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      922 2023-06-30 20:39:20.000000 altob-1.0.0/altob/constellations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     2719 2023-02-13 20:37:46.000000 altob-1.0.0/altob/convert_mutations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)    16961 2023-06-20 15:42:57.000000 altob-1.0.0/altob/lineages.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4522 2023-06-15 19:27:59.000000 altob-1.0.0/altob/make_clades.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     8138 2023-06-30 20:39:20.000000 altob-1.0.0/altob/mutations.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     7114 2023-06-09 20:17:59.000000 altob-1.0.0/altob/precompute.py
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     6413 2023-06-30 20:39:20.000000 altob-1.0.0/altob/tobrfv.py
+drwxrwxr-x   0 jknapp    (1008) jknapp    (1010)        0 2023-07-05 19:27:00.815581 altob-1.0.0/altob.egg-info/
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)     4160 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/PKG-INFO
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      481 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/SOURCES.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        1 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/dependency_links.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       50 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/entry_points.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       70 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/requires.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)        6 2023-07-05 19:27:00.000000 altob-1.0.0/altob.egg-info/top_level.txt
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)       38 2023-07-05 19:27:00.815581 altob-1.0.0/setup.cfg
+-rw-rw-r--   0 jknapp    (1008) jknapp    (1010)      830 2023-07-05 19:26:47.000000 altob-1.0.0/setup.py
```

### Comparing `altob-0.1.1/PKG-INFO` & `altob-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: altob
-Version: 0.1.1
+Version: 1.0.0
 Summary: Identify frequencies of concerning mutations from aligned reads
 Home-page: https://github.com/Ellmen/altob
 Author: Isaac Ellmen
 Author-email: isaac.ellmen@uwaterloo.ca
+Maintainer: Jenn Knapp
+Maintainer-email: jenn.knapp@uwaterloo.ca
 Description-Content-Type: text/markdown
 
 # Altob
 
 Abundance learning for ToBRFV variants. The primary purpose of the tool is:
 
 * Estimating abundace of clades of ToBRFV from sequencing data
```

### Comparing `altob-0.1.1/README.md` & `altob-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/__init__.py` & `altob-1.0.0/altob/__init__.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/amplicon_coverage.py` & `altob-1.0.0/altob/amplicon_coverage.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/analyze.py` & `altob-1.0.0/altob/analyze.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/artic_amplicons.py` & `altob-1.0.0/altob/artic_amplicons.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/consensus.py` & `altob-1.0.0/altob/consensus.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/constellations.py` & `altob-1.0.0/altob/constellations.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/convert_mutations.py` & `altob-1.0.0/altob/convert_mutations.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/lineages.py` & `altob-1.0.0/altob/lineages.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/make_clades.py` & `altob-1.0.0/altob/make_clades.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/mutations.py` & `altob-1.0.0/altob/mutations.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/precompute.py` & `altob-1.0.0/altob/precompute.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob/tobrfv.py` & `altob-1.0.0/altob/tobrfv.py`

 * *Files identical despite different names*

### Comparing `altob-0.1.1/altob.egg-info/PKG-INFO` & `altob-1.0.0/altob.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: altob
-Version: 0.1.1
+Version: 1.0.0
 Summary: Identify frequencies of concerning mutations from aligned reads
 Home-page: https://github.com/Ellmen/altob
 Author: Isaac Ellmen
 Author-email: isaac.ellmen@uwaterloo.ca
+Maintainer: Jenn Knapp
+Maintainer-email: jenn.knapp@uwaterloo.ca
 Description-Content-Type: text/markdown
 
 # Altob
 
 Abundance learning for ToBRFV variants. The primary purpose of the tool is:
 
 * Estimating abundace of clades of ToBRFV from sequencing data
```

### Comparing `altob-0.1.1/setup.py` & `altob-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='altob',
-    version='0.1.1',
+    version='1.0.0',
     description='Identify frequencies of concerning mutations from aligned reads',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Isaac Ellmen',
     author_email='isaac.ellmen@uwaterloo.ca',
+    maintainer='Jenn Knapp',
+    maintainer_email='jenn.knapp@uwaterloo.ca',
     packages=['altob'],
     url='https://github.com/Ellmen/altob',
     install_requires=[
         'fire',
         'numpy',
         'pandas',
         'scikit-learn>=0.24',
```

