# Comparing `tmp/gues-0.1.0.tar.gz` & `tmp/gues-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gues-0.1.0.tar", last modified: Thu Apr 20 07:51:14 2023, max compression
+gzip compressed data, was "gues-0.2.0.tar", last modified: Wed Jul  5 15:16:11 2023, max compression
```

## Comparing `gues-0.1.0.tar` & `gues-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-04-20 07:51:14.092612 gues-0.1.0/
--rw-r--r--   0 alex      (1000) alex      (1001)    34283 2023-04-17 12:57:32.000000 gues-0.1.0/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1001)      583 2023-04-20 07:51:14.092612 gues-0.1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      135 2023-04-17 07:44:40.000000 gues-0.1.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-04-20 07:51:14.092612 gues-0.1.0/gues/
--rw-r--r--   0 alex      (1000) alex      (1001)     3796 2023-04-17 08:58:28.000000 gues-0.1.0/gues/decomposable_score.py
--rw-r--r--   0 alex      (1000) alex      (1001)     9139 2023-04-17 08:59:28.000000 gues-0.1.0/gues/gauss_obs_l0_pen.py
--rw-r--r--   0 alex      (1000) alex      (1001)    20952 2023-04-14 11:36:54.000000 gues-0.1.0/gues/grues.py
--rw-r--r--   0 alex      (1000) alex      (1001)    15430 2023-04-20 07:35:08.000000 gues-0.1.0/gues/gues.py
--rw-r--r--   0 alex      (1000) alex      (1001)     9514 2023-04-17 13:00:32.000000 gues-0.1.0/gues/independence_testing.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-04-20 07:51:14.092612 gues-0.1.0/gues.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)      583 2023-04-20 07:51:14.000000 gues-0.1.0/gues.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      315 2023-04-20 07:51:14.000000 gues-0.1.0/gues.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2023-04-20 07:51:14.000000 gues-0.1.0/gues.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       46 2023-04-20 07:51:14.000000 gues-0.1.0/gues.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        5 2023-04-20 07:51:14.000000 gues-0.1.0/gues.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2023-04-20 07:51:14.092612 gues-0.1.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1001)      728 2023-04-17 12:57:14.000000 gues-0.1.0/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-04-20 07:51:14.092612 gues-0.1.0/tests/
--rw-r--r--   0 alex      (1000) alex      (1001)    10124 2023-04-20 07:00:17.000000 gues-0.1.0/tests/test_grues.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2383 2023-04-20 07:25:40.000000 gues-0.1.0/tests/test_gues.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-07-05 15:16:11.472571 gues-0.2.0/
+-rw-r--r--   0 alex      (1000) alex      (1001)    34283 2023-04-17 12:57:32.000000 gues-0.2.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1001)      589 2023-07-05 15:16:11.472571 gues-0.2.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      147 2023-07-04 14:43:11.000000 gues-0.2.0/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-07-05 15:16:11.472571 gues-0.2.0/gues/
+-rw-r--r--   0 alex      (1000) alex      (1001)     3796 2023-04-17 08:58:28.000000 gues-0.2.0/gues/decomposable_score.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     9139 2023-04-17 08:59:28.000000 gues-0.2.0/gues/gauss_obs_l0_pen.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    21749 2023-06-08 14:58:46.000000 gues-0.2.0/gues/grues.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    15431 2023-04-24 15:03:01.000000 gues-0.2.0/gues/gues.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     9514 2023-04-17 13:00:32.000000 gues-0.2.0/gues/independence_testing.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1865 2023-04-26 10:51:57.000000 gues-0.2.0/gues/sample.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-07-05 15:16:11.472571 gues-0.2.0/gues.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)      589 2023-07-05 15:16:11.000000 gues-0.2.0/gues.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      369 2023-07-05 15:16:11.000000 gues-0.2.0/gues.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2023-07-05 15:16:11.000000 gues-0.2.0/gues.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)      130 2023-07-05 15:16:11.000000 gues-0.2.0/gues.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        5 2023-07-05 15:16:11.000000 gues-0.2.0/gues.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)      100 2023-05-22 10:10:42.000000 gues-0.2.0/pyproject.toml
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-07-05 15:16:11.472571 gues-0.2.0/scripts/
+-rw-r--r--   0 alex      (1000) alex      (1001)    22127 2023-07-05 14:58:18.000000 gues-0.2.0/scripts/reproduce_astat
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2023-07-05 15:16:11.472571 gues-0.2.0/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1001)      966 2023-07-05 15:08:21.000000 gues-0.2.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2023-07-05 15:16:11.472571 gues-0.2.0/tests/
+-rw-r--r--   0 alex      (1000) alex      (1001)    10133 2023-05-04 17:27:05.000000 gues-0.2.0/tests/test_grues.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     2383 2023-04-20 07:25:40.000000 gues-0.2.0/tests/test_gues.py
```

### Comparing `gues-0.1.0/LICENSE.md` & `gues-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gues-0.1.0/PKG-INFO` & `gues-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: gues
-Version: 0.1.0
+Version: 0.2.0
 Summary: This package is for (hybrid and) score-based causal structure learning, using unconditional equivalence classes to reduce the search space.
 Author: Alex Markham
 Author-email: alex.markham@causal.dev
 License: GNU Affero General Public License 3 or later (AGPL 3+)
+Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dcor
-Provides-Extra: ges
-Provides-Extra: all
+Provides-Extra: reproduce_astat
 License-File: LICENSE.md
 
-GUES is a Python package for score-based causal structure learning, using unconditional equivalence classes to reduce the search space.
+GUES is a Python package for score-based and hybrid causal structure learning, using unconditional equivalence classes to reduce the search space.
```

### Comparing `gues-0.1.0/gues/decomposable_score.py` & `gues-0.2.0/gues/decomposable_score.py`

 * *Files identical despite different names*

### Comparing `gues-0.1.0/gues/gauss_obs_l0_pen.py` & `gues-0.2.0/gues/gauss_obs_l0_pen.py`

 * *Files identical despite different names*

### Comparing `gues-0.1.0/gues/grues.py` & `gues-0.2.0/gues/grues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Implement the Groebner basis-based UEC search algorithm (GrUES)."""
-import numpy as np
 import math
 import warnings
+
+import numpy as np
+from numpy.linalg import svd
+from scipy.stats import chi2, beta
+
 from .gauss_obs_l0_pen import GaussObsL0Pen
 from .independence_testing import dcov
-from scipy.stats import chi2, beta
-from scipy.special import factorial
-from numpy.linalg import lstsq, det, inv
 
 
 class InputData(object):
     r"""Feed data into GrUES to learn its UEC.
 
     Attributes
     ----------
@@ -46,23 +47,31 @@
             }
         else:
             self.p = p
         self.init_uec(init)
         self.get_max_cpdag()
         self.reduce_max_cpdag()
         self.moves = 0
-        self.visited = np.empty(max_moves, float)
+        self.bic_markov_chain = np.empty(max_moves, float)
+        self.nuc_markov_chain = np.empty(max_moves, float)
         self.old_rss = self.compute_mle_rss()
