# Comparing `tmp/cypherdataframe-0.3.4.tar.gz` & `tmp/cypherdataframe-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypherdataframe-0.3.4.tar", last modified: Wed Jul  5 19:08:57 2023, max compression
+gzip compressed data, was "cypherdataframe-0.3.5.tar", last modified: Wed Jul  5 19:36:16 2023, max compression
```

## Comparing `cypherdataframe-0.3.4.tar` & `cypherdataframe-0.3.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.875206 cypherdataframe-0.3.4/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:08:57.874772 cypherdataframe-0.3.4/PKG-INFO
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.845126 cypherdataframe-0.3.4/cypherdataframe/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.4/cypherdataframe/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.4/cypherdataframe/branch_maker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.4/cypherdataframe/config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     9296 2023-07-05 19:05:17.000000 cypherdataframe-0.3.4/cypherdataframe/cypher.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.850373 cypherdataframe-0.3.4/cypherdataframe/garner_domain/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/BranchMaker.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.852179 cypherdataframe-0.3.4/cypherdataframe/garner_domain/logistics/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/logistics/TransferBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/logistics/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.853268 cypherdataframe-0.3.4/cypherdataframe/garner_domain/measure/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      634 2023-06-09 21:00:14.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/measure/MeasureBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/measure/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/properties_defaults.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.854353 cypherdataframe-0.3.4/cypherdataframe/garner_domain/queries/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/queries/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.855593 cypherdataframe-0.3.4/cypherdataframe/garner_domain/reference/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/reference/ReferenceBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/reference/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.858653 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/AttainedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/ForecastedBranch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.862971 cypherdataframe-0.3.4/cypherdataframe/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.4/cypherdataframe/model/Branch.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.4/cypherdataframe/model/Config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.4/cypherdataframe/model/LabelNode.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.4/cypherdataframe/model/Property.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.4/cypherdataframe/model/Query.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.4/cypherdataframe/model/QueryAccumulation.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.4/cypherdataframe/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.4/cypherdataframe/testfunctions.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.848825 cypherdataframe-0.3.4/cypherdataframe.egg-info/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:08:57.000000 cypherdataframe-0.3.4/cypherdataframe.egg-info/PKG-INFO
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-05 19:08:57.000000 cypherdataframe-0.3.4/cypherdataframe.egg-info/SOURCES.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-05 19:08:57.000000 cypherdataframe-0.3.4/cypherdataframe.egg-info/dependency_links.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-05 19:08:57.000000 cypherdataframe-0.3.4/cypherdataframe.egg-info/requires.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-05 19:08:57.000000 cypherdataframe-0.3.4/cypherdataframe.egg-info/top_level.txt
--rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-05 19:08:57.875378 cypherdataframe-0.3.4/setup.cfg
--rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-05 19:07:50.000000 cypherdataframe-0.3.4/setup.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.867603 cypherdataframe-0.3.4/tests/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.4/tests/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.4/tests/branch_maker_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.4/tests/conftest.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.4/tests/cypher_integration_test.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.868232 cypherdataframe-0.3.4/tests/fixtures/
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.4/tests/fixtures/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.871269 cypherdataframe-0.3.4/tests/fixtures/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.4/tests/fixtures/model/Branch_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.4/tests/fixtures/model/Node_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.4/tests/fixtures/model/Property_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.4/tests/fixtures/model/Query_fixture.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.4/tests/fixtures/model/__init__.py
-drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:08:57.874333 cypherdataframe-0.3.4/tests/model/
--rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.4/tests/model/Branch_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.4/tests/model/Node_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.4/tests/model/Query_test.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.4/tests/model/__init__.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.4/tests/test_config.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.4/tests/test_testfunctions.py
--rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.4/tests/tsest_ignorefunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.091600 cypherdataframe-0.3.5/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:36:16.091345 cypherdataframe-0.3.5/PKG-INFO
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.078004 cypherdataframe-0.3.5/cypherdataframe/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-09 19:02:36.000000 cypherdataframe-0.3.5/cypherdataframe/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      734 2023-05-05 22:58:23.000000 cypherdataframe-0.3.5/cypherdataframe/branch_maker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      287 2022-03-09 18:38:14.000000 cypherdataframe-0.3.5/cypherdataframe/config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     9529 2023-07-05 19:33:52.000000 cypherdataframe-0.3.5/cypherdataframe/cypher.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.080171 cypherdataframe-0.3.5/cypherdataframe/garner_domain/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1340 2023-06-29 20:43:49.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/BranchMaker.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-03-02 19:12:20.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.080758 cypherdataframe-0.3.5/cypherdataframe/garner_domain/logistics/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:02:39.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/logistics/TransferBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/logistics/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.081259 cypherdataframe-0.3.5/cypherdataframe/garner_domain/measure/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      634 2023-06-09 21:00:14.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/measure/MeasureBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/measure/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2389 2023-06-29 20:46:57.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/properties_defaults.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.081766 cypherdataframe-0.3.5/cypherdataframe/garner_domain/queries/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      919 2023-06-29 20:44:47.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-05 20:18:52.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/queries/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.082627 cypherdataframe-0.3.5/cypherdataframe/garner_domain/reference/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      613 2023-06-29 21:20:43.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/reference/ReferenceBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-05-18 14:37:50.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/reference/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.084407 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      653 2023-06-29 21:17:38.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      606 2023-06-29 21:18:56.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/AttainedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      658 2023-06-29 21:17:38.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      615 2023-06-29 21:18:10.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/ForecastedBranch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2023-06-29 20:45:12.000000 cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.086391 cypherdataframe-0.3.5/cypherdataframe/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2213 2023-06-15 17:59:52.000000 cypherdataframe-0.3.5/cypherdataframe/model/Branch.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      190 2022-03-05 20:10:55.000000 cypherdataframe-0.3.5/cypherdataframe/model/Config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      829 2023-05-05 22:58:23.000000 cypherdataframe-0.3.5/cypherdataframe/model/LabelNode.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      373 2023-05-05 23:13:15.000000 cypherdataframe-0.3.5/cypherdataframe/model/Property.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2561 2023-05-19 01:46:51.000000 cypherdataframe-0.3.5/cypherdataframe/model/Query.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     2658 2023-06-29 21:21:37.000000 cypherdataframe-0.3.5/cypherdataframe/model/QueryAccumulation.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2022-03-09 19:02:36.000000 cypherdataframe-0.3.5/cypherdataframe/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       88 2023-06-30 15:18:00.000000 cypherdataframe-0.3.5/cypherdataframe/testfunctions.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.079377 cypherdataframe-0.3.5/cypherdataframe.egg-info/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      182 2023-07-05 19:36:16.000000 cypherdataframe-0.3.5/cypherdataframe.egg-info/PKG-INFO
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1947 2023-07-05 19:36:16.000000 cypherdataframe-0.3.5/cypherdataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        1 2023-07-05 19:36:16.000000 cypherdataframe-0.3.5/cypherdataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       31 2023-07-05 19:36:16.000000 cypherdataframe-0.3.5/cypherdataframe.egg-info/requires.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       16 2023-07-05 19:36:16.000000 cypherdataframe-0.3.5/cypherdataframe.egg-info/top_level.txt
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       38 2023-07-05 19:36:16.091688 cypherdataframe-0.3.5/setup.cfg
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      772 2023-07-05 19:36:04.000000 cypherdataframe-0.3.5/setup.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.088253 cypherdataframe-0.3.5/tests/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-04 01:04:28.000000 cypherdataframe-0.3.5/tests/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1262 2022-03-09 18:38:44.000000 cypherdataframe-0.3.5/tests/branch_maker_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      349 2022-03-08 00:49:49.000000 cypherdataframe-0.3.5/tests/conftest.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      407 2022-03-09 18:37:32.000000 cypherdataframe-0.3.5/tests/cypher_integration_test.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.088533 cypherdataframe-0.3.5/tests/fixtures/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.5/tests/fixtures/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.089869 cypherdataframe-0.3.5/tests/fixtures/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      267 2022-03-09 18:37:32.000000 cypherdataframe-0.3.5/tests/fixtures/model/Branch_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      409 2022-03-09 18:38:14.000000 cypherdataframe-0.3.5/tests/fixtures/model/Node_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1026 2022-03-09 18:37:32.000000 cypherdataframe-0.3.5/tests/fixtures/model/Property_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      279 2022-03-09 18:37:44.000000 cypherdataframe-0.3.5/tests/fixtures/model/Query_fixture.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.5/tests/fixtures/model/__init__.py
+drwxr-xr-x   0 avanderploeg   (501) staff       (20)        0 2023-07-05 19:36:16.091038 cypherdataframe-0.3.5/tests/model/
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      163 2022-03-07 02:21:55.000000 cypherdataframe-0.3.5/tests/model/Branch_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      201 2022-03-09 18:22:56.000000 cypherdataframe-0.3.5/tests/model/Node_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      110 2023-05-05 21:20:32.000000 cypherdataframe-0.3.5/tests/model/Query_test.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)        0 2022-03-07 02:21:55.000000 cypherdataframe-0.3.5/tests/model/__init__.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)      330 2022-03-09 18:38:44.000000 cypherdataframe-0.3.5/tests/test_config.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)       97 2022-03-08 01:28:36.000000 cypherdataframe-0.3.5/tests/test_testfunctions.py
+-rw-r--r--   0 avanderploeg   (501) staff       (20)     1345 2023-05-05 23:26:35.000000 cypherdataframe-0.3.5/tests/tsest_ignorefunctions.py
```

### Comparing `cypherdataframe-0.3.4/cypherdataframe/branch_maker.py` & `cypherdataframe-0.3.5/cypherdataframe/branch_maker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/cypher.py` & `cypherdataframe-0.3.5/cypherdataframe/cypher.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,14 +216,18 @@
                 continue
 
         data_extracted_time = time.time()
         df.to_csv(
             f"{save_directory}/{table_name_root}_{current_chunk}.csv",
             index=False
         )
