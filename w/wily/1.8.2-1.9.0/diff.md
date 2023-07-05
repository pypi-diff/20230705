# Comparing `tmp/wily-1.8.2.tar.gz` & `tmp/wily-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wily-1.8.2.tar", last modified: Fri Dec 21 08:54:01 2018, max compression
+gzip compressed data, was "wily-1.9.0.tar", last modified: Fri Dec 28 02:31:53 2018, max compression
```

## Comparing `wily-1.8.2.tar` & `wily-1.9.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0      224 2018-11-27 06:18:09.620333 wily-1.8.2/.coveragerc
--rw-r--r--   0        0        0     1300 2018-11-27 06:18:09.638743 wily-1.8.2/.gitignore
--rw-r--r--   0        0        0      298 2018-11-27 06:18:09.642827 wily-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      182 2018-11-27 06:18:09.643253 wily-1.8.2/.travis.yml
--rw-r--r--   0        0        0     4233 2018-11-27 06:18:09.657254 wily-1.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     5128 2018-12-21 08:53:15.314852 wily-1.8.2/HISTORY.md
--rw-r--r--   0        0        0    11357 2018-10-11 22:13:45.000000 wily-1.8.2/LICENSE
--rw-r--r--   0        0        0     8835 2018-12-21 08:50:22.671418 wily-1.8.2/README.md
--rw-r--r--   0        0        0     2002 2018-12-21 08:50:22.671670 wily-1.8.2/azure-pipelines.yml
--rw-r--r--   0        0        0      584 2018-11-07 04:11:13.982545 wily-1.8.2/docs/Makefile
--rw-r--r--   0        0        0      791 2018-11-07 04:11:13.983789 wily-1.8.2/docs/make.bat
--rw-r--r--   0        0        0       92 2018-11-27 06:18:09.676544 wily-1.8.2/docs/requirements_docs.txt
--rw-r--r--   0        0        0   243599 2018-11-30 04:24:26.222473 wily-1.8.2/docs/source/_static/custom_x_axis_graph.png
--rw-r--r--   0        0        0   112266 2018-11-27 06:18:09.685573 wily-1.8.2/docs/source/_static/graph.png
--rw-r--r--   0        0        0    33829 2018-11-07 04:23:19.605479 wily-1.8.2/docs/source/_static/logo.png
--rw-r--r--   0        0        0   190371 2018-11-30 04:24:26.226118 wily-1.8.2/docs/source/_static/single_metric_graph.png
--rw-r--r--   0        0        0   215470 2018-11-30 04:24:26.229449 wily-1.8.2/docs/source/_static/two_metric_graph.png
--rw-r--r--   0        0        0    54703 2018-11-27 06:18:09.693650 wily-1.8.2/docs/source/_static/wily_build.png
--rw-r--r--   0        0        0   107261 2018-11-30 04:24:26.232154 wily-1.8.2/docs/source/_static/wily_diff.png
--rw-r--r--   0        0        0   158080 2018-11-27 06:18:09.696909 wily-1.8.2/docs/source/_static/wily_help.png
--rw-r--r--   0        0        0   289668 2018-11-30 04:24:26.237493 wily-1.8.2/docs/source/_static/wily_index.png
--rw-r--r--   0        0        0   229305 2018-11-27 06:18:09.700990 wily-1.8.2/docs/source/_static/wily_report.png
--rw-r--r--   0        0        0     2314 2018-11-30 04:25:17.366513 wily-1.8.2/docs/source/commands/build.rst
--rw-r--r--   0        0        0     1508 2018-11-30 04:24:26.238813 wily-1.8.2/docs/source/commands/diff.rst
--rw-r--r--   0        0        0     1665 2018-11-30 04:24:26.239281 wily-1.8.2/docs/source/commands/graph.rst
--rw-r--r--   0        0        0      616 2018-11-30 04:24:26.239647 wily-1.8.2/docs/source/commands/index.rst
--rw-r--r--   0        0        0     1170 2018-11-30 04:43:55.552609 wily-1.8.2/docs/source/commands/report.rst
--rw-r--r--   0        0        0     5583 2018-11-27 06:18:09.708385 wily-1.8.2/docs/source/conf.py
--rw-r--r--   0        0        0     3084 2018-11-30 04:54:05.869289 wily-1.8.2/docs/source/index.rst
--rw-r--r--   0        0        0     1209 2018-11-27 06:23:46.399188 wily-1.8.2/pyproject.toml
--rw-r--r--   0        0        0       97 2018-11-27 06:18:09.721855 wily-1.8.2/readthedocs.yml
--rw-r--r--   0        0        0     2139 2018-12-18 20:59:21.274356 wily-1.8.2/test/conftest.py
--rw-r--r--   0        0        0     1831 2018-12-18 20:59:21.274882 wily-1.8.2/test/integration/test_all_operators.py
--rw-r--r--   0        0        0     4099 2018-11-30 04:24:26.241918 wily-1.8.2/test/integration/test_archiver.py
--rw-r--r--   0        0        0     7607 2018-12-18 21:59:52.016527 wily-1.8.2/test/integration/test_build.py
--rw-r--r--   0        0        0     4960 2018-11-30 04:24:26.243299 wily-1.8.2/test/integration/test_diff.py
--rw-r--r--   0        0        0     4590 2018-11-30 04:24:26.243990 wily-1.8.2/test/integration/test_graph.py
--rw-r--r--   0        0        0      740 2018-11-30 04:24:26.244601 wily-1.8.2/test/integration/test_index.py
--rw-r--r--   0        0        0     3331 2018-12-18 20:59:21.275592 wily-1.8.2/test/integration/test_report.py
--rw-r--r--   0        0        0     1025 2018-11-30 04:24:26.245383 wily-1.8.2/test/integration/test_state.py
--rw-r--r--   0        0        0      987 2018-11-30 04:24:26.245795 wily-1.8.2/test/integration/test_wily.py
--rw-r--r--   0        0        0     2435 2018-12-18 20:59:21.276004 wily-1.8.2/test/unit/test_archivers.py
--rw-r--r--   0        0        0     1390 2018-12-21 08:50:22.672756 wily-1.8.2/test/unit/test_build_unit.py
--rw-r--r--   0        0        0     5458 2018-12-18 20:59:21.276298 wily-1.8.2/test/unit/test_cache.py
--rw-r--r--   0        0        0    10987 2018-12-18 20:59:21.276732 wily-1.8.2/test/unit/test_cli.py
--rw-r--r--   0        0        0     1959 2018-11-30 04:24:26.247746 wily-1.8.2/test/unit/test_config.py
--rw-r--r--   0        0        0      740 2018-11-30 04:24:26.248126 wily-1.8.2/test/unit/test_operators.py
--rw-r--r--   0        0        0      788 2018-12-21 08:52:26.362629 wily-1.8.2/wily/__init__.py
--rw-r--r--   0        0        0     8637 2018-12-18 20:59:21.277470 wily-1.8.2/wily/__main__.py
--rw-r--r--   0        0        0     2174 2018-12-18 20:59:21.278689 wily-1.8.2/wily/archivers/__init__.py
--rw-r--r--   0        0        0     1714 2018-12-18 20:59:21.279208 wily-1.8.2/wily/archivers/filesystem.py
--rw-r--r--   0        0        0     4119 2018-12-18 20:59:21.279491 wily-1.8.2/wily/archivers/git.py
--rw-r--r--   0        0        0     7777 2018-12-18 20:59:21.279969 wily-1.8.2/wily/cache.py
--rw-r--r--   0        0        0       39 2018-11-27 06:18:09.771951 wily-1.8.2/wily/commands/__init__.py
--rw-r--r--   0        0        0     4926 2018-12-21 08:50:22.690350 wily-1.8.2/wily/commands/build.py
--rw-r--r--   0        0        0     4443 2018-12-18 20:59:21.280769 wily-1.8.2/wily/commands/diff.py
--rw-r--r--   0        0        0     3952 2018-11-30 04:24:26.251495 wily-1.8.2/wily/commands/graph.py
--rw-r--r--   0        0        0     1890 2018-11-30 04:24:26.251857 wily-1.8.2/wily/commands/index.py
--rw-r--r--   0        0        0      651 2018-12-18 20:59:21.281173 wily-1.8.2/wily/commands/list_metrics.py
--rw-r--r--   0        0        0     4662 2018-11-30 04:24:26.252797 wily-1.8.2/wily/commands/report.py
--rw-r--r--   0        0        0     3115 2018-11-30 04:24:26.253537 wily-1.8.2/wily/config.py
--rw-r--r--   0        0        0     4497 2018-12-19 01:42:57.688382 wily-1.8.2/wily/operators/__init__.py
--rw-r--r--   0        0        0     3513 2018-12-21 08:50:22.695710 wily-1.8.2/wily/operators/cyclomatic.py
--rw-r--r--   0        0        0     2949 2018-12-18 20:59:21.282144 wily-1.8.2/wily/operators/halstead.py
--rw-r--r--   0        0        0     2014 2018-12-21 08:50:22.696202 wily-1.8.2/wily/operators/maintainability.py
--rw-r--r--   0        0        0     1957 2018-12-18 20:59:21.282715 wily-1.8.2/wily/operators/raw.py
--rw-r--r--   0        0        0     6060 2018-12-18 20:59:21.283052 wily-1.8.2/wily/state.py
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 wily-1.8.2/setup.py
--rw-r--r--   0        0        0      168 1970-01-01 00:00:00.000000 wily-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      224 2018-12-14 07:10:36.507412 wily-1.9.0/.coveragerc
+-rw-r--r--   0        0        0     1300 2018-12-14 07:10:36.508266 wily-1.9.0/.gitignore
+-rw-r--r--   0        0        0      298 2018-12-14 07:10:36.508946 wily-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4233 2018-11-15 05:42:24.955193 wily-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5627 2018-12-28 02:26:41.369185 wily-1.9.0/HISTORY.md
+-rw-r--r--   0        0        0    11357 2018-10-15 03:32:44.387290 wily-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8797 2018-12-28 01:46:57.202060 wily-1.9.0/README.md
+-rw-r--r--   0        0        0     1999 2018-12-28 02:27:05.672990 wily-1.9.0/azure-pipelines.yml
+-rw-r--r--   0        0        0      584 2018-11-07 20:59:21.530906 wily-1.9.0/docs/Makefile
+-rw-r--r--   0        0        0      791 2018-11-07 20:59:21.531079 wily-1.9.0/docs/make.bat
+-rw-r--r--   0        0        0       92 2018-11-14 23:16:54.867081 wily-1.9.0/docs/requirements_docs.txt
+-rw-r--r--   0        0        0   243599 2018-12-14 07:10:36.513877 wily-1.9.0/docs/source/_static/custom_x_axis_graph.png
+-rw-r--r--   0        0        0   112266 2018-11-14 23:16:54.868281 wily-1.9.0/docs/source/_static/graph.png
+-rw-r--r--   0        0        0    33829 2018-11-07 20:59:21.531918 wily-1.9.0/docs/source/_static/logo.png
+-rw-r--r--   0        0        0   190371 2018-12-14 07:10:36.515712 wily-1.9.0/docs/source/_static/single_metric_graph.png
+-rw-r--r--   0        0        0   215470 2018-12-14 07:10:36.517577 wily-1.9.0/docs/source/_static/two_metric_graph.png
+-rw-r--r--   0        0        0    54703 2018-11-14 23:16:54.868884 wily-1.9.0/docs/source/_static/wily_build.png
+-rw-r--r--   0        0        0   107261 2018-12-14 07:10:36.518774 wily-1.9.0/docs/source/_static/wily_diff.png
+-rw-r--r--   0        0        0   158080 2018-11-14 23:16:54.870474 wily-1.9.0/docs/source/_static/wily_help.png
+-rw-r--r--   0        0        0   289668 2018-12-14 07:10:36.521498 wily-1.9.0/docs/source/_static/wily_index.png
+-rw-r--r--   0        0        0   229305 2018-11-14 23:16:54.872553 wily-1.9.0/docs/source/_static/wily_report.png
+-rw-r--r--   0        0        0     1888 2018-12-28 02:28:47.246660 wily-1.9.0/docs/source/commands/build.rst
+-rw-r--r--   0        0        0     1508 2018-12-14 07:10:36.522222 wily-1.9.0/docs/source/commands/diff.rst
+-rw-r--r--   0        0        0     1665 2018-12-14 07:10:36.522363 wily-1.9.0/docs/source/commands/graph.rst
+-rw-r--r--   0        0        0      616 2018-12-14 07:10:36.522529 wily-1.9.0/docs/source/commands/index.rst
+-rw-r--r--   0        0        0     1170 2018-12-14 07:10:36.522677 wily-1.9.0/docs/source/commands/report.rst
+-rw-r--r--   0        0        0     5583 2018-11-14 23:16:54.872938 wily-1.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0     3084 2018-12-14 07:10:36.523013 wily-1.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1209 2018-12-14 07:10:36.523593 wily-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       97 2018-11-08 21:32:53.633736 wily-1.9.0/readthedocs.yml
+-rw-r--r--   0        0        0     2269 2018-12-28 02:26:41.370723 wily-1.9.0/test/conftest.py
+-rw-r--r--   0        0        0     1875 2018-12-28 01:46:57.203701 wily-1.9.0/test/integration/test_all_operators.py
+-rw-r--r--   0        0        0     2690 2018-12-28 02:26:41.371271 wily-1.9.0/test/integration/test_archiver.py
+-rw-r--r--   0        0        0     7382 2018-12-28 02:26:41.372180 wily-1.9.0/test/integration/test_build.py
+-rw-r--r--   0        0        0     4954 2018-12-28 01:46:57.205361 wily-1.9.0/test/integration/test_diff.py
+-rw-r--r--   0        0        0     4680 2018-12-28 02:26:41.372881 wily-1.9.0/test/integration/test_graph.py
+-rw-r--r--   0        0        0      775 2018-12-28 02:26:41.373523 wily-1.9.0/test/integration/test_index.py
+-rw-r--r--   0        0        0     3313 2018-12-28 02:26:41.374226 wily-1.9.0/test/integration/test_report.py
+-rw-r--r--   0        0        0      854 2018-12-28 02:26:41.374891 wily-1.9.0/test/integration/test_state.py
+-rw-r--r--   0        0        0      987 2018-12-14 07:10:36.527677 wily-1.9.0/test/integration/test_wily.py
+-rw-r--r--   0        0        0     2435 2018-12-14 07:10:36.529462 wily-1.9.0/test/unit/test_archivers.py
+-rw-r--r--   0        0        0     1390 2018-12-20 10:50:09.507239 wily-1.9.0/test/unit/test_build_unit.py
+-rw-r--r--   0        0        0     5676 2018-12-28 01:46:57.207104 wily-1.9.0/test/unit/test_cache.py
+-rw-r--r--   0        0        0    10987 2018-12-14 07:10:36.531095 wily-1.9.0/test/unit/test_cli.py
+-rw-r--r--   0        0        0     1959 2018-12-28 01:46:57.207570 wily-1.9.0/test/unit/test_config.py
+-rw-r--r--   0        0        0     1282 2018-12-28 01:46:57.207944 wily-1.9.0/test/unit/test_cyclomatic.py
+-rw-r--r--   0        0        0      740 2018-12-14 07:10:36.533327 wily-1.9.0/test/unit/test_operators.py
+-rw-r--r--   0        0        0      788 2018-12-28 02:27:36.853261 wily-1.9.0/wily/__init__.py
+-rw-r--r--   0        0        0     8762 2018-12-28 02:26:41.376226 wily-1.9.0/wily/__main__.py
+-rw-r--r--   0        0        0     2174 2018-12-14 07:10:36.535589 wily-1.9.0/wily/archivers/__init__.py
+-rw-r--r--   0        0        0     1684 2018-12-28 02:26:41.377671 wily-1.9.0/wily/archivers/filesystem.py
+-rw-r--r--   0        0        0     2928 2018-12-28 02:26:41.378381 wily-1.9.0/wily/archivers/git.py
+-rw-r--r--   0        0        0     7765 2018-12-28 02:26:41.379329 wily-1.9.0/wily/cache.py
+-rw-r--r--   0        0        0       39 2018-12-14 07:10:36.537770 wily-1.9.0/wily/commands/__init__.py
+-rw-r--r--   0        0        0     4926 2018-12-20 10:50:09.508766 wily-1.9.0/wily/commands/build.py
+-rw-r--r--   0        0        0     4443 2018-12-14 07:10:36.538967 wily-1.9.0/wily/commands/diff.py
+-rw-r--r--   0        0        0     3952 2018-12-14 07:10:36.539359 wily-1.9.0/wily/commands/graph.py
+-rw-r--r--   0        0        0     1890 2018-12-14 07:10:36.539744 wily-1.9.0/wily/commands/index.py
+-rw-r--r--   0        0        0      651 2018-12-14 07:10:36.540638 wily-1.9.0/wily/commands/list_metrics.py
+-rw-r--r--   0        0        0     4662 2018-12-14 07:10:36.541127 wily-1.9.0/wily/commands/report.py
+-rw-r--r--   0        0        0     3986 2018-12-28 02:26:41.380097 wily-1.9.0/wily/config.py
+-rw-r--r--   0        0        0      400 2018-12-28 01:46:57.212126 wily-1.9.0/wily/decorators.py
+-rw-r--r--   0        0        0     4497 2018-12-18 19:32:14.313061 wily-1.9.0/wily/operators/__init__.py
+-rw-r--r--   0        0        0     3513 2018-12-20 10:50:25.880842 wily-1.9.0/wily/operators/cyclomatic.py
+-rw-r--r--   0        0        0     2949 2018-12-18 19:32:14.314215 wily-1.9.0/wily/operators/halstead.py
+-rw-r--r--   0        0        0     1943 2018-12-28 01:46:57.212698 wily-1.9.0/wily/operators/maintainability.py
+-rw-r--r--   0        0        0     1957 2018-12-18 19:32:14.315215 wily-1.9.0/wily/operators/raw.py
+-rw-r--r--   0        0        0     6141 2018-12-28 02:26:41.380739 wily-1.9.0/wily/state.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 wily-1.9.0/setup.py
+-rw-r--r--   0        0        0      168 1970-01-01 00:00:00.000000 wily-1.9.0/PKG-INFO
```

### Comparing `wily-1.8.2/.gitignore` & `wily-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/CONTRIBUTING.md` & `wily-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/HISTORY.md` & `wily-1.9.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 1.9.0 (master)
+
+* Wily now supports Windows! Full test suite works on Windows, Mac OS and Linux
+* Wily no longer puts the .wily cache in the target path, cache is now stored in the $HOME path. This means you no longer need to add .wily to .gitignore before running a build. Wily will isolate cache folders based on the absolute path
+* Added a --cache flag to specify the path to the cache for shared cache's
+* Added `-V` version flag and added current version to `--help` header @DahlitzFlorian
+
 ## 1.8.2 (21st December 2018)
 
 * [BUGFIX] Fixed an issue where the aggregation of the maintainability.rank metric would cause the build to crash if 2 files in the same directory had the same rank. 
 
 ## 1.8.1 (19th Decemember 2018)
 
 * [BUGFIX] Fixed an issue that occured if a target project contained a revision with invalid Python syntax, this is quite common, especially on long projects. The cyclomatic op would crash, also the aggregation logic would expect all metrics to be inside the output. This change avoids that and raises a warning instead.
