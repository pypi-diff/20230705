# Comparing `tmp/ramanspy-0.0.3.tar.gz` & `tmp/ramanspy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanspy-0.0.3.tar", last modified: Mon Jun 26 22:11:07 2023, max compression
+gzip compressed data, was "ramanspy-0.1.0.tar", last modified: Wed Jul  5 18:49:54 2023, max compression
```

## Comparing `ramanspy-0.0.3.tar` & `ramanspy-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.282372 ramanspy-0.0.3/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.0.3/LICENSE
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       45 2023-06-26 12:05:50.000000 ramanspy-0.0.3/MANIFEST.in
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 22:11:07.282273 ramanspy-0.0.3/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1534 2023-06-26 12:05:35.000000 ramanspy-0.0.3/README.md
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-06-26 22:11:02.000000 ramanspy-0.0.3/pyproject.toml
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-06-26 22:11:07.282407 ramanspy-0.0.3/setup.cfg
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.278118 ramanspy-0.0.3/src/
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.279434 ramanspy-0.0.3/src/ramanspy/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/__init__.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.280666 ramanspy-0.0.3/src/ramanspy/analysis/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/cluster.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2140 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/decompose.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     6702 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/analysis/unmix.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18545 2023-06-26 13:07:02.000000 ramanspy-0.0.3/src/ramanspy/datasets.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10385 2023-06-26 22:05:02.000000 ramanspy-0.0.3/src/ramanspy/load.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/metrics.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.281028 ramanspy-0.0.3/src/ramanspy/plot/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/_core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/plot/plot.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.282117 ramanspy-0.0.3/src/ramanspy/preprocessing/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/Pipeline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/baseline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/denoise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/despike.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/misc.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/normalise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.0.3/src/ramanspy/preprocessing/protocols.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.0.3/src/ramanspy/utils.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 22:11:07.280110 ramanspy-0.0.3/src/ramanspy.egg-info/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/SOURCES.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/dependency_links.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/requires.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-06-26 22:11:07.000000 ramanspy-0.0.3/src/ramanspy.egg-info/top_level.txt
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.806256 ramanspy-0.1.0/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.1.0/LICENSE
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       73 2023-06-30 18:02:25.000000 ramanspy-0.1.0/MANIFEST.in
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4783 2023-07-05 18:49:54.806150 ramanspy-0.1.0/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2335 2023-07-05 18:43:55.000000 ramanspy-0.1.0/README.md
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-07-05 18:46:47.000000 ramanspy-0.1.0/pyproject.toml
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-07-05 18:49:54.806301 ramanspy-0.1.0/setup.cfg
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.800274 ramanspy-0.1.0/src/
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.802301 ramanspy-0.1.0/src/ramanspy/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/__init__.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.803967 ramanspy-0.1.0/src/ramanspy/analysis/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/analysis/cluster.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2284 2023-07-04 16:22:48.000000 ramanspy-0.1.0/src/ramanspy/analysis/decompose.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7553 2023-07-04 18:23:45.000000 ramanspy-0.1.0/src/ramanspy/analysis/unmix.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18768 2023-06-30 17:54:47.000000 ramanspy-0.1.0/src/ramanspy/datasets.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10385 2023-06-26 22:05:02.000000 ramanspy-0.1.0/src/ramanspy/load.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/metrics.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.804587 ramanspy-0.1.0/src/ramanspy/plot/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/_core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/plot/plot.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.805953 ramanspy-0.1.0/src/ramanspy/preprocessing/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/Pipeline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/baseline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/denoise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/despike.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/misc.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/normalise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.1.0/src/ramanspy/preprocessing/protocols.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.1.0/src/ramanspy/utils.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-07-05 18:49:54.803006 ramanspy-0.1.0/src/ramanspy.egg-info/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4783 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/requires.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-07-05 18:49:54.000000 ramanspy-0.1.0/src/ramanspy.egg-info/top_level.txt
```

### Comparing `ramanspy-0.0.3/LICENSE` & `ramanspy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/PKG-INFO` & `ramanspy-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.3
+Version: 0.1.0
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
@@ -94,8 +94,23 @@
 ## Documentation
 
 For more information about the functionalities of the package, refer to
 the [documentation](https://ramanspy.readthedocs.io).
 
 ## Credits
 
-If you find *RamanSPy* useful, please consider leaving a star on [GitHub](https://github.com/barahona-research-group/RamanSPy).
+If you use this package for your research, please cite our paper:
+
+[Georgiev, D., Pedersen, S., Xie, R., Fernández-Galiana, Á., Stevens, M., & Barahona, M. (2023). RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis. ChemRxiv. doi:10.26434/chemrxiv-2023-m3xlm](https://chemrxiv.org/engage/chemrxiv/article-details/64a53861ba3e99daef8c9c51)
+
+```bibtex
+@article{ramanspy_2023,
+    title={RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis},
+    author={Georgiev, Dimitar and Pedersen, Simon Vilms and Xie, Ruoxiao and Fernández-Galiana, Álvaro and Stevens, Molly M. and Barahona, Mauricio},
+    journal={ChemRxiv},
+    publisher={Cambridge Open Engage},
+    year={2023},
+    DOI={10.26434/chemrxiv-2023-m3xlm}
+}
+```
+
+Also, if you find *RamanSPy* useful, please consider leaving a star on [GitHub](https://github.com/barahona-research-group/RamanSPy).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ramanspy-0.0.3/pyproject.toml` & `ramanspy-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramanspy"
-version = "0.0.3"
+version = "0.1.0"
 description = "RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis"
 readme = "README.md"
 authors = [{ name = "Dimitar Georgiev", email = "d.georgiev21@imperial.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `ramanspy-0.0.3/src/ramanspy/analysis/Step.py` & `ramanspy-0.1.0/src/ramanspy/analysis/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/analysis/cluster.py` & `ramanspy-0.1.0/src/ramanspy/analysis/cluster.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/analysis/decompose.py` & `ramanspy-0.1.0/src/ramanspy/analysis/decompose.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         super().__init__(scikit_learn_wrapper(decomp.FastICA), n_components, **kwargs)
 
 
 class NMF(AnalysisStep):
     """
     Non-negative matrix factorisation (NMF).
 
+    Data must be non-negative. If negative values are present, one can use :class:`ramanspy.preprocessing.normalise.MinMax` to scale the data.
+
     Parameters
     ----------
     n_components : int
         The number of components.
     **kwargs :
         Check original `implementation <https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html>`_ for additional parameters.
```

### Comparing `ramanspy-0.0.3/src/ramanspy/analysis/unmix.py` & `ramanspy-0.1.0/src/ramanspy/analysis/unmix.py`

 * *Files 16% similar despite different names*

```diff
@@ -132,63 +132,96 @@
         The abundance finder method to use. Default is ``'fcls'``.
 
         - ``'ucls'`` - Unconstrained Least Squares;
         - ``'nnls'` - Non-negative Least Squares;
         - ``'fcls'`` - Fully-constrained Least Squares.
 
 
-    .. note :: Implementation based on `the MATLAB code provided by the authors <http://www.lx.it.pt/~bioucas/code.htm>`_
+    .. note :: Implementation based on `the MATLAB code provided by the authors <http://www.lx.it.pt/~bioucas/code.htm>`,
                and `Adrien Lagrange's translation to Python <https://github.com/Laadr/VCA>`_.
 
 
     References
     ----------
     Nascimento, J.M. and Dias, J.M., 2005. Vertex component analysis: A fast algorithm to unmix hyperspectral data. IEEE transactions on Geoscience and Remote Sensing, 43(4), pp.898-910.
     """
 
     def __init__(self, *, n_endmembers: int, abundance_method: Literal['ucls', 'nnls', 'fcls'] = 'fcls'):
         super().__init__(unmixer(_vca), n_endmembers, abundance_method)
 
 
-def _vca(data, n_endmembers):
-    data_mean = np.mean(data, axis=0, keepdims=True)
-    data_centered = data - data_mean
-
-    # Project mean-centered data to n_endmembers subspace
-    Ud = splin.svd(np.dot(data_centered, data_centered.T) / float(data.shape[0]))[0]
-    x_p = np.dot(Ud[:, :n_endmembers].T, data_centered)
+def _vca(data, n_endmembers, *, snr_input=0):
+    """
+    Copyright 2018 Adrien Lagrange
+
+    Licensed under the Apache License, Version 2.0.
+
+    Source code available at: https://github.com/Laadr/VCA
+
+    Changes:
+    - sp -> np;
+    - removed comments;
+    - removed semicolons at the end of lines;
+    - removed verbose option and print statements;
+    - renamed some variables;
+    - only return endmembers;
+    """
+    # Transpose data to comply with code
+    data = data.T
+
+    N = data.shape[1]
 
     # Estimate SNR
-    P_y = np.sum(data.T ** 2) / float(data.shape[0])
-    P_x = np.sum(x_p ** 2) / float(data.shape[0]) + np.sum(data_mean ** 2)
-    SNR = 10 * np.log10((P_x - x_p.shape[0] / data.shape[1] * P_y) / (P_y - P_x))
-
-    SNR_threshold = 15 + 10 * np.log10(n_endmembers)
-    if SNR < SNR_threshold:
-        # Project to n_endmembers-1 subspace
-        # """"""""""""""""""""""""""""""""""""""
-        Yp = np.dot(Ud[:, :n_endmembers - 1], x_p[:n_endmembers - 1, :]) + data_mean
+    # ------------
+    if snr_input == 0:
+        data_mean = np.mean(data, axis=1, keepdims=True)
+        data_centered = data - data_mean  # data with zero-mean
+        Ud = splin.svd(np.dot(data_centered, data_centered.T) / float(N))[0][:, :n_endmembers]
+        x_p = np.dot(Ud.T, data_centered)
+
+        P_y = np.sum(data ** 2) / float(N)
+        P_x = np.sum(x_p ** 2) / float(N) + np.sum(data_mean ** 2)
+        SNR = 10 * np.log10((P_x - n_endmembers / data.shape[0] * P_y) / (P_y - P_x))
+    else:
+        SNR = snr_input
+
+    SNR_th = 15 + 10 * np.log10(n_endmembers)
+
+    # Projection to n_endmembers-1 subspace if SNR < SNR_th; else, no projective projection
+    # -------------------------------------------------------------------------------------
+    if SNR < SNR_th:
+        d = n_endmembers - 1
+        if snr_input == 0:
+            Ud = Ud[:, :d]
+        else:
+            data_mean = np.mean(data, axis=1, keepdims=True)
+            data_centered = data - data_mean
+
+            Ud = splin.svd(np.dot(data_centered, data_centered.T) / float(N))[0][:, :d]  # computes the p-projection matrix
+            x_p = np.dot(Ud.T, data_centered)
+
+        Yp = np.dot(Ud, x_p[:d, :]) + data_mean
 
-        x = x_p[:n_endmembers - 1, :]
+        x = x_p[:d, :]
         c = np.amax(np.sum(x ** 2, axis=0)) ** 0.5
-        y = np.vstack((x, c * np.ones((1, data.shape[0]))))
+        y = np.vstack((x, c * np.ones((1, N))))
     else:
-        # Projective Projection
-        # """""""""""""""""""""""
-        Ud = splin.svd(np.dot(data.T, data) / float(data.shape[0]))[0][:, :n_endmembers]
+        d = n_endmembers
+        Ud = splin.svd(np.dot(data, data.T) / float(N))[0][:, :d]
 
-        x = np.dot(Ud.T, data.T)
-        Yp = np.dot(Ud, x[:n_endmembers, :])
+        x_p = np.dot(Ud.T, data)
+        Yp = np.dot(Ud, x_p[:d, :])
 
+        x = np.dot(Ud.T, data)
         u = np.mean(x, axis=1, keepdims=True)
         y = x / np.dot(u.T, x)
 
     # VCA algorithm
-    # --------------
-    indice = np.zeros(n_endmembers, dtype=int)
+    # -------------
+    indice = np.zeros((n_endmembers), dtype=int)
     A = np.zeros((n_endmembers, n_endmembers))
     A[-1, 0] = 1
 
     for i in range(n_endmembers):
         w = np.random.rand(n_endmembers, 1)
         f = w - np.dot(A, np.dot(splin.pinv(A), w))
         f = f / splin.norm(f)
```

### Comparing `ramanspy-0.0.3/src/ramanspy/core.py` & `ramanspy-0.1.0/src/ramanspy/core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/datasets.py` & `ramanspy-0.1.0/src/ramanspy/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     return X, y
 
 
 def covid19(file) -> Tuple[core.SpectralContainer, np.ndarray, np.ndarray]:
     """
     Raman spectra acquired from patients with COVID-19 and healthy controls.
 
-    Data from `Yin G. et al. (2019) <https://pubmed.ncbi.nlm.nih.gov/33821082/>`_.
+    Data from `Yin G. et al. (2021) <https://pubmed.ncbi.nlm.nih.gov/33821082/>`_.
 
     Must be downloaded first. Available on `Kaggle <https://www.kaggle.com/datasets/sfran96/raman-spectroscopy-for-detecting-covid19>`_.
 
     Parameters
     ----------
     file : str, default=None
         Path to the file containing the downloaded data.
@@ -132,14 +132,16 @@
     np.ndarray[string] of shape (B, )
         The names of the labels.
 
     References
     ----------
     Yin G, Li L, Lu S, Yin Y, Su Y, Zeng Y, Luo M, Ma M, Zhou H, Orlandini L, Yao D. An efficient primary screening of COVID‐19 by serum Raman spectroscopy. Journal of Raman Spectroscopy. 2021 May;52(5):949-58.
 
+    Yin G, Li L, Lu S, Yin Y, Su Y, Zeng Y, Luo M, Ma M, Zhou H, Yao D, Liu G, Lang J. Data and code on serum Raman spectroscopy as an efficient primary screening of coronavirus disease in 2019 (COVID-19). figshare; 2020.
+
 
     Examples:
     ----------
 
     .. code::
 
         import ramanspy as rp
```

### Comparing `ramanspy-0.0.3/src/ramanspy/load.py` & `ramanspy-0.1.0/src/ramanspy/load.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/metrics.py` & `ramanspy-0.1.0/src/ramanspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/plot/_core.py` & `ramanspy-0.1.0/src/ramanspy/plot/_core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/plot/plot.py` & `ramanspy-0.1.0/src/ramanspy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/Pipeline.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/Step.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/baseline.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/denoise.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/denoise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/despike.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/despike.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/misc.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/misc.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/normalise.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/normalise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy/preprocessing/protocols.py` & `ramanspy-0.1.0/src/ramanspy/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.3/src/ramanspy.egg-info/PKG-INFO` & `ramanspy-0.1.0/src/ramanspy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.3
+Version: 0.1.0
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
@@ -94,8 +94,23 @@
 ## Documentation
 
 For more information about the functionalities of the package, refer to
 the [documentation](https://ramanspy.readthedocs.io).
 
 ## Credits
 
-If you find *RamanSPy* useful, please consider leaving a star on [GitHub](https://github.com/barahona-research-group/RamanSPy).
+If you use this package for your research, please cite our paper:
+
+[Georgiev, D., Pedersen, S., Xie, R., Fernández-Galiana, Á., Stevens, M., & Barahona, M. (2023). RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis. ChemRxiv. doi:10.26434/chemrxiv-2023-m3xlm](https://chemrxiv.org/engage/chemrxiv/article-details/64a53861ba3e99daef8c9c51)
+
+```bibtex
+@article{ramanspy_2023,
+    title={RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis},
+    author={Georgiev, Dimitar and Pedersen, Simon Vilms and Xie, Ruoxiao and Fernández-Galiana, Álvaro and Stevens, Molly M. and Barahona, Mauricio},
+    journal={ChemRxiv},
+    publisher={Cambridge Open Engage},
+    year={2023},
+    DOI={10.26434/chemrxiv-2023-m3xlm}
+}
+```
+
+Also, if you find *RamanSPy* useful, please consider leaving a star on [GitHub](https://github.com/barahona-research-group/RamanSPy).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ramanspy-0.0.3/src/ramanspy.egg-info/SOURCES.txt` & `ramanspy-0.1.0/src/ramanspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

