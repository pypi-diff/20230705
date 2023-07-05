# Comparing `tmp/pythermalcomfort-2.8.0.tar.gz` & `tmp/pythermalcomfort-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythermalcomfort-2.8.0.tar", last modified: Mon Jul  3 01:32:48 2023, max compression
+gzip compressed data, was "pythermalcomfort-2.8.1.tar", last modified: Wed Jul  5 01:41:46 2023, max compression
```

## Comparing `pythermalcomfort-2.8.0.tar` & `pythermalcomfort-2.8.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/appveyor-with-compiler.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/templates/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/ci/templates/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/contact_us.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/reference/pythermalcomfort.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_adaptive_ASHRAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_adaptive_EN.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_phs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_pmv_ppd.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_set_tmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/examples/calc_utci.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.810787 pythermalcomfort-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/src/pythermalcomfort/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/construction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/thermoregulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   171792 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/optimized_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/shared_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/src/pythermalcomfort/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.814787 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 01:32:48.000000 pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:32:48.818786 pythermalcomfort-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_jos3.py
--rw-r--r--   0 runner    (1001) docker     (123)    44405 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tests/test_pythermalcomfort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-03 01:32:39.000000 pythermalcomfort-2.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.823970 pythermalcomfort-2.8.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/ci/appveyor-with-compiler.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.823970 pythermalcomfort-2.8.1/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/ci/templates/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/ci/templates/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.823970 pythermalcomfort-2.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/contact_us.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.823970 pythermalcomfort-2.8.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/reference/pythermalcomfort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_adaptive_ASHRAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_adaptive_EN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_phs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_pmv_ppd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_set_tmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/examples/calc_utci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.823970 pythermalcomfort-2.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/src/pythermalcomfort/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/thermoregulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171889 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/optimized_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/shared_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/src/pythermalcomfort/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 01:41:46.000000 pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:41:46.827970 pythermalcomfort-2.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/tests/test_jos3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44549 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/tests/test_pythermalcomfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-05 01:41:37.000000 pythermalcomfort-2.8.1/tox.ini
```

### Comparing `pythermalcomfort-2.8.0/.appveyor.yml` & `pythermalcomfort-2.8.1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/.cookiecutterrc` & `pythermalcomfort-2.8.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/.readthedocs.yml` & `pythermalcomfort-2.8.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/.travis.yml` & `pythermalcomfort-2.8.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/AUTHORS.rst` & `pythermalcomfort-2.8.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/CHANGELOG.rst` & `pythermalcomfort-2.8.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/CONTRIBUTING.rst` & `pythermalcomfort-2.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/LICENSE` & `pythermalcomfort-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/PKG-INFO` & `pythermalcomfort-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythermalcomfort
-Version: 2.8.0
+Version: 2.8.1
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.8.0/README.rst` & `pythermalcomfort-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/ci/appveyor-with-compiler.cmd` & `pythermalcomfort-2.8.1/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/ci/bootstrap.py` & `pythermalcomfort-2.8.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/ci/templates/.appveyor.yml` & `pythermalcomfort-2.8.1/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/ci/templates/.travis.yml` & `pythermalcomfort-2.8.1/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/docs/conf.py` & `pythermalcomfort-2.8.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "pythermalcomfort"
 year = "2019"
 author = "Federico Tartarini"
 copyright = "{0}, {1}".format(year, author)
