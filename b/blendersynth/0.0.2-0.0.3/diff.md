# Comparing `tmp/blendersynth-0.0.2.tar.gz` & `tmp/blendersynth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendersynth-0.0.2.tar", last modified: Sun Jun 18 08:47:42 2023, max compression
+gzip compressed data, was "blendersynth-0.0.3.tar", last modified: Wed Jul  5 10:09:56 2023, max compression
```

## Comparing `blendersynth-0.0.2.tar` & `blendersynth-0.0.3.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.862711 blendersynth-0.0.2/
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.853865 blendersynth-0.0.2/BlenderSynth.egg-info/
--rw-r--r--   0 ollie      (501) staff       (20)     2003 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1476 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/SOURCES.txt
--rw-r--r--   0 ollie      (501) staff       (20)        1 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/dependency_links.txt
--rw-r--r--   0 ollie      (501) staff       (20)       13 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/top_level.txt
--rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.2/LICENSE
--rw-r--r--   0 ollie      (501) staff       (20)     2003 2023-06-18 08:47:42.862484 blendersynth-0.0.2/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1728 2023-06-15 17:26:03.000000 blendersynth-0.0.2/README.md
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.854310 blendersynth-0.0.2/blendersynth/
--rw-r--r--   0 ollie      (501) staff       (20)     1365 2023-06-15 17:26:03.000000 blendersynth-0.0.2/blendersynth/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.855229 blendersynth-0.0.2/blendersynth/annotations/
--rw-r--r--   0 ollie      (501) staff       (20)       30 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     1571 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/bbox.py
--rw-r--r--   0 ollie      (501) staff       (20)     1185 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/utils.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.857219 blendersynth-0.0.2/blendersynth/blender/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/blender/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     8420 2023-06-14 19:52:56.000000 blendersynth-0.0.2/blendersynth/blender/aov.py
--rw-r--r--   0 ollie      (501) staff       (20)     1769 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/camera.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.858461 blendersynth-0.0.2/blendersynth/blender/compositor/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/blender/compositor/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     7898 2023-06-14 19:52:56.000000 blendersynth-0.0.2/blendersynth/blender/compositor/compositor.py
--rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/mask_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)      876 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/node_group.py
--rw-r--r--   0 ollie      (501) staff       (20)     5485 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/shape_overlays.py
--rw-r--r--   0 ollie      (501) staff       (20)     1256 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/light.py
--rw-r--r--   0 ollie      (501) staff       (20)    12158 2023-06-18 08:45:26.000000 blendersynth-0.0.2/blendersynth/blender/mesh.py
--rw-r--r--   0 ollie      (501) staff       (20)      503 2023-06-09 15:21:26.000000 blendersynth-0.0.2/blendersynth/blender/render.py
--rw-r--r--   0 ollie      (501) staff       (20)     1475 2023-06-16 13:06:27.000000 blendersynth-0.0.2/blendersynth/blender/utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     1755 2023-06-16 17:58:30.000000 blendersynth-0.0.2/blendersynth/blender/world.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.859417 blendersynth-0.0.2/blendersynth/file/
--rw-r--r--   0 ollie      (501) staff       (20)       39 2023-06-12 08:58:09.000000 blendersynth-0.0.2/blendersynth/file/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      839 2023-06-14 20:54:24.000000 blendersynth-0.0.2/blendersynth/file/dataset_inputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      159 2023-06-09 15:47:06.000000 blendersynth-0.0.2/blendersynth/file/dataset_outputs.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.860494 blendersynth-0.0.2/blendersynth/run/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/run/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.2/blendersynth/run/blender_interface.py
--rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.2/blendersynth/run/blender_threading.py
--rw-r--r--   0 ollie      (501) staff       (20)     2931 2023-06-14 20:49:44.000000 blendersynth-0.0.2/blendersynth/run/run.py
--rw-r--r--   0 ollie      (501) staff       (20)      628 2023-06-14 19:34:31.000000 blendersynth-0.0.2/blendersynth/run_this_script.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.860878 blendersynth-0.0.2/blendersynth/utils/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/utils/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.861957 blendersynth-0.0.2/blendersynth/utils/blender_setup/
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     3885 2023-06-14 21:00:10.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_locator.py
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_python_path.py
--rw-r--r--   0 ollie      (501) staff       (20)     2741 2023-06-15 17:26:03.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/check_blender_install.py
--rw-r--r--   0 ollie      (501) staff       (20)     3359 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/utils/node_arranger.py
--rw-r--r--   0 ollie      (501) staff       (20)      392 2023-06-18 08:47:32.000000 blendersynth-0.0.2/pyproject.toml
--rw-r--r--   0 ollie      (501) staff       (20)       38 2023-06-18 08:47:42.862777 blendersynth-0.0.2/setup.cfg
--rw-r--r--   0 ollie      (501) staff       (20)      173 2023-06-18 08:47:32.000000 blendersynth-0.0.2/setup.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.168607 blendersynth-0.0.3/
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.158096 blendersynth-0.0.3/BlenderSynth.egg-info/
+-rw-r--r--   0 ollie      (501) staff       (20)     1907 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1654 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/SOURCES.txt
+-rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/dependency_links.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/top_level.txt
+-rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.3/LICENSE
+-rw-r--r--   0 ollie      (501) staff       (20)     1907 2023-07-05 10:09:56.168439 blendersynth-0.0.3/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1632 2023-07-03 17:47:18.000000 blendersynth-0.0.3/README.md
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.158520 blendersynth-0.0.3/blendersynth/
+-rw-r--r--   0 ollie      (501) staff       (20)     1458 2023-07-03 17:09:00.000000 blendersynth-0.0.3/blendersynth/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.159825 blendersynth-0.0.3/blendersynth/annotations/
+-rw-r--r--   0 ollie      (501) staff       (20)       87 2023-06-27 20:17:42.000000 blendersynth-0.0.3/blendersynth/annotations/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1979 2023-06-27 20:17:42.000000 blendersynth-0.0.3/blendersynth/annotations/bbox.py
+-rw-r--r--   0 ollie      (501) staff       (20)      272 2023-06-27 20:05:19.000000 blendersynth-0.0.3/blendersynth/annotations/keypoints.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1185 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/annotations/utils.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.162162 blendersynth-0.0.3/blendersynth/blender/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/blender/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     8420 2023-06-14 19:52:56.000000 blendersynth-0.0.3/blendersynth/blender/aov.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4193 2023-07-05 08:58:47.000000 blendersynth-0.0.3/blendersynth/blender/camera.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.163713 blendersynth-0.0.3/blendersynth/blender/compositor/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/blender/compositor/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     9543 2023-07-03 17:32:33.000000 blendersynth-0.0.3/blendersynth/blender/compositor/compositor.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3677 2023-06-27 20:31:49.000000 blendersynth-0.0.3/blendersynth/blender/compositor/image_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/blender/compositor/mask_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)      887 2023-06-27 21:00:21.000000 blendersynth-0.0.3/blendersynth/blender/compositor/node_group.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-06-27 21:00:00.000000 blendersynth-0.0.3/blendersynth/blender/compositor/visuals.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1218 2023-07-05 08:49:09.000000 blendersynth-0.0.3/blendersynth/blender/curve.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1256 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/blender/light.py
+-rw-r--r--   0 ollie      (501) staff       (20)    12586 2023-07-03 17:02:53.000000 blendersynth-0.0.3/blendersynth/blender/mesh.py
+-rw-r--r--   0 ollie      (501) staff       (20)      700 2023-07-03 17:45:30.000000 blendersynth-0.0.3/blendersynth/blender/render.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1940 2023-06-27 20:08:32.000000 blendersynth-0.0.3/blendersynth/blender/utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1755 2023-06-16 17:58:30.000000 blendersynth-0.0.3/blendersynth/blender/world.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.165524 blendersynth-0.0.3/blendersynth/file/
+-rw-r--r--   0 ollie      (501) staff       (20)       84 2023-07-05 09:14:27.000000 blendersynth-0.0.3/blendersynth/file/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      839 2023-06-14 20:54:24.000000 blendersynth-0.0.3/blendersynth/file/dataset_inputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      159 2023-06-09 15:47:06.000000 blendersynth-0.0.3/blendersynth/file/dataset_outputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2929 2023-07-05 10:03:41.000000 blendersynth-0.0.3/blendersynth/file/frames_to_video.py
+-rw-r--r--   0 ollie      (501) staff       (20)      412 2023-06-27 20:38:09.000000 blendersynth-0.0.3/blendersynth/file/tempfiles.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.166608 blendersynth-0.0.3/blendersynth/run/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/run/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.3/blendersynth/run/blender_interface.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.3/blendersynth/run/blender_threading.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3002 2023-06-27 21:08:18.000000 blendersynth-0.0.3/blendersynth/run/run.py
+-rw-r--r--   0 ollie      (501) staff       (20)      722 2023-07-05 10:01:27.000000 blendersynth-0.0.3/blendersynth/run_this_script.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.166880 blendersynth-0.0.3/blendersynth/utils/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/utils/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.167894 blendersynth-0.0.3/blendersynth/utils/blender_setup/
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3885 2023-06-14 21:00:10.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_locator.py
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_python_path.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2744 2023-07-05 09:07:26.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/check_blender_install.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3359 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/utils/node_arranger.py
+-rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-05 10:09:32.000000 blendersynth-0.0.3/pyproject.toml
+-rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-05 10:09:56.168668 blendersynth-0.0.3/setup.cfg
+-rw-r--r--   0 ollie      (501) staff       (20)      173 2023-07-05 10:09:32.000000 blendersynth-0.0.3/setup.py
```

### Comparing `blendersynth-0.0.2/BlenderSynth.egg-info/PKG-INFO` & `blendersynth-0.0.3/BlenderSynth.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.2
+Version: 0.0.3
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -40,25 +40,24 @@
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
 python setup.py install
 python -c "import blendersynth" --local
 ```
 
-## Quickstart
+## Examples
 
-For a quick overview of creating a render: `examples/quickstart.py`
+[See here](examples) for usage examples.
 
-For an overview of creating a dataset: `examples/dataset_creation`
+Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
-Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
 If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
```

