# Comparing `tmp/optimum-neuron-0.0.6.tar.gz` & `tmp/optimum-neuron-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.6.tar", last modified: Mon Jun 26 16:36:24 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.7.tar", last modified: Wed Jul  5 10:24:25 2023, max compression
```

## Comparing `optimum-neuron-0.0.6.tar` & `optimum-neuron-0.0.7.tar`

### file list

```diff
@@ -1,84 +1,93 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.6/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.6/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.6/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4927 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/commands/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/commands/neuron/cache.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.6/optimum/commands/register/register_export.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.6/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5317 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    11086 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12824 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4092 2023-05-30 08:48:22.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/model_configs.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2431 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/accelerate/
--rw-rw-r--   0 michael   (1000) michael   (1000)      732 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12887 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/accelerator.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2330 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/optimizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/scheduler.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15103 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/state.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)      764 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6605 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/dataclasses.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/misc.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/distributed/
--rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7136 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3797 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/encoder_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2172 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/parallelizers_manager.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2324 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/generation/
--rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.6/optimum/neuron/generation/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/generation/utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18203 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/modeling_base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12800 2023-06-08 09:55:27.000000 optimum-neuron-0.0.6/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    15201 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8663 2023-06-26 16:31:54.000000 optimum-neuron-0.0.6/optimum/neuron/training_args.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5967 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    29996 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/constant.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/misc.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6684 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/patching.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-06-26 16:32:38.000000 optimum-neuron-0.0.6/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-06-26 16:36:15.000000 optimum-neuron-0.0.6/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    34743 2023-06-13 15:28:53.000000 optimum-neuron-0.0.6/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/tests/test_compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_generate.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    45311 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.6/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.7/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.7/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.7/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5327 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/optimum/commands/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-07-04 11:50:34.000000 optimum-neuron-0.0.7/optimum/commands/neuron/cache.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.7/optimum/commands/register/register_export.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.7/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.233110 optimum-neuron-0.0.7/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      855 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9110 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12319 2023-07-05 10:19:53.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1669 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    22439 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9148 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/model_configs.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5953 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/exporters/neuron/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2498 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/accelerate/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      785 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    19501 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/accelerator.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3019 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/optimizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/scheduler.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16801 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/state.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      789 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7907 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/dataclasses.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/misc.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/distributed/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7687 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2247 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/decoder_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2666 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/encoder_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4502 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/parallel_layers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3219 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/parallelizers_manager.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4749 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/distributed/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.7/optimum/neuron/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20362 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/modeling_base.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/pipelines/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      666 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.237110 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      658 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9124 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13323 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    17146 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9224 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/training_args.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1297 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6397 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    33731 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/utils/compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/optimum/neuron/utils/constant.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/misc.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1994 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/optimization_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7282 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/utils/patching.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.7/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1461 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-07-05 10:21:01.000000 optimum-neuron-0.0.7/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2513 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-07-05 10:24:25.000000 optimum-neuron-0.0.7/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.7/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-07-05 10:23:48.000000 optimum-neuron-0.0.7/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-07-05 10:24:25.241109 optimum-neuron-0.0.7/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35375 2023-07-05 10:19:16.000000 optimum-neuron-0.0.7/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.7/tests/test_compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.7/tests/test_generate.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    49320 2023-07-04 11:50:41.000000 optimum-neuron-0.0.7/tests/test_modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.7/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.7/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.6/LICENSE` & `optimum-neuron-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/MANIFEST.in` & `optimum-neuron-0.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/PKG-INFO` & `optimum-neuron-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.6/README.md` & `optimum-neuron-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.7/optimum/commands/export/neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.7/optimum/commands/export/neuronx.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,14 +91,29 @@
         help=f"Sequence length {doc_input}",
     )
     input_group.add_argument(
         "--num_choices",
         type=int,
         help=f"Only for the multiple-choice task. Num choices {doc_input}",
     )
+    input_group.add_argument(
+        "--num_channels",
+        type=int,
+        help=f"Image tasks only. Number of channels {doc_input}",
+    )
+    input_group.add_argument(
+        "--width",
+        type=int,
+        help=f"Image tasks only. Width {doc_input}",
+    )
+    input_group.add_argument(
+        "--height",
+        type=int,
+        help=f"Image tasks only. Height {doc_input}",
+    )
 
 
 class NeuronxExportCommand(BaseOptimumCLICommand):
     COMMAND = CommandInfo(name="neuron", help="Export PyTorch models to Neuronx compiled TorchScript models.")
 
     def __init__(
         self,
```

### Comparing `optimum-neuron-0.0.6/optimum/commands/neuron/base.py` & `optimum-neuron-0.0.7/optimum/commands/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/commands/neuron/cache.py` & `optimum-neuron-0.0.7/optimum/commands/neuron/cache.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/commands/register/register_export.py` & `optimum-neuron-0.0.7/optimum/commands/register/register_export.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.7/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/distributed/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding=utf-8
-# Copyright 2023 The HuggingFace Team. All rights reserved.
+# Copyright 2023 The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .base import NeuronConfig
-from .convert import export, validate_model_outputs
+from .base import Parallelizer
+from .parallelizers_manager import ParallelizersManager
```

### Comparing `optimum-neuron-0.0.6/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.7/optimum/exporters/neuron/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         num_choices: Optional[int] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         num_channels: Optional[int] = None,
         feature_size: Optional[int] = None,
         nb_max_frames: Optional[int] = None,
         audio_sequence_length: Optional[int] = None,
+        point_batch_size: Optional[int] = None,
+        nb_points_per_image: Optional[int] = None,
     ):
         self._config = config
         self._normalized_config = self.NORMALIZED_CONFIG_CLASS(self._config)
         self.mandatory_axes = ()
         self.task = task
         self._axes: Dict[str, int] = {}
         self.dynamic_batch_size = dynamic_batch_size
@@ -128,17 +130,23 @@
             "num_choices": num_choices,
             "width": width,
             "height": height,
             "num_channels": num_channels,
             "feature_size": feature_size,
             "nb_max_frames": nb_max_frames,
             "audio_sequence_length": audio_sequence_length,
+            "point_batch_size": point_batch_size,
+            "nb_points_per_image": nb_points_per_image,
         }
+        input_shapes = {}
         for name, value in axes_values.items():
+            if value is not None:
+                input_shapes[name] = value
             setattr(self, name, value)
+        setattr(self, "input_shapes", input_shapes)
 
     @classmethod
     def get_mandatory_axes_for_task(cls, task: str) -> Tuple[str]:
         axes = []
         for axis in cls.MANDATORY_AXES:
             if isinstance(axis, tuple):
                 tasks, name = axis
@@ -253,14 +261,16 @@
         else:
             return dummy_inputs
 
     def check_model_inputs_order(
         self,
         model: "PreTrainedModel",
         dummy_inputs: Dict[str, torch.Tensor],
+        forward_with_tuple: bool = False,
+        eligible_outputs: Optional[List[Union[str, int]]] = None,
     ):
         """
         Checks if inputs order of the model's forward pass correspond to the generated dummy inputs to ensure the dummy inputs tuple used for
         tracing are under the correct order.
         """
 
         class ModelWrapper(torch.nn.Module):
@@ -273,10 +283,26 @@
                 if len(input) != len(self.input_names):
                     raise ValueError(
                         f"The model needs {len(self.input_names)} inputs: {self.input_names}."
                         f" But only {len(input)} inputs are passed."
                     )
 
                 ordered_inputs = dict(zip(self.input_names, input))
-                return self.model(**ordered_inputs)
+
+                if forward_with_tuple is True:
+                    outputs = self.model(*ordered_inputs.values())
+                else:
+                    outputs = self.model(**ordered_inputs)
+
+                if isinstance(outputs, dict) and eligible_outputs is not None:
+                    outputs = {name: outputs[name] for name in outputs.keys() & eligible_outputs}
+
+                if isinstance(outputs, tuple) and eligible_outputs is not None:
+                    if not all(isinstance(x, int) for x in eligible_outputs):
+                        raise ValueError(
+                            "To extract outputs from a tuple, `eligible_outputs` must be a list of integers only."
+                        )
+                    outputs = [outputs[i] for i in eligible_outputs]
+
+                return outputs
 
         return ModelWrapper(model, list(dummy_inputs.keys()))
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,30 @@
         "NeuronModelForMultipleChoice",
     ],
     "accelerate": [
         "NeuronAccelerator",
         "NeuronAcceleratorState",
         "NeuronPartialState",
     ],
+    "pipelines": ["pipeline"],
 }
 
 if TYPE_CHECKING:
     from .accelerate import NeuronAccelerator, NeuronAcceleratorState, NeuronPartialState
     from .hf_argparser import TrainiumHfArgumentParser
     from .modeling import (
         NeuronModelForFeatureExtraction,
         NeuronModelForMaskedLM,
         NeuronModelForMultipleChoice,
         NeuronModelForQuestionAnswering,
         NeuronModelForSequenceClassification,
         NeuronModelForTokenClassification,
     )
     from .modeling_base import NeuronBaseModel
