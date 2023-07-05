# Comparing `tmp/sage_flatsurf-0.5.0.tar.gz` & `tmp/sage_flatsurf-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_flatsurf-0.5.0.tar", last modified: Thu Jun 22 23:26:14 2023, max compression
+gzip compressed data, was "sage_flatsurf-0.5.1.tar", last modified: Wed Jul  5 10:31:40 2023, max compression
```

## Comparing `sage_flatsurf-0.5.0.tar` & `sage_flatsurf-0.5.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/
--rw-r--r--   0 jule      (1000) jule      (1000)    15170 2022-01-18 01:36:32.000000 sage_flatsurf-0.5.0/COPYING
--rw-r--r--   0 jule      (1000) jule      (1000)       34 2023-03-22 01:49:20.000000 sage_flatsurf-0.5.0/MANIFEST.in
--rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/PKG-INFO
--rw-r--r--   0 jule      (1000) jule      (1000)     2964 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/README.md
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.172528 sage_flatsurf-0.5.0/flatsurf/
--rw-r--r--   0 jule      (1000) jule      (1000)      886 2023-06-22 23:01:04.000000 sage_flatsurf-0.5.0/flatsurf/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)     1200 2023-06-05 21:37:59.000000 sage_flatsurf-0.5.0/flatsurf/features.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.175862 sage_flatsurf-0.5.0/flatsurf/geometry/
--rw-r--r--   0 jule      (1000) jule      (1000)     1104 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/__init__.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.175862 sage_flatsurf-0.5.0/flatsurf/geometry/categories/
--rw-r--r--   0 jule      (1000) jule      (1000)     8327 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)    17139 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/cone_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)    23407 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/dilation_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)     9836 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygonal_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)    89332 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons.py
--rw-r--r--   0 jule      (1000) jule      (1000)    46720 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons_with_angles.py
--rw-r--r--   0 jule      (1000) jule      (1000)    25307 2023-06-22 23:01:20.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/half_translation_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)     2344 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/hyperbolic_polygons.py
--rw-r--r--   0 jule      (1000) jule      (1000)    49604 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygonal_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)    19633 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygons.py
--rw-r--r--   0 jule      (1000) jule      (1000)   112904 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/similarity_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)     2588 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/surface_category.py
--rw-r--r--   0 jule      (1000) jule      (1000)    19608 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/topological_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)    28889 2023-06-22 23:01:04.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/translation_surfaces.py
--rw-r--r--   0 jule      (1000) jule      (1000)    10135 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/chamanara.py
--rw-r--r--   0 jule      (1000) jule      (1000)     8896 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/circle.py
--rw-r--r--   0 jule      (1000) jule      (1000)    46514 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/delaunay.py
--rw-r--r--   0 jule      (1000) jule      (1000)    18517 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/euclidean.py
--rw-r--r--   0 jule      (1000) jule      (1000)    13583 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/finitely_generated_matrix_group.py
--rw-r--r--   0 jule      (1000) jule      (1000)    12790 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/fundamental_group.py
--rw-r--r--   0 jule      (1000) jule      (1000)    54160 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/gl2r_orbit_closure.py
--rw-r--r--   0 jule      (1000) jule      (1000)    11740 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/half_dilation_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)   459593 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/hyperbolic.py
--rw-r--r--   0 jule      (1000) jule      (1000)     7303 2023-06-22 22:50:10.000000 sage_flatsurf-0.5.0/flatsurf/geometry/interval_exchange_transformation.py
--rw-r--r--   0 jule      (1000) jule      (1000)    13586 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/l_infinity_delaunay_cells.py
--rw-r--r--   0 jule      (1000) jule      (1000)    31194 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/mappings.py
--rw-r--r--   0 jule      (1000) jule      (1000)     5693 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/mega_wollmilchsau.py
--rw-r--r--   0 jule      (1000) jule      (1000)    26845 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/minimal_cover.py
--rw-r--r--   0 jule      (1000) jule      (1000)     5674 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/origami.py
--rw-r--r--   0 jule      (1000) jule      (1000)    59727 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/polygon.py
--rw-r--r--   0 jule      (1000) jule      (1000)    18571 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/polyhedra.py
--rw-r--r--   0 jule      (1000) jule      (1000)    11077 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/pyflatsurf_conversion.py
--rw-r--r--   0 jule      (1000) jule      (1000)     7658 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/relative_homology.py
--rw-r--r--   0 jule      (1000) jule      (1000)    21216 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/similarity.py
--rw-r--r--   0 jule      (1000) jule      (1000)    76748 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/similarity_surface_generators.py
--rw-r--r--   0 jule      (1000) jule      (1000)    32811 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/straight_line_trajectory.py
--rw-r--r--   0 jule      (1000) jule      (1000)    14681 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/subfield.py
--rw-r--r--   0 jule      (1000) jule      (1000)   105338 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    89410 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface_legacy.py
--rw-r--r--   0 jule      (1000) jule      (1000)    52257 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface_objects.py
--rw-r--r--   0 jule      (1000) jule      (1000)    26371 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/tangent_bundle.py
--rw-r--r--   0 jule      (1000) jule      (1000)     6402 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/thurston_veech.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/flatsurf/graphical/
--rw-r--r--   0 jule      (1000) jule      (1000)     1122 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)    48132 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/hyperbolic.py
--rw-r--r--   0 jule      (1000) jule      (1000)    12346 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/polygon.py
--rw-r--r--   0 jule      (1000) jule      (1000)     4456 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/straight_line_trajectory.py
--rw-r--r--   0 jule      (1000) jule      (1000)    44815 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     2557 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/surface_point.py
--rw-r--r--   0 jule      (1000) jule      (1000)       18 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/flatsurf/version.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/
--rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/PKG-INFO
--rw-r--r--   0 jule      (1000) jule      (1000)     2278 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/SOURCES.txt
--rw-r--r--   0 jule      (1000) jule      (1000)        1 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/dependency_links.txt
--rw-r--r--   0 jule      (1000) jule      (1000)       17 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/requires.txt
--rw-r--r--   0 jule      (1000) jule      (1000)        9 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/top_level.txt
--rw-r--r--   0 jule      (1000) jule      (1000)       38 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/setup.cfg
--rw-r--r--   0 jule      (1000) jule      (1000)     2161 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/setup.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/
+-rw-r--r--   0 jule      (1000) jule      (1000)    15170 2022-01-18 01:36:32.000000 sage_flatsurf-0.5.1/COPYING
+-rw-r--r--   0 jule      (1000) jule      (1000)       34 2023-03-22 01:49:20.000000 sage_flatsurf-0.5.1/MANIFEST.in
+-rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/PKG-INFO
+-rw-r--r--   0 jule      (1000) jule      (1000)     2964 2023-07-05 10:31:36.000000 sage_flatsurf-0.5.1/README.md
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.373228 sage_flatsurf-0.5.1/flatsurf/
+-rw-r--r--   0 jule      (1000) jule      (1000)      886 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     1200 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/features.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.376561 sage_flatsurf-0.5.1/flatsurf/geometry/
+-rw-r--r--   0 jule      (1000) jule      (1000)     1104 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/__init__.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/flatsurf/geometry/categories/
+-rw-r--r--   0 jule      (1000) jule      (1000)     8327 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    17139 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/cone_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    23407 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/dilation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     9836 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygonal_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    89516 2023-07-04 01:11:11.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    46720 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygons_with_angles.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    26513 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/half_translation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2344 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/hyperbolic_polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    49604 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/polygonal_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    19633 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   112904 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/similarity_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2588 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/surface_category.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    19608 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/topological_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    28889 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/categories/translation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    10135 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/chamanara.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     8896 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/circle.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    46514 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/delaunay.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    19003 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/euclidean.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    13583 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/finitely_generated_matrix_group.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    12790 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/fundamental_group.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    54160 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/gl2r_orbit_closure.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    11740 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/half_dilation_surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   459593 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/hyperbolic.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     7303 2023-06-22 22:50:10.000000 sage_flatsurf-0.5.1/flatsurf/geometry/interval_exchange_transformation.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    13586 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/l_infinity_delaunay_cells.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    31194 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/mappings.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     5693 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/mega_wollmilchsau.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    26845 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/minimal_cover.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     5674 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/origami.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    59713 2023-07-04 01:07:28.000000 sage_flatsurf-0.5.1/flatsurf/geometry/polygon.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    18571 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/polyhedra.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    11077 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/pyflatsurf_conversion.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     7658 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/relative_homology.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    21216 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/similarity.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    76748 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/similarity_surface_generators.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    32811 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/straight_line_trajectory.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    14681 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/subfield.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   107512 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    89410 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/surface_legacy.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    52257 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/surface_objects.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    26371 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/tangent_bundle.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     6402 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/geometry/thurston_veech.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/flatsurf/graphical/
+-rw-r--r--   0 jule      (1000) jule      (1000)     1122 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/graphical/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    48132 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/graphical/hyperbolic.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    12346 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/graphical/polygon.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     4456 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/graphical/straight_line_trajectory.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    44873 2023-07-04 01:17:33.000000 sage_flatsurf-0.5.1/flatsurf/graphical/surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2557 2023-07-03 22:41:39.000000 sage_flatsurf-0.5.1/flatsurf/graphical/surface_point.py
+-rw-r--r--   0 jule      (1000) jule      (1000)       20 2023-07-05 10:31:36.000000 sage_flatsurf-0.5.1/flatsurf/version.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/
+-rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-07-05 10:31:40.000000 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/PKG-INFO
+-rw-r--r--   0 jule      (1000) jule      (1000)     2278 2023-07-05 10:31:40.000000 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/SOURCES.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)        1 2023-07-05 10:31:40.000000 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/dependency_links.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)       17 2023-07-05 10:31:40.000000 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/requires.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)        9 2023-07-05 10:31:40.000000 sage_flatsurf-0.5.1/sage_flatsurf.egg-info/top_level.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)       38 2023-07-05 10:31:40.379895 sage_flatsurf-0.5.1/setup.cfg
+-rw-r--r--   0 jule      (1000) jule      (1000)     2161 2023-07-05 10:31:36.000000 sage_flatsurf-0.5.1/setup.py
```

### Comparing `sage_flatsurf-0.5.0/COPYING` & `sage_flatsurf-0.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/PKG-INFO` & `sage_flatsurf-0.5.1/sage_flatsurf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sage_flatsurf
-Version: 0.5.0
+Name: sage-flatsurf
+Version: 0.5.1
 Summary: Flat surfaces in SageMath
 Home-page: https://github.com/flatsurf/sage-flatsurf
 Author: Vincent Delecroix, W. Patrick Hooper, and Julian Rüth
 Author-email: contact@flatsurf.org
 License: GNU General Public License, version 2
 Keywords: surfaces,dynamics,geometry,flat surfaces,Abelian differentials,quadratic differentials,Riemann surfaces
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 See [our documentation](https://flatsurf.github.io/sage-flatsurf/#installation)
 for detailed installation instructions.
 
 ## Run with Binder in the Cloud
 
 You can try out sage-flatsurf in an environment online; unfortunately it might
 take a long time for this environment to start:
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.0?filepath=doc%2Fexamples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.1?filepath=doc%2Fexamples)
 
 ## Developing sage-flatsurf
 
 Please consult our [Developer's
 Guide](https://flatsurf.github.io/sage-flatsurf/developer.html) to build
 sage-flaturf from source and to run our test suite.
```

### Comparing `sage_flatsurf-0.5.0/README.md` & `sage_flatsurf-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 See [our documentation](https://flatsurf.github.io/sage-flatsurf/#installation)
 for detailed installation instructions.
 
 ## Run with Binder in the Cloud
 
 You can try out sage-flatsurf in an environment online; unfortunately it might
 take a long time for this environment to start:
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.0?filepath=doc%2Fexamples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.1?filepath=doc%2Fexamples)
 
 ## Developing sage-flatsurf
 
 Please consult our [Developer's
 Guide](https://flatsurf.github.io/sage-flatsurf/developer.html) to build
 sage-flaturf from source and to run our test suite.
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/__init__.py` & `sage_flatsurf-0.5.1/flatsurf/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/features.py` & `sage_flatsurf-0.5.1/flatsurf/features.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/__init__.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/__init__.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/cone_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/cone_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/dilation_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/dilation_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygonal_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygonal_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygons.py`

 * *Files 1% similar despite different names*

```diff
@@ -744,14 +744,108 @@
                             (y[i - 1] + y[i]) * (x[i - 1] * y[i] - x[i] * y[i - 1])
                             for i in range(nvertices)
                         ]
                     ),
                 )
             )
 
