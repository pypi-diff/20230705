# Comparing `tmp/py_basic_commands-0.2.25b1.tar.gz` & `tmp/py_basic_commands-0.2.25b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_basic_commands-0.2.25b1.tar", last modified: Wed Jul  5 00:32:44 2023, max compression
+gzip compressed data, was "py_basic_commands-0.2.25b2.tar", last modified: Wed Jul  5 00:58:58 2023, max compression
```

## Comparing `py_basic_commands-0.2.25b1.tar` & `py_basic_commands-0.2.25b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/example_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/get_src_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/join_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/remove_file_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/write_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/finput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/create_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/read_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/write_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.390520 py_basic_commands-0.2.25b1/py_basic_commands/other/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/choose_from_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/function_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/py_basic_commands/other/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:32:44.386520 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 00:32:44.000000 py_basic_commands-0.2.25b1/py_basic_commands.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-05 00:32:28.000000 py_basic_commands-0.2.25b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-05 00:32:44.394520 py_basic_commands-0.2.25b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/example_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/get_src_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/join_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/remove_file_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/write_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/finput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/create_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/read_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/write_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/py_basic_commands/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/choose_from_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/function_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/py_basic_commands/other/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:58:58.188336 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 00:58:58.000000 py_basic_commands-0.2.25b2/py_basic_commands.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 00:58:44.000000 py_basic_commands-0.2.25b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 00:58:58.192335 py_basic_commands-0.2.25b2/setup.cfg
```

### Comparing `py_basic_commands-0.2.25b1/LICENSE.md` & `py_basic_commands-0.2.25b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/PKG-INFO` & `py_basic_commands-0.2.25b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_basic_commands
-Version: 0.2.25b1
+Version: 0.2.25b2
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.25b1/README.md` & `py_basic_commands-0.2.25b2/README.md`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/__init__.py` & `py_basic_commands-0.2.25b2/py_basic_commands/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 # From fscripts
 from py_basic_commands.fscripts import finput, fprint_array, fprint
 from py_basic_commands.fscripts import Finput, FprintArray, Fprint
 
 # From json_scripts
 from py_basic_commands.json_scripts import create_json, read_json, write_json
 from py_basic_commands.json_scripts import CreateJson, ReadJson, WriteJson
+from py_basic_commands.json_scripts import JsonEditor
 
 # From other
 from py_basic_commands.other import choose_from_list, chunker, enter_to_continue, flatten_list, func_timer, _func_timer, try_traceback, timer, try_listdir
 from py_basic_commands.other import ChooseFromList, FunctionTimer, Timer
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/base.py` & `py_basic_commands-0.2.25b2/py_basic_commands/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,27 +20,14 @@
         ----------
         **kwargs : Any
             The variables to configure
         """
         for key, value in kwargs.items():
             if hasattr(self, key):
                 setattr(self, key, value)
-       
-
-    def _check_input_val(self, inpt_val, saved_val):
-        """Check if input value is None, if so return saved value
-        
-        Parameters
-        ----------
-        inpt_val : Any
-            The input value to check
-        saved_val : Any
-            The saved value to return if the input value is None
-        """
-        return saved_val if inpt_val == None else inpt_val
 
 
 class EditorBase(Base):
     """Base class for all file editors"""
     def __init__(self, file_path:str, do_print=True) -> None:
         """Initialize the class
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/__init__.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_dirs.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_dirs.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/create_file.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/create_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/file_editor.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/file_editor.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/get_src_path.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/get_src_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from py_basic_commands.base   import Base
 
 fprint = Fprint()
 
 
 class GetSourcePath(Base):
     """Get the path for the given source"""
-    def __init__(self, ret_val:str='a'):
+    def __init__(self, ret_val:str='a', do_print:bool=True):
         """Initialize the class
         
         Parameters
         ----------
         ret_val : str, optional
             Return value; 'a': (directory path, filename), 'd': directory path, 'f': filename, by default 'a'"""
-        super().__init__()
+        super().__init__(do_print=do_print)
 
         self.ret_val = ret_val
 
 
     def __call__(self, src_path:str, **kwargs) -> Any:
         """Get the path for the given source.
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/join_path.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/join_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 
 @dataclass
 class JoinPath(Base):
     join_with:str = '/'
     remove_empty:bool = True
     dir_end:bool = False
+    do_print:bool = False
 
     def __post_init__(self):
-        super().__init__(False)
+        super().__init__(self.do_print)
 
 
     def __call__(self, *args:Any, **kwargs) -> str:
         r"""Join path segments together, removing certain characters (`<>:"/\|?*`) and adjust for correct slash direction.
 
         Parameters
         ----------
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/read_file.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/read_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     splitlines:bool     = True
     remove_empty:bool   = True
     do_strip:bool       = True
     do_lower:bool       = False
     encoding:str        = 'utf-8'
     do_print:bool       = True
 
