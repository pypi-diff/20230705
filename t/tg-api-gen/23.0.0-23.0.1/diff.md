# Comparing `tmp/tg_api_gen-23.0.0.tar.gz` & `tmp/tg_api_gen-23.0.1.tar.gz`

## Comparing `tg_api_gen-23.0.0.tar` & `tg_api_gen-23.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/build.py
--rw-r--r--   0        0        0    85252 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/tg_api_gen/android_devices.txt
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/tg_api_gen/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/.gitignore
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/pyproject.toml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/readme.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tg_api_gen-23.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1321 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/build.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/tg_api_gen/__init__.py
+-rw-r--r--   0        0        0    85252 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/tg_api_gen/android_devices.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/.gitignore
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/pyproject.toml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/readme.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tg_api_gen-23.0.1/PKG-INFO
```

### Comparing `tg_api_gen-23.0.0/build.py` & `tg_api_gen-23.0.1/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/bin/python
 
-from pathlib import Path
 import shutil
 import toml
+import sys
 import os
-from tg_api_gen.main import (
+from pathlib import Path
+from tg_api_gen import (
     proj_version,
     proj_name,
 )
 
 
 app_path = Path(
     __file__
@@ -60,7 +61,9 @@
 
 
 shutil.rmtree(
     dist_path,
     ignore_errors = True,
 )
 
+os.system(f'{sys.executable} -m prettygit')
+
```

### Comparing `tg_api_gen-23.0.0/tg_api_gen/android_devices.txt` & `tg_api_gen-23.0.1/tg_api_gen/android_devices.txt`

 * *Files identical despite different names*

### Comparing `tg_api_gen-23.0.0/tg_api_gen/main.py` & `tg_api_gen-23.0.1/tg_api_gen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from random import (
     choice,
     randint,
 )
 
 
 proj_name = 'tg_api_gen'
-proj_version = '23.0.0'
+proj_version = '23.0.1'
 
 
 def get_device_and_ios_major() -> tuple:
     devices_and_ioses = [
         [
             ['6', '6 Plus', '6S', '6S Plus'],
             [12, 15],
```

### Comparing `tg_api_gen-23.0.0/pyproject.toml` & `tg_api_gen-23.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = []
 name = "tg_api_gen"
-version = "23.0.0"
+version = "23.0.1"
 description = "lightweight skript that generates realistic device_model, app_verion, system_version for telegram"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `tg_api_gen-23.0.0/PKG-INFO` & `tg_api_gen-23.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg_api_gen
-Version: 23.0.0
+Version: 23.0.1
 Summary: lightweight skript that generates realistic device_model, app_verion, system_version for telegram
 Project-URL: Homepage, https://github.com/gmankab/tg_api_gen
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