+        def get_point_position(self, point, translation=None):
+            r"""
+            Return the combinatorial classification of a point and a polygon.
+
+            INPUT:
+
+            - ``point`` -- a point in the plane as a SageMath vector or pair of
+              numbers
+
+            OUTPUT:
+
+            a :class:`.geometry.polygon.PolygonPosition` object
+
+            ALGORITHM:
+
+            We use a winding number algorithm see
+            https://en.wikipedia.org/wiki/Point_in_polygon#Winding_number_algorithm
+
+            EXAMPLES::
+
+                sage: from flatsurf import polygons, Polygon
+                sage: S = polygons.square()
+
+                sage: S.get_point_position((1/2, 1/2))
+                point positioned in interior of polygon
+                sage: S.get_point_position((1, 0))
+                point positioned on vertex 1 of polygon
+                sage: S.get_point_position((1, 1/2))
+                point positioned on interior of edge 1 of polygon
+                sage: S.get_point_position((1, 3/2))
+                point positioned outside polygon
+
+                sage: p = Polygon(edges=[(1, 0), (1, 0), (1, 0), (0, 1), (-3, 0), (0, -1)])
+                sage: p.get_point_position([10, 0])
+                point positioned outside polygon
+                sage: p.get_point_position([1/2, 0])
+                point positioned on interior of edge 0 of polygon
+                sage: p.get_point_position([3/2, 0])
+                point positioned on interior of edge 1 of polygon
+                sage: p.get_point_position([2,0])
+                point positioned on vertex 2 of polygon
+                sage: p.get_point_position([5/2, 0])
+                point positioned on interior of edge 2 of polygon
+                sage: p.get_point_position([5/2, 1/4])
+                point positioned in interior of polygon
+
+            """
+            from sage.all import vector
+
+            point = vector(point)
+
+            if translation is not None:
+                import warnings
+
+                warnings.warn(
+                    "the translation keyword argument to get_point_position() has been deprecated and will be removed in a future version of sage-flatsurf; shift the point instead with the - operator"
+                )
+
+                from sage.all import vector
+
+                return self.get_point_position(point - vector(translation))
+
+            from flatsurf.geometry.euclidean import ccw
+            from flatsurf.geometry.polygon import PolygonPosition
+
+            # Determine whether the point is a vertex of the polygon.
+            for (i, v) in enumerate(self.vertices()):
+                if point == v:
+                    return PolygonPosition(PolygonPosition.VERTEX, vertex=i)
+
+            # Determine whether the point is on an edge of the polygon.
+            for (i, (v, e)) in enumerate(zip(self.vertices(), self.edges())):
+                if ccw(e, point - v) == 0:
+                    # The point lies on the line through this edge.
+                    if 0 < e.dot_product(point - v) < e.dot_product(e):
+                        return PolygonPosition(PolygonPosition.EDGE_INTERIOR, edge=i)
+
+            # Determine whether the point is inside or outside by computing the
+            # winding number of the polygon.
+            winding_number = 0
+
+            for (v, w) in zip(
+                self.vertices(), self.vertices()[1:] + self.vertices()[:1]
+            ):
+                if v[1] < point[1] and w[1] >= point[1] and ccw(w - v, point - v) > 0:
+                    winding_number += 1
+                if v[1] >= point[1] and w[1] < point[1] and ccw(w - v, point - v) < 0:
+                    winding_number -= 1
+
+            if winding_number % 2:
+                return PolygonPosition(PolygonPosition.INTERIOR)
+
+            return PolygonPosition(PolygonPosition.OUTSIDE)
+
     class Rational(CategoryWithAxiom_over_base_ring):
         r"""
         The category of rational Euclidean polygons.
 
         .. NOTE::
 
             This category must be defined here to make SageMath's test suite
@@ -1375,86 +1469,14 @@
                     r"""
                     Return whether the point is within the polygon (after the polygon is possibly translated)
                     """
                     return self.get_point_position(
                         point, translation=translation
                     ).is_inside()
 
-                def get_point_position(self, point, translation=None):
-                    r"""
-                    Get a combinatorial position of a points position compared to the polygon
-
-                    INPUT:
-
-                    - ``point`` -- a point in the plane (vector over the underlying base_ring())
-
-                    - ``translation`` -- optional translation to applied to the polygon (vector over the underlying base_ring())
-
-                    OUTPUT:
-
-                    - a PolygonPosition object
-
-                    EXAMPLES::
-
-                        sage: from flatsurf import polygons, Polygon
-                        sage: s = polygons.square()
-                        sage: V = s.base_ring()**2
-                        sage: s.get_point_position(V((1/2,1/2)))
-                        point positioned in interior of polygon
-                        sage: s.get_point_position(V((1,0)))
-                        point positioned on vertex 1 of polygon
-                        sage: s.get_point_position(V((1,1/2)))
-                        point positioned on interior of edge 1 of polygon
-                        sage: s.get_point_position(V((1,3/2)))
-                        point positioned outside polygon
-
-                        sage: p=Polygon(edges=[(1,0),(1,0),(1,0),(0,1),(-3,0),(0,-1)])
-                        sage: V = p.base_ring()**2
-                        sage: p.get_point_position(V([10,0]))
-                        point positioned outside polygon
-                        sage: p.get_point_position(V([1/2,0]))
-                        point positioned on interior of edge 0 of polygon
-                        sage: p.get_point_position(V([3/2,0]))
-                        point positioned on interior of edge 1 of polygon
-                        sage: p.get_point_position(V([2,0]))
-                        point positioned on vertex 2 of polygon
-                        sage: p.get_point_position(V([5/2,0]))
-                        point positioned on interior of edge 2 of polygon
-                        sage: p.get_point_position(V([5/2,1/4]))
-                        point positioned in interior of polygon
-                    """
-                    from flatsurf.geometry.polygon import PolygonPosition
-
-                    if translation is None:
-                        # Since we allow the initial vertex to be non-zero, this changed:
-                        v1 = self.vertex(0)
-                    else:
-                        # Since we allow the initial vertex to be non-zero, this changed:
-                        v1 = translation + self.vertex(0)
-                    # Below, we only make use of edge vectors:
-                    for i in range(len(self.vertices())):
-                        v0 = v1
-                        e = self.edge(i)
-                        v1 = v0 + e
-                        w = ccw(e, point - v0)
-                        if w < 0:
-                            return PolygonPosition(PolygonPosition.OUTSIDE)
-                        if w == 0:
-                            # Lies on the line through edge i!
-                            dp1 = e.dot_product(point - v0)
-                            if dp1 == 0:
-                                return PolygonPosition(PolygonPosition.VERTEX, vertex=i)
-                            dp2 = e.dot_product(e)
-                            if 0 < dp1 and dp1 < dp2:
-                                return PolygonPosition(
-                                    PolygonPosition.EDGE_INTERIOR, edge=i
-                                )
-                    # Loop terminated (on inside of each edge)
-                    return PolygonPosition(PolygonPosition.INTERIOR)
-
                 def flow_to_exit(self, point, direction):
                     r"""
                     Flow a point in the direction of holonomy until the point leaves the
                     polygon.  Note that ValueErrors may be thrown if the point is not in the
                     polygon, or if it is on the boundary and the holonomy does not point
                     into the polygon.
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons_with_angles.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/euclidean_polygons_with_angles.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/half_translation_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/half_translation_surfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -527,59 +527,86 @@
 
                             sage: from flatsurf import Polygon, similarity_surfaces
                             sage: P = Polygon(vertices=[(0,0), (2,0), (1,4), (0,5)])
                             sage: S = similarity_surfaces.self_glued_polygon(P)
                             sage: S.angles()
                             [1]
 