### Comparing `blendersynth-0.0.2/BlenderSynth.egg-info/SOURCES.txt` & `blendersynth-0.0.3/BlenderSynth.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,36 @@
 blendersynth/run_this_script.py
 blendersynth.egg-info/PKG-INFO
 blendersynth.egg-info/SOURCES.txt
 blendersynth.egg-info/dependency_links.txt
 blendersynth.egg-info/top_level.txt
 blendersynth/annotations/__init__.py
 blendersynth/annotations/bbox.py
+blendersynth/annotations/keypoints.py
 blendersynth/annotations/utils.py
 blendersynth/blender/__init__.py
 blendersynth/blender/aov.py
 blendersynth/blender/camera.py
+blendersynth/blender/curve.py
 blendersynth/blender/light.py
 blendersynth/blender/mesh.py
 blendersynth/blender/render.py
 blendersynth/blender/utils.py
 blendersynth/blender/world.py
 blendersynth/blender/compositor/__init__.py
 blendersynth/blender/compositor/compositor.py
+blendersynth/blender/compositor/image_overlay.py
 blendersynth/blender/compositor/mask_overlay.py
 blendersynth/blender/compositor/node_group.py
-blendersynth/blender/compositor/shape_overlays.py
+blendersynth/blender/compositor/visuals.py
 blendersynth/file/__init__.py
 blendersynth/file/dataset_inputs.py
 blendersynth/file/dataset_outputs.py
