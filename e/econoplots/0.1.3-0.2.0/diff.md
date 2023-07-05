# Comparing `tmp/econoplots-0.1.3.tar.gz` & `tmp/econoplots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econoplots-0.1.3.tar", last modified: Tue Jun 20 15:45:25 2023, max compression
+gzip compressed data, was "econoplots-0.2.0.tar", last modified: Wed Jul  5 16:11:26 2023, max compression
```

## Comparing `econoplots-0.1.3.tar` & `econoplots-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.1.3/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-06-20 15:45:25.624873 econoplots-0.1.3/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.1.3/README.md
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/econoplots/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-06-20 15:42:45.000000 econoplots-0.1.3/econoplots/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4957 2023-05-31 14:08:21.000000 econoplots-0.1.3/econoplots/_standalone_plotters.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3345 2023-06-01 18:36:30.000000 econoplots-0.1.3/econoplots/color_map.json
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3049 2023-06-01 18:36:24.000000 econoplots-0.1.3/econoplots/colors.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3752 2023-06-20 15:42:33.000000 econoplots-0.1.3/econoplots/converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      960 2023-06-20 15:25:38.000000 econoplots-0.1.3/econoplots/params.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    21758 2023-06-20 15:30:30.000000 econoplots-0.1.3/econoplots/utils.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/econoplots.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.1.3/econoplots.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-31 20:11:16.000000 econoplots-0.1.3/pyproject.toml
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-06-20 15:45:25.624873 econoplots-0.1.3/setup.cfg
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.1.3/setup.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1775 2023-06-20 15:00:16.000000 econoplots-0.1.3/tests/test_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.2.0/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-07-05 16:11:26.770766 econoplots-0.2.0/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.2.0/README.md
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/econoplots/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-07-05 16:10:26.000000 econoplots-0.2.0/econoplots/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4963 2023-06-28 15:16:29.000000 econoplots-0.2.0/econoplots/_standalone_plotters.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3513 2023-06-28 17:44:48.000000 econoplots-0.2.0/econoplots/color_map.json
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3193 2023-06-28 17:44:29.000000 econoplots-0.2.0/econoplots/colors.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4731 2023-07-05 16:09:24.000000 econoplots-0.2.0/econoplots/converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1067 2023-06-20 19:01:06.000000 econoplots-0.2.0/econoplots/params.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    24011 2023-06-28 18:09:46.000000 econoplots-0.2.0/econoplots/utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/econoplots.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.2.0/econoplots.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-31 20:11:16.000000 econoplots-0.2.0/pyproject.toml
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-07-05 16:11:26.770766 econoplots-0.2.0/setup.cfg
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.2.0/setup.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2216 2023-06-28 17:21:08.000000 econoplots-0.2.0/tests/test_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.2.0/tests/test_utils.py
```

### Comparing `econoplots-0.1.3/LICENSE` & `econoplots-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.3/PKG-INFO` & `econoplots-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.3
+Version: 0.2.0
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.3/README.md` & `econoplots-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.3/econoplots/_standalone_plotters.py` & `econoplots-0.2.0/econoplots/_standalone_plotters.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 from numpy import absolute, linspace, ndarray
 
 # Econoplots Imports
 # econoplots Imports
 from econoplots.utils import (
+    configDependentYAxis,
     makePatchSpinesInvisible,
     padXAxis,
-    setLineYAxisParams,
 )
 
 # %% Load color map
 with open("econoplots/color_map.json") as json_file:
     color_map = json.load(json_file)
 
 # %% MPL Params
@@ -88,15 +88,15 @@
             ax.fill_between(x, shaded[i][0], shaded[i][1], alpha=0.5)
 
     # set ax labels
     ax.set(xlabel=x_ax_label)
     ax.set(ylabel=y_ax_label)
 
     # set y-axis params
-    setLineYAxisParams(ax, "left")
+    configDependentYAxis(ax, "left")
 
     # delete top, right, left spines
     makePatchSpinesInvisible(ax, ["top", "right", "left"])
 
     # pad left side of x-axis
     padXAxis(ax, "left")
 
