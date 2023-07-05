# Comparing `tmp/autodice-1.0.2.dev2.tar.gz` & `tmp/autodice-1.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodice-1.0.2.dev2.tar", last modified: Thu Jun 29 17:35:00 2023, max compression
+gzip compressed data, was "autodice-1.0.3.dev2.tar", last modified: Wed Jul  5 14:36:36 2023, max compression
```

## Comparing `autodice-1.0.2.dev2.tar` & `autodice-1.0.3.dev2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/
--rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/LICENSE.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)     2702 2023-06-29 17:34:21.000000 autodice-1.0.2.dev2/README.md
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/autodice.egg-info/
--rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/PKG-INFO
--rw-rw-r--   0 sky       (1000) sky       (1000)      361 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/SOURCES.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/dependency_links.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/entry_points.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/requires.txt
--rw-rw-r--   0 sky       (1000) sky       (1000)       10 2023-06-29 17:35:00.000000 autodice-1.0.2.dev2/autodice.egg-info/top_level.txt
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/partition/
--rw-r--r--   0 sky       (1000) sky       (1000)      174 2023-06-29 15:12:52.000000 autodice-1.0.2.dev2/partition/__init__.py
--rwxrwxr-x   0 sky       (1000) sky       (1000)     5290 2022-08-01 20:47:57.000000 autodice-1.0.2.dev2/partition/code_generator.py
--rw-rw-r--   0 sky       (1000) sky       (1000)    44651 2023-06-29 14:19:33.000000 autodice-1.0.2.dev2/partition/dice.py
--rwxrwxr-x   0 sky       (1000) sky       (1000)    44946 2023-06-29 16:08:22.000000 autodice-1.0.2.dev2/partition/interface.py
--rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/pyproject.toml
--rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/setup.cfg
--rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-06-29 17:34:37.000000 autodice-1.0.2.dev2/setup.py
-drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-06-29 17:35:00.030601 autodice-1.0.2.dev2/tests/
--rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.2.dev2/tests/test_simple.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     1081 2022-12-01 16:53:46.000000 autodice-1.0.3.dev2/LICENSE.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)     2702 2023-06-29 17:34:21.000000 autodice-1.0.3.dev2/README.md
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/autodice.egg-info/
+-rw-rw-r--   0 sky       (1000) sky       (1000)     3838 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/PKG-INFO
+-rw-rw-r--   0 sky       (1000) sky       (1000)      361 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/SOURCES.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)        1 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/dependency_links.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       39 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/entry_points.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       50 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/requires.txt
+-rw-rw-r--   0 sky       (1000) sky       (1000)       10 2023-07-05 14:36:36.000000 autodice-1.0.3.dev2/autodice.egg-info/top_level.txt
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/partition/
+-rw-r--r--   0 sky       (1000) sky       (1000)      174 2023-06-29 15:12:52.000000 autodice-1.0.3.dev2/partition/__init__.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)     5290 2022-08-01 20:47:57.000000 autodice-1.0.3.dev2/partition/code_generator.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)    44651 2023-06-29 14:19:33.000000 autodice-1.0.3.dev2/partition/dice.py
+-rwxrwxr-x   0 sky       (1000) sky       (1000)    45526 2023-07-05 14:35:39.000000 autodice-1.0.3.dev2/partition/interface.py
+-rw-rw-r--   0 sky       (1000) sky       (1000)      230 2022-12-01 16:53:46.000000 autodice-1.0.3.dev2/pyproject.toml
+-rw-rw-r--   0 sky       (1000) sky       (1000)       78 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/setup.cfg
+-rw-rw-r--   0 sky       (1000) sky       (1000)     7990 2023-07-05 14:36:06.000000 autodice-1.0.3.dev2/setup.py
+drwxrwxr-x   0 sky       (1000) sky       (1000)        0 2023-07-05 14:36:36.497245 autodice-1.0.3.dev2/tests/
+-rw-rw-r--   0 sky       (1000) sky       (1000)      417 2022-12-01 16:53:46.000000 autodice-1.0.3.dev2/tests/test_simple.py
```

### Comparing `autodice-1.0.2.dev2/LICENSE.txt` & `autodice-1.0.3.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autodice-1.0.2.dev2/PKG-INFO` & `autodice-1.0.3.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodice
-Version: 1.0.2.dev2
+Version: 1.0.3.dev2
 Summary: Automated Distributed CNN inference at the Edge
 Home-page: https://github.com/parrotsky/AutoDiCE
 Author: Parrotsky
 Author-email: x.guo3@uva.nl
 Project-URL: Bug Reports, https://github.com/parrotsky/AutoDiCE/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/parrotsky/AutoDiCE
```

### Comparing `autodice-1.0.2.dev2/README.md` & `autodice-1.0.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `autodice-1.0.2.dev2/autodice.egg-info/PKG-INFO` & `autodice-1.0.3.dev2/autodice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodice
-Version: 1.0.2.dev2
+Version: 1.0.3.dev2
 Summary: Automated Distributed CNN inference at the Edge
 Home-page: https://github.com/parrotsky/AutoDiCE
 Author: Parrotsky
 Author-email: x.guo3@uva.nl
 Project-URL: Bug Reports, https://github.com/parrotsky/AutoDiCE/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/parrotsky/AutoDiCE
```

### Comparing `autodice-1.0.2.dev2/partition/code_generator.py` & `autodice-1.0.3.dev2/partition/code_generator.py`

 * *Files identical despite different names*

### Comparing `autodice-1.0.2.dev2/partition/dice.py` & `autodice-1.0.3.dev2/partition/dice.py`

 * *Files identical despite different names*

### Comparing `autodice-1.0.2.dev2/partition/interface.py` & `autodice-1.0.3.dev2/partition/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,37 @@
 from .code_generator import CppFile
 import itertools as it
 import onnx
 from onnx import helper, checker
 from onnx import TensorProto
 import os
 
+import re
+
+def parse_platform_file(file_path):
+    with open(file_path, 'r') as file:
+        lines = file.readlines()
+
+    pattern = re.compile(r'(.*),\s*(.*),\s*slots=(.*),\s*gpu=(.*)\s*\((.*)\)')
+
+    result = []
+
+    for line in lines:
+        match = pattern.match(line.strip())
+        if match:
+            result.append({
+                'device': match.group(1),
+                'arch': match.group(2),
+                'slots': match.group(3),
+                'gpu_type': match.group(4),
+                'gpu_platform': match.group(5),
+            })
+
+    return result
+
 class ComputingNode:
     def __init__(self, **node_details):
 # name; inbuffs; receiver; outbuffs; sender ; hardware ;number;cores; dist_layers
         self.__dict__.update(node_details)
 
 class Interface:
     def __init__(self, **input_specs):
```

### Comparing `autodice-1.0.2.dev2/setup.py` & `autodice-1.0.3.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="autodice",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.0.2.dev2",  # Required
+    version="1.0.3.dev2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Automated Distributed CNN inference at the Edge",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

