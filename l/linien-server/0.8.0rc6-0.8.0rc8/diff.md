# Comparing `tmp/linien-server-0.8.0rc6.tar.gz` & `tmp/linien-server-0.8.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-server-0.8.0rc6.tar", last modified: Mon Jul  3 14:23:02 2023, max compression
+gzip compressed data, was "linien-server-0.8.0rc8.tar", last modified: Wed Jul  5 09:23:53 2023, max compression
```

## Comparing `linien-server-0.8.0rc6.tar` & `linien-server-0.8.0rc8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.733870 linien-server-0.8.0rc6/linien_server/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/acquisition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/linien_server/autolock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/algorithm_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/autolock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/robust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/autolock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/csr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/csrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/iir_coeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/linien.bin
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/linien_install_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/linien_start_server.sh
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/linien_stop_server.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/linien_server/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/approach_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/linien_server/pid_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/pid_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/pid_optimization/pid_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16857 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/linien_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/linien_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 14:23:02.000000 linien-server-0.8.0rc6/linien_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:23:02.737870 linien-server-0.8.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-03 14:22:35.000000 linien-server-0.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/autolock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/algorithm_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/autolock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/autolock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/csrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/iir_coeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2083740 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_install_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_start_server.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/linien_stop_server.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/approach_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server/pid_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/pid_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/pid_optimization/pid_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/linien_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/linien_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 09:23:53.000000 linien-server-0.8.0rc8/linien_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:23:53.850092 linien-server-0.8.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-05 09:23:25.000000 linien-server-0.8.0rc8/setup.py
```

### Comparing `linien-server-0.8.0rc6/PKG-INFO` & `linien-server-0.8.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.8.0rc6/linien_server/acquisition.py` & `linien-server-0.8.0rc8/linien_server/acquisition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
+# Copyright 2018-2023 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
 # Copyright 2021-2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -303,15 +303,26 @@
             self.skip_next_data_event.clear()
         else:
             self.skip_next_data_event.set()
 
 
 def flash_fpga():
     filepath = Path(__file__).resolve().parent / "linien.bin"
-    shutil.copy(str(filepath), "/dev/xdevcfg")
+
+    # On redpitaya os < 2, flashing fpga works by copying the bit file /dev/xdevcfg. On
+    # recent versions, there is a dedicated command for this
+    # cf. https://forum.redpitaya.com/viewtopic.php?p=33494&sid=5132bf6e33709b1a7daa948f8e8dcdb1#p33494  # noqa: E501
+    fpga_dev_file = Path("/dev/xdevcfg")
+
+    if fpga_dev_file.exists():
+        print("Copying gateware to %s" % fpga_dev_file)
+        shutil.copy(str(filepath), str(fpga_dev_file))
+    else:
+        print("Using fpautil to deploy gateware.")
+        subprocess.Popen(["/opt/redpitaya/bin/fpgautil", "-b", str(filepath)]).wait()
 
 
 def start_nginx():
     subprocess.Popen(["systemctl", "start", "redpitaya_nginx.service"])
 
 
 def stop_nginx():
```

### Comparing `linien-server-0.8.0rc6/linien_server/autolock/algorithm_selection.py` & `linien-server-0.8.0rc8/linien_server/autolock/algorithm_selection.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,21 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from linien_common.common import (
-    AUTO_DETECT_AUTOLOCK_MODE,
-    FAST_AUTOLOCK,
-    N_POINTS,
-    ROBUST_AUTOLOCK,
-    determine_shift_by_correlation,
-)
+from linien_common.common import N_POINTS, AutolockMode, determine_shift_by_correlation
 
 
 class AutolockAlgorithmSelector:
     """This class helps deciding which autolock method should be used."""
 
     def __init__(
         self,
@@ -37,15 +31,15 @@
     ):
         self.done = False
         self.mode = None
         self.spectra = [spectrum] + (additional_spectra or [])
         self.N_spectra_required = N_spectra_required
         self.line_width = line_width
 
