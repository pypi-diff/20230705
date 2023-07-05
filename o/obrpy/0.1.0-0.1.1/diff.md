# Comparing `tmp/obrpy-0.1.0.tar.gz` & `tmp/obrpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.1.0.tar", last modified: Tue Jun 20 12:52:42 2023, max compression
+gzip compressed data, was "obrpy-0.1.1.tar", last modified: Wed Jul  5 18:21:45 2023, max compression
```

## Comparing `obrpy-0.1.0.tar` & `obrpy-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:42.009925 obrpy-0.1.0/
--rw-rw-rw-   0        0        0      283 2023-06-20 12:52:42.008923 obrpy-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:39.992206 obrpy-0.1.0/obrpy/
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.026206 obrpy-0.1.0/obrpy/ANALYSIS/
--rw-rw-rw-   0        0        0     9204 2023-05-30 09:48:03.000000 obrpy-0.1.0/obrpy/ANALYSIS/global_analysis.py
--rw-rw-rw-   0        0        0     8104 2023-06-20 08:13:22.000000 obrpy-0.1.0/obrpy/ANALYSIS/local_analysis.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.029206 obrpy-0.1.0/obrpy/SIGNAL/
--rw-rw-rw-   0        0        0     4814 2023-05-03 10:51:46.000000 obrpy-0.1.0/obrpy/SIGNAL/cross_spectrum.py
--rw-rw-rw-   0        0        0     4762 2023-06-20 07:55:06.000000 obrpy-0.1.0/obrpy/SIGNAL/spectral_shift.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.047214 obrpy-0.1.0/obrpy/UTILS/
--rw-rw-rw-   0        0        0    11916 2023-06-05 08:24:09.000000 obrpy-0.1.0/obrpy/UTILS/read_OBR.py
--rw-rw-rw-   0        0        0    11436 2023-06-19 11:27:53.000000 obrpy-0.1.0/obrpy/UTILS/utils.py
--rw-rw-rw-   0        0        0    12610 2023-06-20 08:28:47.000000 obrpy-0.1.0/obrpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-06-20 07:02:11.000000 obrpy-0.1.0/obrpy/checkouts.py
--rw-rw-rw-   0        0        0      195 2023-06-20 06:55:40.000000 obrpy-0.1.0/obrpy/clear.py
--rw-rw-rw-   0        0        0      683 2023-06-19 10:46:23.000000 obrpy-0.1.0/obrpy/fuego.py
--rw-rw-rw-   0        0        0     1347 2023-06-19 10:11:39.000000 obrpy-0.1.0/obrpy/gui.py
--rw-rw-rw-   0        0        0     1459 2023-06-20 06:56:41.000000 obrpy-0.1.0/obrpy/load.py
--rw-rw-rw-   0        0        0     7468 2023-06-19 11:20:36.000000 obrpy-0.1.0/obrpy/obr.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:41.970922 obrpy-0.1.0/obrpy/obrsdk/
--rw-rw-rw-   0        0        0    73728 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/CommandProcessor.dll
--rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/CyUSBComm.dll
--rw-rw-rw-   0        0        0   217088 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/KL2DLL32.DLL
--rw-rw-rw-   0        0        0   282624 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/LtCore.dll
--rw-rw-rw-   0        0        0 24322048 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/LtMath.dll
--rw-rw-rw-   0        0        0   110592 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/Phoenix.dll
--rw-rw-rw-   0        0        0   106496 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/RemoteInterface.dll
--rw-rw-rw-   0        0        0    57344 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_date_time-mt.dll
--rw-rw-rw-   0        0        0    77824 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_filesystem-mt.dll
--rw-rw-rw-   0        0        0    11776 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_system-mt.dll
--rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_thread-mt.dll
--rw-rw-rw-   0        0        0   756640 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/libiomp5md.dll
--rwxrwxrwx   0        0        0    66560 2023-04-25 11:55:06.000000 obrpy-0.1.0/obrpy/obrsdk/obr.exe
--rw-rw-rw-   0        0        0   466944 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ova32.dll
--rw-rw-rw-   0        0        0   100692 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ova32.lib
--rw-rw-rw-   0        0        0    28672 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ovaGUI.dll
--rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.1.0/obrpy/obrsdk.py
--rw-rw-rw-   0        0        0      972 2023-06-05 07:51:39.000000 obrpy-0.1.0/obrpy/save.py
--rw-rw-rw-   0        0        0     3214 2023-06-19 09:15:05.000000 obrpy-0.1.0/obrpy/settings.py
--rw-rw-rw-   0        0        0     3481 2023-06-20 08:20:09.000000 obrpy-0.1.0/obrpy/take_a_look.py
--rw-rw-rw-   0        0        0     1743 2023-06-19 11:08:24.000000 obrpy-0.1.0/obrpy/to_export.py
--rw-rw-rw-   0        0        0     3472 2023-06-05 08:18:45.000000 obrpy-0.1.0/obrpy/to_import.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.016205 obrpy-0.1.0/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1275 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 12:52:42.009925 obrpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2019 2023-06-20 12:52:32.000000 obrpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:52:42.006928 obrpy-0.1.0/test/
--rw-rw-rw-   0        0        0     1039 2023-06-01 11:42:02.000000 obrpy-0.1.0/test/test.py
--rw-rw-rw-   0        0        0      983 2023-06-20 08:18:30.000000 obrpy-0.1.0/test/test_dataset.py
--rw-rw-rw-   0        0        0     2576 2023-06-19 10:59:54.000000 obrpy-0.1.0/test/test_export_obrfiles.py
--rw-rw-rw-   0        0        0      624 2023-06-19 11:01:21.000000 obrpy-0.1.0/test/test_export_settings.py
--rw-rw-rw-   0        0        0      622 2023-06-19 11:11:13.000000 obrpy-0.1.0/test/test_export_slices.py
--rw-rw-rw-   0        0        0     1792 2023-06-20 10:57:12.000000 obrpy-0.1.0/test/test_obr_ini.py
--rw-rw-rw-   0        0        0      700 2023-06-19 11:12:23.000000 obrpy-0.1.0/test/test_slices.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.164417 obrpy-0.1.1/
+-rw-rw-r--   0 temis     (1000) temis     (1000)      274 2023-07-05 18:21:45.164417 obrpy-0.1.1/PKG-INFO
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.108417 obrpy-0.1.1/obrpy/
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.112417 obrpy-0.1.1/obrpy/ANALYSIS/
+-rw-rw-r--   0 temis     (1000) temis     (1000)     8987 2023-05-30 09:49:53.000000 obrpy-0.1.1/obrpy/ANALYSIS/global_analysis.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     7822 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/ANALYSIS/local_analysis.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.112417 obrpy-0.1.1/obrpy/SIGNAL/
+-rw-rw-r--   0 temis     (1000) temis     (1000)     4717 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/SIGNAL/cross_spectrum.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     4664 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/SIGNAL/spectral_shift.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.112417 obrpy-0.1.1/obrpy/UTILS/
+-rw-rw-r--   0 temis     (1000) temis     (1000)    11651 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/UTILS/read_OBR.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)    11100 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/UTILS/utils.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)    15769 2023-07-05 16:15:16.000000 obrpy-0.1.1/obrpy/__init__.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1401 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/checkouts.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      188 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/clear.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      662 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/fuego.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1305 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/gui.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1471 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/load.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     7431 2023-07-05 16:16:28.000000 obrpy-0.1.1/obrpy/obr.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.160417 obrpy-0.1.1/obrpy/obrsdk/
+-rw-rw-r--   0 temis     (1000) temis     (1000)    73728 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/CommandProcessor.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    53248 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/CyUSBComm.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)   217088 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/KL2DLL32.DLL
+-rw-rw-r--   0 temis     (1000) temis     (1000)   282624 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/LtCore.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000) 24322048 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/LtMath.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)   110592 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/Phoenix.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)   106496 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/RemoteInterface.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    57344 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/boost_date_time-mt.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    77824 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/boost_filesystem-mt.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    11776 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/boost_system-mt.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    53248 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/boost_thread-mt.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)   756640 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/libiomp5md.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)    66560 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/obr.exe
+-rw-rw-r--   0 temis     (1000) temis     (1000)   466944 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/ova32.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)   100692 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/ova32.lib
+-rw-rw-r--   0 temis     (1000) temis     (1000)    28672 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk/ovaGUI.dll
+-rw-rw-r--   0 temis     (1000) temis     (1000)     2044 2023-05-09 07:10:40.000000 obrpy-0.1.1/obrpy/obrsdk.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      930 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/save.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     3285 2023-07-05 16:18:11.000000 obrpy-0.1.1/obrpy/settings.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     3389 2023-07-05 15:29:55.000000 obrpy-0.1.1/obrpy/take_a_look.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1789 2023-07-05 17:34:39.000000 obrpy-0.1.1/obrpy/to_export.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1026 2023-07-05 17:34:39.000000 obrpy-0.1.1/obrpy/to_import.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.112417 obrpy-0.1.1/obrpy.egg-info/
+-rw-rw-r--   0 temis     (1000) temis     (1000)      274 2023-07-05 18:21:45.000000 obrpy-0.1.1/obrpy.egg-info/PKG-INFO
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1222 2023-07-05 18:21:45.000000 obrpy-0.1.1/obrpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 temis     (1000) temis     (1000)        1 2023-07-05 18:21:45.000000 obrpy-0.1.1/obrpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 temis     (1000) temis     (1000)      445 2023-07-05 18:21:45.000000 obrpy-0.1.1/obrpy.egg-info/requires.txt
+-rw-rw-r--   0 temis     (1000) temis     (1000)        6 2023-07-05 18:21:45.000000 obrpy-0.1.1/obrpy.egg-info/top_level.txt
+-rw-rw-r--   0 temis     (1000) temis     (1000)       38 2023-07-05 18:21:45.164417 obrpy-0.1.1/setup.cfg
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1966 2023-07-05 18:17:21.000000 obrpy-0.1.1/setup.py
+drwxrwxr-x   0 temis     (1000) temis     (1000)        0 2023-07-05 18:21:45.164417 obrpy-0.1.1/test/
+-rw-rw-r--   0 temis     (1000) temis     (1000)      992 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      947 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_dataset.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     2463 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_export_obrfiles.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      596 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_export_settings.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      595 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_export_slices.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     5809 2023-07-05 17:34:28.000000 obrpy-0.1.1/test/test_import.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     2985 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_linked_attr.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)     1714 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_obr_ini.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      417 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_psss_dataset.py
+-rw-rw-r--   0 temis     (1000) temis     (1000)      669 2023-07-05 15:29:55.000000 obrpy-0.1.1/test/test_slices.py
```

### Comparing `obrpy-0.1.0/obrpy/ANALYSIS/global_analysis.py` & `obrpy-0.1.1/obrpy/ANALYSIS/global_analysis.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-import numpy as np
-
-try:
-    import cupy as cp
-    cupy_available = True
-except Exception as e:
-    print(e)
-    print('Please install cupy in order to use GPU acceleration')
-    cupy_available = False
-
-import matplotlib.pyplot as plt
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-from UTILS.utils import printProgressBar, find_index
-
-
-def global_analysis(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
-                        z:np.ndarray, f:np.ndarray,
-                        local_function,
-                        delta=200, window=2000,
-                        point=None, progressbar=False):
-    
-    """ Computes some analysis between two signals in a given window over a length
-        
-        :param y0           (np.array)      : first signal  [P,S] (used as reference)
-        :param y1           (np.array)      : second signal [P,S]
-        :param z            (np.ndarray)    : length array    [m]
-        :param f            (np.array)      : frequency array [GHz]
-
-        :param local_function (function): function which will compute some operation for each window
-
-                    Available functions are
-                            
-                            - spectral_shift()   : relative spectral shift
-                            - PSSS()             : phase-spectrum relative spectral shift
-
-                            * All of them are contained in the class Singal of obrpy -> obrpy.Signal.spectral_shift
-                    
-                    Any custom function provided, which have the following inputs will be work
-
-                            - y0 : local reference signal [P,S]
-                            - y1 : local signal [P,S]
-                            - z  : spatial array
-                            - f  : frequency array
-                            - display: will be set as True when the point of global analysis matches the parameter "point"
-
-        
-        :optional delta     (int)       : number of points of each step 
-        :optional window    (int)       : number of points on window 
-
-        :optional progressbar (bool)    : default is False. If True, a progressbar is displayed while processing the signal
-        :optional point       (float)   : default is False. If it is not False, some graphs will be created at this point
-
-        :returns output (np.array)      : array with computed signal at each window in a sequence
-    """
-
-    # Re define the window variable (is easier for the rest of the code)
-    window = round(window/2)
-
-    # Check type of signal
-    if not isinstance(y0, np.ndarray):
-         y0 = np.array(y0)
-    if not isinstance(y1,np.ndarray):
-         y1 = np.array(y1)
-
-    # Check if both y0 and y1 have the same dimension
-    if len(y0.shape) != len(y1.shape):
-        raise Exception("Signal dimension mismatch")
-
-    # Get the total number of points
-    n_points = y0.shape[1]
-
-    # Split the whole points into steps
-    steps = range(window,n_points-window+1,delta)
-
-    # Display the signals at this point
-    if point is not None:
-
-        point = find_index(z, point)
-
-        plt.figure()
-        plt.plot(y0[0],label='y0(P)')
-        plt.plot(y1[0],label='y1(P)')
-        plt.plot(y0[1],label='y0(S)')
-        plt.plot(y1[1],label='y1(S)')
-        plt.axvline(x=point)
-        plt.grid()
-        plt.show()
-
-    # Compute analysis 
-    output = []
-    for i in steps:
-
-            yy0 = np.array([y0[0,i-window:i+window], y0[1,i-window:i+window]])
-            yy1 = np.array([y1[0,i-window:i+window], y1[1,i-window:i+window]])
-            zz  = np.array(z[i-window:i+window])
-
-            output.append(float(local_function(yy0,yy1,zz,f,display=True if point is not None and i==point else False)))
-
-            printProgressBar(i + 1, n_points-window-delta-1, prefix = 'Computing spectral shift:', suffix = 'Complete', length = 50) if progressbar else None
-
-    return np.array(output)
-
-
-if cupy_available:
-
-     def global_analysis_GPU(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
-                         z:np.ndarray, f:np.ndarray,
-                         local_function,
-                         delta=200, window=2000,
-                         point=None, progressbar=False):
-     
-          """ Computes some analysis between two signals in a given window over a length
-               
-               :param y0           (np.array)      : first signal  [P,S] (used as reference)
-               :param y1           (np.array)      : second signal [P,S]
-               :param z            (np.ndarray)    : length array    [m]
-               :param f            (np.array)      : frequency array [GHz]
-
-               :param local_function (function): function which will compute some operation for each window
-
-                              Available functions are
-                                   
-                                   - spectral_shift()   : relative spectral shift
-                                   - PSSS()             : phase-spectrum relative spectral shift
-
-                                   * All of them are contained in the class Singal of obrpy -> obrpy.Signal.spectral_shift
-                              
-                              Any custom function provided, which have the following inputs will be work
-
-                                   - p0 : local reference signal P
-                                   - s0 : local reference signal S
-                                   - p1 : local signal P
-                                   - s1 : local signal S
-                                   - z  : spatial array
-                                   - f  : frequency array
-                                   - display: will be set as True when the point of global analysis matches the parameter "point"
-
-               
-               :optional delta     (int)       : number of points of each step 
-               :optional window    (int)       : number of points on window 
-
-               :optional progressbar (bool)    : default is False. If True, a progressbar is displayed while processing the signal
-               :optional point       (float)   : default is False. If it is not False, some graphs will be created at this point
-
-               :returns output (np.array)      : array with computed signal at each window in a sequence
-          """
-
-          # Check type of signal
-          if not isinstance(y0, np.ndarray):
-               y0 = np.array(y0)
-          if not isinstance(y1,np.ndarray):
-               y1 = np.array(y1)
-          if not isinstance(y0, np.ndarray):
-               f = np.array(f)
-          if not isinstance(y1,np.ndarray):
-               z = np.array(z)
-
-          # Check if both y0 and y1 have the same dimension
-          if len(y0.shape) != len(y1.shape):
-               raise Exception("Signal dimension mismatch")
-
-          # Get the total number of points
-          n_points = y0.shape[1]
-
-          # Split the whole points into steps
-          steps = range(window,n_points-window+1,delta)
-
-          ##### GPU acceleration algorithm #####
-
-          # Unpack the signals 
-          p0 = y0[0,:]
-          p1 = y1[0,:]
-          s0 = y0[1,:]
-          s1 = y1[1,:]
-
-          # Convert input arrays to CuPy arrays
-          p0 = cp.asarray(p0)
-          p1 = cp.asarray(p1)
-          s0 = cp.asarray(s0)
-          s1 = cp.asarray(s1)
-          z = cp.asarray(z)
-          f = cp.asarray(f)
-
-          # Define the window size and stride
-          window_size = window
-          stride = delta
-
-          # Generate a list of window indices
-          start_indices = cp.arange(0, n_points - window_size + 1, stride)
-
-          # Extract the windows from the data
-          p0W = cp.array([p0[i:i+window_size] for i in start_indices])
-          p1W = cp.array([p1[i:i+window_size] for i in start_indices])
-          s0W = cp.array([s0[i:i+window_size] for i in start_indices])
-          s1W = cp.array([s1[i:i+window_size] for i in start_indices])
-          zW  = cp.array([z[i:i+window_size] for i in start_indices])
-
-          # Process signal windowed
-          output = local_function(p0W,s0W,p1W,s1W,zW,f)
-
-          # Convert output array to NumPy array
-          return output.get()
-
-elif not cupy_available:
-
-     def global_analysis_GPU(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
-                    z:np.ndarray, f:np.ndarray,
-                    local_function,
-                    delta=200, window=2000,
-                    point=None, progressbar=False):
-          
-          if local_function.__name__.endswith('_GPU'):
-               func_name = local_function.__name__[:-4] # remove the _GPU suffix
-               local_function = getattr(self.Signal, func_name)
-
+import numpy as np
+
+try:
+    import cupy as cp
+    cupy_available = True
+except Exception as e:
+    print(e)
+    print('Please install cupy in order to use GPU acceleration')
+    cupy_available = False
+
+import matplotlib.pyplot as plt
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+from UTILS.utils import printProgressBar, find_index
+
+
+def global_analysis(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
+                        z:np.ndarray, f:np.ndarray,
+                        local_function,
+                        delta=200, window=2000,
+                        point=None, progressbar=False):
+    
+    """ Computes some analysis between two signals in a given window over a length
+        
+        :param y0           (np.array)      : first signal  [P,S] (used as reference)
+        :param y1           (np.array)      : second signal [P,S]
+        :param z            (np.ndarray)    : length array    [m]
+        :param f            (np.array)      : frequency array [GHz]
+
+        :param local_function (function): function which will compute some operation for each window
+
+                    Available functions are
+                            
+                            - spectral_shift()   : relative spectral shift
+                            - PSSS()             : phase-spectrum relative spectral shift
+
+                            * All of them are contained in the class Singal of obrpy -> obrpy.Signal.spectral_shift
+                    
+                    Any custom function provided, which have the following inputs will be work
+
+                            - y0 : local reference signal [P,S]
+                            - y1 : local signal [P,S]
+                            - z  : spatial array
+                            - f  : frequency array
+                            - display: will be set as True when the point of global analysis matches the parameter "point"
+
+        
+        :optional delta     (int)       : number of points of each step 
+        :optional window    (int)       : number of points on window 
+
+        :optional progressbar (bool)    : default is False. If True, a progressbar is displayed while processing the signal
+        :optional point       (float)   : default is False. If it is not False, some graphs will be created at this point
+
+        :returns output (np.array)      : array with computed signal at each window in a sequence
+    """
+
+    # Re define the window variable (is easier for the rest of the code)
+    window = round(window/2)
+
+    # Check type of signal
+    if not isinstance(y0, np.ndarray):
+         y0 = np.array(y0)
+    if not isinstance(y1,np.ndarray):
+         y1 = np.array(y1)
+
+    # Check if both y0 and y1 have the same dimension
+    if len(y0.shape) != len(y1.shape):
+        raise Exception("Signal dimension mismatch")
+
+    # Get the total number of points
+    n_points = y0.shape[1]
+
+    # Split the whole points into steps
+    steps = range(window,n_points-window+1,delta)
+
+    # Display the signals at this point
+    if point is not None:
+
+        point = find_index(z, point)
+
+        plt.figure()
+        plt.plot(y0[0],label='y0(P)')
+        plt.plot(y1[0],label='y1(P)')
+        plt.plot(y0[1],label='y0(S)')
+        plt.plot(y1[1],label='y1(S)')
+        plt.axvline(x=point)
+        plt.grid()
+        plt.show()
+
+    # Compute analysis 
+    output = []
+    for i in steps:
+
+            yy0 = np.array([y0[0,i-window:i+window], y0[1,i-window:i+window]])
+            yy1 = np.array([y1[0,i-window:i+window], y1[1,i-window:i+window]])
+            zz  = np.array(z[i-window:i+window])
+
+            output.append(float(local_function(yy0,yy1,zz,f,display=True if point is not None and i==point else False)))
+
+            printProgressBar(i + 1, n_points-window-delta-1, prefix = 'Computing spectral shift:', suffix = 'Complete', length = 50) if progressbar else None
+
+    return np.array(output)
+
+
+if cupy_available:
+
+     def global_analysis_GPU(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
+                         z:np.ndarray, f:np.ndarray,
+                         local_function,
+                         delta=200, window=2000,
+                         point=None, progressbar=False):
+     
+          """ Computes some analysis between two signals in a given window over a length
+               
+               :param y0           (np.array)      : first signal  [P,S] (used as reference)
+               :param y1           (np.array)      : second signal [P,S]
+               :param z            (np.ndarray)    : length array    [m]
+               :param f            (np.array)      : frequency array [GHz]
+
+               :param local_function (function): function which will compute some operation for each window
+
+                              Available functions are
+                                   
+                                   - spectral_shift()   : relative spectral shift
+                                   - PSSS()             : phase-spectrum relative spectral shift
+
+                                   * All of them are contained in the class Singal of obrpy -> obrpy.Signal.spectral_shift
+                              
+                              Any custom function provided, which have the following inputs will be work
+
+                                   - p0 : local reference signal P
+                                   - s0 : local reference signal S
+                                   - p1 : local signal P
+                                   - s1 : local signal S
+                                   - z  : spatial array
+                                   - f  : frequency array
+                                   - display: will be set as True when the point of global analysis matches the parameter "point"
+
+               
+               :optional delta     (int)       : number of points of each step 
+               :optional window    (int)       : number of points on window 
+
+               :optional progressbar (bool)    : default is False. If True, a progressbar is displayed while processing the signal
+               :optional point       (float)   : default is False. If it is not False, some graphs will be created at this point
+
+               :returns output (np.array)      : array with computed signal at each window in a sequence
+          """
+
+          # Check type of signal
+          if not isinstance(y0, np.ndarray):
+               y0 = np.array(y0)
+          if not isinstance(y1,np.ndarray):
+               y1 = np.array(y1)
+          if not isinstance(y0, np.ndarray):
+               f = np.array(f)
+          if not isinstance(y1,np.ndarray):
+               z = np.array(z)
+
+          # Check if both y0 and y1 have the same dimension
+          if len(y0.shape) != len(y1.shape):
+               raise Exception("Signal dimension mismatch")
+
+          # Get the total number of points
+          n_points = y0.shape[1]
+
+          # Split the whole points into steps
+          steps = range(window,n_points-window+1,delta)
+
+          ##### GPU acceleration algorithm #####
+
+          # Unpack the signals 
+          p0 = y0[0,:]
+          p1 = y1[0,:]
+          s0 = y0[1,:]
+          s1 = y1[1,:]
+
+          # Convert input arrays to CuPy arrays
+          p0 = cp.asarray(p0)
+          p1 = cp.asarray(p1)
+          s0 = cp.asarray(s0)
+          s1 = cp.asarray(s1)
+          z = cp.asarray(z)
+          f = cp.asarray(f)
+
+          # Define the window size and stride
+          window_size = window
+          stride = delta
+
+          # Generate a list of window indices
+          start_indices = cp.arange(0, n_points - window_size + 1, stride)
+
+          # Extract the windows from the data
+          p0W = cp.array([p0[i:i+window_size] for i in start_indices])
+          p1W = cp.array([p1[i:i+window_size] for i in start_indices])
+          s0W = cp.array([s0[i:i+window_size] for i in start_indices])
+          s1W = cp.array([s1[i:i+window_size] for i in start_indices])
+          zW  = cp.array([z[i:i+window_size] for i in start_indices])
+
+          # Process signal windowed
+          output = local_function(p0W,s0W,p1W,s1W,zW,f)
+
+          # Convert output array to NumPy array
+          return output.get()
+
+elif not cupy_available:
+
+     def global_analysis_GPU(self, y0:np.ndarray[np.ndarray,np.ndarray], y1:np.ndarray[np.ndarray,np.ndarray],
+                    z:np.ndarray, f:np.ndarray,
+                    local_function,
+                    delta=200, window=2000,
+                    point=None, progressbar=False):
+          
+          if local_function.__name__.endswith('_GPU'):
+               func_name = local_function.__name__[:-4] # remove the _GPU suffix
+               local_function = getattr(self.Signal, func_name)
+
           return self.global_analysis(y0=y0, y1=y1, z=z, f=f, local_function = local_function, delta=delta, window=window, point=point, progressbar=progressbar)
