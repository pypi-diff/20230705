# Comparing `tmp/ansys-api-pyensight-0.2.2.tar.gz` & `tmp/ansys-api-pyensight-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-pyensight-0.2.2.tar", last modified: Wed Jul  5 09:16:17 2023, max compression
+gzip compressed data, was "ansys-api-pyensight-0.2.dev0.tar", last modified: Mon Jul  3 09:54:23 2023, max compression
```

## Comparing `ansys-api-pyensight-0.2.2.tar` & `ansys-api-pyensight-0.2.dev0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.399761 ansys-api-pyensight-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-05 09:16:17.399761 ansys-api-pyensight-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:16:17.399761 ansys-api-pyensight-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.375761 ansys-api-pyensight-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.371761 ansys-api-pyensight-0.2.2/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.375761 ansys-api-pyensight-0.2.2/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.395761 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/access_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.395761 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   926642 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_animobj.py
--rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot.py
--rw-r--r--   0 runner    (1001) docker     (123)    48180 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    34554 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)    35302 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_lgnd.py
--rw-r--r--   0 runner    (1001) docker     (123)    35577 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_emitterobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_flipbook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)   214200 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_lightsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_lpart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    56524 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)   264396 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part.py
--rw-r--r--   0 runner    (1001) docker     (123)   195871 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_aux_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)   190146 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_axisymmetric.py
--rw-r--r--   0 runner    (1001) docker     (123)   179413 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_built_up.py
--rw-r--r--   0 runner    (1001) docker     (123)   289827 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)   202105 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)   186771 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_developed_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)   264534 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_discrete_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)   192486 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_elevated_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)   241715 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)   192689 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_sep_att.py
--rw-r--r--   0 runner    (1001) docker     (123)   202494 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_shock.py
--rw-r--r--   0 runner    (1001) docker     (123)   192681 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_vortex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)   192954 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_isosurface.py
--rw-r--r--   0 runner    (1001) docker     (123)   183318 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_mat_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)   264486 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   243979 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_particle_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)   181578 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_point.py
--rw-r--r--   0 runner    (1001) docker     (123)   187760 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)   198386 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_tensor_glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)   204686 2023-07-05 09:16:16.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_vector_arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)   236410 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_vof.py
--rw-r--r--   0 runner    (1001) docker     (123)   132145 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_probe.py
--rw-r--r--   0 runner    (1001) docker     (123)    83457 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cone.py
--rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_revolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_var.py
--rw-r--r--   0 runner    (1001) docker     (123)   211317 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_vport.py
--rw-r--r--   0 runner    (1001) docker     (123)  2000683 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ensight_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.395761 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/enshell.proto
--rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/ensight.proto
--rw-r--r--   0 runner    (1001) docker     (123)  2446593 2023-07-05 09:15:58.000000 ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/ensight_api.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:16:17.399761 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 09:16:17.000000 ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.636831 ansys-api-pyensight-0.2.dev0/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/access_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   926642 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_animobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48180 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34554 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35302 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_lgnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35577 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31771 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30261 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34357 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65944 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_emitterobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_flipbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214200 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lightsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lpart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56524 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264396 2023-07-03 09:54:22.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195871 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_aux_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190146 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179413 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_built_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)   289827 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202105 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186771 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_developed_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264534 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_discrete_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192486 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_elevated_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241715 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192689 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_sep_att.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202494 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_shock.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192681 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_vortex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192954 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183318 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_mat_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   264486 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   243979 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_particle_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181578 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187760 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   198386 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_tensor_glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   204686 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vector_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236410 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vof.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132145 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83457 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18958 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_revolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211317 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_vport.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2000687 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ensight_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.656832 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/enshell.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    18258 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight.proto
+-rw-r--r--   0 runner    (1001) docker     (123)  2446597 2023-07-03 09:54:05.000000 ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight_api.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:54:23.660832 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 09:54:23.000000 ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/top_level.txt
```

### Comparing `ansys-api-pyensight-0.2.2/LICENSE` & `ansys-api-pyensight-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/PKG-INFO` & `ansys-api-pyensight-0.2.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.2.2
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:16:15 on 05 July 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:54:22 on 03 July 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ansys-api-pyensight-0.2.2/README.md` & `ansys-api-pyensight-0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/setup.py` & `ansys-api-pyensight-0.2.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/assets/ensight_api_test_assets.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1494,22 +1494,22 @@
 objs,ENS_ANNOT_LINE,origin1,EMPTY
 objs,ENS_ANNOT_LINE,ORIGIN1,SETTER
 objs,ENS_ANNOT_LINE,origin1,SETTER
 objs,ENS_ANNOT_LINE,ORIGIN2,EMPTY
 objs,ENS_ANNOT_LINE,origin2,EMPTY
 objs,ENS_ANNOT_LINE,ORIGIN2,SETTER
 objs,ENS_ANNOT_LINE,origin2,SETTER
-objs,ENS_ANNOT_LINE,ORIGINBY2,EMPTY
-objs,ENS_ANNOT_LINE,originby2,EMPTY
-objs,ENS_ANNOT_LINE,ORIGINBY2,SETTER
-objs,ENS_ANNOT_LINE,originby2,SETTER
 objs,ENS_ANNOT_LINE,ORIGINBY1,EMPTY
 objs,ENS_ANNOT_LINE,originby1,EMPTY
 objs,ENS_ANNOT_LINE,ORIGINBY1,SETTER
 objs,ENS_ANNOT_LINE,originby1,SETTER
+objs,ENS_ANNOT_LINE,ORIGINBY2,EMPTY
+objs,ENS_ANNOT_LINE,originby2,EMPTY
+objs,ENS_ANNOT_LINE,ORIGINBY2,SETTER
+objs,ENS_ANNOT_LINE,originby2,SETTER
 objs,ENS_ANNOT_LOGO,objid,EMPTY
 objs,ENS_ANNOT_LOGO,_update_attr_list,None
 objs,ENS_ANNOT_LOGO,_remote_obj,ensight.objs.wrap_id(1)
 objs,ENS_ANNOT_LOGO,createannot,ensight.objs.wrap_id(1).createannot(1,0=0)
 objs,ENS_ANNOT_LOGO,attrgroupinfo,ensight.objs.wrap_id(1).attrgroupinfo(1,0=0)
 objs,ENS_ANNOT_LOGO,METADATA,EMPTY
 objs,ENS_ANNOT_LOGO,metadata,EMPTY
@@ -1967,22 +1967,22 @@
 objs,ENS_ANNOT_DIAL,littlehandrange,EMPTY
 objs,ENS_ANNOT_DIAL,LITTLEHANDRANGE,SETTER
 objs,ENS_ANNOT_DIAL,littlehandrange,SETTER
 objs,ENS_ANNOT_DIAL,BACKGROUND,EMPTY
 objs,ENS_ANNOT_DIAL,background,EMPTY
 objs,ENS_ANNOT_DIAL,BACKGROUND,SETTER
 objs,ENS_ANNOT_DIAL,background,SETTER
-objs,ENS_ANNOT_DIAL,VALUERGB,EMPTY
-objs,ENS_ANNOT_DIAL,valuergb,EMPTY
-objs,ENS_ANNOT_DIAL,VALUERGB,SETTER
-objs,ENS_ANNOT_DIAL,valuergb,SETTER
 objs,ENS_ANNOT_DIAL,BACKGROUNDRGB,EMPTY
 objs,ENS_ANNOT_DIAL,backgroundrgb,EMPTY
 objs,ENS_ANNOT_DIAL,BACKGROUNDRGB,SETTER
 objs,ENS_ANNOT_DIAL,backgroundrgb,SETTER
+objs,ENS_ANNOT_DIAL,VALUERGB,EMPTY
+objs,ENS_ANNOT_DIAL,valuergb,EMPTY
+objs,ENS_ANNOT_DIAL,VALUERGB,SETTER
+objs,ENS_ANNOT_DIAL,valuergb,SETTER
 objs,ENS_ANNOT_DIAL,VALUESIZE,EMPTY
 objs,ENS_ANNOT_DIAL,valuesize,EMPTY
 objs,ENS_ANNOT_DIAL,VALUESIZE,SETTER
 objs,ENS_ANNOT_DIAL,valuesize,SETTER
 objs,ENS_ANNOT_DIAL,SHOWAS,EMPTY
 objs,ENS_ANNOT_DIAL,showas,EMPTY
 objs,ENS_ANNOT_DIAL,SHOWAS,SETTER
@@ -2058,22 +2058,22 @@
 objs,ENS_ANNOT_GAUGE,minimum,EMPTY
 objs,ENS_ANNOT_GAUGE,MINIMUM,SETTER
 objs,ENS_ANNOT_GAUGE,minimum,SETTER
 objs,ENS_ANNOT_GAUGE,BACKGROUND,EMPTY
 objs,ENS_ANNOT_GAUGE,background,EMPTY
 objs,ENS_ANNOT_GAUGE,BACKGROUND,SETTER
 objs,ENS_ANNOT_GAUGE,background,SETTER
-objs,ENS_ANNOT_GAUGE,VALUERGB,EMPTY
-objs,ENS_ANNOT_GAUGE,valuergb,EMPTY
-objs,ENS_ANNOT_GAUGE,VALUERGB,SETTER
-objs,ENS_ANNOT_GAUGE,valuergb,SETTER
 objs,ENS_ANNOT_GAUGE,BACKGROUNDRGB,EMPTY
 objs,ENS_ANNOT_GAUGE,backgroundrgb,EMPTY
 objs,ENS_ANNOT_GAUGE,BACKGROUNDRGB,SETTER
 objs,ENS_ANNOT_GAUGE,backgroundrgb,SETTER
+objs,ENS_ANNOT_GAUGE,VALUERGB,EMPTY
+objs,ENS_ANNOT_GAUGE,valuergb,EMPTY
+objs,ENS_ANNOT_GAUGE,VALUERGB,SETTER
+objs,ENS_ANNOT_GAUGE,valuergb,SETTER
 objs,ENS_ANNOT_GAUGE,VALUESIZE,EMPTY
 objs,ENS_ANNOT_GAUGE,valuesize,EMPTY
 objs,ENS_ANNOT_GAUGE,VALUESIZE,SETTER
 objs,ENS_ANNOT_GAUGE,valuesize,SETTER
 objs,ENS_ANNOT_GAUGE,MAXIMUM,EMPTY
 objs,ENS_ANNOT_GAUGE,maximum,EMPTY
 objs,ENS_ANNOT_GAUGE,MAXIMUM,SETTER
@@ -3924,22 +3924,22 @@
 objs,ENS_PART,reducepolygonsfactor,EMPTY
 objs,ENS_PART,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART,reducepolygonsfactor,SETTER
 objs,ENS_PART,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART,eltshrinkfactor,EMPTY
 objs,ENS_PART,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART,eltshrinkfactor,SETTER
-objs,ENS_PART,CULLELEMENTS,EMPTY
-objs,ENS_PART,cullelements,EMPTY
-objs,ENS_PART,CULLELEMENTS,SETTER
-objs,ENS_PART,cullelements,SETTER
 objs,ENS_PART,ELTBLANKING,EMPTY
 objs,ENS_PART,eltblanking,EMPTY
 objs,ENS_PART,ELTBLANKING,SETTER
 objs,ENS_PART,eltblanking,SETTER
+objs,ENS_PART,CULLELEMENTS,EMPTY
+objs,ENS_PART,cullelements,EMPTY
+objs,ENS_PART,CULLELEMENTS,SETTER
+objs,ENS_PART,cullelements,SETTER
 objs,ENS_PART,HIDDENSURFACE,EMPTY
 objs,ENS_PART,hiddensurface,EMPTY
 objs,ENS_PART,HIDDENSURFACE,SETTER
 objs,ENS_PART,hiddensurface,SETTER
 objs,ENS_PART,BOUNDINGREP,EMPTY
 objs,ENS_PART,boundingrep,EMPTY
 objs,ENS_PART,BOUNDINGREP,SETTER
@@ -4638,22 +4638,22 @@
 objs,ENS_PART_MODEL,reducepolygonsfactor,EMPTY
 objs,ENS_PART_MODEL,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_MODEL,reducepolygonsfactor,SETTER
 objs,ENS_PART_MODEL,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_MODEL,eltshrinkfactor,EMPTY
 objs,ENS_PART_MODEL,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_MODEL,eltshrinkfactor,SETTER
-objs,ENS_PART_MODEL,CULLELEMENTS,EMPTY
-objs,ENS_PART_MODEL,cullelements,EMPTY
-objs,ENS_PART_MODEL,CULLELEMENTS,SETTER
-objs,ENS_PART_MODEL,cullelements,SETTER
 objs,ENS_PART_MODEL,ELTBLANKING,EMPTY
 objs,ENS_PART_MODEL,eltblanking,EMPTY
 objs,ENS_PART_MODEL,ELTBLANKING,SETTER
 objs,ENS_PART_MODEL,eltblanking,SETTER
+objs,ENS_PART_MODEL,CULLELEMENTS,EMPTY
+objs,ENS_PART_MODEL,cullelements,EMPTY
+objs,ENS_PART_MODEL,CULLELEMENTS,SETTER
+objs,ENS_PART_MODEL,cullelements,SETTER
 objs,ENS_PART_MODEL,HIDDENSURFACE,EMPTY
 objs,ENS_PART_MODEL,hiddensurface,EMPTY
 objs,ENS_PART_MODEL,HIDDENSURFACE,SETTER
 objs,ENS_PART_MODEL,hiddensurface,SETTER
 objs,ENS_PART_MODEL,BOUNDINGREP,EMPTY
 objs,ENS_PART_MODEL,boundingrep,EMPTY
 objs,ENS_PART_MODEL,BOUNDINGREP,SETTER
@@ -5364,22 +5364,22 @@
 objs,ENS_PART_CLIP,reducepolygonsfactor,EMPTY
 objs,ENS_PART_CLIP,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_CLIP,reducepolygonsfactor,SETTER
 objs,ENS_PART_CLIP,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_CLIP,eltshrinkfactor,EMPTY
 objs,ENS_PART_CLIP,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_CLIP,eltshrinkfactor,SETTER
-objs,ENS_PART_CLIP,CULLELEMENTS,EMPTY
-objs,ENS_PART_CLIP,cullelements,EMPTY
-objs,ENS_PART_CLIP,CULLELEMENTS,SETTER
-objs,ENS_PART_CLIP,cullelements,SETTER
 objs,ENS_PART_CLIP,ELTBLANKING,EMPTY
 objs,ENS_PART_CLIP,eltblanking,EMPTY
 objs,ENS_PART_CLIP,ELTBLANKING,SETTER
 objs,ENS_PART_CLIP,eltblanking,SETTER
+objs,ENS_PART_CLIP,CULLELEMENTS,EMPTY
+objs,ENS_PART_CLIP,cullelements,EMPTY
+objs,ENS_PART_CLIP,CULLELEMENTS,SETTER
+objs,ENS_PART_CLIP,cullelements,SETTER
 objs,ENS_PART_CLIP,HIDDENSURFACE,EMPTY
 objs,ENS_PART_CLIP,hiddensurface,EMPTY
 objs,ENS_PART_CLIP,HIDDENSURFACE,SETTER
 objs,ENS_PART_CLIP,hiddensurface,SETTER
 objs,ENS_PART_CLIP,BOUNDINGREP,EMPTY
 objs,ENS_PART_CLIP,boundingrep,EMPTY
 objs,ENS_PART_CLIP,BOUNDINGREP,SETTER
@@ -5544,22 +5544,22 @@
 objs,ENS_PART_CLIP,cyldradius,EMPTY
 objs,ENS_PART_CLIP,CYLDRADIUS,SETTER
 objs,ENS_PART_CLIP,cyldradius,SETTER
 objs,ENS_PART_CLIP,CYLDORIGIN,EMPTY
 objs,ENS_PART_CLIP,cyldorigin,EMPTY
 objs,ENS_PART_CLIP,CYLDORIGIN,SETTER
 objs,ENS_PART_CLIP,cyldorigin,SETTER
-objs,ENS_PART_CLIP,CYLDENDPOINT,EMPTY
-objs,ENS_PART_CLIP,cyldendpoint,EMPTY
-objs,ENS_PART_CLIP,CYLDENDPOINT,SETTER
-objs,ENS_PART_CLIP,cyldendpoint,SETTER
 objs,ENS_PART_CLIP,CYLDAXISVECT,EMPTY
 objs,ENS_PART_CLIP,cyldaxisvect,EMPTY
 objs,ENS_PART_CLIP,CYLDAXISVECT,SETTER
 objs,ENS_PART_CLIP,cyldaxisvect,SETTER
+objs,ENS_PART_CLIP,CYLDENDPOINT,EMPTY
+objs,ENS_PART_CLIP,cyldendpoint,EMPTY
+objs,ENS_PART_CLIP,CYLDENDPOINT,SETTER
+objs,ENS_PART_CLIP,cyldendpoint,SETTER
 objs,ENS_PART_CLIP,CONEANGLE,EMPTY
 objs,ENS_PART_CLIP,coneangle,EMPTY
 objs,ENS_PART_CLIP,CONEANGLE,SETTER
 objs,ENS_PART_CLIP,coneangle,SETTER
 objs,ENS_PART_CLIP,CONEORIGIN,EMPTY
 objs,ENS_PART_CLIP,coneorigin,EMPTY
 objs,ENS_PART_CLIP,CONEORIGIN,SETTER
@@ -6194,22 +6194,22 @@
 objs,ENS_PART_CONTOUR,reducepolygonsfactor,EMPTY
 objs,ENS_PART_CONTOUR,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_CONTOUR,reducepolygonsfactor,SETTER
 objs,ENS_PART_CONTOUR,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_CONTOUR,eltshrinkfactor,EMPTY
 objs,ENS_PART_CONTOUR,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_CONTOUR,eltshrinkfactor,SETTER
-objs,ENS_PART_CONTOUR,CULLELEMENTS,EMPTY
-objs,ENS_PART_CONTOUR,cullelements,EMPTY
-objs,ENS_PART_CONTOUR,CULLELEMENTS,SETTER
-objs,ENS_PART_CONTOUR,cullelements,SETTER
 objs,ENS_PART_CONTOUR,ELTBLANKING,EMPTY
 objs,ENS_PART_CONTOUR,eltblanking,EMPTY
 objs,ENS_PART_CONTOUR,ELTBLANKING,SETTER
 objs,ENS_PART_CONTOUR,eltblanking,SETTER
+objs,ENS_PART_CONTOUR,CULLELEMENTS,EMPTY
+objs,ENS_PART_CONTOUR,cullelements,EMPTY
+objs,ENS_PART_CONTOUR,CULLELEMENTS,SETTER
+objs,ENS_PART_CONTOUR,cullelements,SETTER
 objs,ENS_PART_CONTOUR,HIDDENSURFACE,EMPTY
 objs,ENS_PART_CONTOUR,hiddensurface,EMPTY
 objs,ENS_PART_CONTOUR,HIDDENSURFACE,SETTER
 objs,ENS_PART_CONTOUR,hiddensurface,SETTER
 objs,ENS_PART_CONTOUR,BOUNDINGREP,EMPTY
 objs,ENS_PART_CONTOUR,boundingrep,EMPTY
 objs,ENS_PART_CONTOUR,BOUNDINGREP,SETTER
@@ -6748,22 +6748,22 @@
 objs,ENS_PART_DISCRETE_PARTICLE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,reducepolygonsfactor,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,eltshrinkfactor,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,eltshrinkfactor,SETTER
-objs,ENS_PART_DISCRETE_PARTICLE,CULLELEMENTS,EMPTY
-objs,ENS_PART_DISCRETE_PARTICLE,cullelements,EMPTY
-objs,ENS_PART_DISCRETE_PARTICLE,CULLELEMENTS,SETTER
-objs,ENS_PART_DISCRETE_PARTICLE,cullelements,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,ELTBLANKING,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,eltblanking,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,ELTBLANKING,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,eltblanking,SETTER
+objs,ENS_PART_DISCRETE_PARTICLE,CULLELEMENTS,EMPTY
+objs,ENS_PART_DISCRETE_PARTICLE,cullelements,EMPTY
+objs,ENS_PART_DISCRETE_PARTICLE,CULLELEMENTS,SETTER
+objs,ENS_PART_DISCRETE_PARTICLE,cullelements,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,hiddensurface,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,HIDDENSURFACE,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,hiddensurface,SETTER
 objs,ENS_PART_DISCRETE_PARTICLE,BOUNDINGREP,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,boundingrep,EMPTY
 objs,ENS_PART_DISCRETE_PARTICLE,BOUNDINGREP,SETTER
@@ -7612,22 +7612,22 @@
 objs,ENS_PART_ISOSURFACE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_ISOSURFACE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_ISOSURFACE,reducepolygonsfactor,SETTER
 objs,ENS_PART_ISOSURFACE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_ISOSURFACE,eltshrinkfactor,EMPTY
 objs,ENS_PART_ISOSURFACE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_ISOSURFACE,eltshrinkfactor,SETTER
-objs,ENS_PART_ISOSURFACE,CULLELEMENTS,EMPTY
-objs,ENS_PART_ISOSURFACE,cullelements,EMPTY
-objs,ENS_PART_ISOSURFACE,CULLELEMENTS,SETTER
-objs,ENS_PART_ISOSURFACE,cullelements,SETTER
 objs,ENS_PART_ISOSURFACE,ELTBLANKING,EMPTY
 objs,ENS_PART_ISOSURFACE,eltblanking,EMPTY
 objs,ENS_PART_ISOSURFACE,ELTBLANKING,SETTER
 objs,ENS_PART_ISOSURFACE,eltblanking,SETTER
+objs,ENS_PART_ISOSURFACE,CULLELEMENTS,EMPTY
+objs,ENS_PART_ISOSURFACE,cullelements,EMPTY
+objs,ENS_PART_ISOSURFACE,CULLELEMENTS,SETTER
+objs,ENS_PART_ISOSURFACE,cullelements,SETTER
 objs,ENS_PART_ISOSURFACE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_ISOSURFACE,hiddensurface,EMPTY
 objs,ENS_PART_ISOSURFACE,HIDDENSURFACE,SETTER
 objs,ENS_PART_ISOSURFACE,hiddensurface,SETTER
 objs,ENS_PART_ISOSURFACE,BOUNDINGREP,EMPTY
 objs,ENS_PART_ISOSURFACE,boundingrep,EMPTY
 objs,ENS_PART_ISOSURFACE,BOUNDINGREP,SETTER
@@ -8146,22 +8146,22 @@
 objs,ENS_PART_PARTICLE_TRACE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_PARTICLE_TRACE,reducepolygonsfactor,SETTER
 objs,ENS_PART_PARTICLE_TRACE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,eltshrinkfactor,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_PARTICLE_TRACE,eltshrinkfactor,SETTER
-objs,ENS_PART_PARTICLE_TRACE,CULLELEMENTS,EMPTY
-objs,ENS_PART_PARTICLE_TRACE,cullelements,EMPTY
-objs,ENS_PART_PARTICLE_TRACE,CULLELEMENTS,SETTER
-objs,ENS_PART_PARTICLE_TRACE,cullelements,SETTER
 objs,ENS_PART_PARTICLE_TRACE,ELTBLANKING,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,eltblanking,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,ELTBLANKING,SETTER
 objs,ENS_PART_PARTICLE_TRACE,eltblanking,SETTER
+objs,ENS_PART_PARTICLE_TRACE,CULLELEMENTS,EMPTY
+objs,ENS_PART_PARTICLE_TRACE,cullelements,EMPTY
+objs,ENS_PART_PARTICLE_TRACE,CULLELEMENTS,SETTER
+objs,ENS_PART_PARTICLE_TRACE,cullelements,SETTER
 objs,ENS_PART_PARTICLE_TRACE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,hiddensurface,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,HIDDENSURFACE,SETTER
 objs,ENS_PART_PARTICLE_TRACE,hiddensurface,SETTER
 objs,ENS_PART_PARTICLE_TRACE,BOUNDINGREP,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,boundingrep,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,BOUNDINGREP,SETTER
@@ -8322,22 +8322,22 @@
 objs,ENS_PART_PARTICLE_TRACE,massedballisticcoef,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,MASSEDBALLISTICCOEF,SETTER
 objs,ENS_PART_PARTICLE_TRACE,massedballisticcoef,SETTER
 objs,ENS_PART_PARTICLE_TRACE,MASSEDINITIALUSEFLUID,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,massedinitialusefluid,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,MASSEDINITIALUSEFLUID,SETTER
 objs,ENS_PART_PARTICLE_TRACE,massedinitialusefluid,SETTER
-objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITY,EMPTY
-objs,ENS_PART_PARTICLE_TRACE,massedfluiddensity,EMPTY
-objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITY,SETTER
-objs,ENS_PART_PARTICLE_TRACE,massedfluiddensity,SETTER
 objs,ENS_PART_PARTICLE_TRACE,MASSEDINITIALVELOCITY,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,massedinitialvelocity,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,MASSEDINITIALVELOCITY,SETTER
 objs,ENS_PART_PARTICLE_TRACE,massedinitialvelocity,SETTER
+objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITY,EMPTY
+objs,ENS_PART_PARTICLE_TRACE,massedfluiddensity,EMPTY
+objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITY,SETTER
+objs,ENS_PART_PARTICLE_TRACE,massedfluiddensity,SETTER
 objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITYVAL,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,massedfluiddensityval,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,MASSEDFLUIDDENSITYVAL,SETTER
 objs,ENS_PART_PARTICLE_TRACE,massedfluiddensityval,SETTER
 objs,ENS_PART_PARTICLE_TRACE,MASSEDGRAVITY,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,massedgravity,EMPTY
 objs,ENS_PART_PARTICLE_TRACE,MASSEDGRAVITY,SETTER
