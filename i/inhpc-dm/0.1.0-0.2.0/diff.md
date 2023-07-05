# Comparing `tmp/inhpc_dm-0.1.0.tar.gz` & `tmp/inhpc_dm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inhpc_dm-0.1.0.tar", last modified: Tue Jan 10 08:03:35 2023, max compression
+gzip compressed data, was "inhpc_dm-0.2.0.tar", last modified: Wed Jul  5 17:19:06 2023, max compression
```

## Comparing `inhpc_dm-0.1.0.tar` & `inhpc_dm-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.031417 inhpc_dm-0.1.0/inhpc_dm/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/inhpc_dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/inhpc_dm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/inhpc_dm/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/inhpc_dm/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/inhpc_dm/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/static/679.fc85b4bc28b059f5d22c.js
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/static/747.642c1c89d20ae0c1637a.js
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/static/remoteEntry.df1990100a93e48e6813.js
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-10 08:03:33.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/inhpc_dm/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/inhpc_dm/uftp_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/inhpc_dm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 08:01:54.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-10 08:03:34.000000 inhpc_dm-0.1.0/inhpc_dm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.031417 inhpc_dm-0.1.0/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/jupyter-config/server-config/inhpc_dm.json
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/src/dm_dialogs.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/src/dm_handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/src/dm_widget.ts
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/src/mod_browser.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 08:03:35.035417 inhpc_dm-0.1.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-10 08:01:01.000000 inhpc_dm-0.1.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/inhpc_dm/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/inhpc_dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/inhpc_dm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/inhpc_dm/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/inhpc_dm/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.700755 inhpc_dm-0.2.0/inhpc_dm/labextension/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/inhpc_dm/labextension/schemas/inhpc_dm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 17:19:05.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/schemas/inhpc_dm/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-05 17:19:05.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/schemas/inhpc_dm/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/inhpc_dm/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/static/153.a409a4ff407ce9b90f51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/static/747.642c1c89d20ae0c1637a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/static/remoteEntry.bea4b8ba39d2dfd35dd4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 17:19:05.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/inhpc_dm/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/inhpc_dm/uftp_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/inhpc_dm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:17:51.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 17:19:06.000000 inhpc_dm-0.2.0/inhpc_dm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.700755 inhpc_dm-0.2.0/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/jupyter-config/server-config/inhpc_dm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/dm_buttons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/dm_dialogs.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/dm_handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/dm_icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/dm_widget.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/mod_browser.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/src/svg.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/style/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:19:06.704755 inhpc_dm-0.2.0/style/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/style/icons/left_arr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/style/icons/right_arr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-05 17:17:06.000000 inhpc_dm-0.2.0/tsconfig.json
```

### Comparing `inhpc_dm-0.1.0/LICENSE` & `inhpc_dm-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020-2022 
+Copyright (c) 2020-2023
   High Performance Computing Center Stuttgart
   Forschungszentrum Jülich GmbH
   Leibniz Supercomputing Centre
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `inhpc_dm-0.1.0/PKG-INFO` & `inhpc_dm-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inhpc_dm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Data Management for InHPC-DE
 Home-page: https://github.com/BerndSchuller/inhpc_dm
 Author: Jochen Buchholz
 Author-email: buchholz@hlrs.de
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # inhpc_dm
 
 JupyterLab extension for InHPC-DE data management
```

### Comparing `inhpc_dm-0.1.0/README.md` & `inhpc_dm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/inhpc_dm/__init__.py` & `inhpc_dm-0.2.0/inhpc_dm/__init__.py`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/inhpc_dm/handlers.py` & `inhpc_dm-0.2.0/inhpc_dm/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,28 +212,51 @@
         if len(target)==0:
             target = "."
         mount_info = self.read_mount_info()
         id_1, target_mount = self.resolve_mount_point(target, mount_info)
         id_2, source_mount = self.resolve_mount_point(sources[0], mount_info)
         if id_1==None and id_2==None:
             raise ValueError("Neither source nor target are remote")
-        if id_1!=None and id_2!=None:
-            raise ValueError("Cannot have both remote source and remote target")
-        
         cmd = uftp_handler.prepare_data_move_operation(sources, target, mount_info)
         self.log.info("Running: %s" % cmd)
         task = tasks.Task(cmd)
         task.launch()
         self.application.dm_task_holder.add(task)
         result_data = { "status": "OK" }
         self.finish(json.dumps(result_data))
 