```

### Comparing `obrpy-0.1.0/obrpy/ANALYSIS/local_analysis.py` & `obrpy-0.1.1/obrpy/ANALYSIS/local_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-import sys
-import os
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import time
-import json
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-from UTILS.utils import printProgressBar, find_index
-
-def genSlices(self,delta=200,window=2000,export=True):
-
-    """
-    Creates a slices object full of slices by slicing .obr data contained in self.OBRfiles
-
-            optional: delta  (int)  = 200      : step
-            optional: window (int)  = 2000     : window
-            optional: settings_update (bool) = True : update settings with the file 
-
-    """
-
-    """ Checkouts """
-    # OBRfiles checkout
-    self.OBR_checkout()
-
-    # Slices checkout (if already exists)
-    if self.slices_checkout():
-        pass
-    else:
-        return
-    
-    """ Slices generation """
-
-    # Open slices object
-    slices_obj = self.slices
-
-    # Generate slices
-    LEN = len(self.obrfiles.files);i=0
-    printProgressBar(0, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
-
-    for key, OBRfile in self.obrfiles.files.items():
-        slices_obj = self._obr2slices(OBRfile,slices_obj,delta=delta,window=window)
-        printProgressBar(i, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
-
-    # Update
-    self.slices = slices_obj
-
-    # Export
-    if export:
-        self.slices.export_book()
-        self.slices.export_obj()
-
-def _obr2slices(self,OBRfile,slices_obj,delta=200,window=2000):
-    """
-    Generates slices from a single OBRfile and labels the slices in slices book.
-
-    The slices are created by taking the entire signal and then
-    traversing it in jumps of points of size "step" and considering
-    the points to be in a bubble of diameter "window".
-
-            param: OBRfile    (OBRfile object)    : an object which contains all the information required
-            param: slices_obj (Slices object)     : the slices object which will contain the slices and that will be saved
-
-            optional: delta  = 200     : step
-            optional: window = 2000    : window size
-
-            returns: slices_obj (slices object): an object which contains all the slices
-    """
-
-    """ Variables checkout """
-
-    # Check if delta is an integer
-    if not isinstance(delta,int):
-         delta = round(delta)
-
-    # Reduce window to the half F¡for easier programation below
-    window = int(window/2)
-
-    """ Get information about state of the fiber from settings """
-
-    # Get environment variables
-    T0 = getattr(OBRfile,self.settings.T0)
-    T1 = getattr(OBRfile,self.settings.T1)
-    E0 = getattr(OBRfile,self.settings.E0)
-    E1 = getattr(OBRfile,self.settings.E1)
-
-    z_ini = self.settings.z_ini
-    z_fin = self.settings.z_fin
-
-    """ Take data from the segment """
-
-    if OBRfile.z[0] != z_ini or OBRfile.z[-1] != z_fin:
-        l = find_index(OBRfile.z,[z_ini,z_fin])
-        P = OBRfile.Data[0][l[0]:l[1]]
-        S = OBRfile.Data[1][l[0]:l[1]]
-        z = OBRfile.z[l[0]:l[1]]
-    elif OBRfile.z[0] == z_ini and OBRfile.z[-1] == z_fin:
-        P = OBRfile.Data[0]
-        S = OBRfile.Data[1]
-        z = OBRfile.z
-    else:
-        raise Exception('Something went wrong with the function obr2slices:( ')
-    
-    
-    """ Make the distributions of the strain and temperature"""
-
-    # Full data length (takes one state of polarization)
-    n = len(P)
-
-    # Corresponding steps
-    steps = range(window,n-window+1,delta)
-    
-    x = np.linspace(0,abs(z_fin-z_ini),len(steps))
-    T = T0 + T1 * x
-    E = E0 + E1 * x
-
-    """ Slices generation """
-
-    # Column names and slice initialization
-    slice_obj = self.Slice()
-    column_names = [key for key in slice_obj.__dict__.keys()]
-
-    # Create a dataframe to storage new information
-    new_information = pd.DataFrame(columns = column_names, dtype=object)
-
-    # ID initialization
-    ID = slices_obj.last_ID
-
-    # Generate slices
-    for idx,i in enumerate(steps):
-
-            # Current ID
-            ID += 1
- 
-            # Update new information
-            new_row = {
-            'ID'                : ID,
-            'T'                 : T[idx],               # [ºC]
-            'E'                 : E[idx],               # 
-            'z'                 : z[i-window:i+window], # [m]                    
-            'x'                 : x[idx]*1e3,           # [mm]
-            'f_0'               : OBRfile.f[0],         # [GHz]
-            'f_end'             : OBRfile.f[-1],        # [GHz]
-            'delta'             : delta,
-            'window'            : window,
-            'date'              : time.strftime("%Y,%m,%d,%H:%M:%S"),
-            'parent_file'       : OBRfile.ID,
-            'P'                 : P[i-window:i+window],
-            'S'                 : S[i-window:i+window]}
-
-            # Append new row
-            new_information = pd.concat([new_information, pd.DataFrame([new_row])], ignore_index=True)
-
-            # Append new element
-            slice_obj = self.Slice()
-            for val in column_names:
-                setattr(slice_obj, val, new_row[val])
-            slices_obj.slices[ID] = slice_obj
-
-    # Update last ID
-    slices_obj.last_ID = ID
-
-    return slices_obj
-
-
-def genDataset(self, layer0, matches = 100, percentage = 100):
-    
-    """ Function to load all slices (previously generated), compute them in pairs with a function, and
-    genenerate new values for a dataset usable for AI 
-
-        : param: layer0 (fun) : function to compute slices by pairs, it must take two rows of slices.book
-                                and return Xcolumns, Ycolumns and the new_row (list) of dataframe whose first columns must be 
-                                the ID of the row, the ID of the first parent and the ID of the second one (in that order)
-
-        : optional: matches (float)                   : percentage of reference segments to consider from total
-        : optional: percentage (float) :              : percentage of dataset to consider
-
-    """
-
-    """ Checkout """
-
-    if not isinstance(self.slices,bool) and len(self.slices.slices) != 0 :
-        pass
-    else:
-        print("No slices found: Please run genSlices() and then genDataset()")
-        return
-
-    if self.dataset_checkout():
-        pass
-    else:
-        return
-
-    """ Dataset generation """
-    dataset = self.dataset
-
-    # Create slices book
-    slices_book = self.slices.create_book()
-    slices_book = slices_book.sample(frac=percentage/100)
-
-    # Generate dataset
-    LEN = int(len(slices_book.index)); i=0; elements=0
-    printProgressBar(0, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
-
-    for index, row in slices_book.iterrows():
-
-        # Search in dataframe for other rows to consider as reference
-        try:
-            ref_rows = slices_book[(round(slices_book['x'], 8) == round(row['x'],8))]
-        except:
-            print('NO REF FOUND for:',row['ID'])
-            z_matches = slices_book[slices_book['x'] == row['x']]
-            print('z_matches: ',len(z_matches))
-            continue
-
-        # Reduce number of references
-        ref_rows = ref_rows.sample(frac=matches/100)
-
-        # For each slice in the same position compute difference
-        for jndex, ref_row in ref_rows.iterrows():
-
-            # Update ID
-            dataset.last_ID += 1
-
-            # Compute the pair of slices
-            dataset.Xcolumns, dataset.Ycolumns, new_row = layer0(dataset.last_ID, row, ref_row)
-            dataset.data = pd.concat([dataset.data, pd.DataFrame([new_row])], ignore_index=True)
-
-            # Just to know later
-            elements += 1
-
-        printProgressBar(i, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
-
-
-    print(f'Dataset with {elements} elements created!')
-
-    # Update book with new information
-    self.dataset = dataset
-
+import sys
+import os
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import time
+import json
+
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+from UTILS.utils import printProgressBar, find_index
+
+def genSlices(self,delta=200,window=2000,export=False):
+
+    """
+    Creates a slices object full of slices by slicing .obr data contained in self.OBRfiles
+
+            optional: delta  (int)  = 200      : step
+            optional: window (int)  = 2000     : window
+            optional: export (bool) = False    : export slices to .csv and .book
+
+    """
+
+    """ Checkouts """
+    # OBRfiles checkout
+    self.OBR_checkout()
+
+    # Slices checkout (if already exists)
+    if self.slices_checkout():
+        pass
+    else:
+        return
+    
+    """ Slices generation """
+
+    # Open slices object
+    slices_obj = self.slices
+
+    # Generate slices
+    LEN = len(self.obrfiles.files);i=0
+    printProgressBar(0, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
+
+    for key, OBRfile in self.obrfiles.files.items():
+        slices_obj = self._obr2slices(OBRfile,slices_obj,delta=delta,window=window)
+        printProgressBar(i, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
+
+    # Update
+    self.slices = slices_obj
+
+    # Export
+    if export:
+        self.slices.export_book()
+        self.slices.export_obj()
+
+def _obr2slices(self,OBRfile,slices_obj,delta=200,window=2000):
+    """
+    Generates slices from a single OBRfile and labels the slices in slices book.
+
+    The slices are created by taking the entire signal and then
+    traversing it in jumps of points of size "step" and considering
+    the points to be in a bubble of diameter "window".
+
+            param: OBRfile    (OBRfile object)    : an object which contains all the information required
+            param: slices_obj (Slices object)     : the slices object which will contain the slices and that will be saved
+
+            optional: delta  = 200     : step
+            optional: window = 2000    : window size
+
+            returns: slices_obj (slices object): an object which contains all the slices
+    """
+
+    """ Variables checkout """
+
+    # Check if delta is an integer
+    if not isinstance(delta,int):
+         delta = round(delta)
+
+    # Reduce window to the half F¡for easier programation below
+    window = int(window/2)
+
+    """ Get information about state of the fiber from settings """
+
+    # Get environment variables
+    T0 = getattr(OBRfile,self.settings.T0)
+    T1 = getattr(OBRfile,self.settings.T1)
+    E0 = getattr(OBRfile,self.settings.E0)
+    E1 = getattr(OBRfile,self.settings.E1)
+
+    z_ini = self.settings.z_ini
+    z_fin = self.settings.z_fin
+
+    """ Take data from the segment """
+
+    if OBRfile.z[0] != z_ini or OBRfile.z[-1] != z_fin:
+        l = find_index(OBRfile.z,[z_ini,z_fin])
+        P = OBRfile.Data[0][l[0]:l[1]]
+        S = OBRfile.Data[1][l[0]:l[1]]
+        z = OBRfile.z[l[0]:l[1]]
+    elif OBRfile.z[0] == z_ini and OBRfile.z[-1] == z_fin:
+        P = OBRfile.Data[0]
+        S = OBRfile.Data[1]
+        z = OBRfile.z
+    else:
+        raise Exception('Something went wrong with the function obr2slices:( ')
+    
+    
+    """ Make the distributions of the strain and temperature"""
+
+    # Full data length (takes one state of polarization)
+    n = len(P)
+
+    # Corresponding steps
+    steps = range(window,n-window+1,delta)
+    
+    x = np.linspace(0,abs(z_fin-z_ini),len(steps))
+    T = T0 + T1 * x
+    E = E0 + E1 * x
+
+    """ Slices generation """
+
+    # Column names and slice initialization
+    slice_obj = self.Slice()
+    column_names = [key for key in slice_obj.__dict__.keys()]
+
+    # Create a dataframe to storage new information
+    new_information = pd.DataFrame(columns = column_names, dtype=object)
+
+    # ID initialization
+    ID = slices_obj.last_ID
+
+    # Generate slices
+    for idx,i in enumerate(steps):
+
+            # Current ID
+            ID += 1
+ 
+            # Update new information
+            new_row = {
+            'ID'                : ID,
+            'T'                 : T[idx],               # [ºC]
+            'E'                 : E[idx],               # 
+            'z'                 : z[i-window:i+window], # [m]                    
+            'x'                 : x[idx]*1e3,           # [mm]
+            'f'                 : OBRfile.f,            # [GHz]
+            'delta'             : delta,
+            'window'            : window,
+            'date'              : time.strftime("%Y,%m,%d,%H:%M:%S"),
+            'parent_file'       : OBRfile.ID,
+            'P'                 : P[i-window:i+window],
+            'S'                 : S[i-window:i+window]}
+
+            # Append new row
+            new_information = pd.concat([new_information, pd.DataFrame([new_row])], ignore_index=True)
+
+            # Append new element
+            slice_obj = self.Slice()
+            for val in column_names:
+                setattr(slice_obj, val, new_row[val])
+            slices_obj.slices[ID] = slice_obj
+
+    # Update last ID
+    slices_obj.last_ID = ID
+
+    return slices_obj
+
+
+def genDataset(self, layer0, matches = 100, percentage = 100):
+    
+    """ Function to load all slices (previously generated), compute them in pairs with a function, and
+    genenerate new values for a dataset usable for AI 
+
+        : param: layer0 (fun) : function to compute slices by pairs, it must take two rows of slices.book
+                                and return Xcolumns, Ycolumns and the new_row (list) of dataframe whose first columns must be 
+                                the ID of the row, the ID of the first parent and the ID of the second one (in that order)
+
+        : optional: matches (float)                   : percentage of reference segments to consider from total
+        : optional: percentage (float) :              : percentage of dataset to consider
+
+    """
+
+    """ Checkout """
+
+    if not isinstance(self.slices,bool) and len(self.slices.slices) != 0 :
+        pass
+    else:
+        print("No slices found: Please run genSlices() and then genDataset()")
+        return
+
+    if self.dataset_checkout():
+        pass
+    else:
+        return
+
+    """ Dataset generation """
+    dataset = self.dataset
+
+    # Create slices book
+    slices_book = self.slices.create_book()
+    slices_book = slices_book.sample(frac=percentage/100)
+
+    # Generate dataset
+    LEN = int(len(slices_book.index)); i=0; elements=0
+    printProgressBar(0, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
+
+    for index, row in slices_book.iterrows():
+
+        # Search in dataframe for other rows to consider as reference
+        try:
+            ref_rows = slices_book[(round(slices_book['x'], 8) == round(row['x'],8))]
+        except:
+            print('NO REF FOUND for:',row['ID'])
+            z_matches = slices_book[slices_book['x'] == row['x']]
+            print('z_matches: ',len(z_matches))
+            continue
+
+        # Reduce number of references
+        ref_rows = ref_rows.sample(frac=matches/100)
+
+        # For each slice in the same position compute difference
+        for jndex, ref_row in ref_rows.iterrows():
+
+            # Update ID
+            dataset.last_ID += 1
+
+            # Compute the pair of slices
+            dataset.Xcolumns, dataset.Ycolumns, new_row = layer0(dataset.last_ID, row, ref_row)
+            dataset.data = pd.concat([dataset.data, pd.DataFrame([new_row])], ignore_index=True)
+
+            # Just to know later
+            elements += 1
+
+        printProgressBar(i, LEN, prefix = 'Progress:', suffix = 'Complete', length = 50); i += 1
+
+
+    print(f'Dataset with {elements} elements created!')
+
+    # Update book with new information
+    self.dataset = dataset
+    print(dataset.data)
+
     return dataset.data
```

### Comparing `obrpy-0.1.0/obrpy/SIGNAL/cross_spectrum.py` & `obrpy-0.1.1/obrpy/SIGNAL/cross_spectrum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import numpy as np
-import nitime.algorithms as tsa
-
-def dB(x, out=None):
-    if out is None:
-        return 10 * np.log10(x)
-    else:
-        np.log10(x, out)
-        np.multiply(out, 10, out)
-
-def mtem(i, j, dt):
-    """
-    multitaper estimation method
-    Input:
-    i      first time series
-    j      second time series
-
-    Output:
-    fki    power spectral density i
-    fkj    power spectral density j
-    cij    cross-spectral density ij
-    coh    coherence
-    ph     phase spectrum between ij at input freq
-
-    """
-    #print('i size', i.shape)
-    #print('j size', j.shape)
-
-    # apply multi taper cross spectral density from nitime module
-    f, pcsd_est = tsa.multi_taper_csd(np.vstack([i,j]), Fs=1/dt, low_bias=True, adaptive=True, sides='onesided')
-
-    # output is MxMxN matrix, extract the psd and csd
-    fki = pcsd_est.diagonal().T[0]
-    fkj = pcsd_est.diagonal().T[1]
-    cij = pcsd_est.diagonal(+1).T.ravel()
-
-    # using complex argument of cxy extract phase component
-    ph = np.angle(cij)
-
-    # calculate coherence using csd and psd
-    coh = np.abs(cij)**2 / (fki * fkj)
-
-    return f, fki, fkj, cij, ph, coh
-
-def mtem_unct(i_, j_, dt_, cf, mc_no=20):
-    """
-    Uncertainty function using Monte Carlo analysis
-    Input:
-    i_     timeseries i
-    j_     timeseries j
-    cf     coherence function between i and j
-    mc_no  number of iterations default is 20, minimum is 3
-
-    Output:
-    phif   phase uncertainty bounded between 0 and pi
-    """
-    #print('iteration no is', mc_no)
-
-    data = np.vstack([i_,j_])
-    # number of iterations
-    # flip coherence and horizontal stack
-    cg = np.hstack((cf[:-1], np.flipud(cf[:-1])))
-
-    # random time series fi
-    mc_fi = np.random.standard_normal(size=(mc_no,len(data[0])))
-    mc_fi = mc_fi / np.sum(abs(mc_fi),axis=1)[None].T
-
-    # random time series fj
-    mc_fj = np.random.standard_normal(size=(mc_no,len(data[0])))
-    mc_fj = mc_fj / np.sum(abs(mc_fj),axis=1)[None].T
-
-    # create semi random timeseries based on magnitude squared coherence
-    # and inverse fourier transform for js
-    js = np.real(np.fft.ifft(mc_fj * np.sqrt(1 - cg ** 2)))
-    js_ = js + np.real(np.fft.ifft(mc_fi *cg))
-
-    # inverse fourier transform for xs
-    is_ = np.real(np.fft.ifft(mc_fi))
-
-    # spectral analysis
-    f_s, pcsd_est = tsa.multi_taper_csd(np.vstack([is_,js_]), Fs=1/dt_, low_bias=True, adaptive=True, sides='onesided')
-    cijx = pcsd_est.diagonal(+int(is_.shape[0])).T
-    phi = np.angle(cijx)
-
-    # sort and average the highest uncertianties
-    pl = int(round(0.95*mc_no)+1)
-    phi = np.sort(phi,axis=0)
-    phi = phi[((mc_no+1)-pl):pl]
-    phi = np.array([phi[pl-2,:],-phi[pl-mc_no,:]])
-    phi = phi.mean(axis=0)#
-    phi = np.convolve(phi, np.array([1,1,1])/3)
-    phif = phi[1:-1]
-    return phif
-
-def PSSS(y0,y1,f,display=False):
-
-    """ Function to compute the relative phase spectrum spectral shift in a region.
-
-        The cross spectrum phase spectrum is computed using the multitapper method defined 
-        in other functions of this module and using the TSA nitime algorithm.
-        Then signal.correlate is used to determine the cross correlation, and the
-        maximum position is located and related with the spectral shift trought the scan ratio
-
-        :param  y0 (np.array)   : First signal to compare, used as reference
-        :param  y1 (np.array)   : Second signal to compare
-        :param  f  (np.array)   : Frequency domain x axis [GHz]
-
-        :optional display=False (bool) : If True, a plot with the cross correlation will be displayed 
-                                        (add  "plt.show()" or "plt.savefig()" after this funtion)
-
-        :retruns -1*out/np.mean(f) (float)   : relative phase spectrum spectral shift
-    """
-
-
-    # Unpack the signals 
-
-    p1 = y0[0,:]
-    p2 = y1[0,:]
-    s1 = y0[1,:]
-    s2 = y1[1,:]
-
-    # Check length of signal to discard a value if necessary
-
-    if len(p1)%2 == 0:
-        p1 = p1[:-1]
-        p2 = p2[:-1]
-        s1 = s1[:-1]
-        s2 = s2[:-1]
-
-    # Frequency sampling
-    DF = f[-1]-f[0]     # Total frequency increment [GHz]
-    n = len(p1)         # Sample lenght
-    dt = 1/(f[1]-f[0])  # Time increment
-
-    # Phase spectrum
-    f, fki, fkj, cij, ph, coh = mtem(p1,s1,dt)
-    Y1 = ph
-    f, fki, fkj, cij, ph, coh = mtem(p2,s2,dt)
-    Y2 = ph
-
-    # Normalization
-    Y1 = (Y1 - np.mean(Y1)) / (np.std(Y1)* len(Y1))
-    Y2 = (Y2 - np.mean(Y2)) / (np.std(Y2))
-
-    # Cross correlation
-    corr = np.correlate(Y1, Y2, mode='same')
-
-    # Frequency lags
-    freq_lags = np.linspace(-0.5*DF, 0.5*DF, n)
-    out = freq_lags[np.argmax(corr)]
-
-    return -1*out/np.mean(f)
+import numpy as np
+import nitime.algorithms as tsa
+
+def dB(x, out=None):
+    if out is None:
+        return 10 * np.log10(x)
+    else:
+        np.log10(x, out)
+        np.multiply(out, 10, out)
+
+def mtem(i, j, dt):
+    """
+    multitaper estimation method
+    Input:
+    i      first time series
+    j      second time series
+
+    Output:
+    fki    power spectral density i
+    fkj    power spectral density j
+    cij    cross-spectral density ij
+    coh    coherence
+    ph     phase spectrum between ij at input freq
+
+    """
+    #print('i size', i.shape)
+    #print('j size', j.shape)
+
+    # apply multi taper cross spectral density from nitime module
+    f, pcsd_est = tsa.multi_taper_csd(np.vstack([i,j]), Fs=1/dt, low_bias=True, adaptive=True, sides='onesided')
+
+    # output is MxMxN matrix, extract the psd and csd
+    fki = pcsd_est.diagonal().T[0]
+    fkj = pcsd_est.diagonal().T[1]
+    cij = pcsd_est.diagonal(+1).T.ravel()
+
+    # using complex argument of cxy extract phase component
+    ph = np.angle(cij)
+
+    # calculate coherence using csd and psd
+    coh = np.abs(cij)**2 / (fki * fkj)
+
+    return f, fki, fkj, cij, ph, coh
+
+def mtem_unct(i_, j_, dt_, cf, mc_no=20):
+    """
+    Uncertainty function using Monte Carlo analysis
+    Input:
+    i_     timeseries i
+    j_     timeseries j
+    cf     coherence function between i and j
+    mc_no  number of iterations default is 20, minimum is 3
+
+    Output:
+    phif   phase uncertainty bounded between 0 and pi
+    """
+    #print('iteration no is', mc_no)
+
+    data = np.vstack([i_,j_])
+    # number of iterations
+    # flip coherence and horizontal stack
+    cg = np.hstack((cf[:-1], np.flipud(cf[:-1])))
+
+    # random time series fi
+    mc_fi = np.random.standard_normal(size=(mc_no,len(data[0])))
+    mc_fi = mc_fi / np.sum(abs(mc_fi),axis=1)[None].T
+
+    # random time series fj
+    mc_fj = np.random.standard_normal(size=(mc_no,len(data[0])))
+    mc_fj = mc_fj / np.sum(abs(mc_fj),axis=1)[None].T
+
+    # create semi random timeseries based on magnitude squared coherence
+    # and inverse fourier transform for js
+    js = np.real(np.fft.ifft(mc_fj * np.sqrt(1 - cg ** 2)))
+    js_ = js + np.real(np.fft.ifft(mc_fi *cg))
+
+    # inverse fourier transform for xs
+    is_ = np.real(np.fft.ifft(mc_fi))
+
+    # spectral analysis
+    f_s, pcsd_est = tsa.multi_taper_csd(np.vstack([is_,js_]), Fs=1/dt_, low_bias=True, adaptive=True, sides='onesided')
+    cijx = pcsd_est.diagonal(+int(is_.shape[0])).T
+    phi = np.angle(cijx)
+
+    # sort and average the highest uncertianties
+    pl = int(round(0.95*mc_no)+1)
+    phi = np.sort(phi,axis=0)
+    phi = phi[((mc_no+1)-pl):pl]
+    phi = np.array([phi[pl-2,:],-phi[pl-mc_no,:]])
+    phi = phi.mean(axis=0)#
+    phi = np.convolve(phi, np.array([1,1,1])/3)
+    phif = phi[1:-1]
+    return phif
+
+def PSSS(y0:np.ndarray,y1:np.ndarray,z:np.ndarray,f:np.ndarray,display=False) -> float:
+
+    """ Function to compute the relative phase spectrum spectral shift in a region.
+
+        The cross spectrum phase spectrum is computed using the multitapper method defined 
+        in other functions of this module and using the TSA nitime algorithm.
+        Then signal.correlate is used to determine the cross correlation, and the
+        maximum position is located and related with the spectral shift trought the scan ratio
+
+        :param  y0 (np.array)   : First signal to compare, used as reference
+        :param  y1 (np.array)   : Second signal to compare
+        :param  f  (np.array)   : Frequency domain x axis [GHz]
+
+        :optional display=False (bool) : If True, a plot with the cross correlation will be displayed 
+                                        (add  "plt.show()" or "plt.savefig()" after this funtion)
+
+        :retruns -1*out/np.mean(f) (float)   : relative phase spectrum spectral shift
+    """
+
+
+    # Unpack the signals 
+
+    p1 = y0[0,:]
+    p2 = y1[0,:]
+    s1 = y0[1,:]
+    s2 = y1[1,:]
+
+    # Check length of signal to discard a value if necessary
+
+    if len(p1)%2 == 0:
+        p1 = p1[:-1]
+        p2 = p2[:-1]
+        s1 = s1[:-1]
+        s2 = s2[:-1]
+
+    # Frequency sampling
+    DF = f[-1]-f[0]     # Total frequency increment [GHz]
+    n = len(p1)         # Sample lenght
+    dt = 1/(f[1]-f[0])  # Time increment
+
+    # Phase spectrum
+    f, fki, fkj, cij, ph, coh = mtem(p1,s1,dt)
+    Y1 = ph
+    f, fki, fkj, cij, ph, coh = mtem(p2,s2,dt)
+    Y2 = ph
+
+    # Normalization
+    Y1 = (Y1 - np.mean(Y1)) / (np.std(Y1)* len(Y1))
+    Y2 = (Y2 - np.mean(Y2)) / (np.std(Y2))
+
+    # Cross correlation
+    corr = np.correlate(Y1, Y2, mode='same')
+
+    # Frequency lags
+    freq_lags = np.linspace(-0.5*DF, 0.5*DF, n)
+    out = freq_lags[np.argmax(corr)]
+
+    return -1*out/np.mean(f)
```

### Comparing `obrpy-0.1.0/obrpy/SIGNAL/spectral_shift.py` & `obrpy-0.1.1/obrpy/SIGNAL/spectral_shift.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import numpy as np
-
-try:
-    import cupy as cp
-    cupy_available = True
-except Exception as e:
-    print(e)
-    print('Please install cupy in order to use GPU acceleration')
-    cupy_available = False
-
-import matplotlib.pyplot as plt
-from scipy import signal
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-from UTILS.utils import printProgressBar
-
-
-""" 
-Spectral shift
-
-    This module contains functions used to compuhow te the relaive spectral shift
-    (which actually is spectralshift/central_frecuency) along an optic fiber longitude
-
-"""
-
-def spectral_shift(y0:np.ndarray,y1,z,f,display=False,fft=True):
-    """ Function to compute the relative spectral shift in a region.
-
-        Scipy's signal.correlate is used to determine the cross correlation, then the
-        maximum position is located and related with the spectral shift trought the scan ratio
-
-        :param  y0 (np.array)   : First signal to compare, used as reference [P,S]
-        :param  y1 (np.array)   : Second signal to compare [P,S]
-        :param  z  (np.array)   : Spatial domain x axis [m] (not used)
-        :param  f  (np.array)   : Frequency domain x axis [GHz]
-
-        :optional display=False (bool) : If True, a plot with the cross correlation will be displayed 
-                                        (add  "plt.show()" or "plt.savefig()" after this funtion)
-        :optional fft=True (bool)      : If True a FFT will be performed after computing the cross correlation
-
-        :retruns spectralshift/mean_f (float)   : relative spectralshift
-    """
-
-    # Unpacking the signal
-    p0 = y0[0,:]
-    p1 = y1[0,:]
-
-    # Length of the signal
-    n_points = len(p0) 
-
-    # Frequency sampling
-    DF = f[-1]-f[0]     # Frequency increment
-    n  = n_points        # Sample lenght
-    sr = 1/(DF/n)       # Scan ratio
-
-    # FFT
-    p0 = np.absolute(np.fft.fft(p0)) if fft else np.absolute(p0)
-    p1 = np.absolute(np.fft.fft(p1)) if fft else np.absolute(p1)
-
-    # Normalization
-    p0 = (p0 - np.mean(p0)) / (np.std(p0) * len(p0))
-    p1 = (p1 - np.mean(p1)) / (np.std(p1))
-
-    # Cross correlation
-    corr = np.correlate(p0, p1, mode='same') if type == '1D' else signal.correlate(p0, p1, mode='same')
-
-    # Spectral shift
-    spectralshift_arr = np.linspace(-0.5*n/sr, 0.5*n/sr, n+1)
-    spectralshift = spectralshift_arr[np.argmax(corr)]
-
-
-    if display:
-
-        plt.figure()
-        plt.title('Cross correlation')
-        plt.plot(spectralshift_arr,np.interp(spectralshift_arr,np.linspace(-len(corr)/2,len(corr)/2,len(corr)),corr))
-        plt.xlabel(r'$\Delta\nu$ [GHz]')
-        plt.grid()
-
-    return -1*spectralshift/np.mean(f)
-
-if cupy_available:
-    
-    @cp.fuse(kernel_name='spectralshift')
-    def spectral_shift_GPU(p0:cp.ndarray,s0:cp.ndarray,p1:cp.ndarray,s1:cp.ndarray,z:cp.ndarray,f:cp.ndarray):
-
-        """ Function to compute the relative spectral shift in a region.
-
-            Scipy's signal.correlate is used to determine the cross correlation, then the
-            maximum position is located and related with the spectral shift trought the scan ratio
-
-            :param  p0 (cp.array)   : First signal to compare, used as reference P
-            :param  s0 (cp.array)   : First signal to compare, used as reference S
-            :param  p1 (cp.array)   : Second signal to compare P
-            :param  s1 (cp.array)   : Second signal to compare S
-            :param  z  (cp.array)   : Spatial domain x axis [m] (not used)
-            :param  f  (cp.array)   : Frequency domain x axis [GHz]
-
-            :retruns spectralshift/mean_f (float)   : relative spectralshift
-        """
-
-        # Length of the signal
-        n_points = cp.ndarray(p0).shape
-
-        print(z[0])
-
-        # Frequency sampling
-        DF = f[-1]-f[0]     # Frequency increment
-        n  = n_points        # Sample lenght
-        sr = 1/(DF/n)       # Scan ratio
-
-        # FFT
-        p0 = cp.absolute(cp.fft.fft(p0)) 
-        p1 = cp.absolute(cp.fft.fft(p1)) 
-
-        # Normalization
-        p0 = (p0 - cp.mean(p0)) / (cp.std(p0) * len(p0))
-        p1 = (p1 - cp.mean(p1)) / (cp.std(p1))
-
-        # Cross corelation
-        corr = cp.correlate(p0, p1, mode='same')
-
-        # Spectral shift
-        spectralshift_arr = cp.linspace(-0.5*n/sr, 0.5*n/sr, n+1)
-        spectralshift = spectralshift_arr[cp.argmax(corr)]
-
-        # Mean f
-        f_bar = np.mean(f.get())
-
-        return -1*spectralshift/f_bar
-
-elif not cupy_available:
-
-    def spectral_shift_GPU(p0,s0,p1,s1,z,f):
-
-        y0 = [p0,s0]
-        y1 = [p1,s1]
-
-        return spectral_shift(y0,y1,z,f,display=False,fft=True)
+import numpy as np
+
+try:
+    import cupy as cp
+    cupy_available = True
+except Exception as e:
+    print(e)
+    print('Please install cupy in order to use GPU acceleration')
+    cupy_available = False
+
+import matplotlib.pyplot as plt
+from scipy import signal
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+from UTILS.utils import printProgressBar
+
+
+""" 
+Spectral shift
+
+    This module contains functions used to compuhow te the relaive spectral shift
+    (which actually is spectralshift/central_frecuency) along an optic fiber longitude
+
+"""
+
+def spectral_shift(y0:np.ndarray,y1:np.ndarray,z:np.ndarray,f:np.ndarray,display=False,fft=True) -> float:
+    """ Function to compute the relative spectral shift in a region.
+
+        Scipy's signal.correlate is used to determine the cross correlation, then the
+        maximum position is located and related with the spectral shift trought the scan ratio
+
+        :param  y0 (np.array)   : First signal to compare, used as reference [P,S]
+        :param  y1 (np.array)   : Second signal to compare [P,S]
+        :param  z  (np.array)   : Spatial domain x axis [m] (not used)
+        :param  f  (np.array)   : Frequency domain x axis [GHz]
+
+        :optional display=False (bool) : If True, a plot with the cross correlation will be displayed 
+                                        (add  "plt.show()" or "plt.savefig()" after this funtion)
+        :optional fft=True (bool)      : If True a FFT will be performed after computing the cross correlation
+
+        :retruns spectralshift/mean_f (float)   : relative spectralshift
+    """
+
+    # Unpacking the signal
+    p0 = y0[0,:]
+    p1 = y1[0,:]
+
+    # Length of the signal
+    n_points = len(p0) 
+
+    # Frequency sampling
+    DF = f[-1]-f[0]     # Frequency increment
+    n  = n_points        # Sample lenght
+    sr = 1/(DF/n)       # Scan ratio
+
+    # FFT
+    p0 = np.absolute(np.fft.fft(p0)) if fft else np.absolute(p0)
+    p1 = np.absolute(np.fft.fft(p1)) if fft else np.absolute(p1)
+
+    # Normalization
+    p0 = (p0 - np.mean(p0)) / (np.std(p0) * len(p0))
+    p1 = (p1 - np.mean(p1)) / (np.std(p1))
+
+    # Cross correlation
+    corr = np.correlate(p0, p1, mode='same') if type == '1D' else signal.correlate(p0, p1, mode='same')
+
+    # Spectral shift
+    spectralshift_arr = np.linspace(-0.5*n/sr, 0.5*n/sr, n+1)
+    spectralshift = spectralshift_arr[np.argmax(corr)]
+
+
+    if display:
+
+        plt.figure()
+        plt.title('Cross correlation')
+        plt.plot(spectralshift_arr,np.interp(spectralshift_arr,np.linspace(-len(corr)/2,len(corr)/2,len(corr)),corr))
+        plt.xlabel(r'$\Delta\nu$ [GHz]')
+        plt.grid()
+
+    return -1*spectralshift/np.mean(f)
+
+if cupy_available:
+    
+    @cp.fuse(kernel_name='spectralshift')
+    def spectral_shift_GPU(p0:cp.ndarray,s0:cp.ndarray,p1:cp.ndarray,s1:cp.ndarray,z:cp.ndarray,f:cp.ndarray):
+
+        """ Function to compute the relative spectral shift in a region.
+
+            Scipy's signal.correlate is used to determine the cross correlation, then the
+            maximum position is located and related with the spectral shift trought the scan ratio
+
+            :param  p0 (cp.array)   : First signal to compare, used as reference P
+            :param  s0 (cp.array)   : First signal to compare, used as reference S
+            :param  p1 (cp.array)   : Second signal to compare P
+            :param  s1 (cp.array)   : Second signal to compare S
+            :param  z  (cp.array)   : Spatial domain x axis [m] (not used)
+            :param  f  (cp.array)   : Frequency domain x axis [GHz]
+
+            :retruns spectralshift/mean_f (float)   : relative spectralshift
+        """
+
+        # Length of the signal
+        n_points = cp.ndarray(p0).shape
+
+        print(z[0])
+
+        # Frequency sampling
+        DF = f[-1]-f[0]     # Frequency increment
+        n  = n_points        # Sample lenght
+        sr = 1/(DF/n)       # Scan ratio
+
+        # FFT
+        p0 = cp.absolute(cp.fft.fft(p0)) 
+        p1 = cp.absolute(cp.fft.fft(p1)) 
+
+        # Normalization
+        p0 = (p0 - cp.mean(p0)) / (cp.std(p0) * len(p0))
+        p1 = (p1 - cp.mean(p1)) / (cp.std(p1))
+
+        # Cross corelation
+        corr = cp.correlate(p0, p1, mode='same')
+
+        # Spectral shift
+        spectralshift_arr = cp.linspace(-0.5*n/sr, 0.5*n/sr, n+1)
+        spectralshift = spectralshift_arr[cp.argmax(corr)]
+
+        # Mean f
+        f_bar = np.mean(f.get())
+
+        return -1*spectralshift/f_bar
+
+elif not cupy_available:
+
+    def spectral_shift_GPU(p0,s0,p1,s1,z,f):
+
+        y0 = [p0,s0]
+        y1 = [p1,s1]
+
+        return spectral_shift(y0,y1,z,f,display=False,fft=True)
```

### Comparing `obrpy-0.1.0/obrpy/UTILS/read_OBR.py` & `obrpy-0.1.1/obrpy/UTILS/read_OBR.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-import sys
-import os
-from .utils import find_index
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-def read_OBR(file:str) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-    """
-        Function to read binaries (OBR)
-
-        param
-            file    (str): path al fichero a leer
-
-        returns
-            f       (np.array)  : Spectral distribution [GHz] (from SF to SF+FI*2*n with FI incrments)
-            z       (np.array)  : Spacial distribution  [m]
-            Pc      (complex 1xn np.array)  : p-polarization readout (spatial-domain)
-            Sc      (complex 1xn np.array)  : s-polarization readout (spatial-domain)
-
-        * Along this file some information has been commented out for a faster reading
-          please feel free of uncoment whenever you may need
-
-    """
-
-    # Lectura de datos
-
-    #FileForVer=np.fromfile(file, count=1, dtype= np.dtype('<f'))[0]                 # File format version (3.4)
-    offset = np.dtype('<f').itemsize
-
-    #ObrOfdr=np.fromfile(file, count=8,dtype= '|S1', offset = offset).astype('|U8')  # Type of file. Nosense string
-    offset += np.dtype('|U8').itemsize
-    offset = 12 # No idea why but it works
-
-    StartFreq=np.fromfile(file, count=1,dtype= np.dtype('<d'), offset = offset)[0]  # [GHz] Scan start frequency, the higher in the whole scaned spectrum
-    offset += np.dtype('<d').itemsize
-
-    SF=StartFreq
-
-    FreqIncr=np.fromfile(file, count=1,dtype= np.dtype('<d'), offset = offset)[0]   # [GHz] Frecuency increments for frequency readouts
-    offset += np.dtype('<d').itemsize
-
-    FI=FreqIncr
-
-    StartTime=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]   # [ns] Measure initial time. Represents when the outter (outter to OBR) optical fiber begins
-    offset += np.dtype('<d').itemsize
-
-    TimeIncr=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]    # [ns] Time increment
-    offset += np.dtype('<d').itemsize
-
-    dt=TimeIncr
-
-    #MeasurementType=np.fromfile(file, count=1,dtype= 'uint16',offset = offset)[0]   # Zero for reflection (backscattering) because OBR also works in transmission (I suppose)
-    offset += np.dtype('uint16').itemsize
-
-    GroupIndex=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]   # Index of refraction, arround 1.5 for silica
-    offset += np.dtype('<d').itemsize
-
-    #GainValue=np.fromfile(file, count=1,dtype= 'int32',offset = offset)[0]          # [dB] Gain 
-    offset += np.dtype('int32').itemsize
-
-    #ZeroLengthIndex=np.fromfile(file, count=1,dtype= 'int32',offset = offset)[0]    # (StartTime)/(Time_increment) Columna que le corresponde al inicio de medida de la fibra exterior al OBR
-    offset += np.dtype('int32').itemsize
-
-    #DataTypeSize=np.fromfile(file, count=1,dtype= 'uint32',offset = offset)[0]      # Number of bytes for each point (8)
-    offset += np.dtype('uint32').itemsize
-
-    nPoints=np.fromfile(file, count=1,dtype= 'uint32',offset = offset)[0]            # Number of points of readouts arrays: readout = |real part|imaginary part|
-    offset += np.dtype('uint32').itemsize
-
-    n=int(nPoints/2)                                                                 # Readout corresponding points
-
-    DateTime=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)              # Acquisition date
-    offset += np.dtype('uint16').itemsize * 8
-
-    CalibrationDate=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)       # Calibration date
-    offset += np.dtype('uint16').itemsize * 8
-
-    #TempCoeffs=np.fromfile(file, count=5,dtype= np.dtype('<d'),offset = offset)     # Temperature coeficients (for measures based on spectral shift)
-    offset += np.dtype('<d').itemsize * 5
-
-    #StrainCoeffs=np.fromfile(file, count=5,dtype= np.dtype('<d'),offset = offset)   # Deformation coeficients (for measures based on spectral shift)
-    offset += np.dtype('<d').itemsize * 5
-
-    #FreqWinFlg=np.fromfile(file, count=1,dtype= 'uint8',offset = offset)[0]         # 1 if a frecuency filter has been applied else 0
-    offset += np.dtype('uint8').itemsize
-
-    #Unused=np.fromfile(file, count=1865,dtype= 'uint8',offset = offset)             # Without use (unknown)
-    offset += np.dtype('uint8').itemsize * 1865
-
-    Preal=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Real part of p-polarization readout (already in time domain)
-    offset += np.dtype('<d').itemsize * n
-    Pimag=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Imag part of p-polarization readout (already in time domain) 
-    offset += np.dtype('<d').itemsize * n
-    Sreal=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Real part of s-polarization readout (already in time domain) 
-    offset += np.dtype('<d').itemsize * n
-    Simag=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Imag part of s-polarization readout (already in time domain) 
-    offset += np.dtype('<d').itemsize * n
-
-    # Device=np.fromfile(file, count=1, dtype= '|S1', offset = offset)[0].astype('|U8')  # Depends on filename
-
-
-    """ Posterior calculations """
-
-    GroupIndex = 1.4682                    # Modified for: Corning SMF-28e+ Optical Fiber
-
-    ### Time and frequency space
-
-    tf = (n-1)*dt                       # [ns] Final readout time, computed from total readout number of values (n)
-    t  = np.arange(0,tf+dt,dt)          # [ns] Time array with a lineal time increment until final readout time 
-    t  = t+StartTime                    # Because the equipment (OBR-4600) reads also its inner part 
-    c  = 299792458                      # [m/s] speed of light                          
-    z  = t*1e-9*((c)/(GroupIndex*2))    # [m] time in [ns] 299792458 es la velocidad de la luz en el vacio y en indice de grupo es el indice de refracción medio de la fibra
-
-    df    = FI                      # [GHz] Frequency increment
-    dw    = df*2*np.pi              # [G·rad/s] Frequency increment in radians per second
-    fl    = SF-FI*2*n               # [GHz] Lower frequency
-    fh    = SF+FI                   # [GHz] Higher frequency
-    f     = np.arange(fl,fh,df)     # [GHz] Frequency axis array
-
-    ### Measurements
-
-    Pt = Preal+Pimag*1j # p-polarization measurement in time domain
-    St = Sreal+Simag*1j # s-polarization measurement in time domain
-
-    #r = (np.abs(P)**2 + np.abs(S)**2)**0.5                                         # reflection
-    #tg = np.angle(Sw[0:-1]*np.conjugate(Sw[1:])+Pw[0:-1]*np.conjugate(Pw[1:]))/df  # group delay
-
-    return f,z,Pt,St
-
-def multi_read_OBR(files,path_to_data='.',limit1 = None,limit2 = None,display=False,n_plots_max=3) -> tuple[np.ndarray,np.ndarray,dict]:
-
-    """ Function to read multiple OBR files and crop it
-    after displaying all signals in the same plot (if display == True)
-
-    :param files        (list)      : List of files to be read (without .orb extension)
-    :param path_to_data (string)    : Path to directory which contains all OBR files
-    :param limit1       (float)     : First length to conserve in data arrays
-    :param limit2       (float)     : Last length to conserve in data arrays
-    :param display      (boolean)   : Boolean to display read data (True) or not (False)
-
-    :return f,z,Data          : Read "read_OBR" above
-                                        Data['filename'] = [P,S]
-                                        f and z are from the last lecture (asuming they are the same for all lectures)
-    """
-
-    Data = dict()
-    pending_files = list()
-    print('*Start reading')
-
-    if display == True:
-        
-        " Let's make a plot with several lines but not too much"
-
-        max_plots = min(n_plots_max,len(files)-1)
-        plt.figure()
-        for idx,file in enumerate(files):
-            print('Reading',file)
-            
-            
-            if idx < max_plots:
-                # Include plot
-                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
-                plt.plot(z,np.log10(np.absolute(Pt+St)))
-                Data[file] = [Pt,St]
-                pending_files.append(file)
-            
-            elif idx == max_plots:
-                # Last plot, display
-                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
-                plt.plot(z,np.log10(np.absolute(Pt+St)))
-                Data[file] = [Pt,St]
-                pending_files.append(file)
-                plt.xlabel('z [m]')
-                plt.ylabel(r'$Log_{10}(H(t))$')
-                plt.grid()
-                plt.show()
-
-                # Ask for limits
-                l1, l2 = ask_for_limits(limit1, limit2, z)
-
-                # Crop previous data
-                for file in pending_files:
-                    f,z,Data = crop_data(f,z,Data,file,l1,l2)
-
-            elif idx > max_plots:
-                # Will not appear
-                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
-                Data[file] = [Pt,St]
-                f,z,Data = crop_data(f,z,Data,file,l1,l2)
-            
-            else:
-                print('Error')
-
-        print('*End reading')
-
-    else:
-        for idx,file in enumerate(files):
-            print('Reading',file)
-            f,z,Pt,St = read_OBR(f'{path_to_data}/{file}.obr')
-            Data[file] = [Pt,St]
-            if idx == 0:
-                l1,l2 = ask_for_limits(limit1, limit2, z)
-            f,z,Data = crop_data(f,z,Data,file,l1,l2)
-
-        print('*End reading\n')
-
-
-    return f,z,Data
-
-def ask_for_limits(limit1:float, limit2:float, z:list) -> tuple:
-    """ Function to get the closest indexes to the start and end points specified, over an array of values
-
-    :param limit1       (float/bool)        : Start point, if 'False' or 'None' 0  will be returned
-    :param limit2       (float/bool)        : End point,   if 'False' or 'None' -1 will be returned
-    :param z            (list/np.array)     : array of values 
-
-    :return l1,l2          : Start and end (respectively) indexes of the array which matches the values specified
-
-    """
-
-    if limit1 == 'manual':
-        try:
-            l1 = float(input('First limit:'))
-        except:
-            l1 = False
-    if limit2 == 'manual':
-        try:
-            l2 = float(input('Second limit:'))
-        except:
-            l2 = False
-    
-
-    l1 = find_index(z,limit1) if limit1 is not False and limit1 is not None else 0
-    l2 = find_index(z,limit2) if limit2 is not False and limit2 is not None else -1
-
-    return l1,l2
-
-def crop_data(f:np.ndarray,z:np.ndarray,Data:list,file:str,l1:int,l2:int) -> tuple[np.ndarray, np.ndarray, list[np.ndarray]]:
-    """ Function designed to crop properly all data extracted from .obr file 
-
-    :param f,z,Data     (np.array,np.array,list of np.array)        : OBR information
-    :param file         (str)                                       : End point,   if 'False' or 'None' -1 will be returned
-    :return l1,l2       (int)                                       : Start and end (respectively) indexes of the array which matches the values specified
-
-
-    :return f,z,Data     (np.array,np.array,list of np.array)       : OBR information crop
-
-    """
-
-    for measure in range(len(Data[file])):
-        if not isinstance(Data[file][measure],list):
-            if len(Data[file][measure].shape) == 1:
-                Data[file][measure] = Data[file][measure][int(l1):int(l2)]
-            elif len(Data[file][measure].shape) == 2:
-                Data[file][measure] = Data[file][measure][:,int(l1):int(l2)]
-        else:
-            pass
-
-    f = f
-    z = z[int(l1):int(l2)]
-
-    return f,z,Data
+import sys
+import os
+from .utils import find_index
+
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+import numpy as np
+import matplotlib.pyplot as plt
+
+def read_OBR(file:str) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+    """
+        Function to read binaries (OBR)
+
+        param
+            file    (str): path al fichero a leer
+
+        returns
+            f       (np.array)  : Spectral distribution [GHz] (from SF to SF+FI*2*n with FI incrments)
+            z       (np.array)  : Spacial distribution  [m]
+            Pc      (complex 1xn np.array)  : p-polarization readout (spatial-domain)
+            Sc      (complex 1xn np.array)  : s-polarization readout (spatial-domain)
+
+        * Along this file some information has been commented out for a faster reading
+          please feel free of uncoment whenever you may need
+
+    """
+
+    # Lectura de datos
+
+    #FileForVer=np.fromfile(file, count=1, dtype= np.dtype('<f'))[0]                 # File format version (3.4)
+    offset = np.dtype('<f').itemsize
+
+    #ObrOfdr=np.fromfile(file, count=8,dtype= '|S1', offset = offset).astype('|U8')  # Type of file. Nosense string
+    offset += np.dtype('|U8').itemsize
+    offset = 12 # No idea why but it works
+
+    StartFreq=np.fromfile(file, count=1,dtype= np.dtype('<d'), offset = offset)[0]  # [GHz] Scan start frequency, the higher in the whole scaned spectrum
+    offset += np.dtype('<d').itemsize
+
+    SF=StartFreq
+
+    FreqIncr=np.fromfile(file, count=1,dtype= np.dtype('<d'), offset = offset)[0]   # [GHz] Frecuency increments for frequency readouts
+    offset += np.dtype('<d').itemsize
+
+    FI=FreqIncr
+
+    StartTime=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]   # [ns] Measure initial time. Represents when the outter (outter to OBR) optical fiber begins
+    offset += np.dtype('<d').itemsize
+
+    TimeIncr=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]    # [ns] Time increment
+    offset += np.dtype('<d').itemsize
+
+    dt=TimeIncr
+
+    #MeasurementType=np.fromfile(file, count=1,dtype= 'uint16',offset = offset)[0]   # Zero for reflection (backscattering) because OBR also works in transmission (I suppose)
+    offset += np.dtype('uint16').itemsize
+
+    GroupIndex=np.fromfile(file, count=1,dtype= np.dtype('<d'),offset = offset)[0]   # Index of refraction, arround 1.5 for silica
+    offset += np.dtype('<d').itemsize
+
+    #GainValue=np.fromfile(file, count=1,dtype= 'int32',offset = offset)[0]          # [dB] Gain 
+    offset += np.dtype('int32').itemsize
+
+    #ZeroLengthIndex=np.fromfile(file, count=1,dtype= 'int32',offset = offset)[0]    # (StartTime)/(Time_increment) Columna que le corresponde al inicio de medida de la fibra exterior al OBR
+    offset += np.dtype('int32').itemsize
+
+    #DataTypeSize=np.fromfile(file, count=1,dtype= 'uint32',offset = offset)[0]      # Number of bytes for each point (8)
+    offset += np.dtype('uint32').itemsize
+
+    nPoints=np.fromfile(file, count=1,dtype= 'uint32',offset = offset)[0]            # Number of points of readouts arrays: readout = |real part|imaginary part|
+    offset += np.dtype('uint32').itemsize
+
+    n=int(nPoints/2)                                                                 # Readout corresponding points
+
+    DateTime=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)              # Acquisition date
+    offset += np.dtype('uint16').itemsize * 8
+
+    CalibrationDate=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)       # Calibration date
+    offset += np.dtype('uint16').itemsize * 8
+
+    #TempCoeffs=np.fromfile(file, count=5,dtype= np.dtype('<d'),offset = offset)     # Temperature coeficients (for measures based on spectral shift)
+    offset += np.dtype('<d').itemsize * 5
+
+    #StrainCoeffs=np.fromfile(file, count=5,dtype= np.dtype('<d'),offset = offset)   # Deformation coeficients (for measures based on spectral shift)
+    offset += np.dtype('<d').itemsize * 5
+
+    #FreqWinFlg=np.fromfile(file, count=1,dtype= 'uint8',offset = offset)[0]         # 1 if a frecuency filter has been applied else 0
+    offset += np.dtype('uint8').itemsize
+
+    #Unused=np.fromfile(file, count=1865,dtype= 'uint8',offset = offset)             # Without use (unknown)
+    offset += np.dtype('uint8').itemsize * 1865
+
+    Preal=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Real part of p-polarization readout (already in time domain)
+    offset += np.dtype('<d').itemsize * n
+    Pimag=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Imag part of p-polarization readout (already in time domain) 
+    offset += np.dtype('<d').itemsize * n
+    Sreal=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Real part of s-polarization readout (already in time domain) 
+    offset += np.dtype('<d').itemsize * n
+    Simag=np.fromfile(file, count=n,dtype= np.dtype('<d'),offset = offset)     # Imag part of s-polarization readout (already in time domain) 
+    offset += np.dtype('<d').itemsize * n
+
+    # Device=np.fromfile(file, count=1, dtype= '|S1', offset = offset)[0].astype('|U8')  # Depends on filename
+
+
+    """ Posterior calculations """
+
+    GroupIndex = 1.4682                    # Modified for: Corning SMF-28e+ Optical Fiber
+
+    ### Time and frequency space
+
+    tf = (n-1)*dt                       # [ns] Final readout time, computed from total readout number of values (n)
+    t  = np.arange(0,tf+dt,dt)          # [ns] Time array with a lineal time increment until final readout time 
+    t  = t+StartTime                    # Because the equipment (OBR-4600) reads also its inner part 
+    c  = 299792458                      # [m/s] speed of light                          
+    z  = t*1e-9*((c)/(GroupIndex*2))    # [m] time in [ns] 299792458 es la velocidad de la luz en el vacio y en indice de grupo es el indice de refracción medio de la fibra
+
+    df    = FI                      # [GHz] Frequency increment
+    dw    = df*2*np.pi              # [G·rad/s] Frequency increment in radians per second
+    fl    = SF-FI*2*n               # [GHz] Lower frequency
+    fh    = SF+FI                   # [GHz] Higher frequency
+    f     = np.arange(fl,fh,df)     # [GHz] Frequency axis array
+
+    ### Measurements
+
+    Pt = Preal+Pimag*1j # p-polarization measurement in time domain
+    St = Sreal+Simag*1j # s-polarization measurement in time domain
+
+    #r = (np.abs(P)**2 + np.abs(S)**2)**0.5                                         # reflection
+    #tg = np.angle(Sw[0:-1]*np.conjugate(Sw[1:])+Pw[0:-1]*np.conjugate(Pw[1:]))/df  # group delay
+
+    return f,z,Pt,St
+
+def multi_read_OBR(files,path_to_data='.',limit1 = None,limit2 = None,display=False,n_plots_max=3) -> tuple[np.ndarray,np.ndarray,dict]:
+
+    """ Function to read multiple OBR files and crop it
+    after displaying all signals in the same plot (if display == True)
+
+    :param files        (list)      : List of files to be read (without .orb extension)
+    :param path_to_data (string)    : Path to directory which contains all OBR files
+    :param limit1       (float)     : First length to conserve in data arrays
+    :param limit2       (float)     : Last length to conserve in data arrays
+    :param display      (boolean)   : Boolean to display read data (True) or not (False)
+
+    :return f,z,Data          : Read "read_OBR" above
+                                        Data['filename'] = [P,S]
+                                        f and z are from the last lecture (asuming they are the same for all lectures)
+    """
+
+    Data = dict()
+    pending_files = list()
+    print('*Start reading')
+
+    if display == True:
+        
+        " Let's make a plot with several lines but not too much"
+
+        max_plots = min(n_plots_max,len(files)-1)
+        plt.figure()
+        for idx,file in enumerate(files):
+            print('Reading',file)
+            
+            
+            if idx < max_plots:
+                # Include plot
+                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
+                plt.plot(z,np.log10(np.absolute(Pt+St)))
+                Data[file] = [Pt,St]
+                pending_files.append(file)
+            
+            elif idx == max_plots:
+                # Last plot, display
+                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
+                plt.plot(z,np.log10(np.absolute(Pt+St)))
+                Data[file] = [Pt,St]
+                pending_files.append(file)
+                plt.xlabel('z [m]')
+                plt.ylabel(r'$Log_{10}(H(t))$')
+                plt.grid()
+                plt.show()
+
+                # Ask for limits
+                l1, l2 = ask_for_limits(limit1, limit2, z)
+
+                # Crop previous data
+                for file in pending_files:
+                    f,z,Data = crop_data(f,z,Data,file,l1,l2)
+
+            elif idx > max_plots:
+                # Will not appear
+                f,z,Pt,St =read_OBR(f'{path_to_data}/{file}.obr')
+                Data[file] = [Pt,St]
+                f,z,Data = crop_data(f,z,Data,file,l1,l2)
+            
+            else:
+                print('Error')
+
+        print('*End reading')
+
+    else:
+        for idx,file in enumerate(files):
+            print('Reading',file)
+            f,z,Pt,St = read_OBR(f'{path_to_data}/{file}.obr')
+            Data[file] = [Pt,St]
+            if idx == 0:
+                l1,l2 = ask_for_limits(limit1, limit2, z)
+            f,z,Data = crop_data(f,z,Data,file,l1,l2)
+
+        print('*End reading\n')
+
+
+    return f,z,Data
+
+def ask_for_limits(limit1:float, limit2:float, z:list) -> tuple:
+    """ Function to get the closest indexes to the start and end points specified, over an array of values
+
+    :param limit1       (float/bool)        : Start point, if 'False' or 'None' 0  will be returned
+    :param limit2       (float/bool)        : End point,   if 'False' or 'None' -1 will be returned
+    :param z            (list/np.array)     : array of values 
+
+    :return l1,l2          : Start and end (respectively) indexes of the array which matches the values specified
+
+    """
+
+    if limit1 == 'manual':
+        try:
+            l1 = float(input('First limit:'))
+        except:
+            l1 = False
+    if limit2 == 'manual':
+        try:
+            l2 = float(input('Second limit:'))
+        except:
+            l2 = False
+    
+
+    l1 = find_index(z,limit1) if limit1 is not False and limit1 is not None else 0
+    l2 = find_index(z,limit2) if limit2 is not False and limit2 is not None else -1
+
+    return l1,l2
+
+def crop_data(f:np.ndarray,z:np.ndarray,Data:list,file:str,l1:int,l2:int) -> tuple[np.ndarray, np.ndarray, list[np.ndarray]]:
+    """ Function designed to crop properly all data extracted from .obr file 
+
+    :param f,z,Data     (np.array,np.array,list of np.array)        : OBR information
+    :param file         (str)                                       : End point,   if 'False' or 'None' -1 will be returned
+    :return l1,l2       (int)                                       : Start and end (respectively) indexes of the array which matches the values specified
+
+
+    :return f,z,Data     (np.array,np.array,list of np.array)       : OBR information crop
+
+    """
+
+    for measure in range(len(Data[file])):
+        if not isinstance(Data[file][measure],list):
+            if len(Data[file][measure].shape) == 1:
+                Data[file][measure] = Data[file][measure][int(l1):int(l2)]
+            elif len(Data[file][measure].shape) == 2:
+                Data[file][measure] = Data[file][measure][:,int(l1):int(l2)]
+        else:
+            pass
+
+    f = f
+    z = z[int(l1):int(l2)]
+
+    return f,z,Data
```

### Comparing `obrpy-0.1.0/obrpy/UTILS/utils.py` & `obrpy-0.1.1/obrpy/UTILS/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,336 +1,336 @@
-def printProgressBar(iteration, total,prefix = 'Progress:', suffix = 'Complete', decimals = 1, length = 50, fill = '█'):
-    """
-    Call in a loop to create terminal progress bar
-    @params:
-        iteration   - Required  : current iteration (Int)
-        total       - Required  : total iterations (Int)
-        prefix      - Optional  : prefix string (Str)
-        suffix      - Optional  : suffix string (Str)
-        decimals    - Optional  : positive number of decimals in percent complete (Int)
-        length      - Optional  : character length of bar (Int)
-        fill        - Optional  : bar fill character (Str)
-    """
-    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    filledLength = int(length * iteration // total)
-    bar = fill * filledLength + '-' * (length - filledLength)
-    if float(percent) < 100:
-        print('\r%s |%s| %s%% %s' % (prefix, bar, percent, suffix), end = '\r')
-        return False
-    elif float(percent) >= 100:
-        print('\r%s |%s| %s%% %s' % (prefix, bar, percent, suffix), end = '\n')
-        return True
-    else:
-        print(percent)
-        
-
-def find_index(array,value):
-
-    """ Function to determine the closest index to some value within an array
-        
-        :param array (list) :   list to be evaluated
-        :param value (float/array):   value (or values) to reach
-
-        :return idx  (int/list)  :   index (or indexes if value is array)
-    """
-
-    import numpy as np
-
-    array = np.asarray(array)
-
-    if isinstance(value, int) or isinstance(value, float):
-        idx = (np.abs(array - value)).argmin()
-        return idx
-
-    elif isinstance(value, list) or type(value).__module__ == np.__name__:
-        idx = list()
-        for val in value:
-            idx.append((np.abs(array - val)).argmin())
-        return idx
-    else:
-        print(f'find_index() error [Type not suported: {type(value)}]')
-        exit()
-
-def get_all_files(path,verbosity = False,extension=False,file_extension='.obr'):
-    """ Get all binaries filenames from a path 
-        
-        :param: path (str): path to directory where files will be found (also within its subdirectories)
-        
-        :optional: verbosity (bool) = False : False for no prints
-        :optional: extension (bool) = False : False to not append extension in the return
-        :optional: file_extension (str) = '.obr': Extension of the files to be found
-
-        :return binaries (list): list with the path to each file (with or without extension)
-
-
-    """
-
-    import os
-
-    binaries = []
-    for root, dirs, files in os.walk(path):
-        print((len(path) - 1) * '---', os.path.basename(root)) if verbosity == True else False
-        for file in files:
-            print(len(path) * '---', file) if verbosity == True else False
-            if file.endswith(file_extension):
-                if extension == False:
-                    binaries.append(file.split('.')[0])
-                elif extension == True:
-                    binaries.append(file)
-
-    try:
-        # Split filenames and get the first number
-        order = list()
-        for file in binaries:
-            try:
-                num =  float(file.split('_')[0])
-                order.append([num , file])
-            except:
-                try:
-                    num =  float(file.split('.')[0])
-                    order.append([num , file])
-                except:
-                    pass
-        # Sort files using the num-> file correspondence  in "order"
-        if order != []:
-            binaries = [file for num,file in sorted(order, key = lambda x:x[0])]
-    except:
-        pass
-
-
-    return binaries
-
-def get_times(file):
-    """ Function to get elapsed time in (HH:MM:SS) format second column of a csv
-        where elapsed time is specified in seconds.
-
-        : param file   (string): path to file
-
-        : retrun times (np.array): array with elapsed times
-    """
-
-    import numpy as np
-    import pandas as pd
-    import time
-
-    # Read file
-    data = pd.read_csv(file, sep=',', header=None)
-
-    # Convert to numpy array
-    data = data.values
-
-    # Get values
-    elapsed_time = data[:, 1]
-    # Change format
-    times = np.array([time.strftime('%H:%M:%S', time.gmtime(t)) for t in elapsed_time])
-
-    return times
-
-def create_onedrive_directdownload(onedrive_link):
-    """ Function to create a One Drive direct download link from the sharing link generated there
-
-        :param: onedrive_link (str): One Drive sharing link generated in One Drive
-
-        :return: resultUrl (str): Direct downloadeabled link
-    """
-
-    import base64
-    data_bytes64 = base64.b64encode(bytes(onedrive_link, 'utf-8'))
-    data_bytes64_String = data_bytes64.decode('utf-8').replace('/','_').replace('+','-').rstrip("=")
-    resultUrl = f"https://api.onedrive.com/v1.0/shares/u!{data_bytes64_String}/root/content"
-    return resultUrl
-
-def find_OBR(path):
-    """ Function to find all .obr files from a folder
-
-        param: path (string): path to folder
-        return: OBR_files (list of string): list of OBR filenames
-
-    """
-    import glob
-    import os
-    # Find all .obr files
-    OBR_files = glob.glob(os.path.join(path,'0_OBR','*.obr'))
-    # Keep just filename and extension
-    OBR_files = [os.path.basename(f) for f in OBR_files]
-    return OBR_files
-
-def sort_OBR(OBR_files):
-    """ Funtion to sort OBR by the first number (before '_' splitter)
-
-        param: OBR_files (list of string) : list of OBR filenames
-        return: OBR_files (list of string) : list of OBR filenames sorted
-
-    """
-    import re
-    OBR_files.sort(key=lambda x: int(re.findall('\d+', x)[0]))
-    return OBR_files
-
-def remove_extension(OBR_files):
-
-    """ Function to remove the extension '.obr' of a bunch of '.obr' files
-
-        :param:  OBR_files (list): '.obr' files' filenames with extension
-        :return: OBR_files (list): '.obr' files' filenames without extension
-    
-    """
-
-    return [OBR_file.replace('.obr','') for OBR_file in OBR_files]
-
-def find_all_OBR(path):
-
-    """ Function to find, sort and remove extension of all '.obr' files contained in path
-    
-        :param:  path (string): path to folder
-        :return: OBR_files (list): '.obr' files' filenames without extension"""
-
-    OBR_files = find_OBR(path)
-    OBR_files = sort_OBR(OBR_files)
-    OBR_files = remove_extension(OBR_files)
-
-    return OBR_files
-
-def check_memory(percentage=90,timeout = 60):
-
-    """ Function to check memory already available
-
-        :optional percentage (float) = 90: non crossing percentage
-        :optional timeout    (float) = 60: [s] elapsed time after closing program
-
-    """
-
-    import time
-    import psutil
-
-    zero_time = float(time.time())
-    while psutil.virtual_memory()[2] > percentage:
-        print('Waiting for memory')
-        time.sleep(1)
-        if float(time.time())-zero_time > timeout:
-            exit()
-
-
-def dict_from_multiplekeys(keys,base=None):
-
-    """ Function to create two nested dictionaries with three levels of deepth.
-
-            :param: keys (list):    List (three elements for the three levels) 
-                                    of list keys which will be used as keys for dictionaries
-            :optional: base = None:     Whatever to be included in each of the lowest
-                                        level of the nested dictionaries
-
-            :return multikeys (dict):   Nested dictionary which contains labels (str) used
-                                        for the representation of the values storaged in the
-                                        other dictionary
-            :return multidict (dict):   Nested dictionary which contains 'base' in each place
-                                       
-
-        This function was created to perform signal analysis therefore the three 
-        levels are: 
-
-            magnitudes  (m)
-            domains     (d)
-            operations  (o)
-    
-        the nested dictionaries keys will be ordered as follows:
-
-            multikeys[m][d][o]
-            multidict[m][d][o]
-
-        and multikeys values are formatted as:
-            
-            if o is None:
-                multikeys[m][d][o] = m+'$($'+d+'$)$'
-            else:
-                multikeys[m][d][o] = m+'$($'+d+'$)$'+o+m+'$_0($'+d+'$)$'
-
-    """
-
-    from copy import deepcopy
-
-    if isinstance(keys[0],list):
-        magnitudes  = keys[0]
-        domains     = keys[1]
-        operations  = keys[2]
-
-        multidict = dict.fromkeys(magnitudes)
-        multikeys = dict.fromkeys(magnitudes)
-        for m in magnitudes:
-            multidict[m] = dict.fromkeys(domains)
-            multikeys[m] = dict.fromkeys(domains)
-            for d in domains:
-                multidict[m][d] = dict.fromkeys(operations)
-                multikeys[m][d] = dict.fromkeys(operations)
-                for o in operations:
-                    multidict[m][d][o] = deepcopy(base)
-                    if o is None:
-                        multikeys[m][d][o] = m+'$($'+d+'$)$'
-                    else:
-                        multikeys[m][d][o] = m+'$($'+d+'$)$'+o+m+'$_0($'+d+'$)$'
-
-    return multikeys, multidict
-
-def magnitude_interpolation(x,y=None,plot=False):
-    """ Function to interpolate a magnitude
-    
-    :optional y = None
-
-    if y is None
-        :param: x (np.array): values to be interpolated (assuming equispaced)
-        :return interp_y1 (np.array): values interpolated
-    
-    else
-        :param: x (np.array): x-axis coordinates of the values
-        :param: y (np.array): y-axis coordinates of the values
-        :return interp_y1 (np.array): y-axis values interpolated (x-axis values are the same)
-
-    :optional plot (bool) = False: Set True to visualize the interpolation stages
-
-    
-
-    """
-
-    import numpy as np
-    import matplotlib.pyplot as plt
-    from scipy.interpolate import CubicSpline
-
-    if y == None:
-        y = np.array(x)
-        x = np.linspace(0,1,len(y))
-    else:
-        y = np.array(y)
-        x = np.array(x)
-
-    step_index = np.where(np.diff(y) != 0)[0]
-    step_ini = np.append(0,step_index+1)           # Inicio del escalón
-    step_fin = np.append(step_index,len(x)-1)      # Final del escalón
-
-    step_width  = x[step_fin] - x[step_ini]        # Ancho de los escalones
-    step_center = x[step_ini] + step_width/2       # Centro de los escalones
-
-    # Linear interpolation
-
-    new_y = np.interp(x,step_center,y[step_ini])
-
-    # Cubic interpolation
-
-    new_x = np.linspace(0,1,10*len(y))
-
-    cs =  CubicSpline(x, new_y)
-    interp_y1 = np.interp(x,new_x,cs(new_x))
-
-    if plot:
-
-        plt.figure()
-        plt.plot(x,y,'-o',label='original')
-        plt.plot(x[step_ini],y[step_ini],'>',label='step_ini')
-        plt.plot(x[step_fin],y[step_fin],'<',label='step_fin')
-        plt.plot(step_center,step_width,'^',label='step_width')
-        plt.plot(step_center,y[step_ini],'-P',label='step_center')
-        plt.plot(x,new_y,'-x',label='interp1')
-        plt.plot(x,interp_y1,'-v',label='interp2')
-        plt.grid()
-        plt.legend()
-        plt.show()
-
-
-    return interp_y1
+def printProgressBar(iteration, total,prefix = 'Progress:', suffix = 'Complete', decimals = 1, length = 50, fill = '█'):
+    """
+    Call in a loop to create terminal progress bar
+    @params:
+        iteration   - Required  : current iteration (Int)
+        total       - Required  : total iterations (Int)
+        prefix      - Optional  : prefix string (Str)
+        suffix      - Optional  : suffix string (Str)
+        decimals    - Optional  : positive number of decimals in percent complete (Int)
+        length      - Optional  : character length of bar (Int)
+        fill        - Optional  : bar fill character (Str)
+    """
+    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
+    filledLength = int(length * iteration // total)
+    bar = fill * filledLength + '-' * (length - filledLength)
+    if float(percent) < 100:
+        print('\r%s |%s| %s%% %s' % (prefix, bar, percent, suffix), end = '\r')
+        return False
+    elif float(percent) >= 100:
+        print('\r%s |%s| %s%% %s' % (prefix, bar, percent, suffix), end = '\n')
+        return True
+    else:
+        print(percent)
+        
+
+def find_index(array,value):
+
+    """ Function to determine the closest index to some value within an array
+        
+        :param array (list) :   list to be evaluated
+        :param value (float/array):   value (or values) to reach
+
+        :return idx  (int/list)  :   index (or indexes if value is array)
+    """
+
+    import numpy as np
+
+    array = np.asarray(array)
+
+    if isinstance(value, int) or isinstance(value, float):
+        idx = (np.abs(array - value)).argmin()
+        return idx
+
+    elif isinstance(value, list) or type(value).__module__ == np.__name__:
+        idx = list()
+        for val in value:
+            idx.append((np.abs(array - val)).argmin())
+        return idx
+    else:
+        print(f'find_index() error [Type not suported: {type(value)}]')
+        exit()
+
+def get_all_files(path,verbosity = False,extension=False,file_extension='.obr'):
+    """ Get all binaries filenames from a path 
+        
+        :param: path (str): path to directory where files will be found (also within its subdirectories)
+        
+        :optional: verbosity (bool) = False : False for no prints
+        :optional: extension (bool) = False : False to not append extension in the return
+        :optional: file_extension (str) = '.obr': Extension of the files to be found
+
+        :return binaries (list): list with the path to each file (with or without extension)
+
+
+    """
+
+    import os
+
+    binaries = []
+    for root, dirs, files in os.walk(path):
+        print((len(path) - 1) * '---', os.path.basename(root)) if verbosity == True else False
+        for file in files:
+            print(len(path) * '---', file) if verbosity == True else False
+            if file.endswith(file_extension):
+                if extension == False:
+                    binaries.append(file.split('.')[0])
+                elif extension == True:
+                    binaries.append(file)
+
+    try:
+        # Split filenames and get the first number
+        order = list()
+        for file in binaries:
+            try:
+                num =  float(file.split('_')[0])
+                order.append([num , file])
+            except:
+                try:
+                    num =  float(file.split('.')[0])
+                    order.append([num , file])
+                except:
+                    pass
+        # Sort files using the num-> file correspondence  in "order"
+        if order != []:
+            binaries = [file for num,file in sorted(order, key = lambda x:x[0])]
+    except:
+        pass
+
+
+    return binaries
+
+def get_times(file):
+    """ Function to get elapsed time in (HH:MM:SS) format second column of a csv
+        where elapsed time is specified in seconds.
+
+        : param file   (string): path to file
+
+        : retrun times (np.array): array with elapsed times
+    """
+
+    import numpy as np
+    import pandas as pd
+    import time
+
+    # Read file
+    data = pd.read_csv(file, sep=',', header=None)
+
+    # Convert to numpy array
+    data = data.values
+
+    # Get values
+    elapsed_time = data[:, 1]
+    # Change format
+    times = np.array([time.strftime('%H:%M:%S', time.gmtime(t)) for t in elapsed_time])
+
+    return times
+
+def create_onedrive_directdownload(onedrive_link):
+    """ Function to create a One Drive direct download link from the sharing link generated there
+
+        :param: onedrive_link (str): One Drive sharing link generated in One Drive
+
+        :return: resultUrl (str): Direct downloadeabled link
+    """
+
+    import base64
+    data_bytes64 = base64.b64encode(bytes(onedrive_link, 'utf-8'))
+    data_bytes64_String = data_bytes64.decode('utf-8').replace('/','_').replace('+','-').rstrip("=")
+    resultUrl = f"https://api.onedrive.com/v1.0/shares/u!{data_bytes64_String}/root/content"
+    return resultUrl
+
+def find_OBR(path):
+    """ Function to find all .obr files from a folder
+
+        param: path (string): path to folder
+        return: OBR_files (list of string): list of OBR filenames
+
+    """
+    import glob
+    import os
+    # Find all .obr files
+    OBR_files = glob.glob(os.path.join(path,'0_OBR','*.obr'))
+    # Keep just filename and extension
+    OBR_files = [os.path.basename(f) for f in OBR_files]
+    return OBR_files
+
+def sort_OBR(OBR_files):
+    """ Funtion to sort OBR by the first number (before '_' splitter)
+
+        param: OBR_files (list of string) : list of OBR filenames
+        return: OBR_files (list of string) : list of OBR filenames sorted
+
+    """
+    import re
+    OBR_files.sort(key=lambda x: int(re.findall('\d+', x)[0]))
+    return OBR_files
+
+def remove_extension(OBR_files):
+
+    """ Function to remove the extension '.obr' of a bunch of '.obr' files
+
+        :param:  OBR_files (list): '.obr' files' filenames with extension
+        :return: OBR_files (list): '.obr' files' filenames without extension
+    
+    """
+
+    return [OBR_file.replace('.obr','') for OBR_file in OBR_files]
+
+def find_all_OBR(path):
+
+    """ Function to find, sort and remove extension of all '.obr' files contained in path
+    
+        :param:  path (string): path to folder
+        :return: OBR_files (list): '.obr' files' filenames without extension"""
+
+    OBR_files = find_OBR(path)
+    OBR_files = sort_OBR(OBR_files)
+    OBR_files = remove_extension(OBR_files)
+
+    return OBR_files
+
+def check_memory(percentage=90,timeout = 60):
+
+    """ Function to check memory already available
+
+        :optional percentage (float) = 90: non crossing percentage
+        :optional timeout    (float) = 60: [s] elapsed time after closing program
+
+    """
+
+    import time
+    import psutil
+
+    zero_time = float(time.time())
+    while psutil.virtual_memory()[2] > percentage:
+        print('Waiting for memory')
+        time.sleep(1)
+        if float(time.time())-zero_time > timeout:
+            exit()
+
+
+def dict_from_multiplekeys(keys,base=None):
+
+    """ Function to create two nested dictionaries with three levels of deepth.
+
+            :param: keys (list):    List (three elements for the three levels) 
+                                    of list keys which will be used as keys for dictionaries
+            :optional: base = None:     Whatever to be included in each of the lowest
+                                        level of the nested dictionaries
+
+            :return multikeys (dict):   Nested dictionary which contains labels (str) used
+                                        for the representation of the values storaged in the
+                                        other dictionary
+            :return multidict (dict):   Nested dictionary which contains 'base' in each place
+                                       
+
+        This function was created to perform signal analysis therefore the three 
+        levels are: 
+
+            magnitudes  (m)
+            domains     (d)
+            operations  (o)
+    
+        the nested dictionaries keys will be ordered as follows:
+
+            multikeys[m][d][o]
+            multidict[m][d][o]
+
+        and multikeys values are formatted as:
+            
+            if o is None:
+                multikeys[m][d][o] = m+'$($'+d+'$)$'
+            else:
+                multikeys[m][d][o] = m+'$($'+d+'$)$'+o+m+'$_0($'+d+'$)$'
+
+    """
+
+    from copy import deepcopy
+
+    if isinstance(keys[0],list):
+        magnitudes  = keys[0]
+        domains     = keys[1]
+        operations  = keys[2]
+
+        multidict = dict.fromkeys(magnitudes)
+        multikeys = dict.fromkeys(magnitudes)
+        for m in magnitudes:
+            multidict[m] = dict.fromkeys(domains)
+            multikeys[m] = dict.fromkeys(domains)
+            for d in domains:
+                multidict[m][d] = dict.fromkeys(operations)
+                multikeys[m][d] = dict.fromkeys(operations)
+                for o in operations:
+                    multidict[m][d][o] = deepcopy(base)
+                    if o is None:
+                        multikeys[m][d][o] = m+'$($'+d+'$)$'
+                    else:
+                        multikeys[m][d][o] = m+'$($'+d+'$)$'+o+m+'$_0($'+d+'$)$'
+
+    return multikeys, multidict
+
+def magnitude_interpolation(x,y=None,plot=False):
+    """ Function to interpolate a magnitude
+    
+    :optional y = None
+
+    if y is None
+        :param: x (np.array): values to be interpolated (assuming equispaced)
+        :return interp_y1 (np.array): values interpolated
+    
+    else
+        :param: x (np.array): x-axis coordinates of the values
+        :param: y (np.array): y-axis coordinates of the values
+        :return interp_y1 (np.array): y-axis values interpolated (x-axis values are the same)
+
+    :optional plot (bool) = False: Set True to visualize the interpolation stages
+
+    
+
+    """
+
+    import numpy as np
+    import matplotlib.pyplot as plt
+    from scipy.interpolate import CubicSpline
+
+    if y == None:
+        y = np.array(x)
+        x = np.linspace(0,1,len(y))
+    else:
+        y = np.array(y)
+        x = np.array(x)
+
+    step_index = np.where(np.diff(y) != 0)[0]
+    step_ini = np.append(0,step_index+1)           # Inicio del escalón
+    step_fin = np.append(step_index,len(x)-1)      # Final del escalón
+
+    step_width  = x[step_fin] - x[step_ini]        # Ancho de los escalones
+    step_center = x[step_ini] + step_width/2       # Centro de los escalones
+
+    # Linear interpolation
+
+    new_y = np.interp(x,step_center,y[step_ini])
+
+    # Cubic interpolation
+
+    new_x = np.linspace(0,1,10*len(y))
+
+    cs =  CubicSpline(x, new_y)
+    interp_y1 = np.interp(x,new_x,cs(new_x))
+
+    if plot:
+
+        plt.figure()
+        plt.plot(x,y,'-o',label='original')
+        plt.plot(x[step_ini],y[step_ini],'>',label='step_ini')
+        plt.plot(x[step_fin],y[step_fin],'<',label='step_fin')
+        plt.plot(step_center,step_width,'^',label='step_width')
+        plt.plot(step_center,y[step_ini],'-P',label='step_center')
+        plt.plot(x,new_y,'-x',label='interp1')
+        plt.plot(x,interp_y1,'-v',label='interp2')
+        plt.grid()
+        plt.legend()
+        plt.show()
+
+
+    return interp_y1
```

### Comparing `obrpy-0.1.0/obrpy/checkouts.py` & `obrpy-0.1.1/obrpy/checkouts.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-
-def OBR_checkout(self, verbose=True):
-
-    """ OBR checkout """
-
-    # Check if OBRfiles are already computed
-    if len(self.obrfiles.files) == 0:
-        print('No obrfiles created, creating and computing ...') if verbose else None
-        self.mainOBR()
-
-    if not any([hasattr(obrfile, 'Data') for key, obrfile in self.obrfiles.files.items()]):
-        print('No data in obrfiles, computing...') if verbose else None
-        self.computeOBR()
-    else:
-        print('OBR data already computed') if verbose else None
-        pass
-
-def slices_checkout(self):
-
-    # Check if slices were previously created
-    if not isinstance(self.slices,bool) and len(self.slices.slices) != 0 : 
-        ans = input('\nSLICES already computed (append/overwrite/quit):')
-        if 'a' in ans:
-            return True
-        if 'o' in ans:
-            self.clear_slices()
-            return True
-        if 'q' in ans:
-            return False
-    else:
-        return True
-
-def dataset_checkout(self):
-    
-    # Check if dataset already exists
-    if not isinstance(self.dataset,bool) and not self.dataset.data.empty: 
-        ans = input('\nDATASET already computed (append/overwrite/quit):')
-        if 'a' in ans:
-            return True
-        if 'o' in ans:
-            self.clear_dataset()
-            return True
-        if 'q' in ans:
-            return False
-    else:
+import os
+
+def OBR_checkout(self, verbose=True):
+
+    """ OBR checkout """
+
+    # Check if OBRfiles are already computed
+    if len(self.obrfiles.files) == 0:
+        print('No obrfiles created, creating and computing ...') if verbose else None
+        self.mainOBR()
+
+    if not any([hasattr(obrfile, 'Data') for key, obrfile in self.obrfiles.files.items()]):
+        print('No data in obrfiles, computing...') if verbose else None
+        self.computeOBR()
+    else:
+        print('OBR data already computed') if verbose else None
+        pass
+
+def slices_checkout(self):
+
+    # Check if slices were previously created
+    if not isinstance(self.slices,bool) and len(self.slices.slices) != 0 : 
+        ans = input('\nSLICES already computed (append/overwrite/quit):')
+        if 'a' in ans:
+            return True
+        if 'o' in ans:
+            self.clear_slices()
+            return True
+        if 'q' in ans:
+            return False
+    else:
+        return True
+
+def dataset_checkout(self):
+    
+    # Check if dataset already exists
+    if not isinstance(self.dataset,bool) and not self.dataset.data.empty: 
+        ans = input('\nDATASET already computed (append/overwrite/quit):')
+        if 'a' in ans:
+            return True
+        if 'o' in ans:
+            self.clear_dataset()
+            return True
+        if 'q' in ans:
+            return False
+    else:
         return True
```

### Comparing `obrpy-0.1.0/obrpy/fuego.py` & `obrpy-0.1.1/obrpy/fuego.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-
-def fuego_purificador(self):
-    """ Function which deletes every file created by the object (even the object.pkl copy)"""
-
-    files_to_burn = [
-        os.path.join(self.path,self.name),
-        self.obrfiles.book_path,
-        self.obrfiles.obj_path,
-        self.settings.book_path,
-        self.settings.obj_path,
-        self.slices.book_path,
-        self.slices.obj_path
-    ]
-
-    for file_path in files_to_burn:
-        if file_path:
-            try:
-                os.remove(file_path)
-                print(f"Deleted file: {file_path}")
-            except OSError as e:
+import os
+
+def fuego_purificador(self):
+    """ Function which deletes every file created by the object (even the object.pkl copy)"""
+
+    files_to_burn = [
+        os.path.join(self.path,self.name),
+        self.obrfiles.book_path,
+        self.obrfiles.obj_path,
+        self.settings.book_path,
+        self.settings.obj_path,
+        self.slices.book_path,
+        self.slices.obj_path
+    ]
+
+    for file_path in files_to_burn:
+        if file_path:
+            try:
+                os.remove(file_path)
+                print(f"Deleted file: {file_path}")
+            except OSError as e:
                 print(f"Error deleting file: {file_path}\n{str(e)}")
```

### Comparing `obrpy-0.1.0/obrpy/obr.py` & `obrpy-0.1.1/obrpy/obr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,205 @@
-import os
-import pandas as pd
-import numpy as np
-import glob
-
-from .UTILS.read_OBR import multi_read_OBR
-
-def mainOBR(self,limit1=None,limit2=None) -> None:
-    """ Computes the following sequence:
-            
-        * First generates OBR book from OBR filenames and the date recorded in each .obr
-                
-            self.initOBR()
-
-        * Then open each one and reads relevant information in the specified segment
-                
-            self.computeOBR(limit1,limit2)
-
-        
-        :optional limit1 (float/bool)=None: Initial point of the region of interest 
-        :optional limit2 (float/bool)=None: Final   point of the region of interest 
-    
-    """
-
-    self.initOBR()
-    self.computeOBR(limit1,limit2)
-
-def initOBR(self,auto_overwrite=False):
-    """
-    Function to generate OBR book from OBR filenames and the date recorded in each .obr
-
-        :optional: auto_overwrite (bool) = False: if True the OBRbook will be auto-overwritten
-        :returns: df (pd.Dataframe): dataframe from OBR book file
-
-    """
-
-    # Check current information
-
-    if len(self.obrfiles.files) != 0:
-        print('OBR files already registered')
-        if auto_overwrite==True:
-            print(' Auto-overwrite enabled, OBRbook will be overwitten')
-        else:
-            ans = input('\nOBR files already initialized (overwrite/quit):')
-            if 'o' in ans:
-                pass
-            if 'q' in ans:
-                return
-
-
-    # Get all OBR files
-    OBR_filenames = find_OBR(os.path.join(self.path,self.folders['OBR']))
-    
-    # Initialize dataframe
-    df = pd.DataFrame()
-
-    # Loop through OBR files saving them into obrfiles.files dict
-    for filename in OBR_filenames:
-        # Get date
-        date = get_date(os.path.join(self.path,self.folders['OBR'],filename))
-        # Get ID from date
-        ID = ID_generator(date)
-        # Append to object OBRfile
-        self.obrfiles.files[filename.replace('.obr','')] = self.OBRfile(ID,filename,date)
-        
-    print('Done!')
-
-
-def computeOBR(self,limit1=None,limit2=None) -> None:
-    """
-    Reads all .obr files and registers information: f,z and Data = [Pc,Sc,Hc]
-    among currently existing (filename, name, flecha, temperature and date)
-
-    * If RAM is not able to allocate enough memory the object will be saved and
-    by running this function a couple of times all the information will be
-    sotoraged correctly
-
-    :optional: limit1 (bool) = None
-    :optional: limit2 (bool) = None
-
-        * If both limits (limit1 and limit2) are None, a prompt will be displayed asking for them
-        * If some limit  (limit1 or  limit2) is False, no prompt will be displayed asking for them and will be assumed that the users wants to keep the whole OBR readouts 
-
-    """
-
-    # Check for region of interest
-    if limit1==None and limit2==None:
-
-        if self.settings.info['Calibration'] is None and self.settings.info['Test'] is None:
-            # If there is not settings file, display warning
-            print('WARNING: No settings found')
-            print('Please if you want to configure the DOFS settings run:')
-            print('>>     your_obrpy_object.genSettings(Calibration_df, Test_df)')
-            print('or')
-            print('>>     your_obrpy_object.genSettingsTemplate()')
-            print('edit it and then import the values with:')
-            print('>>     your_obrpy_object.import_settings("your/path/to/your/file.xslx")')
-            print('WARNING: No limits were specified')
-            print(' if you want to compute the full lenght of sensors leave empty the next prompts')
-
-            limit1 = input(' Region of interest start point [m]: ')
-            limit2 = input(' Region of interest end point [m]: ')
-
-            limit1 = False if limit1 == "" else float(limit1)
-            limit2 = False if limit2 == "" else float(limit2)
-
-        else:
-            print('No limits were specified, taking ones from seetings')
-            # Gets limits from settings
-            limit1 = self.settings.z_ini
-            limit2 = self.settings.z_fin
-
-    # Generate datasets from selected data
-    for key, OBRfile in self.obrfiles.files.items():
-
-        import psutil
-        if psutil.virtual_memory()[2] < 90:
-
-            if not hasattr(OBRfile, 'Data') or OBRfile.Data is None:
-                # Read .obr file
-                f,z,Data = multi_read_OBR([OBRfile.name],os.path.join(self.path,self.folders['OBR']),limit1=limit1,limit2=limit2)
-                # Update OBR file register
-                OBRfile.f           = f
-                OBRfile.z           = z
-                OBRfile.Data        = Data[OBRfile.name]
-            else:
-                pass
-
-        else:
-            # Esta parte hay que mejorarla para la 2.0
-            print('\nUnable to allocate more information')
-            print("DON'T PANIC the information will be saved")
-            print('just run again computeOBR() until no more .obr files are read')
-            self.save()
-            return False
-
-    print('Done!')
-    return True
-
-def find_OBR(path:str, verbose=False) -> list:
-    """ Function to find all .obr files from a folder
-
-        param:  path      (str)          : path to folder
-        return: OBR_files (list of str)  : list of OBR filenames
-
-    """
-    # Find all .obr files
-    OBR_files = glob.glob(os.path.join(path,'*.obr'))
-    print(OBR_files) if verbose else None
-    # Keep just filename and extension (basename)
-    OBR_files = [os.path.basename(f) for f in OBR_files]
-    print(OBR_files) if verbose else None
-    return OBR_files
-
-def get_date(file:str) -> str:
-    """
-    Open an .obr file to get date of the measure
-
-        param: file (str): file to be read
-        return: DateTime (str): date formated as %Y,%M,%D,%h:%m:%s
-
-    """
-
-    # Data lecture (all this offsets are heritage from read_OBR())
-    offset = np.dtype('<f').itemsize
-    offset += np.dtype('|U8').itemsize
-    offset = 12 # Ni idea de por qué este offset pero funciona
-    offset += np.dtype('<d').itemsize
-    offset += np.dtype('<d').itemsize
-    offset += np.dtype('<d').itemsize
-    offset += np.dtype('<d').itemsize
-    offset += np.dtype('uint16').itemsize
-    offset += np.dtype('<d').itemsize
-    offset += np.dtype('int32').itemsize
-    offset += np.dtype('int32').itemsize
-    offset += np.dtype('uint32').itemsize
-    offset += np.dtype('uint32').itemsize
-
-    DateTime=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)                              # Measurement date
-
-    DateTime=f'{DateTime[0]},{DateTime[1]},{DateTime[3]},{DateTime[4]}:{DateTime[5]}:{DateTime[6]}'  # "2022,03,03,13:41:27"
-
-    return DateTime
-
-def ID_generator(date:str) -> str:
-    
-    """Function to create OBRfile ID. Modifies the input date string by removing commas and colons and adds a hyphen between the day and hour.
-    
-    :param date: Date where the measure was taken, formatted as %Y,%m,%d,%H:%M:%S
-    :returns: Date formatted as %Y%m%d-%H%M%S
-    
-    """
-    
-    # Replace commas and colons with empty strings
-    formatted_date = date.replace(',', '').replace(':', '')
-    
-    # Insert a hyphen between the day and hour
-    formatted_date = formatted_date[:8] + '-' + formatted_date[8:]
-    
-    return formatted_date
+import os
+import pandas as pd
+import numpy as np
+import glob
+
+from .UTILS.read_OBR import multi_read_OBR
+
+def mainOBR(self,limit1=None,limit2=None) -> None:
+    """ Computes the following sequence:
+            
+        * First generates OBR book from OBR filenames and the date recorded in each .obr
+                
+            self.initOBR()
+
+        * Then open each one and reads relevant information in the specified segment
+                
+            self.computeOBR(limit1,limit2)
+
+        
+        :optional limit1 (float/bool)=None: Initial point of the region of interest 
+        :optional limit2 (float/bool)=None: Final   point of the region of interest 
+    
+    """
+
+    self.initOBR()
+    self.computeOBR(limit1,limit2)
+
+def initOBR(self,auto_overwrite=False, auto_quit = False) -> None:
+    """
+    Function to generate OBR book from OBR filenames and the date recorded in each .obr
+
+        :optional: auto_overwrite (bool) = False: if True the OBRbook will be auto-overwritten
+        :returns: df (pd.Dataframe): dataframe from OBR book file
+
+    """
+
+    # Check current information
+
+    if len(self.obrfiles.files) != 0:
+        print('OBR files already registered')
+        if auto_quit:
+            print('Auto-quit enabled, returning')
+            return
+        else:
+            if auto_overwrite==True:
+                print(' Auto-overwrite enabled, obrfiles will be overwitten')
+                pass
+            else:
+                ans = input('OBR files already initialized (overwrite/quit):')
+                if 'o' in ans:
+                    pass
+                if 'q' in ans:
+                    return
+
+
+    # Get all OBR files
+    OBR_filenames = find_OBR(os.path.join(self.path,self.folders['OBR']))
+    
+    # Initialize dataframe
+    df = pd.DataFrame()
+
+    # Loop through OBR files saving them into obrfiles.files dict
+    for filename in OBR_filenames:
+        # Get date
+        date = get_date(os.path.join(self.path,self.folders['OBR'],filename))
+        # Get ID from date
+        ID = ID_generator(date)
+        # Append to object OBRfile
+        self.obrfiles.files[filename.replace('.obr','')] = self.OBRfile(ID,filename,date)
+        
+    print('Done!')
+
+
+def computeOBR(self,limit1=None,limit2=None) -> None:
+    """
+    Reads all .obr files and registers information: f,z and Data = [Pc,Sc,Hc]
+    among currently existing (filename, name, flecha, temperature and date)
+
+    * If RAM is not able to allocate enough memory the object will be saved and
+    by running this function a couple of times all the information will be
+    sotoraged correctly
+
+    :optional: limit1 (bool) = None
+    :optional: limit2 (bool) = None
+
+        * If both limits (limit1 and limit2) are None, a prompt will be displayed asking for them
+        * If some limit  (limit1 or  limit2) is False, no prompt will be displayed asking for them and will be assumed that the users wants to keep the whole OBR readouts 
+
+    """
+
+    # Check for region of interest
+    if limit1==None and limit2==None:
+
+        if self.settings.z_ini is None and self.settings.z_fin is None:
+            # If there is not settings file, display warning
+            print('WARNING: No settings found')
+            print('Please if you want to configure the DOFS settings run:')
+            print('>>     your_obrpy_object.genSettings(Calibration_df, Test_df)')
+            print('or')
+            print('>>     your_obrpy_object.genSettingsTemplate()')
+            print('edit it and then import the values with:')
+            print('>>     your_obrpy_object.import_settings("your/path/to/your/file.xslx")')
+            print('WARNING: No limits were specified')
+            print(' if you want to compute the full lenght of sensors leave empty the next prompts')
+
+            limit1 = input(' Region of interest start point [m]: ')
+            limit2 = input(' Region of interest end point [m]: ')
+
+            limit1 = False if limit1 == "" else float(limit1)
+            limit2 = False if limit2 == "" else float(limit2)
+
+        else:
+            print('No limits were specified, taking ones from seetings')
+            # Gets limits from settings
+            limit1 = self.settings.z_ini
+            limit2 = self.settings.z_fin
+
+    # Generate datasets from selected data
+    for key, OBRfile in self.obrfiles.files.items():
+
+        import psutil
+        if psutil.virtual_memory()[2] < 90:
+
+            if not hasattr(OBRfile, 'Data') or OBRfile.Data is None:
+                # Read .obr file
+                f,z,Data = multi_read_OBR([OBRfile.name],os.path.join(self.path,self.folders['OBR']),limit1=limit1,limit2=limit2)
+                # Update OBR file register
+                OBRfile.f           = f
+                OBRfile.z           = z
+                OBRfile.Data        = Data[OBRfile.name]
+            else:
+                pass
+
+        else:
+            # Esta parte hay que mejorarla para la 2.0
+            print('\nUnable to allocate more information')
+            print("DON'T PANIC the information will be saved")
+            print('just run again computeOBR() until no more .obr files are read')
+            self.save()
+            return False
+
+    print('Done!')
+    return True
+
+def find_OBR(path:str, verbose=False) -> list:
+    """ Function to find all .obr files from a folder
+
+        param:  path      (str)          : path to folder
+        return: OBR_files (list of str)  : list of OBR filenames
+
+    """
+    # Find all .obr files
+    OBR_files = glob.glob(os.path.join(path,'*.obr'))
+    print(OBR_files) if verbose else None
+    # Keep just filename and extension (basename)
+    OBR_files = [os.path.basename(f) for f in OBR_files]
+    print(OBR_files) if verbose else None
+    return OBR_files
+
+def get_date(file:str) -> str:
+    """
+    Open an .obr file to get date of the measure
+
+        param: file (str): file to be read
+        return: DateTime (str): date formated as %Y,%M,%D,%h:%m:%s
+
+    """
+
+    # Data lecture (all this offsets are heritage from read_OBR())
+    offset = np.dtype('<f').itemsize
+    offset += np.dtype('|U8').itemsize
+    offset = 12 # Ni idea de por qué este offset pero funciona
+    offset += np.dtype('<d').itemsize
+    offset += np.dtype('<d').itemsize
+    offset += np.dtype('<d').itemsize
+    offset += np.dtype('<d').itemsize
+    offset += np.dtype('uint16').itemsize
+    offset += np.dtype('<d').itemsize
+    offset += np.dtype('int32').itemsize
+    offset += np.dtype('int32').itemsize
+    offset += np.dtype('uint32').itemsize
+    offset += np.dtype('uint32').itemsize
+
+    DateTime=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)                              # Measurement date
+
+    DateTime=f'{DateTime[0]},{DateTime[1]},{DateTime[3]},{DateTime[4]}:{DateTime[5]}:{DateTime[6]}'  # "2022,03,03,13:41:27"
+
+    return DateTime
+
+def ID_generator(date:str) -> str:
+    
+    """Function to create OBRfile ID. Modifies the input date string by removing commas and colons and adds a hyphen between the day and hour.
+    
+    :param date: Date where the measure was taken, formatted as %Y,%m,%d,%H:%M:%S
+    :returns: Date formatted as %Y%m%d-%H%M%S
+    
+    """
+    
+    # Replace commas and colons with empty strings
+    formatted_date = date.replace(',', '').replace(':', '')
+    
+    # Insert a hyphen between the day and hour
+    formatted_date = formatted_date[:8] + '-' + formatted_date[8:]
+    
+    return formatted_date
```

### Comparing `obrpy-0.1.0/obrpy/obrsdk/CommandProcessor.dll` & `obrpy-0.1.1/obrpy/obrsdk/CommandProcessor.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/CyUSBComm.dll` & `obrpy-0.1.1/obrpy/obrsdk/CyUSBComm.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/KL2DLL32.DLL` & `obrpy-0.1.1/obrpy/obrsdk/KL2DLL32.DLL`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/LtCore.dll` & `obrpy-0.1.1/obrpy/obrsdk/LtCore.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/LtMath.dll` & `obrpy-0.1.1/obrpy/obrsdk/LtMath.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/Phoenix.dll` & `obrpy-0.1.1/obrpy/obrsdk/Phoenix.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/RemoteInterface.dll` & `obrpy-0.1.1/obrpy/obrsdk/RemoteInterface.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/boost_date_time-mt.dll` & `obrpy-0.1.1/obrpy/obrsdk/boost_date_time-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/boost_filesystem-mt.dll` & `obrpy-0.1.1/obrpy/obrsdk/boost_filesystem-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/boost_system-mt.dll` & `obrpy-0.1.1/obrpy/obrsdk/boost_system-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/boost_thread-mt.dll` & `obrpy-0.1.1/obrpy/obrsdk/boost_thread-mt.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/libiomp5md.dll` & `obrpy-0.1.1/obrpy/obrsdk/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/obr.exe` & `obrpy-0.1.1/obrpy/obrsdk/obr.exe`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/ova32.dll` & `obrpy-0.1.1/obrpy/obrsdk/ova32.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/ova32.lib` & `obrpy-0.1.1/obrpy/obrsdk/ova32.lib`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk/ovaGUI.dll` & `obrpy-0.1.1/obrpy/obrsdk/ovaGUI.dll`

 * *Files identical despite different names*

