# Comparing `tmp/radbelt-0.1.4.tar.gz` & `tmp/radbelt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radbelt-0.1.4.tar", last modified: Thu Jun 15 02:48:05 2023, max compression
+gzip compressed data, was "radbelt-0.1.5.tar", last modified: Wed Jul  5 14:14:41 2023, max compression
```

## Comparing `radbelt-0.1.4.tar` & `radbelt-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.139757 radbelt-0.1.4/
--rw-r--r--   0 root         (0) root         (0)    12693 2023-06-15 02:47:52.000000 radbelt-0.1.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3431 2023-06-15 02:48:05.139757 radbelt-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2023-06-15 02:47:52.000000 radbelt-0.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-15 02:47:52.000000 radbelt-0.1.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/core.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/extern/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt/extern/aep8/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83596 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ae8max.asc
--rw-r--r--   0 root         (0) root         (0)    81254 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ae8min.asc
--rw-r--r--   0 root         (0) root         (0)   100542 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ap8max.asc
--rw-r--r--   0 root         (0) root         (0)   102318 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/ap8min.asc
--rw-r--r--   0 root         (0) root         (0)    14732 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/aep8/trmfun.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.139757 radbelt-0.1.4/radbelt/extern/igrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1945.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1950.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1955.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1960.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1965.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1970.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1975.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1980.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1985.dat
--rw-r--r--   0 root         (0) root         (0)     1591 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1990.dat
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf1995.dat
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2000.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2005.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2010.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/dgrf2015.dat
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/igrf2020.dat
--rw-r--r--   0 root         (0) root         (0)     1786 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/igrf2020s.dat
--rw-r--r--   0 root         (0) root         (0)    43035 2023-06-15 02:47:52.000000 radbelt-0.1.4/radbelt/extern/igrf/shellig.f
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 02:48:05.135757 radbelt-0.1.4/radbelt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3431 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1050 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-15 02:48:05.000000 radbelt-0.1.4/radbelt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 02:48:05.139757 radbelt-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-15 02:47:52.000000 radbelt-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.369835 radbelt-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)    12693 2023-07-05 14:14:28.000000 radbelt-0.1.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-07-05 14:14:41.369835 radbelt-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-05 14:14:28.000000 radbelt-0.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-05 14:14:28.000000 radbelt-0.1.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.361835 radbelt-0.1.5/radbelt/
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt/_version.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/core.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.361835 radbelt-0.1.5/radbelt/extern/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.365835 radbelt-0.1.5/radbelt/extern/aep8/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83596 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/ae8max.asc
+-rw-r--r--   0 root         (0) root         (0)    81254 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/ae8min.asc
+-rw-r--r--   0 root         (0) root         (0)   100542 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/ap8max.asc
+-rw-r--r--   0 root         (0) root         (0)   102318 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/ap8min.asc
+-rw-r--r--   0 root         (0) root         (0)    14732 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/aep8/trmfun.f
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.369835 radbelt-0.1.5/radbelt/extern/igrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1945.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1950.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1955.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1960.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1965.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1970.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1975.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1980.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1985.dat
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1990.dat
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf1995.dat
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf2000.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf2005.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf2010.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/dgrf2015.dat
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/igrf2020.dat
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/igrf2020s.dat
+-rw-r--r--   0 root         (0) root         (0)    43035 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/extern/igrf/shellig.f
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/paths.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-05 14:14:28.000000 radbelt-0.1.5/radbelt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:14:41.361835 radbelt-0.1.5/radbelt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 14:14:41.000000 radbelt-0.1.5/radbelt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:14:41.369835 radbelt-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-05 14:14:28.000000 radbelt-0.1.5/setup.py
```

### Comparing `radbelt-0.1.4/LICENSE.txt` & `radbelt-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/PKG-INFO` & `radbelt-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: radbelt
-Version: 0.1.4
-Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
-Author-email: Leo Singer <leo.p.singer@nasa.gov>
-License: NOSA
-Project-URL: source, https://github.com/nasa/radbelt
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # radbelt: An Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 
 This is small Python library to model the fluxes of charged particles trapped
 in the Van Allen belt. It provides a fast, simple, and convenient Python
 interface to the [International Geomagnetic Reference Field (IGRF)] model and
 NASA's AE-8/AP-8 models of electron and proton fluxes, which are both
 implemented in Fortran. The package is integrated with the [Astropy] ecosystem