@@ -8832,22 +8832,22 @@
 objs,ENS_PART_PROFILE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_PROFILE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_PROFILE,reducepolygonsfactor,SETTER
 objs,ENS_PART_PROFILE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_PROFILE,eltshrinkfactor,EMPTY
 objs,ENS_PART_PROFILE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_PROFILE,eltshrinkfactor,SETTER
-objs,ENS_PART_PROFILE,CULLELEMENTS,EMPTY
-objs,ENS_PART_PROFILE,cullelements,EMPTY
-objs,ENS_PART_PROFILE,CULLELEMENTS,SETTER
-objs,ENS_PART_PROFILE,cullelements,SETTER
 objs,ENS_PART_PROFILE,ELTBLANKING,EMPTY
 objs,ENS_PART_PROFILE,eltblanking,EMPTY
 objs,ENS_PART_PROFILE,ELTBLANKING,SETTER
 objs,ENS_PART_PROFILE,eltblanking,SETTER
+objs,ENS_PART_PROFILE,CULLELEMENTS,EMPTY
+objs,ENS_PART_PROFILE,cullelements,EMPTY
+objs,ENS_PART_PROFILE,CULLELEMENTS,SETTER
+objs,ENS_PART_PROFILE,cullelements,SETTER
 objs,ENS_PART_PROFILE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_PROFILE,hiddensurface,EMPTY
 objs,ENS_PART_PROFILE,HIDDENSURFACE,SETTER
 objs,ENS_PART_PROFILE,hiddensurface,SETTER
 objs,ENS_PART_PROFILE,BOUNDINGREP,EMPTY
 objs,ENS_PART_PROFILE,boundingrep,EMPTY
 objs,ENS_PART_PROFILE,BOUNDINGREP,SETTER
@@ -9342,22 +9342,22 @@
 objs,ENS_PART_VECTOR_ARROW,reducepolygonsfactor,EMPTY
 objs,ENS_PART_VECTOR_ARROW,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_VECTOR_ARROW,reducepolygonsfactor,SETTER
 objs,ENS_PART_VECTOR_ARROW,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_VECTOR_ARROW,eltshrinkfactor,EMPTY
 objs,ENS_PART_VECTOR_ARROW,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_VECTOR_ARROW,eltshrinkfactor,SETTER
-objs,ENS_PART_VECTOR_ARROW,CULLELEMENTS,EMPTY
-objs,ENS_PART_VECTOR_ARROW,cullelements,EMPTY
-objs,ENS_PART_VECTOR_ARROW,CULLELEMENTS,SETTER
-objs,ENS_PART_VECTOR_ARROW,cullelements,SETTER
 objs,ENS_PART_VECTOR_ARROW,ELTBLANKING,EMPTY
 objs,ENS_PART_VECTOR_ARROW,eltblanking,EMPTY
 objs,ENS_PART_VECTOR_ARROW,ELTBLANKING,SETTER
 objs,ENS_PART_VECTOR_ARROW,eltblanking,SETTER
+objs,ENS_PART_VECTOR_ARROW,CULLELEMENTS,EMPTY
+objs,ENS_PART_VECTOR_ARROW,cullelements,EMPTY
+objs,ENS_PART_VECTOR_ARROW,CULLELEMENTS,SETTER
+objs,ENS_PART_VECTOR_ARROW,cullelements,SETTER
 objs,ENS_PART_VECTOR_ARROW,HIDDENSURFACE,EMPTY
 objs,ENS_PART_VECTOR_ARROW,hiddensurface,EMPTY
 objs,ENS_PART_VECTOR_ARROW,HIDDENSURFACE,SETTER
 objs,ENS_PART_VECTOR_ARROW,hiddensurface,SETTER
 objs,ENS_PART_VECTOR_ARROW,BOUNDINGREP,EMPTY
 objs,ENS_PART_VECTOR_ARROW,boundingrep,EMPTY
 objs,ENS_PART_VECTOR_ARROW,BOUNDINGREP,SETTER
@@ -9908,22 +9908,22 @@
 objs,ENS_PART_ELEVATED_SURFACE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,reducepolygonsfactor,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,eltshrinkfactor,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,eltshrinkfactor,SETTER
-objs,ENS_PART_ELEVATED_SURFACE,CULLELEMENTS,EMPTY
-objs,ENS_PART_ELEVATED_SURFACE,cullelements,EMPTY
-objs,ENS_PART_ELEVATED_SURFACE,CULLELEMENTS,SETTER
-objs,ENS_PART_ELEVATED_SURFACE,cullelements,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,ELTBLANKING,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,eltblanking,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,ELTBLANKING,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,eltblanking,SETTER
+objs,ENS_PART_ELEVATED_SURFACE,CULLELEMENTS,EMPTY
+objs,ENS_PART_ELEVATED_SURFACE,cullelements,EMPTY
+objs,ENS_PART_ELEVATED_SURFACE,CULLELEMENTS,SETTER
+objs,ENS_PART_ELEVATED_SURFACE,cullelements,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,hiddensurface,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,HIDDENSURFACE,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,hiddensurface,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,BOUNDINGREP,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,boundingrep,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,BOUNDINGREP,SETTER
@@ -9972,22 +9972,22 @@
 objs,ENS_PART_ELEVATED_SURFACE,usesurfacenormals,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,USESURFACENORMALS,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,usesurfacenormals,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,OFFSETFROMPART,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,offsetfrompart,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,OFFSETFROMPART,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,offsetfrompart,SETTER
-objs,ENS_PART_ELEVATED_SURFACE,OFFSETSCALE,EMPTY
-objs,ENS_PART_ELEVATED_SURFACE,offsetscale,EMPTY
-objs,ENS_PART_ELEVATED_SURFACE,OFFSETSCALE,SETTER
-objs,ENS_PART_ELEVATED_SURFACE,offsetscale,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,OFFSETVECTOR,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,offsetvector,EMPTY
 objs,ENS_PART_ELEVATED_SURFACE,OFFSETVECTOR,SETTER
 objs,ENS_PART_ELEVATED_SURFACE,offsetvector,SETTER
+objs,ENS_PART_ELEVATED_SURFACE,OFFSETSCALE,EMPTY
+objs,ENS_PART_ELEVATED_SURFACE,offsetscale,EMPTY
+objs,ENS_PART_ELEVATED_SURFACE,OFFSETSCALE,SETTER
+objs,ENS_PART_ELEVATED_SURFACE,offsetscale,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,objid,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,_update_attr_list,None
 objs,ENS_PART_DEVELOPED_SURFACE,_remote_obj,ensight.objs.wrap_id(1)
 objs,ENS_PART_DEVELOPED_SURFACE,createpart,ensight.objs.wrap_id(1).createpart(1,0=0)
 objs,ENS_PART_DEVELOPED_SURFACE,attrgroupinfo,ensight.objs.wrap_id(1).attrgroupinfo(1,0=0)
 objs,ENS_PART_DEVELOPED_SURFACE,realtimemode,ensight.objs.wrap_id(1).realtimemode(1,0=0)
 objs,ENS_PART_DEVELOPED_SURFACE,tracepaths,ensight.objs.wrap_id(1).tracepaths(variables=0)
@@ -10430,22 +10430,22 @@
 objs,ENS_PART_DEVELOPED_SURFACE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,reducepolygonsfactor,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,eltshrinkfactor,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,eltshrinkfactor,SETTER
-objs,ENS_PART_DEVELOPED_SURFACE,CULLELEMENTS,EMPTY
-objs,ENS_PART_DEVELOPED_SURFACE,cullelements,EMPTY
-objs,ENS_PART_DEVELOPED_SURFACE,CULLELEMENTS,SETTER
-objs,ENS_PART_DEVELOPED_SURFACE,cullelements,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,ELTBLANKING,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,eltblanking,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,ELTBLANKING,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,eltblanking,SETTER
+objs,ENS_PART_DEVELOPED_SURFACE,CULLELEMENTS,EMPTY
+objs,ENS_PART_DEVELOPED_SURFACE,cullelements,EMPTY
+objs,ENS_PART_DEVELOPED_SURFACE,CULLELEMENTS,SETTER
+objs,ENS_PART_DEVELOPED_SURFACE,cullelements,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,hiddensurface,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,HIDDENSURFACE,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,hiddensurface,SETTER
 objs,ENS_PART_DEVELOPED_SURFACE,BOUNDINGREP,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,boundingrep,EMPTY
 objs,ENS_PART_DEVELOPED_SURFACE,BOUNDINGREP,SETTER
@@ -10940,22 +10940,22 @@
 objs,ENS_PART_BUILT_UP,reducepolygonsfactor,EMPTY
 objs,ENS_PART_BUILT_UP,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_BUILT_UP,reducepolygonsfactor,SETTER
 objs,ENS_PART_BUILT_UP,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_BUILT_UP,eltshrinkfactor,EMPTY
 objs,ENS_PART_BUILT_UP,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_BUILT_UP,eltshrinkfactor,SETTER
-objs,ENS_PART_BUILT_UP,CULLELEMENTS,EMPTY
-objs,ENS_PART_BUILT_UP,cullelements,EMPTY
-objs,ENS_PART_BUILT_UP,CULLELEMENTS,SETTER
-objs,ENS_PART_BUILT_UP,cullelements,SETTER
 objs,ENS_PART_BUILT_UP,ELTBLANKING,EMPTY
 objs,ENS_PART_BUILT_UP,eltblanking,EMPTY
 objs,ENS_PART_BUILT_UP,ELTBLANKING,SETTER
 objs,ENS_PART_BUILT_UP,eltblanking,SETTER
+objs,ENS_PART_BUILT_UP,CULLELEMENTS,EMPTY
+objs,ENS_PART_BUILT_UP,cullelements,EMPTY
+objs,ENS_PART_BUILT_UP,CULLELEMENTS,SETTER
+objs,ENS_PART_BUILT_UP,cullelements,SETTER
 objs,ENS_PART_BUILT_UP,HIDDENSURFACE,EMPTY
 objs,ENS_PART_BUILT_UP,hiddensurface,EMPTY
 objs,ENS_PART_BUILT_UP,HIDDENSURFACE,SETTER
 objs,ENS_PART_BUILT_UP,hiddensurface,SETTER
 objs,ENS_PART_BUILT_UP,BOUNDINGREP,EMPTY
 objs,ENS_PART_BUILT_UP,boundingrep,EMPTY
 objs,ENS_PART_BUILT_UP,BOUNDINGREP,SETTER
@@ -11430,22 +11430,22 @@
 objs,ENS_PART_TENSOR_GLYPH,reducepolygonsfactor,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_TENSOR_GLYPH,reducepolygonsfactor,SETTER
 objs,ENS_PART_TENSOR_GLYPH,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,eltshrinkfactor,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_TENSOR_GLYPH,eltshrinkfactor,SETTER
-objs,ENS_PART_TENSOR_GLYPH,CULLELEMENTS,EMPTY
-objs,ENS_PART_TENSOR_GLYPH,cullelements,EMPTY
-objs,ENS_PART_TENSOR_GLYPH,CULLELEMENTS,SETTER
-objs,ENS_PART_TENSOR_GLYPH,cullelements,SETTER
 objs,ENS_PART_TENSOR_GLYPH,ELTBLANKING,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,eltblanking,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,ELTBLANKING,SETTER
 objs,ENS_PART_TENSOR_GLYPH,eltblanking,SETTER
+objs,ENS_PART_TENSOR_GLYPH,CULLELEMENTS,EMPTY
+objs,ENS_PART_TENSOR_GLYPH,cullelements,EMPTY
+objs,ENS_PART_TENSOR_GLYPH,CULLELEMENTS,SETTER
+objs,ENS_PART_TENSOR_GLYPH,cullelements,SETTER
 objs,ENS_PART_TENSOR_GLYPH,HIDDENSURFACE,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,hiddensurface,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,HIDDENSURFACE,SETTER
 objs,ENS_PART_TENSOR_GLYPH,hiddensurface,SETTER
 objs,ENS_PART_TENSOR_GLYPH,BOUNDINGREP,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,boundingrep,EMPTY
 objs,ENS_PART_TENSOR_GLYPH,BOUNDINGREP,SETTER
@@ -11972,22 +11972,22 @@
 objs,ENS_PART_FX_VORTEX_CORE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,reducepolygonsfactor,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,eltshrinkfactor,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,eltshrinkfactor,SETTER
-objs,ENS_PART_FX_VORTEX_CORE,CULLELEMENTS,EMPTY
-objs,ENS_PART_FX_VORTEX_CORE,cullelements,EMPTY
-objs,ENS_PART_FX_VORTEX_CORE,CULLELEMENTS,SETTER
-objs,ENS_PART_FX_VORTEX_CORE,cullelements,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,ELTBLANKING,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,eltblanking,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,ELTBLANKING,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,eltblanking,SETTER
+objs,ENS_PART_FX_VORTEX_CORE,CULLELEMENTS,EMPTY
+objs,ENS_PART_FX_VORTEX_CORE,cullelements,EMPTY
+objs,ENS_PART_FX_VORTEX_CORE,CULLELEMENTS,SETTER
+objs,ENS_PART_FX_VORTEX_CORE,cullelements,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,hiddensurface,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,HIDDENSURFACE,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,hiddensurface,SETTER
 objs,ENS_PART_FX_VORTEX_CORE,BOUNDINGREP,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,boundingrep,EMPTY
 objs,ENS_PART_FX_VORTEX_CORE,BOUNDINGREP,SETTER
@@ -12502,22 +12502,22 @@
 objs,ENS_PART_FX_SHOCK,reducepolygonsfactor,EMPTY
 objs,ENS_PART_FX_SHOCK,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_FX_SHOCK,reducepolygonsfactor,SETTER
 objs,ENS_PART_FX_SHOCK,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_FX_SHOCK,eltshrinkfactor,EMPTY
 objs,ENS_PART_FX_SHOCK,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_FX_SHOCK,eltshrinkfactor,SETTER
-objs,ENS_PART_FX_SHOCK,CULLELEMENTS,EMPTY
-objs,ENS_PART_FX_SHOCK,cullelements,EMPTY
-objs,ENS_PART_FX_SHOCK,CULLELEMENTS,SETTER
-objs,ENS_PART_FX_SHOCK,cullelements,SETTER
 objs,ENS_PART_FX_SHOCK,ELTBLANKING,EMPTY
 objs,ENS_PART_FX_SHOCK,eltblanking,EMPTY
 objs,ENS_PART_FX_SHOCK,ELTBLANKING,SETTER
 objs,ENS_PART_FX_SHOCK,eltblanking,SETTER
+objs,ENS_PART_FX_SHOCK,CULLELEMENTS,EMPTY
+objs,ENS_PART_FX_SHOCK,cullelements,EMPTY
+objs,ENS_PART_FX_SHOCK,CULLELEMENTS,SETTER
+objs,ENS_PART_FX_SHOCK,cullelements,SETTER
 objs,ENS_PART_FX_SHOCK,HIDDENSURFACE,EMPTY
 objs,ENS_PART_FX_SHOCK,hiddensurface,EMPTY
 objs,ENS_PART_FX_SHOCK,HIDDENSURFACE,SETTER
 objs,ENS_PART_FX_SHOCK,hiddensurface,SETTER
 objs,ENS_PART_FX_SHOCK,BOUNDINGREP,EMPTY
 objs,ENS_PART_FX_SHOCK,boundingrep,EMPTY
 objs,ENS_PART_FX_SHOCK,BOUNDINGREP,SETTER
@@ -13052,22 +13052,22 @@
 objs,ENS_PART_FX_SEP_ATT,reducepolygonsfactor,EMPTY
 objs,ENS_PART_FX_SEP_ATT,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_FX_SEP_ATT,reducepolygonsfactor,SETTER
 objs,ENS_PART_FX_SEP_ATT,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_FX_SEP_ATT,eltshrinkfactor,EMPTY
 objs,ENS_PART_FX_SEP_ATT,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_FX_SEP_ATT,eltshrinkfactor,SETTER
-objs,ENS_PART_FX_SEP_ATT,CULLELEMENTS,EMPTY
-objs,ENS_PART_FX_SEP_ATT,cullelements,EMPTY
-objs,ENS_PART_FX_SEP_ATT,CULLELEMENTS,SETTER
-objs,ENS_PART_FX_SEP_ATT,cullelements,SETTER
 objs,ENS_PART_FX_SEP_ATT,ELTBLANKING,EMPTY
 objs,ENS_PART_FX_SEP_ATT,eltblanking,EMPTY
 objs,ENS_PART_FX_SEP_ATT,ELTBLANKING,SETTER
 objs,ENS_PART_FX_SEP_ATT,eltblanking,SETTER
+objs,ENS_PART_FX_SEP_ATT,CULLELEMENTS,EMPTY
+objs,ENS_PART_FX_SEP_ATT,cullelements,EMPTY
+objs,ENS_PART_FX_SEP_ATT,CULLELEMENTS,SETTER
+objs,ENS_PART_FX_SEP_ATT,cullelements,SETTER
 objs,ENS_PART_FX_SEP_ATT,HIDDENSURFACE,EMPTY
 objs,ENS_PART_FX_SEP_ATT,hiddensurface,EMPTY
 objs,ENS_PART_FX_SEP_ATT,HIDDENSURFACE,SETTER
 objs,ENS_PART_FX_SEP_ATT,hiddensurface,SETTER
 objs,ENS_PART_FX_SEP_ATT,BOUNDINGREP,EMPTY
 objs,ENS_PART_FX_SEP_ATT,boundingrep,EMPTY
 objs,ENS_PART_FX_SEP_ATT,BOUNDINGREP,SETTER
@@ -13582,22 +13582,22 @@
 objs,ENS_PART_MAT_INTERFACE,reducepolygonsfactor,EMPTY
 objs,ENS_PART_MAT_INTERFACE,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_MAT_INTERFACE,reducepolygonsfactor,SETTER
 objs,ENS_PART_MAT_INTERFACE,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_MAT_INTERFACE,eltshrinkfactor,EMPTY
 objs,ENS_PART_MAT_INTERFACE,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_MAT_INTERFACE,eltshrinkfactor,SETTER
-objs,ENS_PART_MAT_INTERFACE,CULLELEMENTS,EMPTY
-objs,ENS_PART_MAT_INTERFACE,cullelements,EMPTY
-objs,ENS_PART_MAT_INTERFACE,CULLELEMENTS,SETTER
-objs,ENS_PART_MAT_INTERFACE,cullelements,SETTER
 objs,ENS_PART_MAT_INTERFACE,ELTBLANKING,EMPTY
 objs,ENS_PART_MAT_INTERFACE,eltblanking,EMPTY
 objs,ENS_PART_MAT_INTERFACE,ELTBLANKING,SETTER
 objs,ENS_PART_MAT_INTERFACE,eltblanking,SETTER
+objs,ENS_PART_MAT_INTERFACE,CULLELEMENTS,EMPTY
+objs,ENS_PART_MAT_INTERFACE,cullelements,EMPTY
+objs,ENS_PART_MAT_INTERFACE,CULLELEMENTS,SETTER
+objs,ENS_PART_MAT_INTERFACE,cullelements,SETTER
 objs,ENS_PART_MAT_INTERFACE,HIDDENSURFACE,EMPTY
 objs,ENS_PART_MAT_INTERFACE,hiddensurface,EMPTY
 objs,ENS_PART_MAT_INTERFACE,HIDDENSURFACE,SETTER
 objs,ENS_PART_MAT_INTERFACE,hiddensurface,SETTER
 objs,ENS_PART_MAT_INTERFACE,BOUNDINGREP,EMPTY
 objs,ENS_PART_MAT_INTERFACE,boundingrep,EMPTY
 objs,ENS_PART_MAT_INTERFACE,BOUNDINGREP,SETTER
@@ -14076,22 +14076,22 @@
 objs,ENS_PART_POINT,reducepolygonsfactor,EMPTY
 objs,ENS_PART_POINT,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_POINT,reducepolygonsfactor,SETTER
 objs,ENS_PART_POINT,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_POINT,eltshrinkfactor,EMPTY
 objs,ENS_PART_POINT,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_POINT,eltshrinkfactor,SETTER
-objs,ENS_PART_POINT,CULLELEMENTS,EMPTY
-objs,ENS_PART_POINT,cullelements,EMPTY
-objs,ENS_PART_POINT,CULLELEMENTS,SETTER
-objs,ENS_PART_POINT,cullelements,SETTER
 objs,ENS_PART_POINT,ELTBLANKING,EMPTY
 objs,ENS_PART_POINT,eltblanking,EMPTY
 objs,ENS_PART_POINT,ELTBLANKING,SETTER
 objs,ENS_PART_POINT,eltblanking,SETTER
+objs,ENS_PART_POINT,CULLELEMENTS,EMPTY
+objs,ENS_PART_POINT,cullelements,EMPTY
+objs,ENS_PART_POINT,CULLELEMENTS,SETTER
+objs,ENS_PART_POINT,cullelements,SETTER
 objs,ENS_PART_POINT,HIDDENSURFACE,EMPTY
 objs,ENS_PART_POINT,hiddensurface,EMPTY
 objs,ENS_PART_POINT,HIDDENSURFACE,SETTER
 objs,ENS_PART_POINT,hiddensurface,SETTER
 objs,ENS_PART_POINT,BOUNDINGREP,EMPTY
 objs,ENS_PART_POINT,boundingrep,EMPTY
 objs,ENS_PART_POINT,BOUNDINGREP,SETTER
@@ -14566,22 +14566,22 @@
 objs,ENS_PART_AXISYMMETRIC,reducepolygonsfactor,EMPTY
 objs,ENS_PART_AXISYMMETRIC,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_AXISYMMETRIC,reducepolygonsfactor,SETTER
 objs,ENS_PART_AXISYMMETRIC,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_AXISYMMETRIC,eltshrinkfactor,EMPTY
 objs,ENS_PART_AXISYMMETRIC,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_AXISYMMETRIC,eltshrinkfactor,SETTER
-objs,ENS_PART_AXISYMMETRIC,CULLELEMENTS,EMPTY
-objs,ENS_PART_AXISYMMETRIC,cullelements,EMPTY
-objs,ENS_PART_AXISYMMETRIC,CULLELEMENTS,SETTER
-objs,ENS_PART_AXISYMMETRIC,cullelements,SETTER
 objs,ENS_PART_AXISYMMETRIC,ELTBLANKING,EMPTY
 objs,ENS_PART_AXISYMMETRIC,eltblanking,EMPTY
 objs,ENS_PART_AXISYMMETRIC,ELTBLANKING,SETTER
 objs,ENS_PART_AXISYMMETRIC,eltblanking,SETTER
+objs,ENS_PART_AXISYMMETRIC,CULLELEMENTS,EMPTY
+objs,ENS_PART_AXISYMMETRIC,cullelements,EMPTY
+objs,ENS_PART_AXISYMMETRIC,CULLELEMENTS,SETTER
+objs,ENS_PART_AXISYMMETRIC,cullelements,SETTER
 objs,ENS_PART_AXISYMMETRIC,HIDDENSURFACE,EMPTY
 objs,ENS_PART_AXISYMMETRIC,hiddensurface,EMPTY
 objs,ENS_PART_AXISYMMETRIC,HIDDENSURFACE,SETTER
 objs,ENS_PART_AXISYMMETRIC,hiddensurface,SETTER
 objs,ENS_PART_AXISYMMETRIC,BOUNDINGREP,EMPTY
 objs,ENS_PART_AXISYMMETRIC,boundingrep,EMPTY
 objs,ENS_PART_AXISYMMETRIC,BOUNDINGREP,SETTER
@@ -15092,22 +15092,22 @@
 objs,ENS_PART_VOF,reducepolygonsfactor,EMPTY
 objs,ENS_PART_VOF,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_VOF,reducepolygonsfactor,SETTER
 objs,ENS_PART_VOF,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_VOF,eltshrinkfactor,EMPTY
 objs,ENS_PART_VOF,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_VOF,eltshrinkfactor,SETTER
-objs,ENS_PART_VOF,CULLELEMENTS,EMPTY
-objs,ENS_PART_VOF,cullelements,EMPTY
-objs,ENS_PART_VOF,CULLELEMENTS,SETTER
-objs,ENS_PART_VOF,cullelements,SETTER
 objs,ENS_PART_VOF,ELTBLANKING,EMPTY
 objs,ENS_PART_VOF,eltblanking,EMPTY
 objs,ENS_PART_VOF,ELTBLANKING,SETTER
 objs,ENS_PART_VOF,eltblanking,SETTER
+objs,ENS_PART_VOF,CULLELEMENTS,EMPTY
+objs,ENS_PART_VOF,cullelements,EMPTY
+objs,ENS_PART_VOF,CULLELEMENTS,SETTER
+objs,ENS_PART_VOF,cullelements,SETTER
 objs,ENS_PART_VOF,HIDDENSURFACE,EMPTY
 objs,ENS_PART_VOF,hiddensurface,EMPTY
 objs,ENS_PART_VOF,HIDDENSURFACE,SETTER
 objs,ENS_PART_VOF,hiddensurface,SETTER
 objs,ENS_PART_VOF,BOUNDINGREP,EMPTY
 objs,ENS_PART_VOF,boundingrep,EMPTY
 objs,ENS_PART_VOF,BOUNDINGREP,SETTER
@@ -15240,22 +15240,22 @@
 objs,ENS_PART_VOF,specifycellcompnum,EMPTY
 objs,ENS_PART_VOF,SPECIFYCELLCOMPNUM,SETTER
 objs,ENS_PART_VOF,specifycellcompnum,SETTER
 objs,ENS_PART_VOF,CELLCOMPNUM,EMPTY
 objs,ENS_PART_VOF,cellcompnum,EMPTY
 objs,ENS_PART_VOF,CELLCOMPNUM,SETTER
 objs,ENS_PART_VOF,cellcompnum,SETTER