+                        Non-convex examples::
+
+                            sage: from flatsurf import Polygon, MutableOrientedSimilaritySurface
+                            sage: S = MutableOrientedSimilaritySurface(QQ)
+                            sage: L = Polygon(vertices=[(0,0),(1,0),(2,0),(2,1),(1,1),(1,2),(0,2),(0,1)])
+                            sage: S.add_polygon(L)
+                            0
+                            sage: S.glue((0, 0), (0, 5))
+                            sage: S.glue((0, 1), (0, 3))
+                            sage: S.glue((0, 2), (0, 7))
+                            sage: S.glue((0, 4), (0, 6))
+                            sage: S.set_immutable()
+                            sage: S.angles()
+                            [3]
+
+                            sage: S = MutableOrientedSimilaritySurface(QQ)
+                            sage: P = Polygon(vertices=[(0,0),(1,0),(2,0),(2,1),(3,1),(3,2),(2,2),(1,2),(1,1),(0,1)])
+                            sage: S.add_polygon(P)
+                            0
+                            sage: S.glue((0, 0), (0, 8))
+                            sage: S.glue((0, 1), (0, 6))
+                            sage: S.glue((0, 2), (0, 9))
+                            sage: S.glue((0, 3), (0, 5))
+                            sage: S.glue((0, 4), (0, 7))
+                            sage: S.set_immutable()
+                            sage: S.angles()
+                            [2, 2]
                         """
+                        from flatsurf.geometry.euclidean import is_between
+
                         edges = set(self.edges())
                         angles = []
 
-                        if return_adjacent_edges:
-                            while edges:
-                                # Note that iteration order here is different for different
-                                # versions of Python. Therefore, the output in the doctest
-                                # above is random.
-                                pair = p, e = next(iter(edges))
-                                ve = self.polygon(p).edge(e)
-                                angle = 0
-                                adjacent_edges = []
-                                while pair in edges:
-                                    adjacent_edges.append(pair)
-                                    edges.remove(pair)
-                                    f = (e - 1) % len(self.polygon(p).vertices())
-                                    ve = self.polygon(p).edge(e)
-                                    vf = -self.polygon(p).edge(f)
-                                    ppair = pp, ff = self.opposite_edge(p, f)
-                                    angle += (
-                                        (ve[0] > 0 and vf[0] <= 0)
-                                        or (ve[0] < 0 and vf[0] >= 0)
-                                        or (ve[0] == vf[0] == 0)
-                                    )
-                                    pair, p, e = ppair, pp, ff
-                                if numerical:
+                        while edges:
+                            # Note that iteration order here is different for different
+                            # versions of Python. Therefore, the output in the doctest
+                            # above is random.
+                            pair = p, e = next(iter(edges))
+                            ve = self.polygon(p).edge(e)
+                            angle = 0
+                            adjacent_edges = []
+                            while pair in edges:
+                                adjacent_edges.append(pair)
+                                edges.remove(pair)
+                                poly = self.polygon(p)
+                                f = (e - 1) % len(poly.vertices())
+                                ve = poly.edge(e)
+                                vf = -poly.edge(f)
+                                if (
+                                    ve[0] * vf[1] == ve[1] * vf[0]
+                                    and ve[0] * vf[0] >= 0
+                                    and ve[1] * vf[1] >= 0
+                                ):
+                                    # aligned vectors (angle 2pi)
+                                    if ve[0] == 0:
+                                        angle += 1
+                                    else:
+                                        angle += 2
+                                else:
+                                    if vf[0] == 0:
+                                        # include vf because it is vertical
+                                        angle += 1
+                                    angle += is_between(ve, vf, (0, 1))
+                                    angle += is_between(ve, vf, (0, -1))
+                                ppair = pp, ff = self.opposite_edge(p, f)
+                                pair, p, e = ppair, pp, ff
+                            if numerical:
+                                if return_adjacent_edges:
                                     angles.append((float(angle) / 2, adjacent_edges))
                                 else:
-                                    angles.append((QQ((angle, 2)), adjacent_edges))
-                        else:
-                            while edges:
-                                pair = p, e = next(iter(edges))
-                                angle = 0
-                                while pair in edges:
-                                    edges.remove(pair)
-                                    f = (e - 1) % len(self.polygon(p).vertices())
-                                    ve = self.polygon(p).edge(e)
-                                    vf = -self.polygon(p).edge(f)
-                                    ppair = pp, ff = self.opposite_edge(p, f)
-                                    angle += (
-                                        (ve[0] > 0 and vf[0] <= 0)
-                                        or (ve[0] < 0 and vf[0] >= 0)
-                                        or (ve[0] == vf[0] == 0)
-                                    )
-                                    pair, p, e = ppair, pp, ff
-                                if numerical:
+
                                     angles.append(float(angle) / 2)
+                            else:
+                                if return_adjacent_edges:
+                                    angles.append((QQ((angle, 2)), adjacent_edges))
                                 else:
                                     angles.append(QQ((angle, 2)))
 
                         return angles
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/hyperbolic_polygons.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/hyperbolic_polygons.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygonal_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/polygonal_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygons.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/polygons.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/similarity_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/similarity_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/surface_category.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/surface_category.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/topological_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/topological_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/categories/translation_surfaces.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/categories/translation_surfaces.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/chamanara.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/chamanara.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/circle.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/circle.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/delaunay.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/delaunay.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/euclidean.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/euclidean.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,36 +492,42 @@
     r"""
     Check whether the vector ``f`` is strictly in the sector formed by the vectors
     ``e0`` and ``e1`` (in counter-clockwise order).
 
     EXAMPLES::
 
         sage: from flatsurf.geometry.euclidean import is_between
