# Comparing `tmp/optim_esm_tools-0.2.2.tar.gz` & `tmp/optim_esm_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.2.2.tar", last modified: Mon Jul  3 11:43:09 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.3.0.tar", last modified: Wed Jul  5 12:05:43 2023, max compression
```

## Comparing `optim_esm_tools-0.2.2.tar` & `optim_esm_tools-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/extra_requirements/requirements-tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/_test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/tipping_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/map_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/plotting/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.282885 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 11:43:09.000000 optim_esm_tools-0.2.2/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:43:09.286885 optim_esm_tools-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_find_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_pangeo_download.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_region_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-03 11:43:05.000000 optim_esm_tools-0.2.2/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.555327 optim_esm_tools-0.3.0/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.555327 optim_esm_tools-0.3.0/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/calculate_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23233 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/tipping_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.555327 optim_esm_tools-0.3.0/optim_esm_tools/cmip_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/cmip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/optim_esm_tools/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/plotting/map_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/plotting/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.555327 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 12:05:43.000000 optim_esm_tools-0.3.0/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:05:43.559327 optim_esm_tools-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_find_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_pangeo_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_region_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-05 12:05:40.000000 optim_esm_tools-0.3.0/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.2.2/PKG-INFO` & `optim_esm_tools-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,23 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.3.0 / 2023-07-05
+        ------------------
+        * Remove old setup by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/77
+        * Area calculation  & percentile recombination & weighted clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/76
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.2...v0.3.0
+        
+        
         0.2.2 / 2023-07-02
         ------------------
         * Remove todo by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/67
         * small tas tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/68
         * Add non-tas support by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/69
         * Match fuzzy for version last by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/70
```

### Comparing `optim_esm_tools-0.2.2/README.md` & `optim_esm_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/_test_utils.py` & `optim_esm_tools-0.3.0/optim_esm_tools/_test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/analyze/clustering.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/clustering.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 from optim_esm_tools.utils import tqdm, timed
 import typing as ty
 from warnings import warn
+import numba
+from math import sin, cos, sqrt, atan2, radians
 
 
 @timed()
 def build_clusters(
     coordinates_deg: np.ndarray,
+    weights: ty.Optional[np.ndarray] = None,
     max_distance_km: ty.Union[float, int] = 750,
     only_core: bool = True,
     min_samples: int = 10,
     cluster_opts: ty.Optional[dict] = None,
 ) -> ty.List[np.ndarray]:
     """Build clusters based on a list of coordinates, use halfsine metric for spherical spatiol data
 
@@ -32,16 +35,26 @@
     cluster_opts['min_samples'] = min_samples
 
     from sklearn.cluster import DBSCAN
     import numpy as np
 
     coordinates_rad = np.radians(coordinates_deg).T
 
+    # TODO use a more up to date version:
+    #  https://scikit-learn.org/stable/auto_examples/cluster/plot_hdbscan.html#sphx-glr-auto-examples-cluster-plot-hdbscan-py
+    #  https://scikit-learn.org/stable/modules/generated/sklearn.cluster.HDBSCAN.html#sklearn.cluster.HDBSCAN
     # Thanks https://stackoverflow.com/a/38731787/18280620!
-    db_fit = DBSCAN(eps=max_distance_km / 6371.0, **cluster_opts).fit(coordinates_rad)
+    try:
+        db_fit = DBSCAN(eps=max_distance_km / 6371.0, **cluster_opts).fit(
+            X=coordinates_rad, sample_weight=weights
+        )
+    except ValueError as e:
+        raise ValueError(
+            f'With {coordinates_rad.shape} and {weights.shape} {coordinates_rad}, {weights}'
+        ) from e
 
     labels = db_fit.labels_
 
     unique_labels = sorted(set(labels))
     is_core_sample = np.zeros_like(labels, dtype=bool)
     is_core_sample[db_fit.core_sample_indices_] = True
 
@@ -84,71 +97,143 @@
             Defaults to 'infer'.
         show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
 
     Returns:
         ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
     """
 
-    assert global_mask.shape == (len(x_coord), len(y_coord)), (
-        global_mask.shape,
-        (len(x_coord), len(y_coord)),
-    )
+    _check_input(global_mask, x_coord, y_coord)
     xm, ym = np.meshgrid(x_coord, y_coord)
     xy_data = np.array([xm[global_mask.T], ym[global_mask.T]])
+
     if len(xy_data.T) <= 2:
         warn(f'No data from this mask {xy_data}!')
         return [], []
+
     if max_distance_km == 'infer':
         max_distance_km = _infer_max_step_size(x_coord, y_coord)
+
+    masks, clusters = _build_cluster_with_kw(
+        x_coord,
+        y_coord,
+        coordinates_deg=xy_data,
+        show_tqdm=show_tqdm,
+        max_distance_km=max_distance_km,
+        **kw,
+    )
+
+    return masks, clusters
+
+
+@timed()
+def build_weighted_cluster(
+    weights: np.ndarray,
+    x_coord: np.array,
+    y_coord: np.array,
+    show_tqdm: bool = False,
+    threshold=0.99,
+    max_distance_km: ty.Union[str, float, int] = 'infer',
+    **kw,
+) -> ty.Tuple[ty.List[np.ndarray], ty.List[np.ndarray]]:
+    """Build set of clusters and masks based on the weights (which should be a grid)'
+
+    Args:
+        weights (np.ndarray): normalized score data (values in [0,1])
+        x_coord (np.array): all x values
+        y_coord (np.array): all y values
+        max_distance_km (ty.Union[str, float, int]): find an appropriate distance
+            threshold for build_clusters' max_distance_km argument. If nothing is
+            provided, make a guess based on the distance between grid cells.
+            Defaults to 'infer'.
+        show_tqdm (bool, optional): use verboose progressbar. Defaults to False.
+
+    Returns:
+        ty.List[ty.List[np.ndarray], ty.List[np.ndarray]]: Return two lists, containing the masks, and clusters respectively.
+    """
+
+    _check_input(weights, x_coord, y_coord)
+    xm, ym = np.meshgrid(x_coord, y_coord)
+    xy_data = np.array([xm.flatten(), ym.flatten()])
+
+    if max_distance_km == 'infer':
+        max_distance_km = _infer_max_step_size(x_coord, y_coord)
+
+    flat_weights = weights.T.flatten()
+    mask = flat_weights > threshold
+    masks, clusters = _build_cluster_with_kw(
+        x_coord,
+        y_coord,
+        coordinates_deg=xy_data[:, mask],
+        weights=flat_weights[mask],
+        show_tqdm=show_tqdm,
+        max_distance_km=max_distance_km,
+        **kw,
+    )
+
+    return masks, clusters
+
+
+def _check_input(data, x_coord, y_coord):
+    if data.shape != (len(x_coord), len(y_coord)):
+        message = f'Wrong input {data.shape} != {len(x_coord), len(y_coord)}'
+        raise ValueError(message)
+
+
+def _build_cluster_with_kw(x_coord, y_coord, show_tqdm=False, **cluster_kw):
     masks = []