-objs,ENS_PART_VOF,COOLINGCHANNELCOMP,EMPTY
-objs,ENS_PART_VOF,coolingchannelcomp,EMPTY
-objs,ENS_PART_VOF,COOLINGCHANNELCOMP,SETTER
-objs,ENS_PART_VOF,coolingchannelcomp,SETTER
 objs,ENS_PART_VOF,BLANKINGVARIABLE1,EMPTY
 objs,ENS_PART_VOF,blankingvariable1,EMPTY
 objs,ENS_PART_VOF,BLANKINGVARIABLE1,SETTER
 objs,ENS_PART_VOF,blankingvariable1,SETTER
+objs,ENS_PART_VOF,COOLINGCHANNELCOMP,EMPTY
+objs,ENS_PART_VOF,coolingchannelcomp,EMPTY
+objs,ENS_PART_VOF,COOLINGCHANNELCOMP,SETTER
+objs,ENS_PART_VOF,coolingchannelcomp,SETTER
 objs,ENS_PART_VOF,BLANKINGVARIABLE2,EMPTY
 objs,ENS_PART_VOF,blankingvariable2,EMPTY
 objs,ENS_PART_VOF,BLANKINGVARIABLE2,SETTER
 objs,ENS_PART_VOF,blankingvariable2,SETTER
 objs,ENS_PART_VOF,VOFISOZTEST,EMPTY
 objs,ENS_PART_VOF,vofisoztest,EMPTY
 objs,ENS_PART_VOF,VOFISOZTEST,SETTER
@@ -15750,22 +15750,22 @@
 objs,ENS_PART_AUX_GEOM,reducepolygonsfactor,EMPTY
 objs,ENS_PART_AUX_GEOM,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_AUX_GEOM,reducepolygonsfactor,SETTER
 objs,ENS_PART_AUX_GEOM,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_AUX_GEOM,eltshrinkfactor,EMPTY
 objs,ENS_PART_AUX_GEOM,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_AUX_GEOM,eltshrinkfactor,SETTER
-objs,ENS_PART_AUX_GEOM,CULLELEMENTS,EMPTY
-objs,ENS_PART_AUX_GEOM,cullelements,EMPTY
-objs,ENS_PART_AUX_GEOM,CULLELEMENTS,SETTER
-objs,ENS_PART_AUX_GEOM,cullelements,SETTER
 objs,ENS_PART_AUX_GEOM,ELTBLANKING,EMPTY
 objs,ENS_PART_AUX_GEOM,eltblanking,EMPTY
 objs,ENS_PART_AUX_GEOM,ELTBLANKING,SETTER
 objs,ENS_PART_AUX_GEOM,eltblanking,SETTER
+objs,ENS_PART_AUX_GEOM,CULLELEMENTS,EMPTY
+objs,ENS_PART_AUX_GEOM,cullelements,EMPTY
+objs,ENS_PART_AUX_GEOM,CULLELEMENTS,SETTER
+objs,ENS_PART_AUX_GEOM,cullelements,SETTER
 objs,ENS_PART_AUX_GEOM,HIDDENSURFACE,EMPTY
 objs,ENS_PART_AUX_GEOM,hiddensurface,EMPTY
 objs,ENS_PART_AUX_GEOM,HIDDENSURFACE,SETTER
 objs,ENS_PART_AUX_GEOM,hiddensurface,SETTER
 objs,ENS_PART_AUX_GEOM,BOUNDINGREP,EMPTY
 objs,ENS_PART_AUX_GEOM,boundingrep,EMPTY
 objs,ENS_PART_AUX_GEOM,BOUNDINGREP,SETTER
@@ -16288,22 +16288,22 @@
 objs,ENS_PART_FILTER,reducepolygonsfactor,EMPTY
 objs,ENS_PART_FILTER,REDUCEPOLYGONSFACTOR,SETTER
 objs,ENS_PART_FILTER,reducepolygonsfactor,SETTER
 objs,ENS_PART_FILTER,ELTSHRINKFACTOR,EMPTY
 objs,ENS_PART_FILTER,eltshrinkfactor,EMPTY
 objs,ENS_PART_FILTER,ELTSHRINKFACTOR,SETTER
 objs,ENS_PART_FILTER,eltshrinkfactor,SETTER
-objs,ENS_PART_FILTER,CULLELEMENTS,EMPTY
-objs,ENS_PART_FILTER,cullelements,EMPTY
-objs,ENS_PART_FILTER,CULLELEMENTS,SETTER
-objs,ENS_PART_FILTER,cullelements,SETTER
 objs,ENS_PART_FILTER,ELTBLANKING,EMPTY
 objs,ENS_PART_FILTER,eltblanking,EMPTY
 objs,ENS_PART_FILTER,ELTBLANKING,SETTER
 objs,ENS_PART_FILTER,eltblanking,SETTER
+objs,ENS_PART_FILTER,CULLELEMENTS,EMPTY
+objs,ENS_PART_FILTER,cullelements,EMPTY
+objs,ENS_PART_FILTER,CULLELEMENTS,SETTER
+objs,ENS_PART_FILTER,cullelements,SETTER
 objs,ENS_PART_FILTER,HIDDENSURFACE,EMPTY
 objs,ENS_PART_FILTER,hiddensurface,EMPTY
 objs,ENS_PART_FILTER,HIDDENSURFACE,SETTER
 objs,ENS_PART_FILTER,hiddensurface,SETTER
 objs,ENS_PART_FILTER,BOUNDINGREP,EMPTY
 objs,ENS_PART_FILTER,boundingrep,EMPTY
 objs,ENS_PART_FILTER,BOUNDINGREP,SETTER
@@ -16610,18 +16610,14 @@
 objs,ENS_PLOTTER,subgridrgb,EMPTY
 objs,ENS_PLOTTER,SUBGRIDRGB,SETTER
 objs,ENS_PLOTTER,subgridrgb,SETTER
 objs,ENS_PLOTTER,AXISXTITLE,EMPTY
 objs,ENS_PLOTTER,axisxtitle,EMPTY
 objs,ENS_PLOTTER,AXISXTITLE,SETTER
 objs,ENS_PLOTTER,axisxtitle,SETTER
-objs,ENS_PLOTTER,AXISYTITLE,EMPTY
-objs,ENS_PLOTTER,axisytitle,EMPTY
-objs,ENS_PLOTTER,AXISYTITLE,SETTER
-objs,ENS_PLOTTER,axisytitle,SETTER
 objs,ENS_PLOTTER,AXISXTITLESIZE,EMPTY
 objs,ENS_PLOTTER,axisxtitlesize,EMPTY
 objs,ENS_PLOTTER,AXISXTITLESIZE,SETTER
 objs,ENS_PLOTTER,axisxtitlesize,SETTER
 objs,ENS_PLOTTER,AXISXMIN,EMPTY
 objs,ENS_PLOTTER,axisxmin,EMPTY
 objs,ENS_PLOTTER,AXISXMIN,SETTER
@@ -16646,14 +16642,18 @@
 objs,ENS_PLOTTER,axisxsgridtype,EMPTY
 objs,ENS_PLOTTER,AXISXSGRIDTYPE,SETTER
 objs,ENS_PLOTTER,axisxsgridtype,SETTER
 objs,ENS_PLOTTER,AXISXNUMSUBGRID,EMPTY
 objs,ENS_PLOTTER,axisxnumsubgrid,EMPTY
 objs,ENS_PLOTTER,AXISXNUMSUBGRID,SETTER
 objs,ENS_PLOTTER,axisxnumsubgrid,SETTER
+objs,ENS_PLOTTER,AXISYTITLE,EMPTY
+objs,ENS_PLOTTER,axisytitle,EMPTY
+objs,ENS_PLOTTER,AXISYTITLE,SETTER
+objs,ENS_PLOTTER,axisytitle,SETTER
 objs,ENS_PLOTTER,AXISYTITLESIZE,EMPTY
 objs,ENS_PLOTTER,axisytitlesize,EMPTY
 objs,ENS_PLOTTER,AXISYTITLESIZE,SETTER
 objs,ENS_PLOTTER,axisytitlesize,SETTER
 objs,ENS_PLOTTER,AXISYMIN,EMPTY
 objs,ENS_PLOTTER,axisymin,EMPTY
 objs,ENS_PLOTTER,AXISYMIN,SETTER
@@ -18389,18 +18389,14 @@
 objs,ENS_VPORT,subtickscalefactor,EMPTY
 objs,ENS_VPORT,SUBTICKSCALEFACTOR,SETTER
 objs,ENS_VPORT,subtickscalefactor,SETTER
 objs,ENS_VPORT,AXISXTITLE,EMPTY
 objs,ENS_VPORT,axisxtitle,EMPTY
 objs,ENS_VPORT,AXISXTITLE,SETTER
 objs,ENS_VPORT,axisxtitle,SETTER
-objs,ENS_VPORT,AXISYTITLE,EMPTY
-objs,ENS_VPORT,axisytitle,EMPTY
-objs,ENS_VPORT,AXISYTITLE,SETTER
-objs,ENS_VPORT,axisytitle,SETTER
 objs,ENS_VPORT,AXISXTITLESIZE,EMPTY
 objs,ENS_VPORT,axisxtitlesize,EMPTY
 objs,ENS_VPORT,AXISXTITLESIZE,SETTER
 objs,ENS_VPORT,axisxtitlesize,SETTER
 objs,ENS_VPORT,AXISXMIN,EMPTY
 objs,ENS_VPORT,axisxmin,EMPTY
 objs,ENS_VPORT,AXISXMIN,SETTER
@@ -18481,14 +18477,18 @@
 objs,ENS_VPORT,axisxnumsubgrid,EMPTY
 objs,ENS_VPORT,AXISXNUMSUBGRID,SETTER
 objs,ENS_VPORT,axisxnumsubgrid,SETTER
 objs,ENS_VPORT,AXISXGRIDEXTENTLOC,EMPTY
 objs,ENS_VPORT,axisxgridextentloc,EMPTY
 objs,ENS_VPORT,AXISXGRIDEXTENTLOC,SETTER
 objs,ENS_VPORT,axisxgridextentloc,SETTER
+objs,ENS_VPORT,AXISYTITLE,EMPTY
+objs,ENS_VPORT,axisytitle,EMPTY
+objs,ENS_VPORT,AXISYTITLE,SETTER
+objs,ENS_VPORT,axisytitle,SETTER
 objs,ENS_VPORT,AXISYTITLESIZE,EMPTY
 objs,ENS_VPORT,axisytitlesize,EMPTY
 objs,ENS_VPORT,AXISYTITLESIZE,SETTER
 objs,ENS_VPORT,axisytitlesize,SETTER
 objs,ENS_VPORT,AXISYMIN,EMPTY
 objs,ENS_VPORT,axisymin,EMPTY
 objs,ENS_VPORT,AXISYMIN,SETTER
@@ -18505,22 +18505,22 @@
 objs,ENS_VPORT,axisheight,EMPTY
 objs,ENS_VPORT,AXISHEIGHT,SETTER
 objs,ENS_VPORT,axisheight,SETTER
 objs,ENS_VPORT,AXISYLABELAXISLOC,EMPTY
 objs,ENS_VPORT,axisylabelaxisloc,EMPTY
 objs,ENS_VPORT,AXISYLABELAXISLOC,SETTER
 objs,ENS_VPORT,axisylabelaxisloc,SETTER
-objs,ENS_VPORT,AXISYLABELFILTER,EMPTY
-objs,ENS_VPORT,axisylabelfilter,EMPTY
-objs,ENS_VPORT,AXISYLABELFILTER,SETTER
-objs,ENS_VPORT,axisylabelfilter,SETTER
 objs,ENS_VPORT,AXISYLABELEXTENTLOC,EMPTY
 objs,ENS_VPORT,axisylabelextentloc,EMPTY
 objs,ENS_VPORT,AXISYLABELEXTENTLOC,SETTER
 objs,ENS_VPORT,axisylabelextentloc,SETTER
+objs,ENS_VPORT,AXISYLABELFILTER,EMPTY
+objs,ENS_VPORT,axisylabelfilter,EMPTY
+objs,ENS_VPORT,AXISYLABELFILTER,SETTER
+objs,ENS_VPORT,axisylabelfilter,SETTER
 objs,ENS_VPORT,AXISYFORMAT,EMPTY
 objs,ENS_VPORT,axisyformat,EMPTY
 objs,ENS_VPORT,AXISYFORMAT,SETTER
 objs,ENS_VPORT,axisyformat,SETTER
 objs,ENS_VPORT,AXISYLABELRGB,EMPTY
 objs,ENS_VPORT,axisylabelrgb,EMPTY
 objs,ENS_VPORT,AXISYLABELRGB,SETTER
@@ -18593,22 +18593,22 @@
 objs,ENS_VPORT,axiszmax,EMPTY
 objs,ENS_VPORT,AXISZMAX,SETTER
 objs,ENS_VPORT,axiszmax,SETTER
 objs,ENS_VPORT,AXISZLABELAXISLOC,EMPTY
 objs,ENS_VPORT,axiszlabelaxisloc,EMPTY
 objs,ENS_VPORT,AXISZLABELAXISLOC,SETTER
 objs,ENS_VPORT,axiszlabelaxisloc,SETTER
-objs,ENS_VPORT,AXISZLABELFILTER,EMPTY
-objs,ENS_VPORT,axiszlabelfilter,EMPTY
-objs,ENS_VPORT,AXISZLABELFILTER,SETTER
-objs,ENS_VPORT,axiszlabelfilter,SETTER
 objs,ENS_VPORT,AXISZLABELEXTENTLOC,EMPTY
 objs,ENS_VPORT,axiszlabelextentloc,EMPTY
 objs,ENS_VPORT,AXISZLABELEXTENTLOC,SETTER
 objs,ENS_VPORT,axiszlabelextentloc,SETTER
+objs,ENS_VPORT,AXISZLABELFILTER,EMPTY
+objs,ENS_VPORT,axiszlabelfilter,EMPTY
+objs,ENS_VPORT,AXISZLABELFILTER,SETTER
+objs,ENS_VPORT,axiszlabelfilter,SETTER
 objs,ENS_VPORT,AXISZFORMAT,EMPTY
 objs,ENS_VPORT,axiszformat,EMPTY
 objs,ENS_VPORT,AXISZFORMAT,SETTER
 objs,ENS_VPORT,axiszformat,SETTER
 objs,ENS_VPORT,AXISZLABELRGB,EMPTY
 objs,ENS_VPORT,axiszlabelrgb,EMPTY
 objs,ENS_VPORT,AXISZLABELRGB,SETTER
@@ -18661,14 +18661,18 @@
 objs,ENS_VPORT,facexmingrid,EMPTY
 objs,ENS_VPORT,FACEXMINGRID,SETTER
 objs,ENS_VPORT,facexmingrid,SETTER
 objs,ENS_VPORT,FACEXMINSUBGRID,EMPTY
 objs,ENS_VPORT,facexminsubgrid,EMPTY
 objs,ENS_VPORT,FACEXMINSUBGRID,SETTER
 objs,ENS_VPORT,facexminsubgrid,SETTER
+objs,ENS_VPORT,FACEXMINGRIDFILTER,EMPTY
+objs,ENS_VPORT,facexmingridfilter,EMPTY
+objs,ENS_VPORT,FACEXMINGRIDFILTER,SETTER
+objs,ENS_VPORT,facexmingridfilter,SETTER
 objs,ENS_VPORT,FACEYMINGRID,EMPTY
 objs,ENS_VPORT,faceymingrid,EMPTY
 objs,ENS_VPORT,FACEYMINGRID,SETTER
 objs,ENS_VPORT,faceymingrid,SETTER
 objs,ENS_VPORT,FACEYMINSUBGRID,EMPTY
 objs,ENS_VPORT,faceyminsubgrid,EMPTY
 objs,ENS_VPORT,FACEYMINSUBGRID,SETTER
@@ -18685,54 +18689,50 @@
 objs,ENS_VPORT,facezminsubgrid,EMPTY
 objs,ENS_VPORT,FACEZMINSUBGRID,SETTER
 objs,ENS_VPORT,facezminsubgrid,SETTER
 objs,ENS_VPORT,FACEZMINGRIDFILTER,EMPTY
 objs,ENS_VPORT,facezmingridfilter,EMPTY
 objs,ENS_VPORT,FACEZMINGRIDFILTER,SETTER
 objs,ENS_VPORT,facezmingridfilter,SETTER
-objs,ENS_VPORT,FACEXMINGRIDFILTER,EMPTY
-objs,ENS_VPORT,facexmingridfilter,EMPTY
-objs,ENS_VPORT,FACEXMINGRIDFILTER,SETTER
-objs,ENS_VPORT,facexmingridfilter,SETTER
-objs,ENS_VPORT,FACEZMAXGRID,EMPTY
-objs,ENS_VPORT,facezmaxgrid,EMPTY
-objs,ENS_VPORT,FACEZMAXGRID,SETTER
-objs,ENS_VPORT,facezmaxgrid,SETTER
-objs,ENS_VPORT,FACEZMAXGRIDFILTER,EMPTY
-objs,ENS_VPORT,facezmaxgridfilter,EMPTY
-objs,ENS_VPORT,FACEZMAXGRIDFILTER,SETTER
-objs,ENS_VPORT,facezmaxgridfilter,SETTER
+objs,ENS_VPORT,FACEXMAXGRID,EMPTY
+objs,ENS_VPORT,facexmaxgrid,EMPTY
+objs,ENS_VPORT,FACEXMAXGRID,SETTER
+objs,ENS_VPORT,facexmaxgrid,SETTER
+objs,ENS_VPORT,FACEXMAXSUBGRID,EMPTY
+objs,ENS_VPORT,facexmaxsubgrid,EMPTY
+objs,ENS_VPORT,FACEXMAXSUBGRID,SETTER
+objs,ENS_VPORT,facexmaxsubgrid,SETTER
+objs,ENS_VPORT,FACEXMAXGRIDFILTER,EMPTY
+objs,ENS_VPORT,facexmaxgridfilter,EMPTY
+objs,ENS_VPORT,FACEXMAXGRIDFILTER,SETTER
+objs,ENS_VPORT,facexmaxgridfilter,SETTER
 objs,ENS_VPORT,FACEYMAXGRID,EMPTY
 objs,ENS_VPORT,faceymaxgrid,EMPTY
 objs,ENS_VPORT,FACEYMAXGRID,SETTER
 objs,ENS_VPORT,faceymaxgrid,SETTER
 objs,ENS_VPORT,FACEYMAXSUBGRID,EMPTY
 objs,ENS_VPORT,faceymaxsubgrid,EMPTY
 objs,ENS_VPORT,FACEYMAXSUBGRID,SETTER
 objs,ENS_VPORT,faceymaxsubgrid,SETTER
-objs,ENS_VPORT,FACEXMAXGRID,EMPTY
-objs,ENS_VPORT,facexmaxgrid,EMPTY
-objs,ENS_VPORT,FACEXMAXGRID,SETTER
-objs,ENS_VPORT,facexmaxgrid,SETTER
 objs,ENS_VPORT,FACEYMAXGRIDFILTER,EMPTY
 objs,ENS_VPORT,faceymaxgridfilter,EMPTY
 objs,ENS_VPORT,FACEYMAXGRIDFILTER,SETTER
 objs,ENS_VPORT,faceymaxgridfilter,SETTER
+objs,ENS_VPORT,FACEZMAXGRID,EMPTY
+objs,ENS_VPORT,facezmaxgrid,EMPTY
+objs,ENS_VPORT,FACEZMAXGRID,SETTER
+objs,ENS_VPORT,facezmaxgrid,SETTER
 objs,ENS_VPORT,FACEZMAXSUBGRID,EMPTY
 objs,ENS_VPORT,facezmaxsubgrid,EMPTY
 objs,ENS_VPORT,FACEZMAXSUBGRID,SETTER
 objs,ENS_VPORT,facezmaxsubgrid,SETTER
-objs,ENS_VPORT,FACEXMAXSUBGRID,EMPTY
-objs,ENS_VPORT,facexmaxsubgrid,EMPTY
-objs,ENS_VPORT,FACEXMAXSUBGRID,SETTER
-objs,ENS_VPORT,facexmaxsubgrid,SETTER
-objs,ENS_VPORT,FACEXMAXGRIDFILTER,EMPTY
-objs,ENS_VPORT,facexmaxgridfilter,EMPTY
-objs,ENS_VPORT,FACEXMAXGRIDFILTER,SETTER
-objs,ENS_VPORT,facexmaxgridfilter,SETTER
+objs,ENS_VPORT,FACEZMAXGRIDFILTER,EMPTY
+objs,ENS_VPORT,facezmaxgridfilter,EMPTY
+objs,ENS_VPORT,FACEZMAXGRIDFILTER,SETTER
+objs,ENS_VPORT,facezmaxgridfilter,SETTER
 objs,ENS_VPORT,CORETRANSFORM,EMPTY
 objs,ENS_VPORT,coretransform,EMPTY
 objs,ENS_VPORT,CORETRANSFORM,SETTER
 objs,ENS_VPORT,coretransform,SETTER
 objs,ENS_VPORT,CORE2DTRANSFORM,EMPTY
 objs,ENS_VPORT,core2dtransform,EMPTY
 objs,ENS_VPORT,CORE2DTRANSFORM,SETTER
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_animobj.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_animobj.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_arrow.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_arrow.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_dial.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_dial.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1032,94 +1032,94 @@
         return _value
 
     @background.setter
     def background(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.BACKGROUND, value)
 
     @property
-    def VALUERGB(self) -> List[float]:
-        """VALUERGB property
+    def BACKGROUNDRGB(self) -> List[float]:
+        """BACKGROUNDRGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
+        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
         _value = cast(List[float], value)
         return _value
 
-    @VALUERGB.setter
-    def VALUERGB(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
+    @BACKGROUNDRGB.setter
+    def BACKGROUNDRGB(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
 
     @property
-    def valuergb(self) -> List[float]:
-        """VALUERGB property
+    def backgroundrgb(self) -> List[float]:
+        """BACKGROUNDRGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         
-        Note: both 'valuergb' and 'VALUERGB' property names are supported.
+        Note: both 'backgroundrgb' and 'BACKGROUNDRGB' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
+        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
         _value = cast(List[float], value)
         return _value
 
-    @valuergb.setter
-    def valuergb(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
+    @backgroundrgb.setter
+    def backgroundrgb(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
 
     @property
-    def BACKGROUNDRGB(self) -> List[float]:
-        """BACKGROUNDRGB property
+    def VALUERGB(self) -> List[float]:
+        """VALUERGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
+        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
         _value = cast(List[float], value)
         return _value
 
-    @BACKGROUNDRGB.setter
-    def BACKGROUNDRGB(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
+    @VALUERGB.setter
+    def VALUERGB(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
 
     @property
-    def backgroundrgb(self) -> List[float]:
-        """BACKGROUNDRGB property
+    def valuergb(self) -> List[float]:
+        """VALUERGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         
-        Note: both 'backgroundrgb' and 'BACKGROUNDRGB' property names are supported.
+        Note: both 'valuergb' and 'VALUERGB' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
+        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
         _value = cast(List[float], value)
         return _value
 
-    @backgroundrgb.setter
-    def backgroundrgb(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
+    @valuergb.setter
+    def valuergb(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
 
     @property
     def VALUESIZE(self) -> int:
         """VALUESIZE property
         
         Size
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_gauge.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_gauge.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -874,102 +874,102 @@
         return _value
 
     @background.setter
     def background(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.BACKGROUND, value)
 
     @property
-    def VALUERGB(self) -> List[float]:
-        """VALUERGB property
+    def BACKGROUNDRGB(self) -> List[float]:
+        """BACKGROUNDRGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         Range:
             [0.0, 1.0]
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
+        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
         _value = cast(List[float], value)
         return _value
 
-    @VALUERGB.setter
-    def VALUERGB(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
+    @BACKGROUNDRGB.setter
+    def BACKGROUNDRGB(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
 
     @property
-    def valuergb(self) -> List[float]:
-        """VALUERGB property
+    def backgroundrgb(self) -> List[float]:
+        """BACKGROUNDRGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         Range:
             [0.0, 1.0]
         
-        Note: both 'valuergb' and 'VALUERGB' property names are supported.
+        Note: both 'backgroundrgb' and 'BACKGROUNDRGB' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
+        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
         _value = cast(List[float], value)
         return _value
 
-    @valuergb.setter
-    def valuergb(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
+    @backgroundrgb.setter
+    def backgroundrgb(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
 
     @property
-    def BACKGROUNDRGB(self) -> List[float]:
-        """BACKGROUNDRGB property
+    def VALUERGB(self) -> List[float]:
+        """VALUERGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         Range:
             [0.0, 1.0]
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
+        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
         _value = cast(List[float], value)
         return _value
 
-    @BACKGROUNDRGB.setter
-    def BACKGROUNDRGB(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
+    @VALUERGB.setter
+    def VALUERGB(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
 
     @property
-    def backgroundrgb(self) -> List[float]:
-        """BACKGROUNDRGB property
+    def valuergb(self) -> List[float]:
+        """VALUERGB property
         
         Color
         
         Supported operations:
             getattr, setattr
         Datatype:
             Color RGB, 3 element array
         Range:
             [0.0, 1.0]
         
-        Note: both 'backgroundrgb' and 'BACKGROUNDRGB' property names are supported.
+        Note: both 'valuergb' and 'VALUERGB' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.BACKGROUNDRGB)
+        value = self.getattr(self._session.ensight.objs.enums.VALUERGB)
         _value = cast(List[float], value)
         return _value
 
-    @backgroundrgb.setter
-    def backgroundrgb(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.BACKGROUNDRGB, value)
+    @valuergb.setter
+    def valuergb(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.VALUERGB, value)
 
     @property
     def VALUESIZE(self) -> int:
         """VALUESIZE property
         
         Size
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_lgnd.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_lgnd.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_line.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_line.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1097,99 +1097,99 @@
         return _value
 
     @origin2.setter
     def origin2(self, value: List[float]) -> None:
         self.setattr(self._session.ensight.objs.enums.ORIGIN2, value)
 
     @property
-    def ORIGINBY2(self) -> int:
-        """ORIGINBY2 property
+    def ORIGINBY1(self) -> int:
+        """ORIGINBY1 property
         
-        Origin by 2
+        Origin by 1
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
             * ensight.objs.enums.ANNOT_3D_SPACE - 3d_coords
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY2)
+        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY1)
         _value = cast(int, value)
         return _value
 
-    @ORIGINBY2.setter
-    def ORIGINBY2(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ORIGINBY2, value)
+    @ORIGINBY1.setter
+    def ORIGINBY1(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ORIGINBY1, value)
 
     @property
-    def originby2(self) -> int:
-        """ORIGINBY2 property
+    def originby1(self) -> int:
+        """ORIGINBY1 property
         
-        Origin by 2
+        Origin by 1
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
             * ensight.objs.enums.ANNOT_3D_SPACE - 3d_coords
         
-        Note: both 'originby2' and 'ORIGINBY2' property names are supported.
+        Note: both 'originby1' and 'ORIGINBY1' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY2)
+        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY1)
         _value = cast(int, value)
         return _value
 
-    @originby2.setter
-    def originby2(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ORIGINBY2, value)
+    @originby1.setter
+    def originby1(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ORIGINBY1, value)
 
     @property
-    def ORIGINBY1(self) -> int:
-        """ORIGINBY1 property
+    def ORIGINBY2(self) -> int:
+        """ORIGINBY2 property
         
-        Origin by 1
+        Origin by 2
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
             * ensight.objs.enums.ANNOT_3D_SPACE - 3d_coords
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY1)
+        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY2)
         _value = cast(int, value)
         return _value
 
-    @ORIGINBY1.setter
-    def ORIGINBY1(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ORIGINBY1, value)
+    @ORIGINBY2.setter
+    def ORIGINBY2(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ORIGINBY2, value)
 
     @property
-    def originby1(self) -> int:
-        """ORIGINBY1 property
+    def originby2(self) -> int:
+        """ORIGINBY2 property
         
-        Origin by 1
+        Origin by 2
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
             * ensight.objs.enums.ANNOT_3D_SPACE - 3d_coords
         
-        Note: both 'originby1' and 'ORIGINBY1' property names are supported.
+        Note: both 'originby2' and 'ORIGINBY2' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY1)
+        value = self.getattr(self._session.ensight.objs.enums.ORIGINBY2)
         _value = cast(int, value)
         return _value
 
-    @originby1.setter
-    def originby1(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ORIGINBY1, value)
+    @originby2.setter
+    def originby2(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ORIGINBY2, value)
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_logo.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_logo.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_marker.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_marker.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_shape.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_shape.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_annot_text.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_annot_text.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_camera.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_camera.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_case.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_case.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_emitterobj.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_emitterobj.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_flipbook.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_flipbook.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_frame.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_frame.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_globals.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_globals.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_group.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_group.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_lightsource.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lightsource.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_lpart.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_lpart.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_mat.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_mat.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_palette.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_palette.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5446,102 +5446,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_aux_geom.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_aux_geom.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5488,102 +5488,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_axisymmetric.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_axisymmetric.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_built_up.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_built_up.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_clip.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_clip.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5580,102 +5580,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
         
@@ -7603,94 +7603,94 @@
         return _value
 
     @cyldorigin.setter
     def cyldorigin(self, value: List[float]) -> None:
         self.setattr(self._session.ensight.objs.enums.CYLDORIGIN, value)
 
     @property
-    def CYLDENDPOINT(self) -> List[float]:
-        """CYLDENDPOINT property
+    def CYLDAXISVECT(self) -> List[float]:
+        """CYLDAXISVECT property
         
-        End point
+        Axis vector
         
         Supported operations:
             getattr, setattr
         Datatype:
             Float, 3 element array
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CYLDENDPOINT)
+        value = self.getattr(self._session.ensight.objs.enums.CYLDAXISVECT)
         _value = cast(List[float], value)
         return _value
 
