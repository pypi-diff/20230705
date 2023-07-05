# Comparing `tmp/nomad_camels_driver_keithley_237-0.1.0.tar.gz` & `tmp/nomad_camels_driver_keithley_237-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels_driver_keithley_237-0.1.0.tar", last modified: Wed Jun 28 13:32:59 2023, max compression
+gzip compressed data, was "nomad_camels_driver_keithley_237-0.1.1.tar", last modified: Wed Jul  5 16:19:41 2023, max compression
```

## Comparing `nomad_camels_driver_keithley_237-0.1.0.tar` & `nomad_camels_driver_keithley_237-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:32:59.433783 nomad_camels_driver_keithley_237-0.1.0/
--rw-rw-rw-   0        0        0    27028 2023-04-13 14:09:42.000000 nomad_camels_driver_keithley_237-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      889 2023-06-28 13:32:59.433783 nomad_camels_driver_keithley_237-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-24 09:25:53.000000 nomad_camels_driver_keithley_237-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 13:32:59.402799 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237/
--rw-rw-rw-   0        0        0     2471 2023-06-28 09:30:35.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237/keithley_237.py
--rw-rw-rw-   0        0        0    14381 2023-06-28 09:30:35.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237/keithley_237_ophyd.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:32:59.433783 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/
--rw-rw-rw-   0        0        0      889 2023-06-28 13:32:59.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-06-28 13:32:59.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:32:59.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 13:32:59.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-28 13:32:59.000000 nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      686 2023-06-28 09:32:00.000000 nomad_camels_driver_keithley_237-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 13:32:59.433783 nomad_camels_driver_keithley_237-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 16:19:41.387552 nomad_camels_driver_keithley_237-0.1.1/
+-rw-rw-rw-   0        0        0    27028 2023-04-13 14:09:42.000000 nomad_camels_driver_keithley_237-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      911 2023-07-05 16:19:41.387552 nomad_camels_driver_keithley_237-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-28 14:25:08.000000 nomad_camels_driver_keithley_237-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 16:19:41.377552 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237/
+-rw-rw-rw-   0        0        0     2471 2023-07-05 16:18:08.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237/keithley_237.py
+-rw-rw-rw-   0        0        0    23761 2023-07-05 16:17:45.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237/keithley_237_ophyd.py
+drwxrwxrwx   0        0        0        0 2023-07-05 16:19:41.387552 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/
+-rw-rw-rw-   0        0        0      911 2023-07-05 16:19:41.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-05 16:19:41.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 16:19:41.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 16:19:41.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-07-05 16:19:41.000000 nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      697 2023-07-05 16:19:17.000000 nomad_camels_driver_keithley_237-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-05 16:19:41.387552 nomad_camels_driver_keithley_237-0.1.1/setup.cfg
```

### Comparing `nomad_camels_driver_keithley_237-0.1.0/LICENSE.txt` & `nomad_camels_driver_keithley_237-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keithley_237-0.1.0/PKG-INFO` & `nomad_camels_driver_keithley_237-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_keithley_237
-Version: 0.1.0
+Version: 0.1.1
 Summary: Device driver for the Keithley 237 SMU.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
-Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html
+Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NOMAD-CAMELS Driver for Keithley 237  
 
 Driver of the Keithley 237 SMU written for the measurement software [NOMAD-CAMELS](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 
 ## Documentation
 
-For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html).
+For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html).
```

### Comparing `nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237/keithley_237.py` & `nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237/keithley_237.py`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keithley_237-0.1.0/nomad_camels_driver_keithley_237.egg-info/PKG-INFO` & `nomad_camels_driver_keithley_237-0.1.1/nomad_camels_driver_keithley_237.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nomad-camels-driver-keithley-237
-Version: 0.1.0
+Version: 0.1.1
 Summary: Device driver for the Keithley 237 SMU.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
-Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html
+Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NOMAD-CAMELS Driver for Keithley 237  
 
 Driver of the Keithley 237 SMU written for the measurement software [NOMAD-CAMELS](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 
 ## Documentation
 
-For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html).
+For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html).
```

### Comparing `nomad_camels_driver_keithley_237-0.1.0/pyproject.toml` & `nomad_camels_driver_keithley_237-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels_driver_keithley_237"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "Device driver for the Keithley 237 SMU."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
@@ -18,8 +18,8 @@
 ]
 dependencies = [
     "pyvisa",
     "pyvisa-py"
 ]
 [project.urls]
 "GitHub Page" = "https://github.com/FAU-LAP/NOMAD-CAMELS"
-"Documentation" = "https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html"
+"Documentation" = "https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html"
```

