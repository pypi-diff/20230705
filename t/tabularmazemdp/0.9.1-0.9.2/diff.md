# Comparing `tmp/tabularmazemdp-0.9.1.tar.gz` & `tmp/tabularmazemdp-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabularmazemdp-0.9.1.tar", last modified: Wed Jul  5 08:57:30 2023, max compression
+gzip compressed data, was "tabularmazemdp-0.9.2.tar", last modified: Wed Jul  5 17:36:00 2023, max compression
```

## Comparing `tabularmazemdp-0.9.1.tar` & `tabularmazemdp-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.github/workflows/python-publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/tabularmazemdp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/chrono.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10527 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/maze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/maze_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/mdp.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/simple_action_space.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/src/tabularmazemdp/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.275554 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 08:57:30.000000 tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:30.279554 tabularmazemdp-0.9.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 08:57:16.000000 tabularmazemdp-0.9.1/tests/test_mdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.462528 tabularmazemdp-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4213 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.462528 tabularmazemdp-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/src/tabularmazemdp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/chrono.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10698 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/maze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16186 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/maze_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4481 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/simple_action_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3268 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/src/tabularmazemdp/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 17:36:00.000000 tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:36:00.466528 tabularmazemdp-0.9.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-07-05 17:35:50.000000 tabularmazemdp-0.9.2/tests/test_mdp.py
```

### Comparing `tabularmazemdp-0.9.1/.github/workflows/python-publish.yml` & `tabularmazemdp-0.9.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/.gitignore` & `tabularmazemdp-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/LICENSE` & `tabularmazemdp-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/Makefile` & `tabularmazemdp-0.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/PKG-INFO` & `tabularmazemdp-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.1
+Version: 0.9.2
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.1/README.md` & `tabularmazemdp-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/pyproject.toml` & `tabularmazemdp-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/setup.cfg` & `tabularmazemdp-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/chrono.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/chrono.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/maze.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/maze.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,17 +228,21 @@
         # self.mdp = MyMdp(self.nb_states, self.action_space, start_distribution, transition_matrix, reward_matrix,
         #                plotter, proba_action=0.5, gamma=gamma, terminal_states=terminal_states, timeout=timeout)
 
     # --------------------------------- Reward Matrix ---------------------------------
     def simple_reward(self, transition_matrix: np.array):
         reward_matrix = np.zeros((self.nb_states, self.nb_actions))
 
+        # for final_state in self.last_states:
+        #     for from_state, action in zip(*np.nonzero(transition_matrix[:, :, final_state])):
+        #         reward_matrix[from_state, action] = 1.0
         for final_state in self.last_states:
-            for from_state, action in zip(*np.nonzero(transition_matrix[:, :, final_state])):
-                reward_matrix[from_state, action] = 1.0
+            for action in range(self.nb_actions):
+                reward_matrix[final_state, action] = 1.0
+            
         return reward_matrix
 
     # --------------------------------- Reward Matrix ---------------------------------
     def reward_hit_walls(self, transition_matrix: np.array):
         # Get the reward for reaching a final state
         reward_matrix = self.simple_reward(transition_matrix)
```

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/maze_plotter.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/maze_plotter.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/mdp.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/mdp.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/simple_action_space.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/simple_action_space.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp/toolbox.py` & `tabularmazemdp-0.9.2/src/tabularmazemdp/toolbox.py`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/PKG-INFO` & `tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabularmazemdp
-Version: 0.9.1
+Version: 0.9.2
 Summary: An simple maze to test dynamic programming and tabular reinforcement learning algorithms
 Author-email: Olivier Sigaud <Olivier.Sigaud@isir.upmc.fr>, Mathis Koroglu <mathis.koroglu@isir.upmc.fr>
 Project-URL: homepage, https://github.com/arlaz/TabularMazeMDP
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TabularMazeMDP:
```

### Comparing `tabularmazemdp-0.9.1/src/tabularmazemdp.egg-info/SOURCES.txt` & `tabularmazemdp-0.9.2/src/tabularmazemdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabularmazemdp-0.9.1/tests/test_mdp.py` & `tabularmazemdp-0.9.2/tests/test_mdp.py`

 * *Files identical despite different names*