### Comparing `obrpy-0.1.0/obrpy/obrsdk.py` & `obrpy-0.1.1/obrpy/obrsdk.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import subprocess
-import sys
-import os
-
-sys.path.append(os.path.join(os.path.dirname(__file__), 'obrsdk'))
-
-def OBRSDKcalibration(self, verbose=True) -> None:
-    """ Performs Luna's OBR-4600 calibration
-     
-        Only works in a Windows environment :( 
-    
-    """
-
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
-
-    output = subprocess.check_output(f"{exe_path} -c")
-
-    if verbose:
-        for line in output.splitlines():
-            print(line)
-
-
-def OBRSDKalignment(self,verbose=True) -> None:
-    """ Performs Luna's OBR-4600 optical alignment         
-    
-        Only works in a Windows environment :( 
-    
-    """
-
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
-    
-    output = subprocess.check_output(f"{exe_path} -a")
-
-    if verbose:
-        for line in output.splitlines():
-            print(line)
-
-def OBRSDKscan(self,filepath:str,verbose=True):
-    """ Acquires measurement
-
-        * param: filepath: path to save the .obr file
-
-        Only works in a Windows environment :( 
-
-    """
-    
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
-
-    output = subprocess.check_output(f"{exe_path} -s {filepath}")
-
-    if verbose:
-        for line in output.splitlines():
-            print(line)
-
-    return
-
-def OBRSDKextendedScan(self,filepath:str,verbose=True):
-    """ Acquires measurement in extended scan format (less precission)
-
-        * param: filepath: path to save the .obr file
-
-        Only works in a Windows environment :( 
-    
-    """
-    current_directory = os.path.dirname(os.path.abspath(__file__))
-    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
-
-    output = subprocess.check_output(f"{exe_path} -e {filepath}")
-
-    if verbose:
-        for line in output.splitlines():
-            print(line)
-
-    return
-
-    return
+import subprocess
+import sys
+import os
+
+sys.path.append(os.path.join(os.path.dirname(__file__), 'obrsdk'))
+
+def OBRSDKcalibration(self, verbose=True) -> None:
+    """ Performs Luna's OBR-4600 calibration
+     
+        Only works in a Windows environment :( 
+    
+    """
+
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
+
+    output = subprocess.check_output(f"{exe_path} -c")
+
+    if verbose:
+        for line in output.splitlines():
+            print(line)
+
+
+def OBRSDKalignment(self,verbose=True) -> None:
+    """ Performs Luna's OBR-4600 optical alignment         
+    
+        Only works in a Windows environment :( 
+    
+    """
+
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
+    
+    output = subprocess.check_output(f"{exe_path} -a")
+
+    if verbose:
+        for line in output.splitlines():
+            print(line)
+
+def OBRSDKscan(self,filepath:str,verbose=True):
+    """ Acquires measurement
+
+        * param: filepath: path to save the .obr file
+
+        Only works in a Windows environment :( 
+
+    """
+    
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
+
+    output = subprocess.check_output(f"{exe_path} -s {filepath}")
+
+    if verbose:
+        for line in output.splitlines():
+            print(line)
+
+    return
+
+def OBRSDKextendedScan(self,filepath:str,verbose=True):
+    """ Acquires measurement in extended scan format (less precission)
+
+        * param: filepath: path to save the .obr file
+
+        Only works in a Windows environment :( 
+    
+    """
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    exe_path = os.path.join(current_directory, 'obrsdk', 'obr.exe')
+
+    output = subprocess.check_output(f"{exe_path} -e {filepath}")
+
+    if verbose:
+        for line in output.splitlines():
+            print(line)
+
+    return
+
+    return
```

### Comparing `obrpy-0.1.0/obrpy/settings.py` & `obrpy-0.1.1/obrpy/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-import pandas as pd
-import os
-
-def genSettings(self,situation=None,Calibration_df=None,Test_df=None) -> None:
-    """ 
-        Generate settings object out of the setting .xlxs template created before identifies the use given to the FOS 
-        -> "Calibration" stands for calibration of the own sensor (see CalibrationTemplate() for more info)
-        -> "Test" stands for general user of FOS sensor (see TestTemplate() for further information)
-
-        * optional: situation:                      "Calibration" or "Test"
-        * optional: Calibration_df (pd.Dataframe):  generate it from getSettingsTemplates() (it's easier)
-        * optional: Test_df (pd.Dataframe):         generate it from getSettingsTemplates() (it's easier)
-                            
-    """
-
-    # Generate an object of class settings
-    self.settings = self.Settings(situation)
-
-    # Add dataframes if specified
-    self.settings.info = {
-        'Calibration': Calibration_df if isinstance(Calibration_df, pd.DataFrame) else CalibrationTemplate(),
-        'Test': Test_df if isinstance(Test_df, pd.DataFrame) else TestTemplate(self._getNewValuesFromOBRfiles())
-    }
-
-
-def getSettingsTemplates(self) -> tuple:
-
-    """ 
-        Return settings templates for user usage 
-    
-        * return: calibration_data(pd.Dataframe), test_data (pd.DataFrame)
-    
-    """
-
-    # create the "Calibration" sheet
-    calibration_data = CalibrationTemplate()
-
-    # create the "Test" sheet
-    new_values = self._getNewValuesFromOBRfiles() 
-    test_data = TestTemplate(new_values)
-
-
-    return calibration_data, test_data
-
-
-def CalibrationTemplate() -> pd.DataFrame:
-    """ 
-        Generates a tempate datafreme used to generate the seetings for the calibration situation.
-        In the calibration situation the microstrain (Delta eps) and temperature (Delta T) 
-        are asumed to vary in a linerar way, and only one segment (from z_ini->x=0 to z_fin)
-        of the fiber is subjected to these variations.
-
-    """
-
-    data = [
-        ['Delta T = ','','+ ','','x [m]'],
-        ['Delta eps = ','','+ ','','x [m]'],
-        ['z_ini [m] =',''],
-        ['z_fin [m] =','']
-    ]
-    df = pd.DataFrame(data)
-    return df
-
-def TestTemplate(new_values) -> pd.DataFrame:
-    """ 
-        Generates a template dataframe used to generate the seetings for a situation where 
-        several measurements are performed during a process where some magnitudes vary e.g. 
-        load, temperature, time, ...
-
-        *param: new_values(list) 
-    """
-    
-    columns = ['Units','xlabel','ylabel']
-    df = pd.DataFrame(columns=columns, index=new_values)
-
-    return df
-
-def _getNewValuesFromOBRfiles(self) -> list:
-    
-    """ 
-        Get the new values written in the OBRbook by the user.
-
-    """
-    df = self.obrfiles.create_book()
-
-    # Get the column names
-    column_names = df.columns.tolist()
-
-    # Remove the old ones
-    column_names.remove('ID')
-    column_names.remove('filename')
-    column_names.remove('date')
-    column_names.remove('f')
-    column_names.remove('z')
-    column_names.remove('Data')
-
-    return column_names
+import pandas as pd
+import os
+
+def genSettings(self,situation=None,Calibration_df=None,Test_df=None) -> None:
+    """ 
+        Generate settings object out of the setting .xlxs template created before identifies the use given to the FOS 
+        -> "Calibration" stands for calibration of the own sensor (see CalibrationTemplate() for more info)
+        -> "Test" stands for general user of FOS sensor (see TestTemplate() for further information)
+
+        * optional: situation:                      "Calibration" or "Test"
+        * optional: Calibration_df (pd.Dataframe):  generate it from getSettingsTemplates() (it's easier)
+        * optional: Test_df (pd.Dataframe):         generate it from getSettingsTemplates() (it's easier)
+                            
+    """
+
+    # Clear settings
+    self.settings = self.Settings(situation)
+
+    # Add dataframes if specified
+    self.settings.book = {
+        'Calibration': Calibration_df if isinstance(Calibration_df, pd.DataFrame) else CalibrationTemplate(),
+        'Test': Test_df if isinstance(Test_df, pd.DataFrame) else TestTemplate(self._getNewValuesFromOBRfiles())
+    }
+
+
+def getSettingsTemplates(self) -> tuple:
+
+    """ 
+        Return settings templates for user usage 
+    
+        * return: calibration_data(pd.Dataframe), test_data (pd.DataFrame)
+    
+    """
+
+    # create the "Calibration" sheet
+    calibration_data = CalibrationTemplate()
+
+    # create the "Test" sheet
+    new_values = self._getNewValuesFromOBRfiles() 
+    test_data = TestTemplate(new_values)
+
+
+    return calibration_data, test_data
+
+
+def CalibrationTemplate() -> pd.DataFrame:
+    """ 
+        Generates a tempate datafreme used to generate the seetings for the calibration situation.
+        In the calibration situation the microstrain (Delta eps) and temperature (Delta T) 
+        are asumed to vary in a linerar way, and only one segment (from z_ini->x=0 to z_fin)
+        of the fiber is subjected to these variations.
+
+    """
+
+    data = [
+        ['Delta T = ','','+ ','','x [m]'],
+        ['Delta eps = ','','+ ','','x [m]'],
+        ['z_ini [m] =',''],
+        ['z_fin [m] =','']
+    ]
+    df = pd.DataFrame(data)
+    return df
+
+def TestTemplate(new_values) -> pd.DataFrame:
+    """ 
+        Generates a template dataframe used to generate the seetings for a situation where 
+        several measurements are performed during a process where some magnitudes vary e.g. 
+        load, temperature, time, ...
+
+        *param: new_values(list) 
+    """
+    
+    columns = ['Units','xlabel','ylabel']
+    df = pd.DataFrame(columns=columns, index=new_values)
+
+    return df
+
+def _getNewValuesFromOBRfiles(self) -> list:
+    
+    """ 
+        Get the new values written in the OBRbook by the user.
+
+    """
+
+    df = self.obrfiles.create_book()
+
+    # Get the column names
+    column_names = df.columns.tolist()
+
+    # Remove the old ones
+    try:
+        column_names.remove('ID')
+        column_names.remove('filename')
+        column_names.remove('date')
+        column_names.remove('f')
+        column_names.remove('z')
+        column_names.remove('Data')
+        return column_names
+    
+    except Exception as e:
+        if 'list.remove(x): x not in list' == str(e):
+            return list()
+        else:
+            raise e
+
+
```

### Comparing `obrpy-0.1.0/obrpy/take_a_look.py` & `obrpy-0.1.1/obrpy/take_a_look.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import sys
-import os
-import matplotlib.pyplot as plt
-import numpy as np
-
-def take_a_look(self):
-    pass
-
-"""
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-from UTILS.read_OBR import multi_read_OBR
-from SIGNAL.spectral_shift import global_spectral_shift
-from SIGNAL.cross_spectrum import global_cross_spectrum_SS
-
-def take_a_look(self,REF,files,limit1=0, limit2 = 20, delta = 300, window = 1000, val='ss',plot=True, common_origin=False):
-
-    # Get reference
-    if isinstance(REF,list):
-        refData = list()
-        for i,r in enumerate(REF):
-            f,z,Data = multi_read_obr([r],os.path.join(self.path,self.folders['0_OBR']),limit1=limit1[i],limit2=limit2[i])
-            refData.append(Data[r])
-        reftype = 'multiple'
-    else:
-        f,z,Data = multi_read_obr([REF],os.path.join(self.path,self.folders['0_OBR']),limit1=limit1,limit2=limit2)
-        refData = Data[REF]
-        reftype = 'single'
-
-
-    # Get distributions
-    val_distributions = list()
-    z_distributions = list()
-    for i,file in enumerate(files):
-        if reftype == 'single':
-            r  = refData
-            l1 = limit1
-            l2 = limit2
-        elif reftype == 'multiple':
-            r  = refData[i]
-            l1 = limit1[i]
-            l2 = limit2[i]
-
-        f,z,Data = multi_read_obr([file],os.path.join(self.path,self.folders['0_OBR']),limit1=l1,limit2=l2)
-        if val == 'ss':
-            spectralshift = global_spectral_shift(r[0],Data[file][0],f,delta=delta,window=window)
-            val_distribution = spectralshift
-            ylabel = r'$-\frac{\Delta \nu}{\bar{\nu}}$'
-        elif val == 'brf':
-            brf = birefringence(Data[file],f,delta=delta,window=window)
-            val_distribution = brf
-            ylabel = r'$\theta$'
-        elif val == 'temp':
-            T,E = self.sensor(Data[file],r,f,delta=delta,window=window,display = False)
-            val_distribution = T
-            ylabel = r'$\Delta T$[K]'
-        elif val == 'def':
-            #T,E = self.sensor(Data[file],r,f,delta=delta,window=window,display = False)
-            spectralshift = global_spectral_shift(r[0],Data[file][0],f,delta=delta,window=window)
-            E = spectralshift * 189394.17022471415 * -6.6680 * -8.80840637e2/119.88246527477283
-            val_distribution = E
-            ylabel = r'$\Delta \mu \varepsilon$'
-
-        val_distributions.append(val_distribution)
-        z_distributions.append(np.linspace(z[0],z[-1],len(val_distribution)))
-
-
-    # Plot
-    if plot:
-        plt.figure()
-        for file, val, z in zip(files, val_distributions, z_distributions):
-            lbl = file.replace('_',' ')
-            z = z-z[0] if common_origin else z
-            #plt.plot(z,val,'o',markersize=0.75,label=f'{lbl}')
-            plt.plot(z,val,label=f'{lbl}')
-        plt.ylabel(ylabel,fontsize=20,labelpad=15).set_rotation(0) if val == 'ss' else plt.ylabel(ylabel,fontsize=10,labelpad=8).set_rotation(0)
-        plt.xlabel('z [m]')
-
-        """ """
-        lgnd = plt.legend(numpoints=1, fontsize=10)
-
-        #change the marker size manually for both lines
-        lgnd.legendHandles[0]._legmarker.set_markersize(6)
-        lgnd.legendHandles[1]._legmarker.set_markersize(6)
-        lgnd.legendHandles[2]._legmarker.set_markersize(6)
-        """ """
-        plt.legend()
-        plt.grid()
-        plt.show()
-
-    return val_distributions
-
+import sys
+import os
+import matplotlib.pyplot as plt
+import numpy as np
+
+def take_a_look(self):
+    pass
+
+"""
+
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+from UTILS.read_OBR import multi_read_OBR
+from SIGNAL.spectral_shift import global_spectral_shift
+from SIGNAL.cross_spectrum import global_cross_spectrum_SS
+
+def take_a_look(self,REF,files,limit1=0, limit2 = 20, delta = 300, window = 1000, val='ss',plot=True, common_origin=False):
+
+    # Get reference
+    if isinstance(REF,list):
+        refData = list()
+        for i,r in enumerate(REF):
+            f,z,Data = multi_read_obr([r],os.path.join(self.path,self.folders['0_OBR']),limit1=limit1[i],limit2=limit2[i])
+            refData.append(Data[r])
+        reftype = 'multiple'
+    else:
+        f,z,Data = multi_read_obr([REF],os.path.join(self.path,self.folders['0_OBR']),limit1=limit1,limit2=limit2)
+        refData = Data[REF]
+        reftype = 'single'
+
+
+    # Get distributions
+    val_distributions = list()
+    z_distributions = list()
+    for i,file in enumerate(files):
+        if reftype == 'single':
+            r  = refData
+            l1 = limit1
+            l2 = limit2
+        elif reftype == 'multiple':
+            r  = refData[i]
+            l1 = limit1[i]
+            l2 = limit2[i]
+
+        f,z,Data = multi_read_obr([file],os.path.join(self.path,self.folders['0_OBR']),limit1=l1,limit2=l2)
+        if val == 'ss':
+            spectralshift = global_spectral_shift(r[0],Data[file][0],f,delta=delta,window=window)
+            val_distribution = spectralshift
+            ylabel = r'$-\frac{\Delta \nu}{\bar{\nu}}$'
+        elif val == 'brf':
+            brf = birefringence(Data[file],f,delta=delta,window=window)
+            val_distribution = brf
+            ylabel = r'$\theta$'
+        elif val == 'temp':
+            T,E = self.sensor(Data[file],r,f,delta=delta,window=window,display = False)
+            val_distribution = T
+            ylabel = r'$\Delta T$[K]'
+        elif val == 'def':
+            #T,E = self.sensor(Data[file],r,f,delta=delta,window=window,display = False)
+            spectralshift = global_spectral_shift(r[0],Data[file][0],f,delta=delta,window=window)
+            E = spectralshift * 189394.17022471415 * -6.6680 * -8.80840637e2/119.88246527477283
+            val_distribution = E
+            ylabel = r'$\Delta \mu \varepsilon$'
+
+        val_distributions.append(val_distribution)
+        z_distributions.append(np.linspace(z[0],z[-1],len(val_distribution)))
+
+
+    # Plot
+    if plot:
+        plt.figure()
+        for file, val, z in zip(files, val_distributions, z_distributions):
+            lbl = file.replace('_',' ')
+            z = z-z[0] if common_origin else z
+            #plt.plot(z,val,'o',markersize=0.75,label=f'{lbl}')
+            plt.plot(z,val,label=f'{lbl}')
+        plt.ylabel(ylabel,fontsize=20,labelpad=15).set_rotation(0) if val == 'ss' else plt.ylabel(ylabel,fontsize=10,labelpad=8).set_rotation(0)
+        plt.xlabel('z [m]')
+
+        """ """
+        lgnd = plt.legend(numpoints=1, fontsize=10)
+
+        #change the marker size manually for both lines
+        lgnd.legendHandles[0]._legmarker.set_markersize(6)
+        lgnd.legendHandles[1]._legmarker.set_markersize(6)
+        lgnd.legendHandles[2]._legmarker.set_markersize(6)
+        """ """
+        plt.legend()
+        plt.grid()
+        plt.show()
+
+    return val_distributions
+
 """
```

### Comparing `obrpy-0.1.0/setup.py` & `obrpy-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import pathlib
-from setuptools import find_packages, setup
-
-HERE = pathlib.Path(__file__).parent
-
-VERSION = '0.1.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
-PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
-AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
-AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
-URL = 'https://github.com/temisAP' #Modificar con vuestros datos
-
-LICENSE = 'MIT' #Tipo de licencia
-DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
-LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
-LONG_DESC_TYPE = "text/markdown"
-
-
-# Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
-# Path to the requirements.txt file
-requirements_path = "requirements.txt"
-
-# Initialize the INSTALL_REQUIRES list
-INSTALL_REQUIRES = []
-
-# Read the requirements.txt file
-with open(requirements_path, "r", encoding='utf-16') as file:
-    requirements = file.read().splitlines()
-
-#print([r for r in requirements])
-
-# Exclude "cupy" from the requirements and add the rest to INSTALL_REQUIRES
-for requirement in requirements:
-    
-    # Split the requirement at the "==" sign and extract the library name
-    library_name = requirement.split("==")[0].strip()
-    if library_name != "cupy":
-        INSTALL_REQUIRES.append(library_name)
-
-
-setup(
-    name=PACKAGE_NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type=LONG_DESC_TYPE,
-    author=AUTHOR,
-    author_email=AUTHOR_EMAIL,
-    url=URL,
-    install_requires=INSTALL_REQUIRES,
-    license=LICENSE,
-    packages=find_packages(),
-    package_data={'obrpy':['UTILS/*','ANALYSIS/*','obrsdk/*','signal/*']},
-    include_package_data=True
+import pathlib
+from setuptools import find_packages, setup
+
+HERE = pathlib.Path(__file__).parent
+
+VERSION = '0.1.1' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
+AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
+AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
+URL = 'https://github.com/temisAP' #Modificar con vuestros datos
+
+LICENSE = 'MIT' #Tipo de licencia
+DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
+LONG_DESCRIPTION = (HERE / "readme.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
+LONG_DESC_TYPE = "text/markdown"
+
+
+# Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
+# Path to the requirements.txt file
+requirements_path = "requirements.txt"
+
+# Initialize the INSTALL_REQUIRES list
+INSTALL_REQUIRES = []
+
+# Read the requirements.txt file
+with open(requirements_path, "r", encoding='utf-16') as file:
+    requirements = file.read().splitlines()
+
+#print([r for r in requirements])
+
+# Exclude "cupy" from the requirements and add the rest to INSTALL_REQUIRES
+for requirement in requirements:
+    
+    # Split the requirement at the "==" sign and extract the library name
+    library_name = requirement.split("==")[0].strip()
+    if library_name != "cupy":
+        INSTALL_REQUIRES.append(library_name)
+
+
+setup(
+    name=PACKAGE_NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type=LONG_DESC_TYPE,
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    url=URL,
+    install_requires=INSTALL_REQUIRES,
+    license=LICENSE,
+    packages=find_packages(),
+    package_data={'obrpy':['UTILS/*','ANALYSIS/*','obrsdk/*','signal/*']},
+    include_package_data=True
 )
```

### Comparing `obrpy-0.1.0/test/test.py` & `obrpy-0.1.1/test/test.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from obrpy import obrpy
-
-obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-obrpy_obj.mainOBR()
-obrpy_obj.genSettings("Calibration")
-
-input('Open OBRbook, add T0, T1, E0 and E1 columns. Open seetings, write the name of the columns in settings. Once finished press any key to continue')
-
-obrpy_obj.update_OBRbook()
-obrpy_obj.update_OBRfiles()
-obrpy_obj.update_settings()
-
-obrpy_obj.genSlices()
-
-exit()
-
-Y0 = obrpy_obj.OBRfiles['2'].Data
-Y1 = obrpy_obj.OBRfiles['B11'].Data
-F =  obrpy_obj.OBRfiles['2'].f
-Z =  obrpy_obj.OBRfiles['2'].z
-
-import numpy as np
-Y0 = np.array(Y0)
-Y0 = Y0[:,0:5000]
-
-Y1 = np.array(Y1)
-Y1 = Y1[:,0:5000]
-
-Z = np.array(Z)
-Z = Z[0:5000]
-
-
-
-out = obrpy_obj.global_analysis_GPU(Y0, Y1, Z, F, local_function=obrpy_obj.Signal.spectral_shift_GPU, point=1)
-
-
-import matplotlib.pyplot as plt
-
-plt.figure()
-plt.plot(Z,out)
-plt.grid()
-plt.show()
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from obrpy import obrpy
+
+obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+obrpy_obj.mainOBR()
+obrpy_obj.genSettings("Calibration")
+
+input('Open OBRbook, add T0, T1, E0 and E1 columns. Open seetings, write the name of the columns in settings. Once finished press any key to continue')
+
+obrpy_obj.update_OBRbook()
+obrpy_obj.update_OBRfiles()
+obrpy_obj.update_settings()
+
+obrpy_obj.genSlices()
+
+exit()
+
+Y0 = obrpy_obj.OBRfiles['2'].Data
+Y1 = obrpy_obj.OBRfiles['B11'].Data
+F =  obrpy_obj.OBRfiles['2'].f
+Z =  obrpy_obj.OBRfiles['2'].z
+
+import numpy as np
+Y0 = np.array(Y0)
+Y0 = Y0[:,0:5000]
+
+Y1 = np.array(Y1)
+Y1 = Y1[:,0:5000]
+
+Z = np.array(Z)
+Z = Z[0:5000]
+
+
+
+out = obrpy_obj.global_analysis_GPU(Y0, Y1, Z, F, local_function=obrpy_obj.Signal.spectral_shift_GPU, point=1)
+
+
+import matplotlib.pyplot as plt
+
+plt.figure()
+plt.plot(Z,out)
+plt.grid()
+plt.show()
```

### Comparing `obrpy-0.1.0/test/test_dataset.py` & `obrpy-0.1.1/test/test_dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from obrpy import obrpy
-import pandas as pd
-import numpy as np
-
-obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-
-def layer0(ID, slice0, slice1):
-    
-    P0 = slice0.loc["P"]
-    P1 = slice1.loc["P"]
-
-    T0 = slice0.loc["T"]
-    T1 = slice1.loc["T"]
-    E0 = slice0.loc["E"]
-    E1 = slice1.loc["E"]
-
-    p0 = np.absolute(np.fft.fft(P0))
-    p1 = np.absolute(np.fft.fft(P1))
-
-    corr = np.correlate(p0, p1, mode='same')
-    corr = [0,2,3,4]
-    y = [T0-T1, E0-E1]
-
-    #new_row = [ID] + [slice0.loc["ID"]] + [slice1.loc["ID"]] + corr.tolist() + y
-    new_row = [ID] + [slice0.loc["ID"]] + [slice1.loc["ID"]] + corr + y
-
-    Xcolumns = [i+3 for i in range(0,len(corr)+1)]
-    Ycolumns = [len(corr)+3+1, len(corr)+3+2]
-    
-    return Xcolumns, Ycolumns, new_row
-
-ds = obrpy_obj.genDataset(layer0)
-
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from obrpy import obrpy
+import pandas as pd
+import numpy as np
+
+obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+
+def layer0(ID, slice0, slice1):
+    
+    P0 = slice0.loc["P"]
+    P1 = slice1.loc["P"]
+
+    T0 = slice0.loc["T"]
+    T1 = slice1.loc["T"]
+    E0 = slice0.loc["E"]
+    E1 = slice1.loc["E"]
+
+    p0 = np.absolute(np.fft.fft(P0))
+    p1 = np.absolute(np.fft.fft(P1))
+
+    #corr = np.correlate(p0, p1, mode='same')
+    
+    X = [0,2,3,4]
+    Y = [T0-T1, E0-E1]
+
+    #new_row = [ID] + [slice0.loc["ID"]] + [slice1.loc["ID"]] + corr.tolist() + y
+    new_row = [ID] + [slice0.loc["ID"]] + [slice1.loc["ID"]] + X + Y
+
+    Xcolumns = [3+i for i in range(0,len(X))]
+    Ycolumns = [3+len(X)+i for i in range(0,len(Y))]
+    
+    return Xcolumns, Ycolumns, new_row
+
+ds = obrpy_obj.genDataset(layer0)
+
 print(ds)
```

### Comparing `obrpy-0.1.0/test/test_export_obrfiles.py` & `obrpy-0.1.1/test/test_export_obrfiles.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-###
-
-import pandas as pd
-from obrpy import obrpy
-import matplotlib.pyplot as plt
-
-test1 = False
-test2 = False
-test3 = True
-test4 = False
-
-if test1:
-
-    """ TEST 1: OBRfiles book with GUI """
-
-    # Create object
-    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-    # Create OBRbook
-    obrpy_obj.initOBR()
-
-    # Create settings
-    obrpy_obj.genSettings()
-    obrpy_obj.settings.z_ini = 0.1
-    obrpy_obj.settings.z_fin = 0.5
-
-    # Compute OBRfiles (with limits from settings)
-    obrpy_obj.computeOBR()
-
-    # Export obrfiles to .csv using GUI
-    obrpy_obj.obrfiles.export_book()
-
-    # Delete pkl
-    obrpy_obj.fuego_purificador()
-
-if test2:
-
-    """ TEST 2: OBRfiles book without GUI """
-
-    # Create object
-    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-    # Create OBRbook
-    obrpy_obj.initOBR()
-
-    # Create settings
-    obrpy_obj.genSettings()
-    obrpy_obj.settings.z_ini = 0.1
-    obrpy_obj.settings.z_fin = 0.5
-
-    # Compute OBRfiles (with limits from settings)
-    obrpy_obj.computeOBR()
-
-    # Export obrfiles to .csv
-    obrpy_obj.obrfiles.export_book('./here.csv')
-
-    # Delete pkl
-    obrpy_obj.fuego_purificador()
-
-
-if test3:
-
-    """ TEST 3: OBRfiles as object with GUI """
-
-    # Create object
-    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-    # Create OBRbook
-    obrpy_obj.initOBR()
-
-    # Create settings
-    obrpy_obj.genSettings()
-    obrpy_obj.settings.z_ini = 0.1
-    obrpy_obj.settings.z_fin = 0.5
-
-    # Compute OBRfiles (with limits from settings)
-    obrpy_obj.computeOBR()
-
-    # Export obrfiles to .csv using GUI
-    obrpy_obj.obrfiles.export_obj()
-
-    # Delete pkl
-    obrpy_obj.fuego_purificador()
-
-if test4:
-
-    """ TEST 4: OBRfiles as object without GUI """
-
-    # Create object
-    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-    # Create OBRbook
-    obrpy_obj.initOBR()
-
-    # Create settings
-    obrpy_obj.genSettings()
-    obrpy_obj.settings.z_ini = 0.1
-    obrpy_obj.settings.z_fin = 0.5
-
-    # Compute OBRfiles (with limits from settings)
-    obrpy_obj.computeOBR()
-
-    # Export obrfiles to .pkl
-    obrpy_obj.obrfiles.export_obj('./here.pkl')
-
-    # Delete pkl
-    obrpy_obj.fuego_purificador()
-
-
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+###
+
+import pandas as pd
+from obrpy import obrpy
+import matplotlib.pyplot as plt
+
+test1 = False
+test2 = False
+test3 = True
+test4 = False
+
+if test1:
+
+    """ TEST 1: OBRfiles book with GUI """
+
+    # Create object
+    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+    # Create OBRbook
+    obrpy_obj.initOBR()
+
+    # Create settings
+    obrpy_obj.genSettings()
+    obrpy_obj.settings.z_ini = 0.1
+    obrpy_obj.settings.z_fin = 0.5
+
+    # Compute OBRfiles (with limits from settings)
+    obrpy_obj.computeOBR()
+
+    # Export obrfiles to .csv using GUI
+    obrpy_obj.obrfiles.export_book()
+
+    # Delete pkl
+    obrpy_obj.fuego_purificador()
+
+if test2:
+
+    """ TEST 2: OBRfiles book without GUI """
+
+    # Create object
+    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+    # Create OBRbook
+    obrpy_obj.initOBR()
+
+    # Create settings
+    obrpy_obj.genSettings()
+    obrpy_obj.settings.z_ini = 0.1
+    obrpy_obj.settings.z_fin = 0.5
+
+    # Compute OBRfiles (with limits from settings)
+    obrpy_obj.computeOBR()
+
+    # Export obrfiles to .csv
+    obrpy_obj.obrfiles.export_book('./here.csv')
+
+    # Delete pkl
+    obrpy_obj.fuego_purificador()
+
+
+if test3:
+
+    """ TEST 3: OBRfiles as object with GUI """
+
+    # Create object
+    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+    # Create OBRbook
+    obrpy_obj.initOBR()
+
+    # Create settings
+    obrpy_obj.genSettings()
+    obrpy_obj.settings.z_ini = 0.1
+    obrpy_obj.settings.z_fin = 0.5
+
+    # Compute OBRfiles (with limits from settings)
+    obrpy_obj.computeOBR()
+
+    # Export obrfiles to .csv using GUI
+    obrpy_obj.obrfiles.export_obj()
+
+    # Delete pkl
+    obrpy_obj.fuego_purificador()
+
+if test4:
+
+    """ TEST 4: OBRfiles as object without GUI """
+
+    # Create object
+    obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+    # Create OBRbook
+    obrpy_obj.initOBR()
+
+    # Create settings
+    obrpy_obj.genSettings()
+    obrpy_obj.settings.z_ini = 0.1
+    obrpy_obj.settings.z_fin = 0.5
+
+    # Compute OBRfiles (with limits from settings)
+    obrpy_obj.computeOBR()
+
+    # Export obrfiles to .pkl
+    obrpy_obj.obrfiles.export_obj('./here.pkl')
+
+    # Delete pkl
+    obrpy_obj.fuego_purificador()
+
+
```

### Comparing `obrpy-0.1.0/test/test_slices.py` & `obrpy-0.1.1/test/test_slices.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import sys
-import os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from obrpy import obrpy
-
-obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
-
-# Create OBRbook 
-obrpy_obj.initOBR()
-
-# Create settings
-obrpy_obj.genSettings()
-
-# Compute OBRfiles (with limits from settings)
-obrpy_obj.settings.z_ini = 0.1
-obrpy_obj.settings.z_fin = 0.5
-obrpy_obj.computeOBR()
-
-# Add values to OBRfiles 
-i = 0
-for key, val in obrpy_obj.obrfiles.files.items():
-    i += 1
-    val.T0 = 1 + i
-    val.T1 = 2 + 2*i
-    val.E0 = 3 + 3*i
-    val.E1 = 4 + 4*i
-
-
-# Gen slices out of OBRfiles
-obrpy_obj.genSlices()
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from obrpy import obrpy
+
+obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
+
+# Create OBRbook 
+obrpy_obj.initOBR()
+
+# Create settings
+obrpy_obj.genSettings()
+
+# Compute OBRfiles (with limits from settings)
+obrpy_obj.settings.z_ini = 0.1
+obrpy_obj.settings.z_fin = 0.5
+obrpy_obj.computeOBR()
+
+# Add values to OBRfiles 
+i = 0
+for key, val in obrpy_obj.obrfiles.files.items():
+    i += 1
+    val.T0 = 1 + i
+    val.T1 = 2 + 2*i
+    val.E0 = 3 + 3*i
+    val.E1 = 4 + 4*i
+
+
+# Gen slices out of OBRfiles
+obrpy_obj.genSlices()
 obrpy_obj.save()
```

