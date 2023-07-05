# Comparing `tmp/graph-jsp-env-0.2.0.tar.gz` & `tmp/graph-jsp-env-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-jsp-env-0.2.0.tar", last modified: Mon Jan 16 14:17:18 2023, max compression
+gzip compressed data, was "graph-jsp-env-0.2.1.tar", last modified: Wed Jul  5 14:17:31 2023, max compression
```

## Comparing `graph-jsp-env-0.2.0.tar` & `graph-jsp-env-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-01-16 14:17:18.864316 graph-jsp-env-0.2.0/
--rw-r--r--   0 qwerty     (501) staff       (20)     1072 2022-04-21 09:38:44.000000 graph-jsp-env-0.2.0/LICENSE
--rw-r--r--   0 qwerty     (501) staff       (20)       50 2022-12-07 18:44:16.000000 graph-jsp-env-0.2.0/MANIFEST.in
--rw-r--r--   0 qwerty     (501) staff       (20)    11034 2023-01-16 14:17:18.864389 graph-jsp-env-0.2.0/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)     9205 2022-12-14 09:08:30.000000 graph-jsp-env-0.2.0/README.md
--rw-r--r--   0 qwerty     (501) staff       (20)     2028 2023-01-16 14:16:55.000000 graph-jsp-env-0.2.0/pyproject.toml
--rw-r--r--   0 qwerty     (501) staff       (20)      598 2023-01-16 14:17:18.864848 graph-jsp-env-0.2.0/setup.cfg
--rw-r--r--   0 qwerty     (501) staff       (20)       69 2022-12-07 19:01:51.000000 graph-jsp-env-0.2.0/setup.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-01-16 14:17:18.862101 graph-jsp-env-0.2.0/src/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-01-16 14:17:18.863282 graph-jsp-env-0.2.0/src/graph_jsp_env/
--rw-r--r--   0 qwerty     (501) staff       (20)        0 2022-12-07 20:04:28.000000 graph-jsp-env-0.2.0/src/graph_jsp_env/__init__.py
--rw-r--r--   0 qwerty     (501) staff       (20)    46252 2023-01-16 13:54:09.000000 graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_jsp_env.py
--rw-r--r--   0 qwerty     (501) staff       (20)    20971 2022-12-08 10:42:07.000000 graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py
--rw-r--r--   0 qwerty     (501) staff       (20)      592 2022-12-08 13:18:55.000000 graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_logger.py
--rw-r--r--   0 qwerty     (501) staff       (20)     6535 2022-12-08 09:00:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env/wzl_ima_banner.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-01-16 14:17:18.864222 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/
--rw-r--r--   0 qwerty     (501) staff       (20)    11034 2023-01-16 14:17:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)      520 2023-01-16 14:17:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/SOURCES.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2023-01-16 14:17:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/dependency_links.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2022-12-07 20:26:06.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/not-zip-safe
--rw-r--r--   0 qwerty     (501) staff       (20)      232 2023-01-16 14:17:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/requires.txt
--rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-01-16 14:17:18.000000 graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.002413 graph-jsp-env-0.2.1/
+-rw-r--r--   0 qwerty     (501) staff       (20)     1072 2022-04-21 09:38:44.000000 graph-jsp-env-0.2.1/LICENSE
+-rw-r--r--   0 qwerty     (501) staff       (20)       50 2022-12-07 18:44:16.000000 graph-jsp-env-0.2.1/MANIFEST.in
+-rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-07-05 14:17:31.002492 graph-jsp-env-0.2.1/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)     9205 2022-12-14 09:08:30.000000 graph-jsp-env-0.2.1/README.md
+-rw-r--r--   0 qwerty     (501) staff       (20)     2107 2023-07-05 14:15:52.000000 graph-jsp-env-0.2.1/pyproject.toml
+-rw-r--r--   0 qwerty     (501) staff       (20)      598 2023-07-05 14:17:31.002816 graph-jsp-env-0.2.1/setup.cfg
+-rw-r--r--   0 qwerty     (501) staff       (20)       69 2022-12-07 19:01:51.000000 graph-jsp-env-0.2.1/setup.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:30.999926 graph-jsp-env-0.2.1/src/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.001160 graph-jsp-env-0.2.1/src/graph_jsp_env/
+-rw-r--r--   0 qwerty     (501) staff       (20)        0 2022-12-07 20:04:28.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/__init__.py
+-rw-r--r--   0 qwerty     (501) staff       (20)    46294 2023-07-05 14:08:54.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_env.py
+-rw-r--r--   0 qwerty     (501) staff       (20)    20971 2022-12-08 10:42:07.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      592 2022-12-08 13:18:55.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_logger.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     6535 2022-12-08 09:00:18.000000 graph-jsp-env-0.2.1/src/graph_jsp_env/wzl_ima_banner.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.001779 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/
+-rw-r--r--   0 qwerty     (501) staff       (20)    11113 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)      606 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/SOURCES.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/dependency_links.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2022-12-07 20:26:06.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/not-zip-safe
+-rw-r--r--   0 qwerty     (501) staff       (20)      232 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/requires.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-07-05 14:17:30.000000 graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2023-07-05 14:17:31.002089 graph-jsp-env-0.2.1/tests/
+-rw-r--r--   0 qwerty     (501) staff       (20)      210 2022-12-08 09:05:55.000000 graph-jsp-env-0.2.1/tests/test_banner.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     3001 2022-12-14 16:45:39.000000 graph-jsp-env-0.2.1/tests/test_disjunctive_graph_jsp_env.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1357 2022-12-08 12:32:13.000000 graph-jsp-env-0.2.1/tests/test_visualizer.py
```

### Comparing `graph-jsp-env-0.2.0/LICENSE` & `graph-jsp-env-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/PKG-INFO` & `graph-jsp-env-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: graph-jsp-env
-Version: 0.2.0
-Summary: todo
+Version: 0.2.1
+Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2022 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.0 Summary: todo Author:
-Alexander Nasuta Author-email: Alexander Nasuta
+Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.1 Summary: A flexible
+enviorment for job shop scheduling using the disjunctive graph apporach.
+Author: Alexander Nasuta Author-email: Alexander Nasuta
 nasuta@ima.rwth-aachen.de> License: MIT License Copyright (c) 2022 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
