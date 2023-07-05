# Comparing `tmp/xugrid-0.5.0.tar.gz` & `tmp/xugrid-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xugrid-0.5.0.tar", last modified: Thu May 25 15:30:10 2023, max compression
+gzip compressed data, was "xugrid-0.6.0.tar", last modified: Wed Jul  5 14:38:00 2023, max compression
```

## Comparing `xugrid-0.5.0.tar` & `xugrid-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.924360 xugrid-0.5.0/
--rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.5.0/LICENSE
--rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3298 2023-05-25 15:30:10.925357 xugrid-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.5.0/README.rst
--rw-rw-rw-   0        0        0     2199 2023-05-25 15:26:07.000000 xugrid-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      178 2023-05-25 15:30:10.934354 xugrid-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.283814 xugrid-0.5.0/tests/
--rw-rw-rw-   0        0        0    15587 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_connectivity.py
--rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_conventions.py
--rw-rw-rw-   0        0        0     9027 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_conversion.py
--rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_data.py
--rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_interpolate.py
--rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_meshkernel_utils.py
--rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.5.0/tests/test_snap.py
--rw-rw-rw-   0        0        0     9280 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid1d.py
--rw-rw-rw-   0        0        0    30534 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid2d.py
--rw-rw-rw-   0        0        0    26751 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_ugrid_dataset.py
--rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.5.0/tests/test_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.307787 xugrid-0.5.0/xugrid/
--rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/constants.py
--rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/conversion.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.367313 xugrid-0.5.0/xugrid/core/
--rw-rw-rw-   0        0        0     3303 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/accessorbase.py
--rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/core/common.py
--rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/dataarray_accessor.py
--rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/core/dataset_accessor.py
--rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/core/wrap.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.387314 xugrid-0.5.0/xugrid/data/
--rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/data/registry.txt
--rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/sample_data.py
--rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/data/synthetic.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/meshkernel_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.403313 xugrid-0.5.0/xugrid/plot/
--rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/plot/__init__.py
--rw-rw-rw-   0        0        0    24058 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.555314 xugrid-0.5.0/xugrid/regrid/
--rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/regrid/overlap_1d.py
--rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.5.0/xugrid/regrid/reduce.py
--rw-rw-rw-   0        0        0    17648 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/regridder.py
--rw-rw-rw-   0        0        0    22639 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/structured.py
--rw-rw-rw-   0        0        0     4658 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/unstructured.py
--rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.5.0/xugrid/regrid/utils.py
--rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/regrid/weight_matrix.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.921352 xugrid-0.5.0/xugrid/ugrid/
--rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/__init__.py
--rw-rw-rw-   0        0        0    18746 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/connectivity.py
--rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/conventions.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/interpolate.py
--rw-rw-rw-   0        0        0    10227 2023-03-13 10:25:22.000000 xugrid-0.5.0/xugrid/ugrid/partitioning.py
--rw-rw-rw-   0        0        0    14979 2023-05-05 14:49:08.000000 xugrid-0.5.0/xugrid/ugrid/snapping.py
--rw-rw-rw-   0        0        0    17949 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugrid1d.py
--rw-rw-rw-   0        0        0    53962 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugrid2d.py
--rw-rw-rw-   0        0        0    19806 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/ugridbase.py
--rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.5.0/xugrid/ugrid/voronoi.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:30:10.330785 xugrid-0.5.0/xugrid.egg-info/
--rw-rw-rw-   0        0        0     3298 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 15:30:10.000000 xugrid-0.5.0/xugrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 14:38:00.009214 xugrid-0.6.0/
+-rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2023-07-05 14:38:00.010215 xugrid-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.6.0/README.rst
+-rw-rw-rw-   0        0        0     2199 2023-07-05 14:19:40.000000 xugrid-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      178 2023-07-05 14:38:00.012230 xugrid-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.706218 xugrid-0.6.0/tests/
+-rw-rw-rw-   0        0        0    17755 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_connectivity.py
+-rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_conventions.py
+-rw-rw-rw-   0        0        0     9008 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_conversion.py
+-rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_data.py
+-rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_meshkernel_utils.py
+-rw-rw-rw-   0        0        0     8494 2023-06-26 11:20:36.000000 xugrid-0.6.0/tests/test_partitioning.py
+-rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_plot.py
+-rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_snap.py
+-rw-rw-rw-   0        0        0    11263 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_ugrid1d.py
+-rw-rw-rw-   0        0        0    32742 2023-06-26 11:20:36.000000 xugrid-0.6.0/tests/test_ugrid2d.py
+-rw-rw-rw-   0        0        0    28063 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_ugrid_dataset.py
+-rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.6.0/tests/test_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.733220 xugrid-0.6.0/xugrid/
+-rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/constants.py
+-rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.821272 xugrid-0.6.0/xugrid/core/
+-rw-rw-rw-   0        0        0     4322 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/core/accessorbase.py
+-rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/core/common.py
+-rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/core/dataarray_accessor.py
+-rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/core/dataset_accessor.py
+-rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/core/wrap.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.853211 xugrid-0.6.0/xugrid/data/
+-rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/data/registry.txt
+-rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/sample_data.py
+-rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/synthetic.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/meshkernel_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.867212 xugrid-0.6.0/xugrid/plot/
+-rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/plot/__init__.py
+-rw-rw-rw-   0        0        0    24101 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.918213 xugrid-0.6.0/xugrid/regrid/
+-rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/regrid/overlap_1d.py
+-rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.6.0/xugrid/regrid/reduce.py
+-rw-rw-rw-   0        0        0    18493 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/regrid/regridder.py
+-rw-rw-rw-   0        0        0    23864 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/regrid/structured.py
+-rw-rw-rw-   0        0        0     4883 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/regrid/unstructured.py
+-rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.6.0/xugrid/regrid/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/regrid/weight_matrix.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:38:00.002219 xugrid-0.6.0/xugrid/ugrid/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/ugrid/__init__.py
+-rw-rw-rw-   0        0        0    24707 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/connectivity.py
+-rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/ugrid/conventions.py
+-rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/ugrid/interpolate.py
+-rw-rw-rw-   0        0        0    11044 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/ugrid/partitioning.py
+-rw-rw-rw-   0        0        0    15005 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/snapping.py
+-rw-rw-rw-   0        0        0    19654 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/ugrid1d.py
+-rw-rw-rw-   0        0        0    56124 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/ugrid/ugrid2d.py
+-rw-rw-rw-   0        0        0    22664 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/ugridbase.py
+-rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/ugrid/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.765220 xugrid-0.6.0/xugrid.egg-info/
+-rw-rw-rw-   0        0        0     3298 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/top_level.txt
```

### Comparing `xugrid-0.5.0/LICENSE` & `xugrid-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/PKG-INFO` & `xugrid-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.5.0
+Version: 0.6.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.5.0/README.rst` & `xugrid-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/pyproject.toml` & `xugrid-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xugrid"
 description = "Xarray extension for unstructured grids"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.5.0"
+version = "0.6.0"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.7"
 dependencies = [
     'pandas',
     'numba',
     'numba_celltree',
     'numpy',
```

### Comparing `xugrid-0.5.0/tests/test_connectivity.py` & `xugrid-0.6.0/tests/test_connectivity.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 
 def test_neighbors():
     i = [0, 0, 0, 1, 1, 1]
     j = [0, 1, 2, 1, 3, 2]
     coo_content = (j, (i, j))
     A = sparse.coo_matrix(coo_content).tocsr()
-    A = connectivity.AdjacencyMatrix(A.indices, A.indptr, A.nnz)
+    n, m = A.shape
+    A = connectivity.AdjacencyMatrix(A.indices, A.indptr, A.nnz, n, m)
     assert np.array_equal(connectivity.neighbors(A, 0), [0, 1, 2])
     assert np.array_equal(connectivity.neighbors(A, 1), [1, 2, 3])
 
 
 def test_to_ij(triangle_mesh, mixed_mesh):
     faces, fill_value = triangle_mesh
     actual_i, actual_j = connectivity._to_ij(faces, fill_value, invert=False)
@@ -349,14 +350,51 @@
             [3, 5, 4, 2],
         ]
     )
     assert np.array_equal(edge_nodes, expected_edge_nodes)
     assert np.array_equal(face_edges, expected_face_edges)
 
 