@@ -57,19 +36,24 @@
 >>> from radbelt import get_flux
 >>> from astropy import units as u
 >>> from astropy.coordinates import EarthLocation
 >>> from astropy.time import Time
 >>> coords = EarthLocation(-45 * u.deg, -30 * u.deg, 500 * u.km)
 >>> time = Time('2021-03-01')
 >>> energy = 20 * u.MeV
->>> get_flux(coords, time, energy, 'p', 'max')
-<Quantity 2642.50268555 1 / (cm2 s)>
+>>> get_flux(coords, time, energy, 'p', 'max')  # doctest: +FLOAT_CMP
+<Quantity 2642.50268555 1 / (s cm2)>
 ```
 
 ## Known issues
 
-The CCMC IGRF code has spatially varying errors of a few percent, which will
-result in a striped pattern in the resulting particle flux.
+* The CCMC IGRF code has spatially varying errors of a few percent, which will
+  result in a striped pattern in the resulting particle flux.
+* This package does not support Windows yet. If you are a Windows developer,
+  then please help us out by contributing a pull request! Meanwhile, if you
+  need to use this package on Windows, then we recommend using Python under
+  Linux within Windows Subsystem for Linux (WSL), Docker, or a virtual machine.
+  See https://github.com/nasa/radbelt/issues/47.
 
 [International Geomagnetic Reference Field (IGRF)]: https://www.ngdc.noaa.gov/IAGA/vmod/igrf.html
 [Astropy]: https://www.astropy.org
 [Community Coordinated Modeling Center (CCMC)]: https://ccmc.gsfc.nasa.gov/
```

### Comparing `radbelt-0.1.4/README.md` & `radbelt-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: radbelt
+Version: 0.1.5
+Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
+Author-email: Leo Singer <leo.p.singer@nasa.gov>
+License: NOSA
+Project-URL: source, https://github.com/nasa/radbelt
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE.txt
+
 # radbelt: An Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 
 This is small Python library to model the fluxes of charged particles trapped
 in the Van Allen belt. It provides a fast, simple, and convenient Python
 interface to the [International Geomagnetic Reference Field (IGRF)] model and
 NASA's AE-8/AP-8 models of electron and proton fluxes, which are both
 implemented in Fortran. The package is integrated with the [Astropy] ecosystem
@@ -36,19 +60,24 @@
 >>> from radbelt import get_flux
 >>> from astropy import units as u
 >>> from astropy.coordinates import EarthLocation
 >>> from astropy.time import Time
 >>> coords = EarthLocation(-45 * u.deg, -30 * u.deg, 500 * u.km)
 >>> time = Time('2021-03-01')
 >>> energy = 20 * u.MeV
->>> get_flux(coords, time, energy, 'p', 'max')
-<Quantity 2642.50268555 1 / (cm2 s)>
+>>> get_flux(coords, time, energy, 'p', 'max')  # doctest: +FLOAT_CMP
+<Quantity 2642.50268555 1 / (s cm2)>
 ```
 
 ## Known issues
 
-The CCMC IGRF code has spatially varying errors of a few percent, which will
-result in a striped pattern in the resulting particle flux.
+* The CCMC IGRF code has spatially varying errors of a few percent, which will
+  result in a striped pattern in the resulting particle flux.
+* This package does not support Windows yet. If you are a Windows developer,
+  then please help us out by contributing a pull request! Meanwhile, if you
+  need to use this package on Windows, then we recommend using Python under
+  Linux within Windows Subsystem for Linux (WSL), Docker, or a virtual machine.
+  See https://github.com/nasa/radbelt/issues/47.
 
 [International Geomagnetic Reference Field (IGRF)]: https://www.ngdc.noaa.gov/IAGA/vmod/igrf.html
 [Astropy]: https://www.astropy.org
 [Community Coordinated Modeling Center (CCMC)]: https://ccmc.gsfc.nasa.gov/
```

### Comparing `radbelt-0.1.4/pyproject.toml` & `radbelt-0.1.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -12,32 +12,41 @@
 description = "Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model"
 readme = "README.md"
 authors = [ { name = "Leo Singer", email = "leo.p.singer@nasa.gov" } ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved",
+    "Operating System :: MacOS",
+    "Operating System :: POSIX",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Astronomy"
 ]
 license = { text = "NOSA" }
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 dependencies = ["astropy", "numpy"]
 dynamic = [ "version" ]
 
 [project.urls]
 source = "https://github.com/nasa/radbelt"
 
-[tool.setuptools.packages.find]
-include = ["radbelt.*"]
+[project.optional-dependencies]
+test = ["pytest-doctestplus"]
+
+[tool.setuptools.packages]
+find = {}
 
 [tool.setuptools.package-data]
 "radbelt.extern.igrf" = ["*.dat"]
 "radbelt.extern.aep8" = ["*.asc"]
 
 [tool.setuptools_scm]
 write_to = "radbelt/_version.py"