-    @CYLDENDPOINT.setter
-    def CYLDENDPOINT(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.CYLDENDPOINT, value)
+    @CYLDAXISVECT.setter
+    def CYLDAXISVECT(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.CYLDAXISVECT, value)
 
     @property
-    def cyldendpoint(self) -> List[float]:
-        """CYLDENDPOINT property
+    def cyldaxisvect(self) -> List[float]:
+        """CYLDAXISVECT property
         
-        End point
+        Axis vector
         
         Supported operations:
             getattr, setattr
         Datatype:
             Float, 3 element array
         
-        Note: both 'cyldendpoint' and 'CYLDENDPOINT' property names are supported.
+        Note: both 'cyldaxisvect' and 'CYLDAXISVECT' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CYLDENDPOINT)
+        value = self.getattr(self._session.ensight.objs.enums.CYLDAXISVECT)
         _value = cast(List[float], value)
         return _value
 
-    @cyldendpoint.setter
-    def cyldendpoint(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.CYLDENDPOINT, value)
+    @cyldaxisvect.setter
+    def cyldaxisvect(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.CYLDAXISVECT, value)
 
     @property
-    def CYLDAXISVECT(self) -> List[float]:
-        """CYLDAXISVECT property
+    def CYLDENDPOINT(self) -> List[float]:
+        """CYLDENDPOINT property
         
-        Axis vector
+        End point
         
         Supported operations:
             getattr, setattr
         Datatype:
             Float, 3 element array
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CYLDAXISVECT)
+        value = self.getattr(self._session.ensight.objs.enums.CYLDENDPOINT)
         _value = cast(List[float], value)
         return _value
 
-    @CYLDAXISVECT.setter
-    def CYLDAXISVECT(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.CYLDAXISVECT, value)
+    @CYLDENDPOINT.setter
+    def CYLDENDPOINT(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.CYLDENDPOINT, value)
 
     @property
-    def cyldaxisvect(self) -> List[float]:
-        """CYLDAXISVECT property
+    def cyldendpoint(self) -> List[float]:
+        """CYLDENDPOINT property
         
-        Axis vector
+        End point
         
         Supported operations:
             getattr, setattr
         Datatype:
             Float, 3 element array
         
-        Note: both 'cyldaxisvect' and 'CYLDAXISVECT' property names are supported.
+        Note: both 'cyldendpoint' and 'CYLDENDPOINT' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CYLDAXISVECT)
+        value = self.getattr(self._session.ensight.objs.enums.CYLDENDPOINT)
         _value = cast(List[float], value)
         return _value
 
-    @cyldaxisvect.setter
-    def cyldaxisvect(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.CYLDAXISVECT, value)
+    @cyldendpoint.setter
+    def cyldendpoint(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.CYLDENDPOINT, value)
 
     @property
     def CONEANGLE(self) -> float:
         """CONEANGLE property
         
         Cone angle
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_contour.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_contour.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5502,102 +5502,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_developed_surface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_developed_surface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_discrete_particle.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_discrete_particle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_elevated_surface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_elevated_surface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5541,102 +5541,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
         
@@ -6243,87 +6243,87 @@
         return _value
 
     @offsetfrompart.setter
     def offsetfrompart(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.OFFSETFROMPART, value)
 
     @property
-    def OFFSETSCALE(self) -> float:
-        """OFFSETSCALE property
+    def OFFSETVECTOR(self) -> List[float]:
+        """OFFSETVECTOR property
         
-        Offset scale
+        Offset vector
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Float, scalar
+            Float, 3 element array
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.OFFSETSCALE)
-        _value = cast(float, value)
+        value = self.getattr(self._session.ensight.objs.enums.OFFSETVECTOR)
+        _value = cast(List[float], value)
         return _value
 
-    @OFFSETSCALE.setter
-    def OFFSETSCALE(self, value: float) -> None:
-        self.setattr(self._session.ensight.objs.enums.OFFSETSCALE, value)
+    @OFFSETVECTOR.setter
+    def OFFSETVECTOR(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.OFFSETVECTOR, value)
 
     @property
-    def offsetscale(self) -> float:
-        """OFFSETSCALE property
+    def offsetvector(self) -> List[float]:
+        """OFFSETVECTOR property
         
-        Offset scale
+        Offset vector
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Float, scalar
+            Float, 3 element array
         
-        Note: both 'offsetscale' and 'OFFSETSCALE' property names are supported.
+        Note: both 'offsetvector' and 'OFFSETVECTOR' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.OFFSETSCALE)
-        _value = cast(float, value)
+        value = self.getattr(self._session.ensight.objs.enums.OFFSETVECTOR)
+        _value = cast(List[float], value)
         return _value
 
-    @offsetscale.setter
-    def offsetscale(self, value: float) -> None:
-        self.setattr(self._session.ensight.objs.enums.OFFSETSCALE, value)
+    @offsetvector.setter
+    def offsetvector(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.OFFSETVECTOR, value)
 
     @property
-    def OFFSETVECTOR(self) -> List[float]:
-        """OFFSETVECTOR property
+    def OFFSETSCALE(self) -> float:
+        """OFFSETSCALE property
         
-        Offset vector
+        Offset scale
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Float, 3 element array
+            Float, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.OFFSETVECTOR)
-        _value = cast(List[float], value)
+        value = self.getattr(self._session.ensight.objs.enums.OFFSETSCALE)
+        _value = cast(float, value)
         return _value
 
-    @OFFSETVECTOR.setter
-    def OFFSETVECTOR(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.OFFSETVECTOR, value)
+    @OFFSETSCALE.setter
+    def OFFSETSCALE(self, value: float) -> None:
+        self.setattr(self._session.ensight.objs.enums.OFFSETSCALE, value)
 
     @property
-    def offsetvector(self) -> List[float]:
-        """OFFSETVECTOR property
+    def offsetscale(self) -> float:
+        """OFFSETSCALE property
         
-        Offset vector
+        Offset scale
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Float, 3 element array
+            Float, scalar
         
-        Note: both 'offsetvector' and 'OFFSETVECTOR' property names are supported.
+        Note: both 'offsetscale' and 'OFFSETSCALE' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.OFFSETVECTOR)
-        _value = cast(List[float], value)
+        value = self.getattr(self._session.ensight.objs.enums.OFFSETSCALE)
+        _value = cast(float, value)
         return _value
 
-    @offsetvector.setter
-    def offsetvector(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.OFFSETVECTOR, value)
+    @offsetscale.setter
+    def offsetscale(self, value: float) -> None:
+        self.setattr(self._session.ensight.objs.enums.OFFSETSCALE, value)
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_filter.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_filter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_frame.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_frame.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_sep_att.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_sep_att.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_shock.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_shock.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5498,102 +5498,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_fx_vortex_core.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_fx_vortex_core.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_isosurface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_isosurface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5502,102 +5502,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_mat_interface.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_mat_interface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5494,102 +5494,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_model.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_particle_trace.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_particle_trace.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5539,102 +5539,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
         
@@ -7495,14 +7495,55 @@
         return _value
 
     @massedinitialusefluid.setter
     def massedinitialusefluid(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.MASSEDINITIALUSEFLUID, value)
 
     @property
+    def MASSEDINITIALVELOCITY(self) -> List[float]:
+        """MASSEDINITIALVELOCITY property
+        
+        Fluid density
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            Float, 3 element array
+        
+        """
+        value = self.getattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY)
+        _value = cast(List[float], value)
+        return _value
+
+    @MASSEDINITIALVELOCITY.setter
+    def MASSEDINITIALVELOCITY(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY, value)
+
+    @property
+    def massedinitialvelocity(self) -> List[float]:
+        """MASSEDINITIALVELOCITY property
+        
+        Fluid density
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            Float, 3 element array
+        
+        Note: both 'massedinitialvelocity' and 'MASSEDINITIALVELOCITY' property names are supported.
+        """
+        value = self.getattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY)
+        _value = cast(List[float], value)
+        return _value
+
+    @massedinitialvelocity.setter
+    def massedinitialvelocity(self, value: List[float]) -> None:
+        self.setattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY, value)
+
+    @property
     def MASSEDFLUIDDENSITY(self) -> ensobjlist['ENS_VAR']:
         """MASSEDFLUIDDENSITY property
         
         Fluid density
         
         Supported operations:
             getattr, setattr
@@ -7544,55 +7585,14 @@
         return _value
 
     @massedfluiddensity.setter
     def massedfluiddensity(self, value: ensobjlist['ENS_VAR']) -> None:
         self.setattr(self._session.ensight.objs.enums.MASSEDFLUIDDENSITY, value)
 
     @property
-    def MASSEDINITIALVELOCITY(self) -> List[float]:
-        """MASSEDINITIALVELOCITY property
-        
-        Fluid density
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            Float, 3 element array
-        
-        """
-        value = self.getattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY)
-        _value = cast(List[float], value)
-        return _value
-
-    @MASSEDINITIALVELOCITY.setter
-    def MASSEDINITIALVELOCITY(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY, value)
-
-    @property
-    def massedinitialvelocity(self) -> List[float]:
-        """MASSEDINITIALVELOCITY property
-        
-        Fluid density
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            Float, 3 element array
-        
-        Note: both 'massedinitialvelocity' and 'MASSEDINITIALVELOCITY' property names are supported.
-        """
-        value = self.getattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY)
-        _value = cast(List[float], value)
-        return _value
-
-    @massedinitialvelocity.setter
-    def massedinitialvelocity(self, value: List[float]) -> None:
-        self.setattr(self._session.ensight.objs.enums.MASSEDINITIALVELOCITY, value)
-
-    @property
     def MASSEDFLUIDDENSITYVAL(self) -> float:
         """MASSEDFLUIDDENSITYVAL property
         
         Fluid density value
         
         Supported operations:
             getattr, setattr
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_point.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_point.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5447,102 +5447,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_profile.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_profile.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5541,102 +5541,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_tensor_glyph.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_tensor_glyph.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5498,102 +5498,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_vector_arrow.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vector_arrow.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5498,102 +5498,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_part_vof.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_part_vof.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5488,102 +5488,102 @@
         return _value
 
     @eltshrinkfactor.setter
     def eltshrinkfactor(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.ELTSHRINKFACTOR, value)
 
     @property
-    def CULLELEMENTS(self) -> int:
-        """CULLELEMENTS property
+    def ELTBLANKING(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @CULLELEMENTS.setter
-    def CULLELEMENTS(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @ELTBLANKING.setter
+    def ELTBLANKING(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def cullelements(self) -> int:
-        """CULLELEMENTS property
+    def eltblanking(self) -> int:
+        """ELTBLANKING property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.CULL_BACK_FACE - facing_back
-            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-            * ensight.objs.enums.CULL_NO_FACE - off
+            Boolean, scalar
         
-        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
+        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
+        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
         _value = cast(int, value)
         return _value
 
-    @cullelements.setter
-    def cullelements(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
+    @eltblanking.setter
+    def eltblanking(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
 
     @property
-    def ELTBLANKING(self) -> int:
-        """ELTBLANKING property
+    def CULLELEMENTS(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @ELTBLANKING.setter
-    def ELTBLANKING(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @CULLELEMENTS.setter
+    def CULLELEMENTS(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
-    def eltblanking(self) -> int:
-        """ELTBLANKING property
+    def cullelements(self) -> int:
+        """CULLELEMENTS property
         
         Do not show elements
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Boolean, scalar
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.CULL_BACK_FACE - facing_back
+            * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+            * ensight.objs.enums.CULL_NO_FACE - off
         
-        Note: both 'eltblanking' and 'ELTBLANKING' property names are supported.
+        Note: both 'cullelements' and 'CULLELEMENTS' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.ELTBLANKING)
+        value = self.getattr(self._session.ensight.objs.enums.CULLELEMENTS)
         _value = cast(int, value)
         return _value
 
-    @eltblanking.setter
-    def eltblanking(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.ELTBLANKING, value)
+    @cullelements.setter
+    def cullelements(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.CULLELEMENTS, value)
 
     @property
     def HIDDENSURFACE(self) -> int:
         """HIDDENSURFACE property
         
         Hidden surface
         
@@ -7143,110 +7143,110 @@
         return _value
 
     @cellcompnum.setter
     def cellcompnum(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.CELLCOMPNUM, value)
 
     @property
-    def COOLINGCHANNELCOMP(self) -> ensobjlist['ENS_VAR']:
-        """COOLINGCHANNELCOMP property
+    def BLANKINGVARIABLE1(self) -> ensobjlist['ENS_VAR']:
+        """BLANKINGVARIABLE1 property
         
-        Component ID of cooling channel
+        Blanking variable1
         
         Supported operations:
             getattr, setattr
         Datatype:
             ENS_VAR Object, scalar
         Variable type filters:
             * Scalar
             * Nodal
             * Element
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP)
+        value = self.getattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1)
         _value = cast(ensobjlist['ENS_VAR'], value)
         return _value
 
-    @COOLINGCHANNELCOMP.setter
-    def COOLINGCHANNELCOMP(self, value: ensobjlist['ENS_VAR']) -> None:
-        self.setattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP, value)
+    @BLANKINGVARIABLE1.setter
+    def BLANKINGVARIABLE1(self, value: ensobjlist['ENS_VAR']) -> None:
+        self.setattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1, value)
 
     @property
-    def coolingchannelcomp(self) -> ensobjlist['ENS_VAR']:
-        """COOLINGCHANNELCOMP property
+    def blankingvariable1(self) -> ensobjlist['ENS_VAR']:
+        """BLANKINGVARIABLE1 property
         
-        Component ID of cooling channel
+        Blanking variable1
         
         Supported operations:
             getattr, setattr
         Datatype:
             ENS_VAR Object, scalar
         Variable type filters:
             * Scalar
             * Nodal
             * Element
         
-        Note: both 'coolingchannelcomp' and 'COOLINGCHANNELCOMP' property names are supported.
+        Note: both 'blankingvariable1' and 'BLANKINGVARIABLE1' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP)
+        value = self.getattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1)
         _value = cast(ensobjlist['ENS_VAR'], value)
         return _value
 
-    @coolingchannelcomp.setter
-    def coolingchannelcomp(self, value: ensobjlist['ENS_VAR']) -> None:
-        self.setattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP, value)
+    @blankingvariable1.setter
+    def blankingvariable1(self, value: ensobjlist['ENS_VAR']) -> None:
+        self.setattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1, value)
 
     @property
-    def BLANKINGVARIABLE1(self) -> ensobjlist['ENS_VAR']:
-        """BLANKINGVARIABLE1 property
+    def COOLINGCHANNELCOMP(self) -> ensobjlist['ENS_VAR']:
+        """COOLINGCHANNELCOMP property
         
-        Blanking variable1
+        Component ID of cooling channel
         
         Supported operations:
             getattr, setattr
         Datatype:
             ENS_VAR Object, scalar
         Variable type filters:
             * Scalar
             * Nodal
             * Element
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1)
+        value = self.getattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP)
         _value = cast(ensobjlist['ENS_VAR'], value)
         return _value
 
-    @BLANKINGVARIABLE1.setter
-    def BLANKINGVARIABLE1(self, value: ensobjlist['ENS_VAR']) -> None:
-        self.setattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1, value)
+    @COOLINGCHANNELCOMP.setter
+    def COOLINGCHANNELCOMP(self, value: ensobjlist['ENS_VAR']) -> None:
+        self.setattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP, value)
 
     @property
-    def blankingvariable1(self) -> ensobjlist['ENS_VAR']:
-        """BLANKINGVARIABLE1 property
+    def coolingchannelcomp(self) -> ensobjlist['ENS_VAR']:
+        """COOLINGCHANNELCOMP property
         
-        Blanking variable1
+        Component ID of cooling channel
         
         Supported operations:
             getattr, setattr
         Datatype:
             ENS_VAR Object, scalar
         Variable type filters:
             * Scalar
             * Nodal
             * Element
         
-        Note: both 'blankingvariable1' and 'BLANKINGVARIABLE1' property names are supported.
+        Note: both 'coolingchannelcomp' and 'COOLINGCHANNELCOMP' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1)
+        value = self.getattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP)
         _value = cast(ensobjlist['ENS_VAR'], value)
         return _value
 
-    @blankingvariable1.setter
-    def blankingvariable1(self, value: ensobjlist['ENS_VAR']) -> None:
-        self.setattr(self._session.ensight.objs.enums.BLANKINGVARIABLE1, value)
+    @coolingchannelcomp.setter
+    def coolingchannelcomp(self, value: ensobjlist['ENS_VAR']) -> None:
+        self.setattr(self._session.ensight.objs.enums.COOLINGCHANNELCOMP, value)
 
     @property
     def BLANKINGVARIABLE2(self) -> ensobjlist['ENS_VAR']:
         """BLANKINGVARIABLE2 property
         
         Blanking variable2
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_plotter.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_plotter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1443,55 +1443,14 @@
         return _value
 
     @axisxtitle.setter
     def axisxtitle(self, value: str) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISXTITLE, value)
 
     @property
-    def AXISYTITLE(self) -> str:
-        """AXISYTITLE property
-        
-        Title text
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            String, 1024 characters maximum
-        
-        """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
-        _value = cast(str, value)
-        return _value
-
-    @AXISYTITLE.setter
-    def AXISYTITLE(self, value: str) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
-
-    @property
-    def axisytitle(self) -> str:
-        """AXISYTITLE property
-        
-        Title text
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            String, 1024 characters maximum
-        
-        Note: both 'axisytitle' and 'AXISYTITLE' property names are supported.
-        """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
-        _value = cast(str, value)
-        return _value
-
-    @axisytitle.setter
-    def axisytitle(self, value: str) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
-
-    @property
     def AXISXTITLESIZE(self) -> int:
         """AXISXTITLESIZE property
         
         Title size
         
         Supported operations:
             getattr, setattr
@@ -1844,14 +1803,55 @@
         return _value
 
     @axisxnumsubgrid.setter
     def axisxnumsubgrid(self, value: float) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISXNUMSUBGRID, value)
 
     @property
+    def AXISYTITLE(self) -> str:
+        """AXISYTITLE property
+        
+        Title text
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            String, 1024 characters maximum
+        
+        """
+        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
+        _value = cast(str, value)
+        return _value
+
+    @AXISYTITLE.setter
+    def AXISYTITLE(self, value: str) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
+
+    @property
+    def axisytitle(self) -> str:
+        """AXISYTITLE property
+        
+        Title text
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            String, 1024 characters maximum
+        
+        Note: both 'axisytitle' and 'AXISYTITLE' property names are supported.
+        """
+        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
+        _value = cast(str, value)
+        return _value
+
+    @axisytitle.setter
+    def axisytitle(self, value: str) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
+
+    @property
     def AXISYTITLESIZE(self) -> int:
         """AXISYTITLESIZE property
         
         Title size
         
         Supported operations:
             getattr, setattr
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_polyline.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_polyline.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_probe.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_probe.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_query.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_query.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_scene.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_scene.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_source.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_source.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_spec.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_spec.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_state.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_state.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_texture.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_texture.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_box.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_box.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cone.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cone.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cursor.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cursor.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_cylinder.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_line.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_line.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_plane.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_plane.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_revolution.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_revolution.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_tool_sphere.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_tool_sphere.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_var.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_var.py`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ens_vport.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ens_vport.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3400,55 +3400,14 @@
         return _value
 
     @axisxtitle.setter
     def axisxtitle(self, value: str) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISXTITLE, value)
 
     @property
-    def AXISYTITLE(self) -> str:
-        """AXISYTITLE property
-        
-        Title
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            String, 1024 characters maximum
-        
-        """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
-        _value = cast(str, value)
-        return _value
-
-    @AXISYTITLE.setter
-    def AXISYTITLE(self, value: str) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
-
-    @property
-    def axisytitle(self) -> str:
-        """AXISYTITLE property
-        
-        Title
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            String, 1024 characters maximum
-        
-        Note: both 'axisytitle' and 'AXISYTITLE' property names are supported.
-        """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
-        _value = cast(str, value)
-        return _value
-
-    @axisytitle.setter
-    def axisytitle(self, value: str) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
-
-    @property
     def AXISXTITLESIZE(self) -> int:
         """AXISXTITLESIZE property
         
         Title size
         
         Supported operations:
             getattr, setattr
@@ -4407,14 +4366,55 @@
         return _value
 
     @axisxgridextentloc.setter
     def axisxgridextentloc(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISXGRIDEXTENTLOC, value)
 
     @property
