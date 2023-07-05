# Comparing `tmp/wraplab-0.0.1.tar.gz` & `tmp/wraplab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraplab-0.0.1.tar", last modified: Tue Jul  4 14:09:52 2023, max compression
+gzip compressed data, was "wraplab-0.0.2.tar", last modified: Tue Jul  4 15:22:19 2023, max compression
```

## Comparing `wraplab-0.0.1.tar` & `wraplab-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 14:09:52.232777 wraplab-0.0.1/
--rw-rw-rw-   0        0        0      270 2023-07-04 14:09:52.224790 wraplab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-04 14:09:52.232777 wraplab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-04 14:08:29.000000 wraplab-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 14:09:52.184778 wraplab-0.0.1/src/
--rw-rw-rw-   0        0        0      308 2023-07-04 14:02:33.000000 wraplab-0.0.1/src/wrappers.cpp
-drwxrwxrwx   0        0        0        0 2023-07-04 14:09:52.224790 wraplab-0.0.1/wraplab.egg-info/
--rw-rw-rw-   0        0        0      270 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 14:09:51.000000 wraplab-0.0.1/wraplab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 15:22:19.737033 wraplab-0.0.2/
+-rw-rw-rw-   0        0        0      270 2023-07-04 15:22:19.737033 wraplab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-04 15:22:19.745032 wraplab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-07-04 15:19:00.000000 wraplab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 15:22:19.691910 wraplab-0.0.2/wraplab/
+-rw-rw-rw-   0        0        0      182 2023-07-04 15:21:34.000000 wraplab-0.0.2/wraplab/__init__.py
+-rw-rw-rw-   0        0        0      307 2023-07-04 15:19:13.000000 wraplab-0.0.2/wraplab/wrappers.cpp
+drwxrwxrwx   0        0        0        0 2023-07-04 15:22:19.737033 wraplab-0.0.2/wraplab.egg-info/
+-rw-rw-rw-   0        0        0      270 2023-07-04 15:22:18.000000 wraplab-0.0.2/wraplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-04 15:22:19.000000 wraplab-0.0.2/wraplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 15:22:18.000000 wraplab-0.0.2/wraplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 14:09:51.000000 wraplab-0.0.2/wraplab.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-07-04 15:22:18.000000 wraplab-0.0.2/wraplab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-04 15:22:18.000000 wraplab-0.0.2/wraplab.egg-info/top_level.txt
```

### Comparing `wraplab-0.0.1/setup.py` & `wraplab-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/python_example/pull/53)
 
 ext_modules = [
-    Pybind11Extension("wraplab",
-        ["src/wrappers.cpp"],
+    Pybind11Extension("engine",
+        ["wraplab/wrappers.cpp"],
         ),
 ]
 
 setup(
     name="wraplab",
     version=__version__,
     author="Marco Salvalaggio",
     author_email="mar.salvalaggio@gmail.com",
     url="https://github.com/marcosalvalaggio-bip/cpp-study",
     description="A test project using pybind11",
     long_description="",
+    packages = ['wraplab'],
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
-    # Currently, build_ext only provides an optional "highest supported C++
-    # level" feature, but in the future it may provide more features.
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.7",
+    install_requires=[
+          'pybind11',
+      ]
 )
```

