# Comparing `tmp/py_basic_commands-0.2.24.tar.gz` & `tmp/py_basic_commands-0.2.25b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.24.tar", last modified: Wed May 31 00:38:54 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.25b1.tar", last modified: Wed Jul  5 00:32:44 2023, max compression
```

## Comparing `py_basic_commands-0.2.24.tar` & `py_basic_commands-0.2.25b1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.684094 py_basic_commands-0.2.24/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:38:54.688094 py_basic_commands-0.2.24/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 00:38:54.000000 py_basic_commands-0.2.24/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 00:38:35.000000 py_basic_commands-0.2.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 00:38:54.692094 py_basic_commands-0.2.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-05 00:32:44.394520 py_basic_commands-0.2.25b1/setup.cfg
```

### Comparing `py_basic_commands-0.2.24/LICENSE.md` & `py_basic_commands-0.2.25b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.24/PKG-INFO` & `py_basic_commands-0.2.25b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.24
+Version: 0.2.25b1
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.24/README.md` & `py_basic_commands-0.2.25b1/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.24/py_basic_commands/__init__.py` & `py_basic_commands-0.2.25b1/py_basic_commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # From file_dir_scripts
 from py_basic_commands.file_dir_scripts import create_dirs, create_file, get_src_path, join_path, read_file, remove_file_dir, write_file
 from py_basic_commands.file_dir_scripts import CreateDirs, CreateFile, GetSourcePath, JoinPath, ReadFile, RemoveFileDir, WriteFile
+from py_basic_commands.file_dir_scripts import FileEditor
 
 # From fscripts
 from py_basic_commands.fscripts import finput, fprint_array, fprint
 from py_basic_commands.fscripts import Finput, FprintArray, Fprint
 
 # From json_scripts
 from py_basic_commands.json_scripts import create_json, read_json, write_json
 from py_basic_commands.json_scripts import CreateJson, ReadJson, WriteJson
 
 # From other
-from py_basic_commands.other import choose_from_list, chunker, enter_to_continue, flatten_list, func_timer, try_traceback, timer
-from py_basic_commands.other import ChooseFromList, FunctionTimer, Timer
+from py_basic_commands.other import choose_from_list, chunker, enter_to_continue, flatten_list, func_timer, _func_timer, try_traceback, timer, try_listdir
+from py_basic_commands.other import ChooseFromList, FunctionTimer, Timer
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 from py_basic_commands.file_dir_scripts.create_dirs       import create_dirs, CreateDirs
 from py_basic_commands.file_dir_scripts.create_file       import create_file, CreateFile
 from py_basic_commands.file_dir_scripts.get_src_path      import get_src_path, GetSourcePath
 from py_basic_commands.file_dir_scripts.join_path         import join_path, JoinPath
 from py_basic_commands.file_dir_scripts.read_file         import read_file, ReadFile
 from py_basic_commands.file_dir_scripts.remove_file_dir   import remove_file_dir, RemoveFileDir
-from py_basic_commands.file_dir_scripts.write_file        import write_file, WriteFile
+from py_basic_commands.file_dir_scripts.write_file        import write_file, WriteFile
+from py_basic_commands.file_dir_scripts.file_editor       import FileEditor
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/read_json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-from py_basic_commands.file_dir_scripts.get_src_path  import get_src_path
-from py_basic_commands.fscripts   import fprint
-from py_basic_commands.base   import Base
-from dataclasses    import dataclass
-from os     import makedirs
-
-@dataclass
-class CreateDirs(Base):
-    def __post_init__(self):
-        super().__init__()
-
-
-    def __call__(self, dst_path:str, do_print:bool=None) -> bool:
-            """Create all required directories for the given path.
-            
-            Parameters:
-            - `dst_path` (str): Destination path; can include the file name at the end.
-            - `do_print` (bool): Whether to print or not. Default is `True`
-            
-            Returns:
-            - `bool`: If all directories were created or not"""
+import json
 
-            # Check input values
-            do_print = self._check_input_val(do_print, self.do_print)
-
-            fprint.config(do_print=do_print)
-
-            if dst_path == '':
-                return False
-
-            dir_path = get_src_path(dst_path, ret_val='d', do_print=do_print)
+from py_basic_commands.fscripts   import Fprint
+from py_basic_commands.base   import Base
+from traceback  import format_exc
+from typing import Any
 
-            if dir_path == '':
-                return False
+fprint = Fprint()
 
-            try:
-                makedirs(dir_path)
-                fprint(f'Destination created for path: {dir_path}')
-                return True
 
-            except FileExistsError:
-                fprint(f'Path already exists: {dir_path}')
+class ReadJson(Base):
+    def __init__(self, do_print:bool=True) -> None:
+        super().__init__(do_print)
+
+
+    def __call__(self, file_path:str, **kwargs) -> Any:
+        """Read data from a JSON file.
+        
+        Parameters
+        ----------
+        file_path : str
+            The path of the JSON file to read from.
+        do_print : bool, optional
+            Whether to get feedback printed to terminal or not. Default is True.
+        
+        Returns
+        -------
+        Any
+            The data from the JSON file, as a dictionary or list.
+        """
+
+        # Check input values
+        do_print = kwargs.get('do_print', self.do_print)
+
+        fprint.config(do_print=do_print)
+
+        try:
+            with open(file_path, 'r') as f:
+                file_data = json.load(f)
+            return file_data
+        except FileNotFoundError:
+            fprint(f'File not found: {file_path}')
+        except json.decoder.JSONDecodeError:
+            fprint(f'File cannot be read as a JSON: {file_path}')
+        except Exception:
+            fprint(format_exc())
 
-            except TypeError:
-                fprint(f'Type error in {dir_path}')
-            
-            return False
 
+read_json = ReadJson()
 
-create_dirs = CreateDirs()
 
 if __name__ == '__main__':
