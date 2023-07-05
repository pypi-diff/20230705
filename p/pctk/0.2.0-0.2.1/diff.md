# Comparing `tmp/pctk-0.2.0.tar.gz` & `tmp/pctk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pctk-0.2.0.tar", last modified: Wed Jul  5 11:53:45 2023, max compression
+gzip compressed data, was "pctk-0.2.1.tar", last modified: Wed Jul  5 20:18:21 2023, max compression
```

## Comparing `pctk-0.2.0.tar` & `pctk-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     2289 2023-03-31 07:01:57.000000 pctk-0.2.0/LICENSE
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 11:53:45.436128 pctk-0.2.0/PKG-INFO
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     7943 2023-07-03 16:28:04.000000 pctk-0.2.0/README.md
--rw-rw-r--   0 mponce    (1000) mponce    (1000)      912 2023-07-05 11:53:10.000000 pctk-0.2.0/pyproject.toml
--rw-rw-r--   0 mponce    (1000) mponce    (1000)       38 2023-07-05 11:53:45.436128 pctk-0.2.0/setup.cfg
--rw-rw-r--   0 mponce    (1000) mponce    (1000)       92 2023-07-04 17:32:10.000000 pctk-0.2.0/setup.py
-drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.432128 pctk-0.2.0/src/
-drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk/
--rwxrwxr-x   0 mponce    (1000) mponce    (1000)       58 2023-07-03 16:28:04.000000 pctk-0.2.0/src/pctk/__init__.py
-drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk/cmds/
--rw-rw-r--   0 mponce    (1000) mponce    (1000)        0 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/cmds/__init__.py
--rw-rw-r--   0 mponce    (1000) mponce    (1000)      656 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/cmds/animate.py
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     3424 2023-07-04 17:03:44.000000 pctk-0.2.0/src/pctk/cmds/pctk.py
--rwxrwxr-x   0 mponce    (1000) mponce    (1000)     2027 2023-07-04 08:13:30.000000 pctk-0.2.0/src/pctk/cmds/summarize_simulation.py
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     4269 2023-07-04 16:35:28.000000 pctk-0.2.0/src/pctk/config.py
--rwxrwxr-x   0 mponce    (1000) mponce    (1000)     9553 2023-07-04 17:47:37.000000 pctk-0.2.0/src/pctk/multicellds.py
--rwxrwxr-x   0 mponce    (1000) mponce    (1000)     4610 2023-07-04 16:48:21.000000 pctk-0.2.0/src/pctk/plot.py
--rwxrwxr-x   0 mponce    (1000) mponce    (1000)    17754 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/povwriter.py
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     4150 2023-07-04 16:59:37.000000 pctk-0.2.0/src/pctk/render.py
-drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk.egg-info/
--rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/PKG-INFO
--rw-rw-r--   0 mponce    (1000) mponce    (1000)      468 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/SOURCES.txt
--rw-rw-r--   0 mponce    (1000) mponce    (1000)        1 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/dependency_links.txt
--rw-rw-r--   0 mponce    (1000) mponce    (1000)      145 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/entry_points.txt
--rw-rw-r--   0 mponce    (1000) mponce    (1000)       30 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/requires.txt
--rw-rw-r--   0 mponce    (1000) mponce    (1000)        5 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/top_level.txt
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 20:18:21.984125 pctk-0.2.1/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     2289 2023-03-31 07:01:57.000000 pctk-0.2.1/LICENSE
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 20:18:21.984125 pctk-0.2.1/PKG-INFO
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     7943 2023-07-03 16:28:04.000000 pctk-0.2.1/README.md
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      912 2023-07-05 12:01:11.000000 pctk-0.2.1/pyproject.toml
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       38 2023-07-05 20:18:21.984125 pctk-0.2.1/setup.cfg
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       92 2023-07-04 17:32:10.000000 pctk-0.2.1/setup.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 20:18:21.984125 pctk-0.2.1/src/
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 20:18:21.984125 pctk-0.2.1/src/pctk/
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)       58 2023-07-03 16:28:04.000000 pctk-0.2.1/src/pctk/__init__.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 20:18:21.984125 pctk-0.2.1/src/pctk/cmds/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        0 2022-05-19 12:33:12.000000 pctk-0.2.1/src/pctk/cmds/__init__.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      656 2022-05-19 12:33:12.000000 pctk-0.2.1/src/pctk/cmds/animate.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     4119 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/cmds/pctk.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     2027 2023-07-04 08:13:30.000000 pctk-0.2.1/src/pctk/cmds/summarize_simulation.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     4268 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/config.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     9490 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/multicellds.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     4597 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/plot.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)    18040 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/povwriter.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     2182 2023-07-05 20:18:04.000000 pctk-0.2.1/src/pctk/render.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 20:18:21.984125 pctk-0.2.1/src/pctk.egg-info/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/PKG-INFO
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      468 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        1 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      145 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/entry_points.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       30 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/requires.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        5 2023-07-05 20:18:21.000000 pctk-0.2.1/src/pctk.egg-info/top_level.txt
```

### Comparing `pctk-0.2.0/LICENSE` & `pctk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pctk-0.2.0/PKG-INFO` & `pctk-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pctk
-Version: 0.2.0
+Version: 0.2.1
 Summary: PhysiCell ToolKit: a tool for handling MultiCellDS output from PhysiCell and PhysiBoSS simulations.
 Author-email: Miguel Ponce de Leon <miguel.ponce@bsc.es>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/migp11/pctk
 Project-URL: Bug Tracker, https://github.com/migp11/pctk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pctk-0.2.0/README.md` & `pctk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pctk-0.2.0/pyproject.toml` & `pctk-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pctk"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
      {name = "Miguel Ponce de Leon", email = "miguel.ponce@bsc.es"},
 ]
 description = "PhysiCell ToolKit: a tool for handling MultiCellDS output from PhysiCell and PhysiBoSS simulations."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "BSD 3-Clause License"}
