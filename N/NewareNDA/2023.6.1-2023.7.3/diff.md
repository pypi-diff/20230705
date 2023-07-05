# Comparing `tmp/NewareNDA-2023.6.1.tar.gz` & `tmp/NewareNDA-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewareNDA-2023.6.1.tar", last modified: Thu Jun  1 15:09:53 2023, max compression
+gzip compressed data, was "NewareNDA-2023.7.3.tar", last modified: Wed Jul  5 21:39:11 2023, max compression
```

## Comparing `NewareNDA-2023.6.1.tar` & `NewareNDA-2023.7.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-06-01 15:09:53.676402 NewareNDA-2023.6.1/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 NewareNDA-2023.6.1/LICENSE
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-06-01 15:09:53.672402 NewareNDA-2023.6.1/NewareNDA/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     7397 2023-06-01 15:00:41.000000 NewareNDA-2023.6.1/NewareNDA/NewareNDA.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       61 2023-05-26 18:03:59.000000 NewareNDA-2023.6.1/NewareNDA/__init__.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2023-06-01 15:00:41.000000 NewareNDA-2023.6.1/NewareNDA/version.py
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-06-01 15:09:53.676402 NewareNDA-2023.6.1/NewareNDA.egg-info/
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1030 2023-06-01 15:09:53.000000 NewareNDA-2023.6.1/NewareNDA.egg-info/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      277 2023-06-01 15:09:53.000000 NewareNDA-2023.6.1/NewareNDA.egg-info/SOURCES.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2023-06-01 15:09:53.000000 NewareNDA-2023.6.1/NewareNDA.egg-info/dependency_links.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        7 2023-06-01 15:09:53.000000 NewareNDA-2023.6.1/NewareNDA.egg-info/requires.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2023-06-01 15:09:53.000000 NewareNDA-2023.6.1/NewareNDA.egg-info/top_level.txt
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1030 2023-06-01 15:09:53.676402 NewareNDA-2023.6.1/PKG-INFO
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      657 2023-05-26 18:03:59.000000 NewareNDA-2023.6.1/README.md
-drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-06-01 15:09:53.676402 NewareNDA-2023.6.1/bin/
--rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-06-01 15:00:41.000000 NewareNDA-2023.6.1/bin/NewareNDA-cli.py
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2023-06-01 15:09:53.676402 NewareNDA-2023.6.1/setup.cfg
--rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      903 2023-02-02 18:25:45.000000 NewareNDA-2023.6.1/setup.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1488 2023-02-02 18:25:45.000000 NewareNDA-2023.7.3/LICENSE
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/NewareNDA/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     6649 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/NewareNDA/NewareNDA.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     3048 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/NewareNDA/NewareNDAx.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      101 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/NewareNDA/__init__.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1382 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/NewareNDA/dicts.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       28 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/NewareNDA/version.py
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/NewareNDA.egg-info/
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1153 2023-07-05 21:39:11.000000 NewareNDA-2023.7.3/NewareNDA.egg-info/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      320 2023-07-05 21:39:11.000000 NewareNDA-2023.7.3/NewareNDA.egg-info/SOURCES.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        1 2023-07-05 21:39:11.000000 NewareNDA-2023.7.3/NewareNDA.egg-info/dependency_links.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)        7 2023-07-05 21:39:11.000000 NewareNDA-2023.7.3/NewareNDA.egg-info/requires.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       10 2023-07-05 21:39:11.000000 NewareNDA-2023.7.3/NewareNDA.egg-info/top_level.txt
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)     1153 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/PKG-INFO
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      780 2023-07-05 21:23:56.000000 NewareNDA-2023.7.3/README.md
+drwxrwxr-x   0 cogswell  (1001) cogswell  (1001)        0 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/bin/
+-rwxrwxr-x   0 cogswell  (1001) cogswell  (1001)     1405 2023-06-23 14:20:58.000000 NewareNDA-2023.7.3/bin/NewareNDA-cli.py
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)       38 2023-07-05 21:39:11.651072 NewareNDA-2023.7.3/setup.cfg
+-rw-rw-r--   0 cogswell  (1001) cogswell  (1001)      903 2023-02-02 18:25:45.000000 NewareNDA-2023.7.3/setup.py
```

### Comparing `NewareNDA-2023.6.1/LICENSE` & `NewareNDA-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NewareNDA-2023.6.1/NewareNDA/NewareNDA.py` & `NewareNDA-2023.7.3/NewareNDA/NewareNDA.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,43 @@
 # © 2023 Copyright SES AI
 # Author: Daniel Cogswell
 # Email: danielcogswell@ses.ai
 