+blendersynth/file/frames_to_video.py
+blendersynth/file/tempfiles.py
 blendersynth/run/__init__.py
 blendersynth/run/blender_interface.py
 blendersynth/run/blender_threading.py
 blendersynth/run/run.py
 blendersynth/utils/__init__.py
 blendersynth/utils/node_arranger.py
 blendersynth/utils/blender_setup/__init__.py
```

### Comparing `blendersynth-0.0.2/LICENSE` & `blendersynth-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/PKG-INFO` & `blendersynth-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.2
+Version: 0.0.3
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -40,25 +40,24 @@
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
 python setup.py install
 python -c "import blendersynth" --local
 ```
 
-## Quickstart
+## Examples
 
-For a quick overview of creating a render: `examples/quickstart.py`
+[See here](examples) for usage examples.
 
-For an overview of creating a dataset: `examples/dataset_creation`
+Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
-Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
 If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
```

### Comparing `blendersynth-0.0.2/README.md` & `blendersynth-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -31,25 +31,24 @@
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
 python setup.py install
 python -c "import blendersynth" --local
 ```
 
-## Quickstart
+## Examples
 
-For a quick overview of creating a render: `examples/quickstart.py`
+[See here](examples) for usage examples.
 
-For an overview of creating a dataset: `examples/dataset_creation`
+Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
-Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
 If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
```

