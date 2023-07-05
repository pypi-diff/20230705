# Comparing `tmp/tabularmazemdp-0.9.3.tar.gz` & `tmp/tabularmazemdp-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularmazemdp-0.9.3.tar", last modified: Wed Jul  5 18:00:56 2023, max compression
+gzip compressed data, was "tabularmazemdp-0.9.4.tar", last modified: Wed Jul  5 19:20:38 2023, max compression
```

## Comparing `tabularmazemdp-0.9.3.tar` & `tabularmazemdp-0.9.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.797530 tabularmazemdp-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.801530 tabularmazemdp-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.797530 tabularmazemdp-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.801530 tabularmazemdp-0.9.3/src/tabularmazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10755 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.871954 tabularmazemdp-0.9.4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.867954 tabularmazemdp-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.867954 tabularmazemdp-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 19:20:38.871954 tabularmazemdp-0.9.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 19:20:38.871954 tabularmazemdp-0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.867954 tabularmazemdp-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.867954 tabularmazemdp-0.9.4/src/tabularmazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/src/tabularmazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.871954 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 19:20:38.000000 tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:38.871954 tabularmazemdp-0.9.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 19:20:28.000000 tabularmazemdp-0.9.4/tests/test_mdp.py
```

### Comparing `tabularmazemdp-0.9.3/.github/workflows/python-publish.yml` & `tabularmazemdp-0.9.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/.gitignore` & `tabularmazemdp-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/LICENSE` & `tabularmazemdp-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/Makefile` & `tabularmazemdp-0.9.4/Makefile`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/PKG-INFO` & `tabularmazemdp-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.3
+Version: 0.9.4
 Summary: A simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.3/README.md` & `tabularmazemdp-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/pyproject.toml` & `tabularmazemdp-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/setup.cfg` & `tabularmazemdp-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/chrono.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/maze.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/maze.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 v[x] = np.max(v_temp)
 
         # Test if convergence has been reached
         if (np.linalg.norm(v - v_old)) < 0.01:
             stop = True
 
     # We should reach terminal states from any starting point
-    reachable = mdp.nb_states - np.count_nonzero(v) == len(mdp.terminal_states)
+    reachable = (mdp.nb_states - np.count_nonzero(v) == 0)
     return reachable
 
 
 def build_maze(width, height, walls, hit=False):
     ts = height * width - 1 - len(walls)
     maze = Maze(
         width, height, hit, walls=walls, last_states=[ts]
```

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/maze_plotter.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/mdp.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/simple_action_space.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp/toolbox.py` & `tabularmazemdp-0.9.4/src/tabularmazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/PKG-INFO` & `tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.3
+Version: 0.9.4
 Summary: A simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/SOURCES.txt` & `tabularmazemdp-0.9.4/src/tabularmazemdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.3/tests/test_mdp.py` & `tabularmazemdp-0.9.4/tests/test_mdp.py`

 * *Files identical despite different names*