-        sage: V = ZZ^2
-        sage: is_between(V((1, 0)), V((1, 1)), V((2, 1)))
+        sage: is_between((1, 0), (1, 1), (2, 1))
         True
 
+        sage: from itertools import product
+        sage: vecs = [(1, 0), (1, 1), (0, 1), (-1, 1), (-1, 0), (-1, -1), (0, -1), (1, -1)]
+        sage: for (i, vi), (j, vj), (k, vk) in product(enumerate(vecs), repeat=3):
+        ....:     assert is_between(vi, vj, vk) == ((i == j and i != k) or i < k < j or k < j < i or j < i < k), ((i, vi), (j, vj), (k, vk))
     """
     if e0[0] * e1[1] > e1[0] * e0[1]:
         # positive determinant
         # [ e0[0] e1[0] ]^-1 = [ e1[1] -e1[0] ]
         # [ e0[1] e1[1] ]      [-e0[1]  e0[0] ]
         # f[0] * e1[1] - e1[0] * f[1] > 0
         # - f[0] * e0[1] + e0[0] * f[1] > 0
         return e1[1] * f[0] > e1[0] * f[1] and e0[0] * f[1] > e0[1] * f[0]
     elif e0[0] * e1[1] == e1[0] * e0[1]:
         # aligned vector
-        return e0[0] * f[1] > e0[1] * f[0]
+        if e0[0] * e1[0] >= 0 and e0[1] * e1[1] >= 0:
+            return f[0] * e0[1] != f[1] * e0[0] or f[0] * e0[0] < 0 or f[1] * e0[1] < 0
+        else:
+            return e0[0] * f[1] > e0[1] * f[0]
     else:
         # negative determinant
         # [ e1[0] e0[0] ]^-1 = [ e0[1] -e0[0] ]
         # [ e1[1] e0[1] ]      [-e1[1]  e1[0] ]
         # f[0] * e0[1] - e0[0] * f[1] > 0
         # - f[0] * e1[1] + e1[0] * f[1] > 0
-        return e0[1] * f[0] <= e0[0] * f[1] or e1[0] * f[1] <= e1[1] * f[0]
+        return e0[1] * f[0] < e0[0] * f[1] or e1[0] * f[1] < e1[1] * f[0]
 
 
 def solve(x, u, y, v):
     r"""
     Return (a,b) so that: x + au = y + bv
 
     INPUT:
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/finitely_generated_matrix_group.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/finitely_generated_matrix_group.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/fundamental_group.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/fundamental_group.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/gl2r_orbit_closure.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/gl2r_orbit_closure.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/half_dilation_surface.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/half_dilation_surface.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/hyperbolic.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/interval_exchange_transformation.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/interval_exchange_transformation.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/l_infinity_delaunay_cells.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/l_infinity_delaunay_cells.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/mappings.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/mappings.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/mega_wollmilchsau.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/mega_wollmilchsau.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/minimal_cover.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/minimal_cover.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/origami.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/origami.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/polygon.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             (0, 0)
 
             sage: p.position()
             point positioned on vertex 0 of polygon
 
         .. SEEALSO::
 