+    from .pipelines import pipeline
     from .trainers import Seq2SeqTrainiumTrainer, TrainiumTrainer
     from .training_args import Seq2SeqTrainiumTrainingArguments, TrainiumTrainingArguments
 else:
     import sys
 
     sys.modules[__name__] = _LazyModule(
         __name__,
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .accelerator import NeuronAccelerator
 from .state import NeuronAcceleratorState, NeuronPartialState
+from .utils.dataclasses import NeuronDistributedType
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/optimizer.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/optimizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,37 +13,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Custom AcceleratedOptimizer for Neuron."""
 
 from accelerate.optimizer import AcceleratedOptimizer
 from accelerate.utils import DistributedType
 
-from ..utils import is_torch_xla_available
+from ..utils import is_neuronx_distributed_available, is_torch_xla_available
 from .utils.dataclasses import NeuronDistributedType
 
 
 if is_torch_xla_available():
     import accelerate
     import torch_xla.core.xla_model as xm
 
     accelerate.optimizer.xm = xm
 
+if is_neuronx_distributed_available():
+    from neuronx_distributed.parallel_layers import parallel_state
+
 
 class NeuronAcceleratedOptimizer(AcceleratedOptimizer):
     # TODO: might be needed to override this soon.
     def load_state_dict(self, state_dict):
         return super().load_state_dict(state_dict)
 
     def step(self, closure=None):
         if self.gradient_state.sync_gradients:
             if self.accelerator_state.distributed_type is DistributedType.TPU:
                 optimizer_args = {"closure": closure} if closure is not None else {}
                 xm.optimizer_step(self.optimizer, optimizer_args=optimizer_args)
             elif self.accelerator_state.distributed_type is NeuronDistributedType.XLA_FSDP:
                 self.optimizer.step(closure)
+            elif self.accelerator_state.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
+                xm.optimizer_step(self.optimizer, groups=parallel_state.get_data_parallel_group(as_list=True))
+                # xm.reduce_gradients(self.optimizer, groups=parallel_state.get_data_parallel_group(as_list=True))
+                # parameters = [p for group in self.optimizer.param_groups for p in group["params"]]
+                # parallel_layers.clip_grad_norm(parameters, 1.0, norm_type=2)
+                # self.optimizer.step()
             elif self.scaler is not None:
                 scale_before = self.scaler.get_scale()
                 self.scaler.step(self.optimizer, closure)
                 self.scaler.update()
                 scale_after = self.scaler.get_scale()
                 # If we reduced the loss scale, it means the optimizer step was skipped because of gradient overflow.
                 self._is_overflow = scale_after < scale_before
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/scheduler.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/scheduler.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/state.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,27 @@
     is_ipex_available,
     is_xpu_available,
     parse_choice_from_env,
     parse_flag_from_env,
 )
 from accelerate.utils.dataclasses import FullyShardedDataParallelPlugin, SageMakerDistributedType
 
-from ..utils import is_torch_xla_available
+from ...utils import logging
+from ..utils import is_neuronx_distributed_available, is_torch_xla_available
 from .utils import NeuronDistributedType, NeuronFullyShardedDataParallelPlugin
 
 
 if is_torch_xla_available():
     import torch_xla.core.xla_model as xm
 
+if is_neuronx_distributed_available():
+    from neuronx_distributed.parallel_layers import parallel_state
+
+
+logger = logging.get_logger()
 
 SharedDict = ThreadLocalSharedDict
 
 
 class NeuronPartialState(PartialState):
     def __init__(self, cpu: bool = False, **kwargs):
         self.__dict__ = self._shared_state
@@ -178,15 +184,15 @@
 
                 if self.device is None:
                     self.device = torch.device("cpu") if cpu else self.default_device
 
         self.fork_launched = parse_flag_from_env("FORK_LAUNCHED", 0)
 
     def wait_for_everyone(self):
-        if self.distributed_type is NeuronDistributedType.XLA_FSDP:
+        if self.distributed_type in [NeuronDistributedType.XLA_FSDP, NeuronDistributedType.TENSOR_PARALLELISM]:
             xm.rendezvous("accelerate.utils.wait_for_everyone")
         else:
             super().wait_for_everyone()
 
 
 class NeuronAcceleratorState(AcceleratorState):
     """
@@ -212,23 +218,24 @@
         self,
         mixed_precision: str = None,
         cpu: bool = False,
         dynamo_plugin=None,
         deepspeed_plugin=None,
         fsdp_plugin=None,
         megatron_lm_plugin=None,
+        tp_plugin=None,
         _from_accelerator: bool = False,
         **kwargs,
     ):
         self.__dict__ = self._shared_state
         if parse_flag_from_env("ACCELERATE_USE_CPU"):
             cpu = True
