# Comparing `tmp/meow_base-1.0.2.tar.gz` & `tmp/meow_base-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow_base-1.0.2.tar", last modified: Wed Jul  5 13:42:41 2023, max compression
+gzip compressed data, was "meow_base-1.0.3.tar", last modified: Wed Jul  5 13:51:47 2023, max compression
```

## Comparing `meow_base-1.0.2.tar` & `meow_base-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,50 @@
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:42:41.280182 meow_base-1.0.2/
--rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:42:41.280182 meow_base-1.0.2/PKG-INFO
--rw-rw-r--   0 patch     (1000) patch     (1000)     1993 2023-05-16 13:20:34.000000 meow_base-1.0.2/README.md
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:42:41.276182 meow_base-1.0.2/meow_base/
--rw-rw-r--   0 patch     (1000) patch     (1000)      180 2023-07-05 13:41:23.000000 meow_base-1.0.2/meow_base/__init__.py
--rw-r--r--   0 patch     (1000) patch     (1000)      168 2023-07-05 13:42:09.000000 meow_base-1.0.2/meow_base/version.py
-drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:42:41.280182 meow_base-1.0.2/meow_base.egg-info/
--rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:42:41.000000 meow_base-1.0.2/meow_base.egg-info/PKG-INFO
--rw-rw-r--   0 patch     (1000) patch     (1000)      235 2023-07-05 13:42:41.000000 meow_base-1.0.2/meow_base.egg-info/SOURCES.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)        1 2023-07-05 13:42:41.000000 meow_base-1.0.2/meow_base.egg-info/dependency_links.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       35 2023-07-05 13:42:41.000000 meow_base-1.0.2/meow_base.egg-info/requires.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       10 2023-07-05 13:42:41.000000 meow_base-1.0.2/meow_base.egg-info/top_level.txt
--rw-rw-r--   0 patch     (1000) patch     (1000)       79 2023-07-05 13:42:41.280182 meow_base-1.0.2/setup.cfg
--rw-r--r--   0 patch     (1000) patch     (1000)     1223 2023-07-05 13:34:51.000000 meow_base-1.0.2/setup.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.109995 meow_base-1.0.3/
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:51:47.109995 meow_base-1.0.3/PKG-INFO
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1993 2023-05-16 13:20:34.000000 meow_base-1.0.3/README.md
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.101995 meow_base-1.0.3/meow_base/
+-rw-rw-r--   0 patch     (1000) patch     (1000)      180 2023-07-05 13:41:23.000000 meow_base-1.0.3/meow_base/__init__.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.101995 meow_base-1.0.3/meow_base/conductors/
+-rw-rw-r--   0 patch     (1000) patch     (1000)      110 2023-03-30 10:40:02.000000 meow_base-1.0.3/meow_base/conductors/__init__.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1842 2023-07-05 12:48:42.000000 meow_base-1.0.3/meow_base/conductors/local_bash_conductor.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2032 2023-07-05 12:48:33.000000 meow_base-1.0.3/meow_base/conductors/local_python_conductor.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.105995 meow_base-1.0.3/meow_base/core/
+-rw-rw-r--   0 patch     (1000) patch     (1000)        0 2023-07-05 13:41:19.000000 meow_base-1.0.3/meow_base/core/__init__.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    13401 2023-07-05 13:15:45.000000 meow_base-1.0.3/meow_base/core/base_conductor.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    11109 2023-07-05 12:49:50.000000 meow_base-1.0.3/meow_base/core/base_handler.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    15592 2023-07-05 12:50:05.000000 meow_base-1.0.3/meow_base/core/base_monitor.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     7288 2023-07-05 12:50:17.000000 meow_base-1.0.3/meow_base/core/base_pattern.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2603 2023-07-05 12:50:39.000000 meow_base-1.0.3/meow_base/core/base_recipe.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1647 2023-07-05 12:50:59.000000 meow_base-1.0.3/meow_base/core/meow.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1629 2023-07-05 12:51:22.000000 meow_base-1.0.3/meow_base/core/rule.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    18381 2023-07-05 12:51:35.000000 meow_base-1.0.3/meow_base/core/runner.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     4250 2023-05-17 11:09:22.000000 meow_base-1.0.3/meow_base/core/vars.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.105995 meow_base-1.0.3/meow_base/functionality/
+-rw-rw-r--   0 patch     (1000) patch     (1000)        0 2023-03-08 14:25:44.000000 meow_base-1.0.3/meow_base/functionality/__init__.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1386 2023-07-05 12:52:00.000000 meow_base-1.0.3/meow_base/functionality/debug.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     5242 2023-07-05 12:52:14.000000 meow_base-1.0.3/meow_base/functionality/file_io.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1916 2023-07-05 12:52:33.000000 meow_base-1.0.3/meow_base/functionality/hashing.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     7706 2023-07-05 12:53:19.000000 meow_base-1.0.3/meow_base/functionality/meow.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1113 2023-07-05 12:53:27.000000 meow_base-1.0.3/meow_base/functionality/naming.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1001 2023-07-05 12:53:33.000000 meow_base-1.0.3/meow_base/functionality/notifications.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     5764 2023-07-05 12:53:38.000000 meow_base-1.0.3/meow_base/functionality/parameterisation.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1537 2023-07-05 12:53:49.000000 meow_base-1.0.3/meow_base/functionality/process_io.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     5493 2023-07-05 12:53:56.000000 meow_base-1.0.3/meow_base/functionality/requirements.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    15018 2023-07-05 12:54:03.000000 meow_base-1.0.3/meow_base/functionality/validation.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.105995 meow_base-1.0.3/meow_base/patterns/
+-rw-rw-r--   0 patch     (1000) patch     (1000)      130 2023-06-29 13:32:31.000000 meow_base-1.0.3/meow_base/patterns/__init__.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    20028 2023-07-05 12:54:47.000000 meow_base-1.0.3/meow_base/patterns/file_event_pattern.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)    15147 2023-07-05 12:55:35.000000 meow_base-1.0.3/meow_base/patterns/socket_event_pattern.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.109995 meow_base-1.0.3/meow_base/recipes/
+-rw-rw-r--   0 patch     (1000) patch     (1000)      213 2023-03-30 09:37:39.000000 meow_base-1.0.3/meow_base/recipes/__init__.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     4848 2023-07-05 12:55:58.000000 meow_base-1.0.3/meow_base/recipes/bash_recipe.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     5659 2023-07-05 12:56:14.000000 meow_base-1.0.3/meow_base/recipes/jupyter_notebook_recipe.py
+-rw-rw-r--   0 patch     (1000) patch     (1000)     4503 2023-07-05 12:56:31.000000 meow_base-1.0.3/meow_base/recipes/python_recipe.py
+-rw-r--r--   0 patch     (1000) patch     (1000)      168 2023-07-05 13:49:38.000000 meow_base-1.0.3/meow_base/version.py
+drwxrwxr-x   0 patch     (1000) patch     (1000)        0 2023-07-05 13:51:47.101995 meow_base-1.0.3/meow_base.egg-info/
+-rw-rw-r--   0 patch     (1000) patch     (1000)     2435 2023-07-05 13:51:47.000000 meow_base-1.0.3/meow_base.egg-info/PKG-INFO
+-rw-rw-r--   0 patch     (1000) patch     (1000)     1301 2023-07-05 13:51:47.000000 meow_base-1.0.3/meow_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)        1 2023-07-05 13:51:47.000000 meow_base-1.0.3/meow_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       35 2023-07-05 13:51:47.000000 meow_base-1.0.3/meow_base.egg-info/requires.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       10 2023-07-05 13:51:47.000000 meow_base-1.0.3/meow_base.egg-info/top_level.txt
+-rw-rw-r--   0 patch     (1000) patch     (1000)       79 2023-07-05 13:51:47.109995 meow_base-1.0.3/setup.cfg
+-rw-r--r--   0 patch     (1000) patch     (1000)     1390 2023-07-05 13:51:43.000000 meow_base-1.0.3/setup.py
```

### Comparing `meow_base-1.0.2/PKG-INFO` & `meow_base-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow_base
-Version: 1.0.2
+Version: 1.0.3
 Summary: A base framework for MEOW based implementations of workflows
 Home-page: https://github.com/PatchOfScotland/meow_base
 Author: David Marchant
 Author-email: d.marchant@ed-alumni.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meow_base-1.0.2/README.md` & `meow_base-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `meow_base-1.0.2/meow_base.egg-info/PKG-INFO` & `meow_base-1.0.3/meow_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-base
-Version: 1.0.2
+Version: 1.0.3
 Summary: A base framework for MEOW based implementations of workflows
 Home-page: https://github.com/PatchOfScotland/meow_base
 Author: David Marchant
 Author-email: d.marchant@ed-alumni.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meow_base-1.0.2/setup.py` & `meow_base-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,22 @@
     name=module_data['__name__'],
     version=module_data['__version__'],
     author='David Marchant',
     author_email='d.marchant@ed-alumni.net',
     description='A base framework for MEOW based implementations of workflows',
     long_description=long_description,
     url='https://github.com/PatchOfScotland/meow_base',
-    packages=['meow_base'],
+    packages=[
+        "meow_base",
+        "meow_base.conductors",
+        "meow_base.core",
+        "meow_base.functionality",
+        "meow_base.patterns",
+        "meow_base.recipes",
+    ],
     install_requires=[
         "papermill",
         "nbformat",
         "pyyaml",
         "watchdog"
     ],
     license='MIT',
```