-            :meth:`~.categories.euclidean_polygons.EuclideanPolygons.Simple.Convex.ParentMethods.get_point_position`
+            :meth:`~.categories.euclidean_polygons.EuclideanPolygons.ParentMethods.get_point_position`
 
         """
         return self.parent().get_point_position(self._xy)
 
     def _repr_(self):
         r"""
         Return a printable representation of this point.
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/polyhedra.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/polyhedra.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/pyflatsurf_conversion.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/pyflatsurf_conversion.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/relative_homology.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/relative_homology.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/similarity.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/similarity.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/similarity_surface_generators.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/similarity_surface_generators.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/straight_line_trajectory.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/straight_line_trajectory.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/subfield.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/subfield.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/surface.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2016,14 +2016,67 @@
         return s
 
     def triangulate(self, in_place=False, label=None, relabel=None):
         r"""
         Overrides
         :meth:`flatsurf.geometry.categories.similarity_surfaces.SimilaritySurfaces.Oriented.ParentMethods.triangulate`
         to allow triangulating in-place.
+
+        .. TODO::
+
+            The code here is not using
+            :meth:`~.categories.euclidean_polygons.EuclideanPolygons.Simple.ParentMethods.triangulation`.
+            It should probably be rewritten to share the same logic.
+
+        TESTS:
+
+        Verify that the monotile can be triangulated::
+
+            sage: from flatsurf import Polygon, MutableOrientedSimilaritySurface
+            sage: K = QuadraticField(3)
+            sage: a = K.gen()
+            sage: # build the vectors
+            sage: l = [(1, 0), (1, 2), (a, 11), (a, 1), (1, 4), (1, 6), (a, 3),
+            ....:      (a, 5), (1, 8), (1, 6), (a, 9), (a, 7), (1, 10), (1, 0)]
+            sage: vecs = []
+            sage: for m, e in l:
+            ....:     v = vector(K, [m * cos(2*pi*e/12), m * sin(2*pi*e/12)])
+            ....:     vecs.append(v)
+            sage: p = Polygon(edges=vecs)
+
+            sage: from collections import defaultdict
+            sage: d = defaultdict(list)
+            sage: for i, e in enumerate(p.edges()):
+            ....:     e.set_immutable()
+            ....:     d[e].append(i)
+
+            sage: Sbase = MutableOrientedSimilaritySurface(K)
+            sage: _ = Sbase.add_polygon(p)
+            sage: for v in list(d):
+            ....:     if v in d:
+            ....:         indices = d[v]
+            ....:         v_op = -v
+            ....:         v_op.set_immutable()
+            ....:         opposite_indices = d[v_op]
+            ....:         assert len(indices) == len(opposite_indices), (len(indices), len(opposite_indices))
+            ....:         if len(indices) == 1:
+            ....:             del d[v]
+            ....:             del d[v_op]
+            ....:             Sbase.glue((0, indices[0]), (0, opposite_indices[0]))
+
+            sage: (i0, j0), (i1, j1) = d.values()
+
+            sage: S1 = MutableOrientedSimilaritySurface.from_surface(Sbase)
+            sage: S1.glue((0, i0), (0, i1))
+            sage: S1.glue((0, j0), (0, j1))
+            sage: S1.set_immutable()
+
+            sage: S1.triangulate()
+            Translation Surface in H_3(4, 0) built from 5 isosceles triangles, 6 triangles and a right triangle
+
         """
         if relabel is not None:
             import warnings
 
             warnings.warn(
                 "the relabel keyword argument of triangulate() is ignored, it has been deprecated and will be removed in a future version of sage-flatsurf"
             )