+def test_node_node_connectivity():
+    edge_nodes = np.array(
+        [
+            [0, 1],
+            [1, 2],
+            [2, 3],
+            [3, 0],
+            [1, 4],
+            [4, 5],
+            [5, 2],
+            [2, 1],
+        ]
+    )
+    csr = connectivity.node_node_connectivity(edge_nodes)
+    coo = csr.tocoo()
+    actual = np.column_stack([coo.row, coo.col])
+    expected = np.array(
+        [
+            [0, 1],
+            [0, 3],
+            [1, 0],
+            [1, 2],
+            [1, 4],
+            [2, 1],
+            [2, 3],
+            [2, 5],
+            [3, 0],
+            [3, 2],
+            [4, 1],
+            [4, 5],
+            [5, 2],
+            [5, 4],
+        ]
+    )
+    assert np.array_equal(actual, expected)
+
+
 def test_face_face_connectivity():
     edge_faces = np.array(
         [
             [0, -1],
             [0, -1],
             [0, 1],
             [1, -1],
@@ -524,7 +562,53 @@
     )
     assert np.array_equal(actual, ~mask)
 
     a = np.array([False, False, True, False, False])
     actual = connectivity.binary_dilation(con, a)
     expected = np.array([False, True, True, True, False])
     assert np.array_equal(actual, expected)
+
+
+@pytest.fixture(scope="function")
+def dag() -> sparse.csr_matrix:
+    #
+    #    0──►2──►3
+    #    │   ▲
+    #    │   │
+    #    └──►1
+    #
+    i = [0, 1, 0, 2]
+    j = [1, 2, 2, 3]
+    csr = sparse.coo_matrix((j, (i, j)), shape=(4, 4)).tocsr()
+    return csr
+
+
+@pytest.fixture(scope="function")
+def cycle() -> sparse.csr_matrix:
+    # same as dag fixture, but bidirectional
+    i = [0, 1, 0, 2]
+    j = [1, 2, 2, 3]
+    ij = np.concatenate((i, j))
+    ji = np.concatenate((j, i))
+    csr = sparse.coo_matrix((ji, (ij, ji)), shape=(4, 4)).tocsr()
+    return csr
+
+
+def test_topological_sort_by_dfs(dag):
+    actual = connectivity.topological_sort_by_dfs(dag)
+    assert np.array_equal(actual, [0, 1, 2, 3])
+
+
+def test_topological_sort_by_dfs__cycle_error(cycle):
+    with pytest.raises(ValueError, match="The graph contains at least one cycle"):
+        connectivity.topological_sort_by_dfs(cycle)
+
+
+def test_contract_vertices(dag):
+    actual = connectivity.contract_vertices(dag, [0, 1, 3])
+    expected = np.array([[0, 1], [1, 3]])
+    assert np.array_equal(actual, expected)
+
+
+def test_contract_vertices__cycle_error(cycle):
+    with pytest.raises(ValueError, match="The graph contains at least one cycle"):
+        connectivity.contract_vertices(cycle, indices=[1, 3])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xugrid-0.5.0/tests/test_conventions.py` & `xugrid-0.6.0/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_conversion.py` & `xugrid-0.6.0/tests/test_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 
 
 # Cannot use fixtures in parametrize:
 # https://github.com/pytest-dev/pytest/issues/349
 def _faces_geos_roundtrip(mesh):
     x, y, c, fv = mesh
     actual = cv.faces_to_polygons(x, y, c, fv)
-    print(actual)
     x_back, y_back, c_back, fv_back = cv.polygons_to_faces(actual)
     polygons_back = cv.faces_to_polygons(x_back, y_back, c_back, fv_back)
     assert np.array_equal(x, x_back)
     assert np.array_equal(y, y_back)
     assert np.array_equal(c, c_back)
     assert fv == fv_back
     assert np.array_equal(actual, polygons_back)
```

### Comparing `xugrid-0.5.0/tests/test_data.py` & `xugrid-0.6.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_interpolate.py` & `xugrid-0.6.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_meshkernel_utils.py` & `xugrid-0.6.0/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_plot.py` & `xugrid-0.6.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_snap.py` & `xugrid-0.6.0/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/tests/test_ugrid1d.py` & `xugrid-0.6.0/tests/test_ugrid1d.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     assert grid.n_edge == 2
     expected_coords = np.array([[0.0, 0.0], [1.0, 1.0], [2.0, 2.0]])
     assert np.allclose(grid.node_coordinates, expected_coords)
     assert np.allclose(grid.edge_x, [0.5, 1.5])
     assert np.allclose(grid.edge_y, [0.5, 1.5])
     assert np.allclose(grid.edge_coordinates, np.column_stack([[0.5, 1.5], [0.5, 1.5]]))
     assert grid.bounds == (0.0, 0.0, 2.0, 2.0)
-    node_edges = grid.node_edge_connectivity
-    assert isinstance(node_edges, sparse.csr_matrix)
+    assert isinstance(grid.node_edge_connectivity, sparse.csr_matrix)
+    assert isinstance(grid.node_node_connectivity, sparse.csr_matrix)
 
     expected_coords = [
         [[0.0, 0.0], [1.0, 1.0]],
         [[1.0, 1.0], [2.0, 2.0]],
     ]
     actual_coords = grid.edge_node_coordinates
     assert actual_coords.shape == (2, 2, 2)
@@ -317,7 +317,63 @@
     assert np.array_equal(actual.node_y, [1.0, 2.0])
 
 
 def test_ugrid1d_plot():
     grid = grid1d()
     primitive = grid.plot()
     assert isinstance(primitive, LineCollection)
+
+
+def test_ugrid1d_rename():
+    grid = grid1d()
+    original_indexes = grid._indexes.copy()
+    original_attrs = grid._attrs.copy()
+
+    renamed = grid.rename("__renamed")
+
+    # Check that original is unchanged
+    assert grid._attrs == original_attrs
+    assert grid._indexes == original_indexes
+    assert renamed._attrs == {
+        "cf_role": "mesh_topology",
+        "long_name": "Topology data of 1D network",
+        "topology_dimension": 1,
+        "node_dimension": "__renamed_nNodes",
+        "edge_dimension": "__renamed_nEdges",
+        "edge_node_connectivity": "__renamed_edge_nodes",
+        "node_coordinates": "__renamed_node_x __renamed_node_y",
+        "edge_coordinates": "__renamed_edge_x __renamed_edge_y",
+    }
+    assert renamed._indexes == {
+        "node_x": "__renamed_node_x",
+        "node_y": "__renamed_node_y",
+    }
+    assert renamed.name == "__renamed"
+
+
+def test_ugrid1d_rename_with_dataset():
+    grid = grid1d()
+    grid2 = xugrid.Ugrid1d.from_dataset(grid.to_dataset())
+    original_dataset = grid2._dataset.copy()
+
+    renamed2 = grid2.rename("__renamed")
+    dataset = renamed2._dataset
+    assert grid2._dataset.equals(original_dataset)
+    assert sorted(dataset.data_vars) == ["__renamed", "__renamed_edge_nodes"]
+    assert sorted(dataset.dims) == ["__renamed_nEdges", "__renamed_nNodes", "two"]
+    assert sorted(dataset.coords) == ["__renamed_node_x", "__renamed_node_y"]
+
+
+def test_topology_sort_by_dfs():
+    grid = grid1d()
+    vertices = grid.topological_sort_by_dfs()
+    assert isinstance(vertices, np.ndarray)
+    assert np.array_equal(vertices, [0, 1, 2])
+
+
+def test_contract_vertices():
+    grid = grid1d()
+    new = grid.contract_vertices(indices=[0, 2])
+    assert isinstance(new, xugrid.Ugrid1d)
+    assert new.n_node == 2
+    # The nodes have been renumbered
+    assert np.array_equal(new.edge_node_connectivity, [[0, 1]])
```

### Comparing `xugrid-0.5.0/tests/test_ugrid2d.py` & `xugrid-0.6.0/tests/test_ugrid2d.py`

 * *Files 9% similar despite different names*

```diff
@@ -156,16 +156,16 @@
     assert grid.n_node == 7
     assert grid.n_edge == 10
     assert grid.n_face == 4
     assert grid.n_max_node_per_face == 4
     assert np.array_equal(grid.n_node_per_face, [4, 4, 3, 3])
     assert np.allclose(grid.node_coordinates, VERTICES)
     assert grid.bounds == (0.0, 0.0, 2.0, 2.0)
-    node_edges = grid.node_edge_connectivity
-    assert isinstance(node_edges, sparse.csr_matrix)
+    assert isinstance(grid.node_node_connectivity, sparse.csr_matrix)
+    assert isinstance(grid.node_edge_connectivity, sparse.csr_matrix)
     edge_node_coords = grid.edge_node_coordinates
     face_node_coords = grid.face_node_coordinates
     assert edge_node_coords.shape == (10, 2, 2)
     assert face_node_coords.shape == (4, 4, 2)
     are_nan = np.isnan(face_node_coords)
     assert are_nan[2:, -1:, :].all()
     assert not are_nan[:, :-1, :].any()
@@ -945,7 +945,66 @@
     assert isinstance(grid, xugrid.Ugrid2d)
 
 
 def test_ugrid2d_plot():
     grid = grid2d()
     primitive = grid.plot()
     assert isinstance(primitive, LineCollection)
+
+
+def test_ugrid2d_rename():
+    grid = grid2d()
+    original_indexes = grid._indexes.copy()
+    original_attrs = grid._attrs.copy()
+
+    renamed = grid.rename("__renamed")
+
+    # Check that original is unchanged
+    assert grid._attrs == original_attrs
+    assert grid._indexes == original_indexes
+    assert renamed._attrs == {
+        "cf_role": "mesh_topology",
+        "long_name": "Topology data of 2D mesh",
+        "topology_dimension": 2,
+        "node_dimension": "__renamed_nNodes",
+        "edge_dimension": "__renamed_nEdges",
+        "face_dimension": "__renamed_nFaces",
+        "max_face_nodes_dimension": "__renamed_nMax_face_nodes",
+        "boundary_edge_dimension": "__renamed_nBoundary_edges",
+        "edge_node_connectivity": "__renamed_edge_nodes",
+        "face_node_connectivity": "__renamed_face_nodes",
+        "face_edge_connectivity": "__renamed_face_edges",
+        "edge_face_connectivity": "__renamed_edge_faces",
+        "boundary_node_connectivity": "__renamed_boundary_nodes",
+        "face_face_connectivity": "__renamed_face_faces",
+        "node_coordinates": "__renamed_node_x __renamed_node_y",
+        "edge_coordinates": "__renamed_edge_x __renamed_edge_y",
+        "face_coordinates": "__renamed_face_x __renamed_face_y",
+    }
+    assert renamed._indexes == {
+        "node_x": "__renamed_node_x",
+        "node_y": "__renamed_node_y",
+    }
+    assert renamed.name == "__renamed"
+
+
+def test_ugrid2d_rename_with_dataset():
+    grid = grid2d()
+    grid2 = xugrid.Ugrid2d.from_dataset(grid.to_dataset())
+    original_dataset = grid2._dataset.copy()
+
+    renamed2 = grid2.rename("__renamed")
+    dataset = renamed2._dataset
+    assert grid2._dataset.equals(original_dataset)
+    assert sorted(dataset.data_vars) == [
+        "__renamed",
+        "__renamed_edge_nodes",
+        "__renamed_face_nodes",
+    ]
+    assert sorted(dataset.dims) == [
+        "__renamed_nEdges",
+        "__renamed_nFaces",
+        "__renamed_nMax_face_nodes",
+        "__renamed_nNodes",
+        "two",
+    ]
+    assert sorted(dataset.coords) == ["__renamed_node_x", "__renamed_node_y"]
```

### Comparing `xugrid-0.5.0/tests/test_ugrid_dataset.py` & `xugrid-0.6.0/tests/test_ugrid_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pyproj
 import pytest
 import shapely
 import xarray as xr
@@ -245,14 +247,21 @@
         da = xr.DataArray(np.empty((4, 4)), {"y": y, "x": x}, ["y", "x"])
         actual = self.uda.ugrid.rasterize_like(other=da)
         assert isinstance(actual, xr.DataArray)
         assert actual.shape == (4, 4)
         assert np.allclose(actual["x"], x)
         assert np.allclose(actual["y"], y)
 
+    def test_partitioning(self):
+        partitions = self.uda.ugrid.partition(n_part=2)
+        assert len(partitions) == 2
+        for partition in partitions:
+            assert isinstance(partition, xugrid.UgridDataArray)
+            assert partition.name == self.uda.name
+
     def test_crs(self):
         uda = self.uda
         crs = uda.ugrid.crs
         assert crs == {"mesh2d": None}
 
         uda.ugrid.set_crs(epsg=28992)
         assert uda.ugrid.crs == {"mesh2d": pyproj.CRS.from_epsg(28992)}
@@ -353,14 +362,25 @@
         ):
             self.uda.ugrid.assign_node_coords()
 
         with_coords = self.uda.ugrid.assign_face_coords()
         assert "mesh2d_face_x" in with_coords.coords
         assert "mesh2d_face_y" in with_coords.coords
 
