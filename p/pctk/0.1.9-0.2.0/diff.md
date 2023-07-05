# Comparing `tmp/pctk-0.1.9.tar.gz` & `tmp/pctk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pctk-0.1.9.tar", last modified: Thu Jun  9 10:17:13 2022, max compression
+gzip compressed data, was "pctk-0.2.0.tar", last modified: Wed Jul  5 11:53:45 2023, max compression
```

## Comparing `pctk-0.1.9.tar` & `pctk-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.734331 pctk-0.1.9/
--rwxr--r--   0 mponce    (1001) users      (100)    35149 2020-03-16 17:25:13.000000 pctk-0.1.9/LICENSE
--rw-r--r--   0 mponce    (1001) users      (100)     6779 2022-06-09 10:17:13.730331 pctk-0.1.9/PKG-INFO
--rw-r--r--   0 mponce    (1001) users      (100)     6282 2022-06-09 10:11:44.000000 pctk-0.1.9/README.md
--rw-r--r--   0 mponce    (1001) users      (100)       38 2022-06-09 10:17:13.734331 pctk-0.1.9/setup.cfg
--rw-r--r--   0 mponce    (1001) users      (100)     1162 2022-06-09 10:13:54.000000 pctk-0.1.9/setup.py
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.730331 pctk-0.1.9/src/
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.730331 pctk-0.1.9/src/pctk/
--rwxr--r--   0 mponce    (1001) users      (100)       58 2022-06-09 10:16:19.000000 pctk-0.1.9/src/pctk/__init__.py
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.730331 pctk-0.1.9/src/pctk/cmds/
--rw-r--r--   0 mponce    (1001) users      (100)        0 2022-04-04 20:21:47.000000 pctk-0.1.9/src/pctk/cmds/__init__.py
--rw-r--r--   0 mponce    (1001) users      (100)      656 2022-04-04 15:52:15.000000 pctk-0.1.9/src/pctk/cmds/animate.py
--rwxr-xr-x   0 mponce    (1001) users      (100)     4637 2022-06-02 14:28:54.000000 pctk-0.1.9/src/pctk/cmds/plot_time_course.py
--rwxr-xr-x   0 mponce    (1001) users      (100)     3516 2022-05-23 13:53:35.000000 pctk-0.1.9/src/pctk/cmds/summarize_simulation.py
--rw-r--r--   0 mponce    (1001) users      (100)     4047 2022-05-23 14:10:26.000000 pctk-0.1.9/src/pctk/cmds/write_pov_files.py
--rw-r--r--   0 mponce    (1001) users      (100)     1523 2022-04-05 20:58:22.000000 pctk-0.1.9/src/pctk/config.py
--rwxr-xr-x   0 mponce    (1001) users      (100)     9117 2022-06-09 09:20:42.000000 pctk-0.1.9/src/pctk/multicellds.py
--rwxr-xr-x   0 mponce    (1001) users      (100)    17754 2022-05-23 14:10:26.000000 pctk-0.1.9/src/pctk/povwriter.py
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.730331 pctk-0.1.9/src/pctk.egg-info/
--rw-r--r--   0 mponce    (1001) users      (100)     6779 2022-06-09 10:17:12.000000 pctk-0.1.9/src/pctk.egg-info/PKG-INFO
--rw-r--r--   0 mponce    (1001) users      (100)      483 2022-06-09 10:17:13.000000 pctk-0.1.9/src/pctk.egg-info/SOURCES.txt
--rw-r--r--   0 mponce    (1001) users      (100)        1 2022-06-09 10:17:12.000000 pctk-0.1.9/src/pctk.egg-info/dependency_links.txt
--rw-r--r--   0 mponce    (1001) users      (100)      118 2022-06-09 10:17:13.000000 pctk-0.1.9/src/pctk.egg-info/entry_points.txt
--rw-r--r--   0 mponce    (1001) users      (100)       38 2022-06-09 10:17:13.000000 pctk-0.1.9/src/pctk.egg-info/requires.txt
--rw-r--r--   0 mponce    (1001) users      (100)       10 2022-06-09 10:17:13.000000 pctk-0.1.9/src/pctk.egg-info/top_level.txt
-drwxr-xr-x   0 mponce    (1001) users      (100)        0 2022-06-09 10:17:13.730331 pctk-0.1.9/src/test/
--rw-r--r--   0 mponce    (1001) users      (100)        0 2022-04-04 20:13:35.000000 pctk-0.1.9/src/test/__init__.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     2289 2023-03-31 07:01:57.000000 pctk-0.2.0/LICENSE
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 11:53:45.436128 pctk-0.2.0/PKG-INFO
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     7943 2023-07-03 16:28:04.000000 pctk-0.2.0/README.md
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      912 2023-07-05 11:53:10.000000 pctk-0.2.0/pyproject.toml
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       38 2023-07-05 11:53:45.436128 pctk-0.2.0/setup.cfg
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       92 2023-07-04 17:32:10.000000 pctk-0.2.0/setup.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.432128 pctk-0.2.0/src/
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk/
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)       58 2023-07-03 16:28:04.000000 pctk-0.2.0/src/pctk/__init__.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk/cmds/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        0 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/cmds/__init__.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      656 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/cmds/animate.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     3424 2023-07-04 17:03:44.000000 pctk-0.2.0/src/pctk/cmds/pctk.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     2027 2023-07-04 08:13:30.000000 pctk-0.2.0/src/pctk/cmds/summarize_simulation.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     4269 2023-07-04 16:35:28.000000 pctk-0.2.0/src/pctk/config.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     9553 2023-07-04 17:47:37.000000 pctk-0.2.0/src/pctk/multicellds.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)     4610 2023-07-04 16:48:21.000000 pctk-0.2.0/src/pctk/plot.py
+-rwxrwxr-x   0 mponce    (1000) mponce    (1000)    17754 2022-05-19 12:33:12.000000 pctk-0.2.0/src/pctk/povwriter.py
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     4150 2023-07-04 16:59:37.000000 pctk-0.2.0/src/pctk/render.py
+drwxrwxr-x   0 mponce    (1000) mponce    (1000)        0 2023-07-05 11:53:45.436128 pctk-0.2.0/src/pctk.egg-info/
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)     8537 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/PKG-INFO
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      468 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        1 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)      145 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/entry_points.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)       30 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/requires.txt
+-rw-rw-r--   0 mponce    (1000) mponce    (1000)        5 2023-07-05 11:53:45.000000 pctk-0.2.0/src/pctk.egg-info/top_level.txt
```

### Comparing `pctk-0.1.9/src/pctk/cmds/animate.py` & `pctk-0.2.0/src/pctk/cmds/animate.py`

 * *Files identical despite different names*

### Comparing `pctk-0.1.9/src/pctk/cmds/plot_time_course.py` & `pctk-0.2.0/src/pctk/plot.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,79 +3,112 @@
 
 import os, re, sys
 import glob, json
 import argparse
 
 import numpy as np
 import pandas as pd
