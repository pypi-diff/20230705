# Comparing `tmp/acceldata_sdk-2.7.0.tar.gz` & `tmp/acceldata_sdk-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_sdk-2.7.0.tar", last modified: Fri Jun 23 12:29:15 2023, max compression
+gzip compressed data, was "acceldata_sdk-2.7.1.tar", last modified: Wed Jul  5 11:36:01 2023, max compression
```

## Comparing `acceldata_sdk-2.7.0.tar` & `acceldata_sdk-2.7.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992984 acceldata_sdk-2.7.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      140 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/DATASOURCE_README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23249 2023-06-23 12:29:15.992819 acceldata_sdk-2.7.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18634 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.984760 acceldata_sdk-2.7.0/acceldata_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     8561 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/common.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1966 2023-06-14 05:09:30.000000 acceldata_sdk-2.7.0/acceldata_sdk/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/errors.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.986852 acceldata_sdk-2.7.0/acceldata_sdk/events/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      373 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/generic_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/job_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      455 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/log_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1061 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/events/span_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.989860 acceldata_sdk-2.7.0/acceldata_sdk/models/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6504 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/assetType.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     9991 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/connection.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3523 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/create_asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     9033 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/datasource.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10010 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/dqrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4157 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1136 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/notifications.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    22692 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/pipeline.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2782 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/profile.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11289 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/reconcillationrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/rule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7453 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/ruleExecutionResult.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2254 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     8048 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/span_context.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/acceldata_sdk/models/tags.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15627 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    42521 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/acceldata_sdk/torch_http_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.985734 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23249 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1811 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2023-06-23 12:29:15.000000 acceldata_sdk-2.7.0/acceldata_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.990033 acceldata_sdk-2.7.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.981385 acceldata_sdk-2.7.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.981437 acceldata_sdk-2.7.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.991553 acceldata_sdk-2.7.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme_datasource.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/readme_pipeline.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992265 acceldata_sdk-2.7.0/integration_tests/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-06-23 12:29:15.992416 acceldata_sdk-2.7.0/integration_tests/.pytest_cache/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      302 2023-06-14 11:07:12.000000 acceldata_sdk-2.7.0/integration_tests/.pytest_cache/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3791 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.0/integration_tests/test_ds_assets.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_pipelines.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3945 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.0/integration_tests/test_policy.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2023-06-23 12:29:15.993020 acceldata_sdk-2.7.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2023-06-23 05:58:49.000000 acceldata_sdk-2.7.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.955822 acceldata_sdk-2.7.1/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      140 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/DATASOURCE_README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23201 2023-07-05 11:36:01.955648 acceldata_sdk-2.7.1/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18586 2023-07-05 11:23:58.000000 acceldata_sdk-2.7.1/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.947668 acceldata_sdk-2.7.1/acceldata_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8561 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/common.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1966 2023-06-14 05:09:30.000000 acceldata_sdk-2.7.1/acceldata_sdk/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/errors.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.949428 acceldata_sdk-2.7.1/acceldata_sdk/events/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/events/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      373 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/events/generic_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/events/job_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      455 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/events/log_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1061 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/events/span_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.952624 acceldata_sdk-2.7.1/acceldata_sdk/models/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6504 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/assetType.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     9991 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/connection.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3523 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/create_asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     9033 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/datasource.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10010 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/dqrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4157 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1136 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/notifications.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    22800 2023-07-05 11:23:23.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/pipeline.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2782 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/profile.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11289 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/reconcillationrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/rule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7453 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/ruleExecutionResult.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2254 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8048 2023-07-05 03:56:25.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/span_context.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/acceldata_sdk/models/tags.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15627 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.1/acceldata_sdk/torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    42521 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.1/acceldata_sdk/torch_http_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.948690 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23201 2023-07-05 11:36:01.000000 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1811 2023-07-05 11:36:01.000000 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2023-07-05 11:36:01.000000 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2023-07-05 11:36:01.000000 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2023-07-05 11:36:01.000000 acceldata_sdk-2.7.1/acceldata_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.952780 acceldata_sdk-2.7.1/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.944002 acceldata_sdk-2.7.1/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.944103 acceldata_sdk-2.7.1/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.954306 acceldata_sdk-2.7.1/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/readme.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/readme_datasource.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/readme_pipeline.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.events.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.models.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2023-06-14 05:00:43.000000 acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.1/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.955103 acceldata_sdk-2.7.1/integration_tests/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2023-07-05 11:36:01.955254 acceldata_sdk-2.7.1/integration_tests/.pytest_cache/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      302 2023-06-14 11:07:12.000000 acceldata_sdk-2.7.1/integration_tests/.pytest_cache/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2023-07-05 09:07:02.000000 acceldata_sdk-2.7.1/integration_tests/test_constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3791 2023-06-14 05:00:44.000000 acceldata_sdk-2.7.1/integration_tests/test_ds_assets.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2023-07-05 09:07:02.000000 acceldata_sdk-2.7.1/integration_tests/test_pipelines.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3945 2023-06-23 09:12:55.000000 acceldata_sdk-2.7.1/integration_tests/test_policy.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2023-07-05 11:36:01.955859 acceldata_sdk-2.7.1/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2023-07-05 11:26:03.000000 acceldata_sdk-2.7.1/setup.py
```

### Comparing `acceldata_sdk-2.7.0/DATASOURCE_README.md` & `acceldata_sdk-2.7.1/DATASOURCE_README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/LICENCE.txt` & `acceldata_sdk-2.7.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/PKG-INFO` & `acceldata_sdk-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 2.7.0
+Version: 2.7.1
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,41 +40,38 @@
 
 ```
 
 ## Pipeline API 
 There are various pipeline APIs are supported through Acceldata SDK. Pipeline APIs like create pipeline, add jobs and spans, initiate pipeline run et cetera. Acceldata sdk is able to send various event during span life cycle. Hence, Acceldata sdk has full control over the pipelines.
 
 ##### Create Pipeline And Job and span to bound the job
-Pipeline represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
+`Pipeline` represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
 </br>
-Job Node or Process Node represents an entity that does some job in the ETL workflow. From this representation, Job’s input is some assets or some other Jobs, and output is few other assets or few other Jobs.
+`Job Node` or `Process Node` represents an entity that does some job in the ETL workflow. From this representation, `Job’s input` is some assets or some other Jobs, and output is few other assets or few other Jobs.
 Torch will use the set of Jobs definition in the workflow to create the Lineage, and also track version changes for the Pipeline.
 
-To create pipeline and jobs, first create creation object with required parameter. And with use of supported methods by sdk, can do corresponding operation on torch server side.
-
-Acceldata sdk provides CreateJob class which need to be passed to create_job function as a parameter to create a job.
+Acceldata sdk provides `CreateJob` class which need to be passed to `create_job` function as a parameter to create a job.
 
 Params for `CreateJob`:
 
-`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.
+`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.<br/>
 `name`: name of the job. It is a mandatory parameter.
 
 #### NOTE: This changed in 2.4.1 release
 
-`pipeline_run_id`: id of the pipeline_run for which you want to add a job.It is a mandatory parameter if job is being created using pipeline. Its is not needed if job is being created using pipeline_run.
-
-`description`: description of the job
+`pipeline_run_id`: id of the pipeline_run for which you want to add a job. It is a mandatory parameter if `job` is being created using `pipeline`. Its is not needed if job is being created using `pipeline_run`.<br/>
+`description`: description of the job </br>
 `inputs`: (list[Node]) input for the job. This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
 `outputs`: (list[Node]) output for the job.This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
-`meta`: Metadata of the Job
-`context`: context of the job
-`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter
-`span_uid`: (String) This is uid of new span to be created. This is a manadatory parameter if bounded_by_span is set to True
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
+`meta`: Metadata of the Job</br>
+`context`: context of the job</br>
+`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter.
+`span_uid`: (String) This is uid of new span to be created. This is a mandatory parameter if bounded_by_span is set to True.
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 from acceldata_sdk.models.job import CreateJob, JobMetadata, Node
 from acceldata_sdk.models.pipeline import CreatePipeline, PipelineMetadata, PipelineRunResult, PipelineRunStatus
 
 # Create pipeline
@@ -85,14 +82,15 @@
     meta=PipelineMetadata('Vaishvik', 'acceldata_sdk_code', '...'),
     context={'key1': 'value1'}
 )
 torch_client = TorchClient(url="https://torch.acceldata.local", access_key="*******",
                           secret_key="******************************",do_version_check=False)
 pipeline_response = torch_client.create_pipeline(pipeline=pipeline)
 pipeline_run = pipeline_response.create_pipeline_run()
+
 # Create a job using pipeline object.
 # Passing of pipeline_run_id is mandatory
 job = CreateJob(
     uid='monthly_sales_aggregate',
     name='Monthly Sales Aggregate',
     description='Generates the monthly sales aggregate tables for the complete year',
     inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
@@ -103,42 +101,41 @@
     pipeline_run_id=pipeline_run.id,
     span_uid="test_shubh"
 )
 job_response = pipeline_response.create_job(job)
 
 # Create a job using pipeline_run object.
 # Passing of pipeline_run_id is not needed
-
 job = CreateJob(
-    uid='monthly_sales_aggregate_r',
-    name='Monthly Sales Aggregate',
-    description='Generates the monthly sales aggregate tables for the complete year',
-    inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
-    outputs=[Node(job_uid='job2_uid')],
-    meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
-    context={'key21': 'value21'}
+        uid='monthly_sales_aggregate',
+        name='Monthly Sales Aggregate',
+        description='Generates the monthly sales aggregate tables for the complete year',
+        inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
+        outputs=[Node(job_uid='job2_uid')],
+        meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
+        context={'key21': 'value21'}
 )
 job_response_using_run = pipeline_run.create_job(job)
 ```
 ##### Create Pipeline Run And Generate Spans And Send Span Events
 
-Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A Span is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
+Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A `Span` is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
 
 Acceldata sdk also has support for create new pipeline run, add spans in it. During the span life cycle, sdk is able to send some customs and standard span events to collect pipeline run metrics for observability.
 
-Params for create_span function which is available under a pipeline_run
+Params for `create_span` function which is available under a `pipeline_run`
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`associatedJobUids`: List of job uids with which the span needs to be associated with.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`associatedJobUids`: List of job uids with which the span needs to be associated with.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 
-Params for create_child_span function which is available under span_context. This is used to create hierarchy of span by creating a span under another span
+Params for `create_child_span` function which is available under `span_context`. This is used to create hierarchy of span by creating a span under another span
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 `associatedJobUids`: List of job uids with which the span needs to be associated with.
 ```python
 
 from acceldata_sdk.events.generic_event import GenericEvent
 from datetime import datetime
 
 # create a pipeline run of the pipeline
@@ -195,17 +192,17 @@
 ```
 ##### Get Pipeline Run with a particular pipeline run id
 Acceldata sdk can get a pipeline run of the pipeline with a particular pipeline run id. With use of the pipeline run 
 instance, user can continue ETL pipeline and add spans, jobs, events too. Hence, Acceldata sdk has complete access on the torch pipeline service.
 
 Params for `get_pipeline_run`:
 