@@ -2052,15 +2105,15 @@
 
         for i in range(n - 3):
             poly = s.polygon(label)
             n = len(poly.vertices())
             for i in range(n):
                 e1 = poly.edge(i)
                 e2 = poly.edge((i + 1) % n)
-                if ccw(e1, e2) != 0:
+                if ccw(e1, e2) > 0:
                     # This is in case the polygon is a triangle with subdivided edge.
                     e3 = poly.edge((i + 2) % n)
                     if ccw(e1 + e2, e3) != 0:
                         s.subdivide_polygon(label, i, (i + 2) % n)
                         break
         return s
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/surface_legacy.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/surface_legacy.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/surface_objects.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/surface_objects.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/tangent_bundle.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/tangent_bundle.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/geometry/thurston_veech.py` & `sage_flatsurf-0.5.1/flatsurf/geometry/thurston_veech.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/__init__.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/hyperbolic.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/hyperbolic.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/polygon.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/polygon.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/straight_line_trajectory.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/straight_line_trajectory.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/surface.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,15 +647,15 @@
         A point always must be provided. If a vector v is provided then a
         SimilaritySurfaceTangentVector will be returned. If v is not provided, then a
         SurfacePoint is returned.
 
         INPUT:
 
         - ``point`` -- Coordinates of a point in graphical coordinates to be
