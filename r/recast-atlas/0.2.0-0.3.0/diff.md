# Comparing `tmp/recast_atlas-0.2.0.tar.gz` & `tmp/recast_atlas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recast_atlas-0.2.0.tar", last modified: Tue Jun 20 22:48:25 2023, max compression
+gzip compressed data, was "recast_atlas-0.3.0.tar", last modified: Wed Jul  5 05:38:54 2023, max compression
```

## Comparing `recast_atlas-0.2.0.tar` & `recast_atlas-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.992233 recast_atlas-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recast_atlas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 22:48:24.000000 recast_atlas-0.2.0/src/recast_atlas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/backends/reana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.996233 recast_atlas-0.2.0/src/recastatlas/data/catalogue/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/busyboxtest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_checkmate1.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_checkmate2.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_rome.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/expect_script.sh
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/getkrb_reana.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:24.992233 recast_atlas-0.2.0/src/recastatlas/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/recast.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/steps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/specs/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/resultsextraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/software.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/subcommands/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/src/recastatlas/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/test/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/src/recastatlas/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 22:48:25.000233 recast_atlas-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 22:48:07.000000 recast_atlas-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.384783 recast_atlas-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-05 05:38:54.384783 recast_atlas-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-05 05:38:54.384783 recast_atlas-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.376783 recast_atlas-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.376783 recast_atlas-0.3.0/src/recast_atlas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 05:38:54.000000 recast_atlas-0.3.0/src/recast_atlas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/backends/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/backends/reana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/data/catalogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/catalogue/busyboxtest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/catalogue/examples_checkmate1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/catalogue/examples_checkmate2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/catalogue/examples_rome.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/expect_script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/getkrb_reana.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.376783 recast_atlas-0.3.0/src/recastatlas/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/recast.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/specs/steps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/specs/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/resultsextraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/subcommands/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.380783 recast_atlas-0.3.0/src/recastatlas/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/test/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/src/recastatlas/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 05:38:54.384783 recast_atlas-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 05:38:36.000000 recast_atlas-0.3.0/tests/test_cli.py
```

### Comparing `recast_atlas-0.2.0/LICENSE` & `recast_atlas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/PKG-INFO` & `recast_atlas-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: recast_atlas
-Version: 0.2.0
+Version: 0.3.0
 Summary: RECAST for ATLAS at the LHC
 Home-page: https://github.com/recast-hep/recast-atlas
 Author: Lukas Heinrich
 Author-email: lukas.heinrich@cern.ch
 License: Apache
 Project-URL: Documentation, https://github.com/recast-hep/recast-atlas
 Project-URL: Source Code, https://github.com/recast-hep/recast-atlas
 Project-URL: Issue Tracker, https://github.com/recast-hep/recast-atlas/issues
 Keywords: physics recast atlas
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: local
 Provides-Extra: kubernetes
 Provides-Extra: reana
 License-File: LICENSE
```

### Comparing `recast_atlas-0.2.0/README.md` & `recast_atlas-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/setup.cfg` & `recast_atlas-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [metadata]
 name = recast_atlas
-version = 0.2.0
+version = 0.3.0
 description = RECAST for ATLAS at the LHC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/recast-hep/recast-atlas
 author = Lukas Heinrich
 author_email = lukas.heinrich@cern.ch
 license = Apache
 license_file = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Physics
 keywords = physics recast atlas
 project_urls = 
 	Documentation = https://github.com/recast-hep/recast-atlas
 	Source Code = https://github.com/recast-hep/recast-atlas
@@ -31,15 +32,15 @@
 [options]
 packages = find:
 install_requires = 
 	click>=7.0  # for console scripts
 	jsonschema>=3.0.0
 	pyyaml>=5.1  # for parsing CLI options
 	yadage-schemas>=0.10.7  # c.f. https://github.com/yadage/yadage-schemas/issues/35
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
```

### Comparing `recast_atlas-0.2.0/src/recast_atlas.egg-info/PKG-INFO` & `recast_atlas-0.3.0/src/recast_atlas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: recast-atlas
-Version: 0.2.0
+Version: 0.3.0
 Summary: RECAST for ATLAS at the LHC
 Home-page: https://github.com/recast-hep/recast-atlas
 Author: Lukas Heinrich
 Author-email: lukas.heinrich@cern.ch
 License: Apache
 Project-URL: Documentation, https://github.com/recast-hep/recast-atlas
 Project-URL: Source Code, https://github.com/recast-hep/recast-atlas
 Project-URL: Issue Tracker, https://github.com/recast-hep/recast-atlas/issues
 Keywords: physics recast atlas
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: local
 Provides-Extra: kubernetes
 Provides-Extra: reana
 License-File: LICENSE
