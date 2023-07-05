# Comparing `tmp/c3s_sm-0.1.2.tar.gz` & `tmp/c3s_sm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/c3s_sm-0.1.2.tar", last modified: Fri Jul  3 19:49:19 2020, max compression
+gzip compressed data, was "c3s_sm-0.2.0.tar", last modified: Wed Jul  5 11:56:12 2023, max compression
```

## Comparing `c3s_sm-0.1.2.tar` & `c3s_sm-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.852371 c3s_sm-0.1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      541 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.gitattributes
--rw-rw-r--   0 travis    (2000) travis    (2000)      450 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      158 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.gitmodules
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1632 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3434 2020-07-03 19:49:19.852371 c3s_sm-0.1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2312 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.848369 c3s_sm-0.1.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)   394006 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/5x5_cell_partitioning.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     7606 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/Makefile
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.848369 c3s_sm-0.1.2/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/_static/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/_static/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/changelog.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2635 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/img2ts.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      348 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/license.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2192 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/reading.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/docs/varnames.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      216 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/environment.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1471 2020-07-03 19:49:19.852371 c3s_sm-0.1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      570 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.844367 c3s_sm-0.1.2/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.848369 c3s_sm-0.1.2/src/c3s_sm/
--rw-rw-r--   0 travis    (2000) travis    (2000)      480 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/src/c3s_sm/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/src/c3s_sm/grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12904 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/src/c3s_sm/interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14599 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/src/c3s_sm/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7751 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/src/c3s_sm/reshuffle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.848369 c3s_sm-0.1.2/src/c3s_sm.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3434 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1063 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-07-03 19:49:19.000000 c3s_sm-0.1.2/src/c3s_sm.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.852371 c3s_sm-0.1.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      311 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/test_grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5690 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/test_interface_img.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2834 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/test_interface_img_stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5488 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/test_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3839 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/tests/test_reshuffle.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-03 19:49:19.852371 c3s_sm-0.1.2/use_case/
--rw-rw-r--   0 travis    (2000) travis    (2000)    33123 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/use_case/C3S_v201812_COMBINED_sample.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  1280979 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/use_case/Timeseries_locations.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   384902 2020-07-03 19:46:22.000000 c3s_sm-0.1.2/use_case/c3s_sm_monthly_anomalies.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.052391 c3s_sm-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.060392 c3s_sm-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.064392 c3s_sm-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   394006 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/5x5_cell_partitioning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.064392 c3s_sm-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/docs_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/img2ts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/reading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/docs/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/use_case/C3S_v201812_COMBINED_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1280979 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/use_case/Timeseries_locations.png
+-rw-r--r--   0 runner    (1001) docker     (123)   384902 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/use_case/c3s_sm_monthly_anomalies.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/docs/varnames.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.052391 c3s_sm-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/src/c3s_sm/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/src/c3s_sm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/src/c3s_sm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/src/c3s_sm/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/src/c3s_sm/reshuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/src/c3s_sm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-05 11:56:11.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-05 11:56:12.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:56:11.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 11:56:11.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:55:53.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 11:56:11.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 11:56:11.000000 c3s_sm-0.2.0/src/c3s_sm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:56:12.068392 c3s_sm-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/test_interface_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/test_interface_img_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tests/test_reshuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-05 11:53:30.000000 c3s_sm-0.2.0/tox.ini
```

### Comparing `c3s_sm-0.1.2/.coveragerc` & `c3s_sm-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/LICENSE.txt` & `c3s_sm-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/PKG-INFO` & `c3s_sm-0.2.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,85 @@
-Metadata-Version: 2.1
-Name: c3s_sm
-Version: 0.1.2
-Summary: Readers and time series coverters for the C3S Soil Moisture data set
-Home-page: https://github.com/TUW-GEO/c3s_sm
-Author: TU Wien
-Author-email: remote.sensing@geo.tuwien.ac.at
-License: mit
-Project-URL: Documentation, https://c3s-sm.readthedocs.io/en/latest/
-Description: ============
-        c3s_sm
-        ============
-        
-        
-        .. image:: https://travis-ci.org/TUW-GEO/c3s_sm.svg?branch=master
-            :target: https://travis-ci.org/TUW-GEO/c3s_sm
-        
-        .. image:: https://coveralls.io/repos/github/TUW-GEO/c3s_sm/badge.svg?branch=master
-            :target: https://coveralls.io/github/TUW-GEO/c3s_sm?branch=master
-        
-        .. image:: https://badge.fury.io/py/c3s-sm.svg
-            :target: https://badge.fury.io/py/c3s-sm
-         
-        .. image:: https://readthedocs.org/projects/c3s_sm/badge/?version=latest
-            :target: http://c3s_sm.readthedocs.io/en/latest/?badge=latest
-        
-        Reading and reshuffling of C3S soil moisture Written in Python.
-        
-        Installation
-        ============
-        
-        Setup of a complete environment with `conda
-        <http://conda.pydata.org/miniconda.html>`_ can be performed using the following
-        commands:
-        
-        .. code-block:: shell
-        
-          git clone git@github.com:TUW-GEO/c3s_sm.git c3s_sm
-          cd c3s_sm
-          conda env create -f environment.yml
-          source activate c3s_sm
-        
-        Supported Products
-        ==================
-        
-        At the moment this package supports C3S soil moisture data
-        in netCDF format (reading and time series creation)
-        with a spatial sampling of 0.25 degrees.
-        
-        Contribute
-        ==========
-        
-        We are happy if you want to contribute. Please raise an issue explaining what
-        is missing or if you find a bug. We will also gladly accept pull requests
-        against our master branch for new features or bug fixes.
-        
-        Development setup
-        -----------------
-        
-        For Development we also recommend a ``conda`` environment. You can create one
-        including test dependencies and debugger by running
-        ``conda env create -f environment.yml``. This will create a new ``c3s_sm``
-        environment which you can activate by using ``source activate c3s_sm``.
-        
-        Guidelines
-        ----------
-        
-        If you want to contribute please follow these steps:
-        
-        - Fork the c3s_sm repository to your account
-        - Clone the repository, make sure you use ``git clone --recursive`` to also get
-          the test data repository.
-        - make a new feature branch from the c3s_sm master branch
-        - Add your feature
-        - Please include tests for your contributions in one of the test directories.
-          We use py.test so a simple function called test_my_feature is enough
-        - submit a pull request to our master branch
-        
-        Note
-        ====
-        
-        This project has been set up using PyScaffold 2.5. For details and usage
-        information on PyScaffold see http://pyscaffold.readthedocs.org/.
-        
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: testing
+============
+c3s_sm
+============
+
+
+.. image:: https://github.com/TUW-GEO/c3s_sm/workflows/Automated%20Tests/badge.svg?branch=master
+   :target: https://github.com/TUW-GEO/c3s_sm/actions
+
+.. image:: https://coveralls.io/repos/github/TUW-GEO/c3s_sm/badge.svg?branch=master
+    :target: https://coveralls.io/github/TUW-GEO/c3s_sm?branch=master
+
+.. image:: https://badge.fury.io/py/c3s-sm.svg
+    :target: https://badge.fury.io/py/c3s-sm
+ 
+.. image:: https://readthedocs.org/projects/c3s_sm/badge/?version=latest
+    :target: http://c3s_sm.readthedocs.io/en/latest/?badge=latest
+
+Reading and reshuffling of C3S soil moisture Written in Python.
+
+Installation
+============
+
+Setup of a complete environment with `conda
+<http://conda.pydata.org/miniconda.html>`_ can be performed using the following
+commands:
+
+.. code-block:: shell
+
+  git clone git@github.com:TUW-GEO/c3s_sm.git c3s_sm
+  cd c3s_sm
+  conda env create -f environment.yml
+  source activate c3s_sm
+
+Tutorials
+=========
+
+We provide (general) tutorials on using the C3S Soil Moisture data:
+
+- `Tutorial 1: DataAccess from CDS & Anomaly computation <https://c3s-sm.readthedocs.io/en/latest/T1_DataAccess_Anomalies.html>`_
+
+These tutorials are designed to run on `mybinder.org <mybinder.org/>`_
+You can find the code for all examples in
+`this repository <https://github.com/TUW-GEO/c3s_sm-tutorials>`_.
+
+Supported Products
+==================
+
+At the moment this package supports C3S soil moisture data
+in netCDF format (reading and time series creation)
+with a spatial sampling of 0.25 degrees.
+
+Contribute
+==========
+
+We are happy if you want to contribute. Please raise an issue explaining what
+is missing or if you find a bug. We will also gladly accept pull requests
+against our master branch for new features or bug fixes.
+
+Development setup
+-----------------
+
+For Development we also recommend a ``conda`` environment. You can create one
+including test dependencies and debugger by running
+``conda env create -f environment.yml``. This will create a new ``c3s_sm``
+environment which you can activate by using ``source activate c3s_sm``.
+
+Guidelines
+----------
+
+If you want to contribute please follow these steps:
+
+- Fork the c3s_sm repository to your account
+- Clone the repository, make sure you use ``git clone --recursive`` to also get
+  the test data repository.
+- make a new feature branch from the c3s_sm master branch
+- Add your feature
+- Please include tests for your contributions in one of the test directories.
+  We use py.test so a simple function called test_my_feature is enough
+- submit a pull request to our master branch
+
+Note
+====
+
+This project has been set up using PyScaffold 2.5. For details and usage
+information on PyScaffold see http://pyscaffold.readthedocs.org/.
```

### Comparing `c3s_sm-0.1.2/docs/5x5_cell_partitioning.png` & `c3s_sm-0.2.0/docs/5x5_cell_partitioning.png`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/docs/conf.py` & `c3s_sm-0.2.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,68 @@
-# -*- coding: utf-8 -*-
-#
 # This file is execfile()d with the current directory set to its containing dir.
 #
-# Note that not all possible configuration values are present in this
-# autogenerated file.
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import os
 import sys
 import inspect
 import shutil
 
-__location__ = os.path.join(os.getcwd(), os.path.dirname(
-    inspect.getfile(inspect.currentframe())))
+import subprocess
+
+
+# Create kernel for notebooks
+on_rtd = "READTHEDOCS" in os.environ and os.environ["READTHEDOCS"]
+if on_rtd:
+    rtd_project = os.environ["READTHEDOCS_PROJECT"]
+    rtd_version = os.environ["READTHEDOCS_VERSION"]
+    interpreter = (
+        f"/home/docs/checkouts/readthedocs.org/user_builds/{rtd_project}/"
+        f"conda/{rtd_version}/bin/python"
+    )
+else:
+    interpreter = "python"
+
+print("Installing kernel")
+subprocess.run(
+    [
+        interpreter,
+        "-m",
+        "ipykernel",
+        "install",
+        "--user",
+        "--name",
+        "conda-env-c3s_sm-py",
+        "--display-name",
+        "Python [conda env:c3s_sm]"
+    ],
+    check=True,
+    capture_output=True,
+)
+print("Done")
+
+
+# -- Path setup --------------------------------------------------------------
+
+__location__ = os.path.dirname(__file__)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.join(__location__, '../src'))
+sys.path.insert(0, os.path.join(__location__, "../src"))
 
-# -- Run sphinx-apidoc ------------------------------------------------------
+# -- Run sphinx-apidoc -------------------------------------------------------
 # This hack is necessary since RTD does not issue `sphinx-apidoc` before running
 # `sphinx-build -b html . _build/html`. See Issue:
-# https://github.com/rtfd/readthedocs.org/issues/1139
+# https://github.com/readthedocs/readthedocs.org/issues/1139
 # DON'T FORGET: Check the box "Install your project inside a virtualenv using
 # setup.py install" in the RTD Advanced Settings.
 # Additionally it helps us to avoid running apidoc manually
 
 try:  # for Sphinx >= 1.7
     from sphinx.ext import apidoc
 except ImportError:
@@ -39,77 +73,94 @@
 try:
     shutil.rmtree(output_dir)
 except FileNotFoundError:
     pass
 
 try:
     import sphinx
-    from pkg_resources import parse_version
 
-    cmd_line_template = "sphinx-apidoc -f -o {outputdir} {moduledir}"
-    cmd_line = cmd_line_template.format(outputdir=output_dir, moduledir=module_dir)
+    cmd_line = f"sphinx-apidoc --implicit-namespaces -f -o {output_dir} {module_dir}"
 
     args = cmd_line.split(" ")
-    if parse_version(sphinx.__version__) >= parse_version('1.7'):
+    if tuple(sphinx.__version__.split(".")) >= ("1", "7"):
+        # This is a rudimentary parse_version to avoid external dependencies
         args = args[1:]
 
     apidoc.main(args)
 except Exception as e:
     print("Running `sphinx-apidoc` failed!\n{}".format(e))
 
-# -- General configuration -----------------------------------------------------
+# -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx.ext.todo',
-              'sphinx.ext.autosummary', 'sphinx.ext.viewcode', 'sphinx.ext.coverage',
-              'sphinx.ext.doctest', 'sphinx.ext.ifconfig', 'sphinx.ext.mathjax',
-              'sphinx.ext.napoleon']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "nbsphinx",
+]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'c3s_sm'
-copyright = u'2020, TU Wien'
+project = "c3s_sm"
+copyright = "2023, TU Wien"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = ''  # Is set by calling `setup.py docs`
-# The full version, including alpha/beta/rc tags.
-release = ''  # Is set by calling `setup.py docs`
+# version: The short X.Y version.
+# release: The full version, including alpha/beta/rc tags.
+# If you don’t need the separation provided between version and release,
+# just set them both to the same value.
+try:
+    from c3s_sm import __version__ as version
+except ImportError:
+    version = ""
+
+if not version or version.lower() == "unknown":
+    version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
+
+release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".venv",]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
@@ -118,48 +169,47 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
+# If this is True, todo emits a warning for each TODO entries. The default is False.
+todo_emit_warnings = True
+
 
-# -- Options for HTML output ---------------------------------------------------
+# -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "sphinx_rtd_theme"
 
+html_extra_path = ['c3s_sm-tutorials']
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    'sidebar_width': '300px',
-    'page_width': '1200px'
+    "sidebar_width": "300px",
+    "page_width": "1200px"
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-try:
-    from c3s_sm import __version__ as version
-except ImportError:
-    pass
-else:
-    release = version
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # html_logo = ""
@@ -168,15 +218,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -212,35 +262,32 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'c3s_sm-doc'
+htmlhelp_basename = "c3s_sm-doc"
 
 
-# -- Options for LaTeX output --------------------------------------------------
+# -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-# 'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-# 'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-# 'preamble': '',
+    # The paper size ("letterpaper" or "a4paper").
+    # "papersize": "letterpaper",
+    # The font size ("10pt", "11pt" or "12pt").
+    # "pointsize": "10pt",
+    # Additional stuff for the LaTeX preamble.
+    # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'user_guide.tex', u'c3s_sm Documentation',
-   u'Wolfgang Preimesberger', 'manual'),
+    ("index", "user_guide.tex", "c3s_sm Documentation", "TU Wien", "manual")
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -255,18 +302,22 @@
 
 # Documents to append as an appendix to all manuals.
 # latex_appendices = []
 
 # If false, no module index is generated.
 # latex_domain_indices = True
 
-# -- External mapping ------------------------------------------------------------
-python_version = '.'.join(map(str, sys.version_info[0:2]))
+# -- External mapping --------------------------------------------------------
+python_version = ".".join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
-    'sphinx': ('http://www.sphinx-doc.org/en/stable', None),
-    'python': ('https://docs.python.org/' + python_version, None),
-    'matplotlib': ('https://matplotlib.org', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy', None),
-    'sklearn': ('http://scikit-learn.org/stable', None),
-    'pandas': ('http://pandas.pydata.org/pandas-docs/stable', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    "sphinx": ("https://www.sphinx-doc.org/en/master", None),
+    "python": ("https://docs.python.org/" + python_version, None),
+    "matplotlib": ("https://matplotlib.org", None),
+    "numpy": ("https://numpy.org/doc/stable", None),
+    "sklearn": ("https://scikit-learn.org/stable", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
+    "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
+    "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
+
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `c3s_sm-0.1.2/docs/img2ts.rst` & `c3s_sm-0.2.0/docs/img2ts.rst`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/docs/reading.rst` & `c3s_sm-0.2.0/docs/reading.rst`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/docs/varnames.rst` & `c3s_sm-0.2.0/docs/varnames.rst`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/setup.cfg` & `c3s_sm-0.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 [metadata]
 name = c3s_sm
-summary = Readers and time series coverters for the C3S Soil Moisture data set
+description = Readers and time series coverters for the C3S Soil Moisture data set
 author = TU Wien
-author-email = remote.sensing@geo.tuwien.ac.at
+author_email = remote.sensing@geo.tuwien.ac.at
 license = mit
-long-description = file: README.rst
-long-description-content-type = text/x-rst; charset=UTF-8
+long_description = file: README.rst
+long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/TUW-GEO/c3s_sm
-project-urls = 
+project_urls = 
 	Documentation = https://c3s-sm.readthedocs.io/en/latest/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
-packages = find:
+packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-setup_requires = pyscaffold>=3.2a0,<3.3a0
-install_requires = numpy
+install_requires = 
+	importlib-metadata; python_version<"3.8"
+	numpy
 	pandas
 	pygeobase
 	pyresample
 	netCDF4
-	repurpose
 	pynetcf
-	repurpose
+	repurpose>=0.9
 	parse
-	smecv_grid
+	cadati
+	smecv_grid==0.3
 	more_itertools
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
-	pytest==5.0.1
+	pytest
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	c3s_repurpose = c3s_sm.reshuffle:run
 
 [test]
@@ -80,15 +81,15 @@
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
-version = 3.2.3
+version = 4.4
 package = c3s_sm
 extensions = 
 	no_skeleton
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `c3s_sm-0.1.2/src/c3s_sm/reshuffle.py` & `c3s_sm-0.2.0/src/c3s_sm/reshuffle.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,36 +5,32 @@
 """
 
 import os
 import sys
 import argparse
 from datetime import datetime
 
+import pandas as pd
 from repurpose.img2ts import Img2Ts
-from c3s_sm.interface import C3S_Nc_Img_Stack, c3s_filename_template
-from c3s_sm.grid import C3SLandGrid, C3SCellGrid
+from c3s_sm.interface import C3S_Nc_Img_Stack, fntempl
 import c3s_sm.metadata as metadata
 from c3s_sm.metadata import C3S_daily_tsatt_nc, C3S_dekmon_tsatt_nc
-from pygeogrids.grids import BasicGrid
-
-import numpy as np
-
+from smecv_grid.grid import SMECV_Grid_v052
 from parse import parse
-
 from netCDF4 import Dataset
 
-
 def mkdate(datestring):
     """
     Create date string.
 
     Parameters
     ----------
     datestring : str
         Date string.
