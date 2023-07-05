# Comparing `tmp/whisper_mic-1.1.0.tar.gz` & `tmp/whisper_mic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_mic-1.1.0.tar", last modified: Wed Jul  5 05:55:37 2023, max compression
+gzip compressed data, was "whisper_mic-1.1.1.tar", last modified: Wed Jul  5 06:08:27 2023, max compression
```

## Comparing `whisper_mic-1.1.0.tar` & `whisper_mic-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/
--rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.1.0/LICENSE
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)     3231 2023-06-29 22:23:36.000000 whisper_mic-1.1.0/README.md
--rw-rw-r--   0 blake     (1000) blake     (1000)      821 2023-07-05 05:54:48.000000 whisper_mic-1.1.0/pyproject.toml
--rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/setup.cfg
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/whisper_mic/
--rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.1.0/whisper_mic/__init__.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     1600 2023-06-29 19:44:37.000000 whisper_mic-1.1.0/whisper_mic/cli.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)      480 2023-07-05 05:53:32.000000 whisper_mic-1.1.0/whisper_mic/utils.py
--rwxrwxr-x   0 blake     (1000) blake     (1000)     4077 2023-07-05 05:53:32.000000 whisper_mic-1.1.0/whisper_mic/whisper_mic.py
-drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 05:55:37.619970 whisper_mic-1.1.0/whisper_mic.egg-info/
--rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/PKG-INFO
--rw-rw-r--   0 blake     (1000) blake     (1000)      335 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/SOURCES.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/dependency_links.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/entry_points.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)      187 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/requires.txt
--rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-07-05 05:55:37.000000 whisper_mic-1.1.0/whisper_mic.egg-info/top_level.txt
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     1070 2023-06-29 19:44:37.000000 whisper_mic-1.1.1/LICENSE
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3231 2023-06-29 22:23:36.000000 whisper_mic-1.1.1/README.md
+-rw-rw-r--   0 blake     (1000) blake     (1000)      821 2023-07-05 06:08:00.000000 whisper_mic-1.1.1/pyproject.toml
+-rw-rw-r--   0 blake     (1000) blake     (1000)       38 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/setup.cfg
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/whisper_mic/
+-rwxrwxrwx   0 blake     (1000) blake     (1000)        0 2023-04-21 06:07:53.000000 whisper_mic-1.1.1/whisper_mic/__init__.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     1606 2023-07-05 06:07:43.000000 whisper_mic-1.1.1/whisper_mic/cli.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)      480 2023-07-05 05:53:32.000000 whisper_mic-1.1.1/whisper_mic/utils.py
+-rwxrwxr-x   0 blake     (1000) blake     (1000)     4383 2023-07-05 06:07:43.000000 whisper_mic-1.1.1/whisper_mic/whisper_mic.py
+drwxrwxr-x   0 blake     (1000) blake     (1000)        0 2023-07-05 06:08:27.161614 whisper_mic-1.1.1/whisper_mic.egg-info/
+-rw-rw-r--   0 blake     (1000) blake     (1000)     3532 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/PKG-INFO
+-rw-rw-r--   0 blake     (1000) blake     (1000)      335 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/SOURCES.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)        1 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/dependency_links.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       53 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/entry_points.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)      187 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/requires.txt
+-rw-rw-r--   0 blake     (1000) blake     (1000)       12 2023-07-05 06:08:27.000000 whisper_mic-1.1.1/whisper_mic.egg-info/top_level.txt
```

### Comparing `whisper_mic-1.1.0/LICENSE` & `whisper_mic-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.1.0/PKG-INFO` & `whisper_mic-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_mic
-Version: 1.1.0
+Version: 1.1.1
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `whisper_mic-1.1.0/README.md` & `whisper_mic-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whisper_mic-1.1.0/pyproject.toml` & `whisper_mic-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whisper_mic"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Blake Mallory", email="blakecmallory@gmail.com" },
 ]
 description = "Whisper for your microphone"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `whisper_mic-1.1.0/whisper_mic/cli.py` & `whisper_mic-1.1.1/whisper_mic/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torch
 import numpy as np
 
 from whisper_mic.whisper_mic import WhisperMic
 
 @click.command()
 @click.option("--model", default="base", help="Model to use", type=click.Choice(["tiny","base", "small","medium","large"]))
-@click.option("--device", default=("cuda" if torch.cuda.is_available() else "cpu"), help="Device to use", type=click.Choice(["cpu","cuda"]))
+@click.option("--device", default=("cuda" if torch.cuda.is_available() else "cpu"), help="Device to use", type=click.Choice(["cpu","cuda","mps"]))
 @click.option("--english", default=False, help="Whether to use English model",is_flag=True, type=bool)
 @click.option("--verbose", default=False, help="Whether to print verbose output", is_flag=True,type=bool)
 @click.option("--energy", default=300, help="Energy level for mic to detect", type=int)
 @click.option("--dynamic_energy", default=False,is_flag=True, help="Flag to enable dynamic energy", type=bool)
 @click.option("--pause", default=0.8, help="Pause time before entry ends", type=float)
 @click.option("--save_file",default=False, help="Flag to save file", is_flag=True,type=bool)
 @click.option("--loop", default=False, help="Flag to loop", is_flag=True,type=bool)
```

### Comparing `whisper_mic-1.1.0/whisper_mic/whisper_mic.py` & `whisper_mic-1.1.1/whisper_mic/whisper_mic.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,37 @@
 import threading
 import io
 import numpy as np
 from pydub import AudioSegment
 import os
 import tempfile
 import time
+import platform
 
 from whisper_mic.utils import get_logger
 
 
 class WhisperMic:
     def __init__(self,model="base",device=("cuda" if torch.cuda.is_available() else "cpu"),english=False,verbose=False,energy=300,pause=0.8,dynamic_energy=False,save_file=False):
         self.logger = get_logger("whisper_mic", "info")
         self.energy = energy
         self.pause = pause
         self.dynamic_energy = dynamic_energy
         self.save_file = save_file
         self.verbose = verbose
         self.english = english
 
+        self.platform = platform.system()
+
+        if self.platform == "darwin":
+            if device == "mps":
+                self.logger.warning("Using MPS for Mac, this does not work but may in the future")
+                device = "mps"
+                device = torch.device(device)
+
         if model != "large" and self.english:
             model = model + ".en"
 
         self.audio_model = whisper.load_model(model).to(device)
         self.temp_dir = tempfile.mkdtemp() if save_file else None
 
         self.audio_queue = queue.Queue()
```

### Comparing `whisper_mic-1.1.0/whisper_mic.egg-info/PKG-INFO` & `whisper_mic-1.1.1/whisper_mic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-mic
-Version: 1.1.0
+Version: 1.1.1
 Summary: Whisper for your microphone
 Author-email: Blake Mallory <blakecmallory@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