-`pipeline_run_id`: run id of the pipeline run
-`continuation_id`: continuation id of the pipeline run
-`pipeline_id`: id of the pipeline to which the run belongs to
+`pipeline_run_id`: run id of the pipeline run<br/>
+`continuation_id`: continuation id of the pipeline run<br/>
+`pipeline_id`: id of the pipeline to which the run belongs to<br/>
 ```python
 pipeline_run = torch_client.get_pipeline_run(pipeline_run_id=pipeline_run_id)
 pipeline = torch_client.get_pipeline(pipeline_id=pipeline_id)
 pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id, pipeline_id=pipeline.id)
 pipeline_run = pipeline.get_run(continuation_id=continuation_id)
 ```
```

### Comparing `acceldata_sdk-2.7.0/README.md` & `acceldata_sdk-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,41 +23,38 @@
 
 ```
 
 ## Pipeline API 
 There are various pipeline APIs are supported through Acceldata SDK. Pipeline APIs like create pipeline, add jobs and spans, initiate pipeline run et cetera. Acceldata sdk is able to send various event during span life cycle. Hence, Acceldata sdk has full control over the pipelines.
 
 ##### Create Pipeline And Job and span to bound the job
-Pipeline represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
+`Pipeline` represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
 </br>
-Job Node or Process Node represents an entity that does some job in the ETL workflow. From this representation, Job’s input is some assets or some other Jobs, and output is few other assets or few other Jobs.
+`Job Node` or `Process Node` represents an entity that does some job in the ETL workflow. From this representation, `Job’s input` is some assets or some other Jobs, and output is few other assets or few other Jobs.
 Torch will use the set of Jobs definition in the workflow to create the Lineage, and also track version changes for the Pipeline.
 
-To create pipeline and jobs, first create creation object with required parameter. And with use of supported methods by sdk, can do corresponding operation on torch server side.
-
-Acceldata sdk provides CreateJob class which need to be passed to create_job function as a parameter to create a job.
+Acceldata sdk provides `CreateJob` class which need to be passed to `create_job` function as a parameter to create a job.
 
 Params for `CreateJob`:
 
-`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.
+`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.<br/>
 `name`: name of the job. It is a mandatory parameter.
 
 #### NOTE: This changed in 2.4.1 release
 
-`pipeline_run_id`: id of the pipeline_run for which you want to add a job.It is a mandatory parameter if job is being created using pipeline. Its is not needed if job is being created using pipeline_run.
-
-`description`: description of the job
+`pipeline_run_id`: id of the pipeline_run for which you want to add a job. It is a mandatory parameter if `job` is being created using `pipeline`. Its is not needed if job is being created using `pipeline_run`.<br/>
+`description`: description of the job </br>
 `inputs`: (list[Node]) input for the job. This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
 `outputs`: (list[Node]) output for the job.This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
-`meta`: Metadata of the Job
-`context`: context of the job
-`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter
-`span_uid`: (String) This is uid of new span to be created. This is a manadatory parameter if bounded_by_span is set to True
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
+`meta`: Metadata of the Job</br>
+`context`: context of the job</br>
+`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter.
+`span_uid`: (String) This is uid of new span to be created. This is a mandatory parameter if bounded_by_span is set to True.
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 from acceldata_sdk.models.job import CreateJob, JobMetadata, Node
 from acceldata_sdk.models.pipeline import CreatePipeline, PipelineMetadata, PipelineRunResult, PipelineRunStatus
 
 # Create pipeline
@@ -68,14 +65,15 @@
     meta=PipelineMetadata('Vaishvik', 'acceldata_sdk_code', '...'),
     context={'key1': 'value1'}
 )
 torch_client = TorchClient(url="https://torch.acceldata.local", access_key="*******",
                           secret_key="******************************",do_version_check=False)
 pipeline_response = torch_client.create_pipeline(pipeline=pipeline)
 pipeline_run = pipeline_response.create_pipeline_run()
+
 # Create a job using pipeline object.
 # Passing of pipeline_run_id is mandatory
 job = CreateJob(
     uid='monthly_sales_aggregate',
     name='Monthly Sales Aggregate',
     description='Generates the monthly sales aggregate tables for the complete year',
     inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
@@ -86,42 +84,41 @@
     pipeline_run_id=pipeline_run.id,
     span_uid="test_shubh"
 )
 job_response = pipeline_response.create_job(job)
 
 # Create a job using pipeline_run object.
 # Passing of pipeline_run_id is not needed
-
 job = CreateJob(
-    uid='monthly_sales_aggregate_r',
-    name='Monthly Sales Aggregate',
-    description='Generates the monthly sales aggregate tables for the complete year',
-    inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
-    outputs=[Node(job_uid='job2_uid')],
-    meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
-    context={'key21': 'value21'}
+        uid='monthly_sales_aggregate',
+        name='Monthly Sales Aggregate',
+        description='Generates the monthly sales aggregate tables for the complete year',
+        inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
+        outputs=[Node(job_uid='job2_uid')],
+        meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
+        context={'key21': 'value21'}
 )
 job_response_using_run = pipeline_run.create_job(job)
 ```
 ##### Create Pipeline Run And Generate Spans And Send Span Events
 
-Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A Span is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
+Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A `Span` is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
 
 Acceldata sdk also has support for create new pipeline run, add spans in it. During the span life cycle, sdk is able to send some customs and standard span events to collect pipeline run metrics for observability.
 
-Params for create_span function which is available under a pipeline_run
+Params for `create_span` function which is available under a `pipeline_run`
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`associatedJobUids`: List of job uids with which the span needs to be associated with.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`associatedJobUids`: List of job uids with which the span needs to be associated with.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 
-Params for create_child_span function which is available under span_context. This is used to create hierarchy of span by creating a span under another span
+Params for `create_child_span` function which is available under `span_context`. This is used to create hierarchy of span by creating a span under another span
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 `associatedJobUids`: List of job uids with which the span needs to be associated with.
 ```python
 
 from acceldata_sdk.events.generic_event import GenericEvent
 from datetime import datetime
 
 # create a pipeline run of the pipeline
@@ -178,17 +175,17 @@
 ```
 ##### Get Pipeline Run with a particular pipeline run id
 Acceldata sdk can get a pipeline run of the pipeline with a particular pipeline run id. With use of the pipeline run 
 instance, user can continue ETL pipeline and add spans, jobs, events too. Hence, Acceldata sdk has complete access on the torch pipeline service.
 
 Params for `get_pipeline_run`:
 