-from scipy.io import loadmat
 
 import matplotlib.pyplot as plt
-import seaborn as sns
-
 from pctk import multicellds 
+from pctk.config import default_cell_colors
 
-
-sns.set(style="ticks", palette="Paired")
-sns.set_context('paper')
-
-
-def create_parser():
-    parser = argparse.ArgumentParser(description="Plot total cell grouped as Alive/Necrotic/Apoptotic vs Time")
-    
-    parser.add_argument("data_folder", action="store", help="folder were the data is stored")
-    
-    parser.add_argument("--format", action="store", dest="format", choices=("physicell", "physiboss"),
-                        help="Format of the input data", default="physicell")
-
-    parser.add_argument("--figout", action="store", dest="fig_fname", default="./cell_vs_time.png",
-                        help="File name to save the plot")
-                        
-    parser.add_argument("--csvout", action="store", dest="csv_fname", default=None,
-                        help="File name to store the summary table used for the plot")
-
-    return parser
     
 
 def pb_output_iterator(data_folder, sep=";"):
     globing = os.path.join(data_folder, "cells_[0-9]*.txt")
     for fname in sorted(glob.glob(globing)):
         df = pd.read_csv(fname, sep=sep)
         t = df.Time[0]
         yield (t, df)
 
 def count_pb_files(data_folder):
     globing = os.path.join(data_folder, "cells_[0-9]*.txt")
     return len(glob.glob(globing))
 