+        df.to_feather(
+            f"{save_directory}/{table_name_root}_{current_chunk}.feather",
+            index=False
+        )
         data_stored_time = time.time()
         df_keys = df[df.columns[0]].nunique()
         df_rows = df.shape[0]
 
         __add_to_meta(
             meta_path,
             increment=current_chunk,
@@ -295,21 +299,24 @@
 
 
 def gather_chunks_from_dir(gather_to_dir: str, read_directory: str, table_name_root: str):
     if os.path.isdir(read_directory):
         df_list = []
         for file_name in os.listdir(read_directory):
             file_size = os.path.getsize(f"{read_directory}/{file_name}")
-            if "csv" in file_name \
-                    and "-gathered.csv" not in file_name \
-                    and "meta.csv" not in file_name \
+            if ".feather" in file_name \
+                    and "-gathered.feather" not in file_name \
                     and file_size > 10:
-                df_list.append(pd.read_csv(f"{read_directory}/{file_name}"))
+                df_list.append(pd.read_feather(f"{read_directory}/{file_name}"))
         if len(df_list) > 0:
             df = pd.concat(df_list).reset_index(drop=True)
             if not os.path.isdir(gather_to_dir):
                 os.makedirs(gather_to_dir)
 
             df.to_csv(
                 f"{gather_to_dir}/{table_name_root}-gathered.csv",
                 index=False
             )
+            df.to_feather(
+                f"{gather_to_dir}/{table_name_root}-gathered.feathered",
+                index=False
+            )
```

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/BranchMaker.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/BranchMaker.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/logistics/TransferBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/logistics/TransferBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/measure/MeasureBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/measure/MeasureBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/properties_defaults.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/properties_defaults.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/queries/LogisticsTableQuery.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/reference/ReferenceBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/reference/ReferenceBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/AttainedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/AttainedBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/AttainedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/ForecastedArchivedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/garner_domain/status/ForecastedBranch.py` & `cypherdataframe-0.3.5/cypherdataframe/garner_domain/status/ForecastedBranch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/model/Branch.py` & `cypherdataframe-0.3.5/cypherdataframe/model/Branch.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/model/LabelNode.py` & `cypherdataframe-0.3.5/cypherdataframe/model/LabelNode.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/model/Query.py` & `cypherdataframe-0.3.5/cypherdataframe/model/Query.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe/model/QueryAccumulation.py` & `cypherdataframe-0.3.5/cypherdataframe/model/QueryAccumulation.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/cypherdataframe.egg-info/SOURCES.txt` & `cypherdataframe-0.3.5/cypherdataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/setup.py` & `cypherdataframe-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             'cypherdataframe.garner_domain.logistics',
             'cypherdataframe.garner_domain.measure',
             'cypherdataframe.garner_domain.queries',
             'cypherdataframe.garner_domain.reference',
             'cypherdataframe.garner_domain.status'
         ]
     ),
-    version='0.3.4',
+    version='0.3.5',
     description='Cypher Query to df Toolkit',
     author='Attila Vanderploeg',
     license='MIT',
     install_requires=['py2neo>=2021.2.3', 'dacite>=1.6.0'],
     setup_requires=[],
     tests_require=[],
     test_suite='tests',
```

### Comparing `cypherdataframe-0.3.4/tests/branch_maker_test.py` & `cypherdataframe-0.3.5/tests/branch_maker_test.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/tests/fixtures/model/Property_fixture.py` & `cypherdataframe-0.3.5/tests/fixtures/model/Property_fixture.py`

 * *Files identical despite different names*

### Comparing `cypherdataframe-0.3.4/tests/tsest_ignorefunctions.py` & `cypherdataframe-0.3.5/tests/tsest_ignorefunctions.py`

 * *Files identical despite different names*