-`pipeline_run_id`: run id of the pipeline run
-`continuation_id`: continuation id of the pipeline run
-`pipeline_id`: id of the pipeline to which the run belongs to
+`pipeline_run_id`: run id of the pipeline run<br/>
+`continuation_id`: continuation id of the pipeline run<br/>
+`pipeline_id`: id of the pipeline to which the run belongs to<br/>
 ```python
 pipeline_run = torch_client.get_pipeline_run(pipeline_run_id=pipeline_run_id)
 pipeline = torch_client.get_pipeline(pipeline_id=pipeline_id)
 pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id, pipeline_id=pipeline.id)
 pipeline_run = pipeline.get_run(continuation_id=continuation_id)
 ```
```

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/client.py` & `acceldata_sdk-2.7.1/acceldata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/common.py` & `acceldata_sdk-2.7.1/acceldata_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/constants.py` & `acceldata_sdk-2.7.1/acceldata_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/events/job_events.py` & `acceldata_sdk-2.7.1/acceldata_sdk/events/job_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/events/span_event.py` & `acceldata_sdk-2.7.1/acceldata_sdk/events/span_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/asset.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/assetType.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/assetType.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/connection.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/connection.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/create_asset.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/create_asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/datasource.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/dqrule.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/dqrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/job.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/notifications.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/notifications.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/pipeline.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,39 +199,40 @@
         Description:
             used to create job for any pipeline run
         :return: Job class instance of created job        """
         if job.uid is None or job.name is None:
             raise Exception('To create a job job uid and name are required')
         payload = self._convert_job_to_dict(job)
         res = self.client.create_job(payload, self.pipelineId)
-        if job.bounded_by_span and job.span_uid is not None:
-            associated_job_uids = [job.uid]
-            span_uid_temp = job.span_uid
-            # Get root span to create child span under
-            parent_span_context = self.get_root_span()
-            if parent_span_context is not None:
-                # Create child span under root span
-                span_context = parent_span_context.create_child_span(
-                    uid=span_uid_temp,
-                    context_data={
-                        'time': str(datetime.now())
-                    },
-                    associatedJobUids=associated_job_uids
-                )
+        if job.bounded_by_span:
+            if job.span_uid is not None:
+                associated_job_uids = [job.uid]
+                span_uid_temp = job.span_uid
+                # Get root span to create child span under
+                parent_span_context = self.get_root_span()
+                if parent_span_context is not None:
+                    # Create child span under root span
+                    span_context = parent_span_context.create_child_span(
+                        uid=span_uid_temp,
+                        context_data={
+                            'time': str(datetime.now())
+                        },
+                        associatedJobUids=associated_job_uids
+                    )
+                else:
+                    # Create root span under pipeline_run as root span doesn't exist
+                    self.create_span(
+                        uid=span_uid_temp,
+                        context_data={
+                            'time': str(datetime.now())
+                        },
+                        associatedJobUids=associated_job_uids
+                    )
             else:
-                # Create root span under pipeline_run as root span doesn't exist
-                self.create_span(
-                    uid=span_uid_temp,
-                    context_data={
-                        'time': str(datetime.now())
-                    },
-                    associatedJobUids=associated_job_uids
-                )
-        else:
-            raise Exception('To create a span span_uid is required')
+                raise Exception('To create a span span_uid is required')
         return res
 
     # convert pipeline run to dict type
     def _convert_pipeline_run_to_dict(self, pipeline_run=None):
         """
             Description:
                 Convert PipelineRun class instance to dict type
```

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/profile.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/profile.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/reconcillationrule.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/reconcillationrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/rule.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/rule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/ruleExecutionResult.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/ruleExecutionResult.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/span.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/span_context.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/span_context.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/models/tags.py` & `acceldata_sdk-2.7.1/acceldata_sdk/models/tags.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/torch_client.py` & `acceldata_sdk-2.7.1/acceldata_sdk/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk/torch_http_client.py` & `acceldata_sdk-2.7.1/acceldata_sdk/torch_http_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk.egg-info/PKG-INFO` & `acceldata_sdk-2.7.1/acceldata_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata-sdk
-Version: 2.7.0
+Version: 2.7.1
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,41 +40,38 @@
 
 ```
 
 ## Pipeline API 
 There are various pipeline APIs are supported through Acceldata SDK. Pipeline APIs like create pipeline, add jobs and spans, initiate pipeline run et cetera. Acceldata sdk is able to send various event during span life cycle. Hence, Acceldata sdk has full control over the pipelines.
 
 ##### Create Pipeline And Job and span to bound the job
-Pipeline represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
+`Pipeline` represents the ETL pipeline in its entirety and will contain Asset nodes and Jobs associated. The complete pipeline definition forms the Lineage graph for all the data assets.
 </br>
-Job Node or Process Node represents an entity that does some job in the ETL workflow. From this representation, Job’s input is some assets or some other Jobs, and output is few other assets or few other Jobs.
+`Job Node` or `Process Node` represents an entity that does some job in the ETL workflow. From this representation, `Job’s input` is some assets or some other Jobs, and output is few other assets or few other Jobs.
 Torch will use the set of Jobs definition in the workflow to create the Lineage, and also track version changes for the Pipeline.
 
-To create pipeline and jobs, first create creation object with required parameter. And with use of supported methods by sdk, can do corresponding operation on torch server side.
-
-Acceldata sdk provides CreateJob class which need to be passed to create_job function as a parameter to create a job.
+Acceldata sdk provides `CreateJob` class which need to be passed to `create_job` function as a parameter to create a job.
 
 Params for `CreateJob`:
 
-`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.
+`uid`: uid of the job. It should be unique for the job. It is a mandatory parameter.<br/>
 `name`: name of the job. It is a mandatory parameter.
 
 #### NOTE: This changed in 2.4.1 release
 