-        if mode_preference != AUTO_DETECT_AUTOLOCK_MODE:
+        if mode_preference != AutolockMode.AUTO_DETECT:
             self.mode = mode_preference
             self.done = True
             return
 
         self.check()
 
     def handle_new_spectrum(self, spectrum):
@@ -65,12 +59,12 @@
                 abs(determine_shift_by_correlation(1, ref, spectrum)[0] * N_POINTS)
                 for spectrum in additional
             ]
             max_shift = max(abs_shifts)
             print("jitter / line width ratio:", max_shift / (self.line_width / 2))
 
             if max_shift <= self.line_width / 2:
-                self.mode = FAST_AUTOLOCK
+                self.mode = AutolockMode.FAST
             else:
-                self.mode = ROBUST_AUTOLOCK
+                self.mode = AutolockMode.ROBUST
 
             self.done = True
```

### Comparing `linien-server-0.8.0rc6/linien_server/autolock/autolock.py` & `linien-server-0.8.0rc8/linien_server/autolock/autolock.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/autolock/fast.py` & `linien-server-0.8.0rc8/linien_server/autolock/fast.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/autolock/robust.py` & `linien-server-0.8.0rc8/linien_server/autolock/robust.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/autolock/utils.py` & `linien-server-0.8.0rc8/linien_server/autolock/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/csr.py` & `linien-server-0.8.0rc8/linien_server/csr.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/csrmap.py` & `linien-server-0.8.0rc8/linien_server/csrmap.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/iir_coeffs.py` & `linien-server-0.8.0rc8/linien_server/iir_coeffs.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/influxdb.py` & `linien-server-0.8.0rc8/linien_server/influxdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,17 +75,24 @@
             self.write_data(self.credentials, data)
             sleep(interval)
 
     def test_connection(
         self, credentials: InfluxDBCredentials
     ) -> Tuple[bool, int, str]:
         """Write empty data to the server to test the connection"""