+    def AXISYTITLE(self) -> str:
+        """AXISYTITLE property
+        
+        Title
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            String, 1024 characters maximum
+        
+        """
+        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
+        _value = cast(str, value)
+        return _value
+
+    @AXISYTITLE.setter
+    def AXISYTITLE(self, value: str) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
+
+    @property
+    def axisytitle(self) -> str:
+        """AXISYTITLE property
+        
+        Title
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            String, 1024 characters maximum
+        
+        Note: both 'axisytitle' and 'AXISYTITLE' property names are supported.
+        """
+        value = self.getattr(self._session.ensight.objs.enums.AXISYTITLE)
+        _value = cast(str, value)
+        return _value
+
+    @axisytitle.setter
+    def axisytitle(self, value: str) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYTITLE, value)
+
+    @property
     def AXISYTITLESIZE(self) -> int:
         """AXISYTITLESIZE property
         
         Title size
         
         Supported operations:
             getattr, setattr
@@ -4665,110 +4665,110 @@
         return _value
 
     @axisylabelaxisloc.setter
     def axisylabelaxisloc(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISYLABELAXISLOC, value)
 
     @property
-    def AXISYLABELFILTER(self) -> int:
-        """AXISYLABELFILTER property
+    def AXISYLABELEXTENTLOC(self) -> int:
+        """AXISYLABELEXTENTLOC property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC)
         _value = cast(int, value)
         return _value
 
-    @AXISYLABELFILTER.setter
-    def AXISYLABELFILTER(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYLABELFILTER, value)
+    @AXISYLABELEXTENTLOC.setter
+    def AXISYLABELEXTENTLOC(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC, value)
 
     @property
-    def axisylabelfilter(self) -> int:
-        """AXISYLABELFILTER property
+    def axisylabelextentloc(self) -> int:
+        """AXISYLABELEXTENTLOC property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
         
-        Note: both 'axisylabelfilter' and 'AXISYLABELFILTER' property names are supported.
+        Note: both 'axisylabelextentloc' and 'AXISYLABELEXTENTLOC' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC)
         _value = cast(int, value)
         return _value
 
-    @axisylabelfilter.setter
-    def axisylabelfilter(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYLABELFILTER, value)
+    @axisylabelextentloc.setter
+    def axisylabelextentloc(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC, value)
 
     @property
-    def AXISYLABELEXTENTLOC(self) -> int:
-        """AXISYLABELEXTENTLOC property
+    def AXISYLABELFILTER(self) -> int:
+        """AXISYLABELFILTER property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC)
+        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELFILTER)
         _value = cast(int, value)
         return _value
 
-    @AXISYLABELEXTENTLOC.setter
-    def AXISYLABELEXTENTLOC(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC, value)
+    @AXISYLABELFILTER.setter
+    def AXISYLABELFILTER(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYLABELFILTER, value)
 
     @property
-    def axisylabelextentloc(self) -> int:
-        """AXISYLABELEXTENTLOC property
+    def axisylabelfilter(self) -> int:
+        """AXISYLABELFILTER property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
-        Note: both 'axisylabelextentloc' and 'AXISYLABELEXTENTLOC' property names are supported.
+        Note: both 'axisylabelfilter' and 'AXISYLABELFILTER' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC)
+        value = self.getattr(self._session.ensight.objs.enums.AXISYLABELFILTER)
         _value = cast(int, value)
         return _value
 
-    @axisylabelextentloc.setter
-    def axisylabelextentloc(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISYLABELEXTENTLOC, value)
+    @axisylabelfilter.setter
+    def axisylabelfilter(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISYLABELFILTER, value)
 
     @property
     def AXISYFORMAT(self) -> str:
         """AXISYFORMAT property
         
         Value format
         
@@ -5631,110 +5631,110 @@
         return _value
 
     @axiszlabelaxisloc.setter
     def axiszlabelaxisloc(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.AXISZLABELAXISLOC, value)
 
     @property
-    def AXISZLABELFILTER(self) -> int:
-        """AXISZLABELFILTER property
+    def AXISZLABELEXTENTLOC(self) -> int:
+        """AXISZLABELEXTENTLOC property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC)
         _value = cast(int, value)
         return _value
 
-    @AXISZLABELFILTER.setter
-    def AXISZLABELFILTER(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISZLABELFILTER, value)
+    @AXISZLABELEXTENTLOC.setter
+    def AXISZLABELEXTENTLOC(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC, value)
 
     @property
-    def axiszlabelfilter(self) -> int:
-        """AXISZLABELFILTER property
+    def axiszlabelextentloc(self) -> int:
+        """AXISZLABELEXTENTLOC property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
         
-        Note: both 'axiszlabelfilter' and 'AXISZLABELFILTER' property names are supported.
+        Note: both 'axiszlabelextentloc' and 'AXISZLABELEXTENTLOC' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC)
         _value = cast(int, value)
         return _value
 
-    @axiszlabelfilter.setter
-    def axiszlabelfilter(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISZLABELFILTER, value)
+    @axiszlabelextentloc.setter
+    def axiszlabelextentloc(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC, value)
 
     @property
-    def AXISZLABELEXTENTLOC(self) -> int:
-        """AXISZLABELEXTENTLOC property
+    def AXISZLABELFILTER(self) -> int:
+        """AXISZLABELFILTER property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC)
+        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELFILTER)
         _value = cast(int, value)
         return _value
 
-    @AXISZLABELEXTENTLOC.setter
-    def AXISZLABELEXTENTLOC(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC, value)
+    @AXISZLABELFILTER.setter
+    def AXISZLABELFILTER(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISZLABELFILTER, value)
 
     @property
-    def axiszlabelextentloc(self) -> int:
-        """AXISZLABELEXTENTLOC property
+    def axiszlabelfilter(self) -> int:
+        """AXISZLABELFILTER property
         
         Value filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-            * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
-        Note: both 'axiszlabelextentloc' and 'AXISZLABELEXTENTLOC' property names are supported.
+        Note: both 'axiszlabelfilter' and 'AXISZLABELFILTER' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC)
+        value = self.getattr(self._session.ensight.objs.enums.AXISZLABELFILTER)
         _value = cast(int, value)
         return _value
 
-    @axiszlabelextentloc.setter
-    def axiszlabelextentloc(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.AXISZLABELEXTENTLOC, value)
+    @axiszlabelfilter.setter
+    def axiszlabelfilter(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.AXISZLABELFILTER, value)
 
     @property
     def AXISZFORMAT(self) -> str:
         """AXISZFORMAT property
         
         Value format
         
@@ -6380,14 +6380,63 @@
         return _value
 
     @facexminsubgrid.setter
     def facexminsubgrid(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.FACEXMINSUBGRID, value)
 
     @property
+    def FACEXMINGRIDFILTER(self) -> int:
+        """FACEXMINGRIDFILTER property
+        
+        Face filter
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+        
+        """
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER)
+        _value = cast(int, value)
+        return _value
+
+    @FACEXMINGRIDFILTER.setter
+    def FACEXMINGRIDFILTER(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER, value)
+
+    @property
+    def facexmingridfilter(self) -> int:
+        """FACEXMINGRIDFILTER property
+        
+        Face filter
+        
+        Supported operations:
+            getattr, setattr
+        Datatype:
+            Enum, scalar
+        Enums:
+            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+        
+        Note: both 'facexmingridfilter' and 'FACEXMINGRIDFILTER' property names are supported.
+        """
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER)
+        _value = cast(int, value)
+        return _value
+
+    @facexmingridfilter.setter
+    def facexmingridfilter(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER, value)
+
+    @property
     def FACEYMINGRID(self) -> int:
         """FACEYMINGRID property
         
         Grid/Tick show
         
         Supported operations:
             getattr, setattr
@@ -6642,151 +6691,143 @@
         return _value
 
     @facezmingridfilter.setter
     def facezmingridfilter(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.FACEZMINGRIDFILTER, value)
 
     @property
-    def FACEXMINGRIDFILTER(self) -> int:
-        """FACEXMINGRIDFILTER property
+    def FACEXMAXGRID(self) -> int:
+        """FACEXMAXGRID property
         
-        Face filter
+        Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRID)
         _value = cast(int, value)
         return _value
 
-    @FACEXMINGRIDFILTER.setter
-    def FACEXMINGRIDFILTER(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER, value)
+    @FACEXMAXGRID.setter
+    def FACEXMAXGRID(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRID, value)
 
     @property
-    def facexmingridfilter(self) -> int:
-        """FACEXMINGRIDFILTER property
+    def facexmaxgrid(self) -> int:
+        """FACEXMAXGRID property
         
-        Face filter
+        Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
-            Enum, scalar
-        Enums:
-            * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-            * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-            * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+            Boolean, scalar
         
-        Note: both 'facexmingridfilter' and 'FACEXMINGRIDFILTER' property names are supported.
+        Note: both 'facexmaxgrid' and 'FACEXMAXGRID' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRID)
         _value = cast(int, value)
         return _value
 
-    @facexmingridfilter.setter
-    def facexmingridfilter(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMINGRIDFILTER, value)
+    @facexmaxgrid.setter
+    def facexmaxgrid(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRID, value)
 
     @property
-    def FACEZMAXGRID(self) -> int:
-        """FACEZMAXGRID property
+    def FACEXMAXSUBGRID(self) -> int:
+        """FACEXMAXSUBGRID property
         
-        Grid/Tick show
+        Sub Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID)
         _value = cast(int, value)
         return _value
 
-    @FACEZMAXGRID.setter
-    def FACEZMAXGRID(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRID, value)
+    @FACEXMAXSUBGRID.setter
+    def FACEXMAXSUBGRID(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID, value)
 
     @property
-    def facezmaxgrid(self) -> int:
-        """FACEZMAXGRID property
+    def facexmaxsubgrid(self) -> int:
+        """FACEXMAXSUBGRID property
         
-        Grid/Tick show
+        Sub Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
-        Note: both 'facezmaxgrid' and 'FACEZMAXGRID' property names are supported.
+        Note: both 'facexmaxsubgrid' and 'FACEXMAXSUBGRID' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID)
         _value = cast(int, value)
         return _value
 
-    @facezmaxgrid.setter
-    def facezmaxgrid(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRID, value)
+    @facexmaxsubgrid.setter
+    def facexmaxsubgrid(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID, value)
 
     @property
-    def FACEZMAXGRIDFILTER(self) -> int:
-        """FACEZMAXGRIDFILTER property
+    def FACEXMAXGRIDFILTER(self) -> int:
+        """FACEXMAXGRIDFILTER property
         
         Face filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
             * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
             * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER)
         _value = cast(int, value)
         return _value
 
-    @FACEZMAXGRIDFILTER.setter
-    def FACEZMAXGRIDFILTER(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER, value)
+    @FACEXMAXGRIDFILTER.setter
+    def FACEXMAXGRIDFILTER(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER, value)
 
     @property
-    def facezmaxgridfilter(self) -> int:
-        """FACEZMAXGRIDFILTER property
+    def facexmaxgridfilter(self) -> int:
+        """FACEXMAXGRIDFILTER property
         
         Face filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
             * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
             * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
-        Note: both 'facezmaxgridfilter' and 'FACEZMAXGRIDFILTER' property names are supported.
+        Note: both 'facexmaxgridfilter' and 'FACEXMAXGRIDFILTER' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER)
         _value = cast(int, value)
         return _value
 
-    @facezmaxgridfilter.setter
-    def facezmaxgridfilter(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER, value)
+    @facexmaxgridfilter.setter
+    def facexmaxgridfilter(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER, value)
 
     @property
     def FACEYMAXGRID(self) -> int:
         """FACEYMAXGRID property
         
         Grid/Tick show
         
@@ -6863,55 +6904,14 @@
         return _value
 
     @faceymaxsubgrid.setter
     def faceymaxsubgrid(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.FACEYMAXSUBGRID, value)
 
     @property
-    def FACEXMAXGRID(self) -> int:
-        """FACEXMAXGRID property
-        
-        Grid/Tick show
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            Boolean, scalar
-        
-        """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRID)
-        _value = cast(int, value)
-        return _value
-
-    @FACEXMAXGRID.setter
-    def FACEXMAXGRID(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRID, value)
-
-    @property
-    def facexmaxgrid(self) -> int:
-        """FACEXMAXGRID property
-        
-        Grid/Tick show
-        
-        Supported operations:
-            getattr, setattr
-        Datatype:
-            Boolean, scalar
-        
-        Note: both 'facexmaxgrid' and 'FACEXMAXGRID' property names are supported.
-        """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRID)
-        _value = cast(int, value)
-        return _value
-
-    @facexmaxgrid.setter
-    def facexmaxgrid(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRID, value)
-
-    @property
     def FACEYMAXGRIDFILTER(self) -> int:
         """FACEYMAXGRIDFILTER property
         
         Face filter
         
         Supported operations:
             getattr, setattr
@@ -6953,143 +6953,143 @@
         return _value
 
     @faceymaxgridfilter.setter
     def faceymaxgridfilter(self, value: int) -> None:
         self.setattr(self._session.ensight.objs.enums.FACEYMAXGRIDFILTER, value)
 
     @property
-    def FACEZMAXSUBGRID(self) -> int:
-        """FACEZMAXSUBGRID property
+    def FACEZMAXGRID(self) -> int:
+        """FACEZMAXGRID property
         
-        Sub Grid/Tick show
+        Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRID)
         _value = cast(int, value)
         return _value
 
-    @FACEZMAXSUBGRID.setter
-    def FACEZMAXSUBGRID(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID, value)
+    @FACEZMAXGRID.setter
+    def FACEZMAXGRID(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRID, value)
 
     @property
-    def facezmaxsubgrid(self) -> int:
-        """FACEZMAXSUBGRID property
+    def facezmaxgrid(self) -> int:
+        """FACEZMAXGRID property
         
-        Sub Grid/Tick show
+        Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
-        Note: both 'facezmaxsubgrid' and 'FACEZMAXSUBGRID' property names are supported.
+        Note: both 'facezmaxgrid' and 'FACEZMAXGRID' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRID)
         _value = cast(int, value)
         return _value
 
-    @facezmaxsubgrid.setter
-    def facezmaxsubgrid(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID, value)
+    @facezmaxgrid.setter
+    def facezmaxgrid(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRID, value)
 
     @property
-    def FACEXMAXSUBGRID(self) -> int:
-        """FACEXMAXSUBGRID property
+    def FACEZMAXSUBGRID(self) -> int:
+        """FACEZMAXSUBGRID property
         
         Sub Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID)
         _value = cast(int, value)
         return _value
 
-    @FACEXMAXSUBGRID.setter
-    def FACEXMAXSUBGRID(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID, value)
+    @FACEZMAXSUBGRID.setter
+    def FACEZMAXSUBGRID(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID, value)
 
     @property
-    def facexmaxsubgrid(self) -> int:
-        """FACEXMAXSUBGRID property
+    def facezmaxsubgrid(self) -> int:
+        """FACEZMAXSUBGRID property
         
         Sub Grid/Tick show
         
         Supported operations:
             getattr, setattr
         Datatype:
             Boolean, scalar
         
-        Note: both 'facexmaxsubgrid' and 'FACEXMAXSUBGRID' property names are supported.
+        Note: both 'facezmaxsubgrid' and 'FACEZMAXSUBGRID' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID)
         _value = cast(int, value)
         return _value
 
-    @facexmaxsubgrid.setter
-    def facexmaxsubgrid(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXSUBGRID, value)
+    @facezmaxsubgrid.setter
+    def facezmaxsubgrid(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXSUBGRID, value)
 
     @property
-    def FACEXMAXGRIDFILTER(self) -> int:
-        """FACEXMAXGRIDFILTER property
+    def FACEZMAXGRIDFILTER(self) -> int:
+        """FACEZMAXGRIDFILTER property
         
         Face filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
             * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
             * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER)
         _value = cast(int, value)
         return _value
 
-    @FACEXMAXGRIDFILTER.setter
-    def FACEXMAXGRIDFILTER(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER, value)
+    @FACEZMAXGRIDFILTER.setter
+    def FACEZMAXGRIDFILTER(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER, value)
 
     @property
-    def facexmaxgridfilter(self) -> int:
-        """FACEXMAXGRIDFILTER property
+    def facezmaxgridfilter(self) -> int:
+        """FACEZMAXGRIDFILTER property
         
         Face filter
         
         Supported operations:
             getattr, setattr
         Datatype:
             Enum, scalar
         Enums:
             * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
             * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
             * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
         