-`pipeline_run_id`: id of the pipeline_run for which you want to add a job.It is a mandatory parameter if job is being created using pipeline. Its is not needed if job is being created using pipeline_run.
-
-`description`: description of the job
+`pipeline_run_id`: id of the pipeline_run for which you want to add a job. It is a mandatory parameter if `job` is being created using `pipeline`. Its is not needed if job is being created using `pipeline_run`.<br/>
+`description`: description of the job </br>
 `inputs`: (list[Node]) input for the job. This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
 `outputs`: (list[Node]) output for the job.This can be uid of an asset specified using asset_uid parameter of Node object
-        or it can be uid of another job specified using job_uid parameter of Node object.
-`meta`: Metadata of the Job
-`context`: context of the job
-`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter
-`span_uid`: (String) This is uid of new span to be created. This is a manadatory parameter if bounded_by_span is set to True
+        or it can be uid of another job specified using job_uid parameter of Node object.</br>
+`meta`: Metadata of the Job</br>
+`context`: context of the job</br>
+`bounded_by_span`: (Boolean) This has to be set to True if the job has to be bounded with a span. Default value is false. It is an optional parameter.
+`span_uid`: (String) This is uid of new span to be created. This is a mandatory parameter if bounded_by_span is set to True.
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 from acceldata_sdk.models.job import CreateJob, JobMetadata, Node
 from acceldata_sdk.models.pipeline import CreatePipeline, PipelineMetadata, PipelineRunResult, PipelineRunStatus
 
 # Create pipeline
@@ -85,14 +82,15 @@
     meta=PipelineMetadata('Vaishvik', 'acceldata_sdk_code', '...'),
     context={'key1': 'value1'}
 )
 torch_client = TorchClient(url="https://torch.acceldata.local", access_key="*******",
                           secret_key="******************************",do_version_check=False)
 pipeline_response = torch_client.create_pipeline(pipeline=pipeline)
 pipeline_run = pipeline_response.create_pipeline_run()
+
 # Create a job using pipeline object.
 # Passing of pipeline_run_id is mandatory
 job = CreateJob(
     uid='monthly_sales_aggregate',
     name='Monthly Sales Aggregate',
     description='Generates the monthly sales aggregate tables for the complete year',
     inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
@@ -103,42 +101,41 @@
     pipeline_run_id=pipeline_run.id,
     span_uid="test_shubh"
 )
 job_response = pipeline_response.create_job(job)
 
 # Create a job using pipeline_run object.
 # Passing of pipeline_run_id is not needed
-
 job = CreateJob(
-    uid='monthly_sales_aggregate_r',
-    name='Monthly Sales Aggregate',
-    description='Generates the monthly sales aggregate tables for the complete year',
-    inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
-    outputs=[Node(job_uid='job2_uid')],
-    meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
-    context={'key21': 'value21'}
+        uid='monthly_sales_aggregate',
+        name='Monthly Sales Aggregate',
+        description='Generates the monthly sales aggregate tables for the complete year',
+        inputs=[Node(asset_uid='datasource-name.database.schema.table_1')],
+        outputs=[Node(job_uid='job2_uid')],
+        meta=JobMetadata('vaishvik', 'backend', 'https://github.com/'),
+        context={'key21': 'value21'}
 )
 job_response_using_run = pipeline_run.create_job(job)
 ```
 ##### Create Pipeline Run And Generate Spans And Send Span Events
 
-Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A Span is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
+Pipeline run indicates the execution of the pipeline. The same pipeline can be executed multiple times and each execution (run) has new snapshot version. Each pipeline run has hierarchical span's group. A `Span` is a way to group a bunch of metrics, and they are hierarchical. It can be as granular as possible. The APIs will support creating a span object from a pipeline object, and then hierarchical spans are started from parent spans. A Span typically encompasses a process or a task and can be granular. This hierarchical system is powerful enough to model extremely complex pipeline observability flows. Optionally, a span can also be associated with a Job. This way, we can track starting and completion of Job, including the failure tracking. Start and stop are implicitly tracked for a span.
 
 Acceldata sdk also has support for create new pipeline run, add spans in it. During the span life cycle, sdk is able to send some customs and standard span events to collect pipeline run metrics for observability.
 
-Params for create_span function which is available under a pipeline_run
+Params for `create_span` function which is available under a `pipeline_run`
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`associatedJobUids`: List of job uids with which the span needs to be associated with.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`associatedJobUids`: List of job uids with which the span needs to be associated with.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 
-Params for create_child_span function which is available under span_context. This is used to create hierarchy of span by creating a span under another span
+Params for `create_child_span` function which is available under `span_context`. This is used to create hierarchy of span by creating a span under another span
 