-    # Code testing
-    create_dirs('test folder/subfolder/file.txt')
+    from FastDebugger import fd
+    # Test code
+    file_path = 'test.json'
+    data = read_json(file_path)
+    fd(data)
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/write_json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,87 @@
-from py_basic_commands.file_dir_scripts.create_dirs   import create_dirs
-from dataclasses    import dataclass
-from traceback  import format_exc
-from py_basic_commands.fscripts   import fprint
-from os.path   import exists
-from py_basic_commands.base   import Base
+import json
 
 
-@dataclass
-class CreateFile(Base):
-    force:bool = False
+from py_basic_commands.file_dir_scripts.create_dirs import create_dirs
+from py_basic_commands.json_scripts.read_json       import read_json
+from py_basic_commands.fscripts                     import Fprint
+from py_basic_commands.base                         import Base
+from traceback      import format_exc
+from typing         import Any
 
-    def __post_init__(self):
-        super().__init__()
+fprint = Fprint()
 
 
-    def _create_empty_file(self, dst_path:str) -> bool:
-        """Create an empty file at the specified path.
-        
-        Parameters:
-        - `dst_path` (str): The path to create the file at.
-        
-        Returns:
-        - `bool`: Whether the file was created.
-        """
-        try:
-            with open(dst_path, 'w') as f:
-                f.write('')
-            fprint(f'File created: {dst_path}')
-            return True
-        except Exception:
-            fprint(format_exc())
-            return False
+class WriteJson(Base):
+    def __init__(self, force:bool=False, indent:int=4, do_print:bool=True):
+        super().__init__(do_print)
 
+        self.force = force
+        self.indent = indent
+                
 
-    def __call__(self, dst_path:str, force:bool=None, do_print:bool=None) -> bool:
-        """Create a file or directory at the specified path.
+    def __call__(self, data:Any, file_path:str, **kwargs) -> bool:
+        """Write data to a JSON file.
         
-        Parameters:
-        - `dst_path` (str): The path to create the file or directory at.
-        - `force` (bool): Whether to force the creation of the file or directory by deleting any existing file or directory with the same name. Default is `False`
-        - `do_print` (bool): Whether to print information about the file or directory creation process. Default is `True`
+        Parameters
+        ----------
+        data : Any
+            The data to write to the JSON file. This can be a dictionary, list, or a string representation of JSON.
+        file_path : str
+            The path of the JSON file to write to.
+        indent : int, optional
+            The number of spaces to use for indentation in the JSON file. Default is 4.
+        force : bool, optional
+            Whether to overwrite any existing data in the JSON file. Default is False.
+        do_print : bool, optional
+            Whether to print information about the data writing process. Default is True.
         
-        Returns:
-        - `bool`: Whether the file or directory was created.
+        Returns
+        -------
+        bool
+            Whether the file was created.
         """
 
-        if dst_path == '':
-            fprint('No path specified')
-            return False
-
         # Check input values
-        force = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self.do_print)
+        indent = kwargs.get('indent', self.indent)
+        force = kwargs.get('force', self.force)
+        do_print = kwargs.get('do_print', self.do_print)
 
         fprint.config(do_print=do_print)
+        
+        data_type = data.__class__.__name__
 
-        # Check if file already exists
-        create_dirs(dst_path, do_print=do_print)
+        try:
+            if data_type == ('str'):
+                data = json.loads(data)
 
-        if exists(dst_path):
-            fprint(f'File already exists: {dst_path}')
-            if force:
-                fprint('Force is enabled, creating new file...')
-                return self._create_empty_file(dst_path)
-            return False
+            d = read_json(file_path, do_print=do_print)
+            
+            if d and not force:
+                fprint(f'Data found in JSON file, not writing new data: {file_path}')
+                return False
+
+            with open(file_path, 'w') as f:
+                json.dump(data, f, indent=indent)
+
+            fprint(f'Wrote data to JSON file: {file_path}')
+            return True
         
-        return self._create_empty_file(dst_path)
+        except TypeError:
+            fprint(f'Data type is wrong, can\'t write to JSON: {data_type}')
+
+        except FileNotFoundError:
+            if force:
+                fprint('Force is True, creating file path')
+                create_dirs(file_path)
+                self(data, file_path, indent=indent, force=force, do_print=do_print)
+        except Exception:
+            fprint(format_exc())
+        return False
 
 
-create_file = CreateFile()
+write_json = WriteJson()
 
 if __name__ == '__main__':
-    # Code testing
-    create_file('test folder/test.txt', force=True)
+    # Test code
+    data = {"name": "John", "age": 30, "city": "New York"}
+    write_json(data, 'test.json', do_print=True, force=True)
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,78 @@
-from dataclasses    import dataclass
-from py_basic_commands.fscripts   import fprint
+from py_basic_commands.fscripts   import Fprint
 from os.path    import dirname, basename, splitext
 from typing     import Any
 from py_basic_commands.base   import Base
 
-@dataclass
-class GetSourcePath(Base):
-    ret_val:bool = 'a'
+fprint = Fprint()
+
 
-    def __post_init__(self):
+class GetSourcePath(Base):
+    """Get the path for the given source"""
+    def __init__(self, ret_val:str='a'):
+        """Initialize the class
+        
+        Parameters
+        ----------
+        ret_val : str, optional
+            Return value; 'a': (directory path, filename), 'd': directory path, 'f': filename, by default 'a'"""
         super().__init__()
 
+        self.ret_val = ret_val
 
-    def __call__(self, src_path:str, ret_val=None, do_print:bool=None) -> Any:
+
+    def __call__(self, src_path:str, **kwargs) -> Any:
         """Get the path for the given source.
         
