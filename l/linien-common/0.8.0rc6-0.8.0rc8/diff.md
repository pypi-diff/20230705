# Comparing `tmp/linien-common-0.8.0rc6.tar.gz` & `tmp/linien-common-0.8.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-0.8.0rc6.tar", last modified: Mon Jul  3 14:22:48 2023, max compression
+gzip compressed data, was "linien-common-0.8.0rc8.tar", last modified: Wed Jul  5 09:23:38 2023, max compression
```

## Comparing `linien-common-0.8.0rc6.tar` & `linien-common-0.8.0rc8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:48.529630 linien-common-0.8.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:22:48.529630 linien-common-0.8.0rc6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:48.529630 linien-common-0.8.0rc6/linien_common/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:48.529630 linien-common-0.8.0rc6/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:22:48.000000 linien-common-0.8.0rc6/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 14:22:48.000000 linien-common-0.8.0rc6/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:22:48.000000 linien-common-0.8.0rc6/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:22:48.000000 linien-common-0.8.0rc6/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 14:22:48.000000 linien-common-0.8.0rc6/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:22:48.529630 linien-common-0.8.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-03 14:22:35.000000 linien-common-0.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:38.925958 linien-common-0.8.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:38.925958 linien-common-0.8.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:38.925958 linien-common-0.8.0rc8/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:38.925958 linien-common-0.8.0rc8/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:38.000000 linien-common-0.8.0rc8/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-05 09:23:38.000000 linien-common-0.8.0rc8/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:23:38.000000 linien-common-0.8.0rc8/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-05 09:23:38.000000 linien-common-0.8.0rc8/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 09:23:38.000000 linien-common-0.8.0rc8/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:23:38.925958 linien-common-0.8.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-05 09:23:25.000000 linien-common-0.8.0rc8/setup.py
```

### Comparing `linien-common-0.8.0rc6/PKG-INFO` & `linien-common-0.8.0rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.8.0rc6/linien_common/common.py` & `linien-common-0.8.0rc8/linien_common/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,44 +14,53 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 
 """This file contains stuff that is required by the server as well as the client."""
 
+from enum import Enum, IntEnum
 from time import time
 from typing import Tuple
 
 import numpy as np
 from scipy.signal import correlate, resample
 
 MHz = 0x10000000 / 8
 Vpp = ((1 << 14) - 1) / 4
 # conversion of bits to V
 ANALOG_OUT_V = 1.8 / ((2**15) - 1)
 
-LOW_PASS_FILTER = 0
-HIGH_PASS_FILTER = 1
-
-FAST_OUT1 = 0
-FAST_OUT2 = 1
-ANALOG_OUT0 = 2
+AUTOLOCK_MAX_N_INSTRUCTIONS = 32
 
 DECIMATION = 8
 MAX_N_POINTS = 16384
 N_POINTS = int(MAX_N_POINTS / DECIMATION)
 
-AUTOLOCK_MAX_N_INSTRUCTIONS = 32
 
-AUTO_DETECT_AUTOLOCK_MODE = 0
-ROBUST_AUTOLOCK = 1
-FAST_AUTOLOCK = 2
+class FilterType(IntEnum):
+    LOW_PASS = 0
+    HIGH_PASS = 1
+
+
+class OutputChannel(IntEnum):
+    FAST_OUT1 = 0
+    FAST_OUT2 = 1
+    ANALOG_OUT0 = 2
+
+
+class AutolockMode(IntEnum):
+    AUTO_DETECT = 0
+    ROBUST = 1
+    FAST = 2
+
 
-PSD_ALGORITHM_WELCH = "welch"
-PSD_ALGORITHM_LPSD = "lpsd"
+class PSDAlgorithm(str, Enum):
+    WELCH = "welch"
+    LPSD = "lpsd"
 
 
 class SpectrumUncorrelatedException(Exception):
     pass
 
 
 def downsample_history(times, values, max_time_diff, max_N=N_POINTS):
```

### Comparing `linien-common-0.8.0rc6/linien_common/config.py` & `linien-common-0.8.0rc8/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien-common-0.8.0rc6/linien_common/influxdb.py` & `linien-common-0.8.0rc8/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-common-0.8.0rc6/linien_common.egg-info/PKG-INFO` & `linien-common-0.8.0rc8/linien_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Shared components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-common-0.8.0rc6/setup.py` & `linien-common-0.8.0rc8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
 setup(
     name="linien-common",
-    version="0.8.0rc6",
+    version="0.8.0rc8",
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
     maintainer_email="leykauf@physik.hu-berlin.de",
     description="Shared components of the Linien spectroscopy lock application.",
     long_description="Have a look at the [project repository](https://github.com/linien-org/linien) for installation instructions.",  # noqa: E501
     long_description_content_type="text/markdown",
```