-        if PartialState._shared_state == {}:
-            PartialState(cpu, **kwargs)
-        self.__dict__.update(PartialState._shared_state)
+        if NeuronPartialState._shared_state == {}:
+            NeuronPartialState(cpu, **kwargs)
+        self.__dict__.update(NeuronPartialState._shared_state)
         self._check_initialized(mixed_precision, cpu)
         if not self.initialized:
             self.deepspeed_plugin = None
             self.ipex_plugin = None
             mixed_precision = (
                 parse_choice_from_env("ACCELERATE_MIXED_PRECISION", "no")
                 if mixed_precision is None
@@ -250,14 +257,37 @@
                         os.environ["XLA_USE_BF16"] = str(0)
                         os.environ["XLA_DOWNCAST_BF16"] = str(1)
                         self.downcast_bfloat = True
                     else:
                         os.environ["XLA_USE_BF16"] = str(1)
                         os.environ["XLA_DOWNCAST_BF16"] = str(0)
                         self.downcast_bfloat = False
+                if os.environ.get("ACCELERATE_USE_NEURONX_DISTRIBUTED_TP", "false") == "true":
+                    if not is_neuronx_distributed_available():
+                        raise RuntimeError(
+                            "Tensor parallelism requires the neuronx_distributed package. You can install it by "
+                            "running: python -m pip install neuronx_distributed --extra-index-url "
+                            "https://pip.repos.neuron.amazonaws.com"
+                        )
+                    if tp_plugin is None:
+                        raise ValueError(
+                            "Could not initialize `neuronx_distributed` tensor parallelism because no "
+                            "TensorParallelismPlugin was provided."
+                        )
+                    if tp_plugin.should_parallelize:
+                        parallel_state.initialize_model_parallel(
+                            tensor_model_parallel_size=tp_plugin.tensor_parallel_size
+                        )
+                        self.distributed_type = NeuronDistributedType.TENSOR_PARALLELISM
+                    else:
+                        logger.warning(
+                            "Tensor parallelism is requested but nothing is done because the tensor parallel size is "
+                            "set to 1."
+                        )
+                    self.tp_plugin = tp_plugin
                 if os.environ.get("ACCELERATE_USE_FSDP", "false") == "true":
                     self.distributed_type = NeuronDistributedType.XLA_FSDP
                     if self._mixed_precision != "no":
                         # TODO: do we need that?
                         fsdp_plugin.set_mixed_precision(self._mixed_precision)
                     if isinstance(fsdp_plugin, FullyShardedDataParallelPlugin) and not isinstance(
                         fsdp_plugin, NeuronFullyShardedDataParallelPlugin
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .dataclasses import NeuronDistributedType, NeuronFullyShardedDataParallelPlugin
+from .dataclasses import NeuronDistributedType, NeuronFullyShardedDataParallelPlugin, TensorParallelismPlugin
 from .misc import patch_accelerate_is_tpu_available
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/dataclasses.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/dataclasses.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,37 +13,43 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Custom dataclasses for Neuron."""
 
 import enum
 import os
 from dataclasses import dataclass
+from typing import TYPE_CHECKING, Dict, Tuple, Union
 
 import torch
 from accelerate.utils.constants import MODEL_NAME, OPTIMIZER_NAME
 from accelerate.utils.dataclasses import FullyShardedDataParallelPlugin
 
+from ...distributed import ParallelizersManager
 from ...utils import is_torch_xla_available
 
 
 if is_torch_xla_available():
     import torch_xla.core.xla_model as xm
     from torch_xla.distributed.fsdp import XlaFullyShardedDataParallel as FSDP
     from torch_xla.distributed.fsdp.state_dict_utils import consolidate_sharded_model_checkpoints
 
+if TYPE_CHECKING:
+    from transformers import PreTrainedModel
+
 
 class NeuronDistributedType(str, enum.Enum):
     """
     Represents a type of distributed environment specific to Neuron.
 
     Values:
         - **XLA_FSDP** -- Fully Shareded Data Parallelism on Neuron cores using `torch_xla`.
     """
 
     XLA_FSDP = "XLA_FSDP"
+    TENSOR_PARALLELISM = "TENSOR_PARALLELISM"
 
 
 @dataclass
 class NeuronFullyShardedDataParallelPlugin(FullyShardedDataParallelPlugin):
     # TODO: redefine the post init to do checks on which option is supported.
     def save_model(self, accelerator, model, output_dir, model_index=0):
         from torch.distributed.fsdp.fully_sharded_data_parallel import StateDictType
@@ -126,7 +132,35 @@
         # # called from all ranks, though only rank0 has a valid param for full_osd
         # sharded_osd = FSDP.scatter_full_optim_state_dict(full_osd, model)
         # optimizer.load_state_dict(sharded_osd)
         optimizer_path = os.path.join(input_dir, f"{OPTIMIZER_NAME}_rank{accelerator.process_index}.bin")
         optim_state = torch.load(optimizer_path)
         xm.send_cpu_data_to_device(optim_state, accelerator.device)
         optimizer.load_state_dict(optim_state["optimizer"])
+
+
+@dataclass
+class TensorParallelismPlugin:
+    tensor_parallel_size: int = 1
+
+    def __post_init__(self):
+        if self.tensor_parallel_size > 1:
+            raise NotImplementedError("Tensor Parallelism is not supported yet.")
+        if self.tensor_parallel_size < 1:
+            raise ValueError(f"The tensor parallel size must be >= 1, but {self.tensor_parallel_size} was given here.")
+
+    @property
+    def should_parallelize(self):
+        return self.tensor_parallel_size > 1
+
+    def parallelize_model(
+        self, model: "PreTrainedModel", return_orig_to_parallel: bool = False
+    ) -> Union["PreTrainedModel", Tuple["PreTrainedModel", Dict[int, "torch.nn.Parameter"]]]:
+        orig_to_parallel = {}
+        parallelizer = ParallelizersManager.parallelizer_for_model(model)
+        parallelized_model = parallelizer.parallelize(
+            model, orig_to_parallel=orig_to_parallel if return_orig_to_parallel else None
+        )
+        if return_orig_to_parallel:
+            return parallelized_model, orig_to_parallel
+        else:
+            return parallelized_model
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/misc.py` & `optimum-neuron-0.0.7/optimum/neuron/accelerate/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/distributed/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/pipelines/transformers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # coding=utf-8
-# Copyright 2023 The HuggingFace Inc. team. All rights reserved.
+# Copyright 2023 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .base import Parallelizer
-from .parallelizers_manager import ParallelizersManager
+from .base import (
+    pipeline,
+)
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/distributed/base.py` & `optimum-neuron-0.0.7/optimum/neuron/distributed/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,34 +14,39 @@
 # limitations under the License.
 """Base class related to `neuronx_distributed` to perform parallelism."""
 
 import contextlib
 from abc import ABC, abstractclassmethod
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import torch
 from transformers.utils import WEIGHTS_NAME
 
+from ...utils import logging
 from ..utils import is_neuronx_distributed_available, is_torch_xla_available
 from .utils import TENSOR_PARALLEL_SHARDS_DIR_NAME
 
 
 if is_neuronx_distributed_available():
     import neuronx_distributed
+    from neuronx_distributed import parallel_layers
 
 if is_torch_xla_available():
     import torch_xla.core.xla_model as xm
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel
 
 
+logger = logging.get_logger()
+
+
 class SavedModelInTemporaryDirectory:
     def __init__(self, model: "PreTrainedModel"):
         self.tmpdir = TemporaryDirectory()
         self.model = model
 
     def __enter__(self):
         self.model.save_pretrained(self.tmpdir.name)
@@ -83,38 +88,48 @@
 
     @classmethod
     def deparallelize(cls, model: "PreTrainedModel") -> "PreTrainedModel":
         raise NotImplementedError
 
     @classmethod
     def was_parallelized(cls, model: "PreTrainedModel") -> bool:
-        parallel_layers = (
-            neuronx_distributed.parallel_layers.ParallelEmbedding,
-            neuronx_distributed.parallel_layers.ColumnParallelLinear,
-            neuronx_distributed.parallel_layers.RowParallelLinear,
+        parallel_layer_classes = (
+            parallel_layers.ParallelEmbedding,
+            parallel_layers.ColumnParallelLinear,
+            parallel_layers.RowParallelLinear,
         )
-        return any(isinstance(mod, parallel_layers) for mod in model.modules())
+        return any(isinstance(mod, parallel_layer_classes) for mod in model.modules())
 
     @classmethod
     def _check_model_was_parallelized(cls, model: "PreTrainedModel"):
         if not cls.was_parallelized(model):
             raise ValueError("The model needs to be parallelized first.")
 
     @classmethod
-    def save_model_checkpoint_as_regular(cls, model: "PreTrainedModel", output_dir: Union[str, Path]):
+    def save_model_checkpoint_as_regular(
+        cls,
+        model: "PreTrainedModel",
+        output_dir: Union[str, Path],
+        optimizer: Optional["torch.optim.Optimizer"] = None,
+    ):
         cls._check_model_was_parallelized(model)
-        data_parallel_rank = neuronx_distributed.parallel_state.get_data_parallel_rank()
-        tensor_parallel_rank = neuronx_distributed.parallel_state.get_tensor_parallel_rank()
+        data_parallel_rank = parallel_layers.parallel_state.get_data_parallel_rank()
+        tensor_parallel_rank = parallel_layers.parallel_state.get_tensor_parallel_rank()
 
         if data_parallel_rank != 0:
             return
 
         if not isinstance(output_dir, Path):
             output_dir = Path(output_dir)
 
+        if optimizer is not None:
+            logger.warning(
+                "Saving the optimizer state as a regular file under the tensor parallel setting is not supported yet."
+            )
+
         state_dict = {}
         for name, param in model.named_parameters():
             if getattr(param, "tensor_model_parallel", False):
                 if param.partition_dim == 1:
                     tensor = neuronx_distributed.utils.gather_from_tensor_model_parallel_region(param)
                 else:
                     # Because the gather works only on last dim. Need to make it work for all dims.
@@ -130,47 +145,57 @@
         xm._maybe_convert_to_cpu(model_state_dict, convert=should_save)
         if should_save:
             output_path = output_dir / WEIGHTS_NAME
             torch.save(model_state_dict["model"], output_path.as_posix())
         xm.rendevous("saving regular checkpoint")
 
     @classmethod
-    def save_model_checkpoint_as_sharded(cls, model: "PreTrainedModel", output_dir: Union[str, Path]):
+    def save_model_checkpoint_as_sharded(
+        cls,
+        model: "PreTrainedModel",
+        output_dir: Union[str, Path],
+        optimizer: Optional["torch.optim.Optimizer"] = None,
+    ):
         cls._check_model_was_parallelized(model)
-        data_parallel_rank = neuronx_distributed.parallel_state.get_data_parallel_rank()
-        if data_parallel_rank != 0:
-            return
-
         if not isinstance(output_dir, Path):
             output_dir = Path(output_dir)
 
+        state_dict = {"model": model.state_dict()}
+        if optimizer is not None:
+            state_dict["optimizer_state_dict"] = optimizer.state_dict()
+
         output_path = output_dir / TENSOR_PARALLEL_SHARDS_DIR_NAME
-        neuronx_distributed.parallel_layers.save({"model": model.state_dict()}, output_path.as_posix())
+        parallel_layers.save(state_dict, output_path.as_posix())
 
     @classmethod
     def save_model_checkpoint(
-        cls, model: "PreTrainedModel", output_dir: Union[str, Path], as_regular: bool = True, as_sharded: bool = True
+        cls,
+        model: "PreTrainedModel",
+        output_dir: Union[str, Path],
+        as_regular: bool = False,
+        as_sharded: bool = True,
+        optimizer: Optional["torch.optim.Optimizer"] = None,
     ):
         if not as_regular and not as_sharded:
             raise ValueError("At least as_regular or as_sharded must be True.")
         if as_regular:
-            cls.save_model_checkpoint(model, output_dir)
+            cls.save_model_checkpoint_as_regular(model, output_dir, optimizer=optimizer)
         if as_sharded:
-            cls.save_model_checkpoint_as_sharded(model, output_dir)
+            cls.save_model_checkpoint_as_sharded(model, output_dir, optimizer=optimizer)
 
     @classmethod
     def load_model_regular_checkpoint(cls, model: "PreTrainedModel", load_dir: Union[str, Path]):
         raise NotImplementedError("This requires being able to deparallelize the model.")
 
     @classmethod
     def load_model_sharded_checkpoint(cls, model: "PreTrainedModel", load_dir: Union[str, Path]):
         cls._check_model_was_parallelized(model)
         if not isinstance(load_dir, Path):
             load_dir = Path(load_dir)
-        neuronx_distributed.parallel_layers.load(load_dir / TENSOR_PARALLEL_SHARDS_DIR_NAME, model=model, sharded=True)
+        parallel_layers.load(load_dir / TENSOR_PARALLEL_SHARDS_DIR_NAME, model=model, sharded=True)
 
     @classmethod
     def load_model_checkpoint(cls, model: "PreTrainedModel", load_dir: Union[str, Path]):
         if not isinstance(load_dir, Path):
             load_dir = Path(load_dir)
 
         if (load_dir / TENSOR_PARALLEL_SHARDS_DIR_NAME).is_dir():
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/distributed/parallelizers_manager.py` & `optimum-neuron-0.0.7/optimum/neuron/distributed/parallelizers_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,28 +10,57 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Factory class mapping model architectures to their Parallelizer class."""
 
-from typing import Type, Union
+import importlib
+from typing import Dict, Type, Union
 
 from transformers import PreTrainedModel
 
-from optimum.neuron.utils.training_utils import is_model_officially_supported
-
 from .base import Parallelizer
-from .encoder_models import BertParallelizer
+
+
+_PARALLELIZER_CLASSES_MODULE_NAMES = ["encoder_models", "decoder_models"]
+
+
+def parallelizer_classes_resolver(
+    model_type_to_parallelizer_class_name: Dict[str, str]
+) -> Dict[str, Type[Parallelizer]]:
+    modules = []
+    for module_name in _PARALLELIZER_CLASSES_MODULE_NAMES:
+        package_name = __name__.rsplit(".", maxsplit=1)[0]
+        full_module_name = f"{package_name}.{module_name}"
+        modules.append(importlib.import_module(full_module_name))
+
+    resolved = {}
+    for model_type, parallelizer_class_name in model_type_to_parallelizer_class_name.items():
+        found = False
+        for mod in modules:
+            cls = getattr(mod, parallelizer_class_name, None)
+            if cls is not None:
+                found = True
+                resolved[model_type] = cls
+                break
+        if not found:
+            raise ValueError(f"Could not resolve the parallelizer class name {parallelizer_class_name}.")
+    return resolved
 
 
 class ParallelizersManager:
-    _MODEL_TYPE_TO_PARALLEL_MODEL_CLASS = {
-        "bert": BertParallelizer,
-    }
+    _MODEL_TYPE_TO_PARALLEL_MODEL_CLASS = parallelizer_classes_resolver(
+        {
+            "bert": "BertParallelizer",
+            "roberta": "RobertaParallelizer",
+            "gpt_neo": "GPTNeoParallelizer",
+            "llama": "LlamaParallelizer",
+        }
+    )
 
     @classmethod
     def _get_model_type(cls, model_type_or_model: Union[str, PreTrainedModel]) -> str:
         if isinstance(model_type_or_model, PreTrainedModel):
             model_type = model_type_or_model.config.model_type
         else:
             model_type = model_type_or_model
@@ -41,13 +70,13 @@
     def is_model_supported(cls, model_type_or_model: Union[str, PreTrainedModel]) -> bool:
         model_type = cls._get_model_type(model_type_or_model)
         return model_type in cls._MODEL_TYPE_TO_PARALLEL_MODEL_CLASS
 
     @classmethod
     def parallelizer_for_model(cls, model_type_or_model: Union[str, PreTrainedModel]) -> Type[Parallelizer]:
         model_type = cls._get_model_type(model_type_or_model)
-        if not is_model_officially_supported(model_type_or_model):
+        if not cls.is_model_supported(model_type_or_model):
             supported_models = ", ".join(cls._MODEL_TYPE_TO_PARALLEL_MODEL_CLASS.keys())
             raise NotImplementedError(
-                f"{model_type} is not supported for parallelization, supported model: {supported_models}"
+                f"{model_type} is not supported for parallelization, supported models: {supported_models}"
             )
         return cls._MODEL_TYPE_TO_PARALLEL_MODEL_CLASS[model_type]
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/generation/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/generation/utils.py` & `optimum-neuron-0.0.7/optimum/neuron/generation/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.7/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/modeling.py` & `optimum-neuron-0.0.7/optimum/neuron/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/modeling_base.py` & `optimum-neuron-0.0.7/optimum/neuron/modeling_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,25 @@
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 import torch
 from huggingface_hub import HfApi, HfFolder, hf_hub_download
+from packaging import version
 from transformers import AutoConfig, AutoModel
 
 from ..exporters.neuron import export
 from ..exporters.neuron.model_configs import *  # noqa: F403
 from ..exporters.tasks import TasksManager
 from ..modeling_base import OptimizedModel
 from ..utils.save_utils import maybe_load_preprocessors, maybe_save_preprocessors
 from .utils import NEURON_FILE_NAME, is_neuron_available, store_compilation_config
+from .utils.import_utils import is_neuronx_available
+from .utils.version_utils import get_neuroncc_version, get_neuronxcc_version
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
     from ..exporters.neuron import NeuronConfig
 
@@ -150,14 +153,36 @@
                 raise RuntimeError(
                     f"Too many neuron model files were found in {model_path}, specify which one to load by using the "
                     "file_name argument."
                 )
             else:
                 file_name = neuron_files[0].name
 
+        # Check compiler compatibility(compiler type and version) of the saved model vs. system.
+        if hasattr(config, "neuron_compiler"):
+            if config.neuron_compiler == "neuron-cc":
+                compiler_available_fn = is_neuron_available
+                installed_compiler_version_fn = get_neuroncc_version
+            elif config.neuron_compiler == "neuronx-cc":
+                compiler_available_fn = is_neuronx_available
+                installed_compiler_version_fn = get_neuronxcc_version
+            else:
+                raise RuntimeError(f"Pretrained model compiler type {config.neuron_compiler} not recognized.")
+
+            if not compiler_available_fn():
+                raise RuntimeError(
+                    f"Pretrained model was compiled for {config.neuron_compiler}, but {config.neuron_compiler} is not installed."
+                )
+                if hasattr(config, "neuron_compiler_version"):
+                    if version.parse(config.neuron_compiler_version) > version.parse(installed_compiler_version_fn()):
+                        raise RuntimeError(
+                            f"Pretrained model ({config.neuron_compiler}={installed_compiler_version_fn()}) is newer than current compiler ({config.neuron_compiler}={config.neuron_compiler_version}),"
+                            " which may cause runtime incompatabilities."
+                        )
+
         preprocessors = None
         if model_path.is_dir():
             model = NeuronBaseModel.load_model(model_path / file_name)
             new_model_save_dir = model_path
         else:
             model_cache_path = hf_hub_download(
                 repo_id=model_id,
@@ -267,15 +292,31 @@
         input_names, output_names = export(
             model=model,
             config=neuron_config,
             output=save_dir_path / NEURON_FILE_NAME,
             **compiler_kwargs,
         )
 
-        store_compilation_config(config, input_shapes, compiler_kwargs, input_names, output_names, dynamic_batch_size)
+        # This logic is a bit of a reacharound, using the same logic as in `export()` to determine the cc version
+        if is_neuronx_available():
+            neuron_compiler = "neuronx-cc"
+            neuron_compiler_version = get_neuronxcc_version()
+        else:
+            neuron_compiler = "neuron-cc"
+            neuron_compiler_version = get_neuroncc_version()
+        store_compilation_config(
+            config,
+            input_shapes,
+            compiler_kwargs,
+            input_names,
+            output_names,
+            dynamic_batch_size,
+            neuron_compiler,
+            neuron_compiler_version,
+        )
 
         config.save_pretrained(save_dir_path)
         maybe_save_preprocessors(model_id, save_dir_path, src_subfolder=subfolder)
 
         return cls._from_pretrained(save_dir_path, config, model_save_dir=save_dir, neuron_config=neuron_config)
 
     def forward(self, *args, **kwargs):
@@ -314,15 +355,15 @@
         """
         Builds a `NeuronConfig` with an instance of the `PretrainedConfig` and the task.
         """
         # Fetch mandatory shapes from config
         compile_shapes = {
             key.replace("neuron_", ""): value
             for (key, value) in config.to_diff_dict().items()
-            if key.startswith("neuron_")
+            if key.startswith("neuron_") and not key.startswith("neuron_compiler")  # <-- TODO: is there a better way?
         }
 
         # Neuron config constructuor
         task = TasksManager.infer_task_from_model(self.auto_model_class)
         neuron_config_constructor = TasksManager.get_exporter_config_constructor(
             model_type=config.model_type, exporter="neuron", task=task
         )
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.7/optimum/neuron/trainer_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from transformers import TrainerCallback, TrainerState
 
 from ..utils import logging
 from .utils.cache_utils import (
     NEURON_COMPILE_CACHE_NAME,
     NeuronHash,
     download_cached_model_from_hub,
+    follows_new_cache_naming_convention,
     get_neuron_cache_path,
     list_files_in_neuron_cache,
     path_after_folder,
     push_to_cache_on_hub,
     set_neuron_cache_path,
 )
 
@@ -115,59 +116,64 @@
             with open(neuron_cache_path / "cache_stats.json", "r") as fp:
                 cache_stats = json.load(fp)
         else:
             cache_stats = {}
         return cache_stats
 
     @classmethod
-    def _insert_in_cache_stats(cls, cache_stats: Dict[str, Dict[str, Any]], path: Path):
-        path_in_cache = path_after_folder(path, NEURON_COMPILE_CACHE_NAME)
+    def _insert_in_cache_stats(cls, cache_stats: Dict[str, Dict[str, Any]], path: Path, cache_path: Path):
+        path_in_cache = path_after_folder(path, cache_path.name)
         cache_key = path_in_cache.parts[0]
         item = cache_stats.get(cache_key, {})
         if path.parent.as_posix() in item:
             return
         item[path.parent.as_posix()] = {"used_time": 1, "size": cls.get_dir_size(path.parent)}
         cache_stats[cache_key] = item
 
     @classmethod
     def _update_cache_stats(cls, neuron_cache_path: Path):
         cache_stats = cls._load_cache_stats(neuron_cache_path)
         for path in list_files_in_neuron_cache(neuron_cache_path):
-            cls._insert_in_cache_stats(cache_stats, path)
+            cls._insert_in_cache_stats(cache_stats, path, neuron_cache_path)
         with open(neuron_cache_path / "cache_stats.json", "w") as fp:
             json.dump(cache_stats, fp)
 
     @classmethod
     def create_temporary_neuron_cache(cls, neuron_cache_path: Optional[Path]) -> TemporaryDirectory:
         tmp_neuron_cache = TemporaryDirectory()
         tmp_neuron_cache_path = Path(tmp_neuron_cache.name)
         if neuron_cache_path is not None:
             neuron_cache_files = list_files_in_neuron_cache(neuron_cache_path)
         else:
             neuron_cache_files = []
 
-        set_neuron_cache_path(tmp_neuron_cache_path)
-        tmp_neuron_cache_path = tmp_neuron_cache_path / NEURON_COMPILE_CACHE_NAME
+        if follows_new_cache_naming_convention():
+            tmp_neuron_cache_path = tmp_neuron_cache_path / NEURON_COMPILE_CACHE_NAME
+            set_neuron_cache_path(tmp_neuron_cache_path)
+        else:
+            set_neuron_cache_path(tmp_neuron_cache_path)
+            tmp_neuron_cache_path = tmp_neuron_cache_path / NEURON_COMPILE_CACHE_NAME
+
         tmp_neuron_cache_path.mkdir()
 
         cache_stats_exists = False
         if neuron_cache_path is not None:
             cache_stats = cls._load_cache_stats(neuron_cache_path)
         else:
             cache_stats = {}
 
         for cache_file in neuron_cache_files:
             if cache_file.name == "cache_stats.json":
                 continue
-            path_in_neuron_cache = path_after_folder(cache_file, NEURON_COMPILE_CACHE_NAME)
+            path_in_neuron_cache = path_after_folder(cache_file, neuron_cache_path.name)
             tmp_cache_file = tmp_neuron_cache_path / path_in_neuron_cache
             tmp_cache_file.parent.mkdir(parents=True, exist_ok=True)
             tmp_cache_file.symlink_to(cache_file)
 
-            cls._insert_in_cache_stats(cache_stats, cache_file)
+            cls._insert_in_cache_stats(cache_stats, cache_file, neuron_cache_path)
 
         if not cache_stats_exists:
             with open(tmp_neuron_cache_path / "cache_stats.json", "w") as fp:
                 json.dump(cache_stats, fp)
 
         return tmp_neuron_cache
 
@@ -195,16 +201,16 @@
         if neuron_hash is None:
             neuron_hash = NeuronHash(*key)
             self.neuron_hashes[key] = neuron_hash
             if try_to_fetch_cached_model:
                 self.try_to_fetch_cached_model(neuron_hash)
         return neuron_hash
 
-    def full_path_to_path_in_cache(self, path: Path):
-        return path_after_folder(path, NEURON_COMPILE_CACHE_NAME)
+    def full_path_to_path_in_temporary_cache(self, path: Path):
+        return path_after_folder(path, self.tmp_neuron_cache_path.name)
 
     def try_to_fetch_cached_model(self, neuron_hash: NeuronHash) -> bool:
         # TODO: needs to be called ONLY when absolutely needed.
         files_before_fetching = list_files_in_neuron_cache(self.tmp_neuron_cache_path, only_relevant_files=True)
         cache_path = neuron_hash.cache_path
 
         def path_in_repo_to_path_in_target_directory(path):
@@ -219,15 +225,15 @@
         if found_in_cache:
             files_after_fetching = list_files_in_neuron_cache(self.tmp_neuron_cache_path, only_relevant_files=True)
             diff = [f for f in files_after_fetching if f not in files_before_fetching]
             # The fetched files should not be synchronized with the Hub.
             self.tmp_neuron_cache_state += diff
             if self.use_neuron_cache:
                 for path in diff:
-                    path_in_cache = self.full_path_to_path_in_cache(path)
+                    path_in_cache = self.full_path_to_path_in_temporary_cache(path)
                     path_in_original_cache = self.neuron_cache_path / path_in_cache
                     path_in_original_cache.parent.mkdir(parents=True, exist_ok=True)
                     if path_in_original_cache.exists():
                         continue
                     shutil.copy(path, path_in_original_cache)
 
         return found_in_cache
@@ -240,20 +246,23 @@
         self.tmp_neuron_cache_state = current_files_in_neuron_cache
         return diff
 
     def synchronize_temporary_neuron_cache(self):
         for neuron_hash, files in self.neuron_hash_to_files.items():
 
             def local_path_to_path_in_repo(path):
-                return path_after_folder(path, f"USER_neuroncc-{neuron_hash.neuron_compiler_version}")
+                if follows_new_cache_naming_convention():
+                    return path_after_folder(path, f"neuronxcc-{neuron_hash.neuron_compiler_version}")
+                else:
+                    return path_after_folder(path, f"USER_neuroncc-{neuron_hash.neuron_compiler_version}")
 
             for path in files:
                 push_to_cache_on_hub(neuron_hash, path, local_path_to_path_in_repo=local_path_to_path_in_repo)
                 if self.use_neuron_cache:
-                    path_in_cache = self.full_path_to_path_in_cache(path)
+                    path_in_cache = self.full_path_to_path_in_temporary_cache(path)
                     target_file = self.neuron_cache_path / path_in_cache
                     target_file.parent.mkdir(parents=True, exist_ok=True)
                     shutil.copy(path, self.neuron_cache_path / path_in_cache)
 
         if self.use_neuron_cache:
             self._update_cache_stats(self.neuron_cache_path)
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/trainers.py` & `optimum-neuron-0.0.7/optimum/neuron/trainers.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     TRAINER_STATE_NAME,
 )
 from transformers.trainer_pt_utils import reissue_pt_warnings
 from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 from transformers.utils import is_sagemaker_mp_enabled
 
 from ..utils import check_if_transformers_greater, logging
-from .accelerate import NeuronAccelerator
+from .accelerate import NeuronAccelerator, NeuronDistributedType
+from .distributed import ParallelizersManager
 from .trainer_callback import NeuronCacheCallaback
 from .utils import DynamicPatch, ModelPatcher, is_torch_xla_available, patch_within_function
 from .utils.cache_utils import get_neuron_cache_path
 from .utils.training_utils import (
     TRANSFORMERS_MIN_VERSION_USE_ACCELERATE,
     is_precompilation,
     patch_generation_mixin_to_neuron_generation_mixin,
@@ -138,14 +139,15 @@
 
         if not is_precompilation():
             callback = NeuronCacheCallaback(
                 tmp_neuron_cache=_TMP_NEURON_CACHE_DIR,
                 original_neuron_cache_path=_ORIGINAL_NEURON_CACHE_PATH,
                 only_do_fetching=self.args.local_rank > 0,
             )
+            # TODO: re-enable.
             self.add_callback(callback)
 
         # Make the model Neuron-compatible for generation.
         patch_generation_mixin_to_neuron_generation_mixin(self.model)
 
     def prepare_args_for_precompilation(self, args: "TrainingArguments"):
         if args.num_train_epochs != 1:
@@ -160,17 +162,41 @@
         if args.do_predict is True:
             logger.info("Disabling prediction during precompilation as this is not well supported yet.")
             args.do_predict = False
 
     def validate_args(self, args: "TrainingArguments"):
         pass
 
-    @patch_within_function(("transformers.trainer.Accelerator", NeuronAccelerator), ignore_missing_attributes=True)
     def create_accelerator_and_postprocess(self):
-        return super().create_accelerator_and_postprocess()
+        # create accelerator object
+        self.accelerator = NeuronAccelerator(
+            deepspeed_plugin=self.args.deepspeed_plugin,
+            gradient_accumulation_steps=self.args.gradient_accumulation_steps,
+            tp_plugin=self.args.tp_plugin,
+        )
+
+        # deepspeed and accelerate flags covering both trainer args and accelerate launcher
+        self.is_deepspeed_enabled = getattr(self.accelerator.state, "deepspeed_plugin", None) is not None
+        self.is_fsdp_enabled = getattr(self.accelerator.state, "fsdp_plugin", None) is not None
+
+        # post accelerator creation setup
+        if self.is_fsdp_enabled:
+            fsdp_plugin = self.accelerator.state.fsdp_plugin
+            fsdp_plugin.limit_all_gathers = self.args.fsdp_config.get("limit_all_gathers", False)
+            fsdp_plugin.use_orig_params = self.args.fsdp_config.get("use_orig_params", False)
+
+        if self.is_deepspeed_enabled:
+            if getattr(self.args, "hf_deepspeed_config", None) is None:
+                from transformers.deepspeed import HfTrainerDeepSpeedConfig
+
+                ds_plugin = self.accelerator.state.deepspeed_plugin
+
+                ds_plugin.hf_ds_config = HfTrainerDeepSpeedConfig(ds_plugin.hf_ds_config.config)
+                ds_plugin.deepspeed_config = ds_plugin.hf_ds_config.config
+                ds_plugin.hf_ds_config.trainer_config_process(self.args)
 
     def _wrap_model(self, model, training=True, dataloader=None):
         patching_specs = []
         for spec in MODEL_PATCHING_SPECS:
             patching_specs.append((model,) + spec)
 
         with ModelPatcher(patching_specs, ignore_missing_attributes=True):
@@ -230,38 +256,30 @@
     #     return result
 
     # def _nested_gather(self, tensors, name=None):
     #     if self.is_fsdp_enabled:
     #         return self._nested_gather_for_xla_fsdp(tensors, name="nested_gather_for_xla_fsdp")
     #     return super()._nested_gather(tensors, name=name)
 
-    def _save_checkpoint_for_xla_fsdp(self, model, trial, metrics=None):
-        if not self.is_fsdp_enabled:
+    def _save_checkpoint_with_accelerator(self, model, trial, metrics=None):
+        if self.accelerator.distributed_type is NeuronDistributedType.XLA_FSDP and not self.is_fsdp_enabled:
             # TODO: handle this case better?
             # Do we want to fail here? Can we save anyway?
             raise RuntimeError("Cannot save checkpoint if FSDP is not enabled.")
 
         checkpoint_folder = f"{PREFIX_CHECKPOINT_DIR}-{self.state.global_step}"
 
         if self.hp_search_backend is None and trial is None:
             self.store_flos()
 
         run_dir = self._get_output_dir(trial=trial)
         output_dir = os.path.join(run_dir, checkpoint_folder)
         os.makedirs(output_dir, exist_ok=True)
 
-        # Save model
-        self.accelerator.state.fsdp_plugin.save_model(self.accelerator, self.model, output_dir)
-
-        # Save optimizer
-        self.accelerator.state.fsdp_plugin.save_optimizer(self.accelerator, self.optimizer, self.model, output_dir)
-
-        # Save scheduler
-        with warnings.catch_warnings(record=True):
-            xm.save(self.lr_scheduler.state_dict(), os.path.join(output_dir, SCHEDULER_NAME))
+        self.accelerator.save_state(output_dir)
 
         # Save scaler
         # TODO: is grad scaling supported with TORCH XLA?
         # reissue_pt_warnings(caught_warnings)
         # if self.do_grad_scaling:
         #     xm.save(self.scaler.state_dict(), os.path.join(output_dir, SCALER_NAME))
 
@@ -308,18 +326,33 @@
             self._push_from_checkpoint(output_dir)
 
         # Maybe delete some older checkpoints.
         if self.args.should_save:
             self._rotate_checkpoints(use_mtime=True, output_dir=run_dir)
 
     def _save_checkpoint(self, model, trial, metrics=None):
-        if self.fsdp or self.is_fsdp_enabled:
-            return self._save_checkpoint_for_xla_fsdp(model, trial, metrics=metrics)
+        # if self.fsdp or self.is_fsdp_enabled:
+        if check_if_transformers_greater("4.30.0") and self.accelerator.distributed_type in [
+            NeuronDistributedType.XLA_FSDP,
+            NeuronDistributedType.TENSOR_PARALLELISM,
+        ]:
+            return self._save_checkpoint_with_accelerator(model, trial, metrics=metrics)
         return super()._save_checkpoint(model, trial, metrics=metrics)
 
+    def save_model(self, output_dir: Optional[str] = None, _internal_call: bool = False):
+        if output_dir is None:
+            output_dir = self.args.output_dir
+        if self.accelerator.distributed_type is NeuronDistributedType.XLA_FSDP:
+            self.accelerator.state.fsdp_plugin.save_model(self.accelerator, self.model, output_dir, 0)
+        elif self.accelerator.distributed_type is NeuronDistributedType.TENSOR_PARALLELISM:
+            parallelizer = ParallelizersManager.parallelizer_for_model(self.model)
+            parallelizer.save_model_checkpoint(self.model, output_dir, as_regular=False)
+        else:
+            return super().save_model(output_dir=output_dir, _internal_call=_internal_call)
+
     def _load_optimizer_and_scheduler_for_xla_fsdp(self, checkpoint):
         if checkpoint is None:
             return
         checkpoint_file_exists = (
             glob.glob(os.path.join(checkpoint, OPTIMIZER_NAME) + "_*")
             if is_sagemaker_mp_enabled()
             else os.path.isfile(os.path.join(checkpoint, OPTIMIZER_NAME))
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/training_args.py` & `optimum-neuron-0.0.7/optimum/neuron/training_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 """Defines a TrainingArguments class compatible with Trainium."""
 
 import io
 import json
 import os
 import warnings
+from dataclasses import dataclass, field
 from datetime import timedelta
 
 import torch
 from accelerate.utils import DistributedType
 from packaging import version
 from transformers.training_args import ParallelMode, TrainingArguments
 from transformers.training_args_seq2seq import Seq2SeqTrainingArguments
@@ -30,15 +31,15 @@
     is_sagemaker_dp_enabled,
     is_sagemaker_mp_enabled,
     requires_backends,
 )
 
 from ..utils import check_if_transformers_greater, logging
 from .accelerate import NeuronAcceleratorState, NeuronPartialState
-from .accelerate.utils import patch_accelerate_is_tpu_available
+from .accelerate.utils import TensorParallelismPlugin, patch_accelerate_is_tpu_available
 from .utils import is_accelerate_available, is_torch_xla_available
 from .utils.training_utils import TRANSFORMERS_MIN_VERSION_FOR_XLA_FSDP
 
 
 if is_sagemaker_mp_enabled():
     import smdistributed.modelparallel.torch as smp
 
@@ -75,14 +76,15 @@
             if not check_if_transformers_greater(TRANSFORMERS_MIN_VERSION_FOR_XLA_FSDP):
                 import transformers
 
                 raise RuntimeError(
                     "The minimal required Transformers version to perform XLA FSDP is "
                     f"{TRANSFORMERS_MIN_VERSION_FOR_XLA_FSDP} but {transformers.__version__} is installed."
                 )
+        self.tp_plugin = TensorParallelismPlugin(self.tensor_parallel_size)
         super().__post_init__()
 
     # Needed only to specialize the warning message for FSDP.
     @cached_property
     def _setup_devices(self) -> "torch.device":
         if not check_if_transformers_greater("4.30.0"):
             return super()._setup_devices
@@ -175,14 +177,24 @@
                 # Sometimes the line in the postinit has not been run before we end up here, so just checking we're not at
                 # the default value.
                 self._n_gpu = torch.cuda.device_count()
                 if device.type == "cuda":
                     torch.cuda.set_device(device)
         return device
 
+    @property
+    def place_model_on_device(self):
+        return not self.tp_plugin.should_parallelize and super().place_model_on_device
 
+
+@dataclass
 class TrainiumTrainingArguments(TrainiumTrainingArgumentsMixin, TrainingArguments):
-    pass
+    tensor_parallel_size: int = field(
+        default=1, metadata={"help": "The number of replicas the model will be sharded on."}
+    )
 
 
+@dataclass
 class Seq2SeqTrainiumTrainingArguments(TrainiumTrainingArgumentsMixin, Seq2SeqTrainingArguments):
-    pass
+    tensor_parallel_size: int = field(
+        default=1, metadata={"help": "The number of replicas the model will be sharded on."}
+    )
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .import_utils import (
     is_accelerate_available,
     is_neuron_available,
     is_neuronx_available,
     is_neuronx_distributed_available,
     is_torch_xla_available,
 )
+from .optimization_utils import get_attention_scores
 from .patching import DynamicPatch, ModelPatcher, Patcher, patch_everywhere, patch_within_function
 from .training_utils import (
     FirstAndLastDataset,
     is_model_officially_supported,
     is_precompilation,
     patch_transformers_for_neuron_sdk,
     patched_finfo,
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/argument_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities related to CLI arguments."""
 
 import os
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
+from collections import OrderedDict
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 from ...utils import logging
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
@@ -132,28 +133,39 @@
     if disable_fast_relayout is True:
         compiler_args.append("no-fast-relayout")
 
     return compiler_args
 
 
 def store_compilation_config(
-    config: "PretrainedConfig",
+    config: Union["PretrainedConfig", OrderedDict],
     input_shapes: Dict[str, int],
     compiler_kwargs: Dict[str, Any],
     input_names: List[str],
     output_names: List[str],
     dynamic_batch_size: bool,
+    neuron_compiler: str,
+    neuron_compiler_version: str,
     **kwargs,
 ):
+    if isinstance(config, OrderedDict):
+        update_func = config.__setitem__
+    else:
+        update_func = config.__setattr__
+
+    # Add neuron version to the config, so it can be checked at load time
+    update_func("neuron_compiler", neuron_compiler)
+    update_func("neuron_compiler_version", neuron_compiler_version)
+
     # Add input shapes during compilation to the config
     for axe, shape in input_shapes.items():
         axe = f"neuron_{axe}"
-        config.__setattr__(axe, shape)
+        update_func(axe, shape)
 
-    config.__setattr__("dynamic_batch_size", dynamic_batch_size)
+    update_func("dynamic_batch_size", dynamic_batch_size)
 
     # Add compilation args to the config
     for arg, value in compiler_kwargs.items():
-        config.__setattr__(arg, value)
+        update_func(arg, value)
 
     config.input_names = input_names
     config.output_names = output_names
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/cache_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     HfApi,
     HfFolder,
     RepoUrl,
     create_repo,
     hf_hub_download,
 )
 from huggingface_hub.utils import EntryNotFoundError, HfHubHTTPError, RepositoryNotFoundError
+from packaging import version
 
 from ...utils import logging
 from ...utils.logging import warn_once
 from .version_utils import get_neuronxcc_version
 
 
 if TYPE_CHECKING:
@@ -74,14 +75,28 @@
 _IP_PATTERN = re.compile(r"ip-([0-9]{1,3}-){4}")
 _HF_HUB_HTTP_ERROR_REQUEST_ID_PATTERN = re.compile(r"\(Request ID: Root=[\w-]+\)")
 
 _WRITING_ACCESS_CACHE: Dict[Tuple[str, str], bool] = {}
 _REGISTRY_FILE_EXISTS: Dict[str, bool] = {}
 _ADDED_IN_REGISTRY: Dict[Tuple[str, "NeuronHash"], bool] = {}
 
+_NEW_CACHE_NAMING_CONVENTION_NEURONXCC_VERSION = "2.7.0.40+f7c6cf2a3"
+
+
+def follows_new_cache_naming_convention(neuronxcc_version: Optional[str] = None) -> bool:
+    """
+    The ways the cache is handled differs starting from `_NEW_CACHE_NAMING_CONVENTION_NEURONXCC_VERSION`.
+    This helper functions returns `True` if `neuronxcc_version` follows the new way the cache is handled and `False`
+    otherwise.
+    """
+    if neuronxcc_version is None:
+        neuronxcc_version = get_neuronxcc_version()
+    neuronxcc_version = version.parse(neuronxcc_version)
+    return neuronxcc_version >= version.parse(_NEW_CACHE_NAMING_CONVENTION_NEURONXCC_VERSION)
+
 
 def load_custom_cache_repo_name_from_hf_home(
     hf_home_cache_repo_file: Union[str, Path] = HF_HOME_CACHE_REPO_FILE
 ) -> Optional[str]:
     if Path(hf_home_cache_repo_file).exists():
         with open(hf_home_cache_repo_file, "r") as fp:
             return fp.read()
@@ -136,20 +151,20 @@
     if (token, repo_id) in _WRITING_ACCESS_CACHE:
         return _WRITING_ACCESS_CACHE[(token, repo_id)]
 
     has_access = False
     with tempfile.NamedTemporaryFile() as fp:
         tmpfilename = Path(fp.name)
         try:
-            add_file = CommitOperationAdd(tmpfilename.name, tmpfilename.as_posix())
+            add_file = CommitOperationAdd(f"write_access_test/{tmpfilename.name}", tmpfilename.as_posix())
             HfApi().create_commit(repo_id, operations=[add_file], commit_message="Check write access")
         except (HfHubHTTPError, RepositoryNotFoundError):
             pass
         else:
-            delete_file = CommitOperationDelete(tmpfilename.name)
+            delete_file = CommitOperationDelete(f"write_access_test/{tmpfilename.name}")
             HfApi().create_commit(repo_id, operations=[delete_file], commit_message="Check write access [DONE]")
             has_access = True
 
     _WRITING_ACCESS_CACHE[(token, repo_id)] = has_access
     return has_access
 
 
@@ -204,15 +219,19 @@
     else:
         match_ = re.search(r"--cache_dir=([\w\/]+)", neuron_cc_flags)
         if match_:
             path = Path(match_.group(1))
         else:
             path = Path("/var/tmp")
 
-        return path / NEURON_COMPILE_CACHE_NAME
+        # TODO: is that correct?
+        if not follows_new_cache_naming_convention():
+            path = path / NEURON_COMPILE_CACHE_NAME
+
+        return path
 
 
 def set_neuron_cache_path(neuron_cache_path: Union[str, Path], ignore_no_cache: bool = False):
     # NEURON_CC_FLAGS is the environment variable read by the neuron compiler.
     # Among other things, this is where the cache directory is specified.
     neuron_cc_flags = os.environ.get("NEURON_CC_FLAGS", "")
     if "--no-cache" in neuron_cc_flags:
@@ -385,17 +404,17 @@
     model_name_or_path_or_hash: Optional[str] = None,
     neuron_compiler_version: Optional[str] = None,
 ) -> List[str]:
     entries = []
     if neuron_compiler_version is not None:
         registry = registry.get(neuron_compiler_version, {})
     else:
-        for version in registry:
+        for version_ in registry:
             entries += _list_in_registry_dict(
-                registry, model_name_or_path_or_hash=model_name_or_path_or_hash, neuron_compiler_version=version
+                registry, model_name_or_path_or_hash=model_name_or_path_or_hash, neuron_compiler_version=version_
             )
         return entries
 
     def validate_features_input_shapes(input_shapes: Tuple[Tuple[str, Tuple[int, ...]], ...]) -> bool:
         return len(input_shapes) > 0 and all(len(entry) == 2 for entry in input_shapes)
 
     # model_key is either a model name or path or a model hash.
@@ -473,32 +492,96 @@
         return (not self.model_hash) or (not self.overall_hash)
 
     def __hash__(self):
         return hash(f"{self.model_hash}_{self.overall_hash}")
 
 
 @dataclass(frozen=True)
+class _UnspecifiedHashAttribute:
+    min_optimum_neuron_version: Optional[str] = None
+    min_neuron_compiler_version: Optional[str] = None
+    default: Optional[Any] = None
+
+    @classmethod
+    def with_args(
+        cls,
+        min_optimum_neuron_version: Optional[str] = None,
+        min_neuron_compiler_version: Optional[str] = None,
+        default: Optional[Any] = None,
+    ) -> Callable[[], "_UnspecifiedHashAttribute"]:
+        def constructor():
+            return cls(
+                min_optimum_neuron_version=min_optimum_neuron_version,
+                min_neuron_compiler_version=min_neuron_compiler_version,
+                default=default,
+            )
+
+        return constructor
+
+    def check_requirements_are_met(self, neuron_compiler_version: str):
+        from ..version import __version__
+
+        optimum_neuron_requirement = True
+        if self.min_optimum_neuron_version is not None:
+            if version.parse(__version__) >= version.parse(self.min_optimum_neuron_version):
+                optimum_neuron_requirement = self.default is not None
+
+        neuron_compiler_requirement = True
+        if self.min_neuron_compiler_version is not None:
+            if version.parse(neuron_compiler_version) >= version.parse(self.min_neuron_compiler_version):
+                neuron_compiler_requirement = self.default is not None
+
+        if not optimum_neuron_requirement or not neuron_compiler_requirement:
+            raise ValueError("A default value must be specified.")
+
+
+@dataclass(frozen=True)
 class NeuronHash:
     model: "PreTrainedModel"
     input_shapes: Tuple[Tuple[str, Tuple[int, ...]], ...]
     data_type: torch.dtype
     num_neuron_cores: int = field(default_factory=get_num_neuron_cores_used)
     neuron_compiler_version: str = field(default_factory=get_neuronxcc_version)
+    fsdp: Union[int, _UnspecifiedHashAttribute] = field(
+        default_factory=_UnspecifiedHashAttribute.with_args(min_optimum_neuron_version="0.0.8", default=False)
+    )
+    tensor_parallel_size: Union[int, _UnspecifiedHashAttribute] = field(
+        default_factory=_UnspecifiedHashAttribute.with_args(min_optimum_neuron_version="0.0.8", default=1)
+    )
     _hash: _MutableHashAttribute = field(default_factory=_MutableHashAttribute)
 
     def __post_init__(self):
+        for attr in self.__dict__.values():
+            if isinstance(attr, _UnspecifiedHashAttribute):
+                attr.check_requirements_are_met(self.neuron_compiler_version)
         self.compute_hash()
 
+    def _insert_potential_unspecified_hash_attribute(
+        self, attribute_name: str, attribute: Any, hash_dict: Dict[str, Any]
+    ):
+        """
+        Inserts `attribute` in `hash_dict` only if it is a specified attribute or if it has a default value.
+        """
+        if isinstance(attribute, _UnspecifiedHashAttribute):
+            if attribute.default is not None:
+                hash_dict[attribute_name] = attribute
+        else:
+            hash_dict[attribute_name] = attribute
+
     @property
     def hash_dict(self) -> Dict[str, Any]:
         hash_dict = asdict(self)
         hash_dict["model"] = hash_dict["model"].state_dict()
         hash_dict["_model_class"] = self.model.__class__
         hash_dict["_is_model_training"] = self.model.training
         hash_dict.pop("_hash")
+
+        self._insert_potential_unspecified_hash_attribute("tensor_parallel_size", self.tensor_parallel_size, hash_dict)
+        self._insert_potential_unspecified_hash_attribute("fsdp", self.fsdp, hash_dict)
+
         return hash_dict
 
     def state_dict_to_bytes(self, state_dict: Dict[str, torch.Tensor]) -> bytes:
         bytes_to_join = []
         for name, tensor in state_dict.items():
             memfile = io.BytesIO()
             np.save(memfile, tensor.cpu().numpy())
@@ -540,14 +623,16 @@
 
     @property
     def cache_path(self) -> Path:
         return Path().joinpath(*self.folders)
 
     @property
     def neuron_compiler_version_dir_name(self):
+        if follows_new_cache_naming_convention():
+            return f"neuronxcc-{self.neuron_compiler_version}"
         return f"USER_neuroncc-{self.neuron_compiler_version}"
 
     @property
     def is_private(self):
         private = None
         model_name_or_path = _get_model_name_or_path(self.model.config)
         if model_name_or_path is None:
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/compilation_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/constant.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/misc.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/patching.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/patching.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,16 +79,21 @@
             module_qualified_name, attribute_name = orig.rsplit(".", maxsplit=1)
             module = importlib.import_module(module_qualified_name)
             module_has_attr = hasattr(module, attribute_name)
             if module_has_attr:
                 attribute = getattr(module, attribute_name)
             elif ignore_missing_attributes and not isinstance(patch, DynamicPatch):
                 attribute = None
-            else:
+            elif isinstance(patch, DynamicPatch):
                 raise ValueError("Cannot ignore missing attribute with a DynamicPatch.")
+            else:
+                raise AttributeError(
+                    f"Attribute {attribute_name} does not exist in {module}, set `ignore_missing_attributes=True` "
+                    "to allow not failing when an attribute does not exist."
+                )
             if isinstance(patch, DynamicPatch):
                 patch = patch(attribute)
             proccessed_patching_specs.append((module, attribute_name, attribute, patch))
         return proccessed_patching_specs
 
 
 class ModelPatcher(BasePatcher):
@@ -110,16 +115,21 @@
                 module = getattr(module, name)
 
             module_has_attr = hasattr(module, attribute_name)
             if module_has_attr:
                 attribute = getattr(module, attribute_name)
             elif ignore_missing_attributes and not isinstance(patch, DynamicPatch):
                 attribute = None
-            else:
+            elif isinstance(patch, DynamicPatch):
                 raise ValueError("Cannot ignore missing attribute with a DynamicPatch.")
+            else:
+                raise AttributeError(
+                    f"Attribute {attribute_name} does not exist in {module}, set `ignore_missing_attributes=True` "
+                    "to allow not failing when an attribute does not exist."
+                )
 
             if isinstance(patch, DynamicPatch):
                 patch = patch(attribute)
 
             if inspect.ismethod(attribute):
                 patch = patch.__get__(model)
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/utils/training_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     ("albert", ("sequence-classification", "token-classification", "question-answering")),
     "bart",
     "bert",
     "camembert",
     "distilbert",
     "electra",
     "gpt-2",
-    "gpt-neo",
+    "gpt_neo",
     "marian",
     "roberta",
     "t5",
     "vit",
     ("xlm-roberta", ("sequence-classification", "token-classification", "question-answering")),
 ]
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.7/optimum/neuron/pipelines/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # coding=utf-8
-# Copyright 2023 The HuggingFace Inc. team. All rights reserved.
+# Copyright 2023 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Version utilities."""
 
-
-def get_neuronxcc_version() -> str:
-    try:
-        import neuronxcc
-    except ImportError:
-        raise ValueError("NeuronX Compiler python package is not installed.")
-    return neuronxcc.__version__
+from .transformers import (
+    pipeline,
+)
```

### Comparing `optimum-neuron-0.0.6/optimum/neuron/version.py` & `optimum-neuron-0.0.7/optimum/neuron/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
```

### Comparing `optimum-neuron-0.0.6/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.7/optimum_neuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.6/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.7/optimum_neuron.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 optimum/commands/register/register_neuron.py
 optimum/exporters/neuron/__init__.py
 optimum/exporters/neuron/__main__.py
 optimum/exporters/neuron/base.py
 optimum/exporters/neuron/config.py
 optimum/exporters/neuron/convert.py
 optimum/exporters/neuron/model_configs.py
+optimum/exporters/neuron/utils.py
 optimum/neuron/__init__.py
 optimum/neuron/hf_argparser.py
 optimum/neuron/modeling.py
 optimum/neuron/modeling_base.py
 optimum/neuron/trainer_callback.py
 optimum/neuron/trainers.py
 optimum/neuron/training_args.py
@@ -30,26 +31,32 @@
 optimum/neuron/accelerate/scheduler.py
 optimum/neuron/accelerate/state.py
 optimum/neuron/accelerate/utils/__init__.py
 optimum/neuron/accelerate/utils/dataclasses.py
 optimum/neuron/accelerate/utils/misc.py
 optimum/neuron/distributed/__init__.py
 optimum/neuron/distributed/base.py
+optimum/neuron/distributed/decoder_models.py
 optimum/neuron/distributed/encoder_models.py
+optimum/neuron/distributed/parallel_layers.py
 optimum/neuron/distributed/parallelizers_manager.py
 optimum/neuron/distributed/utils.py
 optimum/neuron/generation/__init__.py
 optimum/neuron/generation/utils.py
+optimum/neuron/pipelines/__init__.py
+optimum/neuron/pipelines/transformers/__init__.py
+optimum/neuron/pipelines/transformers/base.py
 optimum/neuron/utils/__init__.py
 optimum/neuron/utils/argument_utils.py
 optimum/neuron/utils/cache_utils.py
 optimum/neuron/utils/compilation_utils.py
 optimum/neuron/utils/constant.py
 optimum/neuron/utils/import_utils.py
 optimum/neuron/utils/misc.py
+optimum/neuron/utils/optimization_utils.py
 optimum/neuron/utils/patching.py
 optimum/neuron/utils/testing_utils.py
 optimum/neuron/utils/training_utils.py
 optimum/neuron/utils/version_utils.py
 optimum_neuron.egg-info/PKG-INFO
 optimum_neuron.egg-info/SOURCES.txt
 optimum_neuron.egg-info/dependency_links.txt
```

### Comparing `optimum-neuron-0.0.6/pyproject.toml` & `optimum-neuron-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/setup.py` & `optimum-neuron-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_cache_utils.py` & `optimum-neuron-0.0.7/tests/test_cache_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     NEURON_COMPILE_CACHE_NAME,
     REGISTRY_FILENAME,
     NeuronHash,
     _list_in_registry_dict,
     add_in_registry,
     create_registry_file_if_does_not_exist,
     download_cached_model_from_hub,
+    follows_new_cache_naming_convention,
     get_cached_model_on_the_hub,
     get_neuron_cache_path,
     get_num_neuron_cores_used,
     has_write_access_to_repo,
     list_files_in_neuron_cache,
     list_in_registry,
     load_custom_cache_repo_name_from_hf_home,
@@ -58,14 +59,15 @@
 
 from .utils import MyTinyModel, StagingTestMixin, get_random_string
 
 
 DUMMY_COMPILER_VERSION = "1.2.3"
 
 
+@is_trainium_test
 class NeuronUtilsTestCase(TestCase):
     def test_load_custom_cache_repo_name_from_hf_home(self):
         with TemporaryDirectory() as tmpdirname:
             hf_home_cache_repo_file = f"{tmpdirname}/{CACHE_REPO_FILENAME}"
             with open(hf_home_cache_repo_file, "w") as fp:
                 fp.write("blablabla")
             self.assertEqual(load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file), "blablabla")
@@ -77,31 +79,43 @@
         os.environ["NEURON_CC_FLAGS"] = "--some --parameters --here --no-cache --other --paremeters --here"
         assert get_neuron_cache_path() is None
 
         custom_cache_dir_name = Path("_this/is_/my1/2custom/cache/dir")
         os.environ[
             "NEURON_CC_FLAGS"
         ] = f"--some --parameters --here --cache_dir={custom_cache_dir_name} --other --paremeters --here"
-        self.assertEqual(get_neuron_cache_path(), custom_cache_dir_name / NEURON_COMPILE_CACHE_NAME)
+        if follows_new_cache_naming_convention():
+            self.assertEqual(get_neuron_cache_path(), custom_cache_dir_name)
+        else:
+            self.assertEqual(get_neuron_cache_path(), custom_cache_dir_name / NEURON_COMPILE_CACHE_NAME)
 
         os.environ["NEURON_CC_FLAGS"] = "--some --parameters --here --other --paremeters --here"
-        self.assertEqual(get_neuron_cache_path(), Path("/var/tmp") / NEURON_COMPILE_CACHE_NAME)
+        if follows_new_cache_naming_convention():
+            self.assertEqual(get_neuron_cache_path(), Path("/var/tmp"))
+        else:
+            self.assertEqual(get_neuron_cache_path(), Path("/var/tmp") / NEURON_COMPILE_CACHE_NAME)
 
     def _test_set_neuron_cache_path(self, new_cache_path):
         os.environ["NEURON_CC_FLAGS"] = "--some --parameters --here --no-cache --other --paremeters --here"
         with self.assertRaisesRegex(ValueError, expected_regex=r"Cannot set the neuron compile cache"):
             set_neuron_cache_path(new_cache_path)
         set_neuron_cache_path(new_cache_path, ignore_no_cache=True)
-        self.assertEqual(get_neuron_cache_path(), Path(new_cache_path) / NEURON_COMPILE_CACHE_NAME)
+        if follows_new_cache_naming_convention():
+            self.assertEqual(get_neuron_cache_path(), Path(new_cache_path))
+        else:
+            self.assertEqual(get_neuron_cache_path(), Path(new_cache_path) / NEURON_COMPILE_CACHE_NAME)
 
         os.environ[
             "NEURON_CC_FLAGS"
         ] = "--some --parameters --here --cache_dir=original_cache_dir --other --paremeters"
         set_neuron_cache_path(new_cache_path)
-        self.assertEqual(get_neuron_cache_path(), Path(new_cache_path) / NEURON_COMPILE_CACHE_NAME)
+        if follows_new_cache_naming_convention():
+            self.assertEqual(get_neuron_cache_path(), Path(new_cache_path))
+        else:
+            self.assertEqual(get_neuron_cache_path(), Path(new_cache_path) / NEURON_COMPILE_CACHE_NAME)
 
     def test_set_neuron_cache_path(self):
         new_cache_path_str = "path/to/my/custom/cache"
         new_cache_path_path = Path(new_cache_path_str)
         self._test_set_neuron_cache_path(new_cache_path_str)
         self._test_set_neuron_cache_path(new_cache_path_path)
```

### Comparing `optimum-neuron-0.0.6/tests/test_compilation_utils.py` & `optimum-neuron-0.0.7/tests/test_compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_examples.py` & `optimum-neuron-0.0.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_generate.py` & `optimum-neuron-0.0.7/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_modeling.py` & `optimum-neuron-0.0.7/tests/test_modeling.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,23 +29,25 @@
     AutoModelForQuestionAnswering,
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
     AutoTokenizer,
     PretrainedConfig,
     set_seed,
 )
+from transformers.onnx.utils import get_preprocessor
 
 from optimum.neuron import (
     NeuronBaseModel,
     NeuronModelForFeatureExtraction,
     NeuronModelForMaskedLM,
     NeuronModelForMultipleChoice,
     NeuronModelForQuestionAnswering,
     NeuronModelForSequenceClassification,
     NeuronModelForTokenClassification,
+    pipeline,
 )
 from optimum.neuron.utils import NEURON_FILE_NAME, is_neuron_available, is_neuronx_available
 from optimum.neuron.utils.testing_utils import is_inferentia_test
 from optimum.utils import (
     CONFIG_NAME,
     logging,
 )
@@ -331,14 +333,30 @@
                     transformers_outputs.pooler_output,
                     atol=self.ATOL_FOR_VALIDATION,
                 )
             )
 
         gc.collect()
 