-        Parameters:
-        - `src_path` (str): The path to the source.
-        - `ret_val` (str): Whether to return the 
-            - `'d'`: directory path
-            - `'fnam'`: name of the file
-            - `'a'`: all (default)
-
-        Returns:
-        - `Any`: If `ret_val` is `'d'`, the directory path. If `ret_val` is `'fnam'`, the filename. Otherwise, a tuple containing the directory path and the filename.
+        Parameters
+        ----------
+        src_path : str
+            Source path to get path for
+        ret_val : str, optional
+            Return value; 'a': (directory path, filename), 'd': directory path, 'f': filename, by default 'a'
+        do_print : bool, optional
+            Print output, by default True
+        
+        Returns
+        -------
+        Any
+            The path for the given source
         """
+        # Check input values
+        ret_val = kwargs.get('ret_val', self.ret_val)
+        do_print = kwargs.get('do_print', self.do_print)
+
+        fprint.config(do_print=do_print)
 
         if not src_path:
             fprint('No source path given')
             return None
 
-        # Check input values
-        ret_val = self._check_input_val(ret_val, self.ret_val)
-        do_print = self._check_input_val(do_print, self.do_print)
-
-        fprint.config(do_print=do_print)
-
         root, ext = splitext(src_path)
         if not ext:
             dir_path = root
-            fnam = ''
+            file_name = ''
         else:
-            dir_path, fnam = dirname(root), basename(root) + ext
+            dir_path, file_name = dirname(root), basename(root) + ext
 
         match ret_val:
             case 'd':
                 return dir_path
-            case 'fnam':
-                return fnam
+            case 'f':
+                return file_name
             case 'a':
-                return dir_path, fnam
+                return dir_path, file_name
             case _:
                 fprint(f'Invalid value for `ret_val`: {ret_val}')
                 return None
     
 
 get_src_path = GetSourcePath()
 
 
 if __name__ == '__main__':
     # Testing code
     src_path = 'folder/subfolder/file.txt'
-    dir_path, fnam = get_src_path(src_path, ret_val='a', do_print=True)
+    dir_path, fnam = get_src_path(src_path, ret_val='f', do_print=True)
 
     print(f'Direcotry path: {dir_path!r}')
     print(f'Filename: {fnam!r}')
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 from dataclasses    import dataclass
-from py_basic_commands.fscripts   import fprint
+from py_basic_commands.fscripts   import Fprint
 from os.path    import dirname, basename, splitext
 from py_basic_commands.base   import Base
+from typing import Any
+
+fprint = Fprint()
 
 
 @dataclass
 class JoinPath(Base):
     join_with:str = '/'
-    remove_empty:bool=True
-    dir_end:bool=False
+    remove_empty:bool = True
+    dir_end:bool = False
 
     def __post_init__(self):
         super().__init__(False)
 
 
-    def __call__(self, *args:str, join_with:str=None, remove_empty:bool=None, dir_end:bool=None, do_print:bool=None) -> str:
+    def __call__(self, *args:Any, **kwargs) -> str:
         r"""Join path segments together, removing certain characters (`<>:"/\|?*`) and adjust for correct slash direction.
 
-        Parameters:
-        - `*args` (str): One or more path segments to join.
-        - `join_with` (str): The separator to use when joining the path segments. Default is `'/'`.
-        - `remove_empty` (bool): Remove empty strings. Default is `True`.
-        - `dir_end` (bool): Specify whether to add join_with character at the end of the returned path. Default is `False`.
-        - `do_print` (bool): Whether to print or not. Default is `False`.
-
-        Return:
-        A `string` representing the joined path.
+        Parameters
+        ----------
+        *args : Any
+            The path segments to join together. If a list is given, the values will be joined by the `join_with` character
+        join_with : str, optional
+            The character to use to join the path segments together. Default is '/'
+        remove_empty : bool, optional
+            Whether to remove empty strings from the path segments. Default is True
+        dir_end : bool, optional
+            Whether to add the `join_with` character at the end of the path. Default is False
+        do_print : bool, optional
+            Whether to print information about the file creation process. Default is True
+        
+        Returns
+        -------
+        str
+            The joined path
         """
 
         def split_join(var:str, split_with:str=' '):
             """Split a string and then join it back together"""
             return join_with.join(var.split(split_with))
         
         # Check input values
-        join_with = self._check_input_val(join_with, self.join_with)
-        remove_empty = self._check_input_val(remove_empty, self.remove_empty)
-        dir_end = self._check_input_val(dir_end, self.dir_end)
-        do_print = self._check_input_val(do_print, self.do_print)
+        join_with = kwargs.get('join_with', self.join_with)
+        remove_empty = kwargs.get('remove_empty', self.remove_empty)
+        dir_end = kwargs.get('dir_end', self.dir_end)
+        do_print = kwargs.get('do_print', self.do_print)
 
         fprint.config(do_print=do_print)
 
         # Iterate through args and join them together
         new_args = []
         for arg_indx, arg in enumerate(args):
             # Remove invalid characters
             arg = split_join(split_join(arg, '\\'), '/')
-            arg = arg.translate({ord(c): None for c in '<>"|?*'}) # ":" is an invalid character on Windows, but drivers can use it. E.g. "C:\"
+            arg = arg.translate({ord(c): None for c in '<>:"|?*'})
 
             # Remove empty strings
             split_arg = arg.split('/')
             if '' in split_arg and remove_empty:
                 fprint(f'Empty string found in input arg (indx: {arg_indx}): {arg!r}')
                 split_arg = [x for x in split_arg if x != '']
                 arg = join_with.join(split_arg)
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,97 +1,122 @@
 from py_basic_commands.file_dir_scripts   import create_file
+from py_basic_commands.fscripts.fprint   import Fprint
+from py_basic_commands.base   import Base
 from dataclasses    import dataclass
-from py_basic_commands.fscripts.fprint   import fprint
 from typing     import Any
-from py_basic_commands.base   import Base
+
+fprint = Fprint()
 
 
 @dataclass
 class ReadFile(Base):
-    create:bool = False
+    """Read the contents of a file"""
+    create:bool         = False
     ret_did_create:bool = False
-    splitlines:bool = True
-    remove_empty:bool = True
-    do_strip:bool = True
-    do_lower:bool = False
-    encoding:str = 'utf-8'
+    splitlines:bool     = True
+    remove_empty:bool   = True
+    do_strip:bool       = True
+    do_lower:bool       = False
+    encoding:str        = 'utf-8'
+    do_print:bool       = True
 
 
     def __post_init__(self):
-        super().__init__()
+        super().__init__(self.do_print)
 
     
-    def __call__(self, file_path:str, create:bool=None, ret_did_create:bool=None, splitlines:bool=None, remove_empty:bool=None, do_strip:bool=None, do_lower:bool=None, encoding:str=None, do_print:bool=None) -> Any:
+    def __call__(self, file_path:str, **kwargs) -> Any:
         """Read the contents of a file.
         