-def main():
-   
-    parser = create_parser()
-    args = parser.parse_args()
+
+def get_timeserie_mean(mcds, filter_alive=True):
+    time = []
+    values = []
+    filter_alive = True
+    for t, df in mcds.cells_as_frames_iterator():
+        time.append(t)
+        df = df.iloc[:,3:]
+        if filter_alive:
+            mask = df['current_phase'] <= 14
+            df = df[mask]
+        values.append(df.mean(axis=0).values)
+
+    cell_columns = df.columns.tolist()
+    df = pd.DataFrame(values, columns=cell_columns)
+    df['time'] = time
+    return df[['time'] + cell_columns]
+
+
+def get_timeserie_density(mcds):
+    data = []
+    for t,m in mcds.microenvironment_as_matrix_iterator():
+        data.append((t, m[5,:].sum()))
+    df = pd.DataFrame(data=data, columns=['time', 'tnf'])
+    return df
+
+def plot_molecular_model(df_cell_variables, list_of_variables, ax1):
+
+    threshold = 0.5
+
+    for label in list_of_variables:
+        y = df_cell_variables[label]
+        time = df_cell_variables["time"]
+        ax1.plot(time, y, label="% X " + label)
+
+    ax1.set_ylabel("% X")
+    ax1.yaxis.grid(True)
+    ax1.set_xlim((0,time.values[-1]))
+    ax1.set_ylim((0,1))
+    # ax1.set_xlabel("time (min)")
+    
+def plot_cells(df_time_course, color_dict, ax, xlabel="Time (min)", ylabel="Nº of cells"):
+
+    # Alive/Apoptotic/Necrotic vs Time
+    for pheno,color in color_dict.items():
+        ax.plot(df_time_course.time, df_time_course[pheno], "-", c=color, label=pheno)
     
+    # setting axes labels
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(ylabel)
+    
+    # Showing legend
+    ax.legend()
+    ax.yaxis.grid(True)
+
+
+
+def plot_time_course(data_folder, fig_fname="time_course.png", csv_fname="time_course.csv", format="physicell"):
     phases_dict = multicellds.default_phases_dict
     phase_grouping = multicellds.default_phase_grouping
     print(phases_dict)
     # Globing output files according to the output format specified
-    if args.format == 'physicell':
+    if format == 'physicell':
         phase_col = "current_phase"
-        mcds = multicellds.MultiCellDS(output_folder=args.data_folder)
+        mcds = multicellds.MultiCellDS(output_folder=data_folder)
         df_iterator = mcds.cells_as_frames_iterator()
         num_of_files = mcds.cells_file_count()
-    elif args.format == 'physiboss':
+    elif format == 'physiboss':
         phase_col = "phase"
-        df_iterator = pb_output_iterator(args.data_folder)
-        num_of_files = count_pb_files(args.data_folder)
+        df_iterator = pb_output_iterator(data_folder)
+        num_of_files = count_pb_files(data_folder)
     
     # Initializing a Pandas Databrafe to store the data
-    columns = ["time", "live", "apoptotic", "necrotic"]
+    
+    cell_columns = ["time", "alive", "apoptotic", "necrotic"]
+
     data = np.zeros((num_of_files, 4), dtype=int)
-    df_time_course = pd.DataFrame(columns=columns, data=data)
+    df_time_course = pd.DataFrame(columns=cell_columns, data=data)
 