+    @parameterized.expand(SUPPORTED_ARCHITECTURES, skip_on_empty=True)
+    def test_pipeline_model(self, model_arch):
+        model_args = {"test_name": model_arch, "model_arch": model_arch}
+        self._setup(model_args)
+
+        model_id = self.ARCH_MODEL_MAP[model_arch] if model_arch in self.ARCH_MODEL_MAP else MODEL_NAMES[model_arch]
+        neuron_model = NeuronModelForSequenceClassification.from_pretrained(self.neuron_model_dirs[model_arch])
+        tokenizer = get_preprocessor(model_id)
+        pipe = pipeline(self.TASK, model=neuron_model, tokenizer=tokenizer)
+        text = "My Name is Philipp."
+        outputs = pipe(text)
+
+        self.assertTrue(all(all(isinstance(item, float) for item in row) for row in outputs[0]))
+
+        gc.collect()
+
 
 @is_inferentia_test
 class NeuronModelForMaskedLMIntegrationTest(NeuronModelTestMixin):
     NEURON_MODEL_CLASS = NeuronModelForMaskedLM
     TASK = "fill-mask"
     if is_neuron_available():
         ATOL_FOR_VALIDATION = 1e-2  # Not good enough, needs to be further investigate
@@ -478,14 +496,32 @@
         )
 
         with self.assertRaises(Exception) as context:
             _ = neuron_model_non_dyn(**tokens)
 
         self.assertIn("set `dynamic_batch_size=True` during the compilation", str(context.exception))
 
