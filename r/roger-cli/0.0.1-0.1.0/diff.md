# Comparing `tmp/roger-cli-0.0.1.tar.gz` & `tmp/roger-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roger-cli-0.0.1.tar", last modified: Wed Jul  5 11:00:17 2023, max compression
+gzip compressed data, was "roger-cli-0.1.0.tar", last modified: Wed Jul  5 12:28:00 2023, max compression
```

## Comparing `roger-cli-0.0.1.tar` & `roger-cli-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 11:00:17.573079 roger-cli-0.0.1/
--rw-r--r--   0 nazar      (501) staff       (20)     1065 2023-07-05 10:00:48.000000 roger-cli-0.0.1/LICENSE
--rw-r--r--   0 nazar      (501) staff       (20)      151 2023-07-05 11:00:17.572576 roger-cli-0.0.1/PKG-INFO
--rw-r--r--   0 nazar      (501) staff       (20)       35 2023-07-05 10:00:48.000000 roger-cli-0.0.1/README.md
-drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 11:00:17.568405 roger-cli-0.0.1/roger_cli.egg-info/
--rw-r--r--   0 nazar      (501) staff       (20)      151 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/PKG-INFO
--rw-r--r--   0 nazar      (501) staff       (20)      322 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nazar      (501) staff       (20)        1 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nazar      (501) staff       (20)       47 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/entry_points.txt
--rw-r--r--   0 nazar      (501) staff       (20)       15 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/requires.txt
--rw-r--r--   0 nazar      (501) staff       (20)        4 2023-07-05 11:00:17.000000 roger-cli-0.0.1/roger_cli.egg-info/top_level.txt
--rw-r--r--   0 nazar      (501) staff       (20)       38 2023-07-05 11:00:17.573242 roger-cli-0.0.1/setup.cfg
--rw-r--r--   0 nazar      (501) staff       (20)      408 2023-07-05 10:59:01.000000 roger-cli-0.0.1/setup.py
-drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 11:00:17.568894 roger-cli-0.0.1/src/
--rw-r--r--   0 nazar      (501) staff       (20)        0 2023-07-05 10:08:31.000000 roger-cli-0.0.1/src/__init__.py
-drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 11:00:17.571508 roger-cli-0.0.1/src/roger/
--rw-r--r--   0 nazar      (501) staff       (20)        0 2023-07-05 10:09:07.000000 roger-cli-0.0.1/src/roger/__init__.py
--rw-r--r--   0 nazar      (501) staff       (20)      148 2023-07-05 10:09:48.000000 roger-cli-0.0.1/src/roger/colors.py
--rw-r--r--   0 nazar      (501) staff       (20)     5055 2023-07-05 10:50:24.000000 roger-cli-0.0.1/src/roger/roger.py
--rw-r--r--   0 nazar      (501) staff       (20)      782 2023-07-05 10:09:43.000000 roger-cli-0.0.1/src/roger/utils.py
+drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 12:28:00.544271 roger-cli-0.1.0/
+-rw-r--r--   0 nazar      (501) staff       (20)     1065 2023-07-05 10:00:48.000000 roger-cli-0.1.0/LICENSE
+-rw-r--r--   0 nazar      (501) staff       (20)      151 2023-07-05 12:28:00.543676 roger-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 nazar      (501) staff       (20)       35 2023-07-05 10:00:48.000000 roger-cli-0.1.0/README.md
+drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 12:28:00.537870 roger-cli-0.1.0/roger_cli.egg-info/
+-rw-r--r--   0 nazar      (501) staff       (20)      151 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nazar      (501) staff       (20)      347 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nazar      (501) staff       (20)        1 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nazar      (501) staff       (20)       47 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nazar      (501) staff       (20)       36 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/requires.txt
+-rw-r--r--   0 nazar      (501) staff       (20)        4 2023-07-05 12:28:00.000000 roger-cli-0.1.0/roger_cli.egg-info/top_level.txt
+-rw-r--r--   0 nazar      (501) staff       (20)       38 2023-07-05 12:28:00.544465 roger-cli-0.1.0/setup.cfg
+-rw-r--r--   0 nazar      (501) staff       (20)      408 2023-07-05 12:27:48.000000 roger-cli-0.1.0/setup.py
+drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 12:28:00.538391 roger-cli-0.1.0/src/
+-rw-r--r--   0 nazar      (501) staff       (20)        0 2023-07-05 10:08:31.000000 roger-cli-0.1.0/src/__init__.py
+drwxr-xr-x   0 nazar      (501) staff       (20)        0 2023-07-05 12:28:00.542381 roger-cli-0.1.0/src/roger/
+-rw-r--r--   0 nazar      (501) staff       (20)        0 2023-07-05 10:09:07.000000 roger-cli-0.1.0/src/roger/__init__.py
+-rw-r--r--   0 nazar      (501) staff       (20)      148 2023-07-05 10:09:48.000000 roger-cli-0.1.0/src/roger/colors.py
+-rw-r--r--   0 nazar      (501) staff       (20)     1666 2023-07-05 12:04:15.000000 roger-cli-0.1.0/src/roger/key_manager.py
+-rw-r--r--   0 nazar      (501) staff       (20)     5078 2023-07-05 12:22:51.000000 roger-cli-0.1.0/src/roger/roger.py
+-rw-r--r--   0 nazar      (501) staff       (20)      782 2023-07-05 10:09:43.000000 roger-cli-0.1.0/src/roger/utils.py
```

### Comparing `roger-cli-0.0.1/LICENSE` & `roger-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roger-cli-0.0.1/src/roger/roger.py` & `roger-cli-0.1.0/src/roger/roger.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import json
 import os
 from pathlib import Path
 import sys
 
 from .utils import SETUP, FEWSHOT, METRICS
 from .colors import Colors
+from .key_manager import get_api_key
 
 USERNAME = "test"
 
 
 class Roger:
     def __init__(self, buffer_size, instance):
         self.buffer_size = buffer_size
         self.instance = instance
         self.script_dir = Path(__file__).parent.absolute()
 
         self.validate_instance_directory()
-        openai.api_key = os.getenv("OPENAI_API_KEY")
+        openai.api_key = get_api_key()
         self.buffer = self.load_buffer()
 
         self.setup = SETUP
         self.fewshot_prompts = FEWSHOT
         self.metrics = self.load_metrics()
 
     def validate_instance_directory(self):
```

### Comparing `roger-cli-0.0.1/src/roger/utils.py` & `roger-cli-0.1.0/src/roger/utils.py`

 * *Files identical despite different names*