+    def test_plot_with_chunks(self, tmp_path):
+        time = xr.DataArray([0.0, 1.0, 2.0], coords={"time": [0, 1, 2]})
+        uda = (self.uda * time).transpose()
+        uda.name = "test"
+
+        path = tmp_path / "test.nc"
+        uda.ugrid.to_netcdf(path)
+        back = xugrid.open_dataarray(path, chunks={"time": 1})
+        primitive = back.isel(time=0).ugrid.plot()
+        assert primitive is not None
+
 
 class TestUgridDataset:
     @pytest.fixture(autouse=True)
     def setup(self):
         ds = xr.Dataset()
         ds["a"] = DARRAY()
         ds["b"] = DARRAY() * 2
@@ -508,14 +528,22 @@
         actual = self.uds.ugrid.rasterize_like(other=da)
         assert isinstance(actual, xr.Dataset)
         assert actual["a"].shape == (4, 4)
         assert actual["b"].shape == (4, 4)
         assert np.allclose(actual["x"], x)
         assert np.allclose(actual["y"], y)
 
+    def test_partitioning(self):
+        partitions = self.uds.ugrid.partition(n_part=2)
+        assert len(partitions) == 2
+        for partition in partitions:
+            assert isinstance(partition, xugrid.UgridDataset)
+            assert "a" in partition
+            assert "b" in partition
+
     def test_crs(self):
         uds = self.uds
         crs = uds.ugrid.crs
         assert crs == {"mesh2d": None}
 
         with pytest.raises(ValueError, match="grid not found"):
             uds.ugrid.set_crs(epsg=28992, topology="grid")
@@ -602,15 +630,14 @@
     attrs["node_coordinates"] += " mesh2d_node_lon mesh2d_node_lat"
     ds = ds.assign_coords(
         mesh2d_node_lon=(grid.node_dimension, np.arange(grid.n_node)),
         mesh2d_node_lat=(grid.node_dimension, np.arange(grid.n_node)),
     )
     ds["mesh2d_node_lon"].attrs["standard_name"] = "longitude"
     ds["mesh2d_node_lat"].attrs["standard_name"] = "latitude"