+    @parameterized.expand(SUPPORTED_ARCHITECTURES, skip_on_empty=True)
+    def test_pipeline_model(self, model_arch):
+        model_args = {"test_name": model_arch, "model_arch": model_arch}
+        self._setup(model_args)
+
+        model_id = self.ARCH_MODEL_MAP[model_arch] if model_arch in self.ARCH_MODEL_MAP else MODEL_NAMES[model_arch]
+        neuron_model = NeuronModelForSequenceClassification.from_pretrained(self.neuron_model_dirs[model_arch])
+        tokenizer = get_preprocessor(model_id)
+        MASK_TOKEN = tokenizer.mask_token
+        pipe = pipeline(self.TASK, model=neuron_model, tokenizer=tokenizer)
+        text = f"The capital of France is {MASK_TOKEN}."
+        outputs = pipe(text)
+
+        self.assertGreaterEqual(outputs[0]["score"], 0.0)
+        self.assertTrue(isinstance(outputs[0]["token_str"], str))
+
+        gc.collect()
+
 
 @is_inferentia_test
 class NeuronModelForQuestionAnsweringIntegrationTest(NeuronModelTestMixin):
     NEURON_MODEL_CLASS = NeuronModelForQuestionAnswering
     TASK = "question-answering"
     if is_neuron_available():
         ATOL_FOR_VALIDATION = 1e-2  # Not good enough, needs to be further investigate