+
     Returns
     -------
     datestr : datetime
         Date string as datetime.
     """
     if len(datestring) == 10:
         return datetime.strptime(datestring, '%Y-%m-%d')
@@ -43,120 +39,123 @@
 
 def str2bool(val):
     if val in ['True', 'true', 't', 'T', '1']:
         return True
     else:
         return False
 
-
 def parse_filename(data_dir):
-    '''
+    """
     Take the first file in the passed directory and use its file name to
     retrieve the product type, version number and variables in the file.
 
     Parameters
     ----------
     inroot : str
         Input root directory
 
     Returns
     -------
     file_args : dict
         Parsed arguments from file name
     file_vars : list
         Names of parameters in the first detected file
-    '''
-    template = c3s_filename_template()
+    """
 
     for curr, subdirs, files in os.walk(data_dir):
-        for f in files:
-            file_args = parse(template, f)
+        for f in sorted(files):
+            file_args = parse(fntempl, f)
             if file_args is None:
                 continue
             else:
                 file_args = file_args.named
                 file_args['datetime'] = '{datetime}'
                 file_vars = Dataset(os.path.join(curr,f)).variables.keys()
                 return file_args, list(file_vars)
 
     raise IOError('No file name in passed directory fits to template')
 
 
 def reshuffle(input_root, outputpath, startdate, enddate,
-              parameters, land_points=True,
-              imgbuffer=50):
+              parameters=None, land_points=True, bbox=None,
+              ignore_meta=False, imgbuffer=500):
     """
     Reshuffle method applied to C3S data.
+
     Parameters
     ----------
     input_root: string
         input path where c3s images were downloaded.
     outputpath : string
         Output path.
     startdate : datetime
         Start date.
     enddate : datetime
         End date.
-    parameters: list
+    parameters: list, optional (default: None)
         parameters to read and convert
     land_points : bool, optional (default: True)
         Use the land grid to calculate time series on.
         Leads to faster processing and smaller files.
+    bbox : tuple, optional (default: None)
+        Min lon, min lat, max lon, max lat
+        BBox to read data for.
+    ignore_meta : bool, optional (default: False)
+        Ignore metadata and reshuffle only the values. Can be used e.g. if a
+        version is not yet supported.
     imgbuffer: int, optional (default: 50)
         How many images to read at once before writing time series.
     """
 
     if land_points:
-        grid = C3SLandGrid()
+        grid = SMECV_Grid_v052('land')
     else:
-        grid = C3SCellGrid()
-
-    gpis, lons, lats, cells = grid.get_grid_points()
-    grid_vars = {'gpis': gpis, 'lons':lons, 'lats':lats}
-    # repurpose cannot handle masked arrays
-    for k, v in grid_vars.items(): # type v: np.ma.MaskedArray
-        if isinstance(v, np.ma.MaskedArray):
-            grid_vars[k] = v.filled()
+        grid = SMECV_Grid_v052(None)
 
-    grid = BasicGrid(lon=grid_vars['lons'], lat=grid_vars['lats'], gpis=grid_vars['gpis']).to_cell_grid(5.)
+    if bbox:
+        grid = grid.subgrid_from_bbox(*bbox)
 
     if parameters is None:
         file_args, file_vars = parse_filename(input_root)
         parameters = [p for p in file_vars if p not in ['lat', 'lon', 'time']]
 
-    input_dataset = C3S_Nc_Img_Stack(data_path=input_root, parameters=parameters,
-                                     subgrid=grid, array_1D=True)
-
-    prod_args = input_dataset.fname_args
-
-
-    kwargs = {'product_sensor_type' : prod_args['sensor_type'].lower(),
-              'sub_version' : '.' + prod_args['sub_version'],
-              'product_sub_type': prod_args['sub_prod']}
+    subpath_templ = ('%Y',) if os.path.isdir(os.path.join(input_root, str(startdate.year))) else None
+    input_dataset = C3S_Nc_Img_Stack(data_path=input_root,
+                                     parameters=parameters,
+                                     subgrid=grid,
+                                     flatten=True,
+                                     fillval=None,
+                                     subpath_templ=subpath_templ)
+
+    if not ignore_meta:
+        prod_args = input_dataset.fname_args
+
+        kwargs = {'sensor_type': prod_args['prod'].lower(),
+                  'cdr_type': prod_args['cdr'],
+                  'product_temp_res':  prod_args['temp'],
+                  'cls': getattr(metadata, f"C3S_SM_TS_Attrs_{prod_args['vers']}")}
+
+        if prod_args['temp'].upper() == 'DAILY':
+            kwargs.pop('product_temp_res')
+            attrs = C3S_daily_tsatt_nc(**kwargs)
+        else:
+            attrs = C3S_dekmon_tsatt_nc(**kwargs)
 
-    class_str = "C3S_SM_TS_Attrs_%s" % (prod_args['version'])
-    subattr = getattr(metadata, class_str)
+        ts_attributes = {}
+        global_attributes = attrs.global_attr
 
-    if prod_args['temp_res'] == 'DAILY':
-        attrs = C3S_daily_tsatt_nc(subattr, **kwargs)
+        for var in parameters:
+            ts_attributes[var] = attrs.ts_attributes[var]
     else:
-        attrs = C3S_dekmon_tsatt_nc(subattr, **kwargs)
-
-    ts_attributes = {}
-    global_attributes = attrs.global_attr
-
-    # todo: attrs for all vars or only for the ones that TS were created for.
-    for var in parameters:
-        ts_attributes.update(attrs.ts_attributes[var])
-
+        global_attributes = None
+        ts_attributes = None
 
     if not os.path.exists(outputpath):
         os.makedirs(outputpath)
 
-
     reshuffler = Img2Ts(input_dataset=input_dataset, outputpath=outputpath,
                         startdate=startdate, enddate=enddate, input_grid=grid,
                         imgbuffer=imgbuffer, cellsize_lat=5.0,
                         cellsize_lon=5.0, global_attr=global_attributes, zlib=True,
                         unlim_chunksize=1000, ts_attributes=ts_attributes)
     reshuffler.calc()
 
@@ -198,26 +197,33 @@
                               "E.g. sm for creating soil moisture time series."
                               "If None are passed, all variables from the first image file in the path are used."))
 
     parser.add_argument("--land_points", type=str2bool, default='False',
                         help=("Set True to convert only land points as defined"
                               " in the C3s land mask (faster and less/smaller files)"))
 
-    parser.add_argument("--imgbuffer", type=int, default=50,
+    parser.add_argument("--bbox", type=float, default=None, nargs=4,
+                        help=("min_lon min_lat max_lon max_lat. "
+                              "Bounding Box (lower left and upper right corner) "
+                              "of area to reshuffle (WGS84)"))
+
+    parser.add_argument("--ignore_meta", type=str2bool, default='False',
+                        help=("Do not apply image metadata to the time series."
+                              "E.g. for unsupported data versions."))
+
+    parser.add_argument("--imgbuffer", type=int, default=200,
                         help=("How many images to read at once. Bigger "
                               "numbers make the conversion faster but "
                               "consume more memory."))
 
     args = parser.parse_args(args)
     # set defaults that can not be handled by argparse
 
-    print("Converting data from {} to"
-          " {} into folder {}.".format(args.start.isoformat(),
-                                      args.end.isoformat(),
-                                      args.timeseries_root))
+    print(f"Converting data from {args.start.isoformat()} to"
+          f" {args.end.isoformat()} into folder {args.timeseries_root}.")
 
     return args
 
 
 def main(args):
     """
     Main routine used for command line interface.
@@ -230,26 +236,13 @@
 
     reshuffle(args.dataset_root,
               args.timeseries_root,
               args.start,
               args.end,
               args.parameters,
               land_points=args.land_points,
+              bbox=args.bbox,
+              ignore_meta=args.ignore_meta,
               imgbuffer=args.imgbuffer)
 
-
-
 def run():
     main(sys.argv[1:])
-
-if __name__ == '__main__':
-
-
-    cmd = [r'C:\Temp\tcdr\active_daily', r'C:\Temp\tcdr\ts',
-           '1991-08-05', '1991-08-10', '--land_points', 'True']
-    main(cmd)
-
-    from interface import C3STs
-
-    ds = C3STs(r'C:\Temp\tcdr\ts')
-    ds.read(47.875, 7.875)
-    run()
```

### Comparing `c3s_sm-0.1.2/src/c3s_sm.egg-info/PKG-INFO` & `c3s_sm-0.2.0/src/c3s_sm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,103 @@
 Metadata-Version: 2.1
 Name: c3s-sm
-Version: 0.1.2
+Version: 0.2.0
 Summary: Readers and time series coverters for the C3S Soil Moisture data set
 Home-page: https://github.com/TUW-GEO/c3s_sm
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: mit
 Project-URL: Documentation, https://c3s-sm.readthedocs.io/en/latest/
-Description: ============
-        c3s_sm
-        ============
-        
-        
-        .. image:: https://travis-ci.org/TUW-GEO/c3s_sm.svg?branch=master
-            :target: https://travis-ci.org/TUW-GEO/c3s_sm
-        
-        .. image:: https://coveralls.io/repos/github/TUW-GEO/c3s_sm/badge.svg?branch=master
-            :target: https://coveralls.io/github/TUW-GEO/c3s_sm?branch=master
-        
-        .. image:: https://badge.fury.io/py/c3s-sm.svg
-            :target: https://badge.fury.io/py/c3s-sm
-         
-        .. image:: https://readthedocs.org/projects/c3s_sm/badge/?version=latest
-            :target: http://c3s_sm.readthedocs.io/en/latest/?badge=latest
-        
-        Reading and reshuffling of C3S soil moisture Written in Python.
-        
-        Installation
-        ============
-        
-        Setup of a complete environment with `conda
-        <http://conda.pydata.org/miniconda.html>`_ can be performed using the following
-        commands:
-        
-        .. code-block:: shell
-        
-          git clone git@github.com:TUW-GEO/c3s_sm.git c3s_sm
-          cd c3s_sm
-          conda env create -f environment.yml
-          source activate c3s_sm
-        
-        Supported Products
-        ==================
-        
-        At the moment this package supports C3S soil moisture data
-        in netCDF format (reading and time series creation)
-        with a spatial sampling of 0.25 degrees.
-        
-        Contribute
-        ==========
-        
-        We are happy if you want to contribute. Please raise an issue explaining what
-        is missing or if you find a bug. We will also gladly accept pull requests
-        against our master branch for new features or bug fixes.
-        
-        Development setup
-        -----------------
-        
-        For Development we also recommend a ``conda`` environment. You can create one
-        including test dependencies and debugger by running
-        ``conda env create -f environment.yml``. This will create a new ``c3s_sm``
-        environment which you can activate by using ``source activate c3s_sm``.
-        
-        Guidelines
-        ----------
-        
-        If you want to contribute please follow these steps:
-        
-        - Fork the c3s_sm repository to your account
-        - Clone the repository, make sure you use ``git clone --recursive`` to also get
-          the test data repository.
-        - make a new feature branch from the c3s_sm master branch
-        - Add your feature
-        - Please include tests for your contributions in one of the test directories.
-          We use py.test so a simple function called test_my_feature is enough
-        - submit a pull request to our master branch
-        
-        Note
-        ====
-        
-        This project has been set up using PyScaffold 2.5. For details and usage
-        information on PyScaffold see http://pyscaffold.readthedocs.org/.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+============
+c3s_sm
+============
+
+
+.. image:: https://github.com/TUW-GEO/c3s_sm/workflows/Automated%20Tests/badge.svg?branch=master
+   :target: https://github.com/TUW-GEO/c3s_sm/actions
+
+.. image:: https://coveralls.io/repos/github/TUW-GEO/c3s_sm/badge.svg?branch=master
+    :target: https://coveralls.io/github/TUW-GEO/c3s_sm?branch=master
+
+.. image:: https://badge.fury.io/py/c3s-sm.svg
+    :target: https://badge.fury.io/py/c3s-sm
+ 
+.. image:: https://readthedocs.org/projects/c3s_sm/badge/?version=latest
+    :target: http://c3s_sm.readthedocs.io/en/latest/?badge=latest
+
+Reading and reshuffling of C3S soil moisture Written in Python.
+
+Installation
+============
+
+Setup of a complete environment with `conda
+<http://conda.pydata.org/miniconda.html>`_ can be performed using the following
+commands:
+
+.. code-block:: shell
+
+  git clone git@github.com:TUW-GEO/c3s_sm.git c3s_sm
+  cd c3s_sm
+  conda env create -f environment.yml
+  source activate c3s_sm
+
+Tutorials
+=========
+
+We provide (general) tutorials on using the C3S Soil Moisture data:
+
+- `Tutorial 1: DataAccess from CDS & Anomaly computation <https://c3s-sm.readthedocs.io/en/latest/T1_DataAccess_Anomalies.html>`_
+
+These tutorials are designed to run on `mybinder.org <mybinder.org/>`_
+You can find the code for all examples in
+`this repository <https://github.com/TUW-GEO/c3s_sm-tutorials>`_.
+
+Supported Products
+==================
+
+At the moment this package supports C3S soil moisture data
+in netCDF format (reading and time series creation)
+with a spatial sampling of 0.25 degrees.
+
+Contribute
+==========
+
+We are happy if you want to contribute. Please raise an issue explaining what
+is missing or if you find a bug. We will also gladly accept pull requests
+against our master branch for new features or bug fixes.
+
+Development setup
+-----------------
+
+For Development we also recommend a ``conda`` environment. You can create one
+including test dependencies and debugger by running
+``conda env create -f environment.yml``. This will create a new ``c3s_sm``
+environment which you can activate by using ``source activate c3s_sm``.
+
+Guidelines
+----------
+
+If you want to contribute please follow these steps:
+
+- Fork the c3s_sm repository to your account
+- Clone the repository, make sure you use ``git clone --recursive`` to also get
+  the test data repository.
+- make a new feature branch from the c3s_sm master branch
+- Add your feature
+- Please include tests for your contributions in one of the test directories.
+  We use py.test so a simple function called test_my_feature is enough
+- submit a pull request to our master branch
+
+Note
+====
+
+This project has been set up using PyScaffold 2.5. For details and usage
+information on PyScaffold see http://pyscaffold.readthedocs.org/.
```

### Comparing `c3s_sm-0.1.2/src/c3s_sm.egg-info/SOURCES.txt` & `c3s_sm-0.2.0/src/c3s_sm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 .coveragerc
 .gitattributes
 .gitignore
 .gitmodules
 .readthedocs.yml
-.travis.yml
 AUTHORS.rst
 CHANGELOG.rst
+CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 environment.yml
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
+.github/workflows/ci.yml
 docs/5x5_cell_partitioning.png
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
+docs/contributing.rst
+docs/docs_env.yml
 docs/img2ts.rst
 docs/index.rst
 docs/license.rst
 docs/reading.rst
+docs/readme.rst
 docs/requirements.txt
 docs/varnames.rst
 docs/_static/.gitignore
-docs/_static/requirements.txt
+docs/use_case/C3S_v201812_COMBINED_sample.csv
+docs/use_case/Timeseries_locations.png
+docs/use_case/c3s_sm_monthly_anomalies.ipynb
 src/c3s_sm/__init__.py
-src/c3s_sm/grid.py
 src/c3s_sm/interface.py
 src/c3s_sm/metadata.py
 src/c3s_sm/reshuffle.py
 src/c3s_sm.egg-info/PKG-INFO
 src/c3s_sm.egg-info/SOURCES.txt
 src/c3s_sm.egg-info/dependency_links.txt
 src/c3s_sm.egg-info/entry_points.txt
 src/c3s_sm.egg-info/not-zip-safe
 src/c3s_sm.egg-info/requires.txt
 src/c3s_sm.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
-tests/test_grid.py
 tests/test_interface_img.py
 tests/test_interface_img_stack.py
 tests/test_metadata.py
-tests/test_reshuffle.py
-use_case/C3S_v201812_COMBINED_sample.csv
-use_case/Timeseries_locations.png
-use_case/c3s_sm_monthly_anomalies.ipynb
+tests/test_reshuffle.py
```

### Comparing `c3s_sm-0.1.2/tests/test_interface_img.py` & `c3s_sm-0.2.0/tests/test_interface_img.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,135 @@
 # -*- coding: utf-8 -*-
 
 from c3s_sm.interface import C3SImg
 import os
 import numpy.testing as nptest
-from c3s_sm.grid import C3SLandGrid, C3SCellGrid
+from smecv_grid.grid import SMECV_Grid_v052
+import numpy as np
+import pytest
 
-# lat=48.125, lon=16.375
-def test_C33Ts_tcdr_combined_daily():
+def test_C3STs_tcdr_combined_daily():
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'TCDR', '060_dailyImages', 'combined', '2014',
                         'C3S-SOILMOISTURE-L3S-SSMV-COMBINED-DAILY-20140101000000-TCDR-v201801.0.0.nc'))
 
 
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
+    ds = C3SImg(file, mode='r', parameters=None, flatten=False, fillval={'sm': np.nan})
     image= ds.read()
 
-    nptest.assert_almost_equal(image.data['sm'][167, 785], 0.34659, 4)
-    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-    #assert(file_meta['creator_name'] == 'Earth Observation Data Center (EODC)')
-
+    test_loc_lonlat = (16.375, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
 
+    nptest.assert_almost_equal(image.data['sm'][row, col], 0.34659, 4)
+    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
 
-def test_C33Ts_tcdr_active_monthly():
 
+def test_C3STs_tcdr_active_monthly():
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'TCDR', '061_monthlyImages', 'active',
                         'C3S-SOILMOISTURE-L3S-SSMS-ACTIVE-MONTHLY-20140101000000-TCDR-v201801.0.0.nc'))
 
+    ds = C3SImg(file, mode='r', parameters='sm', flatten=False, fillval=None,
+                subgrid=SMECV_Grid_v052(None).subgrid_from_bbox(-181,-91, 181,91))
 
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
     image = ds.read()
+    
+    test_loc_lonlat = (16.375, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
 
-    nptest.assert_almost_equal(image.data['sm'][167, 785], 47.69982, 4)
+    assert image.data['sm'].shape == (720,1440)
+    nptest.assert_almost_equal(image.data['sm'][row, col], 47.69982, 4)
     assert(image.metadata['sm']['_FillValue'] == -9999.)
+    assert image.data['sm'].min() == image.metadata['sm']['_FillValue']
     assert(image.metadata['sm']['long_name'] == 'Percent of Saturation Soil Moisture')
-    #assert(file_meta['creator_name'] == 'Earth Observation Data Center (EODC)')
 
 
-def test_C33Ts_tcdr_passive_decadal():
+def test_C3STs_tcdr_passive_decadal():
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'TCDR', '062_dekadalImages', 'passive',
                         'C3S-SOILMOISTURE-L3S-SSMV-PASSIVE-DEKADAL-20140101000000-TCDR-v201801.0.0.nc'))
 
-
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
+    ds = C3SImg(file, mode='r', flatten=False, fillval={'nobs': -1, 'sm': np.nan},
+                subgrid=SMECV_Grid_v052('landcover_class', subset_value=[10,11,60,70]).subgrid_from_bbox(-14, 30, 44, 73))
     image = ds.read()
 
-    nptest.assert_almost_equal(image['sm'][167, 784], 0.50875, 4)
-    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-    #assert(image.metadata['creator_name'] == 'Earth Observation Data Center (EODC)')
+    test_loc_lonlat = (16.125, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
 
-################################################################################
+    assert image['nobs'].min() == -1
+    assert np.any(np.isnan(image['sm']))
+    nptest.assert_almost_equal(image['sm'][row, col], 0.50875, 4)
+    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
 
-def test_C33Ts_icdr_combined_daily():
+def test_C3STs_icdr_combined_daily():
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'ICDR', '060_dailyImages', 'combined', '2017',
                         'C3S-SOILMOISTURE-L3S-SSMV-COMBINED-DAILY-20170701000000-ICDR-v201706.0.0.nc'))
 
 
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
+    ds = C3SImg(file, mode='r', parameters=['sm', 't0'], flatten=False, subgrid=SMECV_Grid_v052('land'))
     image = ds.read()
 
-    nptest.assert_almost_equal(image.data['sm'][167, 785], 0.14548, 4)
-    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-    #assert(image['creator_name'] == 'Earth Observation Data Center (EODC)')
-
+    test_loc_lonlat = (16.375, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
 
+    nptest.assert_almost_equal(image.data['sm'][row, col], 0.14548, 4)
+    assert(image.metadata['t0']['long_name'] == 'Observation Timestamp')
 
-def test_C33Ts_icdr_active_monthly():
+def test_C3STs_icdr_active_monthly():
 
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'ICDR', '061_monthlyImages', 'active',
                         'C3S-SOILMOISTURE-L3S-SSMS-ACTIVE-MONTHLY-20170701000000-ICDR-v201706.0.0.nc'))
 
-
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
+    ds = C3SImg(file, mode='r', parameters=['sm', 'sensor'], flatten=False, fillval=-1)
     image = ds.read()
 
-    nptest.assert_almost_equal(image.data['sm'][167, 785], 65.00162, 4)
+    assert image['sensor'].min() == image['sm'].min() == -1
+    test_loc_lonlat = (16.375, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
+    nptest.assert_almost_equal(image.data['sm'][row, col], 65.00162, 4)
     assert(image.metadata['sm']['_FillValue'] == -9999.)
     assert(image.metadata['sm']['long_name'] == 'Percent of Saturation Soil Moisture')
-    #assert(file_meta['creator_name'] == 'Earth Observation Data Center (EODC)')
 
 
-def test_C33Ts_icdr_passive_decadal():
+def test_C3STs_icdr_passive_decadal():
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'ICDR', '062_dekadalImages', 'passive',
                         'C3S-SOILMOISTURE-L3S-SSMV-PASSIVE-DEKADAL-20170701000000-ICDR-v201706.0.0.nc'))
 
-
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=False)
+    ds = C3SImg(file, mode='r', parameters='sm', flatten=False, fillval=np.nan)
     image = ds.read()
 
-    nptest.assert_almost_equal(image.data['sm'][167, 785], 0.21000, 4)
+    test_loc_lonlat = (16.375, 48.125)
+    row, col = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))
+
+    nptest.assert_almost_equal(image.data['sm'][row, col], 0.21000, 4)
     assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-    #assert(image.metadata['creator_name'] == 'Earth Observation Data Center (EODC)')
 
+@pytest.mark.parametrize("subgrid,",
+                         [(SMECV_Grid_v052(None)),
+                          (SMECV_Grid_v052('land')),
+                          (SMECV_Grid_v052('landcover_class', subset_value=[10,11])),
+                          (SMECV_Grid_v052('land').subgrid_from_bbox(74, 13, 78, 15))])
+def test_1Dreading(subgrid):
+    # Test 1D reading with and without land grid, and if the results are the same
 
-def test_1Dreading():
-    ''' Test 1D reading with and without land grid, and if the results are the same'''
     file = os.path.join(os.path.join(os.path.dirname(__file__),
                         'c3s_sm-test-data', 'img', 'ICDR', '060_dailyImages', 'combined', '2017',
                         'C3S-SOILMOISTURE-L3S-SSMV-COMBINED-DAILY-20170701000000-ICDR-v201706.0.0.nc'))
 
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=True)
-    image = ds.read()
-
-    assert ds.grid.find_nearest_gpi(75.625, 14.625) == (602942, 0)
-    ref_sm = image.data['sm'][434462]
-    ref_lat = image.lat[434462]
-    ref_lon = image.lon[434462]
-
-    assert ref_lat == 14.625
-    assert ref_lon == 75.625
-    nptest.assert_almost_equal(ref_sm, 0.360762, 5)
-    assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-
-    land_grid = C3SLandGrid()
-
-    ds = C3SImg(file, mode='r', parameters='sm', array_1D=True, subgrid=land_grid)
+    ds = C3SImg(file, mode='r', parameters=None, flatten=True, subgrid=subgrid)
     image = ds.read()
 
-    assert ds.grid.find_nearest_gpi(75.625, 14.625) == (602942, 0)
+    test_loc_lonlat = (75.625, 14.625)
+    idx = np.where((image.lon==test_loc_lonlat[0]) & (image.lat==test_loc_lonlat[1]))[0]
 
-    sm = image.data['sm'][177048]
-    lat = image.lat[177048]
-    lon = image.lon[177048]
-
-    assert ref_lat == lat
-    assert ref_lon == lon
-    nptest.assert_almost_equal(ref_sm, sm, 5)
+    assert ds.subgrid.find_nearest_gpi(*test_loc_lonlat) == (602942, 0)
+    ref_sm = image.data['sm'][idx]
+    ref_lat = image.lat[idx]
+    ref_lon = image.lon[idx]
 
+    assert ref_lat == test_loc_lonlat[1]
+    assert ref_lon == test_loc_lonlat[0]
+    nptest.assert_almost_equal(ref_sm, 0.360762, 5)
     assert(image.metadata['sm']['long_name'] == 'Volumetric Soil Moisture')
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-    test_1Dreading()
-    test_C33Ts_tcdr_combined_daily()
-    test_C33Ts_tcdr_active_monthly()
-    test_C33Ts_tcdr_passive_decadal()
-
-    test_C33Ts_icdr_combined_daily()
-    test_C33Ts_icdr_active_monthly()
-    test_C33Ts_icdr_passive_decadal()
```

### Comparing `c3s_sm-0.1.2/use_case/C3S_v201812_COMBINED_sample.csv` & `c3s_sm-0.2.0/docs/use_case/C3S_v201812_COMBINED_sample.csv`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/use_case/Timeseries_locations.png` & `c3s_sm-0.2.0/docs/use_case/Timeseries_locations.png`

 * *Files identical despite different names*

### Comparing `c3s_sm-0.1.2/use_case/c3s_sm_monthly_anomalies.ipynb` & `c3s_sm-0.2.0/docs/use_case/c3s_sm_monthly_anomalies.ipynb`

 * *Files identical despite different names*