```

### Comparing `pctk-0.2.0/src/pctk/cmds/animate.py` & `pctk-0.2.1/src/pctk/cmds/animate.py`

 * *Files identical despite different names*

### Comparing `pctk-0.2.0/src/pctk/cmds/pctk.py` & `pctk-0.2.1/src/pctk/cmds/pctk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,55 @@
 import sys
+import re
 import argparse
 from pctk import plot
 from pctk import render
 from pctk import config
+from pctk.povwriter import create_defulat_config
 
 
 
+def parse_index_string(strn_idxs):
+    index_list = []    
+    pattern_slices = re.compile("(\d*):(\d*):(\d*)")
+    pattern_indexes = re.compile("(\d+)(,\d+)*")
+    pattern_all = re.compile("^all$")
+    
+    match = re.search(pattern_slices, strn_idxs)
+    if match:
+        from_idx = int(match.group(1))
+        to_idx = int(match.group(2))
+        inc = int(match.group(3))
+        index_list = list(range(from_idx, to_idx, inc))
+    elif re.search(pattern_indexes, strn_idxs):
+        index_list = [int(i) for i in strn_idxs.split(",")]
+    
+    return index_list
+
 
-def main(): 
+def main():
+    
     parser = argparse.ArgumentParser(description="PhysiCell Tool Kit for handling and processing Physicell outputs")
+    parser.add_argument("output_folder", action="store", help="Folder where the simulation output is stored")
+    parser.add_argument("--format", action="store", dest="format", choices=("physicell", "physiboss"),
+                        help="Format of the input data", default="physicell")
     subparser = parser.add_subparsers(dest='command', help='sub-command help')
-    
+        
     plot_parser = subparser.add_parser('plot-time-course',
                                         description="Plot total cell grouped as Alive/Necrotic/Apoptotic vs Time")
-    plot_parser.add_argument("output_folder", action="store", help="Folder where the simulation output is stored")
-    plot_parser.add_argument("--format", action="store", dest="format", choices=("physicell", "physiboss"),
-                        help="Format of the input data", default="physicell")
+    
+    
     plot_parser.add_argument("--figout", action="store", dest="fig_fname", default="./cell_vs_time.png",
                         help="File name to save the plot")    
     plot_parser.add_argument("--csvout", action="store", dest="csv_fname", default=None,
                         help="File name to store the summary table used for the plot")
 
 
     pov_parser = subparser.add_parser('povray')
     pov_parser.add_argument("--config", action="store", help="XML configuration file for creating pov files")