### Comparing `blendersynth-0.0.2/blendersynth/__init__.py` & `blendersynth-0.0.3/blendersynth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 import sys
 from .utils.blender_setup.blender_locator import get_blender_path
 
 if get_blender_path() == sys.argv[0]:  # if blender is running this script
 	import bpy
 	from bpy import *
 	from .blender.mesh import Mesh
+	from .blender.curve import Curve
 	from .blender import render
 	from .blender.compositor.compositor import Compositor
 	from .blender import aov
 	from .file.dataset_inputs import INPUTS
 	from . import file
 	from .run.blender_interface import log_event
 	from .blender.world import world
 	from .blender.light import Light
 	from .blender.camera import Camera
 	from . import annotations
+	from .file.tempfiles import cleanup_temp_files as cleanup
 
 	# set render engine to cycles
 	render.set_engine('CYCLES')
 
 	# common aliases
 	load_blend = bpy.ops.wm.open_mainfile
```

### Comparing `blendersynth-0.0.2/blendersynth/annotations/bbox.py` & `blendersynth-0.0.3/blendersynth/annotations/bbox.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import bpy
 from .utils import project_points
 import mathutils
 import numpy as np
 from ..blender.mesh import Mesh
+from typing import List
 
 BBOX_FMTS = ['x1y1x2y2', 'xywh']
 
 def bounding_box(object: Mesh, camera: bpy.types.Camera = None,
 				 scene:bpy.types.Scene=None,
 				 return_fmt='x1y1x2y2', normalized=False, invert_y=True):
 	"""Get the bounding box of an object in camera space.
@@ -42,7 +43,15 @@
 		return xmin, ymin, xmax, ymax
 
 	elif return_fmt == 'xywh':
 		return xmin, ymin, xmax - xmin, ymax - ymin
 
 	else:
 		raise ValueError(f'Invalid return_fmt: {return_fmt}. Must be one of {BBOX_FMTS}')
+
+def bounding_boxes(objects: List[Mesh], camera: bpy.types.Camera = None,
+				 scene:bpy.types.Scene=None,
+				 return_fmt='x1y1x2y2', normalized=False, invert_y=True):
+	"""Get the bounding boxes of multiple objects in image space."""
+
+	return [bounding_box(obj, camera=camera, scene=scene, return_fmt=return_fmt,
+						   normalized=normalized, invert_y=invert_y) for obj in objects]
```

### Comparing `blendersynth-0.0.2/blendersynth/annotations/utils.py` & `blendersynth-0.0.3/blendersynth/annotations/utils.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/blender/aov.py` & `blendersynth-0.0.3/blendersynth/blender/aov.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/blender/compositor/compositor.py` & `blendersynth-0.0.3/blendersynth/blender/compositor/compositor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import bpy
+import numpy as np
 from ..utils import get_node_by_name
 import os
 import shutil
-from ..render import render
+from ..render import render, render_depth
 from .node_group import CompositorNodeGroup
 from ..aov import AOV
 from ..mesh import Mesh
 from .mask_overlay import MaskOverlay
-from .shape_overlays import BBoxOverlays
+from .visuals import DepthVis
+from .image_overlay import KeypointsOverlay, BoundingBoxOverlay
+
+
 from typing import Union, List
 from ...utils.node_arranger import tidy_tree
 
 # Mapping of file formats to extensions
 format_to_extension = {
 	'BMP': '.bmp',
 	'IRIS': '.rgb',
@@ -97,37 +101,68 @@
 			self.node_tree.links.new(ip_node, cng.input('Image'))
 			self.node_tree.links.new(self.render_layers_node.outputs['IndexOB'], cng.input('IndexOB'))
 			self.mask_nodes[index] = cng
 
 		self.tidy_tree()
 		return self.mask_nodes[index]
 
-	def get_bounding_box_visual(self, objs: Union[Mesh, List[Mesh]], col=(1., 0., 0.), thickness=0.01) -> BBoxOverlays:
-		"""Given a single Mesh instance, or a list of Mesh instances, return a CompositorNodeGroup,
-		which will render the bounding box of the object(s)
+	def get_bounding_box_visual(self, col=(0., 0., 255., 255.), thickness=5) -> BoundingBoxOverlay:
+		"""
+		return a CompositorNodeGroup,
+		which will render the bounding boxes of the objects
 
-		:param objs: Mesh instance, or list of Mesh instances
-		:param col: (3,) or (N, 3) Color(s) of bounding box(es)
+		:param col: (3,) or (N, 3) Color(s) of bounding box(es) [in BGR]
 		:param thickness: (,) or (N,) Thickness(es) of bounding box(es)
 		"""
 