-    clusters = [np.rad2deg(cluster) for cluster in build_clusters(xy_data, **kw)]
+    clusters = [np.rad2deg(cluster) for cluster in build_clusters(**cluster_kw)]
 
     for cluster in clusters:
         mask = np.zeros((len(y_coord), len(x_coord)), np.bool_)
         for s_x, s_y in tqdm(cluster, desc='fill_mask', disable=not show_tqdm):
             # This is a bit blunt, but it's fast enough to regain the indexes such that we can build a 2d masked array.
             x_i = np.argwhere(np.isclose(x_coord, s_x))[0]
             y_i = np.argwhere(np.isclose(y_coord, s_y))[0]
             mask[y_i, x_i] = 1
         masks.append(mask)
-
     return masks, clusters
 
 
 def _infer_max_step_size(xs, ys):
     ys = ys[ys > 0]
     # coords = [[[xs[0], ys[0]], [xs[0], ys[1]]], [[xs[0], ys[0]], [xs[1], ys[0]]]]
     # Return long:lat
     coords = [[[ys[0], xs[0]], [ys[0], xs[1]]], [[ys[0], xs[0]], [ys[1], xs[0]]]]
     # Return 2x the distance between grid cells
     return 2 * max(_distance(c) for c in coords)
 
 
-def _distance(coords):
+def _distance(coords, force_math=False):
     """Wrapper for if geopy is not installed"""
-    try:
-        import geopy.distance
+    if not force_math:
+        try:
+            import geopy.distance
+
+            return geopy.distance.geodesic(*coords).km
+        except (ImportError, ModuleNotFoundError):
+            pass
+    return _distance_bf_coord(*coords)
+
+
+@numba.njit
+def _distance_bf_coord(lat1, lon1, lat2, lon2):
+    lat1 = radians(lat1)
+    lon1 = radians(lon1)
+    lat2 = radians(lat2)
+    lon2 = radians(lon2)
+    return _distance_bf(lat1, lon1, lat2, lon2)
 
-        return geopy.distance.geodesic(*coords).km
-    except (ImportError, ModuleNotFoundError):
-        return _distance_bf(coords)
 
-
-def _distance_bf(coords):
+@numba.njit
+def _distance_bf(lat1, lon1, lat2, lon2):
     # https://stackoverflow.com/a/19412565/18280620
-    from math import sin, cos, sqrt, atan2, radians
 
     # Approximate radius of earth in km
     R = 6373.0
 