-
     def __post_init__(self):
         super().__init__(self.do_print)
 
     
     def __call__(self, file_path:str, **kwargs) -> Any:
         """Read the contents of a file.
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/remove_file_dir.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/remove_file_dir.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/file_dir_scripts/write_file.py` & `py_basic_commands-0.2.25b2/py_basic_commands/file_dir_scripts/write_file.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/fscripts/finput.py` & `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/finput.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint.py` & `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/fscripts/fprint_array.py` & `py_basic_commands-0.2.25b2/py_basic_commands/fscripts/fprint_array.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/create_json.py` & `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/create_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/json_editor.py` & `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/json_editor.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/read_json.py` & `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/read_json.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 from traceback  import format_exc
 from typing import Any
 
 fprint = Fprint()
 
 
 class ReadJson(Base):
+    """Read data from a JSON file"""
     def __init__(self, do_print:bool=True) -> None:
+        """Initialize the class
+
+        Parameters
+        ----------
+        do_print : bool, optional
+            Whether to get feedback printed to terminal or not. Default is True.
+        """
         super().__init__(do_print)
 
 
     def __call__(self, file_path:str, **kwargs) -> Any:
         """Read data from a JSON file.
         
         Parameters
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/json_scripts/write_json.py` & `py_basic_commands-0.2.25b2/py_basic_commands/json_scripts/write_json.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/other/basic_commands.py` & `py_basic_commands-0.2.25b2/py_basic_commands/other/basic_commands.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/other/choose_from_list.py` & `py_basic_commands-0.2.25b2/py_basic_commands/other/choose_from_list.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/other/function_timer.py` & `py_basic_commands-0.2.25b2/py_basic_commands/other/function_timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands/other/timer.py` & `py_basic_commands-0.2.25b2/py_basic_commands/other/timer.py`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands.egg-info/PKG-INFO` & `py_basic_commands-0.2.25b2/py_basic_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-basic-commands
-Version: 0.2.25b1
+Version: 0.2.25b2
 Summary: Basic tools for Python
 Home-page: https://github.com/RasseTheBoy/Py_Basic_Commands
 Author: Rasmus Ohert
 Author-email: Rasmus Ohert <rassemichael@gmail.com>
 Project-URL: GitHub, https://github.com/RasseTheBoy/Py_Basic_Commands
 Keywords: python,tool,help
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py_basic_commands-0.2.25b1/py_basic_commands.egg-info/SOURCES.txt` & `py_basic_commands-0.2.25b2/py_basic_commands.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_basic_commands-0.2.25b1/pyproject.toml` & `py_basic_commands-0.2.25b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py_basic_commands"
-version = "0.2.25-beta.01"
+version = "0.2.25-beta.2"
 authors = [
   { name="Rasmus Ohert", email="rassemichael@gmail.com" },
 ]
 description = "Basic tools for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_basic_commands-0.2.25b1/setup.cfg` & `py_basic_commands-0.2.25b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py_basic_commands
-version = 0.2.25-beta.01
+version = 0.2.25-beta.2
 author = Rasmus Ohert
 author_email = rassemichael@gmail.com
 description = Basic tools for Python
 long_description = A package that has some basic tools for your basic Python needs
 url = https://github.com/RasseTheBoy/Py_Basic_Commands
 keywords = python, tool, help
 classifiers =
```

