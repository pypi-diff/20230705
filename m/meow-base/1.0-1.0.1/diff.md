# Comparing `tmp/meow_base-1.0.tar.gz` & `tmp/meow_base-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow_base-1.0.tar", last modified: Wed Jul  5 13:23:39 2023, max compression
+gzip compressed data, was "meow_base-1.0.1.tar", last modified: Wed Jul  5 13:36:07 2023, max compression
```

## Comparing `meow_base-1.0.tar` & `meow_base-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:23:39.467355 meow_base-1.0/
--rw-rw-r--   0 patch     (1000) patch     (1000)     2433 2023-07-05 13:23:39.467355 meow_base-1.0/PKG-INFO
--rw-rw-r--   0 patch     (1000) patch     (1000)     1993 2023-05-16 13:20:34.000000 meow_base-1.0/README.md
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:23:39.467355 meow_base-1.0/meow_base/
--rw-rw-r--   0 patch     (1000) patch     (1000)       56 2023-07-05 13:14:31.000000 meow_base-1.0/meow_base/__init__.py
--rw-r--r--   0 patch     (1000) patch     (1000)      165 2023-07-05 13:14:09.000000 meow_base-1.0/meow_base/version.py
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:23:39.467355 meow_base-1.0/meow_base.egg-info/
--rw-rw-r--   0 patch     (1000) patch     (1000)     2433 2023-07-05 13:23:39.000000 meow_base-1.0/meow_base.egg-info/PKG-INFO
--rw-rw-r--   0 patch     (1000) patch     (1000)      235 2023-07-05 13:23:39.000000 meow_base-1.0/meow_base.egg-info/SOURCES.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)        1 2023-07-05 13:23:39.000000 meow_base-1.0/meow_base.egg-info/dependency_links.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       35 2023-07-05 13:23:39.000000 meow_base-1.0/meow_base.egg-info/requires.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       10 2023-07-05 13:23:39.000000 meow_base-1.0/meow_base.egg-info/top_level.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       79 2023-07-05 13:23:39.467355 meow_base-1.0/setup.cfg
--rw-r--r--   0 patch     (1000) patch     (1000)     1175 2023-07-05 13:23:15.000000 meow_base-1.0/setup.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:36:07.782539 meow_base-1.0.1/
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:36:07.782539 meow_base-1.0.1/PKG-INFO
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1993 2023-05-16 13:20:34.000000 meow_base-1.0.1/README.md
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:36:07.778539 meow_base-1.0.1/meow_base/
+-rw-rw-r--   0 patch     (1000) patch     (1000)       56 2023-07-05 13:14:31.000000 meow_base-1.0.1/meow_base/__init__.py
+-rw-r--r--   0 patch     (1000) patch     (1000)      168 2023-07-05 13:35:59.000000 meow_base-1.0.1/meow_base/version.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:36:07.782539 meow_base-1.0.1/meow_base.egg-info/
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:36:07.000000 meow_base-1.0.1/meow_base.egg-info/PKG-INFO
+-rw-rw-r--   0 patch     (1000) patch     (1000)      235 2023-07-05 13:36:07.000000 meow_base-1.0.1/meow_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)        1 2023-07-05 13:36:07.000000 meow_base-1.0.1/meow_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       35 2023-07-05 13:36:07.000000 meow_base-1.0.1/meow_base.egg-info/requires.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       10 2023-07-05 13:36:07.000000 meow_base-1.0.1/meow_base.egg-info/top_level.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       79 2023-07-05 13:36:07.782539 meow_base-1.0.1/setup.cfg
+-rw-r--r--   0 patch     (1000) patch     (1000)     1223 2023-07-05 13:34:51.000000 meow_base-1.0.1/setup.py
```

### Comparing `meow_base-1.0/PKG-INFO` & `meow_base-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow_base
-Version: 1.0
+Version: 1.0.1
 Summary: A base framework for MEOW based implementations of workflows
 Home-page: https://github.com/PatchOfScotland/meow_base
 Author: David Marchant
 Author-email: d.marchant@ed-alumni.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meow_base-1.0/README.md` & `meow_base-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `meow_base-1.0/meow_base.egg-info/PKG-INFO` & `meow_base-1.0.1/meow_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-base
-Version: 1.0
+Version: 1.0.1
 Summary: A base framework for MEOW based implementations of workflows
 Home-page: https://github.com/PatchOfScotland/meow_base
 Author: David Marchant
 Author-email: d.marchant@ed-alumni.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meow_base-1.0/setup.py` & `meow_base-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     version=module_data['__version__'],
     author='David Marchant',
     author_email='d.marchant@ed-alumni.net',
     description='A base framework for MEOW based implementations of workflows',
     long_description=long_description,
     url='https://github.com/PatchOfScotland/meow_base',
     packages=['meow_base'],
-    install_requires=read_requirements("requirements.txt"),
+    install_requires=[
+        "papermill",
+        "nbformat",
+        "pyyaml",
+        "watchdog"
+    ],
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Operating System :: OS Independent'
     ]
 )
```