@@ -657,14 +693,32 @@
         )
 
         with self.assertRaises(Exception) as context:
             _ = neuron_model_non_dyn(**tokens)
 
         self.assertIn("set `dynamic_batch_size=True` during the compilation", str(context.exception))
 
+    @parameterized.expand(SUPPORTED_ARCHITECTURES, skip_on_empty=True)
+    def test_pipeline_model(self, model_arch):
+        model_args = {"test_name": model_arch, "model_arch": model_arch}
+        self._setup(model_args)
+
+        model_id = self.ARCH_MODEL_MAP[model_arch] if model_arch in self.ARCH_MODEL_MAP else MODEL_NAMES[model_arch]
+        neuron_model = NeuronModelForQuestionAnswering.from_pretrained(self.neuron_model_dirs[model_arch])
+        tokenizer = get_preprocessor(model_id)
+        pipe = pipeline(self.TASK, model=neuron_model, tokenizer=tokenizer)
+        question = "Whats my name?"
+        context = "My Name is Philipp."
+        outputs = pipe(question, context)
+
+        self.assertGreaterEqual(outputs["score"], 0.0)
+        self.assertIsInstance(outputs["answer"], str)
+
+        gc.collect()
+
 
 @is_inferentia_test
 class NeuronModelForSequenceClassificationIntegrationTest(NeuronModelTestMixin):
     NEURON_MODEL_CLASS = NeuronModelForSequenceClassification
     TASK = "text-classification"
     if is_neuron_available():
         ATOL_FOR_VALIDATION = 1e-2  # Not good enough, needs to be further investigate