-        Parameters:
-        - `file_path` (str): The path to the file to read.
-        - `create` (bool): Whether to create the file if it does not exist. Default is `False`
-        - `ret_did_create` (bool): Whether to return a tuple of the file contents and a bool indicating whether the file was created. Default is `False`
-        - `splitlines` (bool): Whether to split the file contents into a list of lines. Default is `True`
-        - `remove_empty` (bool): Whether to remove empty lines when `splitlines` is True. Default is `True`
-        - `strip` (bool): Whether to strip leading and trailing whitespace from each line when `splitlines` is True.
-        - `encoding` (str): The encoding to use when reading the file. Default is `utf-8`
-        - `do_print` (bool): Whether to print information about the file reading process. Default is `True`
+        Parameters
+        ----------
+        file_path : str
+            The path to the file to read
+        create : bool, optional
+            Whether to create the file if it does not exist. Default is False
+        ret_did_create : bool, optional
+            Whether to return whether the file was created. Default is False
+        splitlines : bool, optional
+            Whether to split the file contents by line. Default is True
+        remove_empty : bool, optional
+            Whether to remove empty lines from the file contents; only works if `splitlines` is True. Default is True
+        do_strip : bool, optional
+            Whether to strip the file contents of whitespace; only works if `splitlines` is True. Default is True
+        do_lower : bool, optional
+            Whether to convert the file contents to lowercase. Default is False
+        encoding : str, optional
+            The encoding to use when reading the file. Default is 'utf-8'
+        do_print : bool, optional
+            Whether to print information about the file creation process. Default is True
         
-        Returns:
-        - `Any`: If `ret_did_create` is True, a tuple containing the file contents and a bool indicating whether the file was created. Otherwise, the file contents.
+        Returns
+        -------
+        Any
+            The file contents
         """
         
-        def try_reading(did_create:bool=False) -> list and bool:
+        def try_reading(did_create:bool=False) -> tuple:
             """Tries reading the file. If the file does not exist, creates it if `create` is True.
             
-            Parameters:
-            - `did_create` (bool): Whether the file was created.
+            Parameters
+            ----------
+            did_create : bool, optional
+                Whether the file was created. Default is False
             
-            Returns:
-            - `Any`: If `ret_did_create` is True, a tuple containing the file contents and a bool indicating whether the file was created. Otherwise, the file contents.
+            Returns
+            -------
+            tuple
+                The file contents and whether the file was created
             """
             lines: list[str] | str = []
+
             try:
                 with open(file_path, 'r', encoding=encoding) as f:
                     lines = f.read()
                 if splitlines:
                     lines = lines.splitlines()
                     if remove_empty:
                         lines = [x for x in lines if x != '']
                     if do_strip:
                         lines = [x.strip() for x in lines]
                     if do_lower:
                         lines = [x.lower() for x in lines]
                 return lines, did_create
+            
             except FileNotFoundError:
                 fprint(f'File not found: {file_path}', do_print=do_print)
                 if create:
                     create_file(file_path, force=True, do_print=do_print)
                     return try_reading(True)
+                
             return lines, did_create
 
         # Check input values
-        create      = self._check_input_val(create, self.create)
-        ret_did_create = self._check_input_val(ret_did_create, self.ret_did_create)
-        splitlines  = self._check_input_val(splitlines, self.splitlines)
-        remove_empty = self._check_input_val(remove_empty, self.remove_empty)
-        do_strip    = self._check_input_val(do_strip, self.do_strip)
-        do_lower    = self._check_input_val(do_lower, self.do_lower)
-        encoding    = self._check_input_val(encoding, self.encoding)
-        do_print    = self._check_input_val(do_print, self.do_print)
+        create          = kwargs.get('create', self.create)
+        ret_did_create  = kwargs.get('ret_did_create', self.ret_did_create)
+        splitlines      = kwargs.get('splitlines', self.splitlines)
+        remove_empty    = kwargs.get('remove_empty', self.remove_empty)
+        do_strip        = kwargs.get('do_strip', self.do_strip)
+        do_lower        = kwargs.get('do_lower', self.do_lower)
+        encoding        = kwargs.get('encoding', self.encoding)
+        do_print        = kwargs.get('do_print', self.do_print)
 
         fprint.config(do_print=do_print)
 
         lines, did_create = try_reading()
 
         # Return the file contents
         if ret_did_create:
             return lines, did_create
         return lines
 
 
 read_file = ReadFile()
 
+
 if __name__ == '__main__':
     from FastDebugger import fd
 
     # Test code
     file_path = 'Test folder/here.txt'
     f = read_file(file_path, create=True)
     fd(f)
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,69 @@
-from py_basic_commands.other.basic_commands     import try_traceback
-from py_basic_commands.file_dir_scripts   import read_file
-from py_basic_commands.fscripts   import fprint
+from py_basic_commands.file_dir_scripts.get_src_path  import get_src_path
+from py_basic_commands.fscripts   import Fprint
 from py_basic_commands.base   import Base
-from dataclasses    import dataclass
-from shutil     import rmtree
-from os     import listdir, remove
+from os     import makedirs
 
+fprint = Fprint()
 
-@dataclass
-class RemoveFileDir(Base):
-    force:bool = True
 
-    def __post_init__(self):
-        super().__init__()
+class CreateDirs(Base):
+    """Create all required directories for the given path"""
+    def __init__(self, do_print:bool=True):
+        """Initialize the class
+        
+        Parameters
+        ----------
+        do_print : bool, optional
+            Whether to print information about the directory creation process. Default is True"""
+        super().__init__(do_print)
 
 
-    @try_traceback(print_traceback=True)
-    def __call__(self, do:str, do_path:str, force:bool=None, do_print:bool=None) -> bool:
-        """Remove a file or directory at the specified path.
-        
-        Parameters:
-        - `do` (str): Whether to remove a `'d'`irectory or a `'f'`ile.
-        - `do_path` (str): The path to the file or directory to remove.
-        - `force` (bool): Whether to force the removal of the file or directory.
-        - `do_print` (bool): Whether to print information about the file or directory removal process.
-        
-        Returns:
-        - `bool`: Whether the file or directory was removed.
-        """
+    def __call__(self, dst_path:str, **kwargs) -> bool:
+            """Create all required directories for the given path.
+            
+            Parameters
+            ----------
+            dst_path : str
+                The path to create the directories for.
+            do_print : bool, optional
+                Whether to print information about the directory creation process. Default is True
 