@@ -150,15 +150,15 @@
     # set ax1 colors and labels
     ax1.yaxis.label.set_color(ax1.lines[0].get_color())  # tick label color
     ax1.yaxis.set_tick_params(
         labelcolor=ax1.lines[0].get_color()
     )  # set tick color
 
     # set ax2 colors and labels
-    setLineYAxisParams(ax2, "right")
+    configDependentYAxis(ax2, "right")
     ax2.yaxis.label.set_color(ax2.lines[0].get_color())  # tick label color
     ax2.yaxis.set_tick_params(
         labelcolor=ax2.lines[0].get_color(), colors="#FFFFFF"
     )  # set tick color to transparent
 
     # scale ylimits to align yticks between ax2 and ax1
     pad1 = absolute(ax1.get_ylim()[0] - ax1.get_yticks()[1])
```

### Comparing `econoplots-0.1.3/econoplots/color_map.json` & `econoplots-0.2.0/econoplots/color_map.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897959183673469%*

 * *Differences: {"'web_all'": "{'gold1': '#674E1F', 'gold2': '#826636', 'gold3': '#9D7F4E', 'gold4': '#B99966', "*

 * *              "'gold5': '#D5B480', 'gold6': '#F2CF9A'}"}*

```diff
@@ -112,14 +112,20 @@
             "#E9EDF0",
             "#B7C6CF",
             "#758D99"
         ],
         "cyan": "#3EBCD2",
         "econ_red": "#E3120B",
         "gold": "#D1B07C",
+        "gold1": "#674E1F",
+        "gold2": "#826636",
+        "gold3": "#9D7F4E",
+        "gold4": "#B99966",
+        "gold5": "#D5B480",
+        "gold6": "#F2CF9A",
         "green": "#379A8B",
         "green1": "#005F52",
         "green2": "#00786B",
         "green3": "#2E9284",
         "green4": "#4DAD9E",
         "green5": "#69C9B9",
         "green6": "#86E5D4",
```

### Comparing `econoplots-0.1.3/econoplots/colors.py` & `econoplots-0.2.0/econoplots/colors.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     "green6": "#86E5D4",
     "purple1": "#78405F",
     "purple2": "#925977",
     "purple3": "#AD7291",
     "purple4": "#C98CAC",
     "purple5": "#E6A6C7",
     "purple6": "#FFC2E3",
+    "gold1": "#674E1F",
+    "gold2": "#826636",
+    "gold3": "#9D7F4E",
+    "gold4": "#B99966",
+    "gold5": "#D5B480",
+    "gold6": "#F2CF9A",
     "grey1": "#758D99",
     "grey2": "#3F5661",
     "grey3": "#6F8793",
     "grey4": "#89A2AE",
     "grey5": "#A4BDC9",
     "grey6": "#BFD8E5",
 }
```

### Comparing `econoplots-0.1.3/econoplots/converter.py` & `econoplots-0.2.0/econoplots/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
 
 # Econoplots Imports
 from econoplots.params import setRCParams
 from econoplots.utils import (
+    PutBarsInFront,
+    addOuterMinorTicks,
+    configDepdendentXAxis,
+    configDependentYAxis,
+    configIndependentXAxis,
+    configIndependentYAxis,
     loadColorMap,
     makePatchSpinesInvisible,
     nudgeBottomSpine,
     plotZeroPt,
     replaceAxesMinusGlyphs,
-    setBarXAxisParams,
-    setBarYAxisParams,
     setBoxColor,
     setDefaultLineColors,
     setDefaultPatchColors,
     setLegendParams,
     setLineColor,
-    setLineXAxisParams,
-    setLineYAxisParams,
+    setMajorGrids,
     updateLegendEntryColors,
 )
 
 # %% Load color map and set parameters
 setRCParams()
 
 # with open("econoplots/color_map.json") as json_file:
@@ -41,31 +44,32 @@
     ax_type: str = "line",
     **kwargs,
 ) -> Axes:
     """Formats a Matplotlib Axes as a pseudo-Economist figure.
 
     Args:
         ax (Axes): A Matplotlib object.
-        ax_type (str, optional): ["line" | "fill" | "hbox"] What type of plot is
-            contained in ax. Defaults to "line".
-        fill_area: Used for line plots.
+        ax_type (str, optional): ["line" | "fill" | "bar" | "hbox"] What type of
+            plot is contained in ax. Defaults to "line".
 
     Returns:
         Axes: A Matplotlib object.
     """
     assert isinstance(ax, Axes)
     assert ax_type in [
         "line",
         "fill",
+        "bar",
         "hbox",
     ], "ax_type not in recognized list."
 
     converter_map = {
         "line": convertLine,
         "hbox": convertHBox,
+        "bar": convertBar,
         "fill": convertLineFill,
     }
 
     # color_map = loadColorMap()
     ax = converter_map[ax_type](ax, **kwargs)
 
     return ax
@@ -86,33 +90,31 @@
     if zero_dot is True:
         ax = plotZeroPt(ax, marker_size=10)
 
     return ax
 
 
 def setLineDefaults(ax: Axes) -> Axes:
-    color_map = loadColorMap()
-
     # Change axis color
-    ax.grid(
-        which="major",
-        axis="y",
-        color=color_map["grid"]["grid_gray"],
-        zorder=1,
-        clip_on=False,
-    )
+    setMajorGrids(ax, axis="y")
+
     # set axis params
     # y_offset_text = ax.yaxis.get_offset_text().get_text()
     # x_offset_text = ax.xaxis.get_offset_text().get_text()
     replaceAxesMinusGlyphs(ax)
-    setLineYAxisParams(ax, side="right", label_location="right")
+    configDependentYAxis(ax, side="right", label_location="right")
 
     # Move bottom spine before setting xAxis params to avoid Xticks being regenerated
     nudgeBottomSpine(ax)
-    setLineXAxisParams(ax, pad_side="right", minor_ticks_on=True)
+    configIndependentXAxis(ax, pad_side="right", minor_ticks_on=True)
+
+    # Add minor tick(s) if outer limits of data are NOT on major ticks. Unlike
+    # minor ticks that are in-between major ticks, the outer minor ticks are not
+    # optional.
+    addOuterMinorTicks(ax)
 
     # delete top, right, left spines
     makePatchSpinesInvisible(ax, ["top", "right", "left"])
 
     # Set legend background
     setLegendParams(ax)
 
@@ -126,36 +128,65 @@
     ax = setDefaultPatchColors(ax)
 
     ax = updateLegendEntryColors(ax)
 
     return ax
 
 
+def convertBar(ax: Axes, orientation: str = "vertical") -> Axes:
+    assert orientation in [
+        "vertical",
+        "horizontal",
+    ], "orientation must be 'vertical' or 'horizontal'."
+
+    if orientation == "vertical":
+        grid_axis = "y"
+        invisible_spines = ["left", "right", "top"]
+    else:
+        grid_axis = "x"
+        invisible_spines = ["bottom", "right", "top"]
+
+    # Set grid
+    setMajorGrids(ax, axis=grid_axis)
+
+    # make all but left spine invisible
+    makePatchSpinesInvisible(ax, invisible_spines)
+
+    # Set x and y axes default formats
+    if orientation == "vertical":
+        configIndependentXAxis(ax, pad_side="right", minor_ticks_on=False)
+        configDependentYAxis(ax, side="right", label_location="right")
+    else:
+        configDepdendentXAxis(ax, side="top")
+        configIndependentYAxis(ax)
+
+    # Set bar zorder to be in front of grids
+    PutBarsInFront(ax)
+
+    # Reset legend colors
+    setLegendParams(ax)
+
+    return ax
+
+
 def convertHBox(ax: Axes) -> Axes:
     assert (
         len(ax.patches) > 0
     ), "Input Axes does not have filled boxes. Remake plot by setting patch_artist=True."
 
     color_map = loadColorMap()
     # Set grid on and color