-    print(ds.ugrid_roles.coordinates)
     assert ds.ugrid_roles.coordinates == {
         "mesh2d": {
             "node_coordinates": (
                 ["mesh2d_node_x", "mesh2d_node_lon"],
                 ["mesh2d_node_y", "mesh2d_node_lat"],
             )
         }
@@ -654,14 +681,25 @@
     back = xugrid.open_dataset(path)
     assert isinstance(back, xugrid.UgridDataset)
     assert "b" in back
     assert "mesh2d_face_nodes" in back.ugrid.grids[0].to_dataset()
     assert "mesh2d_face_nodes" not in back.ugrid.obj
 
 
+def test_open_dataset_cast_invalid(tmp_path):
+    grid = GRID()
+    vorgrid = grid.tesselate_centroidal_voronoi()
+    path = tmp_path / "voronoi-grid.nc"
+    vorgrid.to_dataset().to_netcdf(path)
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        xugrid.open_dataset(path)
+
+
 def test_open_dataarray_roundtrip(tmp_path):
     path = tmp_path / "ugrid-dataset.nc"
     uds = xugrid.UgridDataset(UGRID_DS())
     uds.ugrid.to_netcdf(path)
     with pytest.raises(ValueError, match="Given file dataset contains more than one"):
         xugrid.open_dataarray(path)
```

### Comparing `xugrid-0.5.0/tests/test_voronoi.py` & `xugrid-0.6.0/tests/test_voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/__init__.py` & `xugrid-0.6.0/xugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/constants.py` & `xugrid-0.6.0/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/conversion.py` & `xugrid-0.6.0/xugrid/conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/core/accessorbase.py` & `xugrid-0.6.0/xugrid/core/accessorbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
-from typing import Tuple
+from typing import Tuple, Union
 
 import numpy as np
 import xarray as xr
 
+import xugrid
+
 
 class AbstractUgridAccessor(abc.ABC):
     @abc.abstractmethod
     def to_dataset():
         """ """
 
     @abc.abstractmethod
@@ -92,14 +94,50 @@
 
         -------
         clipped:
             xugrid.UgridDataArray or xugrid.UgridDataset
         """
         return self.sel(x=slice(xmin, xmax), y=slice(ymin, ymax))
 
+    def partition_by_label(
+        self, labels: np.ndarray
+    ) -> Union["xugrid.UgridDataArray", "xugrid.UgridDataset"]:
+        """
+        Partition a grid by labels.
+
+        Parameters
+        ----------
+        labels: np.ndarray of integers labeling each face.
+
+        Returns
+        -------
+        partitioned: list of partitions
+        """
+        from xugrid.ugrid import partitioning
+
+        return partitioning.partition_by_label(self.grid, self.obj, labels)
+
+    def partition(
+        self, n_part: int
+    ) -> Union["xugrid.UgridDataArray", "xugrid.UgridDataset"]:
+        """
+        Partition a grid into a given number of parts.
+
+        Parameters
+        ----------
+        n_part: integer
+            The number of parts to partition the mesh.
+
+        Returns
+        -------
+        partitioned: list of partitions
+        """
+        labels = self.grid.label_partitions(n_part)
+        return self.partition_by_label(labels)
+
     def to_netcdf(self, *args, **kwargs):
         """
         Write dataset contents to a UGRID compliant netCDF file.
 
         This function wraps :py:meth:`xr.Dataset.to_netcdf`; it adds the UGRID
         variables and coordinates to a standard xarray Dataset, then writes the
         result to a netCDF.
```

### Comparing `xugrid-0.5.0/xugrid/core/common.py` & `xugrid-0.6.0/xugrid/core/common.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/core/dataarray_accessor.py` & `xugrid-0.6.0/xugrid/core/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/core/dataset_accessor.py` & `xugrid-0.6.0/xugrid/core/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/core/wrap.py` & `xugrid-0.6.0/xugrid/core/wrap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/data/sample_data.py` & `xugrid-0.6.0/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/data/synthetic.py` & `xugrid-0.6.0/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/meshkernel_utils.py` & `xugrid-0.6.0/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/plot/plot.py` & `xugrid-0.6.0/xugrid/plot/plot.py`

 * *Files identical despite different names*

```diff
@@ -584,14 +584,16 @@
     Parameters
     ----------
     darray : DataArray
     grid: Union[Ugrid1d, Ugrid2d]
     **kwargs : optional
         Additional keyword arguments for Matplotlib.
     """
+    darray = darray.squeeze().compute()
+
     dim = darray.dims[0]
     kwargs["ax"] = ax
     if grid.topology_dimension == 1:
         if dim == grid.edge_dimension:
             return line(grid, darray, **kwargs)
         elif dim == grid.node_dimension:
             return scatter(grid, darray, **kwargs)
```

### Comparing `xugrid-0.5.0/xugrid/regrid/overlap_1d.py` & `xugrid-0.6.0/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/regrid/reduce.py` & `xugrid-0.6.0/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/regrid/regridder.py` & `xugrid-0.6.0/xugrid/regrid/regridder.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,19 +50,21 @@
                 if len(indices) > 0:
                     out[extra_index, target_index] = f(source_flat, indices, weights)
         return out
 
     return numba.njit(_regrid, parallel=True, cache=True)
 
 
-def setup_grid(obj):
+def setup_grid(obj, **kwargs):
     if isinstance(obj, (xu.Ugrid2d, xu.UgridDataArray, xu.UgridDataset)):
         return UnstructuredGrid2d(obj)
     elif isinstance(obj, (xr.DataArray, xr.Dataset)):
-        return StructuredGrid2d(obj, name_y="y", name_x="x")
+        return StructuredGrid2d(
+            obj, name_y=kwargs.get("name_y", "y"), name_x=kwargs.get("name_x", "x")
+        )
     else:
         raise TypeError()
 
 
 def convert_to_match(source, target):
     PROMOTIONS = {
         frozenset({StructuredGrid2d}): StructuredGrid2d,
@@ -116,24 +118,22 @@
         else:
             raise TypeError(
                 f"method must be string or callable, received: {type(func).__name}"
             )
         return
 
     def _regrid_array(self, source):
-        if hasattr(self, "_source"):
-            source_grid = self._source
-        else:
-            source_grid = source
+        source_grid = self._source
         first_dims_shape = source.shape[: -source_grid.ndim]
 
-        # The regridding can be mapped over additional dimensions (e.g. for every time slice).
-        # This is the `extra_index` iteration in _regrid().
-        # But it should work consistently even if no additional present: in that case we create
-        # a 1-sized additional dimension in front, so the `extra_index` iteration always applies.
+        # The regridding can be mapped over additional dimensions, e.g. for
+        # every time slice. This is the `extra_index` iteration in _regrid().
+        # But it should work consistently even if no additional present: in
+        # that case we create a 1-sized additional dimension in front, so the
+        # `extra_index` iteration always applies.
         if source.ndim == source_grid.ndim:
             source = source[np.newaxis]
 
         # All additional dimension are flattened into one, in front.
         # E.g.:
         #
         #   * ("dummy", "face") -> ("dummy", "face")
@@ -218,63 +218,82 @@
                 self._target.ugrid_topology,
             )
 
     def to_dataset(self) -> xr.Dataset:
         """
         Store the computed weights and target in a dataset for re-use.
         """
-        ds = xr.Dataset(
+        weights_ds = xr.Dataset(
             {f"__regrid_{k}": v for k, v in zip(self._weights._fields, self._weights)}
         )
-        ugrid_ds = self._target.ugrid_topology.to_dataset()
-        return xr.merge((ds, ugrid_ds))
+        source_ds = self._source.to_dataset("__source")
+        target_ds = self._target.to_dataset("__target")
+        return xr.merge((weights_ds, source_ds, target_ds))
 
     @staticmethod
     def _csr_from_dataset(dataset: xr.Dataset) -> WeightMatrixCSR:
+        """
+        variable n and nnz are expected to be scalar variable
+        """
         return WeightMatrixCSR(
             dataset["__regrid_data"].values,
             dataset["__regrid_indices"].values,
             dataset["__regrid_indptr"].values,
-            dataset["__regrid_n"].values,
-            dataset["__regrid_nnz"].values,
+            dataset["__regrid_n"].values[()],
+            dataset["__regrid_nnz"].values[()],
         )
 
     @staticmethod
     def _coo_from_dataset(dataset: xr.Dataset) -> WeightMatrixCOO:
+        """
+        variable nnz is expected to be scalar variable
+        """
         return WeightMatrixCOO(
             dataset["__regrid_data"].values,
             dataset["__regrid_row"].values,
             dataset["__regrid_col"].values,
-            dataset["__regrid_nnz"].values,
+            dataset["__regrid_nnz"].values[()],
         )
 
     @abc.abstractclassmethod
     def _weights_from_dataset(
         cls, dataset: xr.Dataset
     ) -> Union[WeightMatrixCOO, WeightMatrixCSR]:
         """
         Return either COO or CSR weights.
         """
 
     @classmethod
-    def from_weights(cls, weights, target: "xugrid.Ugrid2d"):
+    def from_weights(
+        cls, weights, target: Union["xugrid.Ugrid2d", xr.DataArray, xr.Dataset]
+    ):
         instance = cls.__new__(cls)
-        instance._weights = weights
-        instance._target = UnstructuredGrid2d(target)
+        instance._weights = cls._weights_from_dataset(weights)
+        instance._target = setup_grid(target)
+        unstructured = weights["__source_type"].attrs["type"] == "UnstructuredGrid2d"
+        if unstructured:
+            instance._source = setup_grid(xu.Ugrid2d.from_dataset(weights, "__source"))
+        else:
+            instance._source = setup_grid(
+                weights, name_x="__source_x", name_y="__source_y"
+            )
         return instance
 
     @classmethod
     def from_dataset(cls, dataset: xr.Dataset):
         """
         Reconstruct the regridder from a dataset with source, target indices
         and weights.
         """
-        target = xu.Ugrid2d.from_dataset(dataset)
-        weights = cls._weights_from_dataset(dataset)
-        return cls.from_weights(weights, target)
+        unstructured = dataset["__target_type"].attrs["type"] == "UnstructuredGrid2d"
+        if unstructured:
+            target = xu.Ugrid2d.from_dataset(dataset, "__target")
+
+        # weights = cls._weights_from_dataset(dataset)
+        return cls.from_weights(dataset, target)
 
 
 class CentroidLocatorRegridder(BaseRegridder):
     """
     The CentroidLocatorRegridded regrids by searching the source grid for the
     centroids of the target grid.
 
@@ -303,15 +322,15 @@
             source_flat = source[extra_index]
             for target_index, source_index in zip(A.row, A.col):
                 out[extra_index, target_index] = source_flat[source_index]
         return out
 
     @property
     def weights(self):
-        return self._weights
+        return self.to_dataset()
 
     @weights.setter
     def weights(self, weights: WeightMatrixCOO, target: "xugrid.Ugrid2d"):
         if not isinstance(weights, WeightMatrixCOO):
             raise TypeError(
                 f"Expected WeightMatrixCOO, received: {type(weights).__name__}"
             )
@@ -330,15 +349,15 @@
             target, relative=relative
         )
         self._weights = weight_matrix_csr(source_index, target_index, weight_values)
         return
 
     @property
     def weights(self):
-        return self._weights
+        return self.to_dataset()
 
     @weights.setter
     def weights(self, weights: WeightMatrixCSR):
         if not isinstance(weights, WeightMatrixCSR):
             raise TypeError(
                 f"Expected WeightMatrixCSR, received: {type(weights).__name__}"
             )
@@ -394,16 +413,16 @@
 
     def _compute_weights(self, source, target) -> None:
         super()._compute_weights(source, target, relative=False)
 
     @classmethod
     def from_weights(
         cls,
-        weights: WeightMatrixCSR,
-        target: "xugrid.Ugrid2d",
+        weights: xr.Dataset,
+        target: Union["xugrid.Ugrid2d", xr.DataArray, xr.Dataset],
         method: Union[str, Callable] = "mean",
     ):
         instance = super().from_weights(weights, target)
         instance._setup_regrid(method)
         return instance
 
 
@@ -493,15 +512,15 @@
         else:
             source_index, target_index, weights = source.barycentric(target)
         self._weights = weight_matrix_csr(source_index, target_index, weights)
         return
 
     @property
     def weights(self):
-        return self._weights
+        return self.to_dataset()
 
     @weights.setter
     def weights(self, weights: WeightMatrixCSR):
         if not isinstance(weights, WeightMatrixCSR):
             raise TypeError(
                 f"Expected WeightMatrixCSR, received: {type(weights).__name__}"
             )
```

### Comparing `xugrid-0.5.0/xugrid/regrid/structured.py` & `xugrid-0.6.0/xugrid/regrid/structured.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 This module contains the logic for regridding from a structured form to another
 structured form. All coordinates are assumed to be fully orthogonal to each
 other.
 
 While the unstructured logic would work for structured data as well, it is much
 less efficient than utilizing the structure of the coordinates.
 """
-from typing import Union
+from typing import Any, Tuple, Union
 
 import numpy as np
 import xarray as xr
 
+from xugrid.constants import FloatArray, IntArray
 from xugrid.regrid.overlap_1d import overlap_1d, overlap_1d_nd
 from xugrid.regrid.unstructured import UnstructuredGrid2d
 from xugrid.regrid.utils import broadcast
 from xugrid.ugrid.ugrid2d import Ugrid2d
 
 # from xugrid import Ugrid2d
 
@@ -25,16 +26,15 @@
 
     Parameters
     ----------
     bounds: (n, 2)
     """
 
     def __init__(self, obj: Union[xr.DataArray, xr.Dataset], name: str):
-        bounds_name_left = f"{name}bounds_left"  # e.g. xbounds
-        bounds_name_right = f"{name}bounds_right"  # e.g. xbounds
+        bounds_name = f"{name}bounds"  # e.g. xbounds
         size_name = f"d{name}"  # e.g. dx
 
         index = obj.indexes[name]
         # take care of potentially decreasing coordinate values
         if index.is_monotonic_decreasing:
             midpoints = index.values[::-1]
             flipped = True
@@ -42,18 +42,16 @@
         elif index.is_monotonic_increasing:
             midpoints = index.values
             flipped = False
             side = "left"
         else:
             raise ValueError(f"{name} is not monotonic for array {obj.name}")
 
-        if bounds_name_left in obj.coords:
-            start = obj[bounds_name_left].values
-            end = obj[bounds_name_right].values
-            bounds = np.column_stack((start, end))
+        if bounds_name in obj.coords:
+            bounds = obj[bounds_name].values
         else:
             if size_name in obj.coords:
                 # works for scalar size and array size
                 size = np.abs(obj[size_name].values)
             else:
                 # no bounds defined, no dx defined
                 # make an estimate of cell size
@@ -75,287 +73,342 @@
         self.midpoints = midpoints
         self.bounds = bounds
         self.flipped = flipped
         self.side = side
         self.grid = obj
 
     @property
-    def ndim(self):
+    def ndim(self) -> int:
         return 1
 
     @property
-    def dims(self):
+    def dims(self) -> Tuple[str]:
         return (self.name,)
 
     @property
