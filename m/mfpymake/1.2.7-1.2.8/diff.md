# Comparing `tmp/mfpymake-1.2.7.tar.gz` & `tmp/mfpymake-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfpymake-1.2.7.tar", last modified: Sat Dec 10 01:53:11 2022, max compression
+gzip compressed data, was "mfpymake-1.2.8.tar", last modified: Wed Jul  5 20:24:55 2023, max compression
```

## Comparing `mfpymake-1.2.7.tar` & `mfpymake-1.2.8.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.258212 mfpymake-1.2.7/
--rwx--x--x   0 jdhughes (179580369) 286921933     1621 2021-12-03 21:16:36.000000 mfpymake-1.2.7/LICENSE.md
--rw-r--r--   0 jdhughes (179580369) 286921933      180 2022-12-09 15:05:45.000000 mfpymake-1.2.7/MANIFEST.in
--rw-r--r--   0 jdhughes (179580369) 286921933    12346 2022-12-10 01:53:11.258348 mfpymake-1.2.7/PKG-INFO
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.138025 mfpymake-1.2.7/docs/
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.158528 mfpymake-1.2.7/docs/css/
--rw-------   0 jdhughes (179580369) 286921933      321 2020-08-19 19:41:40.000000 mfpymake-1.2.7/docs/css/custom.css
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.163677 mfpymake-1.2.7/mfpymake.egg-info/
--rw-------   0 jdhughes (179580369) 286921933    12346 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/PKG-INFO
--rw-------   0 jdhughes (179580369) 286921933      996 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/SOURCES.txt
--rw-------   0 jdhughes (179580369) 286921933        1 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/dependency_links.txt
--rw-r--r--   0 jdhughes (179580369) 286921933      141 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/entry_points.txt
--rw-------   0 jdhughes (179580369) 286921933        1 2021-12-02 03:20:21.000000 mfpymake-1.2.7/mfpymake.egg-info/not-zip-safe
--rw-------   0 jdhughes (179580369) 286921933       53 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/requires.txt
--rw-------   0 jdhughes (179580369) 286921933       16 2022-12-10 01:53:11.000000 mfpymake-1.2.7/mfpymake.egg-info/top_level.txt
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.183787 mfpymake-1.2.7/pymake/
--rw-r--r--   0 jdhughes (179580369) 286921933     2230 2022-12-08 21:16:49.000000 mfpymake-1.2.7/pymake/__init__.py
--rw-------   0 jdhughes (179580369) 286921933      745 2020-08-05 20:00:08.000000 mfpymake-1.2.7/pymake/__main__.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.195276 mfpymake-1.2.7/pymake/autotest/
--rw-------   0 jdhughes (179580369) 286921933      192 2020-08-21 17:54:09.000000 mfpymake-1.2.7/pymake/autotest/__init__.py
--rwxr-xr-x   0 jdhughes (179580369) 286921933    73412 2022-11-27 19:54:06.000000 mfpymake-1.2.7/pymake/autotest/autotest.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.211660 mfpymake-1.2.7/pymake/cmds/
--rw-r--r--   0 jdhughes (179580369) 286921933        0 2022-12-09 15:05:45.000000 mfpymake-1.2.7/pymake/cmds/__init__.py
--rwxr-xr-x   0 jdhughes (179580369) 286921933     3894 2022-12-09 16:01:32.000000 mfpymake-1.2.7/pymake/cmds/build.py
--rwxr-xr-x   0 jdhughes (179580369) 286921933     3603 2022-12-10 01:51:41.000000 mfpymake-1.2.7/pymake/cmds/createjson.py
--rwxr-xr-x   0 jdhughes (179580369) 286921933     2155 2022-12-09 15:05:45.000000 mfpymake-1.2.7/pymake/cmds/mfpymakecli.py
--rw-r--r--   0 jdhughes (179580369) 286921933      499 2022-12-09 15:05:45.000000 mfpymake-1.2.7/pymake/config.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.217010 mfpymake-1.2.7/pymake/plot/
--rw-------   0 jdhughes (179580369) 286921933      133 2020-08-21 17:54:09.000000 mfpymake-1.2.7/pymake/plot/__init__.py
--rw-------   0 jdhughes (179580369) 286921933     4888 2022-04-20 14:16:59.000000 mfpymake-1.2.7/pymake/plot/dependency_graphs.py
--rw-r--r--   0 jdhughes (179580369) 286921933    25953 2022-12-09 20:02:43.000000 mfpymake-1.2.7/pymake/pymake.py
--rw-r--r--   0 jdhughes (179580369) 286921933    57553 2022-12-09 15:05:45.000000 mfpymake-1.2.7/pymake/pymake_base.py
--rw-r--r--   0 jdhughes (179580369) 286921933     8267 2022-12-09 20:02:43.000000 mfpymake-1.2.7/pymake/pymake_build_apps.py
--rw-r--r--   0 jdhughes (179580369) 286921933    11378 2022-12-09 15:05:45.000000 mfpymake-1.2.7/pymake/pymake_parser.py
-drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2022-12-10 01:53:11.257721 mfpymake-1.2.7/pymake/utils/
--rw-------   0 jdhughes (179580369) 286921933     2778 2022-02-17 05:02:12.000000 mfpymake-1.2.7/pymake/utils/_Popen_wrapper.py
--rw-------   0 jdhughes (179580369) 286921933      225 2022-11-27 20:28:28.000000 mfpymake-1.2.7/pymake/utils/__init__.py
--rw-r--r--   0 jdhughes (179580369) 286921933     9566 2022-12-05 21:05:53.000000 mfpymake-1.2.7/pymake/utils/_compiler_language_files.py
--rw-r--r--   0 jdhughes (179580369) 286921933    30018 2022-12-05 19:03:20.000000 mfpymake-1.2.7/pymake/utils/_compiler_switches.py
--rw-------   0 jdhughes (179580369) 286921933    10730 2022-04-20 14:16:59.000000 mfpymake-1.2.7/pymake/utils/_dag.py
--rw-------   0 jdhughes (179580369) 286921933     2000 2022-11-27 16:43:12.000000 mfpymake-1.2.7/pymake/utils/_file_utils.py
--rw-r--r--   0 jdhughes (179580369) 286921933    18802 2022-12-08 21:16:49.000000 mfpymake-1.2.7/pymake/utils/_meson_build.py
--rw-------   0 jdhughes (179580369) 286921933    25605 2022-03-09 02:21:21.000000 mfpymake-1.2.7/pymake/utils/_usgs_src_update.py
--rw-r--r--   0 jdhughes (179580369) 286921933    28719 2022-12-10 01:51:41.000000 mfpymake-1.2.7/pymake/utils/download.py
--rw-r--r--   0 jdhughes (179580369) 286921933    15893 2022-12-10 01:51:41.000000 mfpymake-1.2.7/pymake/utils/usgsprograms.py
--rw-r--r--   0 jdhughes (179580369) 286921933     4952 2022-12-10 01:51:41.000000 mfpymake-1.2.7/pymake/utils/usgsprograms.txt
--rw-r--r--   0 jdhughes (179580369) 286921933      406 2022-11-30 20:04:36.000000 mfpymake-1.2.7/pyproject.toml
--rw-r--r--   0 jdhughes (179580369) 286921933      161 2022-12-10 01:51:41.000000 mfpymake-1.2.7/pytest.ini
--rw-r--r--   0 jdhughes (179580369) 286921933     1637 2022-12-10 01:53:11.260360 mfpymake-1.2.7/setup.cfg
--rwx--x--x   0 jdhughes (179580369) 286921933       38 2022-03-03 15:25:33.000000 mfpymake-1.2.7/setup.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.591522 mfpymake-1.2.8/
+-rwx--x--x   0 jdhughes (179580369) 286921933     1621 2021-12-03 21:16:36.000000 mfpymake-1.2.8/LICENSE.md
+-rw-r--r--   0 jdhughes (179580369) 286921933      180 2022-12-09 15:05:45.000000 mfpymake-1.2.8/MANIFEST.in
+-rw-r--r--   0 jdhughes (179580369) 286921933    12346 2023-07-05 20:24:55.591650 mfpymake-1.2.8/PKG-INFO
+-rw-r--r--   0 jdhughes (179580369) 286921933    11282 2023-07-05 20:22:39.000000 mfpymake-1.2.8/README.md
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.465763 mfpymake-1.2.8/docs/
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.492061 mfpymake-1.2.8/docs/css/
+-rw-------   0 jdhughes (179580369) 286921933      321 2020-08-19 19:41:40.000000 mfpymake-1.2.8/docs/css/custom.css
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.504956 mfpymake-1.2.8/mfpymake.egg-info/
+-rw-------   0 jdhughes (179580369) 286921933    12346 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/PKG-INFO
+-rw-------   0 jdhughes (179580369) 286921933      950 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/SOURCES.txt
+-rw-------   0 jdhughes (179580369) 286921933        1 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/dependency_links.txt
+-rw-r--r--   0 jdhughes (179580369) 286921933      141 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/entry_points.txt
+-rw-------   0 jdhughes (179580369) 286921933        1 2021-12-02 03:20:21.000000 mfpymake-1.2.8/mfpymake.egg-info/not-zip-safe
+-rw-------   0 jdhughes (179580369) 286921933       53 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/requires.txt
+-rw-------   0 jdhughes (179580369) 286921933       16 2023-07-05 20:24:55.000000 mfpymake-1.2.8/mfpymake.egg-info/top_level.txt
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.533364 mfpymake-1.2.8/pymake/
+-rw-r--r--   0 jdhughes (179580369) 286921933     1296 2023-06-29 20:08:39.000000 mfpymake-1.2.8/pymake/__init__.py
+-rw-------   0 jdhughes (179580369) 286921933      745 2020-08-05 20:00:08.000000 mfpymake-1.2.8/pymake/__main__.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.546536 mfpymake-1.2.8/pymake/cmds/
+-rw-r--r--   0 jdhughes (179580369) 286921933        0 2022-12-09 15:05:45.000000 mfpymake-1.2.8/pymake/cmds/__init__.py
+-rwxr-xr-x   0 jdhughes (179580369) 286921933     3894 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/cmds/build.py
+-rwxr-xr-x   0 jdhughes (179580369) 286921933     3603 2022-12-10 01:51:41.000000 mfpymake-1.2.8/pymake/cmds/createjson.py
+-rwxr-xr-x   0 jdhughes (179580369) 286921933     2155 2022-12-09 15:05:45.000000 mfpymake-1.2.8/pymake/cmds/mfpymakecli.py
+-rw-r--r--   0 jdhughes (179580369) 286921933      495 2023-07-05 20:22:39.000000 mfpymake-1.2.8/pymake/config.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.554162 mfpymake-1.2.8/pymake/plot/
+-rw-------   0 jdhughes (179580369) 286921933      133 2020-08-21 17:54:09.000000 mfpymake-1.2.8/pymake/plot/__init__.py
+-rw-------   0 jdhughes (179580369) 286921933     4888 2022-04-20 14:16:59.000000 mfpymake-1.2.8/pymake/plot/dependency_graphs.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    25953 2022-12-09 20:02:43.000000 mfpymake-1.2.8/pymake/pymake.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    57552 2023-06-29 20:08:39.000000 mfpymake-1.2.8/pymake/pymake_base.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     8267 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/pymake_build_apps.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    11378 2023-06-29 23:30:46.000000 mfpymake-1.2.8/pymake/pymake_parser.py
+drwxr-xr-x   0 jdhughes (179580369) 286921933        0 2023-07-05 20:24:55.591144 mfpymake-1.2.8/pymake/utils/
+-rw-------   0 jdhughes (179580369) 286921933     2778 2022-02-17 05:02:12.000000 mfpymake-1.2.8/pymake/utils/_Popen_wrapper.py
+-rw-------   0 jdhughes (179580369) 286921933      225 2022-11-27 20:28:28.000000 mfpymake-1.2.8/pymake/utils/__init__.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     9566 2022-12-05 21:05:53.000000 mfpymake-1.2.8/pymake/utils/_compiler_language_files.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    30018 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/utils/_compiler_switches.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    10730 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/utils/_dag.py
+-rw-------   0 jdhughes (179580369) 286921933     2000 2022-11-27 16:43:12.000000 mfpymake-1.2.8/pymake/utils/_file_utils.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    18802 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/utils/_meson_build.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    30590 2023-07-05 20:22:39.000000 mfpymake-1.2.8/pymake/utils/_usgs_src_update.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    28719 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pymake/utils/download.py
+-rw-r--r--   0 jdhughes (179580369) 286921933    15893 2022-12-10 01:51:41.000000 mfpymake-1.2.8/pymake/utils/usgsprograms.py
+-rw-r--r--   0 jdhughes (179580369) 286921933     4952 2023-07-05 20:22:39.000000 mfpymake-1.2.8/pymake/utils/usgsprograms.txt
+-rw-r--r--   0 jdhughes (179580369) 286921933      406 2023-07-05 18:33:10.000000 mfpymake-1.2.8/pyproject.toml
+-rw-r--r--   0 jdhughes (179580369) 286921933      161 2022-12-10 01:51:41.000000 mfpymake-1.2.8/pytest.ini
+-rw-r--r--   0 jdhughes (179580369) 286921933     1637 2023-07-05 20:24:55.593259 mfpymake-1.2.8/setup.cfg
+-rwxr-xr-x   0 jdhughes (179580369) 286921933       38 2023-07-05 18:33:10.000000 mfpymake-1.2.8/setup.py
```

### Comparing `mfpymake-1.2.7/LICENSE.md` & `mfpymake-1.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/PKG-INFO` & `mfpymake-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfpymake
-Version: 1.2.7
+Version: 1.2.8
 Summary: pymake is a Python package to compile MODFLOW-based models.
 Home-page: https://github.com/modflowpy/pymake
 Download-URL: https://pypi.org/project/mfpymake
 Author: Joseph D. Hughes
 Author-email: modflow@usgs.gov
 Maintainer: Joseph D. Hughes
 Maintainer-email: jdhughes@usgs.gov