```

### Comparing `wily-1.8.2/LICENSE` & `wily-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/README.md` & `wily-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ![wily](https://github.com/tonybaloney/wily/raw/master/docs/source/_static/logo.png)
 
 A command-line application for tracking, reporting on complexity of Python tests and applications.
 
-[![Build Status](https://travis-ci.com/tonybaloney/wily.svg?branch=master)](https://travis-ci.com/tonybaloney/wily)
 [![Build Status](https://dev.azure.com/AnthonyShaw/wily/_apis/build/status/tonybaloney.wily?branchName=master)](https://dev.azure.com/AnthonyShaw/wily/_build/latest?definitionId=1?branchName=master)
 [![codecov](https://codecov.io/gh/tonybaloney/wily/branch/master/graph/badge.svg)](https://codecov.io/gh/tonybaloney/wily) [![Documentation Status](https://readthedocs.org/projects/wily/badge/?version=latest)](https://wily.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/wily.svg)](https://badge.fury.io/py/wily) ![black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 
 ```
 wily [a]:
 quick to think of things, having a very good understanding of situations and possibilities, 
@@ -149,8 +148,13 @@
 ```
 
 You can also override the path to the configuration with the `--config` flag on the command-line.
 
 
 # Credits
 
+## Contributors
+
+- @wcooley (Wil Cooley)
+- @DahlitzFlorian (Florian Dahlitz)
+
 "cute animal doing dabbing" [Designed by Freepik](https://www.freepik.com/free-vector/cute-animal-doing-dabbing_2462508.htm)
```

### Comparing `wily-1.8.2/azure-pipelines.yml` & `wily-1.9.0/azure-pipelines.yml`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,30 @@
 
   steps:
   - task: UsePythonVersion@0
     inputs:
       versionSpec: '$(python.version)'
       architecture: 'x64'
 
-  - script: python -m pip install --upgrade pip && pip install flit mock && flit install
+  - script: |
+      python -m pip install --upgrade pip
+      pip install flit mock codecov pydocstyle pytest-cov
+      flit install
     displayName: 'Install dependencies'
 
   - script: |
       pip install pytest
-      pytest test --junitxml=junit/test-results.xml
+      python -m pytest test/ --junitxml=junit/test-results.xml --cov=wily/
+      codecov
     displayName: 'pytest'
+    env:
+      CODECOV_TOKEN: '48f9ff3a-6358-4607-aa5d-9cb7cada539c'
+  
+  - script: pydocstyle --ignore=D301,D212,D203 wily
+    displayName: 'pydocstyle'
 
   - task: PublishTestResults@2
     inputs:
       testResultsFiles: '**/test-results.xml'
       testRunTitle: 'Python $(python.version)'
     condition: succeededOrFailed()
 
@@ -68,22 +77,7 @@
     displayName: 'pytest'
 
   - task: PublishTestResults@2
     inputs:
       testResultsFiles: '**\test-results.xml'
       testRunTitle: 'Python $(python.version)'
     condition: succeededOrFailed()
-
-- job: 'Publish'
-  dependsOn: 'Test_Linux'
-  pool:
-    vmImage: 'Ubuntu-16.04'
-
-  steps:
-  - task: UsePythonVersion@0
-    inputs:
-      versionSpec: '3.x'
-      architecture: 'x64'
-
-  - script: flit build
-    displayName: 'Build sdist'
-
```

### Comparing `wily-1.8.2/docs/Makefile` & `wily-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/make.bat` & `wily-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/custom_x_axis_graph.png` & `wily-1.9.0/docs/source/_static/custom_x_axis_graph.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/graph.png` & `wily-1.9.0/docs/source/_static/graph.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/logo.png` & `wily-1.9.0/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/single_metric_graph.png` & `wily-1.9.0/docs/source/_static/single_metric_graph.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/two_metric_graph.png` & `wily-1.9.0/docs/source/_static/two_metric_graph.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/wily_build.png` & `wily-1.9.0/docs/source/_static/wily_build.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/wily_diff.png` & `wily-1.9.0/docs/source/_static/wily_diff.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/wily_help.png` & `wily-1.9.0/docs/source/_static/wily_help.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/wily_index.png` & `wily-1.9.0/docs/source/_static/wily_index.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/_static/wily_report.png` & `wily-1.9.0/docs/source/_static/wily_report.png`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/commands/build.rst` & `wily-1.9.0/docs/source/commands/build.rst`

 * *Files 7% similar despite different names*

```diff
@@ -47,22 +47,14 @@
 
 Updating the index
 ------------------
 
 To update the wily cache with any recent commits, simply re-run the ``wily build`` command and it will
 
 
-Ignoring `.wily`
-----------------
-
-Before you run the build command, it is strongly recommended the ``.wily/`` directory be ignored from the git index. This can be achieved by adding
-``.wily/`` to ``.gitignore`` and committing changes to ``.gitignore`` before running ``wily build``.
-
-Without this, you will receive an error when running wily build, this is to prevent uncomitted changes being lost when switching revisions.
-
 Dirty repositories
 ------------------
 
 If you run ``wily build`` with any uncommited files, wily will give an error to protect those files being lost, stash or commit them first.
 
 .. code-block:: none
```

### Comparing `wily-1.8.2/docs/source/commands/diff.rst` & `wily-1.9.0/docs/source/commands/diff.rst`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/commands/graph.rst` & `wily-1.9.0/docs/source/commands/graph.rst`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/commands/index.rst` & `wily-1.9.0/docs/source/commands/index.rst`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/commands/report.rst` & `wily-1.9.0/docs/source/commands/report.rst`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/conf.py` & `wily-1.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/docs/source/index.rst` & `wily-1.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/pyproject.toml` & `wily-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/test/conftest.py` & `wily-1.9.0/test/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pathlib
 from textwrap import dedent
-
+import os
+import shutil
+import tempfile
 import pytest
 from click.testing import CliRunner
 from git import Repo, Actor
 
 import wily.__main__ as main
 
 
@@ -54,18 +56,15 @@
             if b == 6:
                 return 'banana'
     """
 
     with open(testpath, "w") as test_txt:
         test_txt.write(dedent(second_test))
 
-    with open(tmppath / ".gitignore", "w") as test_txt:
-        test_txt.write(".wily/")
-
-    index.add([str(testpath), ".gitignore"])
+    index.add([str(testpath)])
     index.commit("remove line", author=author, committer=committer)
 
     return tmpdir
 
 
 @pytest.fixture
 def builddir(gitdir):
@@ -78,10 +77,19 @@
         main.cli, ["--debug", "--path", gitdir, "build", str(tmppath / "src")]
     )
     assert result1.exit_code == 0, result1.stdout
 
     result2 = runner.invoke(main.cli, ["--debug", "--path", gitdir, "index"])
     assert result2.exit_code == 0, result2.stdout
 
-    assert (tmppath / ".wily" / "git").exists()
-
     return gitdir
+
+
+@pytest.fixture(autouse=True)
+def cache_path(monkeypatch):
+    """
+    Configure wily cache and home path, clean up cache afterward
+    """
+    tmp = tempfile.mkdtemp()
+    monkeypatch.setenv("HOME", tmp)
+    yield tmp
+    shutil.rmtree(tmp)
```

### Comparing `wily-1.8.2/test/integration/test_all_operators.py` & `wily-1.9.0/test/integration/test_all_operators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 Parameterised tests for each operator (and some combinations).
 
 Build them and test out some of the metrics/commands work correctly.
 """
 import pytest
+import sys
 from click.testing import CliRunner
 import pathlib
 from textwrap import dedent
 
 import wily.__main__ as main
 
+_path = "src\\test.py" if sys.platform == "win32" else "src/test.py"
+
+
 operators = (
     "halstead",
     "cyclomatic",
     "maintainability",
     "raw",
     "halstead,cyclomatic",
     "maintainability,raw",
@@ -25,21 +29,19 @@
 def test_operator(operator, gitdir):
     runner = CliRunner()
     result = runner.invoke(
         main.cli, ["--debug", "--path", gitdir, "build", "src", "-o", operator]
     )
     assert result.exit_code == 0, result.stdout
 
-    result = runner.invoke(
-        main.cli, ["--debug", "--path", gitdir, "report", "src/test.py"]
-    )
+    result = runner.invoke(main.cli, ["--debug", "--path", gitdir, "report", _path])
     assert result.exit_code == 0, result.stdout
 
     result = runner.invoke(
-        main.cli, ["--debug", "--path", gitdir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", gitdir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
 
     complex_test = """
             import abc
             foo = 1
@@ -56,11 +58,11 @@
                               print(1)
             """
 
     with open(pathlib.Path(gitdir) / "src" / "test.py", "w") as test_py:
         test_py.write(dedent(complex_test))
 
     result = runner.invoke(
-        main.cli, ["--debug", "--path", gitdir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", gitdir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
```

### Comparing `wily-1.8.2/test/integration/test_archiver.py` & `wily-1.9.0/test/integration/test_archiver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,16 @@
 import pathlib
 
 import pytest
 from git import Repo, Actor
 
-from wily.archivers.git import (
-    GitArchiver,
-    WilyIgnoreGitRepositoryError,
-    DirtyGitRepositoryError,
-)
+from wily.archivers.git import GitArchiver, DirtyGitRepositoryError
 from wily.config import DEFAULT_CONFIG
 
 
-def test_gitignore_missing(tmpdir):
-    repo = Repo.init(path=tmpdir)
-    tmppath = pathlib.Path(tmpdir)
-
-    # Write a test file to the repo
-    with open(tmppath / ".gitignore", "w") as ignore:
-        ignore.write("*.py[co]\n")
-
-    index = repo.index
-    index.add([".gitignore"])
-
-    author = Actor("An author", "author@example.com")
-    committer = Actor("A committer", "committer@example.com")
-
-    index.commit("ignore python cache", author=author, committer=committer)
-
-    config = DEFAULT_CONFIG
-    config.path = tmpdir
-
-    with pytest.raises(WilyIgnoreGitRepositoryError):
-        archiver = GitArchiver(config)
-
-
-gitignore_combinations = (".wily/", ".wily", ".wily/*")
-
-
-@pytest.mark.parametrize("ignore", gitignore_combinations)
-def test_gitignore(tmpdir, ignore, **kwargs):
-    repo = Repo.init(path=tmpdir)
-    tmppath = pathlib.Path(tmpdir)
-
-    # Write a test file to the repo
-    with open(tmppath / ".gitignore", "w") as ignore_f:
-        ignore_f.write(ignore)
-
-    index = repo.index
-    index.add([".gitignore"])
-
-    author = Actor("An author", "author@example.com")
-    committer = Actor("A committer", "committer@example.com")
-
-    index.commit("ignore python cache", author=author, committer=committer)
-
-    config = DEFAULT_CONFIG
-    config.path = tmpdir
-
-    archiver = GitArchiver(config)
-    assert archiver.config == config
-
-
 def test_git_end_to_end(tmpdir):
     """
     Complete end-to-end test of the git integration
     """
     repo = Repo.init(path=tmpdir)
     tmppath = pathlib.Path(tmpdir)
```

### Comparing `wily-1.8.2/test/integration/test_build.py` & `wily-1.9.0/test/integration/test_build.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,74 +2,92 @@
 Tests for the wily build command.
 
 All of the following tests will use a click CLI runner to fully simulate the CLI.
 Many of the tests will depend on a "builddir" fixture which is a compiled wily cache.
 
 TODO : Test build + build with extra operator
 """
+import os
+import sys
 import pathlib
+import tempfile
 import pytest
 from click.testing import CliRunner
 from git import Repo, Actor
 from mock import patch
 
 import wily.__main__ as main
 from wily.archivers import ALL_ARCHIVERS
+from wily.config import generate_cache_path
 
+_path = "src\\test.py" if sys.platform == "win32" else "src/test.py"
 
-def test_build_not_git_repo(tmpdir):
+
+def test_build_not_git_repo(tmpdir, cache_path):
     """
     Test that build defaults to filesystem in a non-git directory
     """
-    with patch("wily.logger") as logger:
-        runner = CliRunner()
-        result = runner.invoke(main.cli, ["--path", tmpdir, "build", "test.py"])
-        assert result.exit_code == 0, result.stdout
-        cache_path = tmpdir / ".wily"
-        assert cache_path.exists()
-        index_path = tmpdir / ".wily" / "filesystem" / "index.json"
-        assert index_path.exists()
+    runner = CliRunner()
+    result = runner.invoke(
+        main.cli, ["--path", tmpdir, "--cache", cache_path, "build", "test.py"]
+    )
+    assert result.exit_code == 0, result.stdout
+    cache_path = pathlib.Path(cache_path)
+    assert cache_path.exists()
+    index_path = cache_path / "filesystem" / "index.json"
+    assert index_path.exists()
+
 
+def test_build_custom_cache(tmpdir):
+    """
+    Test that build defaults to filesystem in a non-git directory with custom cache path.
+    """
+    runner = CliRunner()
+    result = runner.invoke(
+        main.cli, ["--path", tmpdir, "--cache", tmpdir / ".wily", "build", "test.py"]
+    )
+    assert result.exit_code == 0, result.stdout
+    cache_path = tmpdir / ".wily"
+    assert cache_path.exists()
+    index_path = cache_path / "filesystem" / "index.json"
+    assert index_path.exists()
+    assert not pathlib.Path(generate_cache_path(tmpdir)).exists()
 
-def test_build_invalid_path(tmpdir):
+
+def test_build_invalid_path():
     """
     Test that build fails with a garbage path
     """
-    with patch("wily.logger") as logger:
-        runner = CliRunner()
-        result = runner.invoke(main.cli, ["--path", "/fo/v/a", "build", "test.py"])
-        assert result.exit_code == 1, result.stdout
+    runner = CliRunner()
+    result = runner.invoke(main.cli, ["--path", "/fo/v/a", "build", "test.py"])
+    assert result.exit_code == 1, result.stdout
 
 
 def test_build_no_target(tmpdir):
     """
     Test that build fails with no target
     """
-    with patch("wily.logger") as logger:
-        runner = CliRunner()
-        result = runner.invoke(main.cli, ["--path", tmpdir, "build"])
-        assert result.exit_code == 2, result.stdout
+    runner = CliRunner()
+    result = runner.invoke(main.cli, ["--path", tmpdir, "build"])
+    assert result.exit_code == 2, result.stdout
 
 
 def test_build_crash(tmpdir):
     """
-    Test that build works in a basic repository.
+    Simulate a runtime error in the build.
     """
     repo = Repo.init(path=tmpdir)
     tmppath = pathlib.Path(tmpdir)
 
     # Write a test file to the repo
     with open(tmppath / "test.py", "w") as test_txt:
         test_txt.write("import abc")
 
-    with open(tmppath / ".gitignore", "w") as test_txt:
-        test_txt.write(".wily/")
-
     index = repo.index
-    index.add(["test.py", ".gitignore"])
+    index.add(["test.py"])
 
     author = Actor("An author", "author@example.com")
     committer = Actor("A committer", "committer@example.com")
 
     index.commit("basic test", author=author, committer=committer)
     import wily.commands.build
 
@@ -77,113 +95,98 @@
         wily.commands.build.Bar, "finish", side_effect=RuntimeError("arggh")
     ) as bar_finish:
         runner = CliRunner()
         result = runner.invoke(main.cli, ["--path", tmpdir, "build", "test.py"])
         assert bar_finish.called_once
         assert result.exit_code == 1, result.stdout
 
-    with patch("wily.commands.build.logger") as logger:
-        logger.level = "DEBUG"
-        with patch.object(
-            wily.commands.build.Bar, "finish", side_effect=RuntimeError("arggh")
-        ) as bar_finish:
-            runner = CliRunner()
-            result = runner.invoke(
-                main.cli, ["--debug", "--path", tmpdir, "build", "test.py"]
-            )
-            assert bar_finish.called_once
-            assert result.exit_code == 1, result.stdout
 
-
-def test_build(tmpdir):
+def test_build(tmpdir, cache_path):
     """
     Test that build works in a basic repository.
     """
     repo = Repo.init(path=tmpdir)
     tmppath = pathlib.Path(tmpdir)
 
     # Write a test file to the repo
     with open(tmppath / "test.py", "w") as test_txt:
         test_txt.write("import abc")
 
-    with open(tmppath / ".gitignore", "w") as test_txt:
-        test_txt.write(".wily/")
-
     index = repo.index
-    index.add(["test.py", ".gitignore"])
+    index.add(["test.py"])
 
     author = Actor("An author", "author@example.com")
     committer = Actor("A committer", "committer@example.com")
 
     commit = index.commit("basic test", author=author, committer=committer)
+    runner = CliRunner()
+    result = runner.invoke(
+        main.cli,
+        ["--debug", "--path", tmpdir, "--cache", cache_path, "build", "test.py"],
+    )
+    assert result.exit_code == 0, result.stdout
 
-    with patch("wily.logger") as logger:
-        runner = CliRunner()
-        result = runner.invoke(
-            main.cli, ["--debug", "--path", tmpdir, "build", "test.py"]
-        )
-        assert result.exit_code == 0, result.stdout
-
-    cache_path = tmpdir / ".wily"
+    cache_path = pathlib.Path(cache_path)
     assert cache_path.exists()
-    index_path = tmpdir / ".wily" / "git" / "index.json"
+    index_path = cache_path / "git" / "index.json"
     assert index_path.exists()
-    rev_path = tmpdir / ".wily" / "git" / commit.name_rev.split(" ")[0] + ".json"
+    rev_path = cache_path / "git" / (commit.name_rev.split(" ")[0] + ".json")
     assert rev_path.exists()
 
 
-def test_build_twice(tmpdir):
+def test_build_twice(tmpdir, cache_path):
     """
     Test that build works when run twice.
     """
     repo = Repo.init(path=tmpdir)
     tmppath = pathlib.Path(tmpdir)
 
     # Write a test file to the repo
     with open(tmppath / "test.py", "w") as test_txt:
         test_txt.write("import abc")
-    with open(tmppath / ".gitignore", "w") as test_txt:
-        test_txt.write(".wily/")
+
     index = repo.index
-    index.add(["test.py", ".gitignore"])
+    index.add(["test.py"])
 
     author = Actor("An author", "author@example.com")
     committer = Actor("A committer", "committer@example.com")
 
     commit = index.commit("basic test", author=author, committer=committer)
 
     runner = CliRunner()
-    result = runner.invoke(main.cli, ["--debug", "--path", tmpdir, "build", "test.py"])
+    result = runner.invoke(
+        main.cli,
+        ["--debug", "--path", tmpdir, "--cache", cache_path, "build", "test.py"],
+    )
     assert result.exit_code == 0, result.stdout
 
-    cache_path = tmpdir / ".wily"
+    cache_path = pathlib.Path(cache_path) / "git"
     assert cache_path.exists()
-    index_path = tmpdir / ".wily" / "git" / "index.json"
+    index_path = cache_path / "index.json"
     assert index_path.exists()
-    rev_path = tmpdir / ".wily" / "git" / commit.name_rev.split(" ")[0] + ".json"
+    rev_path = cache_path / (commit.name_rev.split(" ")[0] + ".json")
     assert rev_path.exists()
 
     # Write a test file to the repo
     with open(tmppath / "test.py", "w") as test_txt:
         test_txt.write("import abc\nfoo = 1")
 
     index.add(["test.py"])
 
     commit2 = index.commit("basic test", author=author, committer=committer)
 
     result = runner.invoke(main.cli, ["--debug", "--path", tmpdir, "build", "test.py"])
     assert result.exit_code == 0, result.stdout
 
-    cache_path = tmpdir / ".wily"
     assert cache_path.exists()
-    index_path = tmpdir / ".wily" / "git" / "index.json"
+    index_path = cache_path / "index.json"
     assert index_path.exists()
-    rev_path = tmpdir / ".wily" / "git" / commit.name_rev.split(" ")[0] + ".json"
+    rev_path = cache_path / (commit.name_rev.split(" ")[0] + ".json")
     assert rev_path.exists()
-    rev_path2 = tmpdir / ".wily" / "git" / commit2.name_rev.split(" ")[0] + ".json"
+    rev_path2 = cache_path / (commit2.name_rev.split(" ")[0] + ".json")
     assert rev_path2.exists()
 
 
 def test_build_no_commits(tmpdir):
     """
     Test that build fails cleanly with no commits
     """
@@ -209,29 +212,30 @@
     assert result.exit_code == 1, result.stdout
 
 
 def test_build_no_git_history(tmpdir):
     repo = Repo.init(path=tmpdir)
     with patch("wily.logger") as logger:
         runner = CliRunner()
-        result = runner.invoke(main.cli, ["--path", tmpdir, "build", "src/test.py"])
+        result = runner.invoke(main.cli, ["--path", tmpdir, "build", _path])
         assert result.exit_code == 1, result.stdout
 
 
 archivers = {name for name in ALL_ARCHIVERS.keys()}
 
 
 @pytest.mark.parametrize("archiver", archivers)
-def test_build_archiver(gitdir, archiver):
+def test_build_archiver(gitdir, archiver, cache_path):
     """
     Test the build against each type of archiver
     """
     with patch("wily.logger") as logger:
         runner = CliRunner()
         result = runner.invoke(
-            main.cli, ["--path", gitdir, "build", "src/test.py", "-a", archiver]
+            main.cli,
+            ["--path", gitdir, "--cache", cache_path, "build", _path, "-a", archiver],
         )
         assert result.exit_code == 0, result.stdout
-        cache_path = gitdir / ".wily"
+        cache_path = pathlib.Path(cache_path)
         assert cache_path.exists()
-        index_path = gitdir / ".wily" / archiver / "index.json"
+        index_path = cache_path / archiver / "index.json"
         assert index_path.exists()
```

### Comparing `wily-1.8.2/test/integration/test_diff.py` & `wily-1.9.0/test/integration/test_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import pathlib
+import sys
 from textwrap import dedent
 
 from click.testing import CliRunner
 
 import wily.__main__ as main
 
+_path = "src\\test.py" if sys.platform == "win32" else "src/test.py"
+
 
 def test_diff_no_cache(tmpdir):
     runner = CliRunner()
-    result = runner.invoke(main.cli, ["--path", tmpdir, "diff", "src/test.py"])
+    result = runner.invoke(main.cli, ["--path", tmpdir, "diff", _path])
     assert result.exit_code == 1, result.stdout
 
 
 def test_diff_no_path(tmpdir):
     runner = CliRunner()
     result = runner.invoke(main.cli, ["--path", tmpdir, "diff"])
     assert result.exit_code == 2, result.stdout
 
 
 def test_diff_output(builddir):
     """ Test the diff feature with no changes """
     runner = CliRunner()
-    result = runner.invoke(
-        main.cli, ["--debug", "--path", builddir, "diff", "src/test.py"]
-    )
+    result = runner.invoke(main.cli, ["--debug", "--path", builddir, "diff", _path])
     assert result.exit_code == 0, result.stdout
     assert "test.py" not in result.stdout
 
 
 def test_diff_output_all(builddir):
     """ Test the diff feature with no changes and the --all flag """
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--debug", "--path", builddir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", builddir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
 
 
 def test_diff_output_bad_path(builddir):
     """ Test the diff feature with no changes """
@@ -52,15 +53,15 @@
     """ Test the diff feature by removing all functions and classes """
 
     with open(pathlib.Path(builddir) / "src" / "test.py", "w") as test_py:
         test_py.write("print(1)")
 
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--debug", "--path", builddir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", builddir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
 
 
 def test_diff_output_more_complex(builddir):
     """ Test the diff feature by making the test file more complicated """
 
@@ -81,15 +82,15 @@
             """
 
     with open(pathlib.Path(builddir) / "src" / "test.py", "w") as test_py:
         test_py.write(dedent(complex_test))
 
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--debug", "--path", builddir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", builddir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
     assert "- -> -" not in result.stdout
     assert "-> -" not in result.stdout
     assert "- ->" not in result.stdout
 
@@ -108,15 +109,15 @@
             """
 
     with open(pathlib.Path(builddir) / "src" / "test.py", "w") as test_py:
         test_py.write(dedent(simple_test))
 
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--debug", "--path", builddir, "diff", "src/test.py", "--all"]
+        main.cli, ["--debug", "--path", builddir, "diff", _path, "--all"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
     assert "- -> -" not in result.stdout
     assert "-> -" not in result.stdout
     assert "- ->" not in result.stdout
 
@@ -127,16 +128,15 @@
     simple_test = """print("test")"""
 
     with open(pathlib.Path(builddir) / "src" / "test.py", "w") as test_py:
         test_py.write(dedent(simple_test))
 
     runner = CliRunner()
     result = runner.invoke(
-        main.cli,
-        ["--debug", "--path", builddir, "diff", "src/test.py", "--metrics", "raw.loc"],
+        main.cli, ["--debug", "--path", builddir, "diff", _path, "--metrics", "raw.loc"]
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
     assert "10 -> \x1b[33m1\x1b[0m" in result.stdout  # 10 -> 1 (in green)
 
 
 def test_diff_output_rank(builddir):
@@ -151,15 +151,15 @@
     result = runner.invoke(
         main.cli,
         [
             "--debug",
             "--path",
             builddir,
             "diff",
-            "src/test.py",
+            _path,
             "--all",
             "--metrics",
             "maintainability.rank",
         ],
     )
     assert result.exit_code == 0, result.stdout
     assert "test.py" in result.stdout
```

### Comparing `wily-1.8.2/test/integration/test_graph.py` & `wily-1.9.0/test/integration/test_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,71 @@
+import sys
 from mock import patch
-
+import tempfile
 from click.testing import CliRunner
 
 import wily.__main__ as main
 
+_path = "src\\test.py" if sys.platform == "win32" else "src/test.py"
 
-PATCHED_ENV = {"BROWSER": "echo %s", "LC_ALL": "C.UTF-8", "LANG": "C.UTF-8"}
 
+PATCHED_ENV = {
+    "BROWSER": "echo %s",
+    "LC_ALL": "C.UTF-8",
+    "LANG": "C.UTF-8",
+    "HOME": tempfile.gettempdir(),
+}
 
-def test_graph_no_cache(tmpdir):
-    runner = CliRunner()
 
+def test_graph_no_cache(tmpdir, cache_path):
+    runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli, ["--path", tmpdir, "graph", "src/test.py", "raw.loc"]
+            main.cli,
+            ["--path", tmpdir, "--cache", cache_path, "graph", _path, "raw.loc"],
         )
     assert result.exit_code == 1, result.stdout
 
 
 def test_graph(builddir):
     """ Test the graph feature """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli, ["--path", builddir, "graph", "src/test.py", "raw.loc"]
+            main.cli, ["--path", builddir, "graph", _path, "raw.loc"]
         )
     assert result.exit_code == 0, result.stdout
 
 
 def test_graph_all(builddir):
     """ Test the graph feature """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli, ["--path", builddir, "graph", "src/test.py", "raw.loc", "--all"]
+            main.cli, ["--path", builddir, "graph", _path, "raw.loc", "--all"]
         )
     assert result.exit_code == 0, result.stdout
 
 
 def test_graph_changes(builddir):
     """ Test the graph feature """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli,
-            ["--path", builddir, "graph", "src/test.py", "raw.loc", "--changes"],
+            main.cli, ["--path", builddir, "graph", _path, "raw.loc", "--changes"]
         )
     assert result.exit_code == 0, result.stdout
 
 
 def test_graph_custom_x(builddir):
     """ Test the graph feature """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli,
-            ["--path", builddir, "graph", "src/test.py", "raw.loc", "-x", "raw.sloc"],
+            main.cli, ["--path", builddir, "graph", _path, "raw.loc", "-x", "raw.sloc"]
         )
     assert result.exit_code == 0, result.stdout
 
 
 def test_graph_path(builddir):
     """ Test the graph feature """
     runner = CliRunner()
@@ -71,31 +77,30 @@
 
 
 def test_graph_multiple(builddir):
     """ Test the graph feature with multiple metrics """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
-            main.cli,
-            ["--path", builddir, "graph", "src/test.py", "raw.loc", "raw.comments"],
+            main.cli, ["--path", builddir, "graph", _path, "raw.loc", "raw.comments"]
         )
     assert result.exit_code == 0, result.stdout
 
 
 def test_graph_multiple_custom_x(builddir):
     """ Test the graph feature with multiple metrics """
     runner = CliRunner()
     with patch.dict("os.environ", values=PATCHED_ENV, clear=True):
         result = runner.invoke(
             main.cli,
             [
                 "--path",
                 builddir,
                 "graph",
-                "src/test.py",
+                _path,
                 "raw.loc",
                 "raw.comments",
                 "-x",
                 "raw.sloc",
             ],
         )
     assert result.exit_code == 0, result.stdout
@@ -118,15 +123,15 @@
         result = runner.invoke(
             main.cli,
             [
                 "--debug",
                 "--path",
                 builddir,
                 "graph",
-                "src/test.py",
+                _path,
                 "raw.loc",
                 "-o",
                 "test.html",
             ],
         )
 
     assert result.exit_code == 0, result.stdout
```

### Comparing `wily-1.8.2/test/integration/test_index.py` & `wily-1.9.0/test/integration/test_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from click.testing import CliRunner
 
 import wily.__main__ as main
 
 
-def test_index_no_cache(tmpdir):
+def test_index_no_cache(tmpdir, cache_path):
     runner = CliRunner()
-    result = runner.invoke(main.cli, ["--path", tmpdir, "index"])
+    result = runner.invoke(main.cli, ["--path", tmpdir, "--cache", cache_path, "index"])
     assert result.exit_code == 1, result.stdout
 
 
 def test_index(builddir):
     """
     Test that index works with a build
     """
```

### Comparing `wily-1.8.2/test/integration/test_report.py` & `wily-1.9.0/test/integration/test_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from click.testing import CliRunner
-
+import sys
 import wily.__main__ as main
 
+_path = "src\\test.py" if sys.platform == "win32" else "src/test.py"
+
 
-def test_report_no_cache(tmpdir):
+def test_report_no_cache(tmpdir, cache_path):
     runner = CliRunner()
-    result = runner.invoke(main.cli, ["--path", tmpdir, "report", "src/test.py"])
+    result = runner.invoke(
+        main.cli, ["--path", tmpdir, "--cache", cache_path, "report", _path]
+    )
     assert result.exit_code == 1, result.stdout
 
 
 def test_report(builddir):
     """
     Test that report works with a build and a specific metric
     """
     runner = CliRunner()
     result = runner.invoke(
         main.cli,
-        [
-            "--path",
-            builddir,
-            "report",
-            "src/test.py",
-            "raw.multi",
-            "maintainability.rank",
-        ],
+        ["--path", builddir, "report", _path, "raw.multi", "maintainability.rank"],
     )
     assert result.exit_code == 0, result.stdout
     assert "Not found" not in result.stdout
 
 
 def test_report_granular(builddir):
     """
@@ -36,15 +33,15 @@
     runner = CliRunner()
     result = runner.invoke(
         main.cli,
         [
             "--path",
             builddir,
             "report",
-            "src/test.py:function1",
+            _path + ":function1",
             "cyclomatic.complexity",
             "-n",
             1,
         ],
     )
     assert result.exit_code == 0, result.stdout
     assert "Not found" not in result.stdout
@@ -52,26 +49,26 @@
 
 def test_report_not_found(builddir):
     """
     Test that report works with a build but not with an invalid path
     """
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--path", builddir, "report", "src/test1.py", "raw.loc"]
+        main.cli, ["--path", builddir, "report", "test1.py", "raw.loc"]
     )
     assert result.exit_code == 0, result.stdout
     assert "Not found" in result.stdout
 
 
 def test_report_default_metrics(builddir):
     """
     Test that report works with default metrics
     """
     runner = CliRunner()
-    result = runner.invoke(main.cli, ["--path", builddir, "report", "src/test.py"])
+    result = runner.invoke(main.cli, ["--path", builddir, "report", _path])
     assert result.exit_code == 0, result.stdout
     assert "Not found" not in result.stdout
 
 
 def test_report_path(builddir):
     """
     Test that report with a path to a folder (aggregate values)
@@ -84,38 +81,37 @@
 
 def test_report_with_message(builddir):
     """
     Test that report works messages in UI
     """
     runner = CliRunner()
     result = runner.invoke(
-        main.cli,
-        ["--path", builddir, "report", "src/test.py", "raw.multi", "--message"],
+        main.cli, ["--path", builddir, "report", _path, "raw.multi", "--message"]
     )
     assert result.exit_code == 0, result.stdout
     assert "basic test" in result.stdout
     assert "remove line" in result.stdout
     assert "Not found" not in result.stdout
 
 
 def test_report_high_metric(builddir):
     """
     Test that report works with a build on a metric expecting high values
     """
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--path", builddir, "report", "src/test.py", "raw.comments"]
+        main.cli, ["--path", builddir, "report", _path, "raw.comments"]
     )
     assert result.exit_code == 0, result.stdout
     assert "Not found" not in result.stdout
 
 
 def test_report_low_metric(builddir):
     """
     Test that report works with a build on a metric expecting high values
     """
     runner = CliRunner()
     result = runner.invoke(
-        main.cli, ["--path", builddir, "report", "src/test.py", "maintainability.mi"]
+        main.cli, ["--path", builddir, "report", _path, "maintainability.mi"]
     )
     assert result.exit_code == 0, result.stdout
     assert "Not found" not in result.stdout
```

### Comparing `wily-1.8.2/test/integration/test_state.py` & `wily-1.9.0/test/integration/test_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import wily.state
 
 
 @pytest.fixture
 def config(builddir):
     _cfg = wily.config.DEFAULT_CONFIG
     _cfg.path = builddir
-    _cfg.cache_path = os.path.join(builddir, wily.config.DEFAULT_CACHE_PATH)
     return _cfg
 
 
 def test_state_defaults(config):
     """ Test the state defaults """
     state = wily.state.State(config)
     assert state.index
@@ -28,13 +27,11 @@
 
 
 def test_index(config):
     """ Test the state index """
     state = wily.state.State(config)
     assert state.index
     assert state.index["git"] is not None
-    assert len(state.index["git"]) == 3
-    assert len(state.index["git"].revision_keys) == 3
     for revision in state.index["git"].revisions:
         assert state.index["git"][revision.revision.key]
         assert revision.revision in state.index["git"]
         assert revision.revision.key in state.index["git"]
```

### Comparing `wily-1.8.2/test/integration/test_wily.py` & `wily-1.9.0/test/integration/test_wily.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/test/unit/test_archivers.py` & `wily-1.9.0/test/unit/test_archivers.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/test/unit/test_build_unit.py` & `wily-1.9.0/test/unit/test_build_unit.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/test/unit/test_cache.py` & `wily-1.9.0/test/unit/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import pathlib
-
+import sys
 import pytest
 
 import wily.cache as cache
 from wily.archivers import Revision
 from wily.config import DEFAULT_CONFIG, ARCHIVER_GIT
 
 
@@ -111,14 +111,15 @@
     fn = cache.store(config, ARCHIVER_GIT, _TEST_REVISION, _TEST_STATS)
     with open(fn) as cache_item:
         result = json.load(cache_item)
         assert isinstance(result, dict)
         assert result == _TEST_STATS
 
 
+@pytest.mark.skipif(sys.platform == "win32", reason="does not run on windows")
 def test_store_twice(tmpdir):
     """ Test that you can't write the same revision twice """
     config = DEFAULT_CONFIG
     cache_path = pathlib.Path(tmpdir) / ".wily"
     cache_path.mkdir()
     config.cache_path = cache_path
     target_path = str(pathlib.Path(tmpdir) / "foo" / "bar.py")
@@ -153,15 +154,18 @@
         date="17/01/1990",
         message="my changes",
     )
     fn = cache.store(config, ARCHIVER_GIT, _TEST_REVISION, _TEST_STATS)
     with open(fn) as cache_item:
         result = json.load(cache_item)
         assert isinstance(result, dict)
-        assert "foo/bar.py" in result["operator_data"]["test"].keys()
+        if sys.platform == "win32":
+            assert "foo\\bar.py" in result["operator_data"]["test"].keys()
+        else:
+            assert "foo/bar.py" in result["operator_data"]["test"].keys()
 
 
 def test_store_index(tmpdir):
     """
     Test the store index
     """
     config = DEFAULT_CONFIG
```

### Comparing `wily-1.8.2/test/unit/test_cli.py` & `wily-1.9.0/test/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/test/unit/test_config.py` & `wily-1.9.0/test/unit/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os.path
 
 import wily.config
 
 
 def test_config_empty_defaults(tmpdir):
     """
-    TEst that an empty config path sets to defaults.
+    Test that an empty config path sets to defaults.
     """
     config = """
     """
     config_path = os.path.join(tmpdir, "wily.cfg")
     with open(config_path, "w") as config_f:
         config_f.write(config)
```

### Comparing `wily-1.8.2/test/unit/test_operators.py` & `wily-1.9.0/test/unit/test_operators.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/__init__.py` & `wily-1.9.0/wily/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 A Python application for tracking, reporting on timing and complexity in tests and applications.
 """
 import colorlog
 import datetime
 
 
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 
 _handler = colorlog.StreamHandler()
 _handler.setFormatter(colorlog.ColoredFormatter("%(log_color)s%(message)s"))
 
 logger = colorlog.getLogger(__name__)
 logger.addHandler(_handler)
```

### Comparing `wily-1.8.2/wily/__main__.py` & `wily-1.9.0/wily/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: UTF-8 -*-
 """Main command line."""
 
-import os.path
-
 import click
 
-from wily import logger
+from wily import logger, __version__
 from wily.archivers import resolve_archiver
 from wily.cache import exists, get_default_metrics
-from wily.config import DEFAULT_CONFIG_PATH, DEFAULT_CACHE_PATH
+from wily.config import DEFAULT_CONFIG_PATH
 from wily.config import load as load_config
+from wily.decorators import add_version
 from wily.operators import resolve_operators
 
 
 @click.group()
+@click.version_option(
+    __version__, "-V", "--version", message="\U0001F98A %(prog)s, version %(version)s"
+)
 @click.option(
     "--debug/--no-debug",
     default=False,
     help="Print debug information, used for development",
 )
 @click.option(
     "--config",
@@ -27,16 +29,23 @@
 @click.option(
     "-p",
     "--path",
     type=click.Path(resolve_path=True),
     default=".",
     help="Root path to the project folder to scan",
 )
+@click.option(
+    "-c",
+    "--cache",
+    type=click.Path(resolve_path=True),
+    help="Override the default cache path (defaults to $HOME/.wily/HASH)",
+)
 @click.pass_context
-def cli(ctx, debug, config, path):
+@add_version
+def cli(ctx, debug, config, path, cache):
     """
     \U0001F98A Inspect and search through the complexity of your source code.
 
     To get started, run setup:
 
       $ wily setup
 
@@ -59,15 +68,17 @@
     else:
         logger.setLevel("INFO")
 
     ctx.obj["CONFIG"] = load_config(config)
     if path:
         logger.debug(f"Fixing path to {path}")
         ctx.obj["CONFIG"].path = path
-        ctx.obj["CONFIG"].cache_path = os.path.join(path, DEFAULT_CACHE_PATH)
+    if cache:
+        logger.debug(f"Fixing cache to {cache}")
+        ctx.obj["CONFIG"].cache_path = cache
     logger.debug(f"Loaded configuration from {config}")
 
 
 @cli.command()
 @click.option(
     "-n",
     "--max-revisions",
@@ -85,21 +96,16 @@
 @click.option(
     "-a",
     "--archiver",
     type=click.STRING,
     default="git",
     help="Archiver to use, defaults to git if git repo, else filesystem",
 )
-@click.option(
-    "--skip-gitignore-check/--gitignore-check",
-    default=False,
-    help="Skip checking of .gitignore for '.wily/'",
-)
 @click.pass_context
-def build(ctx, max_revisions, targets, operators, skip_gitignore_check, archiver):
+def build(ctx, max_revisions, targets, operators, archiver):
     """Build the wily cache."""
     config = ctx.obj["CONFIG"]
 
     from wily.commands.build import build
 
     if max_revisions:
         logger.debug(f"Fixing revisions to {max_revisions}")
@@ -109,15 +115,14 @@
         logger.debug(f"Fixing operators to {operators}")
         config.operators = operators.strip().split(",")
 
     if archiver:
         logger.debug(f"Fixing archiver to {archiver}")
         config.archiver = archiver
 
-    config.skip_ignore_check = skip_gitignore_check
     logger.debug(f"Fixing targets to {targets}")
     config.targets = targets
 
     build(
         config=config,
         archiver=resolve_archiver(config.archiver),
         operators=resolve_operators(config.operators),
```

### Comparing `wily-1.8.2/wily/archivers/__init__.py` & `wily-1.9.0/wily/archivers/__init__.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/archivers/filesystem.py` & `wily-1.9.0/wily/archivers/filesystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Filesystem Archiver.
 
 Implementation of the archiver API for a standard directory (no revisions)
 """
 import logging
 import os.path
-from datetime import datetime
 import hashlib
 from wily.archivers import BaseArchiver, Revision
 
 logger = logging.getLogger(__name__)
 
 
 class FilesystemArchiver(BaseArchiver):
```

### Comparing `wily-1.8.2/wily/archivers/git.py` & `wily-1.9.0/wily/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,142 @@
 """
-Git Archiver.
+Configuration of wily.
 
-Implementation of the archiver API for the gitpython module.
+TODO : Handle operator settings. Maybe a section for each operator and then pass kwargs to operators?
+TODO : Better utilise default values and factory in @dataclass to replace DEFAULT_CONFIG
+ and replace the logic in load() to set default values.
 """
+from functools import lru_cache
+import configparser
 import logging
 import pathlib
+import hashlib
+from dataclasses import dataclass, field
+from typing import Any, List
 
-from git import Repo
-import git.exc
-
-from wily.archivers import BaseArchiver, Revision
+import wily.operators as operators
+from wily.archivers import ARCHIVER_GIT
 
 logger = logging.getLogger(__name__)
 
-"""Possible combinations in .gitignore."""
-gitignore_options = (".wily/", ".wily", ".wily/*", ".wily/**/*")
-
-
-class InvalidGitRepositoryError(Exception):
-    """Error for when a folder is not a git repo."""
-
-    pass
-
 
-class DirtyGitRepositoryError(Exception):
-    """Error for a dirty git repository (untracked files)."""
-
-    def __init__(self, untracked_files):
-        """
-        Raise error for untracked files.
-
-        :param untracked_files: List of untracked files
-        :param untracked_files: ``list``
-        """
-        self.untracked_files = untracked_files
-        self.message = "Dirty repository, make sure you commit/stash files first"
-
-
-class WilyIgnoreGitRepositoryError(Exception):
-    """Error for .wily/ being missing from .gitignore."""
-
-    def __init__(self):
-        """Raise runtime error for .gitignore being incorrectly configured."""
-        self.message = "Please add '.wily/' to .gitignore before running wily"
-
-
-class GitArchiver(BaseArchiver):
-    """Gitpython implementation of the base archiver."""
-
-    name = "git"
-
-    """Whether to ignore checking for .wily/ in .gitignore files."""
-    ignore_gitignore = False
-
-    def __init__(self, config):
-        """
-        Instantiate a new Git Archiver.
-
-        :param config: The wily configuration
-        :type  config: :class:`wily.config.WilyConfig`
-        """
-        try:
-            self.repo = Repo(config.path)
-        except git.exc.InvalidGitRepositoryError as e:
-            raise InvalidGitRepositoryError from e
-        self.ignore_gitignore = config.skip_ignore_check
-        gitignore = pathlib.Path(config.path) / ".gitignore"
-        if not gitignore.exists():
-            raise WilyIgnoreGitRepositoryError()
-
-        with open(gitignore, "r") as gitignore_f:
-            lines = [line.replace("\n", "") for line in gitignore_f.readlines()]
-            logger.debug(lines)
-            has_ignore = False
-            for gitignore_opt in gitignore_options:
-                if gitignore_opt in lines:
-                    has_ignore = True
-                    break
-
-            if not has_ignore and not self.ignore_gitignore:  # :-/
-                raise WilyIgnoreGitRepositoryError()
-
-        self.config = config
-        self.current_branch = self.repo.active_branch
-        assert not self.repo.bare, "Not a Git repository"
-
-    def revisions(self, path, max_revisions):
-        """
-        Get the list of revisions.
-
-        :param path: the path to target.
-        :type  path: ``str``
-
-        :param max_revisions: the maximum number of revisions.
-        :type  max_revisions: ``int``
-
-        :return: A list of revisions.
-        :rtype: ``list`` of :class:`Revision`
-        """
-        if self.repo.is_dirty():
-            raise DirtyGitRepositoryError(self.repo.untracked_files)
-
-        revisions = []
-        for commit in self.repo.iter_commits(
-            self.current_branch, max_count=max_revisions
-        ):
-            rev = Revision(
-                key=commit.name_rev.split(" ")[0],
-                author_name=commit.author.name,
-                author_email=commit.author.email,
-                date=commit.committed_date,
-                message=commit.message,
-            )
-            revisions.append(rev)
-        return revisions
-
-    def checkout(self, revision, options):
-        """
-        Checkout a specific revision.
-
-        :param revision: The revision identifier.
-        :type  revision: :class:`Revision`
-
-        :param options: Any additional options.
-        :type  options: ``dict``
-        """
-        rev = revision.key
-        self.repo.git.checkout(rev)
-
-    def finish(self):
-        """
-        Clean up any state if processing completed/failed.
-
-        For git, will checkout HEAD on the original branch when finishing
-        """
-        self.repo.git.checkout(self.current_branch)
-        self.repo.close()
+@lru_cache(maxsize=128)
+def generate_cache_path(path):
+    """
+    Generate a reusable path to cache results.
+
+    Will use the --path of the target and hash into
+    a 9-character directory within the HOME folder.
+
+    :return: The cache path
+    :rtype: ``str``
+    """
+    logger.debug(f"Generating cache for {path}")
+    sha = hashlib.sha1(str(path).encode()).hexdigest()[:9]
+    HOME = pathlib.Path.home()
+    cache_path = str(HOME / ".wily" / sha)
+    logger.debug(f"Cache path is {cache_path}")
+    return cache_path
+
+
+@dataclass
+class WilyConfig(object):
+    """
+    Wily configuration.
+
+    A data class to reflect the configurable options within Wily.
+    """
+
+    operators: List
+    archiver: Any
+    path: str
+    max_revisions: int
+    targets: List[str] = None
+    checkout_options: dict = field(default_factory=dict)
+
+    def __post_init__(self):
+        """Clone targets as a list of path."""
+        if self.targets is None or "":
+            self.targets = [self.path]
+        self._cache_path = None
+
+    @property
+    def cache_path(self):
+        """Path to the cache."""
+        if not self._cache_path:
+            self._cache_path = generate_cache_path(pathlib.Path(self.path).absolute())
+        return self._cache_path
+
+    @cache_path.setter
+    def cache_path(self, value):
+        """Override the cache path."""
+        logger.debug(f"Setting custom cache path to {value}")
+        self._cache_path = value
+
+
+# Default values for Wily
+
+""" The default operators """
+DEFAULT_OPERATORS = {
+    operators.OPERATOR_RAW.name,
+    operators.OPERATOR_MAINTAINABILITY.name,
+    operators.OPERATOR_CYCLOMATIC.name,
+}
+
+""" The name of the default archiver """
+DEFAULT_ARCHIVER = ARCHIVER_GIT.name
+
+""" The default configuration file name """
+DEFAULT_CONFIG_PATH = "wily.cfg"
+
+""" The default section name in the config """
+DEFAULT_CONFIG_SECTION = "wily"
+
+""" The default maximum number of revisions to archiver """
+DEFAULT_MAX_REVISIONS = 50
+
+DEFAULT_PATH = "."
+
+""" The default configuration for Wily (if no config file exists) """
+DEFAULT_CONFIG = WilyConfig(
+    operators=DEFAULT_OPERATORS,
+    archiver=DEFAULT_ARCHIVER,
+    path=DEFAULT_PATH,
+    max_revisions=DEFAULT_MAX_REVISIONS,
+)
+
+""" Default table style in console. See tabulate docs for more. """
+DEFAULT_GRID_STYLE = "fancy_grid"
+
+
+def load(config_path=DEFAULT_CONFIG_PATH):
+    """
+    Load config file and set values to defaults where no present.
+
+    :return: The configuration ``WilyConfig``
+    :rtype: :class:`wily.config.WilyConfig`
+    """
+    if not pathlib.Path(config_path).exists():
+        logger.debug(f"Could not locate {config_path}, using default config.")
+        return DEFAULT_CONFIG
+
+    config = configparser.ConfigParser(default_section=DEFAULT_CONFIG_SECTION)
+    config.read(config_path)
+
+    operators = config.get(
+        section=DEFAULT_CONFIG_SECTION, option="operators", fallback=DEFAULT_OPERATORS
+    )
+    archiver = config.get(
+        section=DEFAULT_CONFIG_SECTION, option="archiver", fallback=DEFAULT_ARCHIVER
+    )
+    path = config.get(section=DEFAULT_CONFIG_SECTION, option="path", fallback=".")
+    max_revisions = int(
+        config.get(
+            section=DEFAULT_CONFIG_SECTION,
+            option="max_revisions",
+            fallback=DEFAULT_MAX_REVISIONS,
+        )
+    )
+
+    return WilyConfig(
+        operators=operators, archiver=archiver, path=path, max_revisions=max_revisions
+    )
```

### Comparing `wily-1.8.2/wily/cache.py` & `wily-1.9.0/wily/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 A module for working with the .wily/ cache directory.
 
 This API is not intended to be public and should not be consumed directly.
 The API in this module is for archivers and commands to work with the local cache
 
-TODO: Version .wily/ cache folders?
-
 """
 
 import json
 import os.path
 import pathlib
 import shutil
 
@@ -37,15 +35,15 @@
     index_path = pathlib.Path(config.cache_path) / "index.json"
     if index_path.exists():
         with open(index_path, "r") as out:
             index = json.load(out)
         if index["version"] != __version__:
             # TODO: Inspect the versions properly.
             logger.warning(
-                "! Wily cache is old, you may incur errors until you rebuild the cache."
+                "Wily cache is old, you may incur errors until you rebuild the cache."
             )
     else:
         logger.warning(
             "Wily cache was not versioned, you may incur errors until you rebuild the cache."
         )
         create_index(config)
     return True
@@ -69,15 +67,15 @@
     :return: The path to the cache
     :rtype: ``str``
     """
     if exists(config):
         logger.debug("Wily cache exists, skipping")
         return config.cache_path
     logger.debug(f"Creating wily cache {config.cache_path}")
-    pathlib.Path(config.cache_path).mkdir()
+    pathlib.Path(config.cache_path).mkdir(parents=True, exist_ok=True)
     create_index(config)
     return config.cache_path
 
 
 def clean(config):
     """
     Delete a wily cache.
```

### Comparing `wily-1.8.2/wily/commands/build.py` & `wily-1.9.0/wily/commands/build.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/commands/diff.py` & `wily-1.9.0/wily/commands/diff.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/commands/graph.py` & `wily-1.9.0/wily/commands/graph.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/commands/index.py` & `wily-1.9.0/wily/commands/index.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/commands/list_metrics.py` & `wily-1.9.0/wily/commands/list_metrics.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/commands/report.py` & `wily-1.9.0/wily/commands/report.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/operators/__init__.py` & `wily-1.9.0/wily/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/operators/cyclomatic.py` & `wily-1.9.0/wily/operators/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/operators/halstead.py` & `wily-1.9.0/wily/operators/halstead.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/operators/maintainability.py` & `wily-1.9.0/wily/operators/maintainability.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,15 @@
         "max": "C",
         "multi": True,
         "show": False,
         "sort": False,
     }
 
     metrics = (
-        Metric(
-            "rank",
-            "Maintainability Ranking",
-            str,
-            MetricType.Informational,
-            mode,
-        ),
+        Metric("rank", "Maintainability Ranking", str, MetricType.Informational, mode),
         Metric(
             "mi", "Maintainability Index", float, MetricType.AimLow, statistics.mean
         ),
     )
 
     default_metric_index = 1  # MI
```

### Comparing `wily-1.8.2/wily/operators/raw.py` & `wily-1.9.0/wily/operators/raw.py`

 * *Files identical despite different names*

### Comparing `wily-1.8.2/wily/state.py` & `wily-1.9.0/wily/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,7 +202,9 @@
 
     def ensure_exists(self):
         """Ensure that cache directory exists."""
         if not cache.exists(self.config):
             logger.debug("Wily cache not found, creating.")
             cache.create(self.config)
             logger.debug("Created wily cache")
+        else:
+            logger.debug(f"Cache {self.config.cache_path} exists")
```

### Comparing `wily-1.8.2/setup.py` & `wily-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras_require = \
 {":python_version == '3.6'": ['dataclasses']}
 
 entry_points = \
 {'console_scripts': ['wily = wily.__main__:cli']}
 
 setup(name='wily',
-      version='1.8.2',
+      version='1.9.0',
       description='Wily.',
       author='Anthony Shaw',
       author_email='anthonyshaw@apache.org',
       url='https://github.com/tonybaloney/wily',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