-        # Check input values
-        force    = self._check_input_val(force, self.force)
-        do_print = self._check_input_val(do_print, self.do_print)
+            Returns
+            -------
+            bool
+                Whether the directories were created
+            """
 
-        fprint.config(do_print=do_print)
+            # Check input values
+            do_print = kwargs.get('do_print', self.do_print)
 
-        if do == 'd': # Directory
-            try:
-                dir_content = listdir(do_path)
-            except FileNotFoundError:
-                fprint(f'Directory path not found: {do_path}')
-                return False
-            except NotADirectoryError:
-                fprint(f'Path is not a directory: {do_path}')
-                return False
+            # Set print config
+            fprint.config(do_print=do_print)
 
-            if not dir_content or force:
-                rmtree(do_path)
-                fprint(f'Directory removed: {do_path}')
-                return True
-                
-            elif dir_content:
-                fprint(f'Directory is not empty, not removing: {do_path}')
-                return False
-            
-            else:
+            if dst_path == '':
                 return False
 
-        elif do == 'f': # File
-            lines = read_file(do_path)
-            if lines and not force:
-                fprint(f'File is not empty, not removing: {do_path}')
+            dir_path = get_src_path(dst_path, ret_val='d', do_print=do_print)
+
+            if dir_path == '':
                 return False
+
             try:
-                remove(do_path)
-            except FileNotFoundError:
-                fprint(f'File path not found: {do_path}')
-                return False
-            except IsADirectoryError:
-                fprint(f'Path is a directory: {do_path}')
-                return False
-            except PermissionError:
-                fprint(f'Permission denied: {do_path}')
-                return False
-            except OSError:
-                fprint(f'File is being used by another process: {do_path}')
-                return False
-            except Exception as err:
-                fprint(f'Error removing file: {do_path}')
-                raise err
+                makedirs(dir_path)
+                fprint(f'Destination created for path: {dir_path}')
+                return True
 
-            fprint(f'File removed: {do_path}')
-            return True
+            except FileExistsError:
+                fprint(f'Path already exists: {dir_path}')
+
+            except TypeError:
+                fprint(f'Type error in {dir_path}')
+            
+            return False
 
 
-remove_file_dir = RemoveFileDir()
+create_dirs = CreateDirs()
 
 if __name__ == '__main__':
-    # Test code
-    remove_file_dir.config(do_print=False)
-    remove_file_dir('d', 'Test folder', force=True, do_print=False)
+    # Code testing
+    create_dirs('test folder/subfolder/file.txt')
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.25b1/py_basic_commands/fscripts/finput.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-from dataclasses    import dataclass
-from py_basic_commands.fscripts.fprint   import fprint
+from py_basic_commands.fscripts.fprint   import Fprint
 from py_basic_commands.base   import Base
+from dataclasses    import dataclass
+
+fprint = Fprint()
 
 
 @dataclass
 class Finput(Base):
     text:str = 'Input: '
     nl:bool = True
     use_suffix:bool = True
     ret_type:type = str
+    do_print:bool = True
 
     def __post_init__(self):
-        super().__init__()
+        super().__init__(self.do_print)
 
 
-    def __call__(self, text:str=None, ret_type:type=None, nl:bool=None, use_suffix:bool=None):
+    def __call__(self, **kwargs):
         """Get input from the user and return it as a specified type.
         
-        Parameters:
-        - `text` (str): The text to prompt the user with. Default is an `'Input: '`.
-        - `ret_type` (type): The type to return the input as. Default is `str`.
-        - `nl` (bool): Whether to append a newline character after the input. Default is `True`.
-        - `use_suffix` (bool): Whether to append a colon character to the end of the prompt text. Default is `True`.
-        
-        Returns:
-        - The input value, converted to the specified type. If the conversion fails, the value is returned as a string.
+        Parameters
+        ----------
+        text : str, optional
+            The text to prompt the user with. Default is an `'Input: '`.
+        ret_type : type, optional
+            The type to return the input as. Default is `str`.
+        nl : bool, optional
+            Whether to append a newline character after the input. Default is `True`.
+        use_suffix : bool, optional
+            Whether to append a colon character to the end of the prompt text. Default is `True`.
+
+        Returns
+        -------
+        Any
+            The input value, converted to the specified type. If the conversion fails, the value is returned as a string.
         """
 
-        text = self._check_input_val(text, self.text)
-        nl = self._check_input_val(nl, self.nl)
-        use_suffix = self._check_input_val(use_suffix, self.use_suffix)
-        ret_type = self._check_input_val(ret_type, self.ret_type)
+        text = kwargs.get('text', self.text)
+        nl = kwargs.get('nl', self.nl)
+        use_suffix = kwargs.get('use_suffix', self.use_suffix)
+        ret_type = kwargs.get('ret_type', self.ret_type)
 
         if use_suffix and text.rstrip()[-1] != ':':
             text = f'{text}: '
 
         inpt = input(text)
 
         if nl:
@@ -50,8 +60,8 @@
 
 
 finput = Finput()
 
 
 if __name__ == '__main__':
     # Test `finput`
-    print(finput('Enter a number', ret_type=int))
+    print(finput(text='Enter a number', ret_type=int))
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint_array.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 import executing, sys
 
+from py_basic_commands.base   import Base
 from dataclasses    import dataclass
 from textwrap   import dedent
-from py_basic_commands.base   import Base
 
 
 @dataclass
 class FprintArray(Base):
     header:str=''
     indx_brackets:str='[]'
     print_num=False
     start_num:int=0
     nl:bool=True
+    do_print:bool=True
 
     def __post_init__(self):
-        super().__init__()
+        super().__init__(self.do_print)
 
 
-    def __call__(self, arr, header:str=None, indx_brackets:str=None, print_num=None, start_num:int=None, nl:bool=None) -> None:
+    def __call__(self, arr, **kwargs) -> None:
         """This function prints the elements of an array along with their index numbers.
 
