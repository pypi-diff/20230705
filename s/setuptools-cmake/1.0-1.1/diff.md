# Comparing `tmp/setuptools-cmake-1.0.tar.gz` & `tmp/setuptools-cmake-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-cmake-1.0.tar", last modified: Sun Oct 31 18:38:07 2021, max compression
+gzip compressed data, was "setuptools-cmake-1.1.tar", last modified: Wed Jul  5 19:11:25 2023, max compression
```

## Comparing `setuptools-cmake-1.0.tar` & `setuptools-cmake-1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 18:38:07.154868 setuptools-cmake-1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-10-31 18:38:07.154868 setuptools-cmake-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-10-31 18:37:57.000000 setuptools-cmake-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-31 18:38:07.154868 setuptools-cmake-1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      643 2021-10-31 18:37:57.000000 setuptools-cmake-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 18:38:07.154868 setuptools-cmake-1.0/setuptools_cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2021-10-31 18:37:57.000000 setuptools-cmake-1.0/setuptools_cmake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-10-31 18:37:57.000000 setuptools-cmake-1.0/setuptools_cmake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-31 18:38:07.154868 setuptools-cmake-1.0/setuptools_cmake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-10-31 18:38:06.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-10-31 18:38:07.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-31 18:38:06.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-10-31 18:38:06.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-10-31 18:38:06.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-31 18:38:06.000000 setuptools-cmake-1.0/setuptools_cmake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:11:25.111176 setuptools-cmake-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 19:11:25.107176 setuptools-cmake-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-05 19:11:16.000000 setuptools-cmake-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:11:25.111176 setuptools-cmake-1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-07-05 19:11:16.000000 setuptools-cmake-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:11:25.107176 setuptools-cmake-1.1/setuptools_cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-05 19:11:16.000000 setuptools-cmake-1.1/setuptools_cmake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 19:11:16.000000 setuptools-cmake-1.1/setuptools_cmake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:11:25.107176 setuptools-cmake-1.1/setuptools_cmake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 19:11:25.000000 setuptools-cmake-1.1/setuptools_cmake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 19:11:25.000000 setuptools-cmake-1.1/setuptools_cmake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:11:25.000000 setuptools-cmake-1.1/setuptools_cmake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 19:11:25.000000 setuptools-cmake-1.1/setuptools_cmake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 19:11:25.000000 setuptools-cmake-1.1/setuptools_cmake.egg-info/top_level.txt
```

### Comparing `setuptools-cmake-1.0/PKG-INFO` & `setuptools-cmake-1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: setuptools-cmake
-Version: 1.0
+Version: 1.1
 Summary: A setuptools intrgration for CMake built extension modules
-Home-page: UNKNOWN
 Author: TheClockTwister
-License: UNKNOWN
-Platform: UNKNOWN
 
 # Cmake meets setuptools
 
 
 ## Try the example
 
 The example module `foo` contains the methods `add` and `inverse`.
@@ -29,9 +26,7 @@
 ### Test the example module
 ```bash
 python3 -c "import foo; print(foo.inverse(0.5))"
 ```
 
 This should compile the static library `deadbeef`,
 compile the `foo.bar` submodule and print `2.0` upon execution.
-
-
```

### Comparing `setuptools-cmake-1.0/README.md` & `setuptools-cmake-1.1/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-1.0/setup.py` & `setuptools-cmake-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name='setuptools-cmake',
-    version='1.0',
+    version='1.1',
     author='TheClockTwister',
     description='A setuptools intrgration for CMake built extension modules',
     long_description=long_description,
     packages=find_packages(),
     package_data={
         '': ['CMakeLists.txt'
              ],
```

### Comparing `setuptools-cmake-1.0/setuptools_cmake/CMakeLists.txt` & `setuptools-cmake-1.1/setuptools_cmake/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     endif()
 
     # Define the binding source file
     set(sources ${relpath}/${modname}.${type})
 
     # Invoke pybind11 and set where the library should go, and what it is called
     pybind11_add_module(${target_name} ${sources})
+
+    # This creates a pre-processor definition, so that if the module is renamed,
+    # one does not have to manually edit the PyBind11 CREATE_MODULE call in the code
+    target_compile_definitions(${target_name} PRIVATE PYTHON_MODULE_NAME=${modname})
     
     set(outdir ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/${relpath})
 
     message(info " " ${module} " " ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/${relpath})
     message(info " " ${module} " " ${outdir})
 
     # target_include_directories(${target_name} PUBLIC lib/pybind11/include)
```

### Comparing `setuptools-cmake-1.0/setuptools_cmake/__init__.py` & `setuptools-cmake-1.1/setuptools_cmake/__init__.py`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-1.0/setuptools_cmake.egg-info/PKG-INFO` & `setuptools-cmake-1.1/setuptools_cmake.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: setuptools-cmake
-Version: 1.0
+Version: 1.1
 Summary: A setuptools intrgration for CMake built extension modules
-Home-page: UNKNOWN
 Author: TheClockTwister
-License: UNKNOWN
-Platform: UNKNOWN
 
 # Cmake meets setuptools
 
 
 ## Try the example
 
 The example module `foo` contains the methods `add` and `inverse`.
@@ -29,9 +26,7 @@
 ### Test the example module
 ```bash
 python3 -c "import foo; print(foo.inverse(0.5))"
 ```
 
 This should compile the static library `deadbeef`,
 compile the `foo.bar` submodule and print `2.0` upon execution.
-
-
```