-    lat1 = radians(coords[0][0])
-    lon1 = radians(coords[0][1])
-    lat2 = radians(coords[1][0])
-    lon2 = radians(coords[1][1])
-
     dlon = lon2 - lon1
     dlat = lat2 - lat1
 
     a = sin(dlat / 2) ** 2 + cos(lat1) * cos(lat2) * sin(dlon / 2) ** 2
     c = 2 * atan2(sqrt(a), sqrt(1 - a))
 
     distance = R * c
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     """
     if calculate_conditions is None:
         calculate_conditions = (
             tipping_criteria.StartEndDifference,
             tipping_criteria.StdDetrended,
             tipping_criteria.MaxJump,
             tipping_criteria.MaxDerivitive,
+            tipping_criteria.MaxJumpAndStd,
         )
     if len(set(desc := (c.short_description for c in calculate_conditions))) != len(
         calculate_conditions
     ):
         raise ValueError(f'One or more non unique descriptions {desc}')
     if condition_kwargs is None:
         condition_kwargs = dict()
@@ -74,36 +75,39 @@
                     name=condition_array.name,
                 )
             )
             ds[condition.short_description] = condition_array
     return ds
 
 
+@oet.utils.add_load_kw
 @oet.utils.timed()
 def read_ds(
     base: str,
     variable_of_interest: ty.Tuple[str] = ('tas',),
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     apply_transform: bool = True,
     strict: bool = True,
+    load: bool = True,
     _ma_window: int = 10,
     _cache: bool = True,
     _file_name: str = 'merged.nc',
     **kwargs,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): Variables to handle. Defaults to ('tas',).
         max_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to (2100, 1, 1).
         min_time (ty.Optional[ty.Tuple[int, int, int]], optional): Defines time range in which to load data. Defaults to None.
         transform_ds: (boolm optional): Apply analysis specific postprocessing algoritms. Defaults to True.
         strict (bool, optional): raise errors on loading, if any. Defaults to True.
+        load (bool, optional): apply dataset.load to dataset directly. Defaults to False.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
         _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
 
     kwargs:
         any kwargs are passed onto transfor_ds.
 
     Returns:
@@ -123,26 +127,26 @@
         min_time,
         max_time,
         _ma_window,
         _CMIP_HANDLER_VERSION,
     )
 
     if os.path.exists(post_processed_file) and _cache:
-        return oet.synda_files.format_synda.load_glob(post_processed_file)
+        return oet.analyze.io.load_glob(post_processed_file)
 
     data_path = os.path.join(base, _file_name)
     if not os.path.exists(data_path):
         message = f'No dataset at {data_path}'
         if strict:
             raise FileNotFoundError(message)
         warn(message)
         return None
 
-    data_set = oet.synda_files.format_synda.load_glob(data_path)
-    data_set = oet.synda_files.format_synda.recast(data_set)
+    data_set = oet.analyze.io.load_glob(data_path, load=load)
+    data_set = oet.analyze.io.recast(data_set)
 
     if apply_transform:
         data_set = transform_ds(
             data_set,
             variable_of_interest=variable_of_interest,
             max_time=max_time,
             min_time=min_time,
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/analyze/region_finding.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/region_finding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,59 @@
-import os
 import optim_esm_tools as oet
-from optim_esm_tools.plotting.map_maker import MapMaker
+from optim_esm_tools.plotting.map_maker import MapMaker, HistoricalMapMaker
+from optim_esm_tools.analyze import tipping_criteria
+from optim_esm_tools.analyze.cmip_handler import transform_ds, read_ds
+from optim_esm_tools.analyze.clustering import (
+    build_cluster_mask,
+    build_weighted_cluster,
+)
+from optim_esm_tools.plotting.plot import setup_map, _show
+from optim_esm_tools.analyze.tipping_criteria import var_to_perc, rank2d
+
+
+import os
+
 import numpy as np
+import xarray as xr
+
 import matplotlib.pyplot as plt
-import typing as ty
-from optim_esm_tools.analyze import tipping_criteria
 import logging
-from optim_esm_tools.analyze.cmip_handler import transform_ds, read_ds
+
 import typing as ty
-import matplotlib.pyplot as plt
 from functools import wraps
-import xarray as xr
 import inspect
-from optim_esm_tools.analyze.clustering import build_cluster_mask
-from optim_esm_tools.plotting.plot import setup_map, _show
+import matplotlib.pyplot as plt
+import immutabledict
+
 
 # >>> import scipy
 # >>> scipy.stats.norm.cdf(3)
 # 0.9986501019683699
 # >> scipy.stats.norm.cdf(2)
 # 0.9772498680518208
 _two_sigma_percent = 97.72498680518208
 
 
 # TODO this has too many hardcoded defaults
-def mask_xr_ds(ds_masked, da_mask, masked_dims=('x', 'y'), keep_dims=('time',)):
+def mask_xr_ds(data_set, da_mask, masked_dims=('x', 'y'), keep_dims=('time',)):
+    ds_start = data_set.copy()
     no_drop = set(masked_dims) | set(keep_dims)
-    for spurious_dim in set(ds_masked.dims) - no_drop:
-        oet.config.get_logger().warn(
+    for spurious_dim in set(data_set.dims) - no_drop:
+        message = (
             f'Spurious coordinate {spurious_dim} dropping for safety. Keep {no_drop}'
         )
-        ds_masked = ds_masked.mean(spurious_dim)
-    for k, data_array in ds_masked.data_vars.items():
+        oet.config.get_logger().warn(message)
+        data_set = data_set.mean(spurious_dim)
+    for k, data_array in data_set.data_vars.items():
         if all(dim in list(data_array.dims) for dim in masked_dims):
-            ds_masked[k] = ds_masked[k].where(da_mask, drop=False)
-    return ds_masked
+            da = data_set[k].where(da_mask, drop=False)
+            da = da.assign_attrs(ds_start[k].attrs)
+            data_set[k] = da
+    data_set = data_set.assign_attrs(ds_start.attrs)
+    return data_set
 
 
 def plt_show(*a):
     """Wrapper to disable class methods to follow up with show"""
 
     def somedec_outer(fn):
         @wraps(fn)
@@ -84,31 +99,31 @@
     criteria = (tipping_criteria.StdDetrended, tipping_criteria.MaxJump)
     extra_opt = None
 
     def __init__(
         self,
         variable='tas',
         path=None,
-        dataset=None,
+        data_set=None,
         transform=True,
         save_kw=None,
         extra_opt=None,
         read_ds_kw=None,
     ) -> None:
         read_ds_kw = dict() if read_ds_kw is None else read_ds_kw
         if path is None:
             if transform:
                 self.log.warning(
                     f'Best is to start {self.__class__.__name__} from a synda path'
                 )
-                self.dataset = transform_ds(dataset)
+                self.data_set = transform_ds(data_set)
             else:
-                self.dataset = dataset
+                self.data_set = data_set
         else:
-            self.dataset = read_ds(path, **read_ds_kw)
+            self.data_set = read_ds(path, **read_ds_kw)
         if save_kw is None:
             save_kw = dict(
                 save_in='./',
                 file_types=(
                     'png',
                     'pdf',
                 ),
@@ -128,55 +143,94 @@
             self._logger = oet.config.get_logger()
         return self._logger
 
     @apply_options
     def workflow(self, show_basic=True):
         if show_basic:
             self.plot_basic_map()
-        masks = self.get_masks()
-        self.plot_masks(masks)
-        self.plot_mask_time_series(masks)
+        masks_and_clusters = self.get_masks()
+        masks_and_clusters = self.filter_masks_and_clusters(masks_and_clusters)
+
+        self.plot_masks(masks_and_clusters)
+        self.plot_mask_time_series(masks_and_clusters)
 
     @plt_show
     def plot_basic_map(self):
         self._plot_basic_map()
         self.save(f'{self.title_label}_global_map')
 
     def _plot_basic_map(self):
-        raise NotImplemented(f'{self.__class__.__class__} has no _plot_basic_map')
+        raise NotImplementedError(f'{self.__class__.__class__} has no _plot_basic_map')
 
     def save(self, name):
         assert self.__class__.__name__ in name
         oet.utils.save_fig(name, **self.save_kw)
 
     @property
     def title(self):
-        return MapMaker(self.dataset).title
+        return MapMaker(self.data_set).title
 
     @property
     def title_label(self):
         return self.title.replace(' ', '_') + f'_{self.__class__.__name__}'
 
+    def mask_area(self, mask):
+        try:
+            if mask is None or not np.sum(mask):
+                return 0
+        except Exception as e:
+            print(mask)
+            raise ValueError(
+                mask,
+            ) from e
+        return self.data_set['cell_area'].values[mask].sum()
+
+    @apply_options
+    def mask_is_large_enough(self, mask, min_area_km_sq=0):
+        return self.mask_area(mask) >= min_area_km_sq
+
+    def filter_masks_and_clusters(self, masks_and_clusters):
+        if not len(masks_and_clusters[0]):
+            return [], []
+        ret_m = []
+        ret_c = []
+        for m, c in zip(*masks_and_clusters):
+            if self.mask_is_large_enough(m):
+                ret_m.append(m)
+                ret_c.append(c)
+
+        self.log.warn(f'Keeping {len(ret_m)}/{len(masks_and_clusters[0])} of masks')
+        return ret_m, ret_c
+
 
 class MaxRegion(RegionExtractor):
     def get_masks(self) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         labels = [crit.short_description for crit in self.criteria]
 
         def _val(label):
-            return self.dataset[label].values
+            return self.data_set[label].values
 
         def _max(label):
             return _val(label)[~np.isnan(_val(label))].max()
 
         masks = {label: _val(label) == _max(label) for label in labels}
-        return masks
+        return masks, [None for _ in range(len(masks))]
+
+    @apply_options
+    def filter_masks_and_clusters(self, masks_and_clusters, min_area_km_sq=0):
+        """Wrap filter to work on dicts"""
+        if min_area_km_sq:
+            message = f'Calling {self.__class__.__name__}.filter_masks_and_clusters is nonsensical as masks are single grid cells'
+            oet.config.get_logger().warning(message)
+        return masks_and_clusters
 
     @plt_show
     def plot_masks(self, masks, ax=None, legend=True):
+        masks = masks[0]
         self._plot_masks(masks=masks, ax=ax, legend=legend)
         self.save(f'{self.title_label}_map_maxes_{"-".join(self.labels)}')
 
     @apply_options
     def _plot_masks(self, masks, ax=None, legend=True):
         points = {}
         for key, mask_2d in masks.items():
@@ -190,51 +244,52 @@
             ax.legend(**oet.utils.legend_kw())
         plt.suptitle(self.title, y=0.95)
         plt.ylim(-90, 90)
         plt.xlim(-180, 180)
 
     def _mask_to_coord(self, mask_2d):
         arg_mask = np.argwhere(mask_2d)[0]
-        x = self.dataset.x[arg_mask[1]]
-        y = self.dataset.y[arg_mask[0]]
+        x = self.data_set.x[arg_mask[1]]
+        y = self.data_set.y[arg_mask[0]]
         return x, y
 
     def _plot_basic_map(self):
-        mm = MapMaker(self.dataset)
-        axes = mm.plot_all(2)
+        mm = MapMaker(self.data_set)
+        axes = mm.plot_selected(items=self.labels)
         masks = self.get_masks()
         for ax in axes:
-            self._plot_masks(masks, ax=ax, legend=False)
+            self._plot_masks(masks[0], ax=ax, legend=False)
         plt.suptitle(self.title, y=0.95)
 
     @plt_show
     @apply_options
     def plot_mask_time_series(self, masks, time_series_joined=True):
         res = self._plot_mask_time_series(masks, time_series_joined=time_series_joined)
         if time_series_joined:
             self.save(f'{self.title_label}_time_series_maxes_{"-".join(self.labels)}')
         return res
 
     @apply_options
     def _plot_mask_time_series(
-        self, masks, time_series_joined=True, only_rm=False, axes=None
+        self, masks_and_clusters, time_series_joined=True, only_rm=False, axes=None
     ):
+        masks = masks_and_clusters[0]
         legend_kw = oet.utils.legend_kw(
             loc='upper left', bbox_to_anchor=None, mode=None, ncol=2
         )
         for label, mask_2d in zip(self.labels, masks.values()):
             x, y = self._mask_to_coord(mask_2d)
             plot_labels = {
                 f'{self.variable}': f'{label} at {x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend': f'{label} at {x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
                 f'{self.variable}_run_mean_10': f'$RM_{{10}}$ {label} at {x:.1f}:{y:.1f}',
             }
             argwhere = np.argwhere(mask_2d)[0]
-            ds_sel = self.dataset.isel(x=argwhere[1], y=argwhere[0])
+            ds_sel = self.data_set.isel(x=argwhere[1], y=argwhere[0])
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
                 variable=self.variable,
                 other_dim=(),
                 interval=False,
                 labels=plot_labels,
                 axes=axes,
@@ -250,34 +305,68 @@
 
         for ax in axes:
             ax.legend(**legend_kw)
         plt.suptitle(f'Max. {"-".join(self.labels)} {self.title}', y=0.95)
 
 
 class Percentiles(RegionExtractor):
+    @oet.utils.check_accepts(
+        accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
+    )
     @apply_options
-    def get_masks(self, percentiles=_two_sigma_percent) -> dict:
+    def get_masks(self, cluster_method='masked') -> dict:
         """Get mask for max of ii and iii and a box arround that"""
+        if cluster_method == 'weighted':
+            return self._get_masks_weighted()
+        return self._get_masks_masked()
+
+    @apply_options
+    def _get_masks_weighted(self, min_weight=0.95):
+        labels = [crit.short_description for crit in self.criteria]
+
+        sums = []
+        for lab in labels:
+            vals = self.data_set[lab].values.T
+            vals = rank2d(vals)
+            vals[np.isnan(vals)] = 0
+            sums.append(vals)
+
+        tot_sum = np.zeros_like(sums[0])
+        for s in sums:
+            tot_sum += s
+        tot_sum /= len(sums)
+
+        masks, clusters = build_weighted_cluster(
+            weights=tot_sum,
+            x_coord=self.data_set['x'].values,
+            y_coord=self.data_set['y'].values,
+            threshold=min_weight,
+        )
+        return masks, clusters
+
+    @apply_options
+    def _get_masks_masked(
+        self,
+        percentiles=_two_sigma_percent,
+    ):
         labels = [crit.short_description for crit in self.criteria]
         masks = []
-        vmin_vmax = []
 
         for lab in labels:
-            arr = self.dataset[lab].values.T
+            arr = self.data_set[lab].values.T
             arr_no_nan = arr[~np.isnan(arr)]
-            vmin_vmax.append([np.min(arr_no_nan), np.max(arr_no_nan)])
             thr = np.percentile(arr_no_nan, percentiles)
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         masks, clusters = build_cluster_mask(
-            all_mask, self.dataset['x'].values, self.dataset['y'].values
+            all_mask, self.data_set['x'].values, self.data_set['y'].values
         )
         return masks, clusters
 
     @plt_show
     def plot_masks(self, masks_and_clusters, ax=None, legend=True):
         if not len(masks_and_clusters[0]):
             self.log.warning('No clusters found!')
@@ -296,62 +385,59 @@
         scatter_medians=True,
         ax=None,
         legend=True,
         mask_cbar_kw=None,
         cluster_kw=None,
     ):
         masks, clusters = masks_and_clusters
-        # if masks == [] or masks == [[]]:
-        #     return
-        all_masks = np.zeros(masks[0].shape, np.int16)
-
+        all_masks = np.zeros(masks[0].shape, np.float64)
+        all_masks[:] = np.nan
+        ds_dummy = self.data_set.copy()
+        area = ds_dummy['cell_area'].values
         for m, c in zip(masks, clusters):
-            all_masks[m] = len(c)
+            a = area[m].sum()
+            all_masks[m] = a
+
         if ax is None:
             setup_map()
             ax = plt.gca()
         if mask_cbar_kw is None:
-            mask_cbar_kw = dict(extend='neither', label='Number of gridcells')
+            mask_cbar_kw = dict(extend='neither', label='Area per cluster [km$^2$]')
         mask_cbar_kw.setdefault('orientation', 'horizontal')
-        ds_dummy = self.dataset.copy()
 
-        all_masks = all_masks.astype(np.float16)
-        all_masks[all_masks == 0] = np.nan
-        ds_dummy['n_grid_cells'] = (('y', 'x'), all_masks)
+        ds_dummy['area_square'] = (('y', 'x'), all_masks)
 
-        ds_dummy['n_grid_cells'].plot(
-            cbar_kwargs=mask_cbar_kw, vmin=0, extend='neither'
-        )
+        ds_dummy['area_square'].plot(cbar_kwargs=mask_cbar_kw, vmin=0, extend='neither')
         plt.title('')
         if scatter_medians:
             if cluster_kw is None:
                 cluster_kw = dict()
             for m_i, cluster in enumerate(clusters):
                 ax.scatter(
                     *np.median(cluster, axis=0), label=f'cluster {m_i}', **cluster_kw
                 )
             if legend:
                 plt.legend(**oet.utils.legend_kw())
         plt.suptitle(f'Clusters {self.title}', y=0.97 if len(masks) < 4 else 0.99)
         return ax
 
     def _plot_basic_map(self):
-        mm = MapMaker(self.dataset)
-        axes = mm.plot_all(2)
+        mm = MapMaker(self.data_set)
+        axes = mm.plot_selected(items=self.labels)
         plt.suptitle(self.title, y=0.95)
         return axes
 
         # Could add some masked selection on top
 
     #         masks, _ = self.get_masks()
 
     #         all_masks = masks[0]
     #         for m in masks[1:]:
     #             all_masks &= m
-    #         ds_masked = mask_xr_ds(self.dataset.copy(), all_masks)
+    #         ds_masked = mask_xr_ds(self.data_set.copy(), all_masks)
     #         mm_sel = MapMaker(ds_masked)
     #         for label, ax in zip(mm.labels, axes):
     #             plt.sca(ax)
     #             mm_sel.plot_i(label, ax=ax, coastlines=False)
 
     @plt_show
     @apply_options
@@ -384,15 +470,15 @@
             x, y = np.median(cluster, axis=0)
             plot_labels = {
                 f'{self.variable}': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend': f'Cluster {m_i} near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_detrend_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
                 f'{self.variable}_run_mean_10': f'Cluster {m_i} $RM_{{10}}$ near ~{x:.1f}:{y:.1f}',
             }
-            ds_sel = mask_xr_ds(self.dataset.copy(), mask)
+            ds_sel = mask_xr_ds(self.data_set.copy(), mask)
             mm_sel = MapMaker(ds_sel)
             axes = mm_sel.time_series(
                 variable=self.variable,
                 other_dim=('x', 'y'),
                 interval=True,
                 labels=plot_labels,
                 axes=axes,
@@ -423,27 +509,27 @@
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
-            arr = self.dataset[lab].values.T
+            arr = self.data_set[lab].values.T
             arr_historical = historical_ds[lab].values.T
             thr = np.percentile(
                 arr_historical[~np.isnan(arr_historical)], percentiles_historical
             )
             masks.append(arr >= thr)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         masks, clusters = build_cluster_mask(
-            all_mask, self.dataset['x'].values, self.dataset['y'].values
+            all_mask, self.data_set['x'].values, self.data_set['y'].values
         )
         return masks, clusters
 
     @apply_options
     def find_historical(
         self,
         match_to='piControl',
@@ -451,20 +537,20 @@
         query_updates=None,
         search_kw=None,
     ):
         from optim_esm_tools.config import config
 
         base = os.path.join(
             os.sep,
-            *self.dataset.attrs['path'].split(os.sep)[
+            *self.data_set.attrs['path'].split(os.sep)[
                 : -len(config['CMIP_files']['folder_fmt'].split()) - look_back_extra
             ],
         )
 
-        search = oet.cmip_files.find_matches.folder_to_dict(self.dataset.attrs['path'])
+        search = oet.cmip_files.find_matches.folder_to_dict(self.data_set.attrs['path'])
         search['activity_id'] = 'CMIP'
         if search['experiment_id'] == match_to:
             raise NotImplementedError()
         search['experiment_id'] = match_to
         if search_kw:
             search.update(search_kw)
         if query_updates is None:
@@ -494,54 +580,62 @@
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
         historical_path = self.find_historical(**kw)[0]
         return read_ds(historical_path, **read_ds_kw)
 
 
 class ProductPercentiles(Percentiles):
-    @staticmethod
-    def var_to_perc(ds: xr.Dataset, dest_var: str, source_var: str) -> xr.Dataset:
-        """Calculate the percentile score of each of the data var, and assign it to the data set to get
-
-        Args:
-            ds (xr.Dataset): dataset with data-var to calculate the percentiles of
-            dest_var (str): under wich name the scores should be combined under.
-            source_var (str): property to calculate the percentiles of
-
-        Returns:
-            xr.Dataset: Original dataset with one extra colum (dest_var)
-        """
-        from scipy.stats import percentileofscore
-
-        a = ds[source_var].values
-        a_flat = a[~np.isnan(a)].flatten()
-        pcts = [
-            [percentileofscore(a_flat, i, kind='strict') / 100 for i in aa]
-            for aa in oet.utils.tqdm(a)
-        ]
-        ds[dest_var] = (ds[source_var].dims, pcts)
-        return ds
+    labels = ('ii', 'iii', 'v')
 
+    @oet.utils.check_accepts(
+        accepts=immutabledict.immutabledict(cluster_method=('weighted', 'masked'))
+    )
     @apply_options
-    def get_masks(self, product_percentiles=_two_sigma_percent) -> dict:
+    def get_masks(self, cluster_method='masked') -> dict:
+        """Get mask for max of ii and iii and a box arround that"""
+        if cluster_method == 'weighted':
+            return self._get_masks_weighted()
+        return self._get_masks_masked()
+
+    @apply_options
+    def _get_masks_weighted(self, min_weight=0.95):
+        labels = [crit.short_description for crit in self.criteria]
+        masks = []
+
+        ds = self.data_set.copy()
+        combined_score = np.ones_like(ds[labels[0]].values)
+        for label in labels:
+            combined_score *= rank2d(ds[label].values)
+
+        combined_score = combined_score.T
+
+        masks, clusters = build_weighted_cluster(
+            weights=combined_score,
+            x_coord=self.data_set['x'].values,
+            y_coord=self.data_set['y'].values,
+            threshold=min_weight,
+        )
+        return masks, clusters
+
+    @apply_options
+    def _get_masks_masked(self, product_percentiles=_two_sigma_percent) -> dict:
         """Get mask for max of ii and iii and a box arround that"""
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
-        ds = self.dataset.copy()
+        ds = self.data_set.copy()
         combined_score = np.ones_like(ds[labels[0]].values)
         for label in labels:
-            _name = f'percentile {label}'
-            combined_score *= self.var_to_perc(ds, _name, label)[_name].values
+            combined_score *= rank2d(ds[label].values)
 
         # Combined score is fraction, not percent!
         all_mask = (combined_score > (product_percentiles / 100)).T
 
         masks, clusters = build_cluster_mask(
-            all_mask, self.dataset['x'].values, self.dataset['y'].values
+            all_mask, self.data_set['x'].values, self.data_set['y'].values
         )
         return masks, clusters
 
 
 class LocalHistory(PercentilesHistory):
     @apply_options
     def get_masks(self, n_times_historical=4, read_ds_kw=None) -> dict:
@@ -551,74 +645,39 @@
             read_ds_kw.setdefault(k, v)
 
         historical_ds = self.get_historical_ds(read_ds_kw=read_ds_kw)
         labels = [crit.short_description for crit in self.criteria]
         masks = []
 
         for lab in labels:
-            arr = self.dataset[lab].values.T
+            arr = self.data_set[lab].values.T
             arr_historical = historical_ds[lab].values.T
             mask_divide = arr / arr_historical > n_times_historical
             # If arr_historical is 0, the devision is going to get a nan assigned,
             # despite this being the most interesting region (no historical
             # changes, only in the scenario's)!
             mask_no_std = (arr_historical == 0) & (arr > 0)
             masks.append(mask_divide | mask_no_std)
 
         all_mask = np.ones_like(masks[0])
         for m in masks:
             all_mask &= m
 
         masks, clusters = build_cluster_mask(
-            all_mask, self.dataset['x'].values, self.dataset['y'].values
+            all_mask, self.data_set['x'].values, self.data_set['y'].values
         )
         return masks, clusters
 
     @apply_options
-    def _plot_basic_map(self, read_ds_kw=None):
+    def _plot_basic_map(self, normalizations=None, read_ds_kw=None):
         if read_ds_kw is None:
             read_ds_kw = dict()
         for k, v in dict(min_time=None, max_time=None).items():
             read_ds_kw.setdefault(k, v)
         ds_historical = self.get_historical_ds(read_ds_kw=read_ds_kw)
 
-        class TempMapMaker(MapMaker):
-            def __getattr__(self, item):
-                if item in self.conditions:
-                    condition = self.conditions[item]
-                    da = self.data_set[condition.short_description]
-                    da_historical = ds_historical[condition.short_description]
-
-                    result = da / da_historical
-                    ret_array = result.values
-                    if len(ret_array) == 0:
-                        raise ValueError(
-                            f'Empty ret array, perhaps {da.shape} and {da_historical.shape} don\'t match?'
-                            f'\nGot\n{ret_array}\n{result}\n{da}\n{da_historical}'
-                        )
-                    max_val = np.nanmax(ret_array)
-                    mask_divide_by_zero = (da_historical == 0) & (da > 0)
-                    ret_array[mask_divide_by_zero.values] = 10 * max_val
-                    result.data = ret_array
-                    current_norm = self.normalizations.copy()
-
-                    current_norm.update(dict(item=[None, max_val]))
-
-                    self.set_normalizations(current_norm)
-
-                    result.assign_attrs(
-                        dict(
-                            short_description=condition.short_description,
-                            long_description=condition.long_description,
-                            name=f'Change w.r.t. historical of\n{da.name}',
-                        )
-                    )
-
-                    return result
-                return self.__getattribute__(item)
-
-        mm = TempMapMaker(self.dataset)
-        axes = mm.plot_all(2)
-        # masks = self.get_masks()
-        # for ax in axes:
-        #     self._plot_masks(masks, ax=ax, legend=False)
+        mm = HistoricalMapMaker(
+            self.data_set, ds_historical=ds_historical, normalizations=normalizations
+        )
+        mm.plot_selected()
         plt.suptitle(self.title, y=0.95)
+        return mm
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/analyze/tipping_criteria.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/tipping_criteria.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from .xarray_tools import apply_abs, _native_date_fmt, _remove_any_none_times
 from optim_esm_tools.utils import check_accepts, timed
+from .globals import _SECONDS_TO_YEAR
+
 import xarray as xr
-import numpy as np
+
 import typing as ty
-from .globals import _SECONDS_TO_YEAR
 import abc
 from immutabledict import immutabledict
+import numpy as np
 
 
 class _Condition(abc.ABC):
     short_description: str
     defaults = immutabledict(
         rename_to='long_name',
         unit='absolute',
@@ -36,17 +38,17 @@
 class StartEndDifference(_Condition):
     short_description: str = 'start end difference'
 
     @property
     def long_description(self):
         return f'Difference of running mean ({self.running_mean} yr) between start and end of time series. Not detrended'
 
-    def calculate(self, dataset):
+    def calculate(self, data_set):
         return running_mean_diff(
-            dataset,
+            data_set,
             variable=self.variable,
             time_var=self.time_var,
             naming='{variable}_run_mean_{running_mean}',
             running_mean=self.running_mean,
             # TODO
             # Pass kw arguments on? I think not
             _t_0_date=None,
@@ -58,17 +60,17 @@
 class StdDetrended(_Condition):
     short_description: str = 'std detrended'
 
     @property
     def long_description(self):
         return f'Standard deviation of running mean ({self.running_mean} yr). Detrended'
 
-    def calculate(self, dataset):
+    def calculate(self, data_set):
         return running_mean_std(
-            dataset,
+            data_set,
             variable=self.variable,
             time_var=self.time_var,
             naming='{variable}_detrend_run_mean_{running_mean}',
             running_mean=self.running_mean,
             **self.defaults,
         )
 
@@ -80,17 +82,17 @@
         super().__init__(*args, **kwargs)
         self.number_of_years = 10
 
     @property
     def long_description(self):
         return f'Max change in {self.number_of_years} yr in the running mean ({self.running_mean} yr). Not detrended'
 
-    def calculate(self, dataset):
+    def calculate(self, data_set):
         return max_change_xyr(
-            dataset,
+            data_set,
             variable=self.variable,
             time_var=self.time_var,
             naming='{variable}_run_mean_{running_mean}',
             x_yr=self.number_of_years,
             running_mean=self.running_mean,
             **self.defaults,
         )
@@ -99,25 +101,53 @@
 class MaxDerivitive(_Condition):
     short_description: str = 'max derivative'
 
     @property
     def long_description(self):
         return f'Max value of the first order derivative of the running mean ({self.running_mean} yr). Not deterended'
 
-    def calculate(self, dataset):
+    def calculate(self, data_set):
         return max_derivative(
-            dataset,
+            data_set,
             variable=self.variable,
             time_var=self.time_var,
             naming='{variable}_run_mean_{running_mean}',
             running_mean=self.running_mean,
             **self.defaults,
         )
 
 
+class MaxJumpAndStd(MaxJump, StdDetrended):
+    short_description: str = 'percentile score std and max jump'
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.number_of_years = 10
+
+    @property
+    def long_description(self):
+        return f'Product of {super(MaxJumpAndStd, self).short_description} and {super(MaxJump, self).short_description}'
+
+    def calculate(self, data_set):
+        super_1 = super(MaxJump, self)
+        super_2 = super(MaxJumpAndStd, self)
+        da_1 = super_1.calculate(data_set)
+        da_2 = super_2.calculate(data_set)
+
+        combined_score = np.ones_like(da_1.values)
+        for da, label in zip(
+            [da_1, da_2], [super_1.short_description, super_2.short_description]
+        ):
+            _name = f'percentile {label}'
+            combined_score *= var_to_perc(da, _name, None)
+        return xr.DataArray(
+            combined_score, dims=('y', 'x'), name=self.short_description
+        )
+
+
 @timed
 @apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def running_mean_diff(
     data_set: xr.Dataset,
     variable: str,
     time_var: str = 'time',
@@ -149,15 +179,15 @@
     Returns:
         xr.Dataset:
     """
     var_name = naming.format(variable=variable, running_mean=running_mean)
     _time_values = data_set[time_var].dropna(time_var)
 
     if not len(_time_values):