-        Note: both 'facexmaxgridfilter' and 'FACEXMAXGRIDFILTER' property names are supported.
+        Note: both 'facezmaxgridfilter' and 'FACEZMAXGRIDFILTER' property names are supported.
         """
-        value = self.getattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER)
+        value = self.getattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER)
         _value = cast(int, value)
         return _value
 
-    @facexmaxgridfilter.setter
-    def facexmaxgridfilter(self, value: int) -> None:
-        self.setattr(self._session.ensight.objs.enums.FACEXMAXGRIDFILTER, value)
+    @facezmaxgridfilter.setter
+    def facezmaxgridfilter(self, value: int) -> None:
+        self.setattr(self._session.ensight.objs.enums.FACEZMAXGRIDFILTER, value)
 
     @property
     def CORETRANSFORM(self) -> List[float]:
         """CORETRANSFORM property
         
         core transform details
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/ensight_api.py` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/ensight_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Module ensight_api
-Autogenerated from: ensight_api.xml at 2023-07-05T09:16:16.721072
+Autogenerated from: ensight_api.xml at 2023-07-03T09:54:22.953220
 """
 from ansys.pyensight.core import Session
 from ansys.pyensight.core.ensobj import ENSOBJ
 from ansys.pyensight.core import ensobjlist
 from ansys.api.pyensight.ens_annot import ENS_ANNOT
 from ansys.api.pyensight.ens_annot_text import ENS_ANNOT_TEXT
 from ansys.api.pyensight.ens_annot_line import ENS_ANNOT_LINE
@@ -32471,56 +32471,56 @@
         self.AXISLINEWIDTH: int = 1610613630
         self.AXISLOCAL: int = 1610612923
         self.AXISMODEL: int = 1610612925
         self.AXISMODEL_ANIMATE: int = 1610612926
         self.AXISMODEL_LOCATION: int = 1610612927
         self.AXISRGB: int = 1610613631
         self.AXISSWAP: int = 1610613751
-        self.AXISWIDTH: int = 1610613650
+        self.AXISWIDTH: int = 1610613649
         self.AXISXAUTOSCALE: int = 1610613760
-        self.AXISXDISPLAYONEDGE: int = 1610613656
-        self.AXISXFORMAT: int = 1610613654
-        self.AXISXGRIDEXTENTLOC: int = 1610613667
-        self.AXISXGRIDTYPE: int = 1610613661
-        self.AXISXLABELAXISLOC: int = 1610613651
-        self.AXISXLABELEXTENTLOC: int = 1610613652
-        self.AXISXLABELFILTER: int = 1610613653
+        self.AXISXDISPLAYONEDGE: int = 1610613655
+        self.AXISXFORMAT: int = 1610613653
+        self.AXISXGRIDEXTENTLOC: int = 1610613666
+        self.AXISXGRIDTYPE: int = 1610613660
+        self.AXISXLABELAXISLOC: int = 1610613650
+        self.AXISXLABELEXTENTLOC: int = 1610613651
+        self.AXISXLABELFILTER: int = 1610613652
         self.AXISXLABELFORMAT: int = 1610613756
-        self.AXISXLABELRGB: int = 1610613655
+        self.AXISXLABELRGB: int = 1610613654
         self.AXISXLABELSIZE: int = 1610613754
         self.AXISXLABELTYPE: int = 1610613753
-        self.AXISXMAX: int = 1610613648
-        self.AXISXMIN: int = 1610613647
-        self.AXISXNUMGRID: int = 1610613663
+        self.AXISXMAX: int = 1610613647
+        self.AXISXMIN: int = 1610613646
+        self.AXISXNUMGRID: int = 1610613662
         self.AXISXNUMGRIDLOG: int = 1610613757
-        self.AXISXNUMSUBGRID: int = 1610613666
+        self.AXISXNUMSUBGRID: int = 1610613665
         self.AXISXNUMSUBGRIDLOG: int = 1610613758
-        self.AXISXORIG: int = 1610613649
+        self.AXISXORIG: int = 1610613648
         self.AXISXORIGIN: int = 1610613761
         self.AXISXSCALE: int = 1610613755
-        self.AXISXSGRIDTYPE: int = 1610613664
+        self.AXISXSGRIDTYPE: int = 1610613663
         self.AXISXSIZE: int = 1610613762
-        self.AXISXSUBTICK: int = 1610613665
-        self.AXISXTICK: int = 1610613662
+        self.AXISXSUBTICK: int = 1610613664
+        self.AXISXTICK: int = 1610613661
         self.AXISXTITLE: int = 1610613644
         self.AXISXTITLERGB: int = 1610613752
-        self.AXISXTITLESIZE: int = 1610613646
+        self.AXISXTITLESIZE: int = 1610613645
         self.AXISXVISIBLE: int = 1610613759
-        self.AXISXYMAXZMAX: int = 1610613660
-        self.AXISXYMAXZMIN: int = 1610613659
-        self.AXISXYMINZMAX: int = 1610613658
-        self.AXISXYMINZMIN: int = 1610613657
+        self.AXISXYMAXZMAX: int = 1610613659
+        self.AXISXYMAXZMIN: int = 1610613658
+        self.AXISXYMINZMAX: int = 1610613657
+        self.AXISXYMINZMIN: int = 1610613656
         self.AXISYAUTOSCALE: int = 1610613771
         self.AXISYDISPLAYONEDGE: int = 1610613678
         self.AXISYFORMAT: int = 1610613676
         self.AXISYGRIDEXTENTLOC: int = 1610613690
         self.AXISYGRIDTYPE: int = 1610613684
         self.AXISYLABELAXISLOC: int = 1610613673
-        self.AXISYLABELEXTENTLOC: int = 1610613675
-        self.AXISYLABELFILTER: int = 1610613674
+        self.AXISYLABELEXTENTLOC: int = 1610613674
+        self.AXISYLABELFILTER: int = 1610613675
         self.AXISYLABELFORMAT: int = 1610613767
         self.AXISYLABELRGB: int = 1610613677
         self.AXISYLABELSIZE: int = 1610613765
         self.AXISYLABELTYPE: int = 1610613764
         self.AXISYMAX: int = 1610613670
         self.AXISYMIN: int = 1610613669
         self.AXISYNUMGRID: int = 1610613686
@@ -32530,29 +32530,29 @@
         self.AXISYORIG: int = 1610613671
         self.AXISYORIGIN: int = 1610613772
         self.AXISYSCALE: int = 1610613766
         self.AXISYSGRIDTYPE: int = 1610613687
         self.AXISYSIZE: int = 1610613773
         self.AXISYSUBTICK: int = 1610613688
         self.AXISYTICK: int = 1610613685
-        self.AXISYTITLE: int = 1610613645
+        self.AXISYTITLE: int = 1610613667
         self.AXISYTITLERGB: int = 1610613763
         self.AXISYTITLESIZE: int = 1610613668
         self.AXISYVISIBLE: int = 1610613770
         self.AXISYYMAXZMAX: int = 1610613683
         self.AXISYYMAXZMIN: int = 1610613682
         self.AXISYYMINZMAX: int = 1610613681
         self.AXISYYMINZMIN: int = 1610613680
         self.AXISZDISPLAYONEDGE: int = 1610613679
         self.AXISZFORMAT: int = 1610613698
         self.AXISZGRIDEXTENTLOC: int = 1610613710
         self.AXISZGRIDTYPE: int = 1610613704
         self.AXISZLABELAXISLOC: int = 1610613695
-        self.AXISZLABELEXTENTLOC: int = 1610613697
-        self.AXISZLABELFILTER: int = 1610613696
+        self.AXISZLABELEXTENTLOC: int = 1610613696
+        self.AXISZLABELFILTER: int = 1610613697
         self.AXISZLABELRGB: int = 1610613699
         self.AXISZMAX: int = 1610613694
         self.AXISZMIN: int = 1610613693
         self.AXISZNUMGRID: int = 1610613706
         self.AXISZNUMSUBGRID: int = 1610613709
         self.AXISZSGRIDTYPE: int = 1610613707
         self.AXISZSUBTICK: int = 1610613708
@@ -32564,24 +32564,24 @@
         self.AXISZYMINZMAX: int = 1610613701
         self.AXISZYMINZMIN: int = 1610613700
         self.AXI_TYPE_EXTRUDE: int = 1
         self.AXI_TYPE_ROTATE: int = 0
         self.BACKGROUND: int = 1610613563
         self.BACKGROUNDIMAGE: int = 1610613008
         self.BACKGROUNDIMAGENAME: int = 1610613616
-        self.BACKGROUNDRGB: int = 1610613565
+        self.BACKGROUNDRGB: int = 1610613564
         self.BACKGROUNDTRANSPARENCY: int = 1610613737
         self.BACKGROUNDTYPE: int = 1610613605
         self.BEGINSIMTIME: int = 1610613798
         self.BIGHANDRANGE: int = 1610613559
         self.BIGHANDRGB: int = 1610613557
         self.BLANKINGALGORITHM: int = 1610613477
         self.BLANKINGCLIPALG: int = 1610613476
         self.BLANKINGTHRESHOLD: int = 1610613475
-        self.BLANKINGVARIABLE1: int = 1610613471
+        self.BLANKINGVARIABLE1: int = 1610613470
         self.BLANKINGVARIABLE2: int = 1610613472
         self.BLENDLEVELS: int = 1610613607
         self.BLENDPOSITION2: int = 1610613615
         self.BLENDPOSITION3: int = 1610613614
         self.BLENDPOSITION4: int = 1610613613
         self.BLENDRGB1: int = 1610613612
         self.BLENDRGB2: int = 1610613611
@@ -32733,15 +32733,15 @@
         self.CONSTANT_VALUE: int = 1610612961
         self.CONSTRAINDISTANCE: int = 1610613820
         self.CONSTRAINT: int = 1610613333
         self.CONSTRAINTIME: int = 1610613821
         self.CONTOUR_LABEL_HORIZ: int = 0
         self.CONTOUR_LABEL_TANGN: int = 1
         self.CONTROLPOINTS: int = 1610613030
-        self.COOLINGCHANNELCOMP: int = 1610613470
+        self.COOLINGCHANNELCOMP: int = 1610613471
         self.CORE: int = 1610613041
         self.CORE2DTRANSFORM: int = 1610613017
         self.CORETRANSFORM: int = 1610613016
         self.CREATE_REPORT_TEMPLATE: int = 1610612758
         self.CT_BOX: int = 10
         self.CT_CONE: int = 4
         self.CT_CYLD: int = 2
@@ -32751,15 +32751,15 @@
         self.CT_PART: int = 6
         self.CT_PLNE: int = 1
         self.CT_REVO: int = 5
         self.CT_RTZ: int = 11
         self.CT_SPHR: int = 3
         self.CT_SPLINE: int = 12
         self.CT_XYZ: int = 9
-        self.CULLELEMENTS: int = 1610613165
+        self.CULLELEMENTS: int = 1610613166
         self.CULL_BACK_FACE: int = 0
         self.CULL_FRONT_FACE: int = 1
         self.CULL_NO_FACE: int = 2
         self.CURRENT: int = 1610612759
         self.CURRENTCASE: int = 1610612824
         self.CURRENTFRAME: int = 1610613048
         self.CURRENTGUI: int = 1610612878
@@ -32806,15 +32806,15 @@
         self.CVF_ATTR_NO_MINIMUM: int = 16
         self.CVF_ATTR_OBJPTR: int = 13
         self.CVF_ATTR_PSTRING: int = 8
         self.CVF_ATTR_PTR: int = 9
         self.CVF_ATTR_READONLY: int = 256
         self.CVF_ATTR_SOBJPTR: int = 12
         self.CVF_ATTR_STRING: int = 7
-        self.CVF_ATTR_USERFLG_MASK: int = -65536
+        self.CVF_ATTR_USERFLG_MASK: int = 4294901760
         self.CVF_ATTR_VARID: int = 4
         self.CVF_CP_UTF8: int = 65001
         self.CVF_FONT_BOLD: int = 2
         self.CVF_FONT_DEMILIGHT: int = 256
         self.CVF_FONT_ITALIC: int = 4
         self.CVF_FONT_LIGHT: int = 128
         self.CVF_FONT_NARROW: int = 32
@@ -32839,16 +32839,16 @@
         self.CVF_JLC_RUSERNAME: int = 7006
         self.CVF_JLC_TIMEOUT: int = 7010
         self.CVF_LANG_UNKNOWN: int = 0
         self.CVF_PALETTE_UNDEFINED_AS_ZERO_VALUE: int = 30
         self.CVF_PALETTE_UNDEFINED_BY_INVISIBLE: int = 20
         self.CVF_PALETTE_UNDEFINED_BY_PART_COLOR: int = 10
         self.CVF_PALETTE_UNDEFINED_BY_UNDEF_COLOR: int = 40
-        self.CYLDAXISVECT: int = 1610613268
-        self.CYLDENDPOINT: int = 1610613267
+        self.CYLDAXISVECT: int = 1610613267
+        self.CYLDENDPOINT: int = 1610613268
         self.CYLDORIGIN: int = 1610613266
         self.CYLDRADIUS: int = 1610613265
         self.DATA_BIGENDIAN: int = 0
         self.DATA_LITTLEENDIAN: int = 1
         self.DATA_NATIVE: int = 2
         self.DEFAULTANNOTS: int = 1610612826
         self.DEFAULTPARTS: int = 1610612825
@@ -32914,15 +32914,15 @@
         self.ELE_FAILED_EQUAL: int = 3
         self.ELE_FAILED_GREATER: int = 1
         self.ELE_FAILED_LESS: int = 2
         self.ELE_FAILED_LOGIC_AND: int = 1
         self.ELE_FAILED_LOGIC_NONE: int = 0
         self.ELE_FAILED_LOGIC_OR: int = 2
         self.ELE_FAILED_NOT_EQUAL: int = 4
-        self.ELTBLANKING: int = 1610613166
+        self.ELTBLANKING: int = 1610613165
         self.ELTDEFINEDBY: int = 1610613174
         self.ELTFEATUREANGLE: int = 1610613160
         self.ELTFILTER1ACTIVE: int = 1610613184
         self.ELTFILTER1TESTOP: int = 1610613187
         self.ELTFILTER1TESTVALUE: int = 1610613188
         self.ELTFILTER1TESTVARCOMP: int = 1610613190
         self.ELTFILTER1TESTVARIABLE: int = 1610613189
@@ -33102,32 +33102,32 @@
         self.EPSILON: int = 1610613454
         self.EQUATION: int = 1610613304
         self.EXIST_CASE: int = 1610612955
         self.EXPRESSION: int = 1610612951
         self.EXTENTS: int = 1610613233
         self.E_FORMAT: int = 1
         self.FACEAREAFRACTION: int = 1610613450
-        self.FACEXMAXGRID: int = 1610613724
-        self.FACEXMAXGRIDFILTER: int = 1610613728
-        self.FACEXMAXSUBGRID: int = 1610613727
+        self.FACEXMAXGRID: int = 1610613720
+        self.FACEXMAXGRIDFILTER: int = 1610613722
+        self.FACEXMAXSUBGRID: int = 1610613721
         self.FACEXMINGRID: int = 1610613711
-        self.FACEXMINGRIDFILTER: int = 1610613719
+        self.FACEXMINGRIDFILTER: int = 1610613713
         self.FACEXMINSUBGRID: int = 1610613712
-        self.FACEYMAXGRID: int = 1610613722
+        self.FACEYMAXGRID: int = 1610613723
         self.FACEYMAXGRIDFILTER: int = 1610613725
-        self.FACEYMAXSUBGRID: int = 1610613723
-        self.FACEYMINGRID: int = 1610613713
-        self.FACEYMINGRIDFILTER: int = 1610613715
-        self.FACEYMINSUBGRID: int = 1610613714
-        self.FACEZMAXGRID: int = 1610613720
-        self.FACEZMAXGRIDFILTER: int = 1610613721
-        self.FACEZMAXSUBGRID: int = 1610613726
-        self.FACEZMINGRID: int = 1610613716
-        self.FACEZMINGRIDFILTER: int = 1610613718
-        self.FACEZMINSUBGRID: int = 1610613717
+        self.FACEYMAXSUBGRID: int = 1610613724
+        self.FACEYMINGRID: int = 1610613714
+        self.FACEYMINGRIDFILTER: int = 1610613716
+        self.FACEYMINSUBGRID: int = 1610613715
+        self.FACEZMAXGRID: int = 1610613726
+        self.FACEZMAXGRIDFILTER: int = 1610613728
+        self.FACEZMAXSUBGRID: int = 1610613727
+        self.FACEZMINGRID: int = 1610613717
+        self.FACEZMINGRIDFILTER: int = 1610613719
+        self.FACEZMINSUBGRID: int = 1610613718
         self.FALSE: int = 0
         self.FASTDISPLAY: int = 1610612856
         self.FEATURE_ANGLE: int = 2
         self.FEATURE_FULL: int = 6
         self.FEA_VAR: int = 1677721619
         self.FILENAME: int = 1610613044
         self.FILL: int = 1610613573
@@ -33382,22 +33382,22 @@
         self.MASSEDBALLISTICCOEF: int = 1610613371
         self.MASSEDBUOYANCY: int = 1610613378
         self.MASSEDCOEFFRICTION: int = 1610613383
         self.MASSEDCOEFRESTITUTION: int = 1610613382
         self.MASSEDDRAG: int = 1610613363
         self.MASSEDDRAGCOEFFICIENT: int = 1610613366
         self.MASSEDDRAGCOEFFICIENTVAL: int = 1610613367
-        self.MASSEDFLUIDDENSITY: int = 1610613373
+        self.MASSEDFLUIDDENSITY: int = 1610613374
         self.MASSEDFLUIDDENSITYVAL: int = 1610613375
         self.MASSEDFLUIDVISCOSITY: int = 1610613368
         self.MASSEDFLUIDVISCOSITYVAL: int = 1610613369
         self.MASSEDGRAVITY: int = 1610613376
         self.MASSEDGRAVITYVECTOR: int = 1610613377
         self.MASSEDINITIALUSEFLUID: int = 1610613372
-        self.MASSEDINITIALVELOCITY: int = 1610613374
+        self.MASSEDINITIALVELOCITY: int = 1610613373
         self.MASSEDPARTICLEDENSITY: int = 1610613365
         self.MASSEDPARTICLEDIAMETER: int = 1610613364
         self.MASSEDPARTICLES: int = 1610613362
         self.MASSEDPRESSURE: int = 1610613379
         self.MASSEDPRESSUREGRADIENT: int = 1610613380
         self.MASSEDREBOUND: int = 1610613381
         self.MASSEDREBOUNDFRACTION: int = 1610613384
@@ -33521,32 +33521,32 @@
         self.NUMOFSLICES: int = 1610613441
         self.NUMPOINTS: int = 1610613037
         self.OBJECTFOCUS: int = 1610612944
         self.OBJECT_API_JOURNAL: int = 1610612870
         self.OBJECT_DTOR: int = 1610612918
         self.OFFSET: int = 1610612810
         self.OFFSETFROMPART: int = 1610613408
-        self.OFFSETSCALE: int = 1610613409
-        self.OFFSETVECTOR: int = 1610613410
+        self.OFFSETSCALE: int = 1610613410
+        self.OFFSETVECTOR: int = 1610613409
         self.ONE: int = 1
         self.OPAQUENESS: int = 1610613102
         self.OPERATION: int = 1610613817
         self.OPERATIONFACTOR1: int = 1610613813
         self.OPERATIONFACTOR2: int = 1610613814
         self.OPERATIONQUERY1BYNAME: int = 1610613815
         self.OPERATIONQUERY2BYNAME: int = 1610613816
         self.OPTION_NONE: int = -1
         self.ORDER: int = 1610612946
         self.ORIENTATION: int = 1610613522
         self.ORIGIN: int = 1610613313
         self.ORIGIN1: int = 1610613515
         self.ORIGIN2: int = 1610613516
         self.ORIGINBY: int = 1610613502
-        self.ORIGINBY1: int = 1610613518
-        self.ORIGINBY2: int = 1610613517
+        self.ORIGINBY1: int = 1610613517
+        self.ORIGINBY2: int = 1610613518
         self.ORIGINBYPARTCENTROID: int = 1610613444
         self.ORIGINFRAME: int = 1610613505
         self.ORIGINX: int = 1610613603
         self.ORIGINY: int = 1610613604
         self.ORIGIN_NODE_ID: int = 1610613086
         self.ORIGIN_OPTION: int = 1610613084
         self.ORIGIN_PART_ID: int = 1610613085
@@ -34102,15 +34102,15 @@
         self.USE_LOGO: int = 1610612755
         self.UUID: int = 1610612747
         self.VALUE: int = 1610613312
         self.VALUEDECIMALPLACES: int = 1610613571
         self.VALUEFORMAT: int = 1610613570
         self.VALUEIJK: int = 1610613236
         self.VALUELOCATION: int = 1610613569
-        self.VALUERGB: int = 1610613564
+        self.VALUERGB: int = 1610613565
         self.VALUERTZ: int = 1610613245
         self.VALUESIZE: int = 1610613566
         self.VALUESPLINE: int = 1610613247
         self.VALUEXYZ: int = 1610613242
         self.VARCOMP: int = 1610612993
         self.VARIABLE: int = 1610612988
         self.VARIABLE1: int = 1610613796
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/enshell.proto` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/enshell.proto`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 // mimic EnShell commands by always returning EnShellReturnEnum and any other value(s)
 service EnShellService
 {
     rpc exit_cleanly (google.protobuf.Empty) returns (google.protobuf.Empty) {}
     rpc is_enshell_running (EnShellRoleName) returns (EnShellReturnString) {}
     rpc is_everyone_ready (google.protobuf.Empty) returns (EnShellReturnString) {}
     rpc run_command (EnShellCommandLine) returns (EnShellReturnString) {}
-    rpc run_command_with_env (EnShellCommandWithEnvLine) returns (EnShellReturnString) {}
     rpc show_net (google.protobuf.Empty) returns (EnShellReturnString) {}
 
     // standard grpc.health.v1 health check 
     // rpc Check(health.HealthCheckRequest) returns (health.HealthCheckResponse);
     // rpc Watch(health.HealthCheckRequest) returns (stream health.HealthCheckResponse);
 
 }
@@ -29,20 +28,14 @@
 }
 
 message EnShellCommandLine
 {
   string command_line = 1;
 }
 
-message EnShellCommandWithEnvLine
-{
-  string command_line = 1;
-  string env_line = 2;
-}
-
 enum EnShellReturnEnum {
   ENSHELL_ERROR_OK = 0;               // match the codes for CvfErrorCode
   ENSHELL_ERROR_MISC = 1;
   ENSHELL_ERROR_ALLOC = 2;
   ENSHELL_ERROR_LISTDONE = 3;
   ENSHELL_ERROR_BADID = 4;
   ENSHELL_ERROR_THREAD = 5;
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/ensight.proto` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/ensight_api.xml` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight_api.xml`

 * *Files 0% similar despite different names*

#### Comparing `ansys-api-pyensight-0.2.2/src/ansys/api/pyensight/v0/ensight_api.xml` & `ansys-api-pyensight-0.2.dev0/src/ansys/api/pyensight/v0/ensight_api.xml`