+import os
 import mmap
 import struct
 import logging
 from datetime import datetime
 import pandas as pd
 
-# Names for data fields
-rec_columns = [
-    'Index', 'Cycle', 'Step', 'Status', 'Time', 'Voltage',
-    'Current(mA)', 'Charge_Capacity(mAh)', 'Discharge_Capacity(mAh)',
-    'Charge_Energy(mWh)', 'Discharge_Energy(mWh)', 'Timestamp']
-aux_columns = ['Index', 'Aux', 'T']
-
-# Define precision of fields
-dtype_dict = {
-    'Index': 'uint32',
-    'Cycle': 'uint16',
-    'Step': 'uint32',
-    'Status': 'category',
-    'Time': 'float32',
-    'Voltage': 'float32',
-    'Current(mA)': 'float32',
-    'Charge_Capacity(mAh)': 'float32',
-    'Discharge_Capacity(mAh)': 'float32',
-    'Charge_Energy(mWh)': 'float32',
-    'Discharge_Energy(mWh)': 'float32'
-}
-
-# Dictionary mapping Status integer to string
-state_dict = {
-    1: 'CC_Chg',
-    2: 'CC_DChg',
-    3: 'CV_Chg',
-    4: 'Rest',
-    5: 'Cycle',
-    7: 'CCCV_Chg',
-    10: 'CR_DChg',
-    13: 'Pause',
-    17: 'SIM',
-    19: 'CV_DChg',
-    20: 'CCCV_DChg'
-}
-
-# Define field scaling based on instrument Range setting
-multiplier_dict = {
-    -200000: 1e-2,
-    -100000: 1e-2,
-    -60000: 1e-2,
-    -30000: 1e-2,
-    -50000: 1e-2,
-    -20000: 1e-2,
-    -10000: 1e-2,
-    -6000: 1e-2,
-    -5000: 1e-2,
-    -3000: 1e-2,
-    -1000: 1e-2,
-    -500: 1e-3,
-    -100: 1e-3,
-    0: 0,
-    10: 1e-3,
-    100: 1e-2,
-    200: 1e-2,
-    1000: 1e-1,
-    6000: 1e-1,
-    12000: 1e-1,
-    50000: 1e-1,
-    60000: 1e-1,
-    100000: 1e-1,
-}
+from NewareNDA.dicts import rec_columns, aux_columns, dtype_dict, \
+    multiplier_dict, state_dict
+from .NewareNDAx import read_ndax
 
 
 def read(file, software_cycle_number=False):
     """
+    Read electrochemical data from an Neware nda or ndax binary file.
+
+    Args:
+        file (str): Name of an .nda or .ndax file to read
+    Returns:
+        df (pd.DataFrame): DataFrame containing all records in the file
+    """
+    _, ext = os.path.splitext(file)
+    if ext == '.nda':
+        return read_nda(file, software_cycle_number)
+    elif ext == '.ndax':
+        return read_ndax(file)
+    else:
+        raise TypeError("File type not supported!")
+
+
+def read_nda(file, software_cycle_number):
+    """
     Function read electrochemical data from a Neware nda binary file.
 
     Args:
         file (str): Name of a .nda file to read
         software_cycle_number (bool): Generate the cycle number field
         to match old versions of BTSDA
     Returns:
```

### Comparing `NewareNDA-2023.6.1/README.md` & `NewareNDA-2023.7.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # NewareNDA
 
 © 2023 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
-Python module and command line tool for reading and converting Neware .nda battery cycling files.
+Python module and command line tool for reading and converting Neware nda and ndax battery cycling files. Auxiliary temperature fields are currently supported in nda format, with support for ndax auxiliary fields in development.
 
 # Installation
 To install from the PyPi package repository:
 ```
 pip install NewareNDA
 ```
 
 To install from source, clone this repository and run:
 ```
 cd NewareNDA
-pip install NewareNDA
+pip install .
 ```
 
 # Usage
 ```
 import NewareNDA
 df = NewareNDA.read('filename.nda')
 ```
```

### Comparing `NewareNDA-2023.6.1/bin/NewareNDA-cli.py` & `NewareNDA-2023.7.3/bin/NewareNDA-cli.py`

 * *Files identical despite different names*

### Comparing `NewareNDA-2023.6.1/setup.py` & `NewareNDA-2023.7.3/setup.py`

 * *Files identical despite different names*