-        raise ValueError(f'No values for {time_var} in dataset?')
+        raise ValueError(f'No values for {time_var} in data_set?')
 
     data_var = _remove_any_none_times(data_set[var_name], time_var)
 
     if _t_0_date is not None:
         t_0 = _native_date_fmt(_time_values, _t_0_date)
         data_t_0 = data_var.sel(time=t_0, method='nearest')
     else:
@@ -295,7 +325,51 @@
         return result
 
     if unit == 'std':
         # A local unit of sigma might be better X.std(dim=time_var)
         result = result / data_array.std()
         result.name = f'Max $\partial/\partial t$ {name} [$\sigma$/yr]'
         return result
+
+
+def rank2d(a):
+    """Calculate precentiles of values in `a`"""
+    from scipy.interpolate import interp1d
+
+    a_flat = a[~np.isnan(a)].flatten()
+    # This is equivalent to
+    # from scipy.stats import percentileofscore
+    # import optim_esm_tools as oet
+    # pcts = [[percentileofscore(a_flat, i, kind='mean') / 100 for i in aa]
+    #         for aa in oet.utils.tqdm(a)]
+    # return pcts
+    n = len(a_flat)
+    itp = interp1d(np.sort(a_flat), np.arange(n) / n, bounds_error=False)
+    return itp(a)
+
+
+def var_to_perc(
+    ds: ty.Union[xr.Dataset, xr.DataArray], dest_var: str, source_var: str
+) -> ty.Union[xr.Dataset, np.ndarray]:
+    """Calculate the percentile score of each of the data var, and assign it to the data set to get
+
+    Args:
+        ds (xr.Dataset): data_set with data-var to calculate the percentiles of
+        dest_var (str): under wich name the scores should be combined under.
+        source_var (str): property to calculate the percentiles of
+
+    Returns:
+        xr.Dataset: Original data_set with one extra colum (dest_var)
+    """
+    if source_var is None:
+        # data array
+        source_array = ds
+    else:
+        source_array = ds[source_var]
+
+    percentiles = rank2d(source_array.values)
+
+    if source_var is None:
+        return percentiles
+
+    ds[dest_var] = (source_array.dims, percentiles)
+    return ds
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/xarray_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 import typing as ty
 import xarray as xr
 from functools import wraps