-`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.
-`context_data`: This is dict of key-value pair providing custom context information related to a span.
+`uid`: uid of the span being created. This should be unique. This is a mandatory parameter.<br/>
+`context_data`: This is dict of key-value pair providing custom context information related to a span.<br/>
 `associatedJobUids`: List of job uids with which the span needs to be associated with.
 ```python
 
 from acceldata_sdk.events.generic_event import GenericEvent
 from datetime import datetime
 
 # create a pipeline run of the pipeline
@@ -195,17 +192,17 @@
 ```
 ##### Get Pipeline Run with a particular pipeline run id
 Acceldata sdk can get a pipeline run of the pipeline with a particular pipeline run id. With use of the pipeline run 
 instance, user can continue ETL pipeline and add spans, jobs, events too. Hence, Acceldata sdk has complete access on the torch pipeline service.
 
 Params for `get_pipeline_run`:
 
-`pipeline_run_id`: run id of the pipeline run
-`continuation_id`: continuation id of the pipeline run
-`pipeline_id`: id of the pipeline to which the run belongs to
+`pipeline_run_id`: run id of the pipeline run<br/>
+`continuation_id`: continuation id of the pipeline run<br/>
+`pipeline_id`: id of the pipeline to which the run belongs to<br/>
 ```python
 pipeline_run = torch_client.get_pipeline_run(pipeline_run_id=pipeline_run_id)
 pipeline = torch_client.get_pipeline(pipeline_id=pipeline_id)
 pipeline_run = torch_client.get_pipeline_run(continuation_id=continuation_id, pipeline_id=pipeline.id)
 pipeline_run = pipeline.get_run(continuation_id=continuation_id)
 ```
```

### Comparing `acceldata_sdk-2.7.0/acceldata_sdk.egg-info/SOURCES.txt` & `acceldata_sdk-2.7.1/acceldata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.events.rst.txt` & `acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.events.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.models.rst.txt` & `acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.models.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/docs/_build/html/_sources/torch_sdk.rst.txt` & `acceldata_sdk-2.7.1/docs/_build/html/_sources/torch_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/docs/conf.py` & `acceldata_sdk-2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/integration_tests/test_constants.py` & `acceldata_sdk-2.7.1/integration_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/integration_tests/test_ds_assets.py` & `acceldata_sdk-2.7.1/integration_tests/test_ds_assets.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/integration_tests/test_pipelines.py` & `acceldata_sdk-2.7.1/integration_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/integration_tests/test_policy.py` & `acceldata_sdk-2.7.1/integration_tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-2.7.0/setup.py` & `acceldata_sdk-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # except (IOError, ImportError):
 #     description = open('README.md').read()
 
 # Change MIN_TORCH_BACKEND_VERSION_SUPPORTED in constants as well if needed while updating version here
 
 setup(
     name='acceldata_sdk',
-    version='2.7.0',
+    version='2.7.1',
     description='Acceldata SDK.' + '\n\n' + open('README.txt').read(),
     long_description=open('README.md').read() + '\n\n' + open('DATASOURCE_README.md').read() + '\n\n'  + open('CHANGELOG.txt').read(),
     long_description_content_type="text/markdown",
     url='',
     author='acceldata',
     author_email='apisupport@acceldata.io',
     license='MIT License',
```