```

### Comparing `recast_atlas-0.2.0/src/recast_atlas.egg-info/SOURCES.txt` & `recast_atlas-0.3.0/src/recast_atlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/backends/__init__.py` & `recast_atlas-0.3.0/src/recastatlas/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/backends/docker.py` & `recast_atlas-0.3.0/src/recastatlas/backends/docker.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/backends/kubernetes.py` & `recast_atlas-0.3.0/src/recastatlas/backends/kubernetes.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/backends/local.py` & `recast_atlas-0.3.0/src/recastatlas/backends/local.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/backends/reana.py` & `recast_atlas-0.3.0/src/recastatlas/backends/reana.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/cli.py` & `recast_atlas-0.3.0/src/recastatlas/cli.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/config.py` & `recast_atlas-0.3.0/src/recastatlas/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             },
             "docker": {
                 "metadata": {"short_description": "runs with containerized tools"},
                 "fromstring": conf_from_env(
                     "RECAST_DOCKER_BACKENDSTRING", "multiproc:auto"
                 ),
                 "image": conf_from_env(
-                    "RECAST_DOCKER_IMAGE", "recast/recastatlas:v0.2.0"
+                    "RECAST_DOCKER_IMAGE", "recast/recastatlas:v0.3.0"
                 ),
                 "cvmfs": {"location": "/cvmfs", "propagation": "rprivate"},
                 "reg": {
                     "user": conf_from_env("RECAST_REGISTRY_USERNAME"),
                     "pass": conf_from_env("RECAST_REGISTRY_PASSWORD"),
                     "host": conf_from_env("RECAST_REGISTRY_HOST"),
                 },
```

### Comparing `recast_atlas-0.2.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml` & `recast_atlas-0.3.0/src/recastatlas/data/catalogue/atlas_atlas_conf_2018_041.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: atlas/atlas-conf-2018-041
 
 metadata:
   short_description: ATLAS MBJ
 
 spec:
-  toplevel: gitlab-cern:recast-atlas/susy/ATLAS-CONF-2018-041:specs
+  toplevel: gitlab-cern:recast-atlas/susy/ATLAS-CONF-2018-041@master:specs
   workflow: workflow.yml
 
 example_inputs:
   default:
     dataopts:
       archivematch: '*/examples/inputdata/'
       inputarchive: https://gitlab.cern.ch/api/v4/projects/recast-atlas%2Fsusy%2FATLAS-CONF-2018-041/repository/archive.zip?sha=master
```

### Comparing `recast_atlas-0.2.0/src/recastatlas/data/catalogue/examples_rome.yml` & `recast_atlas-0.3.0/src/recastatlas/data/catalogue/examples_rome.yml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 metadata:
   author: Lukas Heinrich
   input requirements: ''
   short_description: Example from ATLAS Exotics Rome Workshop 2018
 
 spec:
-  toplevel: github:reanahub/reana-demo-atlas-recast
+  toplevel: github:reanahub/reana-demo-atlas-recast@master
   workflow: workflow/workflow.yml
 
 example_inputs:
   default:
     initdata:
       did: 404958
       dxaod_file: https://recastwww.web.cern.ch/recastwww/data/reana-recast-demo/mc15_13TeV.123456.cap_recast_demo_signal_one.root
```

### Comparing `recast_atlas-0.2.0/src/recastatlas/data/expect_script.sh` & `recast_atlas-0.3.0/src/recastatlas/data/expect_script.sh`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/data/templates/helloworld/recast.yml` & `recast_atlas-0.3.0/src/recastatlas/data/templates/helloworld/recast.yml`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/resultsextraction.py` & `recast_atlas-0.3.0/src/recastatlas/resultsextraction.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/auth.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/auth.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/backends.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/backends.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/catalogue.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/catalogue.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/run.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/run.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/software.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/software.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/subcommands/testing.py` & `recast_atlas-0.3.0/src/recastatlas/subcommands/testing.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/src/recastatlas/testing.py` & `recast_atlas-0.3.0/src/recastatlas/testing.py`

 * *Files identical despite different names*

### Comparing `recast_atlas-0.2.0/tests/test_cli.py` & `recast_atlas-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