+import numba
 
 
 def _native_date_fmt(time_array: np.array, date: ty.Tuple[int, int, int]):
     """Create date object using the date formatting from the time-array"""
 
     if isinstance(time_array, xr.DataArray):
         return _native_date_fmt(time_array=time_array.values, date=date)
@@ -47,22 +48,19 @@
             slices[n_slices][1][0] = y
             slices[n_slices][1][1] = y + 1
 
             n_slices += 1
     return slices[:n_slices]
 
 
+_n_mask2d_to_xy_slice = numba.njit(_mask2d_to_xy_slice)
+
+
 def mask2d_to_xy_slice(*args, **kwargs):
-    try:
-        import numba
-    except (ImportError, ModuleNotFoundError) as exeception:
-        raise ModuleNotFoundError(
-            'Numba is an optional dependency, please try pip install numba'
-        ) from e
-    return numba.njit(_mask2d_to_xy_slice)(*args, **kwargs)
+    return _n_mask2d_to_xy_slice(*args, **kwargs)
 
 
 def apply_abs(apply=True, add_abs_to_name=True, _disable_kw='apply_abs'):
     """Apply np.max() to output of function (if apply=True)
     Disable in the function kwargs by using the _disable_kw argument
 
     Example:
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/cmip_files/find_matches.py` & `optim_esm_tools-0.3.0/optim_esm_tools/analyze/find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/config.py` & `optim_esm_tools-0.3.0/optim_esm_tools/config.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.3.0/optim_esm_tools/synda_files/synda_files.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools/utils.py` & `optim_esm_tools-0.3.0/optim_esm_tools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from platform import python_version
 from functools import wraps
 from immutabledict import immutabledict
 import warnings
 import time
 import numpy as np
 import pandas as pd
+import inspect
 
 try:
     from git import Repo, InvalidGitRepositoryError
 
     GIT_INSTALLED = True
 except (ImportError, ModuleNotFoundError):
     GIT_INSTALLED = False
@@ -286,14 +287,31 @@
             return response
 
         return somedec_inner
 
     return somedec_outer
 
 
+def add_load_kw(func):
+    """Add apply `.load` method to the dataset returned by wrapped function"""
+
+    @wraps(func)
+    def dep_fun(*args, **kwargs):
+        if 'load' not in inspect.signature(func).parameters:
+            add_load = kwargs.pop('load', False)
+        else:
+            add_load = kwargs.get('load', False)
+        res = func(*args, **kwargs)
+        if add_load:
+            return res.load()
+        return res
+
+    return dep_fun
+
+
 def deprecated(func, message='is deprecated'):
     @wraps(func)
     def dep_fun(*args, **kwargs):
         warnings.warn(
             f'calling {func.__name__} {message}',
             category=DeprecationWarning,
         )
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-0.3.0/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         [![PyPI version shields.io](https://img.shields.io/pypi/v/optim-esm-tools.svg)](https://pypi.python.org/pypi/optim-esm-tools/)
@@ -15,14 +15,23 @@
         Getting started with OptimESM
         
         Selection of tools and tricks for [OptimESM](https://cordis.europa.eu/project/id/101081193) project.
         
         J.R. Angevaare (KNMI)
         
         
+        0.3.0 / 2023-07-05
+        ------------------
+        * Remove old setup by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/77
+        * Area calculation  & percentile recombination & weighted clustering by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/76
+        
+        
+        **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/compare/v0.2.2...v0.3.0
+        
+        
         0.2.2 / 2023-07-02
         ------------------
         * Remove todo by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/67
         * small tas tweaks by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/68
         * Add non-tas support by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/69
         * Match fuzzy for version last by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/70
```

### Comparing `optim_esm_tools-0.2.2/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.3.0/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-extra_requirements/requirements-tests.txt
 optim_esm_tools/__init__.py
 optim_esm_tools/_test_utils.py
 optim_esm_tools/config.py
 optim_esm_tools/utils.py
 optim_esm_tools.egg-info/PKG-INFO
 optim_esm_tools.egg-info/SOURCES.txt
 optim_esm_tools.egg-info/dependency_links.txt
 optim_esm_tools.egg-info/not-zip-safe
 optim_esm_tools.egg-info/requires.txt
 optim_esm_tools.egg-info/top_level.txt
 optim_esm_tools/analyze/__init__.py
+optim_esm_tools/analyze/calculate_metric.py
 optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
+optim_esm_tools/analyze/find_matches.py
 optim_esm_tools/analyze/globals.py
+optim_esm_tools/analyze/io.py
 optim_esm_tools/analyze/region_finding.py
 optim_esm_tools/analyze/tipping_criteria.py
 optim_esm_tools/analyze/xarray_tools.py
 optim_esm_tools/cmip_files/__init__.py
-optim_esm_tools/cmip_files/find_matches.py
-optim_esm_tools/cmip_files/io.py
 optim_esm_tools/plotting/__init__.py
 optim_esm_tools/plotting/map_maker.py
 optim_esm_tools/plotting/plot.py
 optim_esm_tools/synda_files/__init__.py
 optim_esm_tools/synda_files/format_synda.py
 optim_esm_tools/synda_files/synda_files.py
 test/test_basics.py
```

### Comparing `optim_esm_tools-0.2.2/setup.py` & `optim_esm_tools-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.2.2',
+    version='0.3.0',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
-    packages=setuptools.find_packages() + ['extra_requirements'],
+    packages=setuptools.find_packages(),
     package_dir={
         'optim_esm_tools': 'optim_esm_tools',
-        'extra_requirements': 'extra_requirements',
     },
     package_data={
         'optim_esm_tools': ['data/*'],
-        'extra_requirements': ['requirements-tests.txt'],
     },
     setup_requires=['pytest-runner'],
     install_requires=requirements,
     python_requires='>=3.8',
     tests_require=requirements + open_requirements('requirements_tests.txt'),
     scripts=[],
     keywords=[],
```

### Comparing `optim_esm_tools-0.2.2/test/test_clustering.py` & `optim_esm_tools-0.3.0/test/test_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,11 +46,14 @@
 
 def test_geopy_alternative():
     xs, ys = np.random.rand(1, 4).reshape(2, 2)
     xs *= 360
     ys = ys * 180 - 90
     # LAT:LON!
     coords = np.array([ys, xs]).T
-    print(coords)
+    flat_coord = coords.flatten()
+    print(coords, flat_coord)
     assert np.isclose(
-        clustering._distance_bf(coords), clustering._distance(coords), rtol=0.1
+        clustering._distance_bf_coord(*flat_coord),
+        clustering._distance(coords),
+        rtol=0.1,
     )
```

### Comparing `optim_esm_tools-0.2.2/test/test_find_matches.py` & `optim_esm_tools-0.3.0/test/test_find_matches.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/test/test_region_finding.py` & `optim_esm_tools-0.3.0/test/test_region_finding.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,33 +18,34 @@
             data_name, refresh=refresh
         )
         year_path = optim_esm_tools._test_utils.year_means(path, refresh=refresh)
         assert year_path
         assert os.path.exists(year_path)
         return year_path
 
-    def test_max_region(self, make='MaxRegion', new_opt=None):
+    def test_max_region(self, make='MaxRegion', new_opt=None, skip_save=True):
         cls = getattr(region_finding, make)
+        file_path = self.get_path('ssp585', refresh=False)
+        head, tail = os.path.split(file_path)
         extra_opt = dict(
             time_series_joined=True,
             scatter_medians=True,
             percentiles=50,
-            search_kw=dict(required_file=os.path.split(self.get_path('ssp585'))[1]),
+            search_kw=dict(required_file=tail),
         )
         if new_opt:
             extra_opt.update(new_opt)
         with tempfile.TemporaryDirectory() as temp_dir:
             save_kw = dict(
                 save_in=temp_dir,
                 sub_dir=None,
                 file_types=('png',),
                 dpi=25,
-                skip=False,
+                skip=skip_save,
             )
-            head, tail = os.path.split(self.get_path('ssp585', refresh=False))
             region_finder = cls(
                 path=head,
                 read_ds_kw=dict(_file_name=tail),
                 transform=True,
                 save_kw=save_kw,
                 extra_opt=extra_opt,
             )
@@ -54,18 +55,26 @@
 
     def test_max_region_wo_time_series(self):
         self.test_max_region('MaxRegion', new_opt=dict(time_series_joined=False))
 
     def test_percentiles(self):
         self.test_max_region('Percentiles', new_opt=dict(time_series_joined=False))
 
+    def test_percentiles_weighted(self):
+        self.test_max_region('Percentiles', new_opt=dict(cluster_method='weighted'))
+
     def test_percentiles_history(self):
         region_finder = self.test_max_region('PercentilesHistory')
         with self.assertRaises(RuntimeError):
             # We only have piControl (so this should fail)!
             region_finder.find_historical('historical')
 
     def test_percentiles_product(self):
-        self.test_max_region('ProductPercentiles')
+        self.test_max_region('ProductPercentiles', skip_save=False)
 
     def test_local_history(self):
         self.test_max_region('LocalHistory')
+
+    def test_percentiles_product_weighted(self):
+        self.test_max_region(
+            'ProductPercentiles', new_opt=dict(cluster_method='weighted')
+        )
```

### Comparing `optim_esm_tools-0.2.2/test/test_utils.py` & `optim_esm_tools-0.3.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/test/test_viewer.py` & `optim_esm_tools-0.3.0/test/test_viewer.py`

 * *Files identical despite different names*

### Comparing `optim_esm_tools-0.2.2/test/test_workflow.py` & `optim_esm_tools-0.3.0/test/test_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         )
 
     def setUp(self):
         self.from_amon_to_ayear()
         super().setUp()
 
     def test_read_data(self):
-        data_set = oet.cmip_files.io.load_glob(self.ayear_file)
+        dataset = oet.cmip_files.io.load_glob(self.ayear_file)
 
     def test_make_map(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.plotting.map_maker.MapMaker(data_set=data_set).plot_all(2)
         plt.clf()
 
     def test_map_maker_time_series(self):
```

### Comparing `optim_esm_tools-0.2.2/test/test_xarray_tools.py` & `optim_esm_tools-0.3.0/test/test_xarray_tools.py`

 * *Files identical despite different names*