-    def size(self):
+    def size(self) -> int:
         return len(self.bounds)
 
     @property
-    def length(self):
+    def length(self) -> FloatArray:
         return abs(np.diff(self.bounds, axis=1))
 
-    def flip_if_needed(self, index):
+    def flip_if_needed(self, index: IntArray) -> IntArray:
         if self.flipped:
             return self.size - index - 1
         else:
             return index
 
-    def valid_nodes_within_bounds(self, other):
+    def valid_nodes_within_bounds(
+        self, other: "StructuredGrid1d"
+    ) -> Tuple[IntArray, IntArray]:
         """
         Retruns nodes when midpoints are within bounding box of overlaying grid.
         In cases that midpoints (and bounding boxes) are flipped, computed indexes
         are fliped as well.
 
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-
-        Returns:
-            valid_self_index (np.array): valid source indexes
-            valid_other_index (np.array): valid target indexes
+        Parameters
+        ----------
+        other: StructuredGrid1d
+            The target grid topology
+
+        Returns
+        -------
+        valid_self_index: np.array
+            valid source indexes
+        valid_other_index: np.array
+            valid target indexes
         """
         start = np.searchsorted(self.bounds[:, 0], other.midpoints, side=self.side)
         end = np.searchsorted(self.bounds[:, 1], other.midpoints, side=self.side)
         valid = (
             (start == (end + 1))
             & (other.midpoints > self.bounds[0, 0])
             & (other.midpoints < self.bounds[-1, 1])
         )
         valid_other_index = np.arange(other.size)[valid]
         valid_self_index = end[valid]
         valid_self_index = self.flip_if_needed(valid_self_index)
         valid_other_index = other.flip_if_needed(valid_other_index)
         return valid_self_index, valid_other_index
 
-    def valid_nodes_within_bounds_and_extend(self, other):
-        """
-        returns all valid nodes for linear interpolation. In addition to valid_nodes_within_bounds()
-        is checked if target midpoints are not outside outer source boundary midpoints. In that case
-        there is no interpolation possible.
-
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-
-        Returns:
-            valid_self_index (np.array): valid source indexes
-            valid_other_index (np.array): valid target indexes
+    def valid_nodes_within_bounds_and_extend(
+        self, other: "StructuredGrid1d"
+    ) -> Tuple[IntArray, IntArray]:
+        """
+        Returns all valid nodes for linear interpolation. In addition to
+        valid_nodes_within_bounds() is checked if target midpoints are not
+        outside outer source boundary midpoints. In that case there is no
+        interpolation possible.
+
+        Parameters
+        ----------
+        other: StructuredGrid1d
+            The target grid.
+
+        Returns
+        -------
+        valid_self_index: np.array
+            valid source indexes
+        valid_other_index: np.array
+            valid target indexes
         """
         source_index, target_index = self.valid_nodes_within_bounds(other)
         valid = (other.midpoints[target_index] > self.midpoints[0]) & (
             (other.midpoints[target_index] < self.midpoints[-1])
         )
         return source_index[valid], target_index[valid]
 
-    def overlap_1d_structured(self, other):
+    def overlap_1d_structured(
+        self, other: "StructuredGrid1d"
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns source and target nodes and overlapping length. It utilises overlap_1d()
         and does an aditional flip in cases of reversed midpoints
 
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-
-        Returns:
-            valid_self_index (np.array): valid source indexes
-            valid_other_index (np.array): valid target indexes
-            weights (np.array): length of overlap
+        Parameters
+        ----------
+        other: StructuredGrid1d
+            The target grid.
+
+        Returns
+        -------
+        valid_self_index: np.array
+            valid source indexes
+        valid_other_index: np.array
+            valid target indexes
+        weights: np.array
+            length of overlap
         """
         source_index, target_index, weights = overlap_1d(self.bounds, other.bounds)
         source_index = self.flip_if_needed(source_index)
         target_index = other.flip_if_needed(target_index)
         return source_index, target_index, weights
 
     def centroids_to_linear_sets(
         self,
-        other,
         source_index: np.array,
         target_index: np.array,
         weights: np.array,
         neighbour: np.array,
-    ):
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
         """
-        Returns for every target node an pair of connected source nodes based on
-        centroids connection inputs
+        Returns for every target node an pair of connected source nodes based
+        on centroids connection inputs.
+
+        Parameters
+        ----------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
 
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-            source_index (np.array): source index (centroids)
-            target_index (np.array): target index (centroids)
-            weights (np.array): weights (centroids)
-
-        Returns:biliniar
-
-            source_index (np.array): source index (linear)
-            target_index (np.array): target index (linear)
-            weights (np.array): weights (linear)
+        Returns
+        -------
+        valid_self_index: np.array
+        valid_other_index: np.array
+        weights: np.array
+            lineair interpolation weights.
         """
-        # if source_index is flipped, source-index is decreasing and neighbour need to be flipped
+        # if source_index is flipped, source-index is decreasing and neighbour
+        # need to be flipped
         if self.flipped:
             neighbour = -neighbour
         source_index = np.column_stack((source_index, source_index + neighbour)).ravel()
         target_index = np.repeat(target_index, 2)
         weights = np.column_stack((weights, 1.0 - weights)).ravel()
 
-        # correct for possibility of out of bound due to column-stack source_index + 1 and -1
+        # correct for possibility of out of bound due to column-stack
+        # source_index + 1 and -1
         valid = np.logical_and(source_index <= self.size - 1, source_index >= 0)
         return source_index[valid], target_index[valid], weights[valid]
 
-    def get_midpoint_index(self, array_index):
+    def maybe_reverse_index(self, index: IntArray) -> IntArray:
         """
-        Returns midpoint array indexes for given array_index.
-
-        Args:
-            array_index (np.array): array_index
+        Flips the index if needed for descending coordinates.
 
-        Returns:biliniar
-            midpoint_index (np.array): midpoint_index
+        Parameters
+        ----------
+        index: np.ndarray
 
+        Returns
+        -------
+        checked_index: np.ndarray
         """
         if self.flipped:
-            return self.size - array_index - 1
+            return self.size - index - 1
         else:
-            return array_index
-
-    def compute_distance_to_centroids(self, other, source_index, target_index):
-        """
-        computes linear weights bases on centroid indexes.
-
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-            other (_type_): _description_
-            source_index (np.array): source index (centroids)
-            target_index (np.array): target index (centroids)
+            return index
 
-        Raises:
-            ValueError: for not enought midpoints
+    def compute_linear_weights_to_centroids(
+        self, other: "StructuredGrid1d", source_index: IntArray, target_index: IntArray
+    ) -> Tuple[FloatArray, IntArray]:
+        """
+        Computes linear weights bases on centroid indexes.
+
+        Parameters
+        ----------
+        other: StructuredGrid1d
+        source_index: np.array
+        target_index: np.array
+
+        Raises
+        ------
+        ValueError
+            When the coordinate contains only a single point.
 
-        Returns:
-            weights (np.array): weights
+        Returns
+        -------
+        weights: np.array
+        neighbor: np.narray
         """
-
-        source_midpoint_index = self.get_midpoint_index(source_index)
-        target_midpoints_index = other.get_midpoint_index(target_index)
-        neighbour = np.ones(target_midpoints_index.size, dtype=int)
-        # cases where midpoint target < midpoint source
+        source_midpoint_index = self.maybe_reverse_index(source_index)
+        target_midpoints_index = other.maybe_reverse_index(target_index)
+        neighbor = np.ones(target_midpoints_index.size, dtype=int)
+        # cases where midpoint target <= midpoint source
         condition = (
             other.midpoints[target_midpoints_index]
-            < self.midpoints[source_midpoint_index]
+            <= self.midpoints[source_midpoint_index]
         )
-        neighbour[condition] = -neighbour[condition]
+        neighbor[condition] = -neighbor[condition]
 
-        if not self.midpoints.size > 2:
+        if self.midpoints.size < 2:
             raise ValueError(
-                "source index must larger than 2. Cannot interpolate with one point"
+                f"Coordinate {self.name} has size: {self.midpoints.size}. "
+                "At least two points are required for interpolation."
+            )
+        weights = 1 - (
+            (
+                other.midpoints[target_midpoints_index]
+                - self.midpoints[source_midpoint_index]
+            )
+            / (
+                self.midpoints[source_midpoint_index + neighbor]
+                - self.midpoints[source_midpoint_index]
             )
-        weights = (
-            other.midpoints[target_midpoints_index]
-            - self.midpoints[source_midpoint_index]
-        ) / (
-            self.midpoints[source_midpoint_index + neighbour]
-            - self.midpoints[source_midpoint_index]
         )
-        weights[weights < 0.0] = 0.0
-        weights[weights > 1.0] = 1.0
-
-        return weights, neighbour
+        condition = np.logical_and(weights < 0.0, weights > 1.0)
+        if condition.any():
+            raise ValueError(
+                f"Computed invalid weights for dimensions: {self.name} at coords: {self.midpoints[condition]}"
+            )
+        return weights, neighbor
 
     def sorted_output(
-        self, source_index: np.array, target_index: np.array, weights: np.array
-    ):
+        self, source_index: IntArray, target_index: IntArray, weights: FloatArray
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
         """
-        Returns sorted input based on target index. The regridder needs input sorted on
-        row index of WeightMatrixCOO (target index)
+        Returns sorted input based on target index. The regridder needs input
+        sorted on row index of WeightMatrixCOO (target index).
+
+        Parameters
+        ----------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
 