-    pov_parser.add_argument("--format", action="store", dest="format", choices=("physicell", "physiboss"),
-                        help="Format of the input data", default="physicell")
     pov_parser.add_argument("--render",  action='store_true',
                         help="Render the .pov files into .png. Requires povray ({povray_link})")
     pov_parser.add_argument("--width", action="store", dest="width", type=int, default=2160, 
                         help="Width for povray rendered image")
     pov_parser.add_argument("--height", action="store", dest="height", type=int, default=2160, 
                         help="Heigh for povray rendered image")
     pov_parser.add_argument("--cpus", action="store", dest="cpus", type=int, default=4, 
@@ -45,19 +65,21 @@
     
 
     args = parser.parse_args()
     if args.command == "plot-time-course":
         plot.plot_time_course(args.output_folder, fig_fname=args.fig_fname, csv_fname=args.csv_fname, format=args.format)
     elif args.command == "povray":
         if args.config_out:
-            with open(args.config_out, "w") as fh:
-                print(f"Writing default POV-write config into {args.config_out}.")
-                fh.writelines(config.DEFAULT_XML)
+            print(f"Writing default POV-write config into {args.config_out}.")
+            create_defulat_config(args.config_out, args.output_folder)
         else:
             if args.config:
-                render.write_pov_files(args)
+                index_list = parse_index_string(args.strn_idxs)
+                render.write_pov_files(args.config, index_list=index_list, format=args.format,
+                                       num_of_threads=args.cpus, render=args.render, 
+                                       width=args.width, height=args.height)
             else:
                 print("Error: --config is required parameter")
                 pov_parser.print_help()
     else:
         parser.parse_args(["--help"])
-        sys.exit(0)
+        sys.exit(0)
```

### Comparing `pctk-0.2.0/src/pctk/cmds/summarize_simulation.py` & `pctk-0.2.1/src/pctk/cmds/summarize_simulation.py`

 * *Files identical despite different names*

### Comparing `pctk-0.2.0/src/pctk/config.py` & `pctk-0.2.1/src/pctk/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
             'nuclear':   [0.125, 0.06765, 0.018625],
             'finish':    [0.01, 0.5, 0.1]
         } 
     }
 
 
 DEFAULT_XML = """<?xml version="1.0" encoding="UTF-8"?>
-
 <povwriter_settings>
 	<camera>
 		<distance_from_origin units="micron">750</distance_from_origin>
 		<xy_angle>3.92699081699</xy_angle> <!-- 5*pi/4 -->
 		<yz_angle>1.0471975512</yz_angle> <!-- pi/3 --> 
 	</camera>
```

### Comparing `pctk-0.2.0/src/pctk/multicellds.py` & `pctk-0.2.1/src/pctk/multicellds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
-import json
 import glob
 import pandas as pd
-import scipy
 from scipy.io import loadmat    
 import xml.etree.ElementTree as ET
 
 from .config import phases_dict as default_phases_dict
 from .config import phase_grouping as default_phase_grouping
 
 __author__ = "Miguel Ponce de Leon"
 __copyright__ = "Copyright 2020, PhysiCell ToolKit project"
 __credits__ = ["Miguel Ponce de Leon"]
-__license__ = "GPL 3.0"
-__version__ = "0.1.0"
+__license__ = "BSD 3-Clause"
+__version__ = "0.2.1"
 __maintainer__ = "Miguel Ponce de Leon"
 __email__ = "miguel.ponce@bsc.es"
 __status__ = "dev"
 
 
 class Metadata(object):
     def __init__(self, tree):
@@ -252,16 +250,14 @@
         for xml_fname in xml_list:
             tree = ET.parse(xml_fname)
             microenv_matrix = self.get_microenvironment_matrix(tree)
             time = self.get_time(tree)
             yield (time, microenv_matrix)
 
     def get_cells_summary_frame(self, phase_col="current_phase"):
-    "requests",
-    "importlib-metadata", 
         cell_phases = list(set(self.phase_grouping.values()))
         num_of_files = self.cells_file_count()
 
         # Initializing a Pandas Databrafe to store the data
         index = range(num_of_files)
         columns = ["time"] + cell_phases
         df_time_course = pd.DataFrame(columns=columns, dtype=int, index=index, data=0)
```

### Comparing `pctk-0.2.0/src/pctk/plot.py` & `pctk-0.2.1/src/pctk/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
-import os, re, sys
-import glob, json
-import argparse
+import os
+import glob
 
 import numpy as np
 import pandas as pd
 
 import matplotlib.pyplot as plt
 from pctk import multicellds 
 from pctk.config import default_cell_colors
 
     
 
-def pb_output_iterator(data_folder, sep=";"):
-    globing = os.path.join(data_folder, "cells_[0-9]*.txt")
+def pb_output_iterator(output_folder, sep=";"):
+    globing = os.path.join(output_folder, "cells_[0-9]*.txt")
     for fname in sorted(glob.glob(globing)):
         df = pd.read_csv(fname, sep=sep)
         t = df.Time[0]
         yield (t, df)
 
-def count_pb_files(data_folder):
-    globing = os.path.join(data_folder, "cells_[0-9]*.txt")
+def count_pb_files(output_folder):
+    globing = os.path.join(output_folder, "cells_[0-9]*.txt")
     return len(glob.glob(globing))
 
 
 def get_timeserie_mean(mcds, filter_alive=True):
     time = []
     values = []
     filter_alive = True
@@ -78,37 +77,37 @@
     
     # Showing legend
     ax.legend()
     ax.yaxis.grid(True)
 
 
 
-def plot_time_course(data_folder, fig_fname="time_course.png", csv_fname="time_course.csv", format="physicell"):
+def plot_time_course(output_folder, fig_fname="time_course.png", csv_fname="time_course.csv", format="physicell"):
     phases_dict = multicellds.default_phases_dict
     phase_grouping = multicellds.default_phase_grouping
     print(phases_dict)
     # Globing output files according to the output format specified
     if format == 'physicell':
         phase_col = "current_phase"
-        mcds = multicellds.MultiCellDS(output_folder=data_folder)
+        mcds = multicellds.MultiCellDS(output_folder=output_folder)
         df_iterator = mcds.cells_as_frames_iterator()
         num_of_files = mcds.cells_file_count()
     elif format == 'physiboss':
         phase_col = "phase"
-        df_iterator = pb_output_iterator(data_folder)
-        num_of_files = count_pb_files(data_folder)
+        df_iterator = pb_output_iterator(output_folder)
+        num_of_files = count_pb_files(output_folder)
     
     # Initializing a Pandas Databrafe to store the data
     
     cell_columns = ["time", "alive", "apoptotic", "necrotic"]
 
     data = np.zeros((num_of_files, 4), dtype=int)
     df_time_course = pd.DataFrame(columns=cell_columns, data=data)
 
-    print("Reading cell_output files from %i input files from %s" % (num_of_files, data_folder))
+    print("Reading cell_output files from %i input files from %s" % (num_of_files, output_folder))
     # Iterating over all cell_output files
     for i, (t, df) in enumerate(df_iterator):
         print("\tProcessing time step: %.0f" % t)
 
         # Rename the phases integer codes using the phases_dict as the mapping
         s = df[phase_col]
         s.replace(to_replace=phases_dict, inplace=True)
```

### Comparing `pctk-0.2.0/src/pctk/povwriter.py` & `pctk-0.2.1/src/pctk/povwriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 # coding: utf-8
 import os
 import numpy as np
 from math import pi, sin, cos
-
 import xml.etree.ElementTree as ET
 
+from pctk.config import DEFAULT_XML
 from pctk.config import phase_grouping 
 from pctk.config import phases_dict
 from pctk.config import default_pov_colors
 
 
-
 __author__ = "Miguel Ponce de Leon"
 __copyright__ = "Copyright 2020, PhysiCell ToolsKit project"
 __credits__ = ["Miguel Ponce de Leon"]
-__license__ = "GPL 3.0"
-__version__ = "0.1.0"
+__license__ = "BSD 3-Clause"
+__version__ = "0.2.1"
 __maintainer__ = "Miguel Ponce de Leon"
 __email__ = "miguel.ponce@bsc.es"
 __status__ = "dev"
 
 
 class InvalidFormatException(Exception):
     def __init__(self, format):
@@ -58,19 +57,19 @@
         out = self.coefficients[3]
         for i in range(3):
             out += point[i] * self.coefficients[i]
         return out
 
 
 class PC_Options:
-    def __init__(self, folder="sample", filebase="output", format="physicell",
-                 time_index=0, camera_distance=1500, nuclear_offset=0.1, cell_bound=750, 
+    def __init__(self, output_folder="output", filebase="output", format="physicell",
+                 time_index=0, nuclear_offset=0.1, cell_bound=750, 
                  threads=1, use_standard_colors=True):
 
-        self.folder = folder
+        self.output_folder = output_folder
         self.filebase = filebase
         self.format = format
         self.time_index = time_index
         self.filename = self.create_file_name(time_index)
         
         self.nuclear_offset = nuclear_offset
         self.cell_bound = cell_bound
@@ -83,20 +82,20 @@
         elif self.format == 'physiboss':
             self.columns_index_dict = { "cyto_radius": 4, "cell_type": 11, "phase": 13, "nuc_radius": 6}
         else:
             raise InvalidFormatException(self.format)
 
     def create_file_name(self, index):
         if self.format == 'physicell':
-            fname  = "{base_name}{:08}_cells_physicell.mat".format(index, base_name=self.filebase)
+            fname  = f"{self.filebase}{index:08}_cells_physicell.mat"
         elif self.format == 'physiboss':
-            fname  = "cells_{:05}.txt".format(index)
+            fname  = f"cells_{index:05}.txt"
         else:
             fname = None
-        fname = os.path.join(self.folder, fname)
+        fname = os.path.join(self.output_folder, fname)
         return fname
 
 
 class POV_Options():
     
     def __init__(self, x_size=2000, y_size=2000, z_size=2000):
         
@@ -151,15 +150,15 @@
     def load_config_file(self, fname):
         
         tree = ET.parse(fname)
         root = tree.getroot()
         
         # Parsing save node
         node = root.find("save")
-        self.options.folder = node.find("folder").text
+        self.options.output_folder = node.find("folder").text
         self.options.filebase = node.find("filebase").text
         self.options.time_index = int(node.find("time_index").text)
         self.options.filename = self.options.create_file_name(self.options.time_index)
 
         # Parsing options node
         node = root.find("options")
         self.options.nuclear_offset = float(node.find("nuclear_offset").text)
@@ -415,17 +414,16 @@
         
         pov_fname = fname[:-4] + ".pov"
         with open(pov_fname, 'w') as fh:
             print("Creating file %s for output ... " % pov_fname)
             self._write_pov_header(fh)       
             print("Writing %i cells ... " % mat.shape[0])
             self._write_all_cells(fh, mat)
-            return pov_fname
         
-        return None
+        return pov_fname
 
     def read_cells_file(self, fname):
         if self.format == 'physicell':
             from scipy.io import loadmat
             mat = loadmat(fname)['cells'].T
             return mat
         elif self.format == 'physiboss':
@@ -438,13 +436,21 @@
                 # Removing time storing column
                 data = data[:,1:]
             return data
         else:
             raise InvalidFormatException(self.format)
 
 
+def create_defulat_config(xml_fname, output_folder):
+    root = ET.fromstring(DEFAULT_XML)
+    node = root.find('save')
+    folder_node = node.find('folder')
+    folder_node.text = output_folder
+    with open(xml_fname, "w") as fh:
+        fh.writelines(ET.tostring(root, encoding='unicode'))
+
 
 def standard_pigment_and_finish_function():
     pass
 
 def my_pigment_and_finish_function():
-    pass
+    pass
```

### Comparing `pctk-0.2.0/src/pctk.egg-info/PKG-INFO` & `pctk-0.2.1/src/pctk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pctk
-Version: 0.2.0
+Version: 0.2.1
 Summary: PhysiCell ToolKit: a tool for handling MultiCellDS output from PhysiCell and PhysiBoSS simulations.
 Author-email: Miguel Ponce de Leon <miguel.ponce@bsc.es>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/migp11/pctk
 Project-URL: Bug Tracker, https://github.com/migp11/pctk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