-    ax.grid(
-        which="major",
-        axis="x",
-        color=color_map["grid"]["grid_gray"],
-        zorder=1,
-        clip_on=False,
-    )
-    ax.grid(which="major", axis="y", visible=False)
+    setMajorGrids(ax, axis="x")
 
     # make all but left spine invisible
     makePatchSpinesInvisible(ax, ["top", "right", "bottom"])
 
     # Set axis default params
-    setBarXAxisParams(ax, side="top")
-    setBarYAxisParams(ax)
+    configDepdendentXAxis(ax, side="top")
+    configIndependentYAxis(ax)
     replaceAxesMinusGlyphs(ax)
 
     # Set color of data series
     setBoxColor(ax, color=color_map["web_all"]["blue"])
     setLineColor(ax, color=color_map["web_all"]["blue"])
 
     return ax
```

### Comparing `econoplots-0.1.3/econoplots/params.py` & `econoplots-0.2.0/econoplots/params.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 
 
 # %% Set Params
 def setRCParams():
     color_map = loadColorMap()
 
     mpl.rcParams["font.sans-serif"] = [
+        # "CMU Sans Serif Demi Condensed",
+        # "CMU Sans Serif",
         "CMU Bright",
     ]
     mpl.rcParams["font.family"] = "sans-serif"
     mpl.rcParams.update(
         {
             "font.size": 14,
             # "font.weight": "bold",
+            # "font.weight": "600",
         }
     )
     mpl.rcParams["lines.linestyle"] = "-"
     mpl.rcParams["lines.linewidth"] = 3
     mpl.rcParams["axes.prop_cycle"] = cycler(color=color_map["line_chart"])
     mpl.rcParams["figure.facecolor"] = "w"
     mpl.rcParams["axes.facecolor"] = "w"
```

### Comparing `econoplots-0.1.3/econoplots/utils.py` & `econoplots-0.2.0/econoplots/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,32 @@
 from typing import Tuple
 
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
 from matplotlib.axis import Axis
 from matplotlib.collections import PolyCollection
-from matplotlib.patches import Patch
+from matplotlib.container import BarContainer
+from matplotlib.patches import Patch, Rectangle
 from matplotlib.text import Text
 from matplotlib.ticker import AutoMinorLocator, FixedLocator
 from numpy import (
     absolute,
+    amax,
+    amin,
     append,
+    array,
     intersect1d,
     logical_and,
     max,
     min,
     nanmax,
     nanmin,
     ndarray,
+    stack,
     where,
 )
 from numpy.ma import MaskedArray, getdata
 
 # %% Functions
 
 
@@ -88,15 +93,15 @@
     for tl in tick_labels:
         y_labels.append(replaceMinusWithHyphen(tl))
     ax.set_yticks(y_locs_inbound, y_labels)
 
     return
 
 