-		if isinstance(objs, Mesh):
-			objs = [objs]
-
-		cng = BBoxOverlays(f"Bounding Box Visual - {len(objs)}", self.node_tree, objs, col=col, thickness=thickness)
+		cng = BoundingBoxOverlay(f"Bounding Box Visual", self.node_tree, col=col, thickness=thickness)
 		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
 
 		if 'BBox' in self.overlays:
 			raise ValueError("Only allowed one BBox overlay (it can contain multiple objects).")
 
 		self.overlays['BBox'] = cng
 
 		self.tidy_tree()
 		return cng
 
+	def get_keypoints_visual(self) -> KeypointsOverlay:
+		"""
+		Initialize a keypoints overlay node
+		"""
+
+		cng = KeypointsOverlay(f"Keypoints Visual", self.node_tree)
+		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
+
+		if 'Keypoints' in self.overlays:
+			raise ValueError("Only allowed one Keypoints overlay.")
+
+		self.overlays['Keypoints'] = cng
+
+		self.tidy_tree()
+		return cng
+
+	def get_depth_visual(self, max_depth=1, col=(255, 255, 255)):
+		"""Get depth visual, which normalizes depth values so max_depth = col,
+		and any values below that are depth/max_depth * col.
+
+		Col = 0-255 RGB or RGBA"""
+
+		if 'Depth' not in self.render_layers_node.outputs:
+			render_depth()
+
+		# convert col to 0-1, RGBA
+		col = ([i/255 for i in col] + [1])[:4]
+
+		cng = DepthVis(self.node_tree, max_depth=max_depth, col=col)
+		self.node_tree.links.new(self.render_layers_node.outputs['Depth'], cng.input('Depth'))
+
+		self.tidy_tree()
+		return cng
+
 	def define_output(self, input_data: Union[str, CompositorNodeGroup, AOV], directory, file_name=None, mode='image',
 					  file_format='PNG', color_mode='RGBA', jpeg_quality=90,
 					  png_compression=15, color_depth='8', EXR_color_depth='32',
 					  name=None):
 		"""Add a connection between a valid render output, and a file output node.
 		Supports changing view output.
 
@@ -228,12 +263,40 @@
 			)
 
 	def update_aovs(self):
 		"""Update any AOVs that are connected to the render layers node"""
 		for aov in self.aovs:
 			aov.update()
 
-	def render(self):
+	def render(self, camera=None, scene=None, overlay_kwargs=None,
+			   animation=False, frame_start=0, frame_end=250):
 		"""Render the scene"""
+		if overlay_kwargs is None:
+			overlay_kwargs = {}
+
+		if scene is None:
+			scene = bpy.context.scene
+
+		if camera is None:
+			camera = scene.camera
+
+		for k in overlay_kwargs.keys():
+			assert k in self.overlays, f"overlay_kwarg {k} not in overlays: {[*self.overlays.keys()]}."
+
+		for oname, overlay in self.overlays.items():
+			args = overlay_kwargs.get(oname, {})
+			if isinstance(args, dict):
+				overlay.update(camera=camera, scene=scene, **args)  # multi kwargs
+			else:
+				overlay.update(args, camera=camera, scene=scene)  # single arg
+
+
 		self.update_aovs()
-		render()
-		self.fix_namings()
+
+		if animation:
+			scene.frame_start = frame_start
+			scene.frame_end = frame_end
+
+		render(animation=animation)
+
+		if not animation:
+			self.fix_namings()
```

### Comparing `blendersynth-0.0.2/blendersynth/blender/compositor/mask_overlay.py` & `blendersynth-0.0.3/blendersynth/blender/compositor/mask_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/blender/compositor/node_group.py` & `blendersynth-0.0.3/blendersynth/blender/compositor/node_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 		return self.gn.inputs
 
 	@property
 	def outputs(self):
 		return self.gn.outputs
 
 	def input(self, name):
-		# return self.input_node.outputs[name]
 		return self.inputs[name]
 
 	def output(self, name):
 		return self.outputs[name]
 
 	def __str__(self):
-		return f"CompositorNodeGroup({self.name})"
+		return f"CompositorNodeGroup({self.name})"
+
+	def update(self, camera=None, scene=None):
+		pass
```

### Comparing `blendersynth-0.0.2/blendersynth/blender/light.py` & `blendersynth-0.0.3/blendersynth/blender/light.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/blender/mesh.py` & `blendersynth-0.0.3/blendersynth/blender/mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os.path
 
 import bpy
-from .utils import GetNewObject, SelectObjects
+from .utils import GetNewObject, SelectObjects, handle_vec
 from .aov import AOV
 import numpy as np
 import mathutils
-from mathutils import Vector, Matrix, Euler
+from mathutils import Vector, Euler
 
 _primitives ={
 	"cube": bpy.ops.mesh.primitive_cube_add,
 	"sphere": bpy.ops.mesh.primitive_uv_sphere_add,
 	"cylinder": bpy.ops.mesh.primitive_cylinder_add,
 	"plane": bpy.ops.mesh.primitive_plane_add,
 	"cone": bpy.ops.mesh.primitive_cone_add,
 	"monkey": bpy.ops.mesh.primitive_monkey_add,
 	"torus": bpy.ops.mesh.primitive_torus_add,
 }
 
 default_ids = {
-	'prim_cube': 0,
-	'prim_sphere': 1,
-	'prim_cylinder': 2,
-	'prim_plane': 3,
-	'prim_cone': 4,
-	'prim_monkey': 5,
-	'prim_torus': 6,
-	'loaded_mesh': 7,
+	'loaded_mesh': 0,
+	'prim_cube': 1,
+	'prim_sphere': 2,
+	'prim_cylinder': 3,
+	'prim_plane': 4,
+	'prim_cone': 5,
+	'prim_monkey': 6,
+	'prim_torus': 7,
 }
 
 def get_child_meshes(obj):
 	"""Given an object, return all meshes that are children of it. Recursively searches children of children.
 	Also returns any child objects that aren't meshes"""
 	if obj.type == 'MESH':
 		return [obj], []