@@ -806,14 +860,31 @@
         )
 
         with self.assertRaises(Exception) as context:
             _ = neuron_model_non_dyn(**tokens)
 
         self.assertIn("set `dynamic_batch_size=True` during the compilation", str(context.exception))
 
+    @parameterized.expand(SUPPORTED_ARCHITECTURES, skip_on_empty=True)
+    def test_pipeline_model(self, model_arch):
+        model_args = {"test_name": model_arch, "model_arch": model_arch}
+        self._setup(model_args)
+
+        model_id = self.ARCH_MODEL_MAP[model_arch] if model_arch in self.ARCH_MODEL_MAP else MODEL_NAMES[model_arch]
+        neuron_model = NeuronModelForSequenceClassification.from_pretrained(self.neuron_model_dirs[model_arch])
+        tokenizer = get_preprocessor(model_id)
+        pipe = pipeline(self.TASK, model=neuron_model, tokenizer=tokenizer)
+        text = "I like you."
+        outputs = pipe(text)
+
+        self.assertGreaterEqual(outputs[0]["score"], 0.0)
+        self.assertIsInstance(outputs[0]["label"], str)
+
+        gc.collect()
+
 
 @is_inferentia_test
 class NeuronModelForTokenClassificationIntegrationTest(NeuronModelTestMixin):
     NEURON_MODEL_CLASS = NeuronModelForTokenClassification
     TASK = "token-classification"
     if is_neuron_available():
         ATOL_FOR_VALIDATION = 1e-2  # Not good enough, needs to be further investigate