-        self.visited[0] = self.optimal_bic = self.cpdag.sum() * np.log(
+        u, s, vh = svd(self.cpdag)
+        self.bic_markov_chain[0] = self.best_bic = (s**2).sum() * np.log(
             self.num_samps
         ) + self.num_samps * np.log(self.old_rss)
-        self.markov_chain = np.empty((max_moves, self.num_feats, self.num_feats), bool)
-        self.markov_chain[0] = self.uec
+        self.nuc_markov_chain[0] = self.best_nuc = s.sum() * np.log(
+            self.num_samps
+        ) + self.num_samps * np.log(self.old_rss)
+        self.uec_markov_chain = np.empty(
+            (max_moves, self.num_feats, self.num_feats), bool
+        )
+        self.uec_markov_chain[0] = self.uec
         while self.moves < max_moves - 1:
-            self.old_bic = self.visited[self.moves]
+            self.old_bic = self.bic_markov_chain[self.moves]
+            self.old_nuc = self.nuc_markov_chain[self.moves]
             self.old_cpdag = np.copy(self.cpdag)
             self.old_dag = np.copy(self.dag_reduction)
             self.old_cc = np.copy(self.chain_comps)
 
             moves_dict = {
                 "merge": self.merge,
                 "split": self.split,
@@ -95,18 +104,21 @@
                 "out_add": "out_del",
             }
             inv_move = inv_moves[move]
 
             poss_moves, _, p = self.compute_transition_kernel(moves_dict)
             q_inv = float(self.q[inv_move] * p[poss_moves == inv_move])
 
-            likelihood_ratio, new_rss, new_bic = self.get_likelihood_ratio()
-            if new_bic / self.optimal_bic < 1:
-                self.optimal_bic = new_bic
-                self.optimal_uec = self.uec
+            likelihood_ratio, new_rss, new_bic, new_nuc = self.get_likelihood_ratio()
+            if new_bic / self.best_bic < 1:
+                self.best_bic = new_bic
+                self.bic_uec = self.uec
+            if new_nuc / self.best_nuc < 1:
+                self.best_nuc = new_nuc
+                self.nuc_uec = self.uec
 
             likelihood_and_transition_ratio = likelihood_ratio * (q_inv / q)
             if type(prior) is tuple:
                 prior_ratio = self.scaled_triangle_prior(prior)
                 likelihood_and_transition_ratio *= prior_ratio
             elif prior is not None:
                 prior_ratio = prior(self)
@@ -114,21 +126,32 @@
             h = min(1, likelihood_and_transition_ratio)
             if self.explore:
                 h = 1
             make_move = self.rng.choice((True, False), p=(h, 1 - h))
             if make_move:
                 self.old_rss = new_rss
                 self.moves += 1
-                self.visited[self.moves] = new_bic
-                self.markov_chain[self.moves] = self.uec
-                # (2 ** np.flatnonzero(self.cpdag)).sum()]
+                self.bic_markov_chain[self.moves] = new_bic
+                self.nuc_markov_chain[self.moves] = new_nuc
+                self.uec_markov_chain[self.moves] = self.uec
             else:
                 self.cpdag = self.old_cpdag
                 self.dag_reduction = self.old_dag
                 self.chain_comps = self.old_cc
+                self.moves += 1
+                self.bic_markov_chain[self.moves] = self.old_bic
+                self.nuc_markov_chain[self.moves] = self.old_nuc
+                old_uec = self.uec_markov_chain[self.moves - 1]
+                self.uec_markov_chain[self.moves] = old_uec
+
+        vals, idcs, counts = np.unique(
+            self.bic_markov_chain, return_index=True, return_counts=True
+        )
+        map_idx = idcs[np.argmax(counts)]
+        self.map_uec = self.uec_markov_chain[map_idx]
 
     def init_uec(self, init):
         if type(init) is str:
             if init == "empty":
                 self.uec = np.zeros((self.num_feats, self.num_feats), bool)
             elif init == "complete":
                 self.uec = np.ones((self.num_feats, self.num_feats), bool)
@@ -137,25 +160,26 @@
             init, alpha = init
             if init == "gauss":
                 corr = np.corrcoef(self.samples, rowvar=False)
                 dist = beta(
                     self.num_samps / 2 - 1, self.num_samps / 2 - 1, loc=-1, scale=2
                 )
                 crit_val = abs(dist.ppf(alpha / 2))
-                self.uec = self.indep_test_U = abs(corr) >= crit_val
+                self.uec = self.indep_test_uec = abs(corr) >= crit_val
                 np.fill_diagonal(self.uec, False)
             elif init == "dcov_fast":
                 cov, d_bars = dcov(self.samples)
                 crit_val = chi2(1).ppf(1 - alpha)
                 test_val = self.num_samps * cov / np.outer(d_bars, d_bars)
                 self.uec = test_val >= crit_val
                 np.fill_diagonal(self.uec, False)
         else:
             self.uec = np.array(init, bool)
-        self.optimal_uec = self.uec
+        self.bic_uec = self.uec
+        self.nuc_uec = self.uec
 
     def get_max_cpdag(self):
         r"""Return maximal CPDAG in the UEC."""
 
         U = np.copy(self.uec)
         compliment_U = ~U
         np.fill_diagonal(compliment_U, False)
@@ -169,15 +193,15 @@
         # This orients all v-structures and removes edges violating CI relations
         U[W] = False
 
         self.cpdag = U
         recon_uec = self.get_uec()
         if not (recon_uec == self.uec).all():
             # then self.uec was invalid, so reinitialize
-            self.uec = self.optimal_uec = recon_uec
+            self.uec = self.bic_uec = self.nuc_uec = recon_uec
             self.get_max_cpdag()
 
     def reduce_max_cpdag(self):
         cpdag = np.copy(self.cpdag)
         undir = np.logical_and(cpdag, cpdag.T)
         chain_comps = np.eye(self.num_feats).astype(bool)
         while undir.any() and len(undir) > 1:
@@ -309,19 +333,17 @@
 
         if not self.chain_comps[t].any():
             self.chain_comps = np.delete(self.chain_comps, t, 0)
             self.dag_reduction = np.delete(self.dag_reduction, t, 0)
             self.dag_reduction = np.delete(self.dag_reduction, t, 1)
 
     def pick_source_nodes(self, move):
-        # sources have no parents; sinks have parents and no children
+        # sources have no parents
         non_srcs_mask = self.dag_reduction.sum(0).astype(bool)
         sources = np.flatnonzero(np.logical_not(non_srcs_mask))
-        childless_mask = np.logical_not(self.dag_reduction.sum(1).astype(bool))
-        sinks = np.flatnonzero(np.logical_and(non_srcs_mask, childless_mask))
         if move == "merge":
             singleton_nodes = np.flatnonzero(self.chain_comps.sum(1) == 1)
             sngl_srcs = sources[np.in1d(sources, singleton_nodes)]
             ch_subgraph = self.dag_reduction[sngl_srcs].astype(int)
             empty_ch_subgraph = (~self.dag_reduction[sngl_srcs]).astype(int)
             non_empty_same_ch_mask = ch_subgraph @ ch_subgraph.T
             empty_same_ch_mask = empty_ch_subgraph @ empty_ch_subgraph.T
@@ -395,18 +417,19 @@
         recon_uec = T.T @ T
         np.fill_diagonal(recon_uec, False)
         return recon_uec
 
     def get_likelihood_ratio(self):
         self.expand()
         new_rss = self.compute_mle_rss()
-        new_bic = self.num_samps * np.log(new_rss)
-        new_bic += self.cpdag.sum() * np.log(self.num_samps)
-        # unscaled_ratio = (new_likelihood / self.old_likelihood).astype(np.longdouble)
-        return self.old_rss / new_rss, new_rss, new_bic
+        pen_rss = self.num_samps * np.log(new_rss)
+        u, s, vh = svd(self.cpdag)
+        new_bic = (s**2).sum() * np.log(self.num_samps) + pen_rss
+        new_nuc = s.sum() * np.log(self.num_samps) + pen_rss
+        return self.old_rss / new_rss, new_rss, new_bic, new_nuc
 
     def compute_mle_rss(self, graph=None):
         if graph is None:
             graph = self.cpdag
             self.uec = self.get_uec()
         # children_mask = graph.sum(0)
         # children = np.flatnonzero(children_mask)
@@ -503,15 +526,14 @@
         p /= p.sum()
 
         return np.array(poss_moves), considered, p
 
     def scaled_triangle_prior(self, peak_scale):
         if self.pmf is None:
             peak, scale = peak_scale
-            min = 0
             max = self.num_feats + 1
             pmf = np.arange(1, max, dtype=float)
             pmf[peak - 1] = 2 / max
             below = pmf[: peak - 1]
             above = pmf[peak:]
 
             below *= 2 / (max * peak)
```

### Comparing `gues-0.1.0/gues/gues.py` & `gues-0.2.0/gues/gues.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Implement the Greedy Unconditional Equivalence Search (GUES) algorithm."""
 import numpy as np
 from numpy.linalg import lstsq, norm
-from .gauss_obs_l0_pen import GaussObsL0Pen
 from scipy.stats import chi2, beta
 from scipy.spatial.distance import pdist, squareform
 
+from .gauss_obs_l0_pen import GaussObsL0Pen
+
 
 class InputData(object):
     r"""Feed data into GUES to learn its Markov equivalence class.
 
     Attributes
     ----------
     samples : array_like
```

### Comparing `gues-0.1.0/gues/independence_testing.py` & `gues-0.2.0/gues/independence_testing.py`

 * *Files identical despite different names*

### Comparing `gues-0.1.0/gues.egg-info/PKG-INFO` & `gues-0.2.0/gues.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: gues
-Version: 0.1.0
+Version: 0.2.0
 Summary: This package is for (hybrid and) score-based causal structure learning, using unconditional equivalence classes to reduce the search space.
 Author: Alex Markham
 Author-email: alex.markham@causal.dev
 License: GNU Affero General Public License 3 or later (AGPL 3+)
+Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dcor
-Provides-Extra: ges
-Provides-Extra: all
+Provides-Extra: reproduce_astat
 License-File: LICENSE.md
 
-GUES is a Python package for score-based causal structure learning, using unconditional equivalence classes to reduce the search space.
+GUES is a Python package for score-based and hybrid causal structure learning, using unconditional equivalence classes to reduce the search space.
```

### Comparing `gues-0.1.0/setup.py` & `gues-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,30 @@
 def long_description():
     with open("README.md") as readme:
         return readme.read()
 
 
 setup(
     name="gues",
-    version="0.1.0",
+    version="0.2.0",
     author="Alex Markham",
     author_email="alex.markham@causal.dev",
     description="This package is for (hybrid and) score-based causal structure learning, using unconditional equivalence classes to reduce the search space.",
     long_description_content_type="text/markdown",
     long_description=long_description(),
     license="GNU Affero General Public License 3 or later (AGPL 3+)",
     packages=["gues"],
+    python_requires="~=3.11",
     install_requires=["numpy"],
     extras_require={
-        "dcor": ["dcor"],
-        "ges": ["ges"],
-        "all": ["dcor", "ges"],
+        "reproduce_astat": [
+            "numpy~=1.24.3",
+            "scipy~=1.11.1",
+            "matplotlib~=3.7.1",
+            "pandas~=2.0.2",
+            "seaborn~=0.12.2",
+            "big-O~=0.11.0",
+            "pycurl~=7.45.2",
+        ]
     },
+    scripts=["scripts/reproduce_astat"],
 )
```

### Comparing `gues-0.1.0/tests/test_grues.py` & `gues-0.2.0/tests/test_grues.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,8 +348,8 @@
 
 # integration test
 def test_explore():
     samples = np.random.random_sample((50, 3))
     obj = gues.grues.InputData(samples)
     obj.debug = obj.explore = True
     obj.mcmc(max_moves=100)
-    assert len(np.unique(obj.visited)) == 8
+    assert len(np.unique(obj.bic_markov_chain)) == 8
```

### Comparing `gues-0.1.0/tests/test_gues.py` & `gues-0.2.0/tests/test_gues.py`

 * *Files identical despite different names*