+
+[tool.cibuildwheel]
+test-extras = ["test"]
+test-command = "pytest --pyargs radbelt --doctest-plus"
```

### Comparing `radbelt-0.1.4/radbelt/core.f` & `radbelt-0.1.5/radbelt/core.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/aep8/ae8max.asc` & `radbelt-0.1.5/radbelt/extern/aep8/ae8max.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/aep8/ae8min.asc` & `radbelt-0.1.5/radbelt/extern/aep8/ae8min.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/aep8/ap8max.asc` & `radbelt-0.1.5/radbelt/extern/aep8/ap8max.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/aep8/ap8min.asc` & `radbelt-0.1.5/radbelt/extern/aep8/ap8min.asc`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/aep8/trmfun.f` & `radbelt-0.1.5/radbelt/extern/aep8/trmfun.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1945.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1945.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1950.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1950.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1955.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1955.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1960.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1960.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1965.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1965.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1970.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1970.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1975.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1975.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1980.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1980.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1985.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1985.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1990.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1990.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf1995.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf1995.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf2000.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf2005.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf2010.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/dgrf2015.dat` & `radbelt-0.1.5/radbelt/extern/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/igrf2020.dat` & `radbelt-0.1.5/radbelt/extern/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/igrf2020s.dat` & `radbelt-0.1.5/radbelt/extern/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt/extern/igrf/shellig.f` & `radbelt-0.1.5/radbelt/extern/igrf/shellig.f`

 * *Files identical despite different names*

### Comparing `radbelt-0.1.4/radbelt.egg-info/PKG-INFO` & `radbelt-0.1.5/radbelt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: radbelt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 Author-email: Leo Singer <leo.p.singer@nasa.gov>
 License: NOSA
 Project-URL: source, https://github.com/nasa/radbelt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE.txt
 
 # radbelt: An Astropy-friendly wrapper for the AE-8/AP-8 Van Allen belt model
 
 This is small Python library to model the fluxes of charged particles trapped
 in the Van Allen belt. It provides a fast, simple, and convenient Python
 interface to the [International Geomagnetic Reference Field (IGRF)] model and
@@ -57,19 +60,24 @@
 >>> from radbelt import get_flux
 >>> from astropy import units as u
 >>> from astropy.coordinates import EarthLocation
 >>> from astropy.time import Time
 >>> coords = EarthLocation(-45 * u.deg, -30 * u.deg, 500 * u.km)
 >>> time = Time('2021-03-01')
 >>> energy = 20 * u.MeV
->>> get_flux(coords, time, energy, 'p', 'max')
-<Quantity 2642.50268555 1 / (cm2 s)>
+>>> get_flux(coords, time, energy, 'p', 'max')  # doctest: +FLOAT_CMP
+<Quantity 2642.50268555 1 / (s cm2)>
 ```
 
 ## Known issues
 
-The CCMC IGRF code has spatially varying errors of a few percent, which will
-result in a striped pattern in the resulting particle flux.
+* The CCMC IGRF code has spatially varying errors of a few percent, which will
+  result in a striped pattern in the resulting particle flux.
+* This package does not support Windows yet. If you are a Windows developer,
+  then please help us out by contributing a pull request! Meanwhile, if you
+  need to use this package on Windows, then we recommend using Python under
+  Linux within Windows Subsystem for Linux (WSL), Docker, or a virtual machine.
+  See https://github.com/nasa/radbelt/issues/47.
 
 [International Geomagnetic Reference Field (IGRF)]: https://www.ngdc.noaa.gov/IAGA/vmod/igrf.html
 [Astropy]: https://www.astropy.org
 [Community Coordinated Modeling Center (CCMC)]: https://ccmc.gsfc.nasa.gov/
```

### Comparing `radbelt-0.1.4/radbelt.egg-info/SOURCES.txt` & `radbelt-0.1.5/radbelt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
+radbelt/__init__.py
+radbelt/_version.py
 radbelt/core.f
+radbelt/paths.py
+radbelt/util.py
 radbelt.egg-info/PKG-INFO
 radbelt.egg-info/SOURCES.txt
 radbelt.egg-info/dependency_links.txt
 radbelt.egg-info/requires.txt
 radbelt.egg-info/top_level.txt
 radbelt/extern/__init__.py
 radbelt/extern/aep8/__init__.py
```