+class InfoHandler(AbstractDMHandler):
+    """
+    Show information about a directory
+    """
+
+    @tornado.web.authenticated
+    def get(self):
+        """
+        Get info about a file / directory
+
+        input: URL query parameters
+         "file": file path
+
+        """
+        requested_file = self.get_argument("file")
+        mount_info = self.read_mount_info()
+        id_1, target_mount = self.resolve_mount_point(requested_file, mount_info)
+        result_data = { "status": "OK" }
+        if id_1==None:
+            result_data["protocol"] = "local"
+        else:
+            for key in ["protocol", "endpoint", "remote_directory"]:
+                result_data[key] = target_mount[key]
+        self.finish(json.dumps(result_data))
+
 
 def setup_handlers(web_app, url_path):
     host_pattern = ".*$"
     base_url = web_app.settings["base_url"]
     handlers = [(url_path_join(base_url, url_path, "mount"), MountHandler),
                 (url_path_join(base_url, url_path, "unmount"), UnmountHandler),
                 (url_path_join(base_url, url_path, "tasks"), TaskHandler),
+                (url_path_join(base_url, url_path, "info"), InfoHandler),
                 ]
     web_app.dm_task_holder = tasks.TaskHolder()
     web_app.add_handlers(host_pattern, handlers)
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm/labextension/package.json` & `inhpc_dm-0.2.0/inhpc_dm/labextension/schemas/inhpc_dm/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9416666666666668%*

 * *Differences: {"'contributors'": "{insert: [(1, OrderedDict([('name', 'Myriam Czekala')]))]}",*

 * * "'files'": "{insert: [(2, 'schema/*.json')]}",*

 * * "'jupyterlab'": "{'schemaDir': 'schema', delete: ['_build']}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -6,14 +6,17 @@
     "bugs": {
         "url": "https://github.com/BerndSchuller/inhpc_dm/issues"
     },
     "contributors": [
         {
             "email": "b.schuller@fz-juelich.de",
             "name": "Bernd Schuller"
+        },
+        {
+            "name": "Myriam Czekala"
         }
     ],
     "dependencies": {
         "@jupyterlab/application": "^3.1.0",
         "@jupyterlab/apputils": "^3.1.0",
         "@jupyterlab/docmanager": "^3.1.0",
         "@jupyterlab/filebrowser": "^3.1.0",
@@ -31,25 +34,22 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/*.json"
     ],
     "homepage": "https://github.com/BerndSchuller/inhpc_dm",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.df1990100a93e48e6813.js",
-            "style": "./style"
-        },
         "extension": true,
-        "outputDir": "inhpc_dm/labextension"
+        "outputDir": "inhpc_dm/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -80,9 +80,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm/labextension/static/679.fc85b4bc28b059f5d22c.js` & `inhpc_dm-0.2.0/inhpc_dm/labextension/static/153.a409a4ff407ce9b90f51.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,94 +1,87 @@
 "use strict";
 (self.webpackChunkinhpc_dm = self.webpackChunkinhpc_dm || []).push([
-    [679], {
-        679: (t, e, i) => {
+    [153], {
+        153: (t, e, i) => {
             i.r(e), i.d(e, {
-                default: () => W
+                default: () => v
             });
-            var n = i(714),
-                o = i(740),
-                s = i(773),
-                a = i(0),
-                l = i(305),
-                r = i(544),
+            var n = i(638),
+                o = i(303),
+                s = i(299),
+                a = i(931),
+                l = i(20),
+                r = i(139),
                 d = i(918),
-                c = i(992),
-                h = i(813),
-                _ = i(15);
-            class p extends h.FileBrowser {
+                c = i(832),
+                h = i(122);
+            class _ extends h.FileBrowser {
                 constructor(t, e) {
                     super(t), this.title.label = e
                 }
                 getListing() {
                     return this.listing
                 }
                 getSelectedDirectory() {
                     var t = this.listing.model.path,
                         e = this.listing.selectedItems().next();
                     return e && "directory" == e.type && (t = e.path), t
                 }
                 getCurrentPath() {
                     return this.listing.model.path
                 }
-                async copyFileFrom(t) {
-                    console.log("File is: " + t);
-                    var e = this.getCurrentPath();
-                    let i;
-                    console.log("I'm here: " + this.getCurrentPath()), await this.listing.model.cd("/"), i = _.PathExt.dirname(t), await this.listing.model.cd(i), console.log("I'm here: " + this.getCurrentPath()), this.listing.clearSelectedItems();
-                    var n = _.PathExt.basename(t);
-                    this.selectItemByName(n).catch((() => {
-                        console.log("File " + _.PathExt.basename(t) + " on path " + t + " not found!")
-                    })), console.log(n + " is selected "), this.copy(), console.log("copied "), console.log(" preparing for cd to " + e), await this.listing.model.cd("/"), console.log("I'm here: " + this.getCurrentPath()), await this.listing.model.cd(e), console.log("I'm here: " + this.getCurrentPath()), this.paste()
-                }
             }
-            async function u(t = "", e = {}) {
-                const i = l.ServerConnection.makeSettings(),
-                    n = _.URLExt.join(i.baseUrl, "inhpc_dm", t);
+            var p = i(745),
+                u = i(344);
+            async function m(t = "", e = {}) {
+                const i = r.ServerConnection.makeSettings(),
+                    n = u.URLExt.join(i.baseUrl, "inhpc_dm", t);
                 let o;
                 try {
-                    o = await l.ServerConnection.makeRequest(n, e, i)
+                    o = await r.ServerConnection.makeRequest(n, e, i)
                 } catch (t) {
-                    if (t instanceof Error) throw new l.ServerConnection.NetworkError(t); {
+                    if (t instanceof Error) throw new r.ServerConnection.NetworkError(t); {
                         let t;
-                        throw t = new TypeError("Serverside was not available, something went wrong"), console.log("Serverside was not available, something went wrong"), new l.ServerConnection.NetworkError(t)
+                        throw t = new TypeError("Serverside was not available, something went wrong"), console.log("Serverside was not available, something went wrong"), new r.ServerConnection.NetworkError(t)
                     }
                 }
                 if (!o.ok) {
                     let t;
                     t = o.statusText;
                     try {
                         t += JSON.stringify(await o.json())
                     } catch (t) {}
-                    throw new l.ServerConnection.ResponseError(o, t)
+                    throw new r.ServerConnection.ResponseError(o, t)
                 }
                 return await o.json()
             }
             class g extends c.Widget {
-                constructor(t = [], e = "") {
-                    super(), this.addClass("jp-Input-Dialog"), this._list = document.createElement("select"), t.forEach(((t, e) => {
+                constructor(t = [], e = "", i) {
+                    super(), this.addClass("jp-Input-Dialog"), this._list = document.createElement("select");
+                    let n = "";
+                    null != i && (n = i), t.forEach(((t, e) => {
                         const i = document.createElement("option");
                         i.value = t, i.textContent = t, this._list.appendChild(i)
                     }));
-                    const i = document.createElement("datalist");
-                    i.id = "input-dialog-items", i.appendChild(this._list), this._input_endpoint = document.createElement("input"), this._input_endpoint.classList.add("jp-mod-styled"), this._input_endpoint.id = "jp-dialog-input-id_ep", this._input_endpoint.type = "list", this._input_endpoint.value = "", this._input_endpoint.setAttribute("list", i.id), this.node.appendChild(i);
-                    const n = document.createElement("label");
-                    n.textContent = "UFTP endpoint", n.htmlFor = this._input_endpoint.id, this.node.appendChild(n), this.node.appendChild(this._input_endpoint), this._input_remoteDir = document.createElement("input"), this._input_remoteDir.classList.add("jp-mod-styled"), this._input_remoteDir.id = "jp-dialog-input-id_rd";
-                    const o = document.createElement("label");
-                    o.textContent = "Remote directory", o.htmlFor = this._input_remoteDir.id, this.node.appendChild(o), this.node.appendChild(this._input_remoteDir), this._input_localDir = document.createElement("input"), this._input_localDir.classList.add("jp-mod-styled"), this._input_localDir.id = "jp-dialog-input-id_ld", this._input_localDir.value = e;
+                    const o = document.createElement("datalist");
+                    o.id = "input-dialog-items", o.appendChild(this._list), this._input_endpoint = document.createElement("input"), this._input_endpoint.classList.add("jp-mod-styled"), this._input_endpoint.id = "jp-dialog-input-id_ep", this._input_endpoint.type = "list", this._input_endpoint.value = n, this._input_endpoint.setAttribute("list", o.id), this.node.appendChild(o);
                     const s = document.createElement("label");
-                    s.textContent = "Mount point", s.htmlFor = this._input_localDir.id, this.node.appendChild(s), this.node.appendChild(this._input_localDir), this._input_username = document.createElement("input"), this._input_username.classList.add("jp-mod-styled"), this._input_username.id = "jp-dialog-input-id_un";
+                    s.textContent = "UFTP endpoint", s.htmlFor = this._input_endpoint.id, this.node.appendChild(s), this.node.appendChild(this._input_endpoint), this._input_remoteDir = document.createElement("input"), this._input_remoteDir.classList.add("jp-mod-styled"), this._input_remoteDir.id = "jp-dialog-input-id_rd";
                     const a = document.createElement("label");
-                    a.textContent = "Username", a.htmlFor = this._input_username.id, this.node.appendChild(a), this.node.appendChild(this._input_username), this._input_password = document.createElement("input"), this._input_password.classList.add("jp-mod-styled"), this._input_password.type = "password", this._input_password.id = "jp-dialog-input-id_pw";
+                    a.textContent = "Remote directory", a.htmlFor = this._input_remoteDir.id, this.node.appendChild(a), this.node.appendChild(this._input_remoteDir), this._input_localDir = document.createElement("input"), this._input_localDir.classList.add("jp-mod-styled"), this._input_localDir.id = "jp-dialog-input-id_ld", this._input_localDir.value = e;
                     const l = document.createElement("label");
-                    l.textContent = "Password", l.htmlFor = this._input_password.id, this.node.appendChild(l), this.node.appendChild(this._input_password), this._input_token = document.createElement("input"), this._input_token.classList.add("jp-mod-styled"), this._input_token.id = "jp-dialog-input-id_tok";
+                    l.textContent = "Mount point", l.htmlFor = this._input_localDir.id, this.node.appendChild(l), this.node.appendChild(this._input_localDir), this._input_username = document.createElement("input"), this._input_username.classList.add("jp-mod-styled"), this._input_username.id = "jp-dialog-input-id_un";
                     const r = document.createElement("label");
-                    r.textContent = "OAuth token", r.htmlFor = this._input_token.id, this.node.appendChild(r), this.node.appendChild(this._input_token), this._input_identity = document.createElement("input"), this._input_identity.classList.add("jp-mod-styled"), this._input_identity.id = "jp-dialog-input-id_identity";
+                    r.textContent = "Username", r.htmlFor = this._input_username.id, this.node.appendChild(r), this.node.appendChild(this._input_username), this._input_password = document.createElement("input"), this._input_password.classList.add("jp-mod-styled"), this._input_password.type = "password", this._input_password.id = "jp-dialog-input-id_pw";
                     const d = document.createElement("label");
-                    d.textContent = "Path to private key", d.htmlFor = this._input_identity.id, this.node.appendChild(d), this.node.appendChild(this._input_identity)
+                    d.textContent = "Password", d.htmlFor = this._input_password.id, this.node.appendChild(d), this.node.appendChild(this._input_password), this._input_token = document.createElement("input"), this._input_token.classList.add("jp-mod-styled"), this._input_token.id = "jp-dialog-input-id_tok";
+                    const c = document.createElement("label");
+                    c.textContent = "OAuth token", c.htmlFor = this._input_token.id, this.node.appendChild(c), this.node.appendChild(this._input_token), this._input_identity = document.createElement("input"), this._input_identity.classList.add("jp-mod-styled"), this._input_identity.id = "jp-dialog-input-id_identity";
+                    const h = document.createElement("label");
+                    h.textContent = "Path to private key", h.htmlFor = this._input_identity.id, this.node.appendChild(h), this.node.appendChild(this._input_identity)
                 }
                 getValue() {
                     return {
                         endpoint: this._input_endpoint.value,
                         remote_directory: this._input_remoteDir.value,
                         mount_point: this._input_localDir.value,
                         credentials: {
@@ -96,198 +89,93 @@
                             password: this._input_password.value,
                             token: this._input_token.value,
                             identity: this._input_identity.value
                         }
                     }
                 }
             }
-            class m extends c.Widget {
-                static createNode() {
-                    let t = document.createElement("div"),
-                        e = document.createElement("div"),
-                        i = document.createElement("textarea");
-                    return i.placeholder = "Placeholder...", e.appendChild(i), t.appendChild(e), t
-                }
-                constructor(t) {
-                    super({
-                        node: m.createNode()
-                    }), this.setFlag(c.Widget.Flag.DisallowLayout), this.addClass("content"), this.addClass(t.toLowerCase()), this.title.label = t, this.title.closable = !0, this.title.caption = `Long description for: ${t}`
-                }
-                get textareaNode() {
-                    return this.node.getElementsByTagName("textarea")[0]
-                }
-                onActivateRequest(t) {
-                    this.isAttached && this.textareaNode.focus()
-                }
-            }
-            class f extends c.Widget {
-                constructor(t) {
-                    super(), this._settings = {
-                        uftp_endpoints: ["https://localhost:9000/rest/auth/TEST", "https://gridftp-fr1.hww.hlrs.de:9000/rest/auth/HLRS", "https://uftp.fz-juelich.de:9112/UFTP_Auth/rest/auth/JUDAC", "https://datagw03.supermuc.lrz.de:9000/rest/auth/DATAGW"]
-                    }, this.addClass("my-dmWidget"), this._actionToolbar = new o.Toolbar, this._actionToolbar.id = "actionToolbar";
-                    const e = new o.ToolbarButton({
-                        icon: r.settingsIcon,
-                        onClick: async () => {
-                            try {
-                                const t = await u("mount");
-                                console.log(t), this._logWidget.textareaNode.value = JSON.stringify(t)
-                            } catch (t) {
-                                console.error(`Error on GET /inhpc_dm/mount".\n${t}`)
-                            }
-                        },
-                        tooltip: "Get mounts information"
-                    });
-                    this._actionToolbar.addItem("mount_info", e), this._top_panel = new c.SplitPanel({
-                        orientation: "horizontal"
-                    }), this._top_panel.id = "top_panel", this._top_panel.addClass("dm_Widget-main"), this._top_panel.addWidget(this._actionToolbar);
-                    let i = new a.DocumentRegistry;
-                    const n = new l.ServiceManager;
-                    let d = new s.DocumentManager({
-                            registry: i,
-                            manager: n,
-                            opener
-                        }),
-                        _ = new h.FilterFileBrowserModel({
-                            manager: d
-                        });
-                    this._fbWidget_l = new p({
-                        id: "filebrowser-left",
-                        model: _
-                    }, "Filebrowser left");
-                    const g = new b(this._fbWidget_l, this._settings.uftp_endpoints);
-                    this._fbWidget_l.toolbar.addItem("mountBtn", g);
-                    const f = new w(this._fbWidget_l);
-                    this._fbWidget_l.toolbar.addItem("unmountBtn", f), this._infoWidget_l = new m("Info"), this._infoWidget_l.id = "infoWidget_l", this._infoWidget_l.textareaNode.value = "<n/a>", this._infoWidget_l.textareaNode.style.width = "95%", this._fbPanel_l = new c.SplitPanel({
-                        orientation: "vertical",
-                        spacing: 1
-                    }), this._fbPanel_l.id = "fb_panel_l", this._fbPanel_l.addWidget(this._fbWidget_l), this._fbPanel_l.addWidget(this._infoWidget_l), this._fbPanel_l.setRelativeSizes([85, 15]);
-                    let W = new h.FilterFileBrowserModel({
-                        manager: d
-                    });
-                    this._fbWidget_r = new p({
-                        id: "filebrowser-right",
-                        model: W
-                    }, "Filebrowser right");
-                    const C = new b(this._fbWidget_r, this._settings.uftp_endpoints);
-                    this._fbWidget_r.toolbar.addItem("mountBtn", C);
-                    const P = new w(this._fbWidget_r);
-                    this._fbWidget_r.toolbar.addItem("unmountBtn", P), this._infoWidget_r = new m("Info"), this._infoWidget_r.id = "infoWidget_r", this._infoWidget_r.textareaNode.value = "<n/a>", this._infoWidget_r.textareaNode.style.width = "95%", this._fbPanel_r = new c.SplitPanel({
-                        orientation: "vertical",
-                        spacing: 1
-                    }), this._fbPanel_r.id = "fb_panel_r", this._fbPanel_r.addWidget(this._fbWidget_r), this._fbPanel_r.addWidget(this._infoWidget_r), this._fbPanel_r.setRelativeSizes([90, 10]);
-                    const v = new y(this._fbWidget_l, this._fbWidget_r, "--\x3e", "Copy left selected to right directory directly"),
-                        x = new y(this._fbWidget_r, this._fbWidget_l, "<--", "Copy right selected to left directory directly");
-                    this._transferBoxPanel = new c.BoxPanel({
-                        direction: "top-to-bottom"
-                    }), this._transferBoxPanel.id = "transferToolbar", this._transferBoxPanel.node.style.maxWidth = "100px", this._transferBoxPanel.node.style.maxHeight = "100px", this._transferBoxPanel.node.style.top = "200px", this._transferBoxPanel.addWidget(v), this._transferBoxPanel.addWidget(x), this._fbPanel = new c.BoxPanel({
-                        direction: "left-to-right",
-                        spacing: 1
-                    }), this._fbPanel.id = "fb_panel", this._fbPanel.addClass("dm_Widget-main"), this._fbPanel.addWidget(this._fbPanel_l), this._fbPanel.addWidget(this._transferBoxPanel), this._fbPanel.addWidget(this._fbPanel_r), this._logWidget = new m("Log"), this._logWidget.id = "logWidget", this._logWidget.textareaNode.value = "Log output", this._logWidget.textareaNode.style.width = "95%", this._logWidget.textareaNode.style.height = "95%", this._mainLayout = this.layout = new c.BoxLayout, this._panel_collection = new c.SplitPanel({
-                        orientation: "vertical"
-                    }), this._panel_collection.id = "panel_collection", this._panel_collection.addWidget(this._top_panel), this._panel_collection.addWidget(this._fbPanel), this._panel_collection.addWidget(this._logWidget), this._panel_collection.setRelativeSizes([10, 80, 10]), this._mainLayout.addWidget(this._panel_collection)
-                }
-                formatBytes(t, e = 2) {
-                    if (0 === t) return "0 Bytes";
-                    const i = e < 0 ? 0 : e,
-                        n = Math.floor(Math.log(t) / Math.log(1024));
-                    return parseFloat((t / Math.pow(1024, n)).toFixed(i)) + " " + ["Bytes", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"][n]
-                }
-                print_object_details(t) {
-                    console.log("Print Object Details"), console.log(Object.getOwnPropertyNames(t).sort())
-                }
-                eventSignalHandler(t, e) {
-                    if ("DirListing" === t.constructor.name)
-                        if ("click" === e) {
-                            var i = "Selected Files Info",
-                                n = 0;
-                            (0, d.each)(this._fbWidget_l.getListing().selectedItems(), (t => {
-                                t.size && (n += t.size), t.size && (i = i + "\n" + t.path + "(" + this.formatBytes(t.size) + ")")
-                            })), i = i + "\nOverall Size: " + this.formatBytes(n), i = "Selected Files Info", n = 0, (0, d.each)(this._fbWidget_r.getListing().selectedItems(), (t => {
-                                t.size && (n += t.size), t.size && (i = i + "\n" + t.path + "(" + this.formatBytes(t.size) + ")")
-                            })), i = i + "\nOverall Size: " + this.formatBytes(n)
-                        } else console.log("Unknown in DirListing: ", e);
-                    else console.log("Unknown event sender: ", t.constructor.name)
-                }
-            }
-            class b extends o.ToolbarButton {
-                constructor(t, e) {
+            class f extends o.ToolbarButton {
+                constructor(t, e, i) {
                     super({
-                        icon: r.addIcon,
+                        icon: p.addIcon,
                         tooltip: "Mount remote filesystem via UFTP",
                         onClick: () => {
-                            this.handle_click(t, e)
+                            this.handle_click(t, e, i)
                         }
                     })
                 }
-                handle_click(t, e) {
-                    var i, n;
-                    console.log(this), (i = e, n = t.getSelectedDirectory(), function(t = {}) {
-                        return new o.Dialog(t).launch()
-                    }({
-                        body: new g(i, n),
-                        buttons: [o.Dialog.cancelButton({
-                            label: "Cancel"
-                        }), o.Dialog.okButton({
-                            label: "OK"
-                        })],
-                        focusNodeSelector: "input"
-                    })).then((async t => {
-                        var e = JSON.stringify(t.value);
-                        if ("null" != e) {
-                            console.log("mount params: " + e);
-                            try {
-                                const t = await u("mount", {
-                                    body: e,
-                                    method: "POST"
-                                });
-                                console.log(t), "OK" == t.status ? (0, o.showDialog)({
-                                    title: "OK",
-                                    body: "Mount successful",
-                                    buttons: [o.Dialog.okButton()]
-                                }) : (0, o.showErrorMessage)("Error", t.error_info)
-                            } catch (t) {
-                                console.error(`Error on POST /inhpc_dm/mount".\n${t}`), (0, o.showErrorMessage)("Error", t)
-                            }
-                        } else console.log("Mount cancelled")
-                    }))
+                handle_click(t, e, i) {
+                    console.log(this),
+                        function(t, e, i) {
+                            return function(t = {}) {
+                                return new o.Dialog(t).launch()
+                            }({
+                                body: new g(t, e, i),
+                                buttons: [o.Dialog.cancelButton({
+                                    label: "Cancel"
+                                }), o.Dialog.okButton({
+                                    label: "OK"
+                                })],
+                                focusNodeSelector: "input"
+                            })
+                        }(e, t.getSelectedDirectory(), i).then((async e => {
+                            var i = JSON.stringify(e.value);
+                            if ("null" != i) {
+                                var n = JSON.parse(i).mount_point;
+                                console.log("Mount dir: " + n), console.log("mount params: " + i);
+                                try {
+                                    const e = await m("mount", {
+                                        body: i,
+                                        method: "POST"
+                                    });
+                                    console.log(e), "OK" == e.status ? ((0, o.showDialog)({
+                                        title: "OK",
+                                        body: "Mount successful",
+                                        buttons: [o.Dialog.okButton()]
+                                    }), await t.getListing().model.cd("/"), await t.getListing().model.cd(n)) : (0, o.showErrorMessage)("Error", e.error_info)
+                                } catch (t) {
+                                    console.error(`Error on POST /inhpc_dm/mount".\n${t}`), (0, o.showErrorMessage)("Error", t)
+                                }
+                            } else console.log("Mount cancelled")
+                        }))
                 }
             }
-            class w extends o.ToolbarButton {
+            class b extends o.ToolbarButton {
                 constructor(t) {
                     super({
-                        icon: r.clearIcon,
+                        icon: p.clearIcon,
                         tooltip: "Unmount remote filesystem",
                         onClick: () => {
                             this.handle_click(t)
                         }
                     })
                 }
                 async handle_click(t) {
                     console.log(this);
                     var e = t.getSelectedDirectory(),
                         i = JSON.stringify({
                             mount_point: e
                         });
                     console.log("mount params: " + i);
                     try {
-                        const t = await u("unmount", {
+                        const t = await m("unmount", {
                             body: i,
                             method: "POST"
                         });
                         console.log(t), "OK" == t.status ? (0, o.showDialog)({
                             title: "OK",
                             body: "Unmount successful",
                             buttons: [o.Dialog.okButton()]
                         }) : (0, o.showErrorMessage)("Error", t.error_info)
                     } catch (t) {
                         console.error(`Error on POST /inhpc_dm/unmount".\n${t}`), (0, o.showErrorMessage)("Error", t)
                     }
                 }
             }
-            class y extends o.ToolbarButton {
+            class w extends o.ToolbarButton {
                 constructor(t, e, i, n) {
                     super({
                         label: i,
                         tooltip: n,
                         onClick: () => {
                             this.handle_click(t, e)
                         }
@@ -304,58 +192,163 @@
                         parameters: {
                             target: i,
                             sources: n
                         }
                     });
                     console.log("Copy command params: " + s);
                     try {
-                        const t = await u("tasks", {
+                        const t = await m("tasks", {
                             body: s,
                             method: "POST"
                         });
                         console.log(t), "OK" == t.status ? (0, o.showDialog)({
                             title: "OK",
                             body: "Task launched successfully",
                             buttons: [o.Dialog.okButton()]
                         }) : (0, o.showErrorMessage)("Error", t.error_info)
                     } catch (t) {
                         console.error(`Error on POST /inhpc_dm/tasks".\n${t}`), (0, o.showErrorMessage)("Error", t)
                     }
                 }
             }
-            const W = {
-                id: "jupyterlab_inhpc",
-                autoStart: !0,
-                requires: [o.ICommandPalette, n.ILayoutRestorer],
-                activate: (t, e, i) => {
-                    ! function(t, e, i) {
-                        let n;
-                        console.log("JupyterLab extension InHPC data management activating.");
-                        const s = "inhpc:opendm";
-                        t.commands.addCommand(s, {
-                            label: "InHPC - Data Management dual browser view",
-                            execute: () => {
-                                if (!n || n.isDisposed) {
-                                    const e = new f(t);
-                                    e.id = "dmwidget_id", n = new o.MainAreaWidget({
-                                        content: e
-                                    }), n.id = "inhpc-datamanagement", n.title.label = "Data Management", n.title.closable = !0
-                                }
-                                a.has(n) || a.add(n), n.isAttached || t.shell.add(n, "main"), n.content.update(), t.shell.activateById(n.id)
-                            }
-                        }), e.addItem({
-                            command: s,
-                            category: "Tutorial"
-                        });
-                        let a = new o.WidgetTracker({
-                            namespace: "inhpc_dm"
+            class y extends c.Widget {
+                static createNode() {
+                    let t = document.createElement("div"),
+                        e = document.createElement("div"),
+                        i = document.createElement("textarea");
+                    return i.placeholder = "Placeholder...", e.appendChild(i), t.appendChild(e), t
+                }
+                constructor(t) {
+                    super({
+                        node: y.createNode()
+                    }), this.setFlag(c.Widget.Flag.DisallowLayout), this.addClass("content"), this.addClass(t.toLowerCase()), this.title.label = t, this.title.closable = !0, this.title.caption = `Long description for: ${t}`
+                }
+                get textareaNode() {
+                    return this.node.getElementsByTagName("textarea")[0]
+                }
+                onActivateRequest(t) {
+                    this.isAttached && this.textareaNode.focus()
+                }
+            }
+            class C extends c.Widget {
+                constructor(t) {
+                    super(), this._settings = {
+                        uftp_endpoints: ["https://localhost:9000/rest/auth/TEST", "https://gridftp-fr1.hww.hlrs.de:9000/rest/auth/HLRS", "https://uftp.fz-juelich.de:9112/UFTP_Auth/rest/auth/JUDAC", "https://datagw03.supermuc.lrz.de:9000/rest/auth/DATAGW"]
+                    }, this.addClass("my-dmWidget");
+                    let e = new l.DocumentRegistry;
+                    const i = new r.ServiceManager;
+                    let n = new a.DocumentManager({
+                            registry: e,
+                            manager: i,
+                            opener
+                        }),
+                        o = new h.FilterFileBrowserModel({
+                            manager: n
                         });
-                        i.restore(a, {
-                            command: s,
-                            name: () => "inhpc_dm"
-                        })
-                    }(t, e, i)
+                    this._fbWidget_l = new _({
+                        id: "filebrowser-left",
+                        model: o
+                    }, "Filebrowser left");
+                    const s = new f(this._fbWidget_l, this._settings.uftp_endpoints);
+                    this._fbWidget_l.toolbar.addItem("mountBtn", s);
+                    const d = new b(this._fbWidget_l);
+                    this._fbWidget_l.toolbar.addItem("unmountBtn", d), this._infoWidget_l = new y("Info"), this._infoWidget_l.id = "infoWidget_l", this._infoWidget_l.textareaNode.value = "<n/a>", this._infoWidget_l.textareaNode.style.width = "95%", this._fbPanel_l = new c.SplitPanel({
+                        orientation: "vertical",
+                        spacing: 1
+                    }), this._fbPanel_l.id = "fb_panel_l", this._fbPanel_l.addWidget(this._fbWidget_l), this._fbPanel_l.addWidget(this._infoWidget_l), this._fbPanel_l.setRelativeSizes([90, 10]);
+                    let p = new h.FilterFileBrowserModel({
+                        manager: n
+                    });
+                    this._fbWidget_r = new _({
+                        id: "filebrowser-right",
+                        model: p
+                    }, "Filebrowser right");
+                    const u = new f(this._fbWidget_r, this._settings.uftp_endpoints, this._defaultEndpoint);
+                    this._fbWidget_r.toolbar.addItem("mountBtn", u);
+                    const m = new b(this._fbWidget_r);
+                    this._fbWidget_r.toolbar.addItem("unmountBtn", m), this._infoWidget_r = new y("Info"), this._infoWidget_r.id = "infoWidget_r", this._infoWidget_r.textareaNode.value = "<n/a>", this._infoWidget_r.textareaNode.style.width = "95%", this._fbPanel_r = new c.SplitPanel({
+                        orientation: "vertical",
+                        spacing: 1
+                    }), this._fbPanel_r.id = "fb_panel_r", this._fbPanel_r.addWidget(this._fbWidget_r), this._fbPanel_r.addWidget(this._infoWidget_r), this._fbPanel_r.setRelativeSizes([90, 10]);
+                    const g = new w(this._fbWidget_l, this._fbWidget_r, "--\x3e", "Copy left selected to right directory directly"),
+                        C = new w(this._fbWidget_r, this._fbWidget_l, "<--", "Copy right selected to left directory directly");
+                    this._transferBoxPanel = new c.BoxPanel({
+                        direction: "top-to-bottom"
+                    }), this._transferBoxPanel.id = "transferToolbar", this._transferBoxPanel.node.style.maxWidth = "100px", this._transferBoxPanel.node.style.maxHeight = "100px", this._transferBoxPanel.node.style.top = "200px", this._transferBoxPanel.addWidget(g), this._transferBoxPanel.addWidget(C), this._fbPanel = new c.BoxPanel({
+                        direction: "left-to-right",
+                        spacing: 1
+                    }), this._fbPanel.id = "fb_panel", this._fbPanel.addClass("dm_Widget-main"), this._fbPanel.addWidget(this._fbPanel_l), this._fbPanel.addWidget(this._transferBoxPanel), this._fbPanel.addWidget(this._fbPanel_r), this._mainLayout = this.layout = new c.BoxLayout, this._panel_collection = new c.SplitPanel({
+                        orientation: "vertical"
+                    }), this._panel_collection.id = "panel_collection", this._panel_collection.addWidget(this._fbPanel), this._panel_collection.setRelativeSizes([10, 80, 10]), this._mainLayout.addWidget(this._panel_collection)
+                }
+                formatBytes(t, e = 2) {
+                    if (0 === t) return "0 Bytes";
+                    const i = e < 0 ? 0 : e,
+                        n = Math.floor(Math.log(t) / Math.log(1024));
+                    return parseFloat((t / Math.pow(1024, n)).toFixed(i)) + " " + ["Bytes", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"][n]
+                }
+                print_object_details(t) {
+                    console.log("Print Object Details"), console.log(Object.getOwnPropertyNames(t).sort())
+                }
+                eventSignalHandler(t, e) {
+                    if ("DirListing" === t.constructor.name)
+                        if ("click" === e) {
+                            var i = "Selected Files Info",
+                                n = 0;
+                            (0, d.each)(this._fbWidget_l.getListing().selectedItems(), (t => {
+                                t.size && (n += t.size), t.size && (i = i + "\n" + t.path + "(" + this.formatBytes(t.size) + ")")
+                            })), i = i + "\nOverall Size: " + this.formatBytes(n), i = "Selected Files Info", n = 0, (0, d.each)(this._fbWidget_r.getListing().selectedItems(), (t => {
+                                t.size && (n += t.size), t.size && (i = i + "\n" + t.path + "(" + this.formatBytes(t.size) + ")")
+                            })), i = i + "\nOverall Size: " + this.formatBytes(n)
+                        } else console.log("Unknown in DirListing: ", e);
+                    else console.log("Unknown event sender: ", t.constructor.name)
+                }
+                setDefaultEndpoint(t) {
+                    this._defaultEndpoint = t
                 }
             }
+            const P = {
+                    id: "@jupyterlab/inhpc-extension:plugin",
+                    autoStart: !0,
+                    requires: [o.ICommandPalette, n.ILayoutRestorer, s.ISettingRegistry],
+                    activate: (t, e, i, n) => {
+                        ! function(t, e, i, n, s) {
+                            let a;
+                            console.log("JupyterLab extension InHPC data management activating.");
+                            const l = "inhpc:opendm",
+                                r = new C(t);
+                            t.commands.addCommand(l, {
+                                label: "InHPC - Data Management dual browser view",
+                                execute: () => {
+                                    a && !a.isDisposed || (r.id = "dmwidget_id", a = new o.MainAreaWidget({
+                                        content: r
+                                    }), a.id = "inhpc-datamanagement", a.title.label = "Data Management", a.title.closable = !0), d.has(a) || d.add(a), a.isAttached || t.shell.add(a, "main"), a.content.update(), t.shell.activateById(a.id)
+                                }
+                            }), e.addItem({
+                                command: l,
+                                category: "Tutorial"
+                            });
+                            let d = new o.WidgetTracker({
+                                namespace: "inhpc_dm"
+                            });
+
+                            function c(t) {
+                                let e;
+                                e = t.get("defaultHost").composite.toString(), console.log("Settings are: " + e), r.setDefaultEndpoint(e)
+                            }
+                            i.restore(d, {
+                                command: l,
+                                name: () => "inhpc_dm"
+                            }), Promise.all([n.load(s), t.started]).then((([t]) => {
+                                console.log("entering the promis, loading the settings "), c(t), t.changed.connect((() => {
+                                    c(t)
+                                }))
+                            })).catch((t => {
+                                console.error("Problem with Settings: " + t.message)
+                            }))
+                        }(t, e, i, n, P.id)
+                    }
+                },
+                v = P
         }
     }
 ]);
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm/labextension/static/747.642c1c89d20ae0c1637a.js` & `inhpc_dm-0.2.0/inhpc_dm/labextension/static/747.642c1c89d20ae0c1637a.js`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/inhpc_dm/labextension/static/remoteEntry.df1990100a93e48e6813.js` & `inhpc_dm-0.2.0/inhpc_dm/labextension/static/remoteEntry.bea4b8ba39d2dfd35dd4.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, m, b, g, y, w, j = {
+    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v, m, g, b, y, w, j, S = {
             618: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(679).then((() => () => t(679))),
-                        "./extension": () => t.e(679).then((() => () => t(679))),
+                        "./index": () => t.e(153).then((() => () => t(153))),
+                        "./extension": () => t.e(153).then((() => () => t(153))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -21,112 +21,113 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        S = {};
+        E = {};
 
-    function E(e) {
-        var r = S[e];
+    function k(e) {
+        var r = E[e];
         if (void 0 !== r) return r.exports;
-        var t = S[e] = {
+        var t = E[e] = {
             id: e,
             exports: {}
         };
-        return j[e](t, t.exports, E), t.exports
+        return S[e](t, t.exports, k), t.exports
     }
-    E.m = j, E.c = S, E.n = e => {
+    k.m = S, k.c = E, k.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return E.d(r, {
+        return k.d(r, {
             a: r
         }), r
-    }, E.d = (e, r) => {
-        for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
+    }, k.d = (e, r) => {
+        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        679: "fc85b4bc28b059f5d22c",
+    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
+        153: "a409a4ff407ce9b90f51",
         747: "642c1c89d20ae0c1637a"
     } [e] + ".js?v=" + {
-        679: "fc85b4bc28b059f5d22c",
+        153: "a409a4ff407ce9b90f51",
         747: "642c1c89d20ae0c1637a"
-    } [e], E.g = function() {
+    } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "inhpc_dm:", E.l = (t, n, o, a) => {
+    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "inhpc_dm:", k.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
                     var d = l[s];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, E.r = e => {
+    }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        E.S = {};
+        k.S = {};
         var e = {},
             r = {};
-        E.I = (t, n) => {
+        k.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
+                k.o(k.S, t) || (k.S[t] = {});
+                var a = k.S[t],
                     i = "inhpc_dm",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => E.e(679).then((() => () => E(679))),
+                        get: () => k.e(153).then((() => () => k(153))),
                         from: i,
                         eager: !1
                     })
-                })("inhpc_dm", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("inhpc_dm", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        E.g.importScripts && (e = E.g.location + "");
-        var r = E.g.document;
+        k.g.importScripts && (e = k.g.location + "");
+        var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), E.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -192,100 +193,103 @@
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = E.S[e];
-        if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = k.S[e];
+        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), h(e[t][o])
+        return a(n, o) || c(s(e, t, o, n)), v(e[t][o])
     }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, c = (e, r, t, n) => {
-        "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), m = (v = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || c(r, e, t, n) || u(r, t))))), b = v(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), g = {}, y = {
-        0: () => m("default", "@jupyterlab/docregistry", [1, 3, 5, 2]),
-        15: () => b("default", "@jupyterlab/coreutils", [1, 5, 5, 2]),
-        305: () => b("default", "@jupyterlab/services", [1, 6, 5, 2]),
-        544: () => b("default", "@jupyterlab/ui-components", [1, 3, 5, 2]),
-        714: () => b("default", "@jupyterlab/application", [1, 3, 5, 2]),
-        740: () => b("default", "@jupyterlab/apputils", [1, 3, 5, 2]),
-        773: () => b("default", "@jupyterlab/docmanager", [1, 3, 5, 2]),
-        813: () => b("default", "@jupyterlab/filebrowser", [1, 3, 5, 2]),
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, h = (e, r, t, n) => {
+        c(p(e, r, t, n))
+    }, v = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, n, o) {
+        var a = k.I(r);
+        return a && a.then ? a.then(e.bind(e, r, k.S[r], t, n, o)) : e(r, k.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), v(f(r, t, n) || h(r, e, t, n) || u(r, t))))), b = m(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), y = {}, w = {
+        20: () => g("default", "@jupyterlab/docregistry", [1, 3, 6, 5]),
+        122: () => b("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        139: () => b("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        299: () => b("default", "@jupyterlab/settingregistry", [1, 3, 6, 5]),
+        303: () => b("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        344: () => b("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        638: () => b("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        745: () => b("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
+        832: () => b("default", "@lumino/widgets", [1, 1, 37, 2]),
         918: () => b("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        992: () => b("default", "@lumino/widgets", [1, 1, 33, 0])
-    }, w = {
-        679: [0, 15, 305, 544, 714, 740, 773, 813, 918, 992]
-    }, E.f.consumes = (e, r) => {
-        E.o(w, e) && w[e].forEach((e => {
-            if (E.o(g, e)) return r.push(g[e]);
+        931: () => b("default", "@jupyterlab/docmanager", [1, 3, 6, 5])
+    }, j = {
+        153: [20, 122, 139, 299, 303, 344, 638, 745, 832, 918, 931]
+    }, k.f.consumes = (e, r) => {
+        k.o(j, e) && j[e].forEach((e => {
+            if (k.o(y, e)) return r.push(y[e]);
             var t = r => {
-                    g[e] = 0, E.m[e] = t => {
-                        delete E.c[e], t.exports = r()
+                    y[e] = 0, k.m[e] = t => {
+                        delete k.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete g[e], E.m[e] = t => {
-                        throw delete E.c[e], r
+                    delete y[e], k.m[e] = t => {
+                        throw delete k.c[e], r
                     }
                 };
             try {
-                var o = y[e]();
-                o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
+                var o = w[e]();
+                o.then ? r.push(y[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             892: 0
         };
-        E.f.j = (r, t) => {
-            var n = E.o(e, r) ? e[r] : void 0;
+        k.f.j = (r, t) => {
+            var n = k.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = E.p + E.u(r),
+                    var a = k.p + k.u(r),
                         i = new Error;
-                    E.l(a, (t => {
-                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    k.l(a, (t => {
+                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
-                    u && u(E)
+                    for (n in i) k.o(i, n) && (k.m[n] = i[n]);
+                    u && u(k)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], k.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkinhpc_dm = self.webpackChunkinhpc_dm || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), E.nc = void 0;
-    var k = E(618);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).inhpc_dm = k
+    })(), k.nc = void 0;
+    var _ = k(618);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).inhpc_dm = _
 })();
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm/labextension/static/third-party-licenses.json` & `inhpc_dm-0.2.0/inhpc_dm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/inhpc_dm/tasks.py` & `inhpc_dm-0.2.0/inhpc_dm/tasks.py`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/inhpc_dm/uftp_handler.py` & `inhpc_dm-0.2.0/inhpc_dm/uftp_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 from base64 import b64encode
 from fuse import FUSE
 from os import environ, getenv
 from pathlib import Path, PosixPath, PurePosixPath
 from pyunicore.client import Transport
 from pyunicore.credentials import create_credential
 from pyunicore.uftp import UFTP
@@ -27,20 +28,14 @@
         _identity = None
     return create_credential(username = _user,
                              password = _password,
                              token = _token,
                              identity = _identity)
 
 
-def create_uftp_handler(remote_directory, auth_url, credentials):
-    """ creates a UFTP handler (not yet authenticated or connected) """
-    credential = _setup_credential(credentials)
-    return UFTP(Transport(credential), auth_url, remote_directory)
-
-
 def run_fusedriver(host, port, pwd, mount_point, debug=False):
     cmds = ["export PYTHONPATH=%s" % environ.get("PYTHONPATH", ""),
             "export UFTP_PASSWORD=%s" % pwd,
             "python3 -m pyunicore.uftpfuse %s:%s '%s'" % (host, port, mount_point)]
     cmd = ""
     for c in cmds:
         cmd += c + u"\n"
@@ -56,18 +51,20 @@
             # check if mount point is a parent dir for our target dir
             if mount_point == lookup[0:len(mount_point)]:
                 return m
         # nothing found
         return None
 
     
-def _create_command(host, port, pwd, method, sources, target):
+def _create_command(host, port, pwd, method, sources, target, rhost, rport, rpwd):
     cmd =  "export PYTHONPATH=%s\n" % environ.get("PYTHONPATH", "")
     cmd += "export UFTP_PASSWORD=%s\n" % pwd
-    cmd += "python3 -m inhpc_dm.uftp_handler %s:%s -X %s " %(host,port, method)
+    cmd += f"python3 -m inhpc_dm.uftp_handler {host}:{port} -X {method} "
+    if method=="RCP":
+        cmd += f"-R {rhost}:{rport}:{rpwd} "
     if len(sources)<1:
         raise ValueError("Need sources")
     cmd += "--sources "
     for source in sources:
         cmd += "'%s' " % source
     cmd += "--target '%s'" % target
     return cmd
@@ -85,55 +82,64 @@
 def _relative_path(full, base):
     return str(PosixPath(full).absolute().relative_to(PosixPath(base)))
 
 
 def prepare_data_move_operation(sources, target, mount_info):
     """ Create command to be executed for a data copy operation.
         Will resolve source/target endpoint, and determine what operation 
-        (GET or PUT) is needed.
+        (GET, PUT, RCP) is needed.
         Will authenticate with the stored credentials.
     """
     _target_mount = _resolve_mount_point(target, mount_info)
     _source_mount = _resolve_mount_point(sources[0], mount_info)
-    if _target_mount!=None:
+    _rcp_args = [None,None,None]
+    if _source_mount is None:
         _method = "PUT"
         _mount = _target_mount
         _sources = sources
-        _target = _relative_path(target, _mount["mount_point"])
-    else:
+        _target = _relative_path(target, _mount["mount_point"])+"/"
+    elif _target_mount is None:
         _method = "GET"
         _mount = _source_mount
         _target = target
         _sources = [ _relative_path(full, _mount["mount_point"]) for full in sources ]
-
+    else:
+        # remote copy - issue receive-file on target side
+        _method = "RCP"
+        _mount = _target_mount
+        _sources = [ _relative_path(full, _source_mount["mount_point"]) for full in sources ]
+        _target = _relative_path(target, _target_mount["mount_point"])+"/"
+        _rauth_url = _source_mount["endpoint"]
+        _rcredentials = _source_mount["credentials"]
+        _r_remote_dir = _source_mount["remote_directory"]
+        _rhost, _rport, _rpwd = UFTP().authenticate(_setup_credential(_rcredentials), _rauth_url, _r_remote_dir)
+        _rcp_args = [_rhost, _rport, _rpwd]
     _auth_url = _mount["endpoint"]
     _credentials = _mount["credentials"]
     _remote_dir = _mount["remote_directory"]
-    _uftp = create_uftp_handler(_remote_dir, _auth_url, _credentials)
-    _host, _port, _pwd = _uftp.authenticate()
-
-    return _create_command(_host, int(_port), _pwd, _method, _sources, _target)
+    _host, _port, _pwd = UFTP().authenticate(_setup_credential(_credentials), _auth_url, _remote_dir)
+    return _create_command(_host, int(_port), _pwd, _method, _sources, _target, *_rcp_args)
 
 def mount(mount_directory, parameters):
     """
     Authenticates to UFTPD and mounts the requested directory
     """
     auth_url = parameters['endpoint']
     remote_directory = parameters['remote_directory']
     mount_point = parameters['mount_point']
     credentials = parameters.get('credentials', {})
     try:
-        uftp = create_uftp_handler(remote_directory, auth_url, credentials)
-        (host, port, pwd) = uftp.authenticate()
+        uftp = UFTP()
+        (host, port, pwd) = uftp.authenticate(
+            _setup_credential(credentials), auth_url, remote_directory)
         uftp.open_uftp_session(host, port, pwd)
         # avoid launching FUSE driver after an error during connect
         st = uftp.stat(".")
         error_code, output = run_fusedriver(host, port, pwd, mount_point)
     except Exception as ex:
-        uftp.close()
         error_code = 1
         output = repr(ex)
     return error_code, output
 
 
 def unmount(parameters):
     """
@@ -144,26 +150,26 @@
         error_code, output = _run_command(cmd)
     except Exception as ex:
         error_code = 1
         output = repr(ex)
     return error_code, output
 
 
-if __name__ == "__main__":
+def main():
     """ 
     Main function to run download or upload from UFTPD.
     Requires the one-time password from authentication, which must have been done previously
     """
-    import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument("address", help="UFTPD server's address (host:port)")
     parser.add_argument("-P", "--password",
-        help="one-time password (if not given, it is expected in the environment UFTP_PASSWORD)",
-    )
+                        help="one-time password (if not given, it is expected in the environment UFTP_PASSWORD)")
     parser.add_argument("-X", "--operation", required=True, help="what to do, GET or PUT")
+    parser.add_argument("-R", "--remote", required=False,
+                        help="Remote copy: host:port:password for accessing source file")
     parser.add_argument(
         "-s",
         "--sources",
         nargs="+",
         help="list of source files")
     parser.add_argument(
         "-t",
@@ -174,15 +180,15 @@
     _host, _port = args.address.split(":")
     _pwd = args.password
     if _pwd is None:
         _pwd = getenv("UFTP_PASSWORD")
     if _pwd is None:
         raise TypeError("UFTP one-time password must be given via --P or as environment UFTP_PASSWORD")
     _operation = args.operation
-    if "GET"!=_operation and "PUT"!=_operation:
+    if _operation not in ["GET", "PUT", "RCP"]:
         raise TypeError("Not understood: %s" % _operation)
 
     uftp_session = UFTP()
     uftp_session.open_uftp_session(_host, int(_port), _pwd)
 
     if "GET"==_operation:
         _target = Path(args.target)
@@ -204,7 +210,18 @@
             _source = Path(source)
             if is_dir:
                 _write_to = _target / _source.name
             else:
                 _write_to = _target
             with _source.open("rb") as fp:
                 uftp_session.ftp.storbinary('STOR %s' % str(_write_to), fp)
+    elif "RCP"==_operation:
+        if len(args.sources)>1:
+            raise ValueError("Can only remote copy one file")
+        _source = Path(args.sources[0])
+        _target = args.target
+        _rhost, _rport, _rpwd =  args.remote.split(":")
+        cmd = f"RECEIVE-FILE '{_target}/{_source.name}' '{_source}' '{_rhost}:{_rport}' '{_rpwd}'"
+        uftp_session.ftp.sendcmd(cmd)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm.egg-info/PKG-INFO` & `inhpc_dm-0.2.0/inhpc_dm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inhpc-dm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Data Management for InHPC-DE
 Home-page: https://github.com/BerndSchuller/inhpc_dm
 Author: Jochen Buchholz
 Author-email: buchholz@hlrs.de
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # inhpc_dm
 
 JupyterLab extension for InHPC-DE data management
```

### Comparing `inhpc_dm-0.1.0/inhpc_dm.egg-info/SOURCES.txt` & `inhpc_dm-0.2.0/inhpc_dm.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -14,21 +14,28 @@
 inhpc_dm.egg-info/PKG-INFO
 inhpc_dm.egg-info/SOURCES.txt
 inhpc_dm.egg-info/dependency_links.txt
 inhpc_dm.egg-info/not-zip-safe
 inhpc_dm.egg-info/requires.txt
 inhpc_dm.egg-info/top_level.txt
 inhpc_dm/labextension/package.json
-inhpc_dm/labextension/static/679.fc85b4bc28b059f5d22c.js
+inhpc_dm/labextension/schemas/inhpc_dm/package.json.orig
+inhpc_dm/labextension/schemas/inhpc_dm/plugin.json
+inhpc_dm/labextension/static/153.a409a4ff407ce9b90f51.js
 inhpc_dm/labextension/static/747.642c1c89d20ae0c1637a.js
-inhpc_dm/labextension/static/remoteEntry.df1990100a93e48e6813.js
+inhpc_dm/labextension/static/remoteEntry.bea4b8ba39d2dfd35dd4.js
 inhpc_dm/labextension/static/style.js
 inhpc_dm/labextension/static/third-party-licenses.json
 jupyter-config/server-config/inhpc_dm.json
+src/dm_buttons.ts
 src/dm_dialogs.ts
 src/dm_handler.ts
+src/dm_icons.ts
 src/dm_widget.ts
 src/index.ts
 src/mod_browser.ts
+src/svg.d.ts
 style/base.css
 style/index.css
-style/index.js
+style/index.js
+style/icons/left_arr.svg
+style/icons/right_arr.svg
```

### Comparing `inhpc_dm-0.1.0/package.json` & `inhpc_dm-0.2.0/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9458333333333334%*

 * *Differences: {"'contributors'": "{insert: [(1, OrderedDict([('name', 'Myriam Czekala')]))]}",*

 * * "'files'": "{insert: [(2, 'schema/*.json')]}",*

 * * "'jupyterlab'": "{'schemaDir': 'schema'}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -6,14 +6,17 @@
     "bugs": {
         "url": "https://github.com/BerndSchuller/inhpc_dm/issues"
     },
     "contributors": [
         {
             "email": "b.schuller@fz-juelich.de",
             "name": "Bernd Schuller"
+        },
+        {
+            "name": "Myriam Czekala"
         }
     ],
     "dependencies": {
         "@jupyterlab/application": "^3.1.0",
         "@jupyterlab/apputils": "^3.1.0",
         "@jupyterlab/docmanager": "^3.1.0",
         "@jupyterlab/filebrowser": "^3.1.0",
@@ -31,20 +34,22 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/*.json"
     ],
     "homepage": "https://github.com/BerndSchuller/inhpc_dm",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "inhpc_dm/labextension"
+        "outputDir": "inhpc_dm/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -75,9 +80,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `inhpc_dm-0.1.0/setup.py` & `inhpc_dm-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     cmdclass=cmdclass,
     packages=setuptools.find_packages(),
     install_requires=[
         "jupyterlab~=3.0",
         "fusepy~=3.0.1",
-        "pyunicore>=0.10.2"
+        "pyunicore>=0.15.0"
     ],
     zip_safe=False,
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

### Comparing `inhpc_dm-0.1.0/src/dm_dialogs.ts` & `inhpc_dm-0.2.0/src/dm_dialogs.ts`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 const INPUT_DIALOG_CLASS = 'jp-Input-Dialog';
 
 /**
  * A popup dialog for choosing a system to mount via UFTP.
  */
 class MountDialog<T> extends Widget implements Dialog.IBodyWidget<T> {
 
-  constructor(availableEndpoints: string[] = [], mountDirectory: string = "") {
+  constructor(availableEndpoints: string[] = [], mountDirectory: string = "", defaultEndoint?: string) {
     super();
     this.addClass(INPUT_DIALOG_CLASS);
 
     // editable list of endpoints
     this._list = document.createElement('select');
+
     let current = '';
+    if(defaultEndoint!=undefined)
+    {
+      current = defaultEndoint;
+    }
     availableEndpoints.forEach((item, index) => {
         const option = document.createElement('option');
         option.value = item;
         option.textContent = item;
         this._list.appendChild(option);
     });
     const data = document.createElement('datalist');
@@ -146,17 +151,17 @@
 export function showDialog<T>(
   options: Partial<Dialog.IOptions<T>> = {}
 ): Promise<Dialog.IResult<T>> {
   const dialog = new Dialog(options);
   return dialog.launch();
 }
 
- export function getMountInfo(availableEndpoints: string[], mountDirectory: string): Promise<Dialog.IResult<string>> {
+ export function getMountInfo(availableEndpoints: string[], mountDirectory: string, defaultEndpoint?: string): Promise<Dialog.IResult<string>> {
     return showDialog({
-      body: new MountDialog(availableEndpoints, mountDirectory),
+      body: new MountDialog(availableEndpoints, mountDirectory, defaultEndpoint),
       buttons: [
         Dialog.cancelButton({ label: 'Cancel' }),
         Dialog.okButton({ label: 'OK' })
       ],
       focusNodeSelector: 'input'
     });
   }
```

### Comparing `inhpc_dm-0.1.0/src/dm_handler.ts` & `inhpc_dm-0.2.0/src/dm_handler.ts`

 * *Files identical despite different names*

### Comparing `inhpc_dm-0.1.0/src/index.ts` & `inhpc_dm-0.2.0/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -11,26 +11,30 @@
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import {
   ICommandPalette,
 } from '@jupyterlab/apputils';
 
+import{ ISettingRegistry } from '@jupyterlab/settingregistry';
+
 import { activate_dm } from './dm_widget';
 
 /**
  * Initialization data for the jupyterlab extensions
  */
 const extension: JupyterFrontEndPlugin<void> = {
-  id: 'jupyterlab_inhpc',
+  id: '@jupyterlab/inhpc-extension:plugin',
   autoStart: true,
-  requires: [ICommandPalette, ILayoutRestorer],
+  requires: [ICommandPalette, ILayoutRestorer, ISettingRegistry],
   activate: (
     app: JupyterFrontEnd, 
     palette: ICommandPalette, 
-    restorer: ILayoutRestorer) =>
+    restorer: ILayoutRestorer,
+    settingReg: ISettingRegistry
+) =>
   {
-    activate_dm(app, palette, restorer);
+    activate_dm(app, palette, restorer, settingReg, extension.id);
   }
 };
 
 export default extension;
```

### Comparing `inhpc_dm-0.1.0/tsconfig.json` & `inhpc_dm-0.2.0/tsconfig.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'compilerOptions'": "{'skipLibCheck': True}"}*

```diff
@@ -11,14 +11,15 @@
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
+        "skipLibCheck": true,
         "strict": true,
         "strictNullChecks": false,
         "target": "es2017",
         "types": [
             "node"
         ]
     },
```

