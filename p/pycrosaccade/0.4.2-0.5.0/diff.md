# Comparing `tmp/pycrosaccade-0.4.2.tar.gz` & `tmp/pycrosaccade-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrosaccade-0.4.2.tar", last modified: Wed Nov 30 08:00:23 2022, max compression
+gzip compressed data, was "pycrosaccade-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycrosaccade-0.4.2.tar` & `pycrosaccade-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0       66 2022-11-09 15:30:31.779249 pycrosaccade-0.4.2/.gitattributes
--rw-r--r--   0        0        0       18 2022-11-30 07:59:53.369369 pycrosaccade-0.4.2/.gitignore
--rw-r--r--   0        0        0     6292 2022-11-09 15:30:31.779401 pycrosaccade-0.4.2/README.md
--rw-r--r--   0        0        0      876 2022-11-30 07:59:50.235514 pycrosaccade-0.4.2/README_raw.md
--rw-r--r--   0        0        0 15049260 2022-11-09 15:30:31.805858 pycrosaccade-0.4.2/data/sub_1.asc
--rw-r--r--   0        0        0 14342618 2022-11-09 15:30:31.828800 pycrosaccade-0.4.2/data/sub_2.asc
--rw-r--r--   0        0        0 14921433 2022-11-09 15:30:31.852162 pycrosaccade-0.4.2/data/sub_3.asc
--rw-r--r--   0        0        0    33429 2022-11-09 15:30:31.885189 pycrosaccade-0.4.2/plot.png
--rw-r--r--   0        0        0      154 2022-11-30 07:59:42.283237 pycrosaccade-0.4.2/pycrosaccade/__init__.py
--rw-r--r--   0        0        0     8688 2022-11-30 07:31:50.382271 pycrosaccade-0.4.2/pycrosaccade/_pycrosaccade.py
--rw-r--r--   0        0        0      537 2022-11-09 15:30:31.885499 pycrosaccade-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6744 1970-01-01 00:00:00.000000 pycrosaccade-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-06-21 13:13:14.783275 pycrosaccade-0.5.0/.gitattributes
+-rw-r--r--   0        0        0       32 2023-06-21 13:13:14.783329 pycrosaccade-0.5.0/.gitignore
+-rw-r--r--   0        0        0      548 2023-07-05 12:33:32.930558 pycrosaccade-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0     7354 2023-07-05 14:43:50.136255 pycrosaccade-0.5.0/README.md
+-rw-r--r--   0        0        0     2035 2023-07-05 14:43:37.848210 pycrosaccade-0.5.0/README_raw.md
+-rw-r--r--   0        0        0 15049260 2023-06-21 13:13:14.808497 pycrosaccade-0.5.0/data/sub_1.asc
+-rw-r--r--   0        0        0 14342618 2023-06-21 13:13:14.839003 pycrosaccade-0.5.0/data/sub_2.asc
+-rw-r--r--   0        0        0 14921433 2023-06-21 13:13:14.866507 pycrosaccade-0.5.0/data/sub_3.asc
+-rw-r--r--   0        0        0    48389 2023-07-05 14:43:49.929332 pycrosaccade-0.5.0/defaults.png
+-rw-r--r--   0        0        0    35299 2023-07-05 14:43:49.238167 pycrosaccade-0.5.0/plot.png
+-rw-r--r--   0        0        0      155 2023-07-05 12:33:19.536607 pycrosaccade-0.5.0/pycrosaccade/__init__.py
+-rw-r--r--   0        0        0     9613 2023-07-05 12:42:41.558368 pycrosaccade-0.5.0/pycrosaccade/_pycrosaccade.py
+-rw-r--r--   0        0        0      530 2023-07-05 12:33:17.394436 pycrosaccade-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    51220 2023-07-05 14:43:50.135343 pycrosaccade-0.5.0/thres3.png
+-rw-r--r--   0        0        0     7799 1970-01-01 00:00:00.000000 pycrosaccade-0.5.0/PKG-INFO
```

### Comparing `pycrosaccade-0.4.2/data/sub_1.asc` & `pycrosaccade-0.5.0/data/sub_1.asc`

 * *Files identical despite different names*

### Comparing `pycrosaccade-0.4.2/data/sub_2.asc` & `pycrosaccade-0.5.0/data/sub_2.asc`

 * *Files identical despite different names*

### Comparing `pycrosaccade-0.4.2/data/sub_3.asc` & `pycrosaccade-0.5.0/data/sub_3.asc`

 * *Files identical despite different names*

### Comparing `pycrosaccade-0.4.2/pycrosaccade/_pycrosaccade.py` & `pycrosaccade-0.5.0/pycrosaccade/_pycrosaccade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Extract microsaccades
 
 @author: robbertmijn
 """
-#%%
+
 from datamatrix import (
     series as srs,
     SeriesColumn,
     plot
     )
 import numpy as np
 from matplotlib import pyplot as plt
 plt.style.use('default')
 
-#%%
+
 def _round_to_odd(k):
     return 2 * int(k/2) + 1
 
-#%%
-def _find_microsaccades(xtrace, ytrace, msVthres = 6, mindur = 9, maxdur = 50, 
-                  mindist = .08, maxdist = 2, saccISI = 50, 
-                  vel_smooth = 7, pix2degree = 1/34.6, sampfreq = 1000):
+
+def _find_microsaccades(xtrace, ytrace, msVthres=6, mindur=3, maxdur=float('inf'), 
+                  mindist=0.057, maxdist=float('inf'), saccISI=100, 
+                  vel_smooth=5, pix2degree=1/34.6, sampfreq=1000):
     
     """
     desc:
         Get microsaccades for a trace of x and y coordinates for a single trial