@@ -18,23 +18,23 @@
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pymake
 
 Python package for building MODFLOW-based programs from source files.
 
-### Version 1.2.7
+### Version 1.2.8
 
 ![pymake continuous integration](https://github.com/modflowpy/pymake/workflows/pymake%20continuous%20integration/badge.svg)
 [![codecov](https://codecov.io/gh/modflowpy/pymake/branch/master/graph/badge.svg)](https://codecov.io/gh/modflowpy/pymake)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/fe4275a3cfb84acf9c84aba7b4ae2086)](https://www.codacy.com/gh/modflowpy/pymake/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=modflowpy/pymake&amp;utm_campaign=Badge_Grade)
 [![Documentation Status](https://readthedocs.org/projects/mfpymake/badge/?version=latest)](https://mfpymake.readthedocs.io/en/latest/?badge=latest)
 [![PyPI Version](https://img.shields.io/pypi/v/mfpymake.png)](https://pypi.python.org/pypi/mfpymake)
```

### Comparing `mfpymake-1.2.7/mfpymake.egg-info/PKG-INFO` & `mfpymake-1.2.8/mfpymake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfpymake
-Version: 1.2.7
+Version: 1.2.8
 Summary: pymake is a Python package to compile MODFLOW-based models.
 Home-page: https://github.com/modflowpy/pymake
 Download-URL: https://pypi.org/project/mfpymake
 Author: Joseph D. Hughes
 Author-email: modflow@usgs.gov
 Maintainer: Joseph D. Hughes
 Maintainer-email: jdhughes@usgs.gov
@@ -18,23 +18,23 @@
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pymake
 
 Python package for building MODFLOW-based programs from source files.
 
-### Version 1.2.7
+### Version 1.2.8
 
 ![pymake continuous integration](https://github.com/modflowpy/pymake/workflows/pymake%20continuous%20integration/badge.svg)
 [![codecov](https://codecov.io/gh/modflowpy/pymake/branch/master/graph/badge.svg)](https://codecov.io/gh/modflowpy/pymake)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/fe4275a3cfb84acf9c84aba7b4ae2086)](https://www.codacy.com/gh/modflowpy/pymake/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=modflowpy/pymake&amp;utm_campaign=Badge_Grade)
 [![Documentation Status](https://readthedocs.org/projects/mfpymake/badge/?version=latest)](https://mfpymake.readthedocs.io/en/latest/?badge=latest)
 [![PyPI Version](https://img.shields.io/pypi/v/mfpymake.png)](https://pypi.python.org/pypi/mfpymake)
```

### Comparing `mfpymake-1.2.7/mfpymake.egg-info/SOURCES.txt` & `mfpymake-1.2.8/mfpymake.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.md
 MANIFEST.in
+README.md
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 docs/css/custom.css
 mfpymake.egg-info/PKG-INFO
 mfpymake.egg-info/SOURCES.txt
@@ -15,16 +16,14 @@
 pymake/__init__.py
 pymake/__main__.py
 pymake/config.py
 pymake/pymake.py
 pymake/pymake_base.py
 pymake/pymake_build_apps.py
 pymake/pymake_parser.py
-pymake/autotest/__init__.py
-pymake/autotest/autotest.py
 pymake/cmds/__init__.py
 pymake/cmds/build.py
 pymake/cmds/createjson.py
 pymake/cmds/mfpymakecli.py
 pymake/plot/__init__.py
 pymake/plot/dependency_graphs.py
 pymake/utils/_Popen_wrapper.py
```

### Comparing `mfpymake-1.2.7/pymake/__init__.py` & `mfpymake-1.2.8/pymake/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,14 @@
 """pymake is a python package for compiling MODFLOW-based and other Fortran, C,
 and  C++ programs. The package determines the build order using a directed
 acyclic graph and then compiles the source files using GNU compilers
 (:code:`gcc`, :code:`g++`, :code:`gfortran`) or Intel compilers
 (:code:`ifort`, :code:`icc`)."""
 
 
-# autotest
-from .autotest.autotest import (
-    compare,
-    compare_budget,
-    compare_concs,
-    compare_heads,
-    compare_stages,
-    compare_swrbudget,
-    get_entries_from_namefile,
-    get_input_files,
-    get_mf6_blockdata,
-    get_mf6_comparison,
-    get_mf6_files,
-    get_mf6_ftypes,
-    get_mf6_mshape,
-    get_mf6_nper,
-    get_namefiles,
-    get_sim_name,
-    setup,
-    setup_comparison,
-    setup_mf6,
-    setup_mf6_comparison,
-    teardown,
-)
-
 # pymake
 from .config import (
     __author__,
     __date__,
     __description__,
     __email__,
     __maintainer__,
@@ -73,30 +48,8 @@
     "getmfexes",
     "repo_latest_version",
     "get_repo_assets",
     "zip_all",
     # plot
     "make_plots",
     "to_pydot",
-    # autotest
-    "setup",
-    "setup_comparison",
-    "teardown",
-    "get_namefiles",
-    "get_entries_from_namefile",
-    "get_sim_name",
-    "get_input_files",
-    "compare_budget",
-    "compare_swrbudget",
-    "compare_heads",
-    "compare_concs",
-    "compare_stages",
-    "compare",
-    "setup_mf6",
-    "setup_mf6_comparison",
-    "get_mf6_comparison",
-    "get_mf6_files",
-    "get_mf6_blockdata",
-    "get_mf6_ftypes",
-    "get_mf6_mshape",
-    "get_mf6_nper",
 ]
```

### Comparing `mfpymake-1.2.7/pymake/__main__.py` & `mfpymake-1.2.8/pymake/__main__.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/cmds/build.py` & `mfpymake-1.2.8/pymake/cmds/build.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/cmds/createjson.py` & `mfpymake-1.2.8/pymake/cmds/createjson.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/cmds/mfpymakecli.py` & `mfpymake-1.2.8/pymake/cmds/mfpymakecli.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/plot/dependency_graphs.py` & `mfpymake-1.2.8/pymake/plot/dependency_graphs.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/pymake.py` & `mfpymake-1.2.8/pymake/pymake.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/pymake_base.py` & `mfpymake-1.2.8/pymake/pymake_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,14 @@
             inplace = True
             print(
                 f"Using meson to build {os.path.basename(target)}, "
                 + "ressetting inplace to True"
             )
 
     if srcdir is not None and target is not None:
-
         objdir_temp, moddir_temp, srcdir_temp = get_temporary_directories(
             appdir=appdir,
             target=pl.Path(target).stem,
         )
         if inplace:
             srcdir_temp = srcdir
```

### Comparing `mfpymake-1.2.7/pymake/pymake_build_apps.py` & `mfpymake-1.2.8/pymake/pymake_build_apps.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/pymake_parser.py` & `mfpymake-1.2.8/pymake/pymake_parser.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_Popen_wrapper.py` & `mfpymake-1.2.8/pymake/utils/_Popen_wrapper.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_compiler_language_files.py` & `mfpymake-1.2.8/pymake/utils/_compiler_language_files.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_compiler_switches.py` & `mfpymake-1.2.8/pymake/utils/_compiler_switches.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_dag.py` & `mfpymake-1.2.8/pymake/utils/_dag.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_file_utils.py` & `mfpymake-1.2.8/pymake/utils/_file_utils.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_meson_build.py` & `mfpymake-1.2.8/pymake/utils/_meson_build.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/_usgs_src_update.py` & `mfpymake-1.2.8/pymake/utils/_usgs_src_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Private functions to edit target source files in distributed software
 releases.
 
 """
 import os
+import pathlib as pl
 import shutil
 import sys
 import types
+from typing import Union
 
 from .usgsprograms import usgs_program_data
 
 
 def _get_function_names(module, select_name=None):
     """Get a dictionary of functions available in a user-specified source file.
     This function was developed to create a dictionary of functions in this
@@ -60,16 +62,15 @@
 
     """
     if isinstance(targets, str):
         targets = [targets]
 
     # remove exe extension from targets
     for idx, target in enumerate(targets):
-        if ".exe" in target.lower():
-            targets[idx] = target[:-4]
+        targets[idx] = pl.Path(target).with_suffix("").name
 
     # get a dictionary of update functions
     funcs = _get_function_names(sys.modules[__name__], select_name="_update_")
 
     # generate a list of available functions
     replace_funcs = []
     for target in targets:
@@ -402,14 +403,96 @@
     # update gwf2swt7.f
     _update_swt(srcdir)
 
     # update pcg7.f
     _update_pcg(srcdir)
 
 
+def _update_mfusg_gsi_files(srcdir, fc, cc, arch, double):
+    """Update GSI version of MODFLOW-USG source files
+
+    Parameters
+    ----------
+    srcdir : str
+        path to directory with source files
+    fc : str
+        fortran compiler
+    cc : str
+        c/c++ compiler
+    arch : str
+        architecture
+    double : bool
+        boolean indicating if compiler switches are used to build a
+        double precision target
+
+    Returns
+    -------
+
+    """
+    tags = {
+        "FMTARG = 'BINARY'": "FMTARG = 'UNFORMATTED'\n        ACCARG = 'STREAM'",
+        ",SHARED,ACCESS='SEQUENTIAL'": ",ACCESS='SEQUENTIAL'",
+        "FORM=FMTARG,SHARED,": "FORM=FMTARG,",
+        ",BUFFERED='YES',": ",",
+        ", BUFFERED='NO')": ")",
+        ",SHARE = 'DENYNONE'": ",",
+        ", SHARE = 'DENYNONE',": ",",
+        "FORM='FORMATTED',ACCESS='SEQUENTIAL',": "FORM='FORMATTED',ACCESS='SEQUENTIAL'",
+    }
+
+    fpth = pl.Path(srcdir) / "glo2basu1.f"
+    if fpth.exists():
+        with open(fpth) as f:
+            lines = f.readlines()
+        f = open(fpth, "w")
+        for idx, line in enumerate(lines):
+            for key, value in tags.items():
+                if key in line:
+                    line = line.replace(key, value)
+            f.write(line)
+        f.close()
+
+    tags = {",share='DENYNONE',": ","}
+
+    fpth = pl.Path(srcdir) / "UpdtSt.for"
+    if fpth.exists():
+        with open(fpth) as f:
+            lines = f.readlines()
+        f = open(fpth, "w")
+        for idx, line in enumerate(lines):
+            for key, value in tags.items():
+                if key in line:
+                    line = line.replace(key, value)
+            f.write(line)
+        f.close()
+
+    tag = "DEALLOCATE(ITHFLG)"
+    tag2 = "DEALLOCATE(LAYTYP)"
+    fpth = pl.Path(srcdir) / "gwf2bcf-lpf-u1.f"
+    if fpth.exists():
+        with open(fpth) as f:
+            lines = f.readlines()
+        f = open(fpth, "w")
+        for idx, line in enumerate(lines):
+            if tag in line:
+                line = line.replace(tag, f"!{tag}")
+                if tag2 in line:
+                    line = line.replace(tag2, f"{tag}\n        {tag2}")
+            f.write(line)
+        f.close()
+
+    # rename "utl7u1 RD.f" to "utl7u1_RD.f"
+    fpth = pl.Path(srcdir) / "utl7u1 RD.f"
+    if fpth.exists():
+        fpth_rename = pl.Path(srcdir) / "utl7u1_RD.f"
+        if fpth_rename.exists():
+            os.remove(fpth_rename)
+        os.rename(fpth, fpth_rename)
+
+
 def _update_mfnwt_files(srcdir, fc, cc, arch, double):
     """Update MODFLOW-NWT source files
 
     Parameters
     ----------
     srcdir : str
         path to directory with source files
@@ -761,15 +844,124 @@
         os.path.join(srcdir, "vs2dt3_3.f.tmp"),
         os.path.join(srcdir, "vs2dt3_3.f"),
     )
 
     return
 
 
+def _update_mf6_files(
+    srcdir: Union[str, os.PathLike],
+    fc: str,
+    cc: str,
+    arch: str,
+    double: bool,
+) -> None:
+    """
+    Update MODFLOW 6 source files to remove files with external dependencies.
+    This was required for releases >= 6.4.2
+
+    Parameters
+    ----------
+    srcdir : str
+        path to directory with source files
+    fc : str
+        fortran compiler
+    cc : str
+        c/c++ compiler
+    arch : str
+        architecture
+    double : bool
+        boolean indicating if compiler switches are used to build a
+        double precision target
+
+    Returns
+    -------
+
+    """
+    _update_mf6_external_dependencies(srcdir)
+    return
+
+
+def _update_libmf6_files(
+    srcdir: Union[str, os.PathLike],
+    fc: str,
+    cc: str,
+    arch: str,
+    double: bool,
+) -> None:
+    """
+    Update MODFLOW 6 shared object source files to remove files with external
+    dependencies. This was required for releases >= 6.4.2
+
+    Parameters
+    ----------
+    srcdir : str
+        path to directory with source files
+    fc : str
+        fortran compiler
+    cc : str
+        c/c++ compiler
+    arch : str
+        architecture
+    double : bool
+        boolean indicating if compiler switches are used to build a
+        double precision target
+
+    Returns
+    -------
+
+    """
+    _update_mf6_external_dependencies(srcdir, target="libmf6")
+    return
+
+
 # common source file replacement functions
+def _update_mf6_external_dependencies(
+    srcdir: Union[str, os.PathLike],
+    target: str = "mf6",
+) -> None:
+    """
+    Remove MODFLOW 6 files with external library dependencies (PETSc, MPI).
+
+
+    Parameters
+    ----------
+    srcdir : os.PathLike
+        path to directory with source files
+    target: str
+        target to create (Default is mf6)
+
+    Returns
+    -------
+    None
+
+    """
+    if not isinstance(srcdir, pl.Path):
+        srcdir = pl.Path(srcdir)
+    if target == "libmf6":
+        srcdir = srcdir.parent / "src"
+    parallel_files = (
+        "Utilities/Vector/PetscVector.F90",
+        "Utilities/Matrix/PetscMatrix.F90",
+        "Solution/PETSc/PetscSolver.F90",
+        "Solution/PETSc/PetscConvergence.F90",
+        "Distributed/MpiMessageBuilder.f90",
+        "Distributed/MpiRouter.f90",
+        "Distributed/MpiRunControl.F90",
+        "Distributed/MpiWorld.f90",
+        "Solution/ParallelSolution.f90",
+    )
+    for file in parallel_files:
+        path = srcdir / file
+        if path.is_file():
+            print(f'Removing..."{path}"')
+            os.remove(path)
+    return
+
+
 def _update_utl7(srcdir):
     """Update utl7.f source file
 
     Parameters
     ----------
     srcdir : str
         path to directory with source files
```

### Comparing `mfpymake-1.2.7/pymake/utils/download.py` & `mfpymake-1.2.8/pymake/utils/download.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/usgsprograms.py` & `mfpymake-1.2.8/pymake/utils/usgsprograms.py`

 * *Files identical despite different names*

### Comparing `mfpymake-1.2.7/pymake/utils/usgsprograms.txt` & `mfpymake-1.2.8/pymake/utils/usgsprograms.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 target     ,  version,  current, url                                                                                            , dirname             , srcdir              ,    standard_switch, double_switch, shared_object
-mf6        ,  6.4.1  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.1/mf6.4.1_linux.zip             , mf6.4.1_linux       , src                 ,    True           , False        , False
-zbud6      ,  6.4.1  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.1/mf6.4.1_linux.zip             , mf6.4.1_linux       , utils/zonebudget/src,    True           , False        , False
-libmf6     ,  6.4.1  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.1/mf6.4.1_linux.zip             , mf6.4.1_linux       , srcbmi              ,    True           , False        , True
+mf6        ,  6.4.2  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.2/mf6.4.2_linux.zip             , mf6.4.2_linux       , src                 ,    True           , False        , False
+zbud6      ,  6.4.2  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.2/mf6.4.2_linux.zip             , mf6.4.2_linux       , utils/zonebudget/src,    True           , False        , False
+libmf6     ,  6.4.2  ,  True   , https://github.com/MODFLOW-USGS/modflow6/releases/download/6.4.2/mf6.4.2_linux.zip             , mf6.4.2_linux       , srcbmi              ,    True           , False        , True
 mp7        ,  7.2.001,  True   , https://water.usgs.gov/water-resources/software/MODPATH/modpath_7_2_001.zip                    , modpath_7_2_001     , source              ,    True           , False        , False
 mt3dms     ,  5.3.0  ,  True   , https://hydro.geo.ua.edu/mt3d/mt3dms_530.exe                                                   , mt3dms5.3.0         , src/true-binary     ,    True           , False        , False
 mt3dusgs   ,  1.1.0  ,  True   , https://water.usgs.gov/water-resources/software/MT3D-USGS/mt3dusgs1.1.0.zip                    , mt3dusgs1.1.0       , src                 ,    True           , False        , False
 vs2dt      ,  3.3    ,  True   , https://water.usgs.gov/water-resources/software/VS2DI/vs2dt3_3.zip                             , vs2dt3_3            , include             ,    True           , False        , False
 triangle   ,  1.6    ,  True   , https://www.netlib.org/voronoi/triangle.zip                                                    , triangle1.6         , src                 ,    True           , False        , False
 gridgen    ,  1.0.02 ,  True   , https://water.usgs.gov/water-resources/software/GRIDGEN/gridgen.1.0.02.zip                     , gridgen.1.0.02      , src                 ,    True           , False        , False
 crt        ,  1.3.1  ,  True   , https://water.usgs.gov/ogw/CRT/CRT_1.3.1.zip                                                   , CRT_1.3.1           , SOURCE              ,    True           , False        , False
 sutra      ,  3.0    ,  True   , https://water.usgs.gov/water-resources/software/sutra/SUTRA_3_0_0.zip                          , SutraSuite          , SUTRA_3_0/source    ,    True           , False        , False
 mf2000     ,  1.19.01,  True   , https://water.usgs.gov/nrp/gwsoftware/modflow2000/mf2k1_19_01.tar.gz                           , mf2k.1_19           , src                 ,    True           , False        , False
 mf2005     ,  1.12.00,  True   , https://github.com/MODFLOW-USGS/mf2005/releases/download/v.1.12.00/MF2005.1_12u.zip            , MF2005.1_12u        , src                 ,    True           , True         , False
-mf2005.1.11,  1.11.00,  False  , https://water.usgs.gov/ogw/modflow/archive-mf2005/MODFLOW-2005_v1.11.00/mf2005v1_11_00_unix.zip, Unix                , src                 ,    True           , False        , False
 mfusg      ,  1.5    ,  True   , https://water.usgs.gov/water-resources/software/MODFLOW-USG/mfusg1_5.zip                       , mfusg1_5            , src                 ,    True           , True         , False
 zonbudusg  ,  1.5    ,  True   , https://water.usgs.gov/water-resources/software/MODFLOW-USG/mfusg1_5.zip                       , mfusg1_5            , src/zonebudusg      ,    True           , False        , False
 swtv4      ,  4.00.05,  True   , https://water.usgs.gov/water-resources/software/SEAWAT/swt_v4_00_05.zip                        , swt_v4_00_05        , source              ,    False          , True         , False
 mp6        ,  6.0.1  ,  True   , https://water.usgs.gov/water-resources/software/MODPATH/modpath.6_0_01.zip                     , modpath.6_0         , src                 ,    True           , False        , False
 mflgr      ,  2.0.0  ,  True   , https://water.usgs.gov/ogw/modflow-lgr/modflow-lgr-v2.0.0/mflgrv2_0_00.zip                     , mflgr.2_0           , src                 ,    True           , True         , False
 zonbud3    ,  3.01   ,  True   , https://water.usgs.gov/water-resources/software/ZONEBUDGET/zonbud3_01.exe                      , Zonbud.3_01         , Src                 ,    True           , False        , False
 mfnwt1.1.4 ,  1.1.4  ,  False  , https://water.usgs.gov/water-resources/software/MODFLOW-NWT/MODFLOW-NWT_1.1.4.zip              , MODFLOW-NWT_1.1.4   , src                 ,    True           , False        , False
 mfnwt      ,  1.3.0  ,  True   , https://water.usgs.gov/water-resources/software/MODFLOW-NWT/MODFLOW-NWT_1.3.0.zip              , MODFLOW-NWT         , src                 ,    True           , True         , False
+mfusg_gsi  ,  2.1.1  ,  True   , https://www.gsienv.com/wp-content/uploads/2023/04/USG-Transport-V_2.1.1.zip                    , USGT-v2-1-1-source  , .                   ,    True           , False        , False
```

### Comparing `mfpymake-1.2.7/setup.cfg` & `mfpymake-1.2.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	Bug Tracker = https://github.com/modflowpy/pymake/issues
 	Source Code = https://github.com/modflowpy/pymake
 
 [options]
 include_package_data = True  # includes files listed in MANIFEST.in
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	numpy
 	requests
 	networkx >= 2.6.3
 	meson
 	ninja
 	pydotplus
```