-        Args:
-            source_index (np.array): source index
-            target_index (np.array): target index
-            weights (np.array): weights
-
-        Returns:
-            source_index (np.array): source index
-            target_index (np.array): target index
-            weights (np.array): weights
+        Returns
+        -------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
         """
         sorter_target = np.argsort(target_index)
         return (
             source_index[sorter_target],
             target_index[sorter_target],
             weights[sorter_target],
         )
 
-    def overlap(self, other: "StructuredGrid1d", relative: bool):
+    def overlap(
+        self, other: "StructuredGrid1d", relative: bool
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns source and target indexes and overlapping length
 
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-            relative (bool): overlapping length target relative to source length
-
-        Returns:
-            source_index (np.array): source indexes
-            target_index (np.array): target indexes
-            weights (np.array): overlapping length
+        Parameters
+        ----------
+        other: StructuredGrid1d
+        relative: bool
+            Overlapping length target relative to source length
+
+        Returns
+        -------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
+            Overlapping length
         """
         source_index, target_index, weights = self.overlap_1d_structured(other)
         if relative:
             weights /= self.length()[source_index]
         return self.sorted_output(source_index, target_index, weights)
 
-    def locate_centroids(self, other: "StructuredGrid1d"):
-        """
-        Returns source and target indexes based on nearest neighbor of centroids
+    def locate_centroids(
+        self, other: "StructuredGrid1d"
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
+        """
+        Returns source and target indexes based on nearest neighbor of
+        centroids.
+
+        Parameters
+        ----------
+        other: StructuredGrid1d
 
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
-
-        Returns:
-            source_index (np.array): source indexes
-            target_index (np.array): target indexes
-            weights (np.array): array of ones
+        Returns
+        -------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
         """
         source_index, target_index = self.valid_nodes_within_bounds(other)
         weights = np.ones(source_index.size, dtype=float)
         return self.sorted_output(source_index, target_index, weights)
 
-    def linear_weights(self, other: "StructuredGrid1d"):
-        """
-        Returns linear source and target indexes and corresponding weights
-
-        Args:
-            self (StructuredGrid1d): source grid
-            other (StructuredGrid1d): target grid
+    def linear_weights(
+        self, other: "StructuredGrid1d"
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
+        """
+        Returns linear source and target indexes and corresponding weights.
+
+        Parameters
+        ----------
+        other: StructuredGrid1d
 
-        Raises:
-            ValueError: when number of nodes is to small to compute linear weights
-
-        Returns:
-            source_index (np.array): overlaying self indexes
-            target_index (np.array): overlaying other indexes
-            weights (np.array): array linear weights
+        Returns
+        -------
+        source_index: np.array
+        target_index: np.array
+        weights: np.array
         """
-
         source_index, target_index = self.valid_nodes_within_bounds_and_extend(other)
-        weights, neighbour = self.compute_distance_to_centroids(
+        weights, neighbour = self.compute_linear_weights_to_centroids(
             other, source_index, target_index
         )
         source_index, target_index, weights = self.centroids_to_linear_sets(
-            other,
             source_index,
             target_index,
             weights,
             neighbour,
         )
         return self.sorted_output(source_index, target_index, weights)
 
+    def to_dataset(self, name: str) -> xr.DataArray:
+        export_name = name + "_" + self.name
+        return xr.DataArray(
+            name=name,
+            data=np.nan,
+            dims=[export_name, export_name + "nbounds"],
+            coords={
+                export_name: self.midpoints,
+                export_name
+                + "bounds": ([export_name, export_name + "nbounds"], self.bounds),
+                export_name + "nbounds": np.arange(2),
+            },
+        )
+
 
 class StructuredGrid2d(StructuredGrid1d):
     """
     e.g. (x,y) -> (x,y)
     """
 
     def __init__(
@@ -364,64 +417,64 @@
         name_x: str,
         name_y: str,
     ):
         self.xbounds = StructuredGrid1d(obj, name_x)
         self.ybounds = StructuredGrid1d(obj, name_y)
 
     @property
-    def ndim(self):
+    def ndim(self) -> int:
         return 2
 
     @property
-    def dims(self):
+    def dims(self) -> Tuple[str, str]:
         return self.ybounds.dims + self.xbounds.dims  # ("y", "x")
 
     @property
-    def size(self):
+    def size(self) -> int:
         return self.ybounds.size * self.xbounds.size
 
     @property
-    def shape(self):
+    def shape(self) -> Tuple[int, int]:
         return (self.ybounds.size, self.xbounds.size)
 
     @property
-    def area(self):
+    def area(self) -> FloatArray:
         return np.multiply.outer(self.ybounds.length, self.xbounds.length)
 
-    def convert_to(self, matched_type):
+    def convert_to(self, matched_type: Any) -> Any:
         if isinstance(self, matched_type):
             return self
         elif isinstance(self, UnstructuredGrid2d):
             return Ugrid2d.from_structured(self.xbounds, self.ybounds)
         else:
             raise TypeError(
                 f"Cannot convert StructuredGrid2d to {matched_type.__name__}"
             )
 
     def broadcast_sorted(
         self,
-        other,
-        source_index_y: np.array,
-        source_index_x: np.array,
-        target_index_y: np.array,
-        target_index_x: np.array,
-        weights_y: np.array,
-        weights_x: np.array,
-    ):
+        other: Any,
+        source_index_y: IntArray,
+        source_index_x: IntArray,
+        target_index_y: IntArray,
+        target_index_x: IntArray,
+        weights_y: FloatArray,
+        weights_x: FloatArray,
+    ) -> Tuple[IntArray, IntArray, FloatArray]:
         source_index, target_index, weights = broadcast(
             self.shape,
             other.shape,
             (source_index_y, source_index_x),
             (target_index_y, target_index_x),
             (weights_y, weights_x),
         )
         sorter = np.argsort(target_index)
         return source_index[sorter], target_index[sorter], weights[sorter]
 
-    def overlap(self, other, relative: bool):
+    def overlap(self, other, relative: bool) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns
         -------
         source_index: 1d np.ndarray of int
         target_index: 1d np.ndarray of int
         weights: 1d np.ndarray of float
         """
@@ -437,15 +490,15 @@
             source_index_x,
             target_index_y,
             target_index_x,
             weights_y,
             weights_x,
         )
 
-    def locate_centroids(self, other):
+    def locate_centroids(self, other) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns
         -------
         source_index: 1d np.ndarray of int
         target_index: 1d np.ndarray of int
         weights: 1d np.ndarray of float
         """
@@ -461,15 +514,15 @@
             source_index_x,
             target_index_y,
             target_index_x,
             weights_y,
             weights_x,
         )
 