-    print("Reading cell_output files from %i input files from %s" % (num_of_files, args.data_folder))
+    print("Reading cell_output files from %i input files from %s" % (num_of_files, data_folder))
     # Iterating over all cell_output files
     for i, (t, df) in enumerate(df_iterator):
         print("\tProcessing time step: %.0f" % t)
 
         # Rename the phases integer codes using the phases_dict as the mapping
         s = df[phase_col]
         s.replace(to_replace=phases_dict, inplace=True)
@@ -86,55 +119,34 @@
         df_time_course.loc[i, 'time'] = t
         # group the previous phases count into the three general classes:
         # Alive, Apoptotic, Necrotic
         for k, v in counts.to_dict().items():
             if k not in phase_grouping:
                 continue
             df_time_course.loc[i, phase_grouping[k]] += v
-            
     
     print("Finish processing files")    
-    # Set time column as the dataframe index
-    sns.set_context('paper')
-    patch_color = "lightgrey"
     
+        # plot Alive vs Time
     print("Creating figure")
-    # Create a figure
     fig, ax = plt.subplots(1, 1, figsize=(8,3), dpi=300)
-    
-    # plot Alive vs Time
-    curve_params = {}
-    curve_params['live'] = {'color': '#75db75', 'label': 'Alive'}
-    curve_params['apoptotic'] = {'color': '#ef4242', 'label': 'Apoptotic'}
-    curve_params['necrotic'] = {'color':'#97723d', 'label': 'Necrotic'}
-    line_width = 2.
-    for k,pdict in curve_params.items():
-        c = pdict['color']
-        l = pdict['label']
-        ax.plot(df_time_course.time, df_time_course[k], "-", c=c, label=l, linewidth=line_width)
-    
-    # setting axes labels
-    ax.set_xlabel("Time (min)")
-    ax.set_ylabel("Nº of cells")
+    plot_cells(df_time_course, default_cell_colors, ax)
 
     ax.tick_params(axis='x', labelsize=12)
     ax.tick_params(axis='y', labelsize=12)
-    
-    # Showing legend
     ax.spines['right'].set_visible(False)
     ax.spines['top'].set_visible(False)
     ax.yaxis.grid(linestyle='dotted')
     ax.legend()
     
     # Saving fig
     fig.tight_layout()
-    fig.savefig(args.fig_fname)
-    print("Saving fig as %s" % args.fig_fname)
+    fig.savefig(fig_fname)
+    print("Saving fig as %s" % fig_fname)
     
-    if args.csv_fname:
-        df_time_course.to_csv(args.csv_fname, sep="\t")
-        print("Saving csv as %s" % args.csv_fname)
+    if csv_fname:
+        df_time_course.to_csv(csv_fname, sep="\t")
+        print("Saving csv as %s" % csv_fname)
+
 
 
-if __name__ == '__main__':
-    main()
```

### Comparing `pctk-0.1.9/src/pctk/cmds/summarize_simulation.py` & `pctk-0.2.0/src/pctk/cmds/summarize_simulation.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,67 +10,15 @@
 
 modules_path = os.path.dirname(os.path.realpath(__file__))
 modules_path = os.path.join(modules_path, 'modules')
 sys.path.append(modules_path)
 
 from multicellds import MultiCellDS
 