```

### Comparing `graph-jsp-env-0.2.0/README.md` & `graph-jsp-env-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/pyproject.toml` & `graph-jsp-env-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "graph-jsp-env"
-version = "0.2.0"
-description = "todo"
+version = "0.2.1"
+description = "A flexible enviorment for job shop scheduling using the disjunctive graph apporach."
 readme = "README.md"
 authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@ima.rwth-aachen.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -71,15 +71,15 @@
 # version_pattern = "YYYY.BUILD[-TAG]"
 # commit_message = "bump version {old_version} -> {new_version}"
 # commit = true
 # tag = true
 # push = true
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `graph-jsp-env-0.2.0/setup.cfg` & `graph-jsp-env-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_jsp_env.py` & `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -965,15 +965,16 @@
 
                 mask[task_id - 1] = True
 
             if True not in mask:
                 if self.verbose >= 1:
                     log.warning("no action options remaining")
                 if not self.env_transform == 'mask':
-                    raise RuntimeError("something went wrong")  # todo: remove error?
+                    log.warning("no action options remaining")
+                    # raise RuntimeError("something went wrong")
             return mask
         elif action_mode == 'job':
             task_mask = self.valid_action_mask(action_mode='task')
             masks_per_job = np.array_split(task_mask, self.n_jobs)
             return [True in job_mask for job_mask in masks_per_job]
         else:
             raise ValueError(f"only 'task' and 'job' are valid arguments for 'action_mode'. {action_mode} is not.")
```

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py` & `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_jsp_visualizer.py`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env/disjunctive_graph_logger.py` & `graph-jsp-env-0.2.1/src/graph_jsp_env/disjunctive_graph_logger.py`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env/wzl_ima_banner.py` & `graph-jsp-env-0.2.1/src/graph_jsp_env/wzl_ima_banner.py`

 * *Files identical despite different names*

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/PKG-INFO` & `graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: graph-jsp-env
-Version: 0.2.0
-Summary: todo
+Version: 0.2.1
+Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@ima.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2022 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.0 Summary: todo Author:
-Alexander Nasuta Author-email: Alexander Nasuta
+Metadata-Version: 2.1 Name: graph-jsp-env Version: 0.2.1 Summary: A flexible
+enviorment for job shop scheduling using the disjunctive graph apporach.
+Author: Alexander Nasuta Author-email: Alexander Nasuta
 nasuta@ima.rwth-aachen.de> License: MIT License Copyright (c) 2022 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
```

### Comparing `graph-jsp-env-0.2.0/src/graph_jsp_env.egg-info/SOURCES.txt` & `graph-jsp-env-0.2.1/src/graph_jsp_env.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,8 +10,11 @@
 src/graph_jsp_env/disjunctive_graph_logger.py
 src/graph_jsp_env/wzl_ima_banner.py
 src/graph_jsp_env.egg-info/PKG-INFO
 src/graph_jsp_env.egg-info/SOURCES.txt
 src/graph_jsp_env.egg-info/dependency_links.txt
 src/graph_jsp_env.egg-info/not-zip-safe
 src/graph_jsp_env.egg-info/requires.txt
-src/graph_jsp_env.egg-info/top_level.txt
+src/graph_jsp_env.egg-info/top_level.txt
+tests/test_banner.py
+tests/test_disjunctive_graph_jsp_env.py
+tests/test_visualizer.py
```