-    def linear_weights(self, other):
+    def linear_weights(self, other) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns
         -------
         source_index: 1d np.ndarray of int
         target_index: 1d np.ndarray of int
         weights: 1d np.ndarray of float
         """
@@ -485,14 +538,21 @@
             source_index_x,
             target_index_y,
             target_index_x,
             weights_y,
             weights_x,
         )
 
+    def to_dataset(self, name: str) -> xr.Dataset:
+        ds_x = self.xbounds.to_dataset(name)
+        ds_y = self.ybounds.to_dataset(name)
+        ds = xr.merge([ds_x, ds_y])
+        ds[name + "_type"] = xr.DataArray(-1, attrs={"type": "StructuredGrid2d"})
+        return ds
+
 
 class StructuredGrid3d:
     """
     e.g. (x,y,z) -> (x,y,z)
 
     A voxel model (GeoTOP)
     """
```

### Comparing `xugrid-0.5.0/xugrid/regrid/unstructured.py` & `xugrid-0.6.0/xugrid/regrid/unstructured.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import xarray as xr
 
 import xugrid as xu
 from xugrid.constants import FloatDType
 from xugrid.ugrid import voronoi
 from xugrid.ugrid.ugrid2d import Ugrid2d
 
 
@@ -134,7 +135,12 @@
         # Combine first and second
         source_index = np.concatenate((source_index, other_source))
         target_index = np.concatenate((target_index, other_target))
         weights = np.concatenate((weights, np.ones(other_target.size, dtype=float)))
 
         order = np.argsort(target_index)
         return source_index[order], target_index[order], weights[order]
+
+    def to_dataset(self, name: str):
+        ds = self.ugrid_topology.rename(name).to_dataset()
+        ds[name + "_type"] = xr.DataArray(-1, attrs={"type": "UnstructuredGrid2d"})
+        return ds
```

### Comparing `xugrid-0.5.0/xugrid/regrid/utils.py` & `xugrid-0.6.0/xugrid/regrid/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/regrid/weight_matrix.py` & `xugrid-0.6.0/xugrid/regrid/weight_matrix.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/ugrid/conventions.py` & `xugrid-0.6.0/xugrid/ugrid/conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/ugrid/interpolate.py` & `xugrid-0.6.0/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid/ugrid/partitioning.py` & `xugrid-0.6.0/xugrid/ugrid/partitioning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,82 @@
 """
 Create and merge partitioned UGRID topologies.
 """
 from collections import defaultdict
 from itertools import accumulate
+from typing import List
 
 import numpy as np
 import xarray as xr
 
-from xugrid.constants import IntDType
+from xugrid.constants import IntArray, IntDType
 from xugrid.core.wrap import UgridDataArray, UgridDataset
 from xugrid.ugrid.connectivity import renumber
 
 
-def partition_by_label(xugrid_obj, labels):
+def labels_to_indices(labels: IntArray) -> List[IntArray]:
+    """
+    Convert a 1D array of N labels into a N arrays of indices.
+
+    E.g. [0, 1, 0, 2, 2] -> [[0, 2], [1], [3, 4]]
+    """
+    sorter = np.argsort(labels)
+    split_indices = np.cumsum(np.bincount(labels)[:-1])
+    indices = np.split(sorter, split_indices)
+    for index in indices:
+        index.sort()
+    return indices
+
+
+def partition_by_label(grid, obj, labels: IntArray):
+    """
+    This function is used by UgridDataArray.partition_by_label and
+    UgridDataset.partition_by_label.
+
+    Parameters
+    ----------
+    grid: Ugrid1d, Ugrid2d
+    obj: DataArray or Dataset
+    labels: UgridDataArray of integers
+
+    Returns
+    -------
+    partitions: List of (grid, obj)
+    """
     if not isinstance(labels, UgridDataArray):
         raise TypeError(
-            f"labels must be a UgridDataArray, received {type(labels).__name__}"
+            "labels must be a UgridDataArray, " f"received: {type(labels).__name__}"
         )
     if not np.issubdtype(labels.dtype, np.integer):
         raise TypeError(f"labels must have integer dtype, received {labels.dtype}")
-    if len(xugrid_obj.grids) > 1:
-        raise NotImplementedError("Can only partition a single UGRID topology")
 
-    grid = xugrid_obj.grid
-    coredim = grid.core_dimension
     if labels.grid != grid:
         raise ValueError("grid of labels does not match xugrid object")
-    if labels.dims != (coredim,):
+    if labels.dims != (grid.core_dimension,):
         raise ValueError(
-            f"Can only partition this topology by {coredim}, found in labels "
-            f"the dimensions: {labels.dims}"
+            f"Can only partition this topology by {grid.core_dimension}, found"
+            f" the dimensions: {labels.dims}"
         )
 
-    sorter = np.argsort(labels.values)
-    sorted = labels[sorter]
-    flag = sorted[:-1] != sorted[1:]
-    slices = np.concatenate(
-        (
-            [0],
-            np.flatnonzero(flag) + 1,
-            [sorter.size],
+    if isinstance(obj, xr.Dataset):
+        obj_type = UgridDataset
+    elif isinstance(obj, xr.DataArray):
+        obj_type = UgridDataArray
+    else:
+        raise TypeError(
+            f"Expected DataArray or Dataset, received: {type(obj).__name__}"
         )
-    )
 
-    partitions = [
-        xugrid_obj.isel({grid.core_dimension: sorter[start:end]})
-        for start, end in zip(slices[:-1, slices[1:]])
-    ]
+    indices = labels_to_indices(labels.values)
+    partitions = []
+    for index in indices:
+        new_grid, indexes = grid.topology_subset(index, return_index=True)
+        new_obj = obj.isel(indexes, missing_dims="ignore")
+        partitions.append(obj_type(new_obj, new_grid))
+
     return partitions
 
 
 def merge_nodes(grids):
     node_x = np.hstack([grid.node_x for grid in grids])
     node_y = np.hstack([grid.node_y for grid in grids])
     node_xy = np.column_stack((node_x, node_y))
@@ -130,15 +156,15 @@
         types = set(type(grid) for grid in grids)
         if len(types) > 1:
             raise TypeError(
                 f"All partition topologies with name {name} should be of the "
                 f"same type, received: {types}"
             )
 
-        griddims = set(tuple(grid.dimensions) for grid in grids)
+        griddims = list(set(tuple(grid.dimensions) for grid in grids))
         if len(griddims) > 1:
             raise ValueError(
                 f"Dimension names on UGRID topology {name} do not match "
                 f"across partitions: {griddims[0]} versus {griddims[1]}"
             )
 
     return None
@@ -152,23 +178,23 @@
 
     validate_partition_topology(grouped, len(partitions))
     return grouped
 
 
 def validate_partition_objects(data_objects):
     # Check presence of variables.
-    allvars = set(tuple(sorted(ds.dims)) for ds in data_objects)
+    allvars = list(set(tuple(sorted(ds.data_vars)) for ds in data_objects))
     if len(allvars) > 1:
         raise ValueError(
             "These variables are present in some partitions, but not in "
             f"others: {set(allvars[0]).symmetric_difference(allvars[1])}"
         )
     # Check dimensions
     for var in allvars.pop():
-        vardims = set(ds[var].dims for ds in data_objects)
+        vardims = list(set(ds[var].dims for ds in data_objects))
         if len(vardims) > 1:
             raise ValueError(
                 f"Dimensions for {var} do not match across partitions: "
                 f"{vardims[0]} versus {vardims[1]}"
             )
 
 
@@ -270,14 +296,14 @@
         merged_grid, indexes = grid.merge_partitions(grids)
         merged_grids.append(merged_grid)
 
         # Now remove duplicates, then concatenate along the UGRID dimension.
         for dim, dim_indexes in indexes.items():
             vars = vars_by_dim[dim]
             selection = [
-                obj[vars].isel({dim: index})
+                obj[vars].isel({dim: index}, missing_dims="ignore")
                 for obj, index in zip(data_objects, dim_indexes)
             ]
             merged_selection = xr.concat(selection, dim=dim)
             merged.update(merged_selection)
 
     return UgridDataset(merged, merged_grids)
```

### Comparing `xugrid-0.5.0/xugrid/ugrid/snapping.py` & `xugrid-0.6.0/xugrid/ugrid/snapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,16 @@
     faces = topology.face_node_connectivity
 
     # Derive connectivity
     edge_node_connectivity, face_edge_connectivity = connectivity.edge_connectivity(
         faces, -1
     )
     A = connectivity.to_sparse(face_edge_connectivity, fill_value=-1)
-    face_edge_connectivity = AdjacencyMatrix(A.indices, A.indptr, A.nnz)
+    n, m = A.shape
+    face_edge_connectivity = AdjacencyMatrix(A.indices, A.indptr, A.nnz, n, m)
 
     # Create geometric data
     edge_centroids = vertices[edge_node_connectivity].mean(axis=1)
     line_geometry = coerce_geometry(lines)
     line_coords, line_index = shapely.get_coordinates(line_geometry, return_index=True)
     # Snap line_coords to grid
     x, y = snap_to_nodes(
```

### Comparing `xugrid-0.5.0/xugrid/ugrid/ugrid1d.py` & `xugrid-0.6.0/xugrid/ugrid/ugrid1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from xarray.core.utils import either_dict_or_kwargs
 
 from xugrid import conversion
@@ -77,14 +77,15 @@
         self._xmax = None
         self._ymin = None
         self._ymax = None
         # Edges
         self._edge_x = None
         self._edge_y = None
         # Connectivity
+        self._node_node_connectivity = None
         self._node_edge_connectivity = None
         # crs
         if crs is None:
             self.crs = None
         else:
             import pyproj
 
@@ -247,31 +248,30 @@
     def core_dimension(self):
         return self.node_dimension
 
     @property
     def dimensions(self):
         return {self.node_dimension: self.n_node, self.edge_dimension: self.n_edge}
 
-    # These are all optional UGRID attributes. They are not computed by
-    # default, only when called upon.
+    # These are all optional attributes. They are not computed by default, only
+    # when called upon.
 
     @property
     def mesh(self) -> "mk.Mesh1d":  # type: ignore # noqa
         """
         Create if needed, and return meshkernel Mesh1d object.
 
         Returns
         -------
         mesh: meshkernel.Mesh1d
         """
         import meshkernel as mk
 
-        edge_nodes = self.edge_node_connectivity.ravel().astype(np.int32)
-
         if self._mesh is None:
+            edge_nodes = self.edge_node_connectivity.ravel().astype(np.int32)
             self._mesh = mk.Mesh1d(
                 node_x=self.node_x,
                 node_y=self.node_y,
                 edge_nodes=edge_nodes,
             )
         return self._mesh
 
@@ -515,16 +515,72 @@
         xmin: float,
         ymin: float,
         xmax: float,
         ymax: float,
     ):
         return self.sel(x=slice(xmin, xmax), y=slice(ymin, ymax))
 
+    def topological_sort_by_dfs(self) -> IntArray:
+        """
+        Returns an array of vertices in topological order.
+
+        Returns
+        -------
+        sorted_vertices: np.ndarray of integer
+        """
+        return connectivity.topological_sort_by_dfs(
+            self.directed_node_node_connectivity
+        )
+
+    def contract_vertices(self, indices: IntArray) -> "Ugrid1d":
+        """
+        Returns a simplified network topology by removing all nodes that are
+        not listed in ``indices``.
+
+        Parameters
+        ----------
+        indices: np.ndarray of integers
+
+        Returns
+        -------
+        contracted: Ugrid1d
+        """
+        edges = connectivity.contract_vertices(
+            self.directed_node_node_connectivity, indices
+        )
+        node_index = np.unique(edges.ravel())
+        new_edges = connectivity.renumber(edges)
+        return Ugrid1d(
+            node_x=self.node_x[node_index],
+            node_y=self.node_y[node_index],
+            fill_value=self.fill_value,
+            edge_node_connectivity=new_edges,
+            name=self.name,
+            indexes=self._indexes,
+            projected=self.projected,
+            crs=self.crs,
+            attrs=self._attrs,
+        )
+
     @staticmethod
-    def merge_partitions(grids):
+    def merge_partitions(grids: Sequence["Ugrid1d"]) -> "Ugrid1d":
+        """
+        Merge grid partitions into a single whole.
+
+        Duplicate edges are included only once, and removed from subsequent
+        partitions before merging.
+
+        Parameters
+        ----------
+        grids: sequence of Ugrid1d
+
+        Returns
+        -------
+        merged: Ugrid1d
+        """
         from xugrid.ugrid import partitioning
 
         # Grab a sample grid
         grid = next(iter(grids))
         fill_value = grid.fill_value
         node_coordinates, node_indexes, node_inverse = partitioning.merge_nodes(grids)
         new_edges, edge_indexes = partitioning.merge_edges(grids, node_inverse)
```

### Comparing `xugrid-0.5.0/xugrid/ugrid/ugrid2d.py` & `xugrid-0.6.0/xugrid/ugrid/ugrid2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from itertools import chain
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numba_celltree import CellTree2d
 from scipy.sparse import coo_matrix, csr_matrix
 from scipy.sparse.csgraph import reverse_cuthill_mckee
 from xarray.core.utils import either_dict_or_kwargs
 
+import xugrid
 from xugrid import conversion
 from xugrid import meshkernel_utils as mku
 from xugrid.constants import (
     BoolArray,
     FloatArray,
     FloatDType,
     IntArray,
@@ -133,14 +134,15 @@
         self._ymax = None
         # Edges
         self._edge_x = None
         self._edge_y = None
         # Connectivity
         self.edge_node_connectivity = edge_node_connectivity
         self._edge_face_connectivity = None
+        self._node_node_connectivity = None
         self._node_edge_connectivity = None
         self._node_face_connectivity = None
         self._face_edge_connectivity = None
         self._face_face_connectivity = None
         self._boundary_node_connectivity = None
         # Derived topology
         self._triangulation = None
@@ -1266,16 +1268,88 @@
             f = self.sel_points
         else:
             raise TypeError(
                 f"Invalid indexer types: {type(x).__name__}, and {type(y).__name__}"
             )
         return f(obj, x, y)
 
+    def label_partitions(self, n_part: int) -> "xugrid.UgridDataArray":
+        """
+        Generate partition labesl for this grid topology using METIS:
+        https://github.com/KarypisLab/METIS
+
+        This method utilizes the pymetis Python bindings:
+        https://github.com/inducer/pymetis
+
+        Parameters
+        ----------
+        n_part: integer
+            The number of parts to partition the mesh.
+
+        Returns
+        -------
+        partition_labels: UgridDataArray of integers
+        """
+        import pymetis
+
+        adjacency_matrix = self.face_face_connectivity
+        _, partition_index = pymetis.part_graph(
+            nparts=n_part,
+            xadj=adjacency_matrix.indptr,
+            adjncy=adjacency_matrix.indices,
+        )
+        return xugrid.UgridDataArray(
+            obj=xr.DataArray(
+                data=np.array(partition_index),
+                dims=(self.core_dimension,),
+                name="labels",
+            ),
+            grid=self,
+        )
+
+    def partition(self, n_part: int):
+        """
+        Partition this grid topology using METIS:
+        https://github.com/KarypisLab/METIS
+
+        This method utilizes the pymetis Python bindings:
+        https://github.com/inducer/pymetis
+
+        Parameters
+        ----------
+        n_part: integer
+            The number of parts to partition the mesh.
+
+        Returns
+        -------
+        partitions
+        """
+        from xugrid.ugrid.partitioning import labels_to_indices
+
+        labels = self.label_partitions(n_part)
+        indices = labels_to_indices(labels.values)
+        return [self.topology_subset(index) for index in indices]
+
     @staticmethod
-    def merge_partitions(grids):
+    def merge_partitions(grids: Sequence["Ugrid2d"]) -> "Ugrid2d":
+        """
+        Merge grid partitions into a single whole.
+
+        Duplicate faces are included only once, and removed from subsequent
+        partitions before merging.
+
+        Parameters
+        ----------
+        grids: sequence of Ugrid2d
+
+        Returns
+        -------
+        merged: Ugrid2d
+        """
+
         from xugrid.ugrid import partitioning
 
         # Grab a sample grid
         grid = next(iter(grids))
         fill_value = grid.fill_value
         node_coordinates, node_indexes, node_inverse = partitioning.merge_nodes(grids)
         new_faces, face_indexes = partitioning.merge_faces(
```

### Comparing `xugrid-0.5.0/xugrid/ugrid/ugridbase.py` & `xugrid-0.6.0/xugrid/ugrid/ugridbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,18 @@
         )
 
     if not pd_index.is_unique:
         raise ValueError(
             "index contains repeated values; only subsets will result "
             "in valid UGRID topology."
         )
-    if not pd_index.is_monotonic_increasing:
-        raise NotImplementedError("UGRID indexes must be sorted and unique.")
+    #    # TODO?
+    #    # Uniqueness is required, but sorting arguably not.
+    #    if not pd_index.is_monotonic_increasing:
+    #        raise NotImplementedError("UGRID indexes must be sorted and unique.")
 
     return pd_index
 
 
 def align(obj, grids, old_indexes):
     """
     Check which indexes have changed. Index on those new values.
