# Comparing `tmp/qtaf-5.6.3.tar.gz` & `tmp/qtaf-5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.6.3.tar", last modified: Mon May 29 03:01:23 2023, max compression
+gzip compressed data, was "qtaf-5.6.4.tar", last modified: Wed Jul  5 13:10:03 2023, max compression
```

## Comparing `qtaf-5.6.3.tar` & `qtaf-5.6.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.520467 qtaf-5.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-29 03:01:09.000000 qtaf-5.6.3/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 03:01:09.000000 qtaf-5.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 03:01:23.520467 qtaf-5.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-29 03:01:09.000000 qtaf-5.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-29 03:01:09.000000 qtaf-5.6.3/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.516466 qtaf-5.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 03:01:09.000000 qtaf-5.6.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-29 03:01:09.000000 qtaf-5.6.3/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.516466 qtaf-5.6.3/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-29 03:01:09.000000 qtaf-5.6.3/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-29 03:01:09.000000 qtaf-5.6.3/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:09.000000 qtaf-5.6.3/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-05-29 03:01:09.000000 qtaf-5.6.3/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.516466 qtaf-5.6.3/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 03:01:23.000000 qtaf-5.6.3/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 03:01:09.000000 qtaf-5.6.3/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 03:01:09.000000 qtaf-5.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 03:01:23.520467 qtaf-5.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-29 03:01:09.000000 qtaf-5.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.520467 qtaf-5.6.3/testbase/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27250 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-05-29 03:01:09.000000 qtaf-5.6.3/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 03:01:23.000000 qtaf-5.6.3/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 03:01:23.520467 qtaf-5.6.3/tuia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 03:01:09.000000 qtaf-5.6.3/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 03:01:22.000000 qtaf-5.6.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.132534 qtaf-5.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-05 13:09:48.000000 qtaf-5.6.4/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 13:09:48.000000 qtaf-5.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-05 13:10:03.132534 qtaf-5.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-05 13:09:48.000000 qtaf-5.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-05 13:09:48.000000 qtaf-5.6.4/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.124534 qtaf-5.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 13:09:48.000000 qtaf-5.6.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 13:09:48.000000 qtaf-5.6.4/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.124534 qtaf-5.6.4/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-05 13:09:48.000000 qtaf-5.6.4/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-05 13:09:48.000000 qtaf-5.6.4/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:09:48.000000 qtaf-5.6.4/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-07-05 13:09:48.000000 qtaf-5.6.4/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.128534 qtaf-5.6.4/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 13:10:03.000000 qtaf-5.6.4/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 13:09:48.000000 qtaf-5.6.4/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 13:09:48.000000 qtaf-5.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:10:03.132534 qtaf-5.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-05 13:09:48.000000 qtaf-5.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.132534 qtaf-5.6.4/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27311 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-07-05 13:09:48.000000 qtaf-5.6.4/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 13:10:02.000000 qtaf-5.6.4/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:10:03.132534 qtaf-5.6.4/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 13:09:48.000000 qtaf-5.6.4/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 13:10:01.000000 qtaf-5.6.4/version.txt
```

### Comparing `qtaf-5.6.3/LICENSE.TXT` & `qtaf-5.6.4/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/PKG-INFO` & `qtaf-5.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.3
+Version: 5.6.4
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.3/README.md` & `qtaf-5.6.4/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/__main__.py` & `qtaf-5.6.4/__main__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qta-manage.py` & `qtaf-5.6.4/qta-manage.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qta_statics/TestReport.xsl` & `qtaf-5.6.4/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qta_statics/TestResult.xsl` & `qtaf-5.6.4/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qta_statics/qta-report.html` & `qtaf-5.6.4/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.4/qtaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.3
+Version: 5.6.4
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.3/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.4/qtaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/qtaf_settings.py` & `qtaf-5.6.4/qtaf_settings.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/setup.py` & `qtaf-5.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/__init__.py` & `qtaf-5.6.4/testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/assertion.py` & `qtaf-5.6.4/testbase/assertion.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     def iter_ast_node(self, node):
         for field, value in ast.iter_fields(node):
             if isinstance(value, list):
                 new_nodes = []
                 for child in value:
                     if isinstance(child, ast.Expr):
                         new_nodes.extend(self.visit(child))
-                    elif isinstance(child, ast.For):
+                    elif isinstance(child, ast.For) or isinstance(child, ast.While) or isinstance(child, ast.If):
                         self.iter_ast_node(child)
                         new_nodes.append(child)
                     else:
                         new_nodes.append(child)
                 setattr(node, field, new_nodes)
             if isinstance(value, ast.Expr):
                 self.visit(value)
```

### Comparing `qtaf-5.6.3/testbase/conf.py` & `qtaf-5.6.4/testbase/conf.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/context.py` & `qtaf-5.6.4/testbase/context.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/datadrive.py` & `qtaf-5.6.4/testbase/datadrive.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/dist.py` & `qtaf-5.6.4/testbase/dist.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/exlib.py` & `qtaf-5.6.4/testbase/exlib.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/loader.py` & `qtaf-5.6.4/testbase/loader.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/logger.py` & `qtaf-5.6.4/testbase/logger.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/management.py` & `qtaf-5.6.4/testbase/management.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/plan.py` & `qtaf-5.6.4/testbase/plan.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/project.py` & `qtaf-5.6.4/testbase/project.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/report.py` & `qtaf-5.6.4/testbase/report.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/resource.py` & `qtaf-5.6.4/testbase/resource.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/retry.py` & `qtaf-5.6.4/testbase/retry.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/runner.py` & `qtaf-5.6.4/testbase/runner.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/serialization.py` & `qtaf-5.6.4/testbase/serialization.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/test.py` & `qtaf-5.6.4/testbase/test.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/testcase.py` & `qtaf-5.6.4/testbase/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/testresult.py` & `qtaf-5.6.4/testbase/testresult.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/testsuite.py` & `qtaf-5.6.4/testbase/testsuite.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/types.py` & `qtaf-5.6.4/testbase/types.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/testbase/util.py` & `qtaf-5.6.4/testbase/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/__init__.py` & `qtaf-5.6.4/tuia/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/_tif.py` & `qtaf-5.6.4/tuia/_tif.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/accessible.py` & `qtaf-5.6.4/tuia/accessible.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/app.py` & `qtaf-5.6.4/tuia/app.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/control.py` & `qtaf-5.6.4/tuia/control.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/env.py` & `qtaf-5.6.4/tuia/env.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/exceptions.py` & `qtaf-5.6.4/tuia/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/filedialog.py` & `qtaf-5.6.4/tuia/filedialog.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/gfcontrols.py` & `qtaf-5.6.4/tuia/gfcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/keyboard.py` & `qtaf-5.6.4/tuia/keyboard.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/mouse.py` & `qtaf-5.6.4/tuia/mouse.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/qpath.py` & `qtaf-5.6.4/tuia/qpath.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/qpathparser.py` & `qtaf-5.6.4/tuia/qpathparser.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/remoteprocessing.py` & `qtaf-5.6.4/tuia/remoteprocessing.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/testcase.py` & `qtaf-5.6.4/tuia/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/uiacontrols.py` & `qtaf-5.6.4/tuia/uiacontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/util.py` & `qtaf-5.6.4/tuia/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/webcontrols.py` & `qtaf-5.6.4/tuia/webcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/wincontrols.py` & `qtaf-5.6.4/tuia/wincontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.3/tuia/wintypes.py` & `qtaf-5.6.4/tuia/wintypes.py`

 * *Files identical despite different names*