-def get_timeserie_mean(mcds, filter_alive=True):
-    time = []
-    values = []
-    filter_alive = True
-    for t, df in mcds.cells_as_frames_iterator():
-        time.append(t)
-        df = df.iloc[:,3:]
-        if filter_alive:
-            mask = df['current_phase'] <= 14
-            df = df[mask]
-        values.append(df.mean(axis=0).values)
-
-    cell_columns = df.columns.tolist()
-    df = pd.DataFrame(values, columns=cell_columns)
-    df['time'] = time
-    return df[['time'] + cell_columns]
-
-
-def get_timeserie_density(mcds):
-    data = []
-    for t,m in mcds.microenvironment_as_matrix_iterator():
-        data.append((t, m[5,:].sum()))
-    df = pd.DataFrame(data=data, columns=['time', 'tnf'])
-    return df
-
-def plot_molecular_model(df_cell_variables, list_of_variables, ax1):
-
-    threshold = 0.5
-
-    for label in list_of_variables:
-        y = df_cell_variables[label]
-        time = df_cell_variables["time"]
-        ax1.plot(time, y, label="% X " + label)
-
-    ax1.set_ylabel("% X")
-    ax1.yaxis.grid(True)
-    ax1.set_xlim((0,time.values[-1]))
-    ax1.set_ylim((0,1))
-    # ax1.set_xlabel("time (min)")
-    
-def plot_cells(df_time_course, color_dict, ax):
-
-    # Alive/Apoptotic/Necrotic vs Time
-    for k in color_dict:
-        ax.plot(df_time_course.time, df_time_course[k], "-", c=color_dict[k], label=k)
-    
-    # setting axes labels
-    # ax.set_xlabel("time (min)")
-    ax.set_ylabel("Nº of cells")
-    
-    # Showing legend
-    ax.legend()
-    ax.yaxis.grid(True)
+
 
 def main():
 
     color_dict = {"live": "g", "apoptotic": "r", "necrotic":"k"}
 
     instance_folder = sys.argv[1]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pctk-0.1.9/src/pctk/cmds/write_pov_files.py` & `pctk-0.2.0/src/pctk/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import argparse
 import numpy as np
 
 
 import multiprocessing as mp
 from pctk.povwriter import POVWriter
 
+povray_path = None
+
+
+
 def create_parser():
 
     povray_link = "http://www.povray.org/download/"
 
     parser = argparse.ArgumentParser(description="Render a bunch of PhysiCell output file into povray files")
     
     parser.add_argument("xml_config", action="store", help="XML configuration file")
@@ -40,50 +44,41 @@
                         help="Total CPUs availabile to run in parallel using multiprocessing")
 
     parser.add_argument("--create-config", dest="create_default_config", default=False,
                         help="Output format")
 
     return parser
 
-
 def check_povray(exec='povray'):
     global povray_path
     povray_path = shutil.which(exec)
     return (povray_path is not None)
 
-
 def local_write_pov_file(writer, idx):
     fname = writer.write_pov_file(idx)
     return fname
 
-def render_to_png(pov_fname, width, height):
-    cmd_line = f"{povray_path} -h{height} -w{width} -a {pov_fname}"
+def render_to_png(pov_fname, width, height, png_fname=None):
+    if png_fname is None:
+        png_fname = pov_fname[0:-4] + ".png"
+    cmd_line = f"{povray_path} +H{height} +W{width} +I{pov_fname} +O{png_fname}"
     exit_flag = os.system(cmd_line)
     if exit_flag != 0:
         print(f"Somthing went wrong running povray {cmd_line}. Command finished with exit flag {exit_flag}")
-
-    png_fname = pov_fname[0:-4] + ".png"
     return png_fname
 
 def animate_pngs(png_files):
     pass
 
-
-povray_path = None
-
-
-def main():
-    parser = create_parser()
-    args = parser.parse_args()
-
+def write_pov_files(args):
     if args.render:
         assert check_povray()
     
     # Loadgin XML configuration 
-    pov_writer = POVWriter(args.xml_config, format=args.format)
+    pov_writer = POVWriter(args.config, format=args.format)
 
     num_of_jobs = args.cpus
 
     index_list = []    
     pattern_slices = re.compile("(\d*):(\d*):(\d*)")
     pattern_indexes = re.compile("(\d+)(,\d+)*")
     pattern_all = re.compile("^all$")
@@ -104,25 +99,28 @@
     print(f"Start processing  {num_of_jobs} cpus")
     if num_of_jobs > 1:
 
         pool = mp.Pool(num_of_jobs)
         pov_files = [pool.apply(local_write_pov_file, args=((pov_writer,idx)))
                                         for idx in index_list]
         pool.close()