-        Parameters:
-        - `arr` (`list`|`set`|`tuple`|`dict`): The input array whose elements are to be printed.
-        - `header` (str):  The header message to be printed before the array elements. Defaults is ''.
-        - `indx_brackets` (str): The type of brackets to be used for index numbers. Defaults is '`[]`'.
-        - `start_num` (int): First shown value starts with this number. Default is `0`.
-        - `nl` (bool): Whether to append a newline character after the input. Default is `True`
-        
-        Returns:
-        - `None`
+        Parameters
+        ----------
+        arr : list|set|tuple|dict
+            The input array whose elements are to be printed.
+        header : str, optional
+            The header message to be printed before the array elements. Defaults is ''.
+        indx_brackets : str, optional
+            The type of brackets to be used for index numbers. Defaults is '`[]`'.
+        print_num : bool, optional
+            Whether to print the index numbers of the array elements. Default is `False`.
+        start_num : int, optional
+            First shown value starts with this number. Default is `0`.
+        nl : bool, optional
+            Whether to append a newline character after the input. Default is `True`
         """
 
         def _get_array_name() -> str:
-            """Get the name of the input array."""
+            """Get the name of the input array.
+            
+            Returns
+            -------
+            str
+                The name of the input array"""
             class Source(executing.Source):
                 def get_text_with_indentation(self, node):
                     result = self.asttokens().get_text(node)
                     if '\n' in result:
                         result = ' ' * node.first_token.start[1] + result
                         result = dedent(result)
                     result = result.strip()
                     return result
             
             callFrame = sys._getframe(2)
             callNode = Source.executing(callFrame).node
             source = Source.for_frame(callFrame)
-            inpt_array_name = source.get_text_with_indentation(callNode.args[0])
+            inpt_array_name = source.get_text_with_indentation(callNode.args[0]) # type: ignore
 
             return inpt_array_name
 
 
         def _print_output(text) -> None:
             """Print the output of the array elements and their index numbers if `print_num` is `True`. Otherwise, just print the array elements.
             If the input is a dictionary, then print the key-value pairs."""
@@ -59,19 +70,19 @@
             if print_num:
                 print(f'{config_indx_num(indx)} {text}')
             else:
                 print(text)
 
 
         # Check input values
-        header      = self._check_input_val(header, self.header)
-        indx_brackets = self._check_input_val(indx_brackets, self.indx_brackets)
-        print_num   = self._check_input_val(print_num, self.print_num)
-        start_num   = self._check_input_val(start_num, self.start_num)
-        nl          = self._check_input_val(nl, self.nl)
+        header      = kwargs.get('header', self.header)
+        indx_brackets = kwargs.get('indx_brackets', self.indx_brackets)
+        print_num   = kwargs.get('print_num', self.print_num)
+        start_num   = kwargs.get('start_num', self.start_num)
+        nl          = kwargs.get('nl', self.nl)
 
         config_indx_num = lambda indx : f'{indx_brackets[0]}{indx}{indx_brackets[1]}'
 
         arr_type = arr.__class__.__name__
 
         # Check if the input is a valid array
         if arr_type in ['list', 'set', 'tuple', 'dict']:
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/create_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 import json
 
 from py_basic_commands.file_dir_scripts   import create_file, read_file
-from dataclasses    import dataclass
 from py_basic_commands.json_scripts.read_json  import read_json
-from py_basic_commands.fscripts   import fprint
+from py_basic_commands.fscripts   import Fprint
 from py_basic_commands.base   import Base
 
+fprint = Fprint()
+
 
-@dataclass
 class CreateJson(Base):
-    force:bool = True
+    """Create a new empty JSON file."""
+    def __init__(self, force:bool=True, do_print:bool=True):
+        """Initialize the class
+        
+        Parameters
+        ----------
+        force : bool, optional
+            Whether to overwrite any existing file with the same name. Default is True
+        do_print : bool, optional
+            Whether to print information about the file creation process. Default is True"""
+        super().__init__(do_print)
 
-    def __post_init__(self):
-        super().__init__()
+        self.force = force
 
 
-    def __call__(self, file_path:str, force:bool=None, do_print:bool=None) -> bool:
+    def __call__(self, file_path:str, **kwargs) -> bool:
         """Create a new empty JSON file.
         
-        Parameters:
-        - `file_path` (str): The path for the new JSON file.
-        - `force` (bool): Whether to overwrite any existing file with the same name. Default is `True`.
-        - `do_print` (bool): Whether to print information about the file creation process. Default is `True`.
+        Parameters
+        ----------
+        file_path : str
+            The path for the new JSON file
+        force : bool, optional
+            Whether to overwrite any existing file with the same name. Default is True
         