@@ -57,22 +57,14 @@
 	if mesh.type == 'MESH':
 		delta = mesh.location - mathutils.Vector(vec)
 		delta_object = mesh.matrix_world.inverted() @ delta
 		mesh.data.transform(mathutils.Matrix.Translation(delta_object))  # Move the mesh vertices in the opposite direction
 		mesh.location -= delta_object
 		bpy.context.view_layer.update()
 
-def handle_vec(vec, expected_length=3):
-	"""Check ven is expected_length. Convert from tuple or ndarray to mathutils.Vector """
-	if isinstance(vec, (tuple, list)):
-		vec = mathutils.Vector(vec)
-	elif isinstance(vec, np.ndarray):
-		vec = mathutils.Vector(vec.tolist())
-	assert len(vec) == expected_length, "Vector must be length {}".format(expected_length)
-	return vec
 
 def euler_from(a: mathutils.Euler, b: mathutils.Euler):
 	"""Get euler rotation from a to b"""
 	return (b.to_matrix() @ a.to_matrix().inverted()).to_euler()
 
 def euler_add(a: mathutils.Euler, b: mathutils.Euler):
 	"""Compute euler rotation of a, followed by b"""
@@ -265,22 +257,18 @@
 	# @property
 	# def bound_box(self):
 	# 	"""Return bounding box of object(s)"""
 	# 	return self.obj.bound_box
 
 	@property
 	def matrix_world(self):
-		"""Return world matrix of object(s)"""
+		"""Return world matrix of object(s).
+		"""
 		bpy.context.evaluated_depsgraph_get() # required to update object matrix
-
-		if len(self._meshes) == 1:
-			return self.obj.matrix_world
-
-		else:
-			return [m.matrix_world for m in self._meshes]
+		return self._meshes[0].matrix_world
 
 	@property
 	def scale(self):
 		"""Return scale of primary mesh."""
 		return self._scale
 
 	@scale.setter
@@ -392,8 +380,33 @@
 
 		return np.mean(centroids, axis=0)
 
 	def origin_to_centroid(self, method='bounds'):
 		"""Move object origin to centroid"""
 		centroid = self.centroid(method=method)
 		for mesh in self._meshes:
