# Comparing `tmp/tabularmazemdp-0.0.0.tar.gz` & `tmp/tabularmazemdp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularmazemdp-0.0.0.tar", last modified: Tue Jul  4 12:04:08 2023, max compression
+gzip compressed data, was "tabularmazemdp-0.9.1.tar", last modified: Wed Jul  5 08:57:30 2023, max compression
```

## Comparing `tabularmazemdp-0.0.0.tar` & `tabularmazemdp-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 mathis     (501) staff       (20)        0 2023-07-04 12:04:08.947193 tabularmazemdp-0.0.0/
--rwxr-xr-x   0 mathis     (501) staff       (20)     1071 2023-06-01 13:50:36.000000 tabularmazemdp-0.0.0/LICENSE
--rw-r--r--   0 mathis     (501) staff       (20)       27 2023-06-01 13:50:36.000000 tabularmazemdp-0.0.0/MANIFEST.in
--rw-r--r--   0 mathis     (501) staff       (20)     4600 2023-07-04 12:04:08.947242 tabularmazemdp-0.0.0/PKG-INFO
--rwxr-xr-x   0 mathis     (501) staff       (20)     4213 2023-07-03 12:52:15.000000 tabularmazemdp-0.0.0/README.md
--rw-r--r--   0 mathis     (501) staff       (20)      677 2023-07-04 12:00:01.000000 tabularmazemdp-0.0.0/pyproject.toml
--rwxr-xr-x   0 mathis     (501) staff       (20)      712 2023-07-04 12:04:08.947490 tabularmazemdp-0.0.0/setup.cfg
--rwxr-xr-x   0 mathis     (501) staff       (20)       37 2023-06-01 13:50:36.000000 tabularmazemdp-0.0.0/setup.py
-drwxr-xr-x   0 mathis     (501) staff       (20)        0 2023-07-04 12:04:08.944660 tabularmazemdp-0.0.0/src/
-drwxr-xr-x   0 mathis     (501) staff       (20)        0 2023-07-04 12:04:08.946342 tabularmazemdp-0.0.0/src/tabularmazemdp/
--rwxr-xr-x   0 mathis     (501) staff       (20)      241 2023-07-04 12:01:09.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/__init__.py
--rwxr-xr-x   0 mathis     (501) staff       (20)      865 2023-06-01 13:50:36.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/chrono.py
--rwxr-xr-x   0 mathis     (501) staff       (20)    10509 2023-07-04 12:01:14.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/maze.py
--rwxr-xr-x   0 mathis     (501) staff       (20)    16186 2023-07-04 12:02:25.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/maze_plotter.py
--rwxr-xr-x   0 mathis     (501) staff       (20)     4481 2023-07-04 12:01:59.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/mdp.py
--rw-r--r--   0 mathis     (501) staff       (20)      764 2023-06-01 13:50:36.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/simple_action_space.py
--rwxr-xr-x   0 mathis     (501) staff       (20)     3268 2023-07-04 12:01:38.000000 tabularmazemdp-0.0.0/src/tabularmazemdp/toolbox.py
-drwxr-xr-x   0 mathis     (501) staff       (20)        0 2023-07-04 12:04:08.946962 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/
--rw-r--r--   0 mathis     (501) staff       (20)     4600 2023-07-04 12:04:08.000000 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/PKG-INFO
--rw-r--r--   0 mathis     (501) staff       (20)      510 2023-07-04 12:04:08.000000 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 mathis     (501) staff       (20)        1 2023-07-04 12:04:08.000000 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 mathis     (501) staff       (20)       17 2023-07-04 12:04:08.000000 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/requires.txt
--rw-r--r--   0 mathis     (501) staff       (20)       15 2023-07-04 12:04:08.000000 tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/top_level.txt
-drwxr-xr-x   0 mathis     (501) staff       (20)        0 2023-07-04 12:04:08.947081 tabularmazemdp-0.0.0/tests/
--rwxr-xr-x   0 mathis     (501) staff       (20)     1654 2023-06-01 14:13:12.000000 tabularmazemdp-0.0.0/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/tabularmazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10527 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/tests/test_mdp.py
```

### Comparing `tabularmazemdp-0.0.0/LICENSE` & `tabularmazemdp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/PKG-INFO` & `tabularmazemdp-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.0.0
+Version: 0.9.1
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.0.0/README.md` & `tabularmazemdp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/pyproject.toml` & `tabularmazemdp-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/setup.cfg` & `tabularmazemdp-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/chrono.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/maze.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/maze.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     # the loop below is used to check that the maze has a solution
     # if one of the values after check_navigability is null, then another maze should be produced
     while not stop:
         walls = random.sample(range(size), int(n_walls))
 
         mdp, nb_states, coord_x, coord_y = build_maze(width, height, walls, hit=hit)
         stop = check_navigability(mdp)
-    return mdp, nb_states
+    return mdp, nb_states, coord_x, coord_y
 
 
 class Maze:  # describes a maze-like environment
     def __init__(
         self,
         width,
         height,
```

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/maze_plotter.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/mdp.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/simple_action_space.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp/toolbox.py` & `tabularmazemdp-0.9.1/src/tabularmazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.0.0/src/tabularmazemdp.egg-info/PKG-INFO` & `tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.0.0
+Version: 0.9.1
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.0.0/tests/test_mdp.py` & `tabularmazemdp-0.9.1/tests/test_mdp.py`

 * *Files identical despite different names*