-        response = self.write_data(credentials, data={})
-        success = response.status_code == 204
-        return success, response.status_code, response.text
+        try:
+            response = self.write_data(credentials, data={})
+            success = response.status_code == 204
+            status_code = response.status_code
+            text = response.text
+        except requests.exceptions.ConnectionError:
+            success = False
+            status_code = 404
+            text = "Failed to establish connection."
+        return success, status_code, text
 
     def write_data(
         self, credentials: InfluxDBCredentials, data: dict
     ) -> requests.Response:
         """Write data to the database"""
         endpoint = credentials.url + "/api/v2/write"
         headers = {
```

### Comparing `linien-server-0.8.0rc6/linien_server/linien.bin` & `linien-server-0.8.0rc8/linien_server/linien.bin`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/linien_start_server.sh` & `linien-server-0.8.0rc8/linien_server/linien_start_server.sh`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/optimization/approach_line.py` & `linien-server-0.8.0rc8/linien_server/optimization/approach_line.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/optimization/engine.py` & `linien-server-0.8.0rc8/linien_server/optimization/engine.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/optimization/general.py` & `linien-server-0.8.0rc8/linien_server/optimization/general.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/optimization/optimization.py` & `linien-server-0.8.0rc8/linien_server/optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/optimization/utils.py` & `linien-server-0.8.0rc8/linien_server/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/linien_server/parameters.py` & `linien-server-0.8.0rc8/linien_server/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,15 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import json
 from time import time
 from typing import Any, Callable, Dict, Iterator, List, Tuple
 
 import linien_server
-from linien_common.common import (
-    AUTO_DETECT_AUTOLOCK_MODE,
-    FAST_AUTOLOCK,
-    PSD_ALGORITHM_LPSD,
-    MHz,
-    Vpp,
-)
+from linien_common.common import AutolockMode, MHz, PSDAlgorithm, Vpp
 from linien_common.config import USER_DATA_PATH
 
 PARAMETER_STORE_FILENAME = "linien_parameters.json"
 
 
 class Parameter:
     """Represents a single parameter and is used by `Parameters`."""
@@ -466,30 +460,32 @@
         """The filter frequency in units of Hz"""
 
         self.filter_2_frequency_b = Parameter(start=10000, restorable=True)
         """The filter frequency in units of Hz"""
 
         self.filter_1_type_a = Parameter(start=0, restorable=True)
         """
-        Either `LOW_PASS_FILTER` or `HIGH_PASS_FILTER` of linien_common.common` module.
+        Either `LOW_PASS` or `HIGH_PASS` of linien_common.common.FilterType` enum class.
         """
 
         self.filter_2_type_a = Parameter(start=0, restorable=True)
         """
-        Either `LOW_PASS_FILTER` or `HIGH_PASS_FILTER` of linien_common.common` module.
+        Either `LOW_PASS` or `HIGH_PASS` of linien_common.common.FilterType` enum class.
         """
 
         self.filter_1_type_b = Parameter(start=0, restorable=True)
         """
-        Either `LOW_PASS_FILTER` or `HIGH_PASS_FILTER` of linien_common.common` module.
+        Either `LOW_PASS` or `HIGH_PASS` of linien_common.common.FilterType` enum class.
         """
+
         self.filter_2_type_b = Parameter(start=0, restorable=True)
         """
-        Either `LOW_PASS_FILTER` or `HIGH_PASS_FILTER` of linien_common.common` module.
+        Either `LOW_PASS` or `HIGH_PASS` of linien_common.common.FilterType` enum class.
         """
+
         # ------------------- LOCK AND PID PARAMETERS ----------------------------------
 
         self.combined_offset = Parameter(min_=-8191, max_=8191, start=0)
         """
         After combining channels A and B and before passing the result to the PID,
         `combined_offset` is added. It uses the same units as the channel offsets, i.e.
         a value of -8191 shifts the data down by 1V, a value of +8191 moves it up.
@@ -532,17 +528,17 @@
         # ------------------- AUTOLOCK PARAMETERS --------------------------------------
         # These parameters are used internally by the optimization algorithm and usually
         # should not be manipulated
         self.task = Parameter(start=None, sync=False)
         self.automatic_mode = Parameter(start=True)
         self.autolock_target_position = Parameter(start=0)
         self.autolock_mode_preference = Parameter(
-            start=AUTO_DETECT_AUTOLOCK_MODE, restorable=True
+            start=AutolockMode.AUTO_DETECT, restorable=True
         )
-        self.autolock_mode = Parameter(start=FAST_AUTOLOCK)
+        self.autolock_mode = Parameter(start=AutolockMode.FAST)
         self.autolock_time_scale = Parameter(start=0)
         self.autolock_instructions = Parameter(start=[], sync=False)
         self.autolock_final_wait_time = Parameter(start=0)
         self.autolock_selection = Parameter(start=False)
         self.autolock_running = Parameter(start=False)
         self.autolock_preparing = Parameter(start=False)
         self.autolock_percentage = Parameter(start=0, min_=0, max_=100)
@@ -583,15 +579,15 @@
         """
 
         self.acquisition_raw_filter_frequency = Parameter(start=0)
         """The filter frequency in units of Hz"""
 
         self.psd_data_partial = Parameter(start=None)
         self.psd_data_complete = Parameter(start=None)
-        self.psd_algorithm = Parameter(start=PSD_ALGORITHM_LPSD)
+        self.psd_algorithm = Parameter(start=PSDAlgorithm.LPSD)
         self.psd_acquisition_running = Parameter(start=False)
         self.psd_optimization_running = Parameter(start=False)
         self.psd_acquisition_max_decimation = Parameter(
             start=18, min_=1, max_=32, restorable=True
         )
 
     def __iter__(self) -> Iterator[Tuple[str, Parameter]]:
```

### Comparing `linien-server-0.8.0rc6/linien_server/pid_optimization/pid_optimization.py` & `linien-server-0.8.0rc8/linien_server/pid_optimization/pid_optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,49 +16,51 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 import random
 import string
 from time import sleep, time
+from typing import Tuple
 
 import numpy as np
-from linien_common.common import PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH
+from linien_common.common import PSDAlgorithm
 from linien_server.optimization.engine import MultiDimensionalOptimizationEngine
 from pylpsd import lpsd
 from scipy import signal
 
 ALL_DECIMATIONS = list(range(32))
 
 
-def calculate_psd(sig, fs, algorithm):
+def calculate_psd(
+    sig: np.ndarray, fs: float, algorithm: PSDAlgorithm
+) -> Tuple[np.ndarray, np.ndarray]:
     """
-    Calculates the power spectral density.
+    Calculate the power spectral density.
 
     :param sig: The signal to calculate the PSD for.
     :param fs: The sampling frequency.
-    :param algorithm: The PSD algorithm to use. Options are 'lpsd' and 'welch'.
+    :param algorithm: The PSD algorithm to use.
     :return: One-sided power spectral density.
     """
-    assert algorithm in [PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH]
 
     # at beginning or end of signal, we sometimes have more glitches --> ignore
     # them (200 points less @ 16384 points doesn't hurt much)
     sig = sig[100:-100]
 
     num_pts = 256
     window = "hann"  # passed to scipy.signal.get_window for welch and lpsd
 
     sig = sig.astype(np.float64)
 
-    if algorithm == PSD_ALGORITHM_WELCH:
+    if algorithm == PSDAlgorithm.WELCH:
         f, Pxx = signal.welch(
             sig, fs, window=window, nperseg=num_pts, scaling="density"
         )
-    elif algorithm == PSD_ALGORITHM_LPSD:
+    elif algorithm == PSDAlgorithm.LPSD:
         fmin = fs / len(sig) * 10  # lowest frequency of interest
         fmax = fs / 20.0  # highest frequency of interest
 
         f, Pxx = lpsd(
             sig,
             fs,
             window=window,
```

### Comparing `linien-server-0.8.0rc6/linien_server/registers.py` & `linien-server-0.8.0rc8/linien_server/registers.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Optional
 
 import numpy as np
 import rpyc
-from linien_common.common import (
-    HIGH_PASS_FILTER,
-    LOW_PASS_FILTER,
-    MHz,
-    convert_channel_mixing_value,
-)
+from linien_common.common import FilterType, MHz, convert_channel_mixing_value
 from linien_common.config import ACQUISITION_PORT, DEFAULT_SWEEP_SPEED
 from linien_server.parameters import Parameters
 
 from . import csrmap
 from .iir_coeffs import make_filter
 
 
@@ -298,15 +293,15 @@
                         chain,
                         ("c", "d")[iir_idx],
                         iir_sub_idx + 1,
                     )
 
                     if automatic:
                         filter_enabled = True
-                        filter_type = LOW_PASS_FILTER
+                        filter_type = FilterType.LOW_PASS
                         filter_frequency = (
                             self.parameters.modulation_frequency.value / MHz * 1e6 / 2
                         )
 
                         # if the filter frequency is too low (< 10Hz), the IIR doesn't
                         # work properly anymore. In that case, don't filter. This is
                         # also helpful if the raw (not demodulated) signal should be
@@ -326,22 +321,22 @@
                             self.parameters,
                             "filter_%d_frequency_%s" % (iir_idx + 1, chain),
                         ).value
 
                     if not filter_enabled:
                         self.set_iir(iir_name, *make_filter("P", k=1))
                     else:
-                        if filter_type == LOW_PASS_FILTER:
+                        if filter_type == FilterType.LOW_PASS:
                             self.set_iir(
                                 iir_name,
                                 *make_filter(
                                     "LP", f=filter_frequency / fpga_base_freq, k=1
                                 ),
                             )
-                        elif filter_type == HIGH_PASS_FILTER:
+                        elif filter_type == FilterType.HIGH_PASS:
                             self.set_iir(
                                 iir_name,
                                 *make_filter(
                                     "HP", f=filter_frequency / fpga_base_freq, k=1
                                 ),
                             )
                         else:
```

### Comparing `linien-server-0.8.0rc6/linien_server/server.py` & `linien-server-0.8.0rc8/linien_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 from time import sleep
 from typing import List, Tuple
 
 import click
 import numpy as np
 import rpyc
 from linien_common.common import N_POINTS, check_plot_data, update_signal_history
-from linien_common.communication import pack, unpack
+from linien_common.communication import (
+    pack,
+    unpack,
+    username_and_password_authenticator,
+)
 from linien_common.config import DEFAULT_SERVER_PORT
 from linien_common.influxdb import InfluxDBCredentials, restore_credentials
 from linien_server import __version__
 from linien_server.autolock.autolock import Autolock
 from linien_server.influxdb import InfluxDBLogger
 from linien_server.optimization.optimization import OptimizeSpectroscopy
 from linien_server.parameters import Parameters, restore_parameters, save_parameters