@@ -91,14 +93,22 @@
     def core_dimension():
         """ """
 
     @abc.abstractproperty
     def dimensions():
         """ """
 
+    @abc.abstractproperty
+    def mesh():
+        """ """
+
+    @abc.abstractproperty
+    def meshkernel():
+        """ """
+
     @abc.abstractstaticmethod
     def from_dataset():
         """ """
 
     @abc.abstractmethod
     def to_dataset():
         """ """
@@ -152,14 +162,55 @@
             self._indexes = indexes
             self._attrs = {**defaults, **derived_dims, **dataset[name].attrs}
 
         # Ensure the name is always in sync.
         self._attrs["name"] = name
         return
 
+    def rename(self, name: str):
+        """
+        Create a new grid with all variables named according to the default
+        naming conventions.
+        """
+        # Get the old and the new names. Their keys are the same.
+        old_attrs = self._attrs
+        new_attrs = conventions.default_topology_attrs(name, self.topology_dimension)
+
+        # The attrs will have some roles joined together, e.g. node_coordinates
+        # will contain x and y as "mesh2d_node_x mesh2d_node_y".
+        name_dict = {self.name: name}
+        skip = ("cf_role", "long_name", "topology_dimension")
+        for key, value in old_attrs.items():
+            if key in new_attrs and key not in skip:
+                split_new = new_attrs[key].split()
+                split_old = value.split()
+                if len(split_new) != len(split_old):
+                    raise ValueError(
+                        f"Number of entries does not match on {key}: "
+                        f"{split_new} versus {split_old}"
+                    )
+                for name_key, name_value in zip(split_old, split_new):
+                    name_dict[name_key] = name_value
+
+        new = self.copy()
+        new.name = name
+        new._attrs = new_attrs
+        new._indexes = {k: name_dict[v] for k, v in new._indexes.items()}
+        if new._dataset is not None:
+            to_rename = (
+                tuple(new._dataset.data_vars)
+                + tuple(new._dataset.coords)
+                + tuple(new._dataset.dims)
+            )
+            new._dataset = new._dataset.rename(
+                {k: v for k, v in name_dict.items() if k in to_rename}
+            )
+
+        return new
+
     @staticmethod
     def _single_topology(dataset: xr.Dataset):
         topologies = dataset.ugrid_roles.topology
         n_topology = len(topologies)
         if n_topology == 0:
             raise ValueError("Dataset contains no UGRID topology variable.")
         elif n_topology > 1:
@@ -313,24 +364,27 @@
     def _prepare_connectivity(
         da: xr.DataArray, fill_value: Union[float, int], dtype: type
     ) -> xr.DataArray:
         start_index = da.attrs.get("start_index", 0)
         if start_index not in (0, 1):
             raise ValueError(f"start_index should be 0 or 1, received: {start_index}")
 
-        data = da.values
+        data = da.to_numpy()
+        # If xarray detects a _FillValue, it converts the array to floats and
+        # replaces the fill value by NaN, and moves the _FillValue to
+        # da.encoding.
         if "_FillValue" in da.attrs:
             is_fill = data == da.attrs["_FillValue"]
         else:
             is_fill = np.isnan(data)
+        data[is_fill] = fill_value
 
         cast = data.astype(dtype, copy=True)
         if start_index:
             cast -= start_index
-        cast[is_fill] = fill_value
         if (cast[~is_fill] < 0).any():
             raise ValueError("connectivity contains negative values")
         return da.copy(data=cast)
 
     def _precheck(self, multi_index):
         dim, index = multi_index.popitem()
         for check_dim, check_index in multi_index.items():
@@ -484,14 +538,40 @@
         """
         if self._node_edge_connectivity is None:
             self._node_edge_connectivity = connectivity.invert_dense_to_sparse(
                 self.edge_node_connectivity, self.fill_value
             )
         return self._node_edge_connectivity
 
+    @property
+    def node_node_connectivity(self) -> csr_matrix:
+        """
+        Node to node connectivity.
+
+        Returns
+        -------
+        connectivity: csr_matrix
+        """
+        if self._node_node_connectivity is None:
+            self._node_node_connectivity = connectivity.node_node_connectivity(
+                self.edge_node_connectivity
+            )
+        return self._node_node_connectivity
+
+    @property
+    def directed_node_node_connectivity(self) -> csr_matrix:
+        """
+        Directed node to node connectivity.
+
+        Returns
+        -------
+        connectivity: csr_matrix
+        """
+        return connectivity.directed_node_node_connectivity(self.edge_node_connectivity)
+
     def set_crs(
         self,
         crs: Union["pyproj.CRS", str] = None,  # type: ignore # noqa
         epsg: int = None,
         allow_override: bool = False,
     ):
         """
```

### Comparing `xugrid-0.5.0/xugrid/ugrid/voronoi.py` & `xugrid-0.6.0/xugrid/ugrid/voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.5.0/xugrid.egg-info/PKG-INFO` & `xugrid-0.6.0/xugrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.5.0
+Version: 0.6.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.5.0/xugrid.egg-info/SOURCES.txt` & `xugrid-0.6.0/xugrid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 tests/test_connectivity.py
 tests/test_conventions.py
 tests/test_conversion.py
 tests/test_data.py
 tests/test_interpolate.py
 tests/test_meshkernel_utils.py
+tests/test_partitioning.py
 tests/test_plot.py
 tests/test_snap.py
 tests/test_ugrid1d.py
 tests/test_ugrid2d.py
 tests/test_ugrid_dataset.py
 tests/test_voronoi.py
 xugrid/__init__.py
```