-        Returns:
-        - `bool`: Whether the file was created.
+        Returns
+        -------
+        bool
+            Whether the file was created
         """
 
         # Check input values
-        force = self._check_input_val(force, self._force)
-        do_print = self._check_input_val(do_print, self.do_print)
+        force = kwargs.get('force', self.force)
+        do_print = kwargs.get('do_print', self.do_print)
 
         fprint.config(do_print=do_print)
 
         write_empty_json = lambda: open(file_path, 'w').write(json.dumps({}, indent=4))
 
         did_create = create_file(file_path, force=force, do_print=do_print)
         if did_create:
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,101 @@
-import json
-
-from py_basic_commands.json_scripts.read_json  import read_json
-from py_basic_commands.file_dir_scripts.create_dirs import create_dirs
-from dataclasses    import dataclass
-from traceback  import format_exc
-from py_basic_commands.fscripts   import fprint
-from typing     import Any
+from py_basic_commands.file_dir_scripts   import read_file
+from py_basic_commands.fscripts   import Fprint
 from py_basic_commands.base   import Base
+from dataclasses    import dataclass
+from send2trash import send2trash
+from os     import listdir
+
+fprint = Fprint()
 
 
 @dataclass
-class WriteJson(Base):
-    indent:bool = True
-    force:bool = False
+class RemoveFileDir(Base):
+    """Remove a file or directory at the specified path."""
+    def __init__(self, force:bool=True, do_print:bool=True):
+        """Initialize the class
+
+        Parameters
+        ----------
+        force : bool, optional
+            Whether to force the removal of the file or directory. Default is True
+        do_print : bool, optional
+            Whether to print information about the file or directory removal process. Default is True
+        """
+        super().__init__(do_print)
 
-    def __post_init__(self):
-        super().__init__()
-                
+        self.force = force
 
-    def __call__(self, data:Any, file_path:str, force:bool=None, indent:int=None, do_print:bool=None) -> bool:
-        """Write data to a JSON file.
-        
-        Parameters:
-        - `data` (Any): The data to write to the JSON file. This can be a dictionary, list, or a string representation of JSON.
-        - `file_path` (str): The path of the JSON file to write to.
-        - `indent` (int): The number of spaces to use for indentation in the JSON file. Default is `4`.
-        - `force` (bool): Whether to overwrite any existing data in the JSON file. Default is `False`.
-        - `do_print` (bool): Whether to print information about the data writing process. Default is `True`.
 
-        Return:
-        - `bool`: Whether the file was created.
+    def __call__(self, do:str, do_path:str, **kwargs) -> bool:
+        """Remove a file or directory at the specified path.
+        
+        Parameters
+        ----------
+        do : str
+            Whether to remove a file or directory. Must be either 'f' or 'd'
+        do_path : str
+            The path to remove the file or directory at
+        force : bool, optional
+            Whether to force the removal of the file or directory. Default is True
+        do_print : bool, optional
+            Whether to print information about the file or directory removal process. Default is True
+    
+        Returns
+        -------
+        bool
+            Whether the file or directory was removed
+
+        Raises
+        ------
+        ValueError
+            If an invalid `do` value is given
         """
 
         # Check input values
-        indent = self._check_input_val(indent, self.indent)
-        force = self._check_input_val(force, self.force)
-        do_print = self._check_input_val(do_print, self.do_print)
+        force    = kwargs.get('force', self.force)
+        do_print = kwargs.get('do_print', self.do_print)
 
         fprint.config(do_print=do_print)
 
-        try:
-            if data.__class__.__name__ == ('str'):
-                data = json.loads(data)
-
-            d = read_json(file_path, do_print=do_print)
+        if do == 'd': # Directory
+            try:
+                dir_content = listdir(do_path)
+                
+            except FileNotFoundError:
+                fprint(f'Directory path not found: {do_path}')
+                return False
             
-            if d and not force:
-                fprint(f'Data found in JSON file, not writing new data: {file_path}')
+            except NotADirectoryError:
+                fprint(f'Path is not a directory: {do_path}')
                 return False
 
-            with open(file_path, 'w') as f:
-                json.dump(data, f, indent=indent)
+            if not dir_content or force:
+                send2trash(do_path)
+                fprint(f'Directory removed: {do_path}')
+                return True
+                
+            elif dir_content:
+                fprint(f'Directory is not empty, not removing: {do_path}')
+                return False
+            
+            else:
+                return False
 
-            fprint(f'Wrote data to JSON file: {file_path}')
+        elif do == 'f': # File
+            lines = read_file(do_path)
+            if lines and not force:
+                fprint(f'File is not empty, not removing: {do_path}')
+                return False
+            send2trash(do_path)
+            fprint(f'File removed: {do_path}')
             return True
-        except TypeError:
-            fprint(f'Data type is wrong, can\'t write to JSON: {data.__class__.__name__}')
-        except FileNotFoundError:
-            if force:
-                fprint('Force is True, creating file path')
-                create_dirs(file_path)
-                self(data, file_path, indent=indent, force=force, do_print=do_print)
-        except Exception:
-            fprint(format_exc())
-        return False
+        
+        else:
+            raise ValueError(f'Invalid do value given: {do}')
 
 
-write_json = WriteJson()
+remove_file_dir = RemoveFileDir()
 
 if __name__ == '__main__':
     # Test code
-    data = {"name": "John", "age": 30, "city": "New York"}
-    write_json(data, 'test.json', do_print=True, force=True)
+    remove_file_dir('d', 'Test folder', force=True)
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.25b1/py_basic_commands/other/basic_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,113 @@
 from traceback  import format_exc
 from functools  import wraps
-from py_basic_commands.fscripts     import fprint
+from py_basic_commands.fscripts     import Fprint
 from typing     import Any
+from os     import listdir 
 
+fprint = Fprint()
 
 def try_traceback(print_traceback=False):
     """Decorator to catch and handle exceptions raised by a function.
     
-    Parameters:
-    - `print_traceback` (bool): Whether to skip printing the traceback information.
-    
-    Returns:
-    - `function`: The decorated function.
+    Parameters
+    ----------
+    print_traceback : bool, optional
+        Whether to print the traceback if an exception is raised, by default False
+    
+    Returns
+    -------
+    function
+        The decorated function
     """