-        Returns three lists with respectively first sample, last sample and the distance travelled during the microsaccade.
+        Returns three lists: 
+        1. first sample
+        2. last sample 
+        3. distance travelled during the microsaccade (degr. visual angle)
+        4. peak velocity (degr. visual angle per second)
         
     arguments:
         xtrace: SeriesColumn with x coordinates
         ytrace: SeriesColumn with y coordinates
         msVthres: Velocity threshold of eye movement to mark a microsaccade. Its unit is the number of median absoute deviations the velocity must deviate from the median velocity for each trial.
+            default: 6 (Engbert & Kliegl, 2003). (but 3 in Liu et al., 2021)
         mindur: minumum duration for the velocity to be above threshold for it to be considered a saccade
+            default: 3 (Engbert & Kliegl, 2003)
         maxdur: saccades longer than maxdur are not considered
-        mindist: minimum distance the gaze has to travel
-        maxdist: maximum distance the gaze has to travel
+            default: Inf
+        mindist: minimum distance (visual angle) the gaze has to travel
+            default: 0.057 (Liu et al., 2021)
+        maxdist: maximum distance (visual angle) the gaze has to travel
+            default: Inf
         saccISI: At least this many samples must pass before a new microsaccade is considered
+            default: 100 (Liu at al., 2021)
         vel_smooth: How many ms to smooth over gaze velocity
+            default: 5 ms (Engbert & Kliegl, 2003), (but 7 ms Liu at al., 2021)
         pix2degree: depending on distance to screen and resolution, how many pixels make up one degree visual angle
