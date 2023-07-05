# Comparing `tmp/cmake-init-0.36.1.tar.gz` & `tmp/cmake-init-0.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-init-0.36.1.tar", last modified: Sun May 21 14:03:42 2023, max compression
+gzip compressed data, was "cmake-init-0.37.0.tar", last modified: Wed Jul  5 01:08:34 2023, max compression
```

## Comparing `cmake-init-0.36.1.tar` & `cmake-init-0.37.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:03:42.775147 cmake-init-0.36.1/
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-05-21 14:03:42.771147 cmake-init-0.36.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:03:42.771147 cmake-init-0.36.1/cmake_init.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:03:42.771147 cmake-init-0.36.1/cmake_init_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init_lib/cmake_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-21 14:03:42.000000 cmake-init-0.36.1/cmake_init_lib/template.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:03:42.775147 cmake-init-0.36.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-21 14:03:30.000000 cmake-init-0.36.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-05 01:08:34.928245 cmake-init-0.37.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/cmake_init.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:08:34.928245 cmake-init-0.37.0/cmake_init_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/cmake_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 01:08:34.000000 cmake-init-0.37.0/cmake_init_lib/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:08:34.928245 cmake-init-0.37.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-05 01:08:24.000000 cmake-init-0.37.0/setup.py
```

### Comparing `cmake-init-0.36.1/PKG-INFO` & `cmake-init-0.37.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.36.1
+Version: 0.37.0
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.36.1/cmake_init.egg-info/PKG-INFO` & `cmake-init-0.37.0/cmake_init.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.36.1
+Version: 0.37.0
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.36.1/cmake_init_lib/cmake_init.py` & `cmake-init-0.37.0/cmake_init_lib/cmake_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 import platform
 import re
 import subprocess
 import sys
 import zipfile
 
-__version__ = "0.36.1"
+__version__ = "0.37.0"
 
 is_windows = os.name == "nt"
 
 compile_template = None
 
 
 class Language:
@@ -174,14 +174,15 @@
         "include_source": False,
         "has_source": True,
         "cpus": os.cpu_count(),
         "pm_name": "",
         "catch3": False,
         "cpp_std": "",
         "msvc_cpp_std": "",
+        "c99": False,
     }
     package_manager = ask(
         "Package manager to use ([N]one/[c]onan/[v]cpkg)",
         cli_args.package_manager or "n",
         mapper=lambda v: v[0:1].lower(),
         predicate=lambda v: v in ["n", "c", "v"],
         header="""\
@@ -216,14 +217,16 @@
     if d["conan"]:
         if d["c"]:
             d["cpp_std"] = "11"
             d["msvc_cpp_std"] = "14"
         else:
             d["cpp_std"] = d["std"]
             d["msvc_cpp_std"] = d["std"] if d["std"] != "11" else "14"
+    if d["c"] and d["std"] != "90":
+        d["c99"] = True
     return d
 
 
 def mkdir(path):
     os.makedirs(path, exist_ok=True)
 
 
@@ -249,14 +252,16 @@
         return not d["exe"]
     if name == "windows-set-path.cmake":
         return not d["pm"]
     if name == "header_impl.c":
         return d["c_header"] and d["pm"]
     if name == "clang-14.profile":
         return d["conan"]
+    if name == "env.ps1" or name == "env.bat":
+        return d["lib"] and not d["pm"]
     return True
 
 
 def should_install_dir(at, d):
     if at.endswith("/example/"):
         if d["c"]:
             return d["c_examples"] if "/c/" in at else False
```

### Comparing `cmake-init-0.36.1/cmake_init_lib/template.py` & `cmake-init-0.37.0/cmake_init_lib/template.py`

 * *Files identical despite different names*

### Comparing `cmake-init-0.36.1/setup.py` & `cmake-init-0.37.0/setup.py`

 * *Files identical despite different names*