-			set_origin(mesh, centroid)
+			set_origin(mesh, centroid)
+
+	def get_keypoints(self, idxs=None, position=None):
+		"""Return 3D keypoint positions in world coordinates, given either:
+
+		idxs: list of indices or ndarray of keypoints to project (only valid for single-mesh objects)
+		position: 3D position of keypoints to project - in LOCAL object coordinates
+
+		:return N list of Vectors of keypoints in world space, where N is the number of keypoints:
+		"""
+
+		assert (idxs is not None) ^ (position is not None), "Must provide either idxs or position, but not both."
+
+
+		if idxs is not None:
+			assert len(self._meshes) == 1, "Can only project keypoints by index for single-mesh objects."
+			kps3d = [self.matrix_world @ self._meshes[0].data.vertices[i].co for i in idxs]
+
+		elif position is not None:
+			kps3d = [self.matrix_world @ p for p in position]
+
+		return kps3d
+
+	@property
+	def name(self):
+		return self._meshes[0].name
```

### Comparing `blendersynth-0.0.2/blendersynth/blender/world.py` & `blendersynth-0.0.3/blendersynth/blender/world.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/file/dataset_inputs.py` & `blendersynth-0.0.3/blendersynth/file/dataset_inputs.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/run/blender_threading.py` & `blendersynth-0.0.3/blendersynth/run/blender_threading.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/run/run.py` & `blendersynth-0.0.3/blendersynth/run/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from .blender_threading import BlenderThreadManager, list_split
 from ..utils.blender_setup.blender_locator import get_blender_path
 from copy import deepcopy
+from ..file.tempfiles import cleanup_temp_files as cleanup
 
 from sys import platform
 if platform == "linux" or platform == "linux2" or platform == "darwin":
 	nul_text = '/dev/null'
 elif platform == "win32":
 	nul_text = 'nul'
 
@@ -89,8 +90,10 @@
 	if print_to_stdout:
 		raise NotImplementedError("Print to stdout not supported yet.")
 
 	if isinstance(json_src, str):
 		json_src = sorted([os.path.join(json_src, f) for f in os.listdir(json_src) if f.endswith(".json")])
 
 	Runner(script, json_src, output_directory, num_threads, print_to_stdout=print_to_stdout,
-			**script_kwargs)
+			**script_kwargs)
+
+	cleanup()
```

### Comparing `blendersynth-0.0.2/blendersynth/run_this_script.py` & `blendersynth-0.0.3/blendersynth/run_this_script.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Quick utility to run the current script from Blender"""
 import subprocess
 import inspect
 import sys
 from .utils.blender_setup.blender_locator import get_blender_path
+from .file.tempfiles import cleanup_temp_files as cleanup
 
 def run_this_script(debug=False):
 	"""Run the current script from Blender"""
 	blender_path = get_blender_path()
 	if blender_path != sys.argv[0]:  # if blender is not running this script
 
 		caller_path = inspect.stack()[1].filename # path of script that called this function
 
 		commands = [blender_path] + \
 			['--background'] * (not debug) + \
 			['--python', caller_path]
 
 		subprocess.call(commands)
-		sys.exit() # exit the script once blender is finished
+
+		cleanup()  # cleanup temp files
+		sys.exit()  # exit the script once blender is finished
```

### Comparing `blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_locator.py` & `blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_locator.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.2/blendersynth/utils/blender_setup/check_blender_install.py` & `blendersynth-0.0.3/blendersynth/utils/blender_setup/check_blender_install.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import subprocess
 import os
 from blendersynth.utils.blender_setup.blender_locator import find_blender_python, get_blender_path, remove_config, write_to_config, read_from_config, remove_from_config
 
-from time import perf_counter
-
-dependencies = ['imageio', 'numpy', 'appdirs', 'tqdm']
+dependencies = ['imageio', 'numpy', 'appdirs', 'tqdm', 'opencv-python', 'ffmpeg-python']
 
 def check_module(python_executable, module_name):
 	try:
 		subprocess.check_call([python_executable, '-m', 'pip', 'show', module_name],
 							  stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
 		return True
 	except subprocess.CalledProcessError:
```

### Comparing `blendersynth-0.0.2/blendersynth/utils/node_arranger.py` & `blendersynth-0.0.3/blendersynth/utils/node_arranger.py`

 * *Files identical despite different names*