```diff
@@ -6356,29 +6356,29 @@
 Origin 2
 
 Supported operations:
     getattr, setattr
 Datatype:
     Float, 3 element array
 "/>
-        <property name="ORIGINBY2" type="int" ns="ensight.objs.ENS_ANNOT.ORIGINBY2" ro="0" description="ORIGINBY2 property
+        <property name="ORIGINBY1" type="int" ns="ensight.objs.ENS_ANNOT.ORIGINBY1" ro="0" description="ORIGINBY1 property
 
-Origin by 2
+Origin by 1
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
     * ensight.objs.enums.ANNOT_3D_SPACE - 3d_coords
 "/>
-        <property name="ORIGINBY1" type="int" ns="ensight.objs.ENS_ANNOT.ORIGINBY1" ro="0" description="ORIGINBY1 property
+        <property name="ORIGINBY2" type="int" ns="ensight.objs.ENS_ANNOT.ORIGINBY2" ro="0" description="ORIGINBY2 property
 
-Origin by 1
+Origin by 2
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.ANNOT_2D_SPACE - screen_coords
@@ -7812,24 +7812,24 @@
 Visible
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="VALUERGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.VALUERGB" ro="0" description="VALUERGB property
+        <property name="BACKGROUNDRGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.BACKGROUNDRGB" ro="0" description="BACKGROUNDRGB property
 
 Color
 
 Supported operations:
     getattr, setattr
 Datatype:
     Color RGB, 3 element array
 "/>
-        <property name="BACKGROUNDRGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.BACKGROUNDRGB" ro="0" description="BACKGROUNDRGB property
+        <property name="VALUERGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.VALUERGB" ro="0" description="VALUERGB property
 
 Color
 
 Supported operations:
     getattr, setattr
 Datatype:
     Color RGB, 3 element array
@@ -8079,26 +8079,26 @@
 Visible
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="VALUERGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.VALUERGB" ro="0" description="VALUERGB property
+        <property name="BACKGROUNDRGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.BACKGROUNDRGB" ro="0" description="BACKGROUNDRGB property
 
 Color
 
 Supported operations:
     getattr, setattr
 Datatype:
     Color RGB, 3 element array
 Range:
     [0.0, 1.0]
 "/>
-        <property name="BACKGROUNDRGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.BACKGROUNDRGB" ro="0" description="BACKGROUNDRGB property
+        <property name="VALUERGB" type="List[float]" ns="ensight.objs.ENS_ANNOT.VALUERGB" ro="0" description="VALUERGB property
 
 Color
 
 Supported operations:
     getattr, setattr
 Datatype:
     Color RGB, 3 element array
@@ -13460,35 +13460,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -15564,35 +15564,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -17700,35 +17700,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -18194,26 +18194,26 @@
 Origin
 
 Supported operations:
     getattr, setattr
 Datatype:
     Float, 3 element array
 "/>
-        <property name="CYLDENDPOINT" type="List[float]" ns="ensight.objs.ENS_PART.CYLDENDPOINT" ro="0" description="CYLDENDPOINT property
+        <property name="CYLDAXISVECT" type="List[float]" ns="ensight.objs.ENS_PART.CYLDAXISVECT" ro="0" description="CYLDAXISVECT property
 
-End point
+Axis vector
 
 Supported operations:
     getattr, setattr
 Datatype:
     Float, 3 element array
 "/>
-        <property name="CYLDAXISVECT" type="List[float]" ns="ensight.objs.ENS_PART.CYLDAXISVECT" ro="0" description="CYLDAXISVECT property
+        <property name="CYLDENDPOINT" type="List[float]" ns="ensight.objs.ENS_PART.CYLDENDPOINT" ro="0" description="CYLDENDPOINT property
 
-Axis vector
+End point
 
 Supported operations:
     getattr, setattr
 Datatype:
     Float, 3 element array
 "/>
         <property name="CONEANGLE" type="float" ns="ensight.objs.ENS_PART.CONEANGLE" ro="0" description="CONEANGLE property
@@ -20057,35 +20057,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -21686,35 +21686,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -24313,35 +24313,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -25886,35 +25886,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -26358,35 +26358,35 @@
 Use fluid for initial velocity
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="MASSEDFLUIDDENSITY" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.MASSEDFLUIDDENSITY" ro="0" description="MASSEDFLUIDDENSITY property
+        <property name="MASSEDINITIALVELOCITY" type="List[float]" ns="ensight.objs.ENS_PART.MASSEDINITIALVELOCITY" ro="0" description="MASSEDINITIALVELOCITY property
 
 Fluid density
 
 Supported operations:
     getattr, setattr
 Datatype:
-    ENS_VAR Object, scalar
-Variable type filters:
-    * Scalar
-    * Nodal
-    * Element
+    Float, 3 element array
 "/>
-        <property name="MASSEDINITIALVELOCITY" type="List[float]" ns="ensight.objs.ENS_PART.MASSEDINITIALVELOCITY" ro="0" description="MASSEDINITIALVELOCITY property
+        <property name="MASSEDFLUIDDENSITY" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.MASSEDFLUIDDENSITY" ro="0" description="MASSEDFLUIDDENSITY property
 
 Fluid density
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Float, 3 element array
+    ENS_VAR Object, scalar
+Variable type filters:
+    * Scalar
+    * Nodal
+    * Element
 "/>
         <property name="MASSEDFLUIDDENSITYVAL" type="float" ns="ensight.objs.ENS_PART.MASSEDFLUIDDENSITYVAL" ro="0" description="MASSEDFLUIDDENSITYVAL property
 
 Fluid density value
 
 Supported operations:
     getattr, setattr
@@ -27867,35 +27867,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -29377,35 +29377,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -31057,35 +31057,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -31224,31 +31224,31 @@
 Offset from part
 
 Supported operations:
     getattr, setattr
 Datatype:
     Integer, scalar
 "/>
-        <property name="OFFSETSCALE" type="float" ns="ensight.objs.ENS_PART.OFFSETSCALE" ro="0" description="OFFSETSCALE property
+        <property name="OFFSETVECTOR" type="List[float]" ns="ensight.objs.ENS_PART.OFFSETVECTOR" ro="0" description="OFFSETVECTOR property
 
-Offset scale
+Offset vector
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Float, scalar
+    Float, 3 element array
 "/>
-        <property name="OFFSETVECTOR" type="List[float]" ns="ensight.objs.ENS_PART.OFFSETVECTOR" ro="0" description="OFFSETVECTOR property
+        <property name="OFFSETSCALE" type="float" ns="ensight.objs.ENS_PART.OFFSETSCALE" ro="0" description="OFFSETSCALE property
 
-Offset vector
+Offset scale
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Float, 3 element array
+    Float, scalar
 "/>
       </class>
       <class name="ENS_PART_DEVELOPED_SURFACE" ns="ensight.objs.ENS_PART" super="ENS_PART" subtypeattr="PARTTYPE" subtypevalue="10">
         <method name="__init__"/>
         <property name="__ids__" type="List[int]" ns="ensight.objs.ENS_PART.__ids__" ro="1"/>
         <method name="setattr" ns="ensight.objs.ENS_PART.setattr" description="Set object attribute"/>
         <method name="setattr_begin" ns="ensight.objs.ENS_PART.setattr_begin" description="Begin setting multiple attributes"/>
@@ -32592,35 +32592,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -34103,35 +34103,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -35568,35 +35568,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -37165,35 +37165,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -38747,35 +38747,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -40393,35 +40393,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -41973,35 +41973,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -43448,35 +43448,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -44917,35 +44917,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -46465,35 +46465,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -46867,30 +46867,30 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Integer, scalar
 Range:
     [0, inf]
 "/>
-        <property name="COOLINGCHANNELCOMP" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.COOLINGCHANNELCOMP" ro="0" description="COOLINGCHANNELCOMP property
+        <property name="BLANKINGVARIABLE1" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.BLANKINGVARIABLE1" ro="0" description="BLANKINGVARIABLE1 property
 
-Component ID of cooling channel
+Blanking variable1
 
 Supported operations:
     getattr, setattr
 Datatype:
     ENS_VAR Object, scalar
 Variable type filters:
     * Scalar
     * Nodal
     * Element
 "/>
-        <property name="BLANKINGVARIABLE1" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.BLANKINGVARIABLE1" ro="0" description="BLANKINGVARIABLE1 property
+        <property name="COOLINGCHANNELCOMP" type="'ensobjlist'['ENS_VAR']" ns="ensight.objs.ENS_PART.COOLINGCHANNELCOMP" ro="0" description="COOLINGCHANNELCOMP property
 
-Blanking variable1
+Component ID of cooling channel
 
 Supported operations:
     getattr, setattr
 Datatype:
     ENS_VAR Object, scalar
 Variable type filters:
     * Scalar
@@ -48367,35 +48367,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -49940,35 +49940,35 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [0.0, 1.0]
 "/>
-        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
+        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.CULL_BACK_FACE - facing_back
-    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
-    * ensight.objs.enums.CULL_NO_FACE - off
+    Boolean, scalar
 "/>
-        <property name="ELTBLANKING" type="int" ns="ensight.objs.ENS_PART.ELTBLANKING" ro="0" description="ELTBLANKING property
+        <property name="CULLELEMENTS" type="int" ns="ensight.objs.ENS_PART.CULLELEMENTS" ro="0" description="CULLELEMENTS property
 
 Do not show elements
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Boolean, scalar
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.CULL_BACK_FACE - facing_back
+    * ensight.objs.enums.CULL_FRONT_FACE - facing_front
+    * ensight.objs.enums.CULL_NO_FACE - off
 "/>
         <property name="HIDDENSURFACE" type="int" ns="ensight.objs.ENS_PART.HIDDENSURFACE" ro="0" description="HIDDENSURFACE property
 
 Hidden surface
 
 Supported operations:
     getattr, setattr
@@ -50879,23 +50879,14 @@
 Title text
 
 Supported operations:
     getattr, setattr
 Datatype:
     String, 1024 characters maximum
 "/>
-        <property name="AXISYTITLE" type="str" ns="ensight.objs.ENS_PLOTTER.AXISYTITLE" ro="0" description="AXISYTITLE property
-
-Title text
-
-Supported operations:
-    getattr, setattr
-Datatype:
-    String, 1024 characters maximum
-"/>
         <property name="AXISXTITLESIZE" type="int" ns="ensight.objs.ENS_PLOTTER.AXISXTITLESIZE" ro="0" description="AXISXTITLESIZE property
 
 Title size
 
 Supported operations:
     getattr, setattr
 Datatype:
@@ -50976,14 +50967,23 @@
 Supported operations:
     getattr, setattr
 Datatype:
     Float, scalar
 Range:
     [1.0, 100.0]
 "/>
+        <property name="AXISYTITLE" type="str" ns="ensight.objs.ENS_PLOTTER.AXISYTITLE" ro="0" description="AXISYTITLE property
+
+Title text
+
+Supported operations:
+    getattr, setattr
+Datatype:
+    String, 1024 characters maximum
+"/>
         <property name="AXISYTITLESIZE" type="int" ns="ensight.objs.ENS_PLOTTER.AXISYTITLESIZE" ro="0" description="AXISYTITLESIZE property
 
 Title size
 
 Supported operations:
     getattr, setattr
 Datatype:
@@ -56248,23 +56248,14 @@
 Title
 
 Supported operations:
     getattr, setattr
 Datatype:
     String, 1024 characters maximum
 "/>
-        <property name="AXISYTITLE" type="str" ns="ensight.objs.ENS_VPORT.AXISYTITLE" ro="0" description="AXISYTITLE property
-
-Title
-
-Supported operations:
-    getattr, setattr
-Datatype:
-    String, 1024 characters maximum
-"/>
         <property name="AXISXTITLESIZE" type="int" ns="ensight.objs.ENS_VPORT.AXISXTITLESIZE" ro="0" description="AXISXTITLESIZE property
 
 Title size
 
 Supported operations:
     getattr, setattr
 Datatype:
@@ -56487,14 +56478,23 @@
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
     * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
     * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
 "/>
+        <property name="AXISYTITLE" type="str" ns="ensight.objs.ENS_VPORT.AXISYTITLE" ro="0" description="AXISYTITLE property
+
+Title
+
+Supported operations:
+    getattr, setattr
+Datatype:
+    String, 1024 characters maximum
+"/>
         <property name="AXISYTITLESIZE" type="int" ns="ensight.objs.ENS_VPORT.AXISYTITLESIZE" ro="0" description="AXISYTITLESIZE property
 
 Title size
 
 Supported operations:
     getattr, setattr
 Datatype:
@@ -56547,39 +56547,39 @@
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.XY_LABEL_NONE - none
     * ensight.objs.enums.XY_LABEL_ALL - all
     * ensight.objs.enums.XY_LABEL_BEG_END - beg_end
 "/>
-        <property name="AXISYLABELFILTER" type="int" ns="ensight.objs.ENS_VPORT.AXISYLABELFILTER" ro="0" description="AXISYLABELFILTER property
+        <property name="AXISYLABELEXTENTLOC" type="int" ns="ensight.objs.ENS_VPORT.AXISYLABELEXTENTLOC" ro="0" description="AXISYLABELEXTENTLOC property
 
 Value filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
-    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
 "/>
-        <property name="AXISYLABELEXTENTLOC" type="int" ns="ensight.objs.ENS_VPORT.AXISYLABELEXTENTLOC" ro="0" description="AXISYLABELEXTENTLOC property
+        <property name="AXISYLABELFILTER" type="int" ns="ensight.objs.ENS_VPORT.AXISYLABELFILTER" ro="0" description="AXISYLABELFILTER property
 
 Value filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
 "/>
         <property name="AXISYFORMAT" type="str" ns="ensight.objs.ENS_VPORT.AXISYFORMAT" ro="0" description="AXISYFORMAT property
 
 Value format
 
 Supported operations:
     getattr, setattr
@@ -56777,39 +56777,39 @@
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.XY_LABEL_NONE - none
     * ensight.objs.enums.XY_LABEL_ALL - all
     * ensight.objs.enums.XY_LABEL_BEG_END - beg_end
 "/>
-        <property name="AXISZLABELFILTER" type="int" ns="ensight.objs.ENS_VPORT.AXISZLABELFILTER" ro="0" description="AXISZLABELFILTER property
+        <property name="AXISZLABELEXTENTLOC" type="int" ns="ensight.objs.ENS_VPORT.AXISZLABELEXTENTLOC" ro="0" description="AXISZLABELEXTENTLOC property
 
 Value filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
-    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
+    * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
 "/>
-        <property name="AXISZLABELEXTENTLOC" type="int" ns="ensight.objs.ENS_VPORT.AXISZLABELEXTENTLOC" ro="0" description="AXISZLABELEXTENTLOC property
+        <property name="AXISZLABELFILTER" type="int" ns="ensight.objs.ENS_VPORT.AXISZLABELFILTER" ro="0" description="AXISZLABELFILTER property
 
 Value filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MINIMUM - min
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MAXIMUM - max
-    * ensight.objs.enums.STAGE_SHOW_STUFF_MINANDMAX - both
+    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
 "/>
         <property name="AXISZFORMAT" type="str" ns="ensight.objs.ENS_VPORT.AXISZFORMAT" ro="0" description="AXISZFORMAT property
 
 Value format
 
 Supported operations:
     getattr, setattr
@@ -56956,14 +56956,27 @@
 Sub Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
+        <property name="FACEXMINGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEXMINGRIDFILTER" ro="0" description="FACEXMINGRIDFILTER property
+
+Face filter
+
+Supported operations:
+    getattr, setattr
+Datatype:
+    Enum, scalar
+Enums:
+    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
+    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
+    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+"/>
         <property name="FACEYMINGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEYMINGRID" ro="0" description="FACEYMINGRID property
 
 Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
@@ -57018,37 +57031,33 @@
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
     * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
     * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
 "/>
-        <property name="FACEXMINGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEXMINGRIDFILTER" ro="0" description="FACEXMINGRIDFILTER property
+        <property name="FACEXMAXGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXGRID" ro="0" description="FACEXMAXGRID property
 
-Face filter
+Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
-    Enum, scalar
-Enums:
-    * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
-    * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
-    * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
+    Boolean, scalar
 "/>
-        <property name="FACEZMAXGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXGRID" ro="0" description="FACEZMAXGRID property
+        <property name="FACEXMAXSUBGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXSUBGRID" ro="0" description="FACEXMAXSUBGRID property
 
-Grid/Tick show
+Sub Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="FACEZMAXGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXGRIDFILTER" ro="0" description="FACEZMAXGRIDFILTER property
+        <property name="FACEXMAXGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXGRIDFILTER" ro="0" description="FACEXMAXGRIDFILTER property
 
 Face filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
@@ -57071,55 +57080,46 @@
 Sub Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="FACEXMAXGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXGRID" ro="0" description="FACEXMAXGRID property
-
-Grid/Tick show
-
-Supported operations:
-    getattr, setattr
-Datatype:
-    Boolean, scalar
-"/>
         <property name="FACEYMAXGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEYMAXGRIDFILTER" ro="0" description="FACEYMAXGRIDFILTER property
 
 Face filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
 Enums:
     * ensight.objs.enums.STAGE_LABEL_BACK_FACES - facing_back
     * ensight.objs.enums.STAGE_LABEL_FRONT_FACES - facing_front
     * ensight.objs.enums.STAGE_LABEL_FRONT_AND_BACK_FACES - off
 "/>
-        <property name="FACEZMAXSUBGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXSUBGRID" ro="0" description="FACEZMAXSUBGRID property
+        <property name="FACEZMAXGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXGRID" ro="0" description="FACEZMAXGRID property
 
-Sub Grid/Tick show
+Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="FACEXMAXSUBGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXSUBGRID" ro="0" description="FACEXMAXSUBGRID property
+        <property name="FACEZMAXSUBGRID" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXSUBGRID" ro="0" description="FACEZMAXSUBGRID property
 
 Sub Grid/Tick show
 
 Supported operations:
     getattr, setattr
 Datatype:
     Boolean, scalar
 "/>
-        <property name="FACEXMAXGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEXMAXGRIDFILTER" ro="0" description="FACEXMAXGRIDFILTER property
+        <property name="FACEZMAXGRIDFILTER" type="int" ns="ensight.objs.ENS_VPORT.FACEZMAXGRIDFILTER" ro="0" description="FACEZMAXGRIDFILTER property
 
 Face filter
 
 Supported operations:
     getattr, setattr
 Datatype:
     Enum, scalar
@@ -57327,56 +57327,56 @@
         <variable name="AXISLINEWIDTH" type="int" ns="ensight.objs.enums.AXISLINEWIDTH">1610613630</variable>
         <variable name="AXISLOCAL" type="int" ns="ensight.objs.enums.AXISLOCAL">1610612923</variable>
         <variable name="AXISMODEL" type="int" ns="ensight.objs.enums.AXISMODEL">1610612925</variable>
         <variable name="AXISMODEL_ANIMATE" type="int" ns="ensight.objs.enums.AXISMODEL_ANIMATE">1610612926</variable>
         <variable name="AXISMODEL_LOCATION" type="int" ns="ensight.objs.enums.AXISMODEL_LOCATION">1610612927</variable>
         <variable name="AXISRGB" type="int" ns="ensight.objs.enums.AXISRGB">1610613631</variable>
         <variable name="AXISSWAP" type="int" ns="ensight.objs.enums.AXISSWAP">1610613751</variable>
-        <variable name="AXISWIDTH" type="int" ns="ensight.objs.enums.AXISWIDTH">1610613650</variable>
+        <variable name="AXISWIDTH" type="int" ns="ensight.objs.enums.AXISWIDTH">1610613649</variable>
         <variable name="AXISXAUTOSCALE" type="int" ns="ensight.objs.enums.AXISXAUTOSCALE">1610613760</variable>
-        <variable name="AXISXDISPLAYONEDGE" type="int" ns="ensight.objs.enums.AXISXDISPLAYONEDGE">1610613656</variable>
-        <variable name="AXISXFORMAT" type="int" ns="ensight.objs.enums.AXISXFORMAT">1610613654</variable>
-        <variable name="AXISXGRIDEXTENTLOC" type="int" ns="ensight.objs.enums.AXISXGRIDEXTENTLOC">1610613667</variable>
-        <variable name="AXISXGRIDTYPE" type="int" ns="ensight.objs.enums.AXISXGRIDTYPE">1610613661</variable>
-        <variable name="AXISXLABELAXISLOC" type="int" ns="ensight.objs.enums.AXISXLABELAXISLOC">1610613651</variable>
-        <variable name="AXISXLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISXLABELEXTENTLOC">1610613652</variable>
-        <variable name="AXISXLABELFILTER" type="int" ns="ensight.objs.enums.AXISXLABELFILTER">1610613653</variable>
+        <variable name="AXISXDISPLAYONEDGE" type="int" ns="ensight.objs.enums.AXISXDISPLAYONEDGE">1610613655</variable>
+        <variable name="AXISXFORMAT" type="int" ns="ensight.objs.enums.AXISXFORMAT">1610613653</variable>
+        <variable name="AXISXGRIDEXTENTLOC" type="int" ns="ensight.objs.enums.AXISXGRIDEXTENTLOC">1610613666</variable>
+        <variable name="AXISXGRIDTYPE" type="int" ns="ensight.objs.enums.AXISXGRIDTYPE">1610613660</variable>
+        <variable name="AXISXLABELAXISLOC" type="int" ns="ensight.objs.enums.AXISXLABELAXISLOC">1610613650</variable>
+        <variable name="AXISXLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISXLABELEXTENTLOC">1610613651</variable>
+        <variable name="AXISXLABELFILTER" type="int" ns="ensight.objs.enums.AXISXLABELFILTER">1610613652</variable>
         <variable name="AXISXLABELFORMAT" type="int" ns="ensight.objs.enums.AXISXLABELFORMAT">1610613756</variable>
-        <variable name="AXISXLABELRGB" type="int" ns="ensight.objs.enums.AXISXLABELRGB">1610613655</variable>
+        <variable name="AXISXLABELRGB" type="int" ns="ensight.objs.enums.AXISXLABELRGB">1610613654</variable>
         <variable name="AXISXLABELSIZE" type="int" ns="ensight.objs.enums.AXISXLABELSIZE">1610613754</variable>
         <variable name="AXISXLABELTYPE" type="int" ns="ensight.objs.enums.AXISXLABELTYPE">1610613753</variable>
-        <variable name="AXISXMAX" type="int" ns="ensight.objs.enums.AXISXMAX">1610613648</variable>
-        <variable name="AXISXMIN" type="int" ns="ensight.objs.enums.AXISXMIN">1610613647</variable>
-        <variable name="AXISXNUMGRID" type="int" ns="ensight.objs.enums.AXISXNUMGRID">1610613663</variable>
+        <variable name="AXISXMAX" type="int" ns="ensight.objs.enums.AXISXMAX">1610613647</variable>
+        <variable name="AXISXMIN" type="int" ns="ensight.objs.enums.AXISXMIN">1610613646</variable>
+        <variable name="AXISXNUMGRID" type="int" ns="ensight.objs.enums.AXISXNUMGRID">1610613662</variable>
         <variable name="AXISXNUMGRIDLOG" type="int" ns="ensight.objs.enums.AXISXNUMGRIDLOG">1610613757</variable>
-        <variable name="AXISXNUMSUBGRID" type="int" ns="ensight.objs.enums.AXISXNUMSUBGRID">1610613666</variable>
+        <variable name="AXISXNUMSUBGRID" type="int" ns="ensight.objs.enums.AXISXNUMSUBGRID">1610613665</variable>
         <variable name="AXISXNUMSUBGRIDLOG" type="int" ns="ensight.objs.enums.AXISXNUMSUBGRIDLOG">1610613758</variable>
-        <variable name="AXISXORIG" type="int" ns="ensight.objs.enums.AXISXORIG">1610613649</variable>
+        <variable name="AXISXORIG" type="int" ns="ensight.objs.enums.AXISXORIG">1610613648</variable>
         <variable name="AXISXORIGIN" type="int" ns="ensight.objs.enums.AXISXORIGIN">1610613761</variable>
         <variable name="AXISXSCALE" type="int" ns="ensight.objs.enums.AXISXSCALE">1610613755</variable>
-        <variable name="AXISXSGRIDTYPE" type="int" ns="ensight.objs.enums.AXISXSGRIDTYPE">1610613664</variable>
+        <variable name="AXISXSGRIDTYPE" type="int" ns="ensight.objs.enums.AXISXSGRIDTYPE">1610613663</variable>
         <variable name="AXISXSIZE" type="int" ns="ensight.objs.enums.AXISXSIZE">1610613762</variable>
-        <variable name="AXISXSUBTICK" type="int" ns="ensight.objs.enums.AXISXSUBTICK">1610613665</variable>
-        <variable name="AXISXTICK" type="int" ns="ensight.objs.enums.AXISXTICK">1610613662</variable>
+        <variable name="AXISXSUBTICK" type="int" ns="ensight.objs.enums.AXISXSUBTICK">1610613664</variable>
+        <variable name="AXISXTICK" type="int" ns="ensight.objs.enums.AXISXTICK">1610613661</variable>
         <variable name="AXISXTITLE" type="int" ns="ensight.objs.enums.AXISXTITLE">1610613644</variable>
         <variable name="AXISXTITLERGB" type="int" ns="ensight.objs.enums.AXISXTITLERGB">1610613752</variable>
-        <variable name="AXISXTITLESIZE" type="int" ns="ensight.objs.enums.AXISXTITLESIZE">1610613646</variable>
+        <variable name="AXISXTITLESIZE" type="int" ns="ensight.objs.enums.AXISXTITLESIZE">1610613645</variable>
         <variable name="AXISXVISIBLE" type="int" ns="ensight.objs.enums.AXISXVISIBLE">1610613759</variable>
-        <variable name="AXISXYMAXZMAX" type="int" ns="ensight.objs.enums.AXISXYMAXZMAX">1610613660</variable>
-        <variable name="AXISXYMAXZMIN" type="int" ns="ensight.objs.enums.AXISXYMAXZMIN">1610613659</variable>
-        <variable name="AXISXYMINZMAX" type="int" ns="ensight.objs.enums.AXISXYMINZMAX">1610613658</variable>
-        <variable name="AXISXYMINZMIN" type="int" ns="ensight.objs.enums.AXISXYMINZMIN">1610613657</variable>
+        <variable name="AXISXYMAXZMAX" type="int" ns="ensight.objs.enums.AXISXYMAXZMAX">1610613659</variable>
+        <variable name="AXISXYMAXZMIN" type="int" ns="ensight.objs.enums.AXISXYMAXZMIN">1610613658</variable>
+        <variable name="AXISXYMINZMAX" type="int" ns="ensight.objs.enums.AXISXYMINZMAX">1610613657</variable>
+        <variable name="AXISXYMINZMIN" type="int" ns="ensight.objs.enums.AXISXYMINZMIN">1610613656</variable>
         <variable name="AXISYAUTOSCALE" type="int" ns="ensight.objs.enums.AXISYAUTOSCALE">1610613771</variable>
         <variable name="AXISYDISPLAYONEDGE" type="int" ns="ensight.objs.enums.AXISYDISPLAYONEDGE">1610613678</variable>
         <variable name="AXISYFORMAT" type="int" ns="ensight.objs.enums.AXISYFORMAT">1610613676</variable>
         <variable name="AXISYGRIDEXTENTLOC" type="int" ns="ensight.objs.enums.AXISYGRIDEXTENTLOC">1610613690</variable>
         <variable name="AXISYGRIDTYPE" type="int" ns="ensight.objs.enums.AXISYGRIDTYPE">1610613684</variable>
         <variable name="AXISYLABELAXISLOC" type="int" ns="ensight.objs.enums.AXISYLABELAXISLOC">1610613673</variable>
-        <variable name="AXISYLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISYLABELEXTENTLOC">1610613675</variable>
-        <variable name="AXISYLABELFILTER" type="int" ns="ensight.objs.enums.AXISYLABELFILTER">1610613674</variable>
+        <variable name="AXISYLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISYLABELEXTENTLOC">1610613674</variable>
+        <variable name="AXISYLABELFILTER" type="int" ns="ensight.objs.enums.AXISYLABELFILTER">1610613675</variable>
         <variable name="AXISYLABELFORMAT" type="int" ns="ensight.objs.enums.AXISYLABELFORMAT">1610613767</variable>
         <variable name="AXISYLABELRGB" type="int" ns="ensight.objs.enums.AXISYLABELRGB">1610613677</variable>
         <variable name="AXISYLABELSIZE" type="int" ns="ensight.objs.enums.AXISYLABELSIZE">1610613765</variable>
         <variable name="AXISYLABELTYPE" type="int" ns="ensight.objs.enums.AXISYLABELTYPE">1610613764</variable>
         <variable name="AXISYMAX" type="int" ns="ensight.objs.enums.AXISYMAX">1610613670</variable>
         <variable name="AXISYMIN" type="int" ns="ensight.objs.enums.AXISYMIN">1610613669</variable>
         <variable name="AXISYNUMGRID" type="int" ns="ensight.objs.enums.AXISYNUMGRID">1610613686</variable>
@@ -57386,29 +57386,29 @@
         <variable name="AXISYORIG" type="int" ns="ensight.objs.enums.AXISYORIG">1610613671</variable>
         <variable name="AXISYORIGIN" type="int" ns="ensight.objs.enums.AXISYORIGIN">1610613772</variable>
         <variable name="AXISYSCALE" type="int" ns="ensight.objs.enums.AXISYSCALE">1610613766</variable>
         <variable name="AXISYSGRIDTYPE" type="int" ns="ensight.objs.enums.AXISYSGRIDTYPE">1610613687</variable>
         <variable name="AXISYSIZE" type="int" ns="ensight.objs.enums.AXISYSIZE">1610613773</variable>
         <variable name="AXISYSUBTICK" type="int" ns="ensight.objs.enums.AXISYSUBTICK">1610613688</variable>
         <variable name="AXISYTICK" type="int" ns="ensight.objs.enums.AXISYTICK">1610613685</variable>
-        <variable name="AXISYTITLE" type="int" ns="ensight.objs.enums.AXISYTITLE">1610613645</variable>
+        <variable name="AXISYTITLE" type="int" ns="ensight.objs.enums.AXISYTITLE">1610613667</variable>
         <variable name="AXISYTITLERGB" type="int" ns="ensight.objs.enums.AXISYTITLERGB">1610613763</variable>
         <variable name="AXISYTITLESIZE" type="int" ns="ensight.objs.enums.AXISYTITLESIZE">1610613668</variable>
         <variable name="AXISYVISIBLE" type="int" ns="ensight.objs.enums.AXISYVISIBLE">1610613770</variable>
         <variable name="AXISYYMAXZMAX" type="int" ns="ensight.objs.enums.AXISYYMAXZMAX">1610613683</variable>
         <variable name="AXISYYMAXZMIN" type="int" ns="ensight.objs.enums.AXISYYMAXZMIN">1610613682</variable>
         <variable name="AXISYYMINZMAX" type="int" ns="ensight.objs.enums.AXISYYMINZMAX">1610613681</variable>
         <variable name="AXISYYMINZMIN" type="int" ns="ensight.objs.enums.AXISYYMINZMIN">1610613680</variable>
         <variable name="AXISZDISPLAYONEDGE" type="int" ns="ensight.objs.enums.AXISZDISPLAYONEDGE">1610613679</variable>
         <variable name="AXISZFORMAT" type="int" ns="ensight.objs.enums.AXISZFORMAT">1610613698</variable>
         <variable name="AXISZGRIDEXTENTLOC" type="int" ns="ensight.objs.enums.AXISZGRIDEXTENTLOC">1610613710</variable>
         <variable name="AXISZGRIDTYPE" type="int" ns="ensight.objs.enums.AXISZGRIDTYPE">1610613704</variable>
         <variable name="AXISZLABELAXISLOC" type="int" ns="ensight.objs.enums.AXISZLABELAXISLOC">1610613695</variable>
-        <variable name="AXISZLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISZLABELEXTENTLOC">1610613697</variable>
-        <variable name="AXISZLABELFILTER" type="int" ns="ensight.objs.enums.AXISZLABELFILTER">1610613696</variable>
+        <variable name="AXISZLABELEXTENTLOC" type="int" ns="ensight.objs.enums.AXISZLABELEXTENTLOC">1610613696</variable>
+        <variable name="AXISZLABELFILTER" type="int" ns="ensight.objs.enums.AXISZLABELFILTER">1610613697</variable>
         <variable name="AXISZLABELRGB" type="int" ns="ensight.objs.enums.AXISZLABELRGB">1610613699</variable>
         <variable name="AXISZMAX" type="int" ns="ensight.objs.enums.AXISZMAX">1610613694</variable>
         <variable name="AXISZMIN" type="int" ns="ensight.objs.enums.AXISZMIN">1610613693</variable>
         <variable name="AXISZNUMGRID" type="int" ns="ensight.objs.enums.AXISZNUMGRID">1610613706</variable>
         <variable name="AXISZNUMSUBGRID" type="int" ns="ensight.objs.enums.AXISZNUMSUBGRID">1610613709</variable>
         <variable name="AXISZSGRIDTYPE" type="int" ns="ensight.objs.enums.AXISZSGRIDTYPE">1610613707</variable>
         <variable name="AXISZSUBTICK" type="int" ns="ensight.objs.enums.AXISZSUBTICK">1610613708</variable>
@@ -57420,24 +57420,24 @@
         <variable name="AXISZYMINZMAX" type="int" ns="ensight.objs.enums.AXISZYMINZMAX">1610613701</variable>
         <variable name="AXISZYMINZMIN" type="int" ns="ensight.objs.enums.AXISZYMINZMIN">1610613700</variable>
         <variable name="AXI_TYPE_EXTRUDE" type="int" ns="ensight.objs.enums.AXI_TYPE_EXTRUDE">1</variable>
         <variable name="AXI_TYPE_ROTATE" type="int" ns="ensight.objs.enums.AXI_TYPE_ROTATE">0</variable>
         <variable name="BACKGROUND" type="int" ns="ensight.objs.enums.BACKGROUND">1610613563</variable>
         <variable name="BACKGROUNDIMAGE" type="int" ns="ensight.objs.enums.BACKGROUNDIMAGE">1610613008</variable>
         <variable name="BACKGROUNDIMAGENAME" type="int" ns="ensight.objs.enums.BACKGROUNDIMAGENAME">1610613616</variable>
-        <variable name="BACKGROUNDRGB" type="int" ns="ensight.objs.enums.BACKGROUNDRGB">1610613565</variable>
+        <variable name="BACKGROUNDRGB" type="int" ns="ensight.objs.enums.BACKGROUNDRGB">1610613564</variable>
         <variable name="BACKGROUNDTRANSPARENCY" type="int" ns="ensight.objs.enums.BACKGROUNDTRANSPARENCY">1610613737</variable>
         <variable name="BACKGROUNDTYPE" type="int" ns="ensight.objs.enums.BACKGROUNDTYPE">1610613605</variable>
         <variable name="BEGINSIMTIME" type="int" ns="ensight.objs.enums.BEGINSIMTIME">1610613798</variable>
         <variable name="BIGHANDRANGE" type="int" ns="ensight.objs.enums.BIGHANDRANGE">1610613559</variable>
         <variable name="BIGHANDRGB" type="int" ns="ensight.objs.enums.BIGHANDRGB">1610613557</variable>
         <variable name="BLANKINGALGORITHM" type="int" ns="ensight.objs.enums.BLANKINGALGORITHM">1610613477</variable>
         <variable name="BLANKINGCLIPALG" type="int" ns="ensight.objs.enums.BLANKINGCLIPALG">1610613476</variable>
         <variable name="BLANKINGTHRESHOLD" type="int" ns="ensight.objs.enums.BLANKINGTHRESHOLD">1610613475</variable>
-        <variable name="BLANKINGVARIABLE1" type="int" ns="ensight.objs.enums.BLANKINGVARIABLE1">1610613471</variable>
+        <variable name="BLANKINGVARIABLE1" type="int" ns="ensight.objs.enums.BLANKINGVARIABLE1">1610613470</variable>
         <variable name="BLANKINGVARIABLE2" type="int" ns="ensight.objs.enums.BLANKINGVARIABLE2">1610613472</variable>
         <variable name="BLENDLEVELS" type="int" ns="ensight.objs.enums.BLENDLEVELS">1610613607</variable>
         <variable name="BLENDPOSITION2" type="int" ns="ensight.objs.enums.BLENDPOSITION2">1610613615</variable>
         <variable name="BLENDPOSITION3" type="int" ns="ensight.objs.enums.BLENDPOSITION3">1610613614</variable>
         <variable name="BLENDPOSITION4" type="int" ns="ensight.objs.enums.BLENDPOSITION4">1610613613</variable>
         <variable name="BLENDRGB1" type="int" ns="ensight.objs.enums.BLENDRGB1">1610613612</variable>
         <variable name="BLENDRGB2" type="int" ns="ensight.objs.enums.BLENDRGB2">1610613611</variable>
@@ -57589,15 +57589,15 @@
         <variable name="CONSTANT_VALUE" type="int" ns="ensight.objs.enums.CONSTANT_VALUE">1610612961</variable>
         <variable name="CONSTRAINDISTANCE" type="int" ns="ensight.objs.enums.CONSTRAINDISTANCE">1610613820</variable>
         <variable name="CONSTRAINT" type="int" ns="ensight.objs.enums.CONSTRAINT">1610613333</variable>
         <variable name="CONSTRAINTIME" type="int" ns="ensight.objs.enums.CONSTRAINTIME">1610613821</variable>
         <variable name="CONTOUR_LABEL_HORIZ" type="int" ns="ensight.objs.enums.CONTOUR_LABEL_HORIZ">0</variable>
         <variable name="CONTOUR_LABEL_TANGN" type="int" ns="ensight.objs.enums.CONTOUR_LABEL_TANGN">1</variable>
         <variable name="CONTROLPOINTS" type="int" ns="ensight.objs.enums.CONTROLPOINTS">1610613030</variable>
-        <variable name="COOLINGCHANNELCOMP" type="int" ns="ensight.objs.enums.COOLINGCHANNELCOMP">1610613470</variable>
+        <variable name="COOLINGCHANNELCOMP" type="int" ns="ensight.objs.enums.COOLINGCHANNELCOMP">1610613471</variable>
         <variable name="CORE" type="int" ns="ensight.objs.enums.CORE">1610613041</variable>
         <variable name="CORE2DTRANSFORM" type="int" ns="ensight.objs.enums.CORE2DTRANSFORM">1610613017</variable>
         <variable name="CORETRANSFORM" type="int" ns="ensight.objs.enums.CORETRANSFORM">1610613016</variable>
         <variable name="CREATE_REPORT_TEMPLATE" type="int" ns="ensight.objs.enums.CREATE_REPORT_TEMPLATE">1610612758</variable>
         <variable name="CT_BOX" type="int" ns="ensight.objs.enums.CT_BOX">10</variable>
         <variable name="CT_CONE" type="int" ns="ensight.objs.enums.CT_CONE">4</variable>
         <variable name="CT_CYLD" type="int" ns="ensight.objs.enums.CT_CYLD">2</variable>
@@ -57607,15 +57607,15 @@
         <variable name="CT_PART" type="int" ns="ensight.objs.enums.CT_PART">6</variable>
         <variable name="CT_PLNE" type="int" ns="ensight.objs.enums.CT_PLNE">1</variable>
         <variable name="CT_REVO" type="int" ns="ensight.objs.enums.CT_REVO">5</variable>
         <variable name="CT_RTZ" type="int" ns="ensight.objs.enums.CT_RTZ">11</variable>
         <variable name="CT_SPHR" type="int" ns="ensight.objs.enums.CT_SPHR">3</variable>
         <variable name="CT_SPLINE" type="int" ns="ensight.objs.enums.CT_SPLINE">12</variable>
         <variable name="CT_XYZ" type="int" ns="ensight.objs.enums.CT_XYZ">9</variable>
-        <variable name="CULLELEMENTS" type="int" ns="ensight.objs.enums.CULLELEMENTS">1610613165</variable>
+        <variable name="CULLELEMENTS" type="int" ns="ensight.objs.enums.CULLELEMENTS">1610613166</variable>
         <variable name="CULL_BACK_FACE" type="int" ns="ensight.objs.enums.CULL_BACK_FACE">0</variable>
         <variable name="CULL_FRONT_FACE" type="int" ns="ensight.objs.enums.CULL_FRONT_FACE">1</variable>
         <variable name="CULL_NO_FACE" type="int" ns="ensight.objs.enums.CULL_NO_FACE">2</variable>
         <variable name="CURRENT" type="int" ns="ensight.objs.enums.CURRENT">1610612759</variable>
         <variable name="CURRENTCASE" type="int" ns="ensight.objs.enums.CURRENTCASE">1610612824</variable>
         <variable name="CURRENTFRAME" type="int" ns="ensight.objs.enums.CURRENTFRAME">1610613048</variable>
         <variable name="CURRENTGUI" type="int" ns="ensight.objs.enums.CURRENTGUI">1610612878</variable>
@@ -57662,15 +57662,15 @@
         <variable name="CVF_ATTR_NO_MINIMUM" type="int" ns="ensight.objs.enums.CVF_ATTR_NO_MINIMUM">16</variable>
         <variable name="CVF_ATTR_OBJPTR" type="int" ns="ensight.objs.enums.CVF_ATTR_OBJPTR">13</variable>
         <variable name="CVF_ATTR_PSTRING" type="int" ns="ensight.objs.enums.CVF_ATTR_PSTRING">8</variable>
         <variable name="CVF_ATTR_PTR" type="int" ns="ensight.objs.enums.CVF_ATTR_PTR">9</variable>
         <variable name="CVF_ATTR_READONLY" type="int" ns="ensight.objs.enums.CVF_ATTR_READONLY">256</variable>
         <variable name="CVF_ATTR_SOBJPTR" type="int" ns="ensight.objs.enums.CVF_ATTR_SOBJPTR">12</variable>
         <variable name="CVF_ATTR_STRING" type="int" ns="ensight.objs.enums.CVF_ATTR_STRING">7</variable>
-        <variable name="CVF_ATTR_USERFLG_MASK" type="int" ns="ensight.objs.enums.CVF_ATTR_USERFLG_MASK">-65536</variable>
+        <variable name="CVF_ATTR_USERFLG_MASK" type="int" ns="ensight.objs.enums.CVF_ATTR_USERFLG_MASK">4294901760</variable>
         <variable name="CVF_ATTR_VARID" type="int" ns="ensight.objs.enums.CVF_ATTR_VARID">4</variable>
         <variable name="CVF_CP_UTF8" type="int" ns="ensight.objs.enums.CVF_CP_UTF8">65001</variable>
         <variable name="CVF_FONT_BOLD" type="int" ns="ensight.objs.enums.CVF_FONT_BOLD">2</variable>
         <variable name="CVF_FONT_DEMILIGHT" type="int" ns="ensight.objs.enums.CVF_FONT_DEMILIGHT">256</variable>
         <variable name="CVF_FONT_ITALIC" type="int" ns="ensight.objs.enums.CVF_FONT_ITALIC">4</variable>
         <variable name="CVF_FONT_LIGHT" type="int" ns="ensight.objs.enums.CVF_FONT_LIGHT">128</variable>
         <variable name="CVF_FONT_NARROW" type="int" ns="ensight.objs.enums.CVF_FONT_NARROW">32</variable>
@@ -57695,16 +57695,16 @@
         <variable name="CVF_JLC_RUSERNAME" type="int" ns="ensight.objs.enums.CVF_JLC_RUSERNAME">7006</variable>
         <variable name="CVF_JLC_TIMEOUT" type="int" ns="ensight.objs.enums.CVF_JLC_TIMEOUT">7010</variable>
         <variable name="CVF_LANG_UNKNOWN" type="int" ns="ensight.objs.enums.CVF_LANG_UNKNOWN">0</variable>
         <variable name="CVF_PALETTE_UNDEFINED_AS_ZERO_VALUE" type="int" ns="ensight.objs.enums.CVF_PALETTE_UNDEFINED_AS_ZERO_VALUE">30</variable>
         <variable name="CVF_PALETTE_UNDEFINED_BY_INVISIBLE" type="int" ns="ensight.objs.enums.CVF_PALETTE_UNDEFINED_BY_INVISIBLE">20</variable>
         <variable name="CVF_PALETTE_UNDEFINED_BY_PART_COLOR" type="int" ns="ensight.objs.enums.CVF_PALETTE_UNDEFINED_BY_PART_COLOR">10</variable>
         <variable name="CVF_PALETTE_UNDEFINED_BY_UNDEF_COLOR" type="int" ns="ensight.objs.enums.CVF_PALETTE_UNDEFINED_BY_UNDEF_COLOR">40</variable>
-        <variable name="CYLDAXISVECT" type="int" ns="ensight.objs.enums.CYLDAXISVECT">1610613268</variable>
-        <variable name="CYLDENDPOINT" type="int" ns="ensight.objs.enums.CYLDENDPOINT">1610613267</variable>
+        <variable name="CYLDAXISVECT" type="int" ns="ensight.objs.enums.CYLDAXISVECT">1610613267</variable>
+        <variable name="CYLDENDPOINT" type="int" ns="ensight.objs.enums.CYLDENDPOINT">1610613268</variable>
         <variable name="CYLDORIGIN" type="int" ns="ensight.objs.enums.CYLDORIGIN">1610613266</variable>
         <variable name="CYLDRADIUS" type="int" ns="ensight.objs.enums.CYLDRADIUS">1610613265</variable>
         <variable name="DATA_BIGENDIAN" type="int" ns="ensight.objs.enums.DATA_BIGENDIAN">0</variable>
         <variable name="DATA_LITTLEENDIAN" type="int" ns="ensight.objs.enums.DATA_LITTLEENDIAN">1</variable>
         <variable name="DATA_NATIVE" type="int" ns="ensight.objs.enums.DATA_NATIVE">2</variable>
         <variable name="DEFAULTANNOTS" type="int" ns="ensight.objs.enums.DEFAULTANNOTS">1610612826</variable>
         <variable name="DEFAULTPARTS" type="int" ns="ensight.objs.enums.DEFAULTPARTS">1610612825</variable>
@@ -57770,15 +57770,15 @@
         <variable name="ELE_FAILED_EQUAL" type="int" ns="ensight.objs.enums.ELE_FAILED_EQUAL">3</variable>
         <variable name="ELE_FAILED_GREATER" type="int" ns="ensight.objs.enums.ELE_FAILED_GREATER">1</variable>
         <variable name="ELE_FAILED_LESS" type="int" ns="ensight.objs.enums.ELE_FAILED_LESS">2</variable>
         <variable name="ELE_FAILED_LOGIC_AND" type="int" ns="ensight.objs.enums.ELE_FAILED_LOGIC_AND">1</variable>
         <variable name="ELE_FAILED_LOGIC_NONE" type="int" ns="ensight.objs.enums.ELE_FAILED_LOGIC_NONE">0</variable>
         <variable name="ELE_FAILED_LOGIC_OR" type="int" ns="ensight.objs.enums.ELE_FAILED_LOGIC_OR">2</variable>
         <variable name="ELE_FAILED_NOT_EQUAL" type="int" ns="ensight.objs.enums.ELE_FAILED_NOT_EQUAL">4</variable>
-        <variable name="ELTBLANKING" type="int" ns="ensight.objs.enums.ELTBLANKING">1610613166</variable>
+        <variable name="ELTBLANKING" type="int" ns="ensight.objs.enums.ELTBLANKING">1610613165</variable>
         <variable name="ELTDEFINEDBY" type="int" ns="ensight.objs.enums.ELTDEFINEDBY">1610613174</variable>
         <variable name="ELTFEATUREANGLE" type="int" ns="ensight.objs.enums.ELTFEATUREANGLE">1610613160</variable>
         <variable name="ELTFILTER1ACTIVE" type="int" ns="ensight.objs.enums.ELTFILTER1ACTIVE">1610613184</variable>
         <variable name="ELTFILTER1TESTOP" type="int" ns="ensight.objs.enums.ELTFILTER1TESTOP">1610613187</variable>
         <variable name="ELTFILTER1TESTVALUE" type="int" ns="ensight.objs.enums.ELTFILTER1TESTVALUE">1610613188</variable>
         <variable name="ELTFILTER1TESTVARCOMP" type="int" ns="ensight.objs.enums.ELTFILTER1TESTVARCOMP">1610613190</variable>
         <variable name="ELTFILTER1TESTVARIABLE" type="int" ns="ensight.objs.enums.ELTFILTER1TESTVARIABLE">1610613189</variable>
@@ -57958,32 +57958,32 @@
         <variable name="EPSILON" type="int" ns="ensight.objs.enums.EPSILON">1610613454</variable>
         <variable name="EQUATION" type="int" ns="ensight.objs.enums.EQUATION">1610613304</variable>
         <variable name="EXIST_CASE" type="int" ns="ensight.objs.enums.EXIST_CASE">1610612955</variable>
         <variable name="EXPRESSION" type="int" ns="ensight.objs.enums.EXPRESSION">1610612951</variable>
         <variable name="EXTENTS" type="int" ns="ensight.objs.enums.EXTENTS">1610613233</variable>
         <variable name="E_FORMAT" type="int" ns="ensight.objs.enums.E_FORMAT">1</variable>
         <variable name="FACEAREAFRACTION" type="int" ns="ensight.objs.enums.FACEAREAFRACTION">1610613450</variable>
-        <variable name="FACEXMAXGRID" type="int" ns="ensight.objs.enums.FACEXMAXGRID">1610613724</variable>
-        <variable name="FACEXMAXGRIDFILTER" type="int" ns="ensight.objs.enums.FACEXMAXGRIDFILTER">1610613728</variable>
-        <variable name="FACEXMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEXMAXSUBGRID">1610613727</variable>
+        <variable name="FACEXMAXGRID" type="int" ns="ensight.objs.enums.FACEXMAXGRID">1610613720</variable>
+        <variable name="FACEXMAXGRIDFILTER" type="int" ns="ensight.objs.enums.FACEXMAXGRIDFILTER">1610613722</variable>
+        <variable name="FACEXMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEXMAXSUBGRID">1610613721</variable>
         <variable name="FACEXMINGRID" type="int" ns="ensight.objs.enums.FACEXMINGRID">1610613711</variable>
-        <variable name="FACEXMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEXMINGRIDFILTER">1610613719</variable>
+        <variable name="FACEXMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEXMINGRIDFILTER">1610613713</variable>
         <variable name="FACEXMINSUBGRID" type="int" ns="ensight.objs.enums.FACEXMINSUBGRID">1610613712</variable>
-        <variable name="FACEYMAXGRID" type="int" ns="ensight.objs.enums.FACEYMAXGRID">1610613722</variable>
+        <variable name="FACEYMAXGRID" type="int" ns="ensight.objs.enums.FACEYMAXGRID">1610613723</variable>
         <variable name="FACEYMAXGRIDFILTER" type="int" ns="ensight.objs.enums.FACEYMAXGRIDFILTER">1610613725</variable>
-        <variable name="FACEYMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEYMAXSUBGRID">1610613723</variable>
-        <variable name="FACEYMINGRID" type="int" ns="ensight.objs.enums.FACEYMINGRID">1610613713</variable>
-        <variable name="FACEYMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEYMINGRIDFILTER">1610613715</variable>
-        <variable name="FACEYMINSUBGRID" type="int" ns="ensight.objs.enums.FACEYMINSUBGRID">1610613714</variable>
-        <variable name="FACEZMAXGRID" type="int" ns="ensight.objs.enums.FACEZMAXGRID">1610613720</variable>
-        <variable name="FACEZMAXGRIDFILTER" type="int" ns="ensight.objs.enums.FACEZMAXGRIDFILTER">1610613721</variable>
-        <variable name="FACEZMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEZMAXSUBGRID">1610613726</variable>
-        <variable name="FACEZMINGRID" type="int" ns="ensight.objs.enums.FACEZMINGRID">1610613716</variable>
-        <variable name="FACEZMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEZMINGRIDFILTER">1610613718</variable>
-        <variable name="FACEZMINSUBGRID" type="int" ns="ensight.objs.enums.FACEZMINSUBGRID">1610613717</variable>
+        <variable name="FACEYMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEYMAXSUBGRID">1610613724</variable>
+        <variable name="FACEYMINGRID" type="int" ns="ensight.objs.enums.FACEYMINGRID">1610613714</variable>
+        <variable name="FACEYMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEYMINGRIDFILTER">1610613716</variable>
+        <variable name="FACEYMINSUBGRID" type="int" ns="ensight.objs.enums.FACEYMINSUBGRID">1610613715</variable>
+        <variable name="FACEZMAXGRID" type="int" ns="ensight.objs.enums.FACEZMAXGRID">1610613726</variable>
+        <variable name="FACEZMAXGRIDFILTER" type="int" ns="ensight.objs.enums.FACEZMAXGRIDFILTER">1610613728</variable>
+        <variable name="FACEZMAXSUBGRID" type="int" ns="ensight.objs.enums.FACEZMAXSUBGRID">1610613727</variable>
+        <variable name="FACEZMINGRID" type="int" ns="ensight.objs.enums.FACEZMINGRID">1610613717</variable>
+        <variable name="FACEZMINGRIDFILTER" type="int" ns="ensight.objs.enums.FACEZMINGRIDFILTER">1610613719</variable>
+        <variable name="FACEZMINSUBGRID" type="int" ns="ensight.objs.enums.FACEZMINSUBGRID">1610613718</variable>
         <variable name="FALSE" type="int" ns="ensight.objs.enums.FALSE">0</variable>
         <variable name="FASTDISPLAY" type="int" ns="ensight.objs.enums.FASTDISPLAY">1610612856</variable>
         <variable name="FEATURE_ANGLE" type="int" ns="ensight.objs.enums.FEATURE_ANGLE">2</variable>
         <variable name="FEATURE_FULL" type="int" ns="ensight.objs.enums.FEATURE_FULL">6</variable>
         <variable name="FEA_VAR" type="int" ns="ensight.objs.enums.FEA_VAR">1677721619</variable>
         <variable name="FILENAME" type="int" ns="ensight.objs.enums.FILENAME">1610613044</variable>
         <variable name="FILL" type="int" ns="ensight.objs.enums.FILL">1610613573</variable>
@@ -58238,22 +58238,22 @@
         <variable name="MASSEDBALLISTICCOEF" type="int" ns="ensight.objs.enums.MASSEDBALLISTICCOEF">1610613371</variable>
         <variable name="MASSEDBUOYANCY" type="int" ns="ensight.objs.enums.MASSEDBUOYANCY">1610613378</variable>
         <variable name="MASSEDCOEFFRICTION" type="int" ns="ensight.objs.enums.MASSEDCOEFFRICTION">1610613383</variable>
         <variable name="MASSEDCOEFRESTITUTION" type="int" ns="ensight.objs.enums.MASSEDCOEFRESTITUTION">1610613382</variable>
         <variable name="MASSEDDRAG" type="int" ns="ensight.objs.enums.MASSEDDRAG">1610613363</variable>
         <variable name="MASSEDDRAGCOEFFICIENT" type="int" ns="ensight.objs.enums.MASSEDDRAGCOEFFICIENT">1610613366</variable>
         <variable name="MASSEDDRAGCOEFFICIENTVAL" type="int" ns="ensight.objs.enums.MASSEDDRAGCOEFFICIENTVAL">1610613367</variable>
-        <variable name="MASSEDFLUIDDENSITY" type="int" ns="ensight.objs.enums.MASSEDFLUIDDENSITY">1610613373</variable>
+        <variable name="MASSEDFLUIDDENSITY" type="int" ns="ensight.objs.enums.MASSEDFLUIDDENSITY">1610613374</variable>
         <variable name="MASSEDFLUIDDENSITYVAL" type="int" ns="ensight.objs.enums.MASSEDFLUIDDENSITYVAL">1610613375</variable>
         <variable name="MASSEDFLUIDVISCOSITY" type="int" ns="ensight.objs.enums.MASSEDFLUIDVISCOSITY">1610613368</variable>
         <variable name="MASSEDFLUIDVISCOSITYVAL" type="int" ns="ensight.objs.enums.MASSEDFLUIDVISCOSITYVAL">1610613369</variable>
         <variable name="MASSEDGRAVITY" type="int" ns="ensight.objs.enums.MASSEDGRAVITY">1610613376</variable>
         <variable name="MASSEDGRAVITYVECTOR" type="int" ns="ensight.objs.enums.MASSEDGRAVITYVECTOR">1610613377</variable>
         <variable name="MASSEDINITIALUSEFLUID" type="int" ns="ensight.objs.enums.MASSEDINITIALUSEFLUID">1610613372</variable>
-        <variable name="MASSEDINITIALVELOCITY" type="int" ns="ensight.objs.enums.MASSEDINITIALVELOCITY">1610613374</variable>
+        <variable name="MASSEDINITIALVELOCITY" type="int" ns="ensight.objs.enums.MASSEDINITIALVELOCITY">1610613373</variable>
         <variable name="MASSEDPARTICLEDENSITY" type="int" ns="ensight.objs.enums.MASSEDPARTICLEDENSITY">1610613365</variable>
         <variable name="MASSEDPARTICLEDIAMETER" type="int" ns="ensight.objs.enums.MASSEDPARTICLEDIAMETER">1610613364</variable>
         <variable name="MASSEDPARTICLES" type="int" ns="ensight.objs.enums.MASSEDPARTICLES">1610613362</variable>
         <variable name="MASSEDPRESSURE" type="int" ns="ensight.objs.enums.MASSEDPRESSURE">1610613379</variable>
         <variable name="MASSEDPRESSUREGRADIENT" type="int" ns="ensight.objs.enums.MASSEDPRESSUREGRADIENT">1610613380</variable>
         <variable name="MASSEDREBOUND" type="int" ns="ensight.objs.enums.MASSEDREBOUND">1610613381</variable>
         <variable name="MASSEDREBOUNDFRACTION" type="int" ns="ensight.objs.enums.MASSEDREBOUNDFRACTION">1610613384</variable>
@@ -58377,32 +58377,32 @@
         <variable name="NUMOFSLICES" type="int" ns="ensight.objs.enums.NUMOFSLICES">1610613441</variable>
         <variable name="NUMPOINTS" type="int" ns="ensight.objs.enums.NUMPOINTS">1610613037</variable>
         <variable name="OBJECTFOCUS" type="int" ns="ensight.objs.enums.OBJECTFOCUS">1610612944</variable>
         <variable name="OBJECT_API_JOURNAL" type="int" ns="ensight.objs.enums.OBJECT_API_JOURNAL">1610612870</variable>
         <variable name="OBJECT_DTOR" type="int" ns="ensight.objs.enums.OBJECT_DTOR">1610612918</variable>
         <variable name="OFFSET" type="int" ns="ensight.objs.enums.OFFSET">1610612810</variable>
         <variable name="OFFSETFROMPART" type="int" ns="ensight.objs.enums.OFFSETFROMPART">1610613408</variable>
-        <variable name="OFFSETSCALE" type="int" ns="ensight.objs.enums.OFFSETSCALE">1610613409</variable>
-        <variable name="OFFSETVECTOR" type="int" ns="ensight.objs.enums.OFFSETVECTOR">1610613410</variable>
+        <variable name="OFFSETSCALE" type="int" ns="ensight.objs.enums.OFFSETSCALE">1610613410</variable>
+        <variable name="OFFSETVECTOR" type="int" ns="ensight.objs.enums.OFFSETVECTOR">1610613409</variable>
         <variable name="ONE" type="int" ns="ensight.objs.enums.ONE">1</variable>
         <variable name="OPAQUENESS" type="int" ns="ensight.objs.enums.OPAQUENESS">1610613102</variable>
         <variable name="OPERATION" type="int" ns="ensight.objs.enums.OPERATION">1610613817</variable>
         <variable name="OPERATIONFACTOR1" type="int" ns="ensight.objs.enums.OPERATIONFACTOR1">1610613813</variable>
         <variable name="OPERATIONFACTOR2" type="int" ns="ensight.objs.enums.OPERATIONFACTOR2">1610613814</variable>
         <variable name="OPERATIONQUERY1BYNAME" type="int" ns="ensight.objs.enums.OPERATIONQUERY1BYNAME">1610613815</variable>
         <variable name="OPERATIONQUERY2BYNAME" type="int" ns="ensight.objs.enums.OPERATIONQUERY2BYNAME">1610613816</variable>
         <variable name="OPTION_NONE" type="int" ns="ensight.objs.enums.OPTION_NONE">-1</variable>
         <variable name="ORDER" type="int" ns="ensight.objs.enums.ORDER">1610612946</variable>
         <variable name="ORIENTATION" type="int" ns="ensight.objs.enums.ORIENTATION">1610613522</variable>
         <variable name="ORIGIN" type="int" ns="ensight.objs.enums.ORIGIN">1610613313</variable>
         <variable name="ORIGIN1" type="int" ns="ensight.objs.enums.ORIGIN1">1610613515</variable>
         <variable name="ORIGIN2" type="int" ns="ensight.objs.enums.ORIGIN2">1610613516</variable>
         <variable name="ORIGINBY" type="int" ns="ensight.objs.enums.ORIGINBY">1610613502</variable>
-        <variable name="ORIGINBY1" type="int" ns="ensight.objs.enums.ORIGINBY1">1610613518</variable>
-        <variable name="ORIGINBY2" type="int" ns="ensight.objs.enums.ORIGINBY2">1610613517</variable>
+        <variable name="ORIGINBY1" type="int" ns="ensight.objs.enums.ORIGINBY1">1610613517</variable>
+        <variable name="ORIGINBY2" type="int" ns="ensight.objs.enums.ORIGINBY2">1610613518</variable>
         <variable name="ORIGINBYPARTCENTROID" type="int" ns="ensight.objs.enums.ORIGINBYPARTCENTROID">1610613444</variable>
         <variable name="ORIGINFRAME" type="int" ns="ensight.objs.enums.ORIGINFRAME">1610613505</variable>
         <variable name="ORIGINX" type="int" ns="ensight.objs.enums.ORIGINX">1610613603</variable>
         <variable name="ORIGINY" type="int" ns="ensight.objs.enums.ORIGINY">1610613604</variable>
         <variable name="ORIGIN_NODE_ID" type="int" ns="ensight.objs.enums.ORIGIN_NODE_ID">1610613086</variable>
         <variable name="ORIGIN_OPTION" type="int" ns="ensight.objs.enums.ORIGIN_OPTION">1610613084</variable>
         <variable name="ORIGIN_PART_ID" type="int" ns="ensight.objs.enums.ORIGIN_PART_ID">1610613085</variable>
@@ -58958,15 +58958,15 @@
         <variable name="USE_LOGO" type="int" ns="ensight.objs.enums.USE_LOGO">1610612755</variable>
         <variable name="UUID" type="int" ns="ensight.objs.enums.UUID">1610612747</variable>
         <variable name="VALUE" type="int" ns="ensight.objs.enums.VALUE">1610613312</variable>
         <variable name="VALUEDECIMALPLACES" type="int" ns="ensight.objs.enums.VALUEDECIMALPLACES">1610613571</variable>
         <variable name="VALUEFORMAT" type="int" ns="ensight.objs.enums.VALUEFORMAT">1610613570</variable>
         <variable name="VALUEIJK" type="int" ns="ensight.objs.enums.VALUEIJK">1610613236</variable>
         <variable name="VALUELOCATION" type="int" ns="ensight.objs.enums.VALUELOCATION">1610613569</variable>
-        <variable name="VALUERGB" type="int" ns="ensight.objs.enums.VALUERGB">1610613564</variable>
+        <variable name="VALUERGB" type="int" ns="ensight.objs.enums.VALUERGB">1610613565</variable>
         <variable name="VALUERTZ" type="int" ns="ensight.objs.enums.VALUERTZ">1610613245</variable>
         <variable name="VALUESIZE" type="int" ns="ensight.objs.enums.VALUESIZE">1610613566</variable>
         <variable name="VALUESPLINE" type="int" ns="ensight.objs.enums.VALUESPLINE">1610613247</variable>
         <variable name="VALUEXYZ" type="int" ns="ensight.objs.enums.VALUEXYZ">1610613242</variable>
         <variable name="VARCOMP" type="int" ns="ensight.objs.enums.VARCOMP">1610612993</variable>
         <variable name="VARIABLE" type="int" ns="ensight.objs.enums.VARIABLE">1610612988</variable>
         <variable name="VARIABLE1" type="int" ns="ensight.objs.enums.VARIABLE1">1610613796</variable>
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/PKG-INFO` & `ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-pyensight
-Version: 0.2.2
-Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:16:15 on 05 July 2023
+Version: 0.2.dev0
+Summary: Autogenerated python gRPC interface package for ansys-api-pyensight, built on 09:54:22 on 03 July 2023
 Home-page: https://github.com/ansys/ansys-api-pyensight
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ansys-api-pyensight-0.2.2/src/ansys_api_pyensight.egg-info/SOURCES.txt` & `ansys-api-pyensight-0.2.dev0/src/ansys_api_pyensight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