@@ -389,26 +393,33 @@
 @click.option(
     "--host",
     help=(
         "Allows to run the server locally for development and connects to a RedPitaya. "
         "Specify the RP's host as follows: --host=rp-f0xxxx.local"
     ),
 )
-def run_server(port, fake=False, host=None):
+@click.option("--no-auth", is_flag=True, help="Disable authentication")
+def run_server(port, fake=False, host=None, no_auth=False):
     print("Start server on port", port)
 
     if fake:
         print("starting fake server")
         control = FakeRedPitayaControlService()
     else:
         control = RedPitayaControlService(host=host)
 
+    if no_auth:
+        authenticator = None
+    else:
+        authenticator = username_and_password_authenticator
+
     thread = ThreadedServer(
         control,
         port=port,
+        authenticator=authenticator,
         protocol_config={"allow_pickle": True},
     )
     thread.start()
 
 
 if __name__ == "__main__":
     run_server()
```

### Comparing `linien-server-0.8.0rc6/linien_server.egg-info/PKG-INFO` & `linien-server-0.8.0rc8/linien_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-server
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Server components of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-server-0.8.0rc6/linien_server.egg-info/SOURCES.txt` & `linien-server-0.8.0rc8/linien_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-server-0.8.0rc6/setup.py` & `linien-server-0.8.0rc8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2018-2022 Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>
-# Copyright 2022 Bastian Leykauf <leykauf@physik.hu-berlin.de>
+# Copyright 2022-2023 Bastian Leykauf <leykauf@physik.hu-berlin.de>
 #
 # This file is part of Linien and based on redpid.
 #
 # Linien is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc6"
+version = "0.8.0rc8"
 
 setup(
     name="linien-server",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -37,21 +37,21 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["linien-server=linien_server.server:run_server"]},
     python_requires=">=3.5",
     install_requires=[
         "appdirs>=1.4.4",
-        "certifi==2021.10.8",  # pinned because of bug in default pip 9.0.1, see #339
+        "certifi==2021.10.8;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
         "click>=7.1.2",
         "cma>=3.0.3",
-        "pip>=20.3.4",
         "pylpsd>=0.1.4",
         "pyrp3>=1.1.0;platform_machine=='armv7l'",  # only install on RedPitaya
-        "requests<=2.25.1",
+        "requests==2.25.1;python_version<'3.10'",  # pinned because of bug in pip 9.0.1, see #339 # noqa: E501
+        "requests>=2.25.1;python_version>='3.10'",
         "linien-common=={}".format(version),
     ],
     scripts=[
         "linien_server/linien_start_server.sh",
         "linien_server/linien_stop_server.sh",
         "linien_server/linien_install_requirements.sh",
     ],
```

