# Comparing `tmp/p4tools-0.8.0.tar.gz` & `tmp/p4tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/p4tools-0.8.0.tar", last modified: Wed Jul 10 17:36:07 2019, max compression
+gzip compressed data, was "p4tools-0.9.0.tar", last modified: Wed Jul  5 14:36:41 2023, max compression
```

## Comparing `p4tools-0.8.0.tar` & `p4tools-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:07.000000 p4tools-0.8.0/
--rw-r--r--   0 klay6683 (273771)     2260      162 2018-11-24 06:41:36.000000 p4tools-0.8.0/AUTHORS.rst
--rw-r--r--   0 klay6683 (273771)     2260     3176 2019-06-21 06:44:13.000000 p4tools-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 klay6683 (273771)     2260       89 2018-11-24 06:41:36.000000 p4tools-0.8.0/HISTORY.rst
--rw-r--r--   0 klay6683 (273771)     2260      748 2018-11-24 06:41:36.000000 p4tools-0.8.0/LICENSE
--rw-r--r--   0 klay6683 (273771)     2260      262 2018-11-24 06:41:36.000000 p4tools-0.8.0/MANIFEST.in
--rw-r--r--   0 klay6683 (273771)     2260     3857 2019-07-10 17:36:07.000000 p4tools-0.8.0/PKG-INFO
--rw-r--r--   0 klay6683 (273771)     2260     2473 2019-06-27 21:26:24.000000 p4tools-0.8.0/README.rst
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:06.000000 p4tools-0.8.0/docs/
--rw-r--r--   0 klay6683 (273771)     2260     6766 2019-06-21 06:44:32.000000 p4tools-0.8.0/docs/Makefile
--rw-r--r--   0 klay6683 (273771)     2260       28 2018-11-24 06:41:36.000000 p4tools-0.8.0/docs/authors.rst
--rwxr-xr-x   0 klay6683 (273771)     2260     8435 2019-06-21 06:44:21.000000 p4tools-0.8.0/docs/conf.py
--rw-r--r--   0 klay6683 (273771)     2260       33 2018-11-24 06:41:36.000000 p4tools-0.8.0/docs/contributing.rst
--rw-r--r--   0 klay6683 (273771)     2260       28 2018-11-24 06:41:36.000000 p4tools-0.8.0/docs/history.rst
--rw-r--r--   0 klay6683 (273771)     2260      303 2018-11-24 06:41:36.000000 p4tools-0.8.0/docs/index.rst
--rw-r--r--   0 klay6683 (273771)     2260     1152 2019-06-21 06:44:24.000000 p4tools-0.8.0/docs/installation.rst
--rw-r--r--   0 klay6683 (273771)     2260     6703 2019-06-21 06:44:29.000000 p4tools-0.8.0/docs/make.bat
--rw-r--r--   0 klay6683 (273771)     2260       27 2018-11-24 06:41:36.000000 p4tools-0.8.0/docs/readme.rst
--rw-r--r--   0 klay6683 (273771)     2260       79 2019-06-21 06:44:34.000000 p4tools-0.8.0/docs/usage.rst
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools/
--rw-r--r--   0 klay6683 (273771)     2260      166 2019-07-10 17:35:07.000000 p4tools-0.8.0/p4tools/__init__.py
--rw-r--r--   0 klay6683 (273771)     2260      360 2019-06-21 06:44:52.000000 p4tools-0.8.0/p4tools/cli.py
--rw-r--r--   0 klay6683 (273771)     2260     4428 2019-06-28 05:44:27.000000 p4tools-0.8.0/p4tools/io.py
--rw-r--r--   0 klay6683 (273771)     2260    15239 2019-07-10 17:29:56.000000 p4tools-0.8.0/p4tools/markings.py
--rw-r--r--   0 klay6683 (273771)     2260      671 2019-07-10 17:32:52.000000 p4tools-0.8.0/p4tools/plotting.py
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/
--rw-r--r--   0 klay6683 (273771)     2260     3857 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/PKG-INFO
--rw-r--r--   0 klay6683 (273771)     2260      671 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/SOURCES.txt
--rw-r--r--   0 klay6683 (273771)     2260        1 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/dependency_links.txt
--rw-r--r--   0 klay6683 (273771)     2260       46 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/entry_points.txt
--rw-r--r--   0 klay6683 (273771)     2260        1 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/not-zip-safe
--rw-r--r--   0 klay6683 (273771)     2260       39 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/requires.txt
--rw-r--r--   0 klay6683 (273771)     2260        8 2019-07-10 17:36:06.000000 p4tools-0.8.0/p4tools.egg-info/top_level.txt
--rw-r--r--   0 klay6683 (273771)     2260      815 2019-07-10 17:36:07.000000 p4tools-0.8.0/setup.cfg
--rw-r--r--   0 klay6683 (273771)     2260     1372 2019-07-10 17:35:07.000000 p4tools-0.8.0/setup.py
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:07.000000 p4tools-0.8.0/tests/
-drwxr-xr-x   0 klay6683 (273771)     2260        0 2019-07-10 17:36:07.000000 p4tools-0.8.0/tests/.ipynb_checkpoints/
--rw-r--r--   0 klay6683 (273771)     2260       72 2019-06-27 21:47:58.000000 p4tools-0.8.0/tests/.ipynb_checkpoints/test_p4tools.io-checkpoint.ipynb
--rw-r--r--   0 klay6683 (273771)     2260     1007 2019-06-27 21:28:44.000000 p4tools-0.8.0/tests/test_p4_tools.py
--rw-r--r--   0 klay6683 (273771)     2260      713 2019-06-27 21:50:01.000000 p4tools-0.8.0/tests/test_p4tools.io.ipynb
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.192963 p4tools-0.9.0/
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      189 2023-05-12 11:59:17.000000 p4tools-0.9.0/AUTHORS.rst
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     3176 2019-06-21 06:44:13.000000 p4tools-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)       89 2018-11-24 06:41:36.000000 p4tools-0.9.0/HISTORY.rst
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      748 2018-11-24 06:41:36.000000 p4tools-0.9.0/LICENSE
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      189 2023-07-03 08:43:02.000000 p4tools-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)      741 2023-07-05 14:36:41.192963 p4tools-0.9.0/PKG-INFO
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     2473 2019-06-27 21:26:24.000000 p4tools-0.9.0/README.rst
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.180963 p4tools-0.9.0/p4tools/
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)       22 2023-07-03 21:02:29.000000 p4tools-0.9.0/p4tools/__init__.py
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)    10443 2023-07-05 14:33:57.000000 p4tools-0.9.0/p4tools/_modidx.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      228 2023-07-03 21:05:13.000000 p4tools-0.9.0/p4tools/data_extract.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     3953 2023-07-03 21:02:29.000000 p4tools-0.9.0/p4tools/io.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    18408 2023-07-03 21:02:29.000000 p4tools-0.9.0/p4tools/markings.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     3101 2023-07-03 21:02:29.000000 p4tools-0.9.0/p4tools/plotting.py
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.184963 p4tools-0.9.0/p4tools.egg-info/
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)      741 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/PKG-INFO
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)     1006 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)        1 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)       36 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/entry_points.txt
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)        1 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/not-zip-safe
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)       36 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/requires.txt
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)       20 2023-07-05 14:36:41.000000 p4tools-0.9.0/p4tools.egg-info/top_level.txt
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.184963 p4tools-0.9.0/p4tools_bak/
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      229 2023-07-03 14:12:57.000000 p4tools-0.9.0/p4tools_bak/__init__.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    10474 2023-07-03 20:58:46.000000 p4tools-0.9.0/p4tools_bak/_modidx.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      497 2022-05-16 04:08:40.000000 p4tools-0.9.0/p4tools_bak/cli.py
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.184963 p4tools-0.9.0/p4tools_bak/data/
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)        0 2023-07-03 14:12:57.000000 p4tools-0.9.0/p4tools_bak/data/__init__.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      228 2023-07-03 20:28:11.000000 p4tools-0.9.0/p4tools_bak/data_extract.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     3953 2023-07-03 14:12:57.000000 p4tools-0.9.0/p4tools_bak/io.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    18408 2023-07-03 14:12:57.000000 p4tools-0.9.0/p4tools_bak/markings.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     3101 2023-07-03 14:12:57.000000 p4tools-0.9.0/p4tools_bak/plotting.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)      499 2023-07-05 14:36:41.192963 p4tools-0.9.0/setup.cfg
+-rw-rw-r--   0 ayek72    (1000) ayek72    (1000)     2596 2023-07-03 08:31:03.000000 p4tools-0.9.0/setup.py
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.188963 p4tools-0.9.0/tests/
+drwxrwxr-x   0 ayek72    (1000) ayek72    (1000)        0 2023-07-05 14:36:41.192963 p4tools-0.9.0/tests/.ipynb_checkpoints/
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    42842 2019-09-12 23:57:16.000000 p4tools-0.9.0/tests/.ipynb_checkpoints/plotcircles-checkpoint.pdf
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    46257 2019-09-12 23:57:16.000000 p4tools-0.9.0/tests/.ipynb_checkpoints/plotcircles-checkpoint.png
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)   761698 2023-07-03 08:32:43.000000 p4tools-0.9.0/tests/.ipynb_checkpoints/test_markings-checkpoint.ipynb
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     1007 2019-06-27 21:28:44.000000 p4tools-0.9.0/tests/.ipynb_checkpoints/test_p4_tools-checkpoint.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    78513 2023-07-03 08:32:43.000000 p4tools-0.9.0/tests/.ipynb_checkpoints/test_p4tools.io-checkpoint.ipynb
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     5781 2019-09-13 00:33:59.000000 p4tools-0.9.0/tests/plotcircles.pdf
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     6725 2019-09-13 00:33:59.000000 p4tools-0.9.0/tests/plotcircles.png
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)   761698 2023-07-03 08:32:43.000000 p4tools-0.9.0/tests/test_markings.ipynb
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)     1007 2019-06-27 21:28:44.000000 p4tools-0.9.0/tests/test_p4_tools.py
+-rw-r--r--   0 ayek72    (1000) ayek72    (1000)    78513 2023-07-03 08:32:43.000000 p4tools-0.9.0/tests/test_p4tools.io.ipynb
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `p4tools-0.8.0/CONTRIBUTING.rst` & `p4tools-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `p4tools-0.8.0/LICENSE` & `p4tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p4tools-0.8.0/README.rst` & `p4tools-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `p4tools-0.8.0/p4tools/markings.py` & `p4tools-0.9.0/p4tools/markings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,66 @@
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/01_markings.ipynb.
+
+# %% auto 0
+__all__ = ['IMG_X_SIZE', 'IMG_Y_SIZE', 'show_subframe', 'set_subframe_size', 'calc_fig_size', 'Blotch', 'TileBlotches',
+           'rotate_vector', 'Fan']
+
+# %% ../notebooks/01_markings.ipynb 2
 import math
 from math import cos, degrees, pi, radians, sin
 from pathlib import Path
 
 import matplotlib.lines as lines
 import matplotlib.patches as mpatches
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
+from matplotlib.collections import PatchCollection
 from matplotlib.patches import Ellipse
 from numpy import arctan2
 from numpy import linalg as LA
 from shapely import affinity
 from shapely import geometry as geom
 
 from . import io
 
+# %% ../notebooks/01_markings.ipynb 3
 IMG_X_SIZE = 840
+
+# %% ../notebooks/01_markings.ipynb 4
 IMG_Y_SIZE = 648
 
+# %% ../notebooks/01_markings.ipynb 5
+def show_subframe(tile_id, ax=None, aspect="auto"):
+    subframe = io.get_subframe_by_tile_id(tile_id)
+    if ax is None:
+        _, ax = plt.subplots(figsize=calc_fig_size(8))
+    ax.imshow(subframe, origin="upper", aspect=aspect)
+    ax.set_axis_off()
+    return ax
 
+# %% ../notebooks/01_markings.ipynb 6
 def set_subframe_size(ax):
     """Set plot view limit on Planet 4 subframe size."""
     ax.set_xlim(0, IMG_X_SIZE)
     ax.set_ylim(IMG_Y_SIZE, 0)
 
-
+# %% ../notebooks/01_markings.ipynb 7
 def calc_fig_size(width):
     """Calc figure height in ratio of subframes."""
     ratio = IMG_X_SIZE / IMG_Y_SIZE
     return (width, width / ratio)
 
+# %% ../notebooks/01_markings.ipynb 8
+# class Marking:
+#     def __init__(self, data, scope="planet4"):
+#         self.data = data
+#         self.scope = scope
 
-class Marking:
-    def __init__(self, data, scope="planet4"):
-        self.data = data
-        self.scope = scope
-
-
+# %% ../notebooks/01_markings.ipynb 9
 class Blotch(Ellipse):
 
     """Blotch management class for P4.
 
     Parameters
     ----------
     data : object with blotch data attributes
@@ -57,14 +77,20 @@
     data : object with blotch data attributes, as provided by `data`
     center : tuple (inherited from matplotlib.Ellipse)
         Coordinates of center, i.e. self.x, self.y
     """
 
     to_average = "x y image_x image_y angle radius_1 radius_2".split()
 
+    @classmethod
+    def from_tile_id(cls, tile_id, n=0, **kwargs):
+        df = io.get_blotch_catalog()
+        data = df[df.tile_id == tile_id].iloc[n]
+        return cls(data, **kwargs)
+        
     def __init__(self, data, scope="planet4", with_center=False, url_db="", **kwargs):
         self.data = data
         self.scope = scope if scope is not None else "planet4"
         self.with_center = with_center
         self.url_db = Path(url_db)
         self.ax = None
         if scope not in ["hirise", "planet4"]:
@@ -78,26 +104,29 @@
         # default member number is 1. This is set to the cluster member inside
         # clustering execution.
         self._n_members = 1
         super(Blotch, self).__init__(
             (self.x, self.y),
             data.radius_1 * 2,
             data.radius_2 * 2,
-            data.angle,
+            angle=data.angle,
             alpha=0.65,
             linewidth=2,
             fill=False,
             **kwargs
         )
         self.data = data
 
     @property
+    def tile_id(self):
+        return self.data.tile_id
+
+    @property
     def subframe(self):
-        url = io.get_url_for_tile_id(self.data.tile_id)
-        return io.get_subframe(url)
+        return io.get_subframe_by_tile_id(self.data.tile_id)
 
     def show_subframe(self, ax=None, aspect="auto"):
         if ax is None:
             _, ax = plt.subplots(figsize=calc_fig_size(8))
         ax.imshow(self.subframe, origin="upper", aspect=aspect)
         ax.set_axis_off()
         self.ax = ax
@@ -178,23 +207,24 @@
         return self._n_members
 
     @n_members.setter
     def n_members(self, value):
         self._n_members = value
 
     def plot(self, color="green", ax=None):
-        self.show_subframe(ax)
-        ax = self.ax
         if ax is None:
             _, ax = plt.subplots()
+        self.show_subframe(ax)
+        ax = self.ax
         if color is not None:
             self.set_color(color)
         ax.add_patch(self)
         if self.with_center:
             self.plot_center(ax, color=color)
+        set_subframe_size(ax)
 
     def store(self, fpath=None):
         out = self.data
         for p in range(1, 5):
             attr = "p" + str(p)
             point = getattr(self, attr)
             out[attr + "_x"] = point[0]
@@ -213,32 +243,57 @@
         s += "\n"
         s += "N_members: {}".format(self.n_members)
         return s
 
     def __repr__(self):
         return self.__str__()
 
+# %% ../notebooks/01_markings.ipynb 13
+class TileBlotches:
+    def __init__(self, tile_id, with_center=False, color='green'):
+        """Container for all blotches of a tile.
+
+        Parameters
+        ----------
+        tile_id :  str
+            planetfour tile_id
+        """
+        self.tile_id = tile_id
+        self.with_center = with_center
+        self.blotches_df = io.get_blotches_for_tile(tile_id)
+        self.collection = [
+            Blotch(blotch, with_center=self.with_center, color=color)
+            for _, blotch in self.blotches_df.iterrows()
+        ]
+        self.p = PatchCollection(self.collection, match_original=True)
 
+    def plot(self, ax=None):
+        if ax is None:
+            _, ax = plt.subplots()
+        ax = show_subframe(self.tile_id, ax=ax)
+        ax.add_collection(self.p)
+        set_subframe_size(ax)
+
+# %% ../notebooks/01_markings.ipynb 16
 def rotate_vector(v, angle):
     """Rotate vector by angle given in degrees.
 
     Parameters
     ----------
     v : np.array
         Vector to be rotated
     angle : float
         Angle in degrees
     """
     rangle = radians(angle)
     rotmat = np.array([[cos(rangle), -sin(rangle)], [sin(rangle), cos(rangle)]])
     return rotmat.dot(v)
 
-
+# %% ../notebooks/01_markings.ipynb 17
 class Fan(lines.Line2D):
-
     """Fan management class for P4.
 
     Parameters
     ----------
     data : object with fan data attributes
         object has to provide [`x`, `y`, `angle`, `spread`, `distance`]
     scope : {'planet4', 'hirise'}
@@ -268,25 +323,32 @@
     radius
     midpoint
     base_to_midpoint_vec
     """
 
     to_average = "x y image_x image_y angle spread distance".split()
 
+    @classmethod
+    def from_tile_id(cls, tile_id, n=0, **kwargs):
+        df = io.get_fan_catalog()
+        data = df[df.tile_id==tile_id].iloc[n]
+        return cls(data, **kwargs)
+        
     def __init__(self, data, scope="planet4", with_center=False, **kwargs):
         self.data = data
         self.scope = scope if scope is not None else "planet4"
         self.with_center = with_center
         if scope not in ["hirise", "planet4"]:
             raise TypeError("Unknown scope: {}".format(scope))
         # first coordinate is the base of fan
         actual_x = "x" if scope == "planet4" else "image_x"
         actual_y = "y" if scope == "planet4" else "image_y"
         try:
-            self.base = self.data.loc[[actual_x, actual_y]].values.astype("float")
+            self.base = self.data.loc[[actual_x,
+                                       actual_y]].values.astype("float")
         except KeyError:
             print("No x and y in the data:\n{}".format(data))
             raise KeyError
         # default n_members value (property)
         self._n_members = 1
         # angles
         self.inside_half = self.data.spread / 2.0
@@ -295,56 +357,56 @@
         # length of arms
         self.armlength = self.get_arm_length()
         # first arm
         self.v1 = rotate_vector([self.armlength, 0], alpha)
         # second arm
         self.v2 = rotate_vector([self.armlength, 0], beta)
         # vector matrix, stows the 1D vectors row-wise
-        self.coords = np.vstack((self.base + self.v1, self.base, self.base + self.v2))
+        self.coords = np.vstack(
+            (self.base + self.v1, self.base, self.base + self.v2))
         # init fan line, first column are the x-components of the row-vectors
-        lines.Line2D.__init__(
-            self,
-            self.coords[:, 0],
-            self.coords[:, 1],
-            alpha=0.65,
-            color="white",
-            **kwargs
-        )
+        lines.Line2D.__init__(self,
+                              self.coords[:, 0],
+                              self.coords[:, 1],
+                              alpha=0.65,
+                              color="white",
+                              **kwargs)
 
     def is_equal(self, other):
-        if (
-            self.data.x == other.data.x
-            and self.data.y == other.data.y
-            and self.data.image_x == other.data.image_x
-            and self.data.image_y == other.data.image_y
-            and self.data.angle == other.data.angle
-            and self.data.spread == other.data.spread
-            and self.data.distance == other.data.distance
-        ):
+        if (self.data.x == other.data.x and self.data.y == other.data.y and
+                self.data.image_x == other.data.image_x and
+                self.data.image_y == other.data.image_y and
+                self.data.angle == other.data.angle and
+                self.data.spread == other.data.spread and
+                self.data.distance == other.data.distance):
             return True
         else:
             return False
 
     @property
+    def tile_id(self):
+        return self.data.tile_id
+
+    @property
     def n_members(self):
         return self._n_members
 
     @n_members.setter
     def n_members(self, value):
         self._n_members = value
 
     def get_arm_length(self):
         half = radians(self.inside_half)
         return self.data.distance / (cos(half) + sin(half))
 
     @property
     def area(self):
-        tr_h = np.sqrt(self.armlength ** 2 - self.radius ** 2)
+        tr_h = np.sqrt(self.armlength**2 - self.radius**2)
         tr_area = tr_h * self.radius
-        half_circ_area = 0.5 * pi * self.radius ** 2
+        half_circ_area = 0.5 * pi * self.radius**2
         return tr_area + half_circ_area
 
     @property
     def circle_base(self):
         "float[2] : Vector between end of first arm and second arm of fan."
         return self.v1 - self.v2
 
@@ -379,65 +441,83 @@
         ax.add_patch(wedge)
 
     def add_mean_wind_pointer(self, ax, color="b", ls="-"):
         "Draw a thicker mean wind direction pointer for better visibility in plots."
         endpoint = rotate_vector([3 * self.armlength, 0], self.data.angle)
         coords = np.vstack((self.base, self.base + endpoint))
         self.wind_pointer_end = coords[1]
-        pointer = lines.Line2D(
-            coords[:, 0], coords[:, 1], alpha=0.65, linewidth=1, linestyle=ls
-        )
+        pointer = lines.Line2D(coords[:, 0],
+                               coords[:, 1],
+                               alpha=0.65,
+                               linewidth=1,
+                               linestyle=ls)
         pointer.set_color(color)
         ax.add_line(pointer)
 
-    def plot(self, color=None, ax=None):
+    def plot(self, color="green", ax=None):
         if ax is None:
             _, ax = plt.subplots()
-            set_subframe_size(ax)
+        ax = show_subframe(self.tile_id, ax=ax)
         if color is not None:
             self.set_color(color)
         ax.add_line(self)
         self.add_semicircle(ax, color=color)
         if self.with_center:
             self.plot_center(ax, color=color)
+        set_subframe_size(ax)
+
+    # def plot(self, color="green", ax=None):
+    #     self.show_subframe(ax)
+    #     ax = self.ax
+    #     if ax is None:
+    #         _, ax = plt.subplots()
+    #     if color is not None:
+    #         self.set_color(color)
+    #     ax.add_patch(self)
+    #     if self.with_center:
+    #         self.plot_center(ax, color=color)
 
     @property
     def center(self):
         """Calculate vector to half total length.
 
         As total length, I define the armlength + the radius of the semi-circle
         at the end.
         """
-        mid_point_vec = rotate_vector(
-            [0.5 * (self.armlength + self.radius), 0], self.data.angle
-        )
+        mid_point_vec = rotate_vector([0.5 * (self.armlength + self.radius), 0],
+                                      self.data.angle)
         return self.base + mid_point_vec
 
     def plot_center(self, ax, color="b"):
-        ax.scatter(self.center[0], self.center[1], color=color, s=20, marker=".")
+        ax.scatter(self.center[0],
+                   self.center[1],
+                   color=color,
+                   s=20,
+                   marker=".")
 
     @property
     def base_to_center_vec(self):
         coords = np.vstack((self.base, self.center))
         return coords
 
     def add_midpoint_pointer(self, ax, color="b", ls="-"):
         coords = self.base_to_center_vec
-        pointer = lines.Line2D(
-            coords[:, 0], coords[:, 1], alpha=0.65, linewidth=3, linestyle=ls
-        )
+        pointer = lines.Line2D(coords[:, 0],
+                               coords[:, 1],
+                               alpha=0.65,
+                               linewidth=3,
+                               linestyle=ls)
         pointer.set_color(color)
         ax.add_line(pointer)
 
     def __str__(self):
         out = "markings.Fan object. Input data:\n"
 
         out += "base: {0}\narmlength: {1}\narm1: {2}\narm2: {3}".format(
-            self.base, self.armlength, self.base + self.v1, self.base + self.v2
-        )
+            self.base, self.armlength, self.base + self.v1, self.base + self.v2)
         return out
 
     def __repr__(self):
         return self.__str__()
 
     def store(self, fpath=None):
         out = self.data
@@ -465,19 +545,20 @@
         # make a semi-circle first that points to the x-axis, rotate later.
         start_angle = 270  # In degrees
 
         # number of elements for the semi-circle
         numsegments = 100
 
         # The coordinates of the arc
-        theta = np.radians(np.linspace(start_angle, start_angle + 180, numsegments))
+        theta = np.radians(
+            np.linspace(start_angle, start_angle + 180, numsegments))
         x = centerx + self.radius * np.cos(theta)
         y = centery + self.radius * np.sin(theta)
 
         arc = geom.LineString(np.column_stack([x, y]))
 
-        rotated = affinity.rotate(
-            arc, self.data.angle, origin=tuple(self.semi_circle_center)
-        )
+        rotated = affinity.rotate(arc,
+                                  self.data.angle,
+                                  origin=tuple(self.semi_circle_center))
 
         df = pd.DataFrame(np.vstack([self.coords[::-1][:2], np.array(rotated)]))
         return geom.Polygon(df.round(2).drop_duplicates().values)
```

### Comparing `p4tools-0.8.0/tests/test_p4_tools.py` & `p4tools-0.9.0/tests/.ipynb_checkpoints/test_p4_tools-checkpoint.py`

 * *Files identical despite different names*

