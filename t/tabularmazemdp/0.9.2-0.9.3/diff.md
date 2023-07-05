# Comparing `tmp/tabularmazemdp-0.9.2.tar.gz` & `tmp/tabularmazemdp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularmazemdp-0.9.2.tar", last modified: Wed Jul  5 17:36:00 2023, max compression
+gzip compressed data, was "tabularmazemdp-0.9.3.tar", last modified: Wed Jul  5 18:00:56 2023, max compression
```

## Comparing `tabularmazemdp-0.9.2.tar` & `tabularmazemdp-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.462528 tabularmazemdp-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.462528 tabularmazemdp-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/src/tabularmazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10698 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.797530 tabularmazemdp-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.801530 tabularmazemdp-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.797530 tabularmazemdp-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.801530 tabularmazemdp-0.9.3/src/tabularmazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10755 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/src/tabularmazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 18:00:56.000000 tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:56.805530 tabularmazemdp-0.9.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 18:00:46.000000 tabularmazemdp-0.9.3/tests/test_mdp.py
```

### Comparing `tabularmazemdp-0.9.2/.github/workflows/python-publish.yml` & `tabularmazemdp-0.9.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/.gitignore` & `tabularmazemdp-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/LICENSE` & `tabularmazemdp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/Makefile` & `tabularmazemdp-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/PKG-INFO` & `tabularmazemdp-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.2
-Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
+Version: 0.9.3
+Summary: A simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.2/README.md` & `tabularmazemdp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/pyproject.toml` & `tabularmazemdp-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tabularmazemdp"
-description = "An simple maze to test dynamic programming and tabular reinforcement learning algorithms"
+description = "A simple maze to test dynamic programming and tabular reinforcement learning algorithms"
 authors = [
     {name = "Olivier Sigaud", email = "Olivier.Sigaud@isir.upmc.fr"},
     {name = "Mathis Koroglu", email = "mathis.koroglu@isir.upmc.fr"}
 ]
 dependencies = [
     "numpy", 
     "matplotlib"
```

### Comparing `tabularmazemdp-0.9.2/setup.cfg` & `tabularmazemdp-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/chrono.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/maze.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/maze.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     stop = False
 
     while not stop:
         v_old = v.copy()
 
         for x in range(mdp.nb_states):  # for each state x
             # Compute the value of state x for each action u of the MDP action space
-            if x not in mdp.terminal_states:
+            if x in mdp.terminal_states:
+                v[x] = np.max(mdp.r[x, :])
+            else:
                 v_temp = []
                 for u in range(mdp.nb_actions):
                     # Process sum of the values of the neighbouring states
                     summ = 0
                     for y in range(mdp.nb_states):
                         summ = summ + mdp.P[x, u, y] * v_old[y]
                     v_temp.append(mdp.r[x, u] + summ)
```

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/maze_plotter.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/mdp.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/simple_action_space.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp/toolbox.py` & `tabularmazemdp-0.9.3/src/tabularmazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/PKG-INFO` & `tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.2
-Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
+Version: 0.9.3
+Summary: A simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/SOURCES.txt` & `tabularmazemdp-0.9.3/src/tabularmazemdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.2/tests/test_mdp.py` & `tabularmazemdp-0.9.3/tests/test_mdp.py`

 * *Files identical despite different names*