@@ -955,14 +1026,30 @@
         )
 
         with self.assertRaises(Exception) as context:
             _ = neuron_model_non_dyn(**tokens)
 
         self.assertIn("set `dynamic_batch_size=True` during the compilation", str(context.exception))
 
+    @parameterized.expand(SUPPORTED_ARCHITECTURES, skip_on_empty=True)
+    def test_pipeline_model(self, model_arch):
+        model_args = {"test_name": model_arch, "model_arch": model_arch}
+        self._setup(model_args)
+
+        model_id = self.ARCH_MODEL_MAP[model_arch] if model_arch in self.ARCH_MODEL_MAP else MODEL_NAMES[model_arch]
+        neuron_model = NeuronModelForTokenClassification.from_pretrained(self.neuron_model_dirs[model_arch])
+        tokenizer = get_preprocessor(model_id)
+        pipe = pipeline(self.TASK, model=neuron_model, tokenizer=tokenizer)
+        text = "My Name is Philipp."
+        outputs = pipe(text)
+
+        self.assertTrue(all(item["score"] > 0.0 for item in outputs))
+
+        gc.collect()
+
 
 @is_inferentia_test
 class NeuronModelForMultipleChoiceIntegrationTest(NeuronModelTestMixin):
     NEURON_MODEL_CLASS = NeuronModelForMultipleChoice
     TASK = "multiple-choice"
     STATIC_INPUTS_SHAPES = {"batch_size": 1, "num_choices": 4, "sequence_length": 128}
     if is_neuron_available():
```

### Comparing `optimum-neuron-0.0.6/tests/test_trainer_callback.py` & `optimum-neuron-0.0.7/tests/test_trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_trainers.py` & `optimum-neuron-0.0.7/tests/test_trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.6/tests/test_utils.py` & `optimum-neuron-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