+            default: 1/34.6 (Wilschut & Mathot, 2022)
         sampfreq: sampling frequency
         
     """
 
     # initiate lists for start time, end time, and distance
     saccstlist = []
     saccetlist = []
+    saccdurlist = []
     saccdistlist = []
+    saccpvlist = []
     
     # get number of samples for mindur and maxdur (depending on sampfreq)
-    mindur = max(1, int(mindur * sampfreq/1000))
-    maxdur = max(1, int(maxdur * sampfreq/1000))
+    mindur = max(1, int(mindur * sampfreq/1000))    
+    if maxdur != float('inf'):
+        maxdur = max(1, int(maxdur * sampfreq/1000))
+
     vel_smooth = max(1, _round_to_odd(vel_smooth * sampfreq/1000))
-    dist_margin = max(1, int(5 * sampfreq/1000))
     
-    # calculate distance from one pair of xy samples to the next pair (i.e., velocity)
-    vtrace = np.sqrt(np.square(srs.smooth(np.diff(xtrace), winlen = vel_smooth)) + 
-                     np.square(srs.smooth(np.diff(ytrace), winlen = vel_smooth)))
+    # calculate distance from one pair of xy samples to the next pair. Smooth it over 7 samples (default).
+    vtrace = srs.smooth(np.sqrt(np.square(np.diff(xtrace)) + np.square(np.diff(ytrace))), winlen = vel_smooth)
     
-    # calculate raw threshold for current trial
-    vt = np.nanmedian(np.absolute(vtrace - np.nanmedian(vtrace))) * msVthres
+    # calculate threshold for current phase
+    vt = np.nanmedian(vtrace) * msVthres
     
     # find microsaccades in the velocity trace
     ifrom = 0
     while ifrom < len(vtrace):
         
         # find first index where velocity exceeds threshold
         l = np.where(vtrace[ifrom:] > vt)[0]
@@ -80,119 +94,127 @@
         
         if len(l) == 0:
             # iend = len(vtrace)
             break
         else:
             iend = l[0] + istart
         
-        # determine distance between start and end of saccade
-        # use the median location 5 ms before and 5 ms after the saccade to calculate distance
-        saccdist = pix2degree * (np.sqrt(np.square(np.nanmedian(xtrace[istart - dist_margin:istart]) - np.nanmedian(xtrace[iend:iend + dist_margin])) + 
-                           np.square(np.nanmedian(ytrace[istart - dist_margin:istart]) - np.nanmedian(ytrace[iend:iend + dist_margin]))))
-                
+        # determine distance travelled between start and end of saccade
+        saccdist = pix2degree * vtrace[istart:iend].sum()
+        
+        # determine peak velocity between start and end of saccade
+        saccpv = pix2degree * np.nanmax(vtrace[istart:iend]) 
+        
         # append this saccade if duration and distance is within margins
         if l[0] > mindur and l[0] < maxdur and saccdist < maxdist and saccdist > mindist:
             saccstlist.append(istart)
             saccetlist.append(iend)
+            saccdurlist.append(l[0])
             saccdistlist.append(saccdist)
+            saccpvlist.append(saccpv)
             ifrom = iend + saccISI
         else:
             ifrom = iend
     
-    return np.array(saccstlist, dtype = float), np.array(saccetlist, dtype = float), np.array(saccdistlist, dtype = float)
+    return np.array(saccstlist, dtype=int), np.array(saccetlist, dtype=int), np.array(saccdurlist, dtype=int), np.array(saccdistlist, dtype=float), np.array(saccpvlist, dtype=float)
 
-#%%
-def microsaccades(dm, msVthres = 6, mindur = 9, maxdur = 50, 
-                  mindist = .08, maxdist = 2, saccISI = 50, 
-                  vel_smooth = 7, freq_smooth = 100, varname = "",
-                  pix2degree = 1/34.6, sampfreq = None):
+
+def microsaccades(dm, msVthres=6, mindur=3, maxdur=float('inf'), 
+                  mindist=0.057, maxdist=float('inf'), saccISI=100, 
+                  vel_smooth=5, varname="", pix2degree=1/34.6, sampfreq=None, freq_smooth=100):
 
     """
     desc:
         find microsaccades for all trials and phases of an experiment and adds them to the dm
         
     arguments:
         dm: DataMatrix containing data from the experiment
         
     """
-        
+    
     # extract the phases of the experiment from the dm
     phases = [c.replace("xtrace_", "") for c in dm.column_names if c.startswith("xtrace_")]
     
     for phase in phases:
-        
+        print(f'Calculating microsaccades in phase \"{phase}\"')
+
         if sampfreq is None:
             # extract sampling frequency from time
             sampfreq = int(1000/(dm["ttrace_" + phase][0,1] - dm["ttrace_" + phase][0,0]))
         else:
             pass
         
-        freq_smooth_samps = max(1, _round_to_odd(freq_smooth * sampfreq/1000))
-
-        # create new columns start times, end times and distance
+        # create new columns start times, end times, distance, and peak velocity
         dm[varname + "saccstlist_" + phase] = SeriesColumn(0)
         dm[varname + "saccetlist_" + phase] = SeriesColumn(0)
+        dm[varname + "saccdurlist_" + phase] = SeriesColumn(0)
         dm[varname + "saccdistlist_" + phase] = SeriesColumn(0)
-        
-        # create new column for saccade frequency over time (list of zeros to start with)
-        dm[varname + "saccfreq_" + phase] = SeriesColumn(depth = dm["xtrace_" + phase].depth)
-        dm[varname + "saccfreq_" + phase] = [0] * dm[varname + "saccfreq_" + phase].depth
+        dm[varname + "saccpvlist_" + phase] = SeriesColumn(0)
         
         # update max_depth depending on the maximum number of microsaccades we find in phases/trials
         max_depth = 0
         
+        freq_smooth_samps = max(1, _round_to_odd(freq_smooth * sampfreq/1000))
+        # create new column for saccade frequency over time (list of zeros to start with)
+        dm[varname + "saccfreq_" + phase] = SeriesColumn(depth = dm["xtrace_" + phase].depth)
+        dm[varname + "saccfreq_" + phase] = [0] * dm[varname + "saccfreq_" + phase].depth
+
         for i, row in enumerate(dm):
 
             # find microsaccades for each trial/phase, store start times, end times and distances
-            saccstlist, saccetlist, saccdistlist = _find_microsaccades(row["xtrace_" + phase], 
+            saccstlist, saccetlist, saccdurlist, saccdistlist, saccpvlist = _find_microsaccades(row["xtrace_" + phase], 
                                                                       row["ytrace_" + phase], 
-                                                                      msVthres = msVthres, mindur = mindur, maxdur = maxdur, 
-                                                                      mindist = mindist, maxdist = maxdist, saccISI = saccISI, 
-                                                                      vel_smooth = vel_smooth, pix2degree = pix2degree, sampfreq = sampfreq)
+                                                                      msVthres=msVthres, mindur=mindur, maxdur=maxdur, 
+                                                                      mindist=mindist, maxdist=maxdist, saccISI=saccISI, 
+                                                                      vel_smooth=vel_smooth, pix2degree=pix2degree, sampfreq=sampfreq)
             
             # update max depth if more saccades are found than previously in this trial
             max_depth = max([max_depth, len(saccstlist)])
             
             if len(saccstlist) > dm[varname + "saccstlist_" + phase].depth:
                 dm[varname + "saccstlist_" + phase].depth = len(saccstlist)
                 dm[varname + "saccetlist_" + phase].depth = len(saccetlist)
+                dm[varname + "saccdurlist_" + phase].depth = len(saccetlist)
                 dm[varname + "saccdistlist_" + phase].depth = len(saccdistlist)
- 
+                dm[varname + "saccpvlist_" + phase].depth = len(saccpvlist)
+                
             # store lists in dm
             row[varname + "saccstlist_" + phase][:len(saccstlist)] = saccstlist
             row[varname + "saccetlist_" + phase][:len(saccetlist)] = saccetlist
+            row[varname + "saccdurlist_" + phase][:len(saccetlist)] = saccetlist - saccstlist
             row[varname + "saccdistlist_" + phase][:len(saccdistlist)] = saccdistlist
-            
+            row[varname + "saccpvlist_" + phase][:len(saccpvlist)] = saccpvlist
+        
             # create a trace with saccade frequency over time
-            # set frequency to 1 at the onsets of saccades
-            row[varname + "saccfreq_" + phase][list(map(int, saccstlist))] = 1
+            # set frequency to 1 at the midpoints of saccades
+            midsacclist = [np.mean([st, et]) for st, et in zip(saccstlist, saccetlist)]
+            row[varname + "saccfreq_" + phase][list(map(int, midsacclist))] = 1
             
             # smooth signal
             row[varname + "saccfreq_" + phase] = srs.smooth(row[varname + "saccfreq_" + phase], freq_smooth_samps) * sampfreq
-        
-def plot_dist_dur(dm, phase, msVthres = 6, mindur = 9, maxdur = 50, 
-                 mindist = .08, maxdist = 2, saccISI = 50, 
-                 vel_smooth = 7, freq_smooth = 100, varname = "",
-                 pix2degree = 1/34.6, sampfreq = None, label = ""):
-
-    microsaccades(dm, msVthres, mindur, maxdur, 
-                      mindist, maxdist, saccISI, 
-                      vel_smooth, freq_smooth, varname,
-                      pix2degree, sampfreq)
-    
-    dm["saccdurlist_" + phase] = dm["saccetlist_" + phase] - dm["saccstlist_" + phase]
-    
-    dm_flat = dm["saccdistlist_" + phase, "saccdurlist_" + phase]
-    dm_flat = srs.flatten(dm_flat)
-    dm_flat = dm_flat["saccdistlist_" + phase] != np.nan
-    
-    plt.figure()
-    plt.scatter(dm_flat["saccdistlist_" + phase], dm_flat["saccdurlist_" + phase])
-    plt.title("{}, {} saccades".format(label, len(dm_flat)))
-    plt.xlabel("Distance (degree)")
-    plt.ylabel("Duration (ms)")
-    
-    plt.figure()
-    plot.trace(dm["saccfreq_" + phase])
-    plt.title("{}, {} saccades".format(label, len(dm_flat)))
-    plt.xlabel("Time since rsvp (ms)")
-    plt.ylabel("Microsaccades (Hz)")
+
+
+def ms_diagnostics(dm, phase, varname=""):
+    
+    sampfreq = int(1000/(dm["ttrace_" + phase][0,1] - dm["ttrace_" + phase][0,0]))
+
+    sacc_dm = dm[varname + "saccdistlist_" + phase, varname + "saccdurlist_" + phase, varname + "saccpvlist_" + phase]
+    sacc_dm = srs.flatten(sacc_dm)
+    sacc_dm = sacc_dm[varname + "saccdistlist_" + phase] != np.nan
+    
+    fig, axs = plt.subplots(2, 2, constrained_layout=True)
+    fig.suptitle(f"Microsaccades for ... {varname}")
+
+    axs[0,0].scatter(sacc_dm[varname + "saccdistlist_" + phase], sacc_dm[varname + "saccdurlist_" + phase])
+    axs[0,0].set_xlabel("Distance (degree)")
+    axs[0,0].set_ylabel("Duration (ms)")
+    
+    axs[0,1].scatter(sacc_dm[varname + "saccdistlist_" + phase], sacc_dm[varname + "saccpvlist_" + phase])
+    axs[0,1].set_xlabel("Distance (degree)")
+    axs[0,1].set_ylabel("Peak velocity (degree/s)")
+    
+    saccfreq = dm[varname + "saccfreq_" + phase].mean
+    axs[1,0].plot(saccfreq)
+    axs[1,0].set_xlabel("Time (ms)")
+    axs[1,0].set_ylabel("Microsaccades (Hz)")
+
+    return fig, axs
```

### Comparing `pycrosaccade-0.4.2/pyproject.toml` & `pycrosaccade-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.5"
 dynamic = ["version", "description"]
 dependencies = [
-    "python-datamatrix",
+    "datamatrix",
     "numpy"
 ]
 [project.urls]
 Documentation = "https://github.com/robbertmijn/pycrosaccade"
 Source = "https://github.com/robbertmijn/pycrosaccade"
```