-
         print("Finished!")
         if args.render:
             png_files = []
             for fname in pov_files:
                 png = render_to_png(fname, args.width, args.height)
                 png_files.append(png)
             
             pool.close()
             #animate_pngs(png_files)
         
     else:
         for idx in index_list:
             pov_writer.write_pov_file(idx)
 
+def main():
+    parser = create_parser()
+    args = parser.parse_args()
+    write_pov_files(args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `pctk-0.1.9/src/pctk/multicellds.py` & `pctk-0.2.0/src/pctk/multicellds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 import glob
 import pandas as pd
+import scipy
 from scipy.io import loadmat    
 import xml.etree.ElementTree as ET
 
 from .config import phases_dict as default_phases_dict
 from .config import phase_grouping as default_phase_grouping
 
 __author__ = "Miguel Ponce de Leon"
@@ -111,18 +112,24 @@
         for child in cellular_info_node:
             column = child.text
             index = child.attrib["index"]
             size = int(child.attrib["size"])
             if size == 1:
                 cell_columns.append(column)
                 continue
-            for i, v in enumerate(['x', 'y', 'z']):
-                cell_columns.append(v + self._separator + column)
-                if i == size: 
-                    break
+            if size == 2:
+                for i, v in enumerate(['x', 'y']):
+                    cell_columns.append(v + self._separator + column)
+                    if i == size: 
+                        break
+            if size == 3:
+                for i, v in enumerate(['x', 'y', 'z']):
+                    cell_columns.append(v + self._separator + column)
+                    if i == size: 
+                        break
                 
                 
         return cell_columns
 
     def _get_microenvironment_columns(self):
         root = self._tree.getroot()
         node = root.find("microenvironment")
@@ -171,18 +178,21 @@
         return self._phases_dict
 
     @property
     def phase_grouping(self):
         return self._phase_grouping
 
     def _read_matlab_mat(self, fname, column):
-        stru = loadmat(fname)
-        data = stru[column]
-        return data
-
+        try:
+            stru = loadmat(fname)
+            data = stru[column]
+            return data
+        except:
+            print("cannot read mat file " + fname)
+            return None
     def get_time(self, tree):
         root = tree.getroot()
         node = root.find("metadata")
         node = node.find("current_time")
         time = int(float(node.text))
         return time
 
@@ -242,29 +252,30 @@
         for xml_fname in xml_list:
             tree = ET.parse(xml_fname)
             microenv_matrix = self.get_microenvironment_matrix(tree)
             time = self.get_time(tree)
             yield (time, microenv_matrix)
 
     def get_cells_summary_frame(self, phase_col="current_phase"):
-
+    "requests",
+    "importlib-metadata", 
         cell_phases = list(set(self.phase_grouping.values()))
         num_of_files = self.cells_file_count()
 
         # Initializing a Pandas Databrafe to store the data
         index = range(num_of_files)
         columns = ["time"] + cell_phases
         df_time_course = pd.DataFrame(columns=columns, dtype=int, index=index, data=0)
         
         for i, (time, df) in enumerate(self.cells_as_frames_iterator()):
             df_time_course.iloc[i, 0] = time
 
             # Rename the phases integer codes using the phases_dict as the mapping
             s = df[phase_col]
-            s.replace(to_replace=self.phases_dict, inplace=True)
+            s.replace(to_replace=self.phases_dict,  value=None,inplace=True)
 
             # Count the number of cells in each phase
             counts = s.value_counts()
 
             # group the previous phases count into the three general classes:
             # Alive, Apoptotic, Necrotic
             for k, v in counts.to_dict().items():
```

### Comparing `pctk-0.1.9/src/pctk/povwriter.py` & `pctk-0.2.0/src/pctk/povwriter.py`

 * *Files identical despite different names*