-def setLineYAxisParams(
+def configDependentYAxis(
     ax: Axes,
     side: str,
     label_location: str,
 ) -> None:
     """Set y-axis side, label, tick label location and style.
 
     Args:
@@ -136,15 +141,15 @@
 
     # Move yaxis label to upper-left or -right
     relocateYAxisLabel(ax, side=label_location)
 
     return
 
 
-def setLineXAxisParams(
+def configIndependentXAxis(
     ax: Axes,
     pad_side: str,
     minor_ticks_on: bool = True,
     n_minortick_subdivisions: int = None,
 ):
     """Set x-axis padding, label, tick label location and style.
 
@@ -164,23 +169,18 @@
     # Set Major ticks. Make major ticks that are wider than span of the data invisible.
     makeOutOfRangeXTicksInvisible(ax)
 
     if minor_ticks_on is True:
         # Turn on minor ticks and set frequency between major ticks
         addInnerMinorTicks(ax, n_minortick_subdivisions)
 
-    # Add minor tick(s) if outer limits of data are NOT on major ticks. Unlike
-    # minor ticks that are in-between major ticks, the outer minor ticks are not
-    # optional.
-    addOuterMinorTicks(ax)
-
     return
 
 
-def setBarXAxisParams(ax: Axes, side: str) -> Axes:
+def configDepdendentXAxis(ax: Axes, side: str) -> Axes:
     """Set default x-axis params for a bar chart.
 
     Args:
         ax (Axes): _description_
         side (str): ["top" | "bottom"] Which side the x-axis should be on.
 
     Returns:
@@ -205,15 +205,15 @@
 
     # Move x-axis label to top
     ax.xaxis.set_label_position(axis_label_pos)
 
     return ax
 
 
-def setBarYAxisParams(ax: Axes) -> Axes:
+def configIndependentYAxis(ax: Axes) -> Axes:
     ax.yaxis.set_tick_params(length=0)
 
     # TODO: Move ytick label baseline to left of plot area and align to left.
     for label in ax.yaxis.get_ticklabels():
         label.set_verticalalignment("center")
         label.set_horizontalalignment("right")
 
@@ -414,16 +414,18 @@
         y_lims(list): y data limits [min, max]
     """
     x_lims = [0, 0]
     y_lims = [0, 0]
     lines = ax.get_lines()
     if len(lines) == 0:
         # If plot is a patch plot (no lines)
-        patches = getAxPatches(ax)
-        # TODO: Fill in this part
+        patch_likes = getFilledAreas(ax)
+        x_lims, y_lims = getPatchBounds(patch_likes, ax)
+        x_lims = list(x_lims)
+        y_lims = list(y_lims)
     else:
         for line in lines:
             xdat = line.get_xdata()
             ydat = line.get_ydata()
 
             # extract data from MaskedArrays
             if isinstance(xdat, MaskedArray):
@@ -447,20 +449,69 @@
                 y_lims[0] = min_y
             if max_y > y_lims[1]:
                 y_lims[1] = max_y
 
     return x_lims, y_lims
 
 
-def getAxPatches(ax: Axes) -> list[PolyCollection]:
+def getFilledAreas(ax: Axes) -> list[PolyCollection | BarContainer]:
+    """Get filled areas, such as a PolyCollection or BarContainer."""
     children = ax.get_children()
-    patches = [child for child in children if isinstance(child, PolyCollection)]
+    children_types = [type(child) for child in children]
+    containers = ax.containers
+    container_types = [type(container) for container in containers]
+    if PolyCollection in children_types:
+        patches = [
+            child for child in children if isinstance(child, PolyCollection)
+        ]
+    elif BarContainer in container_types:
+        patches = [c for c in containers if isinstance(c, BarContainer)]
+
     return patches
 
 
+def getPatchBounds(
+    patches: list[PolyCollection | BarContainer],
+    ax: Axes,
+) -> Tuple[ndarray[float]]:
+    """Get bounds for a list of PolyCollections or BarContainer.
+
+    Args:
+        patches (list[PolyCollection  |  Patch]): List of PolyCollections or Patches.
+        ax (Axes): Used to get data transform.
+
+    Returns:
+        x_bounds (ndarray[float]): X-axis bounds of data, in data coordinates.
+        y_bounds (ndarray[float]): Y-axis bounds of data, in data coordinates.
+    """
+    trans = ax.transData
+
+    # Different commands for different types of patches. Assumes all entries in
+    # patches are same type.
+    if isinstance(patches[0], PolyCollection):
+        bboxes = [p.get_tightbbox() for p in patches]
+    elif isinstance(patches[0], BarContainer):
+        # Get extends from a bar container (vice list of Rectangles) to avoid using
+        # rectangles unrelated to the data series in a bar chart.
+        bboxes = []
+        for patch_group in patches:
+            bboxes.extend([p.get_extents() for p in patch_group])
+
+    # transform bboxes to data frame
+    bounds = stack([trans.inverted().transform(bbox) for bbox in bboxes])
+    x_min = amin(bounds[:, 0, 0])
+    x_max = amax(bounds[:, 1, 0])
+    y_min = amin(bounds[:, 0, 1])
+    y_max = amax(bounds[:, 1, 1])
+    x_bounds = array([x_min, x_max])
+    y_bounds = array([y_min, y_max])
+
+    return x_bounds, y_bounds
+
+
 def getInBoundsTickPos(ax: Axes) -> Tuple[list[ndarray], list[ndarray]]:
     """Get major tick locations that are within axis limits.
 
     Args:
         ax (Axes): _description_
 
     Returns:
@@ -612,29 +663,33 @@
     if leg is None:
         # Return early if ax doesn't have legend
         return ax
 
     # Change line colors
     leg_lines = leg.get_lines()
     plot_lines = ax.get_lines()
-    for pline, lline in zip(plot_lines, leg_lines):
-        new_color = pline.get_color()
-        lline.set_color(new_color)
+    if len(leg_lines) > 0:
+        for pline, lline in zip(plot_lines, leg_lines):
+            new_color = pline.get_color()
+            lline.set_color(new_color)
 
     # Change patch colors
     leg_patches = leg.get_patches()
-    # Patches are not stored separately in ax (like lines are), so need to get
-    # all children, then filter out from there.
-    all_children = ax.get_children()
-    patch_indices = where([isinstance(c, PolyCollection) for c in all_children])
-    patch_children = [all_children[indx] for indx in list(*patch_indices)]
-    for ppatch, lpatch in zip(patch_children, leg_patches):
-        new_color = ppatch.get_facecolor()
-        lpatch.set_facecolor(new_color)
-        lpatch.set_edgecolor(new_color)
+    if len(leg_patches) > 0:
+        # Patches can be different types (eg PolyCollection or BarContainer)
+        plot_patches = getFilledAreas(ax)
+
+        for ppatch, lpatch in zip(plot_patches, leg_patches):
+            if isinstance(ppatch, BarContainer):
+                new_color = plt.getp(ppatch[0], "facecolor")
+            elif isinstance(ppatch, PolyCollection):
+                new_color = ppatch.get_facecolor()
+
+            lpatch.set_facecolor(new_color)
+            lpatch.set_edgecolor(new_color)
 
     return ax
 
 
 def replaceMinusWithHyphen(text: Text) -> Text:
     """Replace all minus signs chr(8722) with hyphens chr(45)."""
     t = text._text
@@ -670,31 +725,14 @@
     for i in range(num_series):
         line = lines[i * lines_per_series + 4]
         line.set_color("black")
 
     return ax
 
 
-def fillArea(ax: Axes) -> Axes:
-    """Replaces lines in ax with filled areas between y-values and 0."""
-    lines = ax.get_lines()
-    for line in lines:
-        x_data = line.get_xdata()
-        y_data = line.get_ydata()
-        color = line.get_color()
-        poly = ax.fill_between(x_data, y_data, color=color)
-        # By default the fill area is zorder=1, which puts it behind grid lines.
-        # Move to zorder=2, which is same as default lines.
-        poly.set_zorder(2)
-        # Set line to invisible.
-        line.set_linestyle("")
-
-    return ax
-
-
 def plotZeroPt(ax: Axes, marker_size: float) -> Axes:
     """Add a black dot marker at 0,0 on a plot."""
     ax.plot(
         0,
         0,
         marker=".",
         markersize=marker_size,
@@ -709,7 +747,49 @@
     # only move spine if there is no data beneath bottom major tick
     major_tick_locs = ax.yaxis.get_majorticklocs()
     _, y_lims = getDataLimits(ax)
     if min(y_lims) >= min(major_tick_locs):
         ax.spines["bottom"].set_position(("data", min(major_tick_locs)))
 
     return ax
+
+
+def setMajorGrids(ax: Axes, axis: str) -> Axes:
+    """Set major grid style and color.
+
+    Args:
+        ax (Axes): Matplotlib Axes.
+        axis (str): ["x" | "y"] Which major grid lines will be visible.
+
+    Returns:
+        Axes: Matplotlib Axes.
+    """
+    assert axis in [
+        "x",
+        "y",
+    ], "Value of axis not recognized. Must be 'x' or 'y'."
+
+    if axis == "x":
+        opposite_axis = "y"
+    else:
+        opposite_axis = "x"
+
+    color_map = loadColorMap()
+
+    ax.grid(
+        which="major",
+        axis=axis,
+        color=color_map["grid"]["grid_gray"],
+        zorder=1,
+        clip_on=True,
+    )
+    ax.grid(which="major", axis=opposite_axis, visible=False)
+
+    return ax
+
+
+def PutBarsInFront(ax: Axes) -> Axes:
+    """Move bars in bar chart to zorder = 2."""
+    bar_containers = [c for c in ax.containers if isinstance(c, BarContainer)]
+    plt.setp(bar_containers, zorder=2)
+
+    return ax
```

### Comparing `econoplots-0.1.3/econoplots.egg-info/PKG-INFO` & `econoplots-0.2.0/econoplots.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.3
+Version: 0.2.0
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.3/pyproject.toml` & `econoplots-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.3/tests/test_converter.py` & `econoplots-0.2.0/tests/test_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from matplotlib import pyplot as plt
 from numpy import arange, array, cos, max, min, sin
 
 # Econoplots Imports
 from econoplots.converter import convert2Econo
 
 # %% Make data
-x = arange(-1, 1, 0.1)
-y = array([1.1 * sin(x), 2 * cos(x), sin(x + 0.2)]).T
+x = arange(-1, 1, 0.2)
+y = array([3.1 * sin(x), 2 * cos(x), sin(x + 0.2)]).T
 print(f"min(x) = {min(x)}")
 print(f"max(x) = {max(x)}")
 print(f"min(y) = {min(y)}")
 print(f"max(y) = {max(y)}")
 
 # %% Test line converter function
 fig, ax_line = plt.subplots()
@@ -27,15 +27,15 @@
 ax_line.legend()
 
 ax_new = convert2Econo(deepcopy(ax_line))
 # %% Test line convert with 0,0 dot
 ax_new = convert2Econo(deepcopy(ax_line), zero_dot=True)
 
 
-# %% Test fill converter
+# %% Test line fill converter
 fig, ax_fill = plt.subplots()
 ax_fill.fill_between(x, y[:, 0], label="der", color="green")
 # ax_line.plot(x, y, color="red", label=["a", "b", "c"])
 ax_fill.set_xlabel("X label")
 ax_fill.set_ylabel("Y label")
 ax_fill.legend(loc="center")
 
@@ -62,10 +62,23 @@
     labels=["seriesA", "sB", "Another Series"],
     patch_artist=True,
     showfliers=False,
 )
 ax_box.set_xlabel("X Label, showfliers=False")
 
 ax_new = convert2Econo(ax_box, ax_type="hbox")
+# %% Test bar converter (vertical)
+x_bar = [1, 2, 3, 4]
+y_bar = [3, 5, 7, 1.1]
+fig, ax_bar = plt.subplots()
+ax_bar.bar(x_bar, y_bar, label="series A")
+ax_bar.legend(loc="center")
+ax_new = convert2Econo(ax_bar, ax_type="bar")
+# %% Test bar converter (horizontal)
+x_bar = [1, 2, 3, 4]
+y_bar = [3, 5, 7, 1.1]
+fig, ax_hbar = plt.subplots()
+ax_hbar.barh(x_bar, y_bar)
+ax_new = convert2Econo(ax_hbar, ax_type="bar", orientation="horizontal")
 # %% done
 plt.show()
 print("done")
```

### Comparing `econoplots-0.1.3/tests/test_utils.py` & `econoplots-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