-            converted to graphical coordinates.
+            converted to surface coordinates.
 
         - ``v`` -- (default ``None``) If provided a tangent vector in graphical
             coordinates based at the provided point.
 
         - ``label`` -- (default ``None``) If provided, then we only convert
             points and tangent vectors in the corresponding graphical polygon.
 
@@ -717,14 +717,16 @@
             sage: v = gs.to_surface((3/2,3/2),(sqrt(3),sqrt(2)),ring=AA,search_all=True, search_limit=20)
             sage: v.bundle()
             Tangent bundle of Minimal Planar Cover of Translation Surface in H_1(0) built from a square defined over Algebraic Real Field
 
         """
         surface = self.get_surface()
 
+        point = vector(point, ring or surface.base_ring())
+
         if label is None:
             if search_all:
                 if search_limit is None:
                     if surface.is_finite_type():
                         labels = surface.labels()
                     else:
                         raise ValueError(
```

### Comparing `sage_flatsurf-0.5.0/flatsurf/graphical/surface_point.py` & `sage_flatsurf-0.5.1/flatsurf/graphical/surface_point.py`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/sage_flatsurf.egg-info/PKG-INFO` & `sage_flatsurf-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sage-flatsurf
-Version: 0.5.0
+Name: sage_flatsurf
+Version: 0.5.1
 Summary: Flat surfaces in SageMath
 Home-page: https://github.com/flatsurf/sage-flatsurf
 Author: Vincent Delecroix, W. Patrick Hooper, and Julian Rüth
 Author-email: contact@flatsurf.org
 License: GNU General Public License, version 2
 Keywords: surfaces,dynamics,geometry,flat surfaces,Abelian differentials,quadratic differentials,Riemann surfaces
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 See [our documentation](https://flatsurf.github.io/sage-flatsurf/#installation)
 for detailed installation instructions.
 
 ## Run with Binder in the Cloud
 
 You can try out sage-flatsurf in an environment online; unfortunately it might
 take a long time for this environment to start:
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.0?filepath=doc%2Fexamples)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/flatsurf/sage-flatsurf/0.5.1?filepath=doc%2Fexamples)
 
 ## Developing sage-flatsurf
 
 Please consult our [Developer's
 Guide](https://flatsurf.github.io/sage-flatsurf/developer.html) to build
 sage-flaturf from source and to run our test suite.
```

### Comparing `sage_flatsurf-0.5.0/sage_flatsurf.egg-info/SOURCES.txt` & `sage_flatsurf-0.5.1/sage_flatsurf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.5.0/setup.py` & `sage_flatsurf-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 setup(
     name="sage_flatsurf",
     author="Vincent Delecroix, W. Patrick Hooper, and Julian Rüth",
     author_email="contact@flatsurf.org",
     description="Flat surfaces in SageMath",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.5.0',
+    version='0.5.1',
     url="https://github.com/flatsurf/sage-flatsurf",
     license="GNU General Public License, version 2",
     packages=[
         "flatsurf",
         "flatsurf.geometry",
         "flatsurf.geometry.categories",
         "flatsurf.graphical",
```