-
     def try_except(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception:
-                if print_traceback:
-                    fprint(format_exc())
-                return None
+                fprint(format_exc(), do_print=print_traceback)
         return wrapper
     return try_except
 
 
 def enter_to_continue(text:str='', nl:bool=True, use_suffix:bool=True) -> bool:
     """Prompt the user to press the enter key to continue.
     
-    Parameters:
-    - `text` (str): The text to prompt the user with.
-    - `nl` (bool): Whether to append a newline character after the input.
-    - `use_suffix` (bool): Whether to append '(press enter to continue)' to the end of the prompt text.
-    
-    Returns:
-    - `bool`: True if the user pressed the enter key, False otherwise.
+    Parameters
+    ----------
+    text : str, optional
+        The text to display, by default ''
+    nl : bool, optional
+        Whether to print a newline after the text, by default True
+    use_suffix : bool, optional
+        Whether to use the default suffix, by default True
+
+    Returns
+    -------
+    bool
+        Whether the user pressed the enter key
     """
-
     if text and use_suffix:
         text = f'{text} (press enter to continue or type anything to break) '
 
     elif not text and use_suffix:
         text = 'Press enter to continue or type anything to break... '
     
     inpt = input(text)
     
     if nl:
         print()
 
     return not any(inpt)
 
 
-def chunker(seq, size:int) -> Any:
+def chunker(seq, size:int) -> list[Any]:
     """Split a sequence into chunks of the specified size.
     
-    Parameters:
-    - `seq` (Any): The sequence to split. Can be a list, tuple, or any other iterable object.
-    - `size` (int): The size of the chunks.
-    
-    Returns:
-    - `Any`: A list of chunks of the specified size.
+    Parameters
+    ----------
+    seq : Any
+        The sequence to split
+    size : int
+        The size of each chunk
+    
+    Returns
+    -------
+    Any
+        The sequence split into chunks of the specified size
     """
-
     return [seq[pos:pos + size] for pos in range(0, len(seq), size)]
 
 
 def flatten_list(lst:list[Any]) -> Any:
-    return [item for sublist in lst for item in sublist]
+    """Flatten a list of lists.
+    
+    Parameters
+    ----------
+    lst : list[Any]
+        The list to flatten
+        
+    Returns
+    -------
+    Any
+        The flattened list"""
+    return [item for sublist in lst for item in sublist]
+
+
+def try_listdir(path:str) -> list[str]:
+    """Try to list the contents of the given directory.
+    
+    Parameters
+    ----------
+    path : str
+        The path to list the contents of
+
+    Returns
+    -------
+    list[str]
+        The contents of the directory, or an empty list if the directory does not exist or the file cannot be read
+    """
+    try:
+        return listdir(path)
+    except FileNotFoundError:
+        return []
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.25b1/py_basic_commands/other/timer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,68 @@
-from dataclasses    import dataclass
-from py_basic_commands.fscripts   import fprint
+from py_basic_commands.fscripts import Fprint
+from py_basic_commands.base     import Base
 from time   import perf_counter
-from py_basic_commands.base   import Base
 
-@dataclass
+fprint = Fprint()
+
+
 class Timer(Base):
-    def __post_init__(self) -> None:
-        super().__init__()
+    """A class for timing processes"""
+    def __init__(self, do_print:bool=True) -> None:
+        """Initialize the class
+        
+        Parameters
+        ----------
+        do_print : bool, optional
+            Whether to print information about the timer starting process. Default is True"""
+        super().__init__(do_print)
 
         self.timer_lst:dict[str,float] = {}
 
 
-    def start_timer(self, timer_name:str, do_print:bool=True) -> bool:
-        """Start a timer with a specified name"""
+    def start_timer(self, timer_name:str, **kwargs) -> bool:
+        """Start a timer with a specified name
+        
+        Parameters
+        ----------
+        timer_name : str
+            The name of the timer
+        do_print : bool, optional
+            Whether to print information about the timer starting process. Default is True
+            
+        Returns
+        -------
+        bool
+            Whether the timer was started"""
 
         # Chek values
-        do_print = self._check_input_val(do_print, self.do_print)
+        do_print = kwargs.get('do_print', self.do_print)
 
         if self.timer_lst.get(timer_name):
             print(f'Timer with name already started: {timer_name}')
             return False
 
         self.timer_lst[timer_name] = perf_counter()
         fprint(f'Timer started: {timer_name}', do_print=do_print)
 
         return True
 
 
     def end_timer(self, timer_name:str) -> float:
-        """End timer with given name"""
+        """End timer with given name
+        
+        Parameters
+        ----------
+        timer_name : str
+            The name of the timer
+        
+        Returns
+        -------
+        float
+            The time in seconds that the timer ran for"""
 
         if not self.timer_lst.get(timer_name):
             print(f'No timer found with name: {timer_name}')
             return 0.0
 
         delta_time = perf_counter() - self.timer_lst[timer_name]
         if delta_time < 0.0001:
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.25b1/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.24
+Version: 0.2.25b1
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.24/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.25b1/py_basic_commands.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 py_basic_commands.egg-info/PKG-INFO
 py_basic_commands.egg-info/SOURCES.txt
 py_basic_commands.egg-info/dependency_links.txt
 py_basic_commands.egg-info/top_level.txt
 py_basic_commands/file_dir_scripts/__init__.py
 py_basic_commands/file_dir_scripts/create_dirs.py
 py_basic_commands/file_dir_scripts/create_file.py
+py_basic_commands/file_dir_scripts/file_editor.py
 py_basic_commands/file_dir_scripts/get_src_path.py
 py_basic_commands/file_dir_scripts/join_path.py
 py_basic_commands/file_dir_scripts/read_file.py
 py_basic_commands/file_dir_scripts/remove_file_dir.py
 py_basic_commands/file_dir_scripts/write_file.py
 py_basic_commands/fscripts/__init__.py
 py_basic_commands/fscripts/finput.py
 py_basic_commands/fscripts/fprint.py
 py_basic_commands/fscripts/fprint_array.py
 py_basic_commands/json_scripts/__init__.py
 py_basic_commands/json_scripts/create_json.py
+py_basic_commands/json_scripts/json_editor.py
 py_basic_commands/json_scripts/read_json.py
 py_basic_commands/json_scripts/write_json.py
 py_basic_commands/other/__init__.py
 py_basic_commands/other/basic_commands.py
 py_basic_commands/other/choose_from_list.py
 py_basic_commands/other/function_timer.py
 py_basic_commands/other/timer.py
```

### Comparing `py_basic_commands-0.2.24/pyproject.toml` & `py_basic_commands-0.2.25b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.24"
+version = "0.2.25-beta.01"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.24/setup.cfg` & `py_basic_commands-0.2.25b1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.24
+version = 0.2.25-beta.01
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