-version = release = "2.8.0"
+version = release = "2.8.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": (
         "https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort/issues/%s",
         "#",
```

### Comparing `pythermalcomfort-2.8.0/docs/contact_us.rst` & `pythermalcomfort-2.8.1/docs/contact_us.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/docs/reference/pythermalcomfort.rst` & `pythermalcomfort-2.8.1/docs/reference/pythermalcomfort.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/docs/usage.rst` & `pythermalcomfort-2.8.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_adaptive_ASHRAE.py` & `pythermalcomfort-2.8.1/examples/calc_adaptive_ASHRAE.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_adaptive_EN.py` & `pythermalcomfort-2.8.1/examples/calc_adaptive_EN.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_jos3.py` & `pythermalcomfort-2.8.1/examples/calc_jos3.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_phs.py` & `pythermalcomfort-2.8.1/examples/calc_phs.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_pmv_ppd.py` & `pythermalcomfort-2.8.1/examples/calc_pmv_ppd.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/examples/calc_utci.py` & `pythermalcomfort-2.8.1/examples/calc_utci.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/setup.cfg` & `pythermalcomfort-2.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/setup.py` & `pythermalcomfort-2.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="pythermalcomfort",
-    version="2.8.0",
+    version="2.8.1",
     license="MIT",
     description=(
         "Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET,"
         " adaptive) and convert physical variables. Please cite us if you use this"
         " package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python"
         " package for thermal comfort research. SoftwareX 12, 100578."
         " https://doi.org/10.1016/j.softx.2020.100578"
```

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/cli.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/cli.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/construction.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/construction.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/matrix.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/matrix.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/parameters.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/parameters.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/thermoregulation.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/thermoregulation.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/jos3_functions/utilities.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/jos3_functions/utilities.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/models.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,17 @@
     except ValueError:
         ce = 0
 
     warnings.simplefilter("always")
 
     if ce == 0:
         warnings.warn(
-            "The cooling effect could not be calculated, assuming ce = 0", UserWarning
+            "Assuming cooling effect = 0 since it could not be calculated for this set"
+            f" of inputs {tdb=}, {tr=}, {rh=}, {vr=}, {clo=}, {met=}",
+            UserWarning,
         )
 
     if units.lower() == "ip":
         ce = ce / 1.8 * 3.28
 
     return round(ce, 2)
```

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/optimized_functions.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/optimized_functions.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/psychrometrics.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort/utilities.py` & `pythermalcomfort-2.8.1/src/pythermalcomfort/utilities.py`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/PKG-INFO` & `pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythermalcomfort
-Version: 2.8.0
+Version: 2.8.1
 Summary: Package to calculate several thermal comfort indices (e.g. PMV, PPD, SET, adaptive) and convert physical variables. Please cite us if you use this package: Tartarini, F., Schiavon, S., 2020. pythermalcomfort: A Python package for thermal comfort research. SoftwareX 12, 100578. https://doi.org/10.1016/j.softx.2020.100578
 Home-page: https://github.com/CenterForTheBuiltEnvironment/pythermalcomfort
 Author: Federico Tartarini
 Author-email: cbecomforttool@gmail.com
 License: MIT
 Project-URL: Documentation, https://pythermalcomfort.readthedocs.io/
 Project-URL: Changelog, https://pythermalcomfort.readthedocs.io/en/latest/changelog.html
```

### Comparing `pythermalcomfort-2.8.0/src/pythermalcomfort.egg-info/SOURCES.txt` & `pythermalcomfort-2.8.1/src/pythermalcomfort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythermalcomfort-2.8.0/tests/test_models.py` & `pythermalcomfort-2.8.1/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,14 +626,17 @@
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=80, met=1, clo=0.6)) == 2.06
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=20, met=1, clo=0.6)) == 2.29
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=60, met=1.3, clo=0.6)) == 2.84
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=60, met=1.6, clo=0.6)) == 3.5
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=60, met=1, clo=0.3)) == 2.41
     assert (cooling_effect(tdb=25, tr=25, vr=0.5, rh=60, met=1, clo=1)) == 2.05
 
+    # test what happens when the cooling effect cannot be calculated
+    assert (cooling_effect(tdb=0, tr=80, vr=5, rh=60, met=3, clo=1)) == 0
+
     assert (
         cooling_effect(tdb=77, tr=77, vr=1.64, rh=50, met=1, clo=0.6, units="IP")
     ) == 3.95
 
 
 def test_running_mean_outdoor_temperature():
     assert (running_mean_outdoor_temperature([20, 20], alpha=0.7)) == 20
```

### Comparing `pythermalcomfort-2.8.0/tox.ini` & `pythermalcomfort-2.8.1/tox.ini`

 * *Files identical despite different names*

