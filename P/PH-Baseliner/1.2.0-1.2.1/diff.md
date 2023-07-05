# Comparing `tmp/PH-Baseliner-1.2.0.tar.gz` & `tmp/PH-Baseliner-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-Baseliner-1.2.0.tar", last modified: Tue Jul  4 19:15:10 2023, max compression
+gzip compressed data, was "dist/PH-Baseliner-1.2.1.tar", last modified: Wed Jul  5 20:28:52 2023, max compression
```

## Comparing `PH-Baseliner-1.2.0.tar` & `PH-Baseliner-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1589 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/
--rw-r--r--   0 runner     (501) staff       (20)    13031 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/ECCCNYS_2020.json
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2071 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/lighting_space_types.py
--rw-r--r--   0 runner     (501) staff       (20)    17467 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/model.py
--rw-r--r--   0 runner     (501) staff       (20)     1406 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/options.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4685 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1484 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/components.py
--rw-r--r--   0 runner     (501) staff       (20)     1725 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     3285 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/u_values.py
--rw-r--r--   0 runner     (501) staff       (20)     5410 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/windows.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2526 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     2583 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/constructions.py
--rw-r--r--   0 runner     (501) staff       (20)      488 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     6056 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/windows.py
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      839 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/
+-rw-r--r--   0 runner     (501) staff       (20)    13031 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/ECCCNYS_2020.json
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2071 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/lighting_space_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    17467 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/options.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4685 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     1725 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     3285 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)     5410 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/windows.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2526 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     2583 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/constructions.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     6888 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/windows.py
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      839 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/setup.py
```

### Comparing `PH-Baseliner-1.2.0/.github/workflows/ci.yaml` & `PH-Baseliner-1.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/LICENSE` & `PH-Baseliner-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/PH_Baseliner.egg-info/PKG-INFO` & `PH-Baseliner-1.2.1/PH_Baseliner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.2.0/PH_Baseliner.egg-info/SOURCES.txt` & `PH-Baseliner-1.2.1/PH_Baseliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/PKG-INFO` & `PH-Baseliner-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.2.0/README.md` & `PH-Baseliner-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/codes/ECCCNYS_2020.json` & `PH-Baseliner-1.2.1/ph_baseliner/codes/ECCCNYS_2020.json`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/codes/lighting_space_types.py` & `PH-Baseliner-1.2.1/ph_baseliner/codes/lighting_space_types.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/codes/model.py` & `PH-Baseliner-1.2.1/ph_baseliner/codes/model.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/codes/options.py` & `PH-Baseliner-1.2.1/ph_baseliner/codes/options.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phpp/areas.py` & `PH-Baseliner-1.2.1/ph_baseliner/phpp/areas.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phpp/components.py` & `PH-Baseliner-1.2.1/ph_baseliner/phpp/components.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phpp/lighting.py` & `PH-Baseliner-1.2.1/ph_baseliner/phpp/lighting.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phpp/u_values.py` & `PH-Baseliner-1.2.1/ph_baseliner/phpp/u_values.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phpp/windows.py` & `PH-Baseliner-1.2.1/ph_baseliner/phpp/windows.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phx/areas.py` & `PH-Baseliner-1.2.1/ph_baseliner/phx/areas.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phx/constructions.py` & `PH-Baseliner-1.2.1/ph_baseliner/phx/constructions.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.0/ph_baseliner/phx/windows.py` & `PH-Baseliner-1.2.1/ph_baseliner/phx/windows.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 3.7 -*-
 
 """Functions to set baseline PHX Model windows."""
 
-from typing import Callable
+from typing import Callable, Dict
 
 from PHX.model.project import PhxProject
+from PHX.model.components import PhxComponentAperture
 from PHX.model.constructions import PhxConstructionWindow
 
 from ph_baseliner.codes.model import BaselineCode
 from ph_baseliner.codes.options import ClimateZones, PF_Groups, Use_Groups
 
 
 def get_baseline_window_u_value(
@@ -40,26 +41,40 @@
     _use_group: Use_Groups,
     _output: Callable = print,
 ) -> PhxProject:
     # -- Get the baseline values for U-Value and SHGC
     u_value = get_baseline_window_u_value(_baseline_code, _climate_zone, _use_group)
     shgc = get_baseline_window_SHGC(_baseline_code, _climate_zone, _pf_group)
 
-    # -- Create the new baseline window construction
-    baseline_phx_window = PhxConstructionWindow.from_total_u_value(
-        u_value, shgc, "BASELINE: WINDOW"
-    )
+    # -- Collect all the unique window types in the PHX project
+    unique_window_types: Dict[str, PhxComponentAperture] = {}
+    for variant in _phx_project.variants:
+        for aperture_component in variant.building.aperture_components:
+            unique_window_types[aperture_component.unique_key] = aperture_component
 
-    # -- Add the new baseline window construction to the PHX project
-    _phx_project.add_new_window_type(baseline_phx_window)
+    # -- Create the new baseline window construction for each
+    for i, unique_window_type_key in enumerate(unique_window_types.keys(), start=1):
+        window_type = unique_window_types[unique_window_type_key]
+        baseline_phx_window = PhxConstructionWindow.from_total_u_value(
+            u_value, shgc, f"BASELINE: WINDOW {i :03}"
+        )
+        baseline_phx_window.id_num_shade = window_type.shade_type_id_num
+
+        # -- Add the new baseline window construction to the PHX project
+        _phx_project.add_new_window_type(
+            baseline_phx_window, _key=unique_window_type_key
+        )
 
     # -- Set the baseline window construction in the PHX project
     for variant in _phx_project.variants:
         for aperture_component in variant.building.aperture_components:
-            aperture_component.set_window_type(baseline_phx_window)
+            baseline_phx_window_type = _phx_project.get_window_type(
+                aperture_component.unique_key
+            )
+            aperture_component.set_window_type(baseline_phx_window_type)
 
     return _phx_project
 
 
 def set_baseline_window_area(
     _phx_project: PhxProject, _baseline_code: BaselineCode, _output: Callable = print
 ) -> PhxProject:
```

### Comparing `PH-Baseliner-1.2.0/setup.cfg` & `PH-Baseliner-1.2.1/setup.cfg`

 * *Files identical despite different names*

