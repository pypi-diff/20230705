# Comparing `tmp/torchtnt-nightly-2023.7.3.tar.gz` & `tmp/torchtnt-nightly-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.7.3.tar", last modified: Mon Jul  3 11:23:59 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.7.4.tar", last modified: Tue Jul  4 11:25:00 2023, max compression
```

## Comparing `torchtnt-nightly-2023.7.3.tar` & `torchtnt-nightly-2023.7.4.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.248587 torchtnt-nightly-2023.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-03 11:23:59.248587 torchtnt-nightly-2023.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:23:59.248587 torchtnt-nightly-2023.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.236587 torchtnt-nightly-2023.7.3/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.240587 torchtnt-nightly-2023.7.3/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40669 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.240587 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.244587 torchtnt-nightly-2023.7.3/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.244587 torchtnt-nightly-2023.7.3/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.248587 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 11:22:15.000000 torchtnt-nightly-2023.7.3/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:23:59.248587 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:23:59.000000 torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.406852 torchtnt-nightly-2023.7.4/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.410852 torchtnt-nightly-2023.7.4/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36195 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.410852 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.410852 torchtnt-nightly-2023.7.4/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/prepare_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-04 11:23:35.000000 torchtnt-nightly-2023.7.4/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:25:00.414852 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:25:00.000000 torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.7.3/LICENSE` & `torchtnt-nightly-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/PKG-INFO` & `torchtnt-nightly-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.3/README.md` & `torchtnt-nightly-2023.7.4/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/setup.py` & `torchtnt-nightly-2023.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/auto_unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,120 +6,58 @@
 
 # ignore errors due to `Any` type
 # pyre-ignore-all-errors[2]
 # pyre-ignore-all-errors[3]
 
 import contextlib
 from abc import ABCMeta, abstractmethod
-from dataclasses import asdict, dataclass
+from dataclasses import dataclass
 from functools import partial
-from typing import Any, Callable, Iterable, Iterator, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Iterator, Optional, Tuple, TypeVar, Union
 
 import torch
-import torch.distributed as dist
-
 from pyre_extensions import none_throws
 from torch.cuda.amp import GradScaler
-from torch.distributed import ProcessGroup
-
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     apply_activation_checkpointing,
     checkpoint_wrapper,
     CheckpointImpl,
 )
-from torch.distributed.fsdp import FullyShardedDataParallel as FSDP, StateDictType
-from torch.distributed.fsdp.api import OptimStateDictConfig, StateDictConfig
-from torch.distributed.fsdp.fully_sharded_data_parallel import (
-    BackwardPrefetch,
-    CPUOffload,
-    MixedPrecision,
-    ShardingStrategy,
-)
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim.swa_utils import AveragedModel, SWALR
 from torchtnt.framework.state import ActivePhase, State
 from torchtnt.framework.unit import EvalUnit, PredictUnit, TPredictData, TrainUnit
 from torchtnt.framework.utils import (
     _get_timing_context,
     _is_fsdp_module,
     get_current_progress,
 )
 from torchtnt.utils import (
     init_from_env,
-    is_torch_version_geq_1_12,
     TLRScheduler,
     transfer_batch_norm_stats,
     transfer_weights,
 )
 from torchtnt.utils.device import copy_data_to_device, record_data_in_stream
+from torchtnt.utils.prepare_model import (
+    DDPStrategy,
+    FSDPStrategy,
+    prepare_ddp,
+    prepare_fsdp,
+    Strategy,
+)
 from torchtnt.utils.rank_zero_log import rank_zero_warn
 from torchtnt.utils.version import is_torch_version_ge_1_13_1
 from typing_extensions import Literal
 
 TSWA_avg_fn = Callable[[torch.Tensor, torch.Tensor, int], torch.Tensor]
 
 
 @dataclass
-class Strategy:
-    """Dataclass representing the parallelization strategy for the AutoUnit"""
-
-    pass
-
-
-@dataclass
-class DDPStrategy(Strategy):
-    """
-    Dataclass representing the `DistributedDataParallel <https://pytorch.org/docs/stable/generated/torch.nn.parallel.DistributedDataParallel.html>`_ strategy.
-    Includes params for registering `DDP communication hooks <https://pytorch.org/docs/stable/ddp_comm_hooks.html>`_ and `syncing batch norm <https://pytorch.org/docs/stable/generated/torch.nn.SyncBatchNorm.html>`_.
-    """
-
-    # DDP Constructor params
-    output_device: Optional[Union[int, torch.device]] = None
-    dim: int = 0
-    broadcast_buffers: bool = True
-    process_group: Optional[ProcessGroup] = None
-    bucket_cap_mb: int = 25
-    find_unused_parameters: bool = False
-    check_reduction: bool = False
-    gradient_as_bucket_view: bool = False
-    static_graph: bool = False
-
-    # DDP Comm Hook params
-    comm_state: Optional[object] = None
-    comm_hook: Optional[
-        Callable[[object, dist.GradBucket], torch.futures.Future[torch.Tensor]]
-    ] = None
-
-    # SyncBatchNorm params
-    sync_batchnorm: bool = True
-
-
-@dataclass
-class FSDPStrategy(Strategy):
-    """Dataclass representing the `FullyShardedDataParallel <https://pytorch.org/docs/stable/fsdp.html>`_ strategy"""
-
-    process_group: Optional[ProcessGroup] = None
-    sharding_strategy: Optional[ShardingStrategy] = None
-    cpu_offload: Optional[CPUOffload] = None
-    auto_wrap_policy: Optional[Callable[[torch.nn.Module, bool, int], bool]] = None
-    backward_prefetch: Optional[BackwardPrefetch] = None
-    ignored_modules: Optional[Iterable[torch.nn.Module]] = None
-    sync_module_states: bool = False
-    forward_prefetch: bool = False
-    limit_all_gathers: bool = False
-    use_orig_params: bool = False
-
-    # FSDP set_state_dict_type params: https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.set_state_dict_type
-    # for setting type of state dict for checkpointing
-    state_dict_type: Optional[StateDictType] = None
-    state_dict_config: Optional[StateDictConfig] = None
-    optim_state_dict_config: Optional[OptimStateDictConfig] = None
-
-
-@dataclass
 class SWAParams:
     """
     Dataclass to store parameters for stochastic weight averaging.
 
     Args:
         epoch_start: number of epochs to wait for before starting SWA
         anneal_epochs: number of epochs to anneal the SWA Scheduler to the learning rate (lr)
@@ -251,21 +189,25 @@
             dtype=self.precision,
             enabled=self.precision is not None,
         )
         if strategy:
             if isinstance(strategy, str):
                 strategy = _convert_str_to_strategy(strategy)
             if isinstance(strategy, DDPStrategy):
-                module = _prepare_ddp(module, strategy, self.device, torchdynamo_params)
+                if torchdynamo_params:
+                    # TODO: Add support for dynamo and DDP
+                    rank_zero_warn(
+                        "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
+                    )
+                module = prepare_ddp(module, self.device, strategy)
             elif isinstance(strategy, FSDPStrategy):
-                module = _prepare_fsdp(
+                module = prepare_fsdp(
                     module,
-                    strategy,
                     self.device,
-                    None,  # SWA params
+                    strategy,
                     self.precision,
                 )
         else:
             module = module.to(self.device)
         if torchdynamo_params:
             module = _dynamo_wrapper(module, torchdynamo_params)
         self.module: torch.nn.Module = module
@@ -469,19 +411,26 @@
         else:
             self.precision = precision
 
         if strategy:
             if isinstance(strategy, str):
                 strategy = _convert_str_to_strategy(strategy)
             if isinstance(strategy, DDPStrategy):
-                module = _prepare_ddp(module, strategy, self.device, torchdynamo_params)
+                if torchdynamo_params:
+                    # TODO: Add support for dynamo and DDP
+                    rank_zero_warn(
+                        "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
+                    )
+                module = prepare_ddp(module, self.device, strategy)
             elif isinstance(strategy, FSDPStrategy):
-                module = _prepare_fsdp(
-                    module, strategy, self.device, swa_params, self.precision
-                )
+                if swa_params:
+                    raise RuntimeError(
+                        "Stochastic Weight Averaging is currently not supported with the FSDP strategy"
+                    )
+                module = prepare_fsdp(module, self.device, strategy, self.precision)
         else:
             module = module.to(self.device)
 
         if activation_checkpoint_params:
             checkpoint_impl = activation_checkpoint_params.checkpoint_impl
             check_fn = activation_checkpoint_params.check_fn
             custom_checkpoint_wrapper = partial(
@@ -664,15 +613,14 @@
         module = self.module
 
         # if using gradient accumulation with either DDP or FSDP, when in a step where we will not update the weights,
         # run forward and backward in no_sync context
         # https://pytorch.org/docs/stable/_modules/torch/nn/parallel/distributed.html#DistributedDataParallel.no_sync
         # https://pytorch.org/docs/stable/fsdp.html#torch.distributed.fsdp.FullyShardedDataParallel.no_sync
         maybe_no_sync = (
-            # pyre-ignore[29]
             module.no_sync()
             if not should_update_weights
             and (isinstance(module, DDP) or _is_fsdp_module(module))
             else contextlib.nullcontext()
         )
 
         # if detect_anomaly is true, run forward and backward pass in detect_anomaly context
@@ -951,89 +899,7 @@
         raise RuntimeError(
             f"Torchdynamo backend {torchdynamo_params.backend} is not supported."
         ) from e
     except Exception as e:
         raise RuntimeError(
             f"The following error encountered when calling torch.compile for dynamo: {e}"
         ) from e
-
-
-def _prepare_ddp(
-    module: torch.nn.Module,
-    strategy: DDPStrategy,
-    device: torch.device,
-    torchdynamo_params: Optional[TorchDynamoParams],
-) -> DDP:
-    # wrap module in DDP
-    device_ids = None
-    if device.type == "cuda":
-        device_ids = [device.index]
-    params_dict = asdict(strategy)
-    # remove ddp comm hook variables from params dict
-    del params_dict["comm_state"]
-    del params_dict["comm_hook"]
-    module = module.to(device)
-
-    # remove sync batch norm from params dict before converting module
-    del params_dict["sync_batchnorm"]
-    if strategy.sync_batchnorm:
-        if device.type == "cuda":
-            module = torch.nn.SyncBatchNorm.convert_sync_batchnorm(module)
-        else:
-            rank_zero_warn(
-                f"SyncBatchNorm layers only work with GPU modules. Skipping the conversion because the device type is {device.type}."
-            )
-
-    module = DDP(module, device_ids=device_ids, **params_dict)
-    if torchdynamo_params:
-        # TODO: Add support for dynamo and DDP
-        rank_zero_warn(
-            "Torchdynamo params has been set with DDP - Note that performance will likely be slower and we recommend using only one."
-        )
-    if strategy.comm_hook:
-        module.register_comm_hook(state=strategy.comm_state, hook=strategy.comm_hook)
-    return module
-
-
-def _prepare_fsdp(
-    module: torch.nn.Module,
-    strategy: FSDPStrategy,
-    device: torch.device,
-    swa_params: Optional[SWAParams],
-    precision: Optional[torch.dtype],
-) -> FSDP:
-    if not is_torch_version_geq_1_12():
-        raise RuntimeError(
-            "Please install PyTorch 1.12 or higher to use FSDP: https://pytorch.org/get-started/locally/"
-        )
-    elif swa_params:
-        raise RuntimeError(
-            "Stochastic Weight Averaging is currently not supported with the FSDP strategy"
-        )
-    mixed_precision = None
-    if precision:
-        mixed_precision = MixedPrecision(
-            param_dtype=precision,
-            reduce_dtype=precision,
-            buffer_dtype=precision,
-        )
-
-    params_dict = asdict(strategy)
-
-    # extract params to set state dict type
-    state_dict_type = params_dict.pop("state_dict_type")
-    state_dict_config = params_dict.pop("state_dict_config")
-    optim_state_dict_config = params_dict.pop("optim_state_dict_config")
-
-    # wrap module in FSDP
-    module = FSDP(
-        module,
-        device_id=device,
-        mixed_precision=mixed_precision,
-        **params_dict,
-    )
-
-    if state_dict_type:
-        FSDP.set_state_dict_type(
-            module, state_dict_type, state_dict_config, optim_state_dict_config
-        )
-    return module
```

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     can then be passed to the :func:`~torchtnt.framework.fit` entry point.
 
     Args:
         train_dataloader: dataloader to be used during training, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         eval_dataloader: dataloader to be used during evaluation, which can be *any* iterable, including PyTorch DataLoader, DataLoader2, etc.
         max_epochs: the max number of epochs to run for training. ``None`` means no limit (infinite training) unless stopped by max_steps.
         max_steps: the max number of steps to run for training. ``None`` means no limit (infinite training) unless stopped by max_epochs.
-        max_train_steps_per_epoch: the max number of steps to run per epoch for training. None means train until the dataloader is exhausted.
+        max_train_steps_per_epoch: the max number of steps to run per epoch for training. None means train until ``train_dataloader`` is exhausted.
+        max_eval_steps_per_epoch: the max number of steps to run per epoch for evaluation. None means evaluate until ``eval_dataloader`` is exhausted.
         evaluate_every_n_steps: how often to run the evaluation loop in terms of training steps.
         evaluate_every_n_epochs: how often to run the evaluation loop in terms of training epochs.
         auto_timing: whether to automatically time the training and evaluation loop, using the state's timer (enabling auto_timing may degrade performance).
 
     Returns:
         An initialized state object containing metadata.
```

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/state.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/train.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.7.4/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .oom import (
     attach_oom_observer,
     is_out_of_cpu_memory,
     is_out_of_cuda_memory,
     is_out_of_memory_error,
     log_memory_snapshot,
 )
+from .prepare_model import DDPStrategy, FSDPStrategy, prepare_ddp, prepare_fsdp
 from .progress import Progress
 from .rank_zero_log import (
     rank_zero_critical,
     rank_zero_debug,
     rank_zero_error,
     rank_zero_info,
     rank_zero_print,
@@ -89,14 +90,18 @@
     "RSSProfiler",
     "days_to_secs",
     "attach_oom_observer",
     "is_out_of_cpu_memory",
     "is_out_of_cuda_memory",
     "is_out_of_memory_error",
     "log_memory_snapshot",
+    "DDPStrategy",
+    "FSDPStrategy",
+    "prepare_ddp",
+    "prepare_fsdp",
     "Progress",
     "rank_zero_critical",
     "rank_zero_debug",
     "rank_zero_error",
     "rank_zero_info",
     "rank_zero_print",
     "rank_zero_warn",
```

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/device.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/env.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt/utils/version.py` & `torchtnt-nightly-2023.7.4/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.7.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.7.3/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.7.4/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 torchtnt/utils/early_stop_checker.py
 torchtnt/utils/env.py
 torchtnt/utils/fsspec.py
 torchtnt/utils/lr_scheduler.py
 torchtnt/utils/memory.py
 torchtnt/utils/misc.py
 torchtnt/utils/oom.py
+torchtnt/utils/prepare_model.py
 torchtnt/utils/progress.py
 torchtnt/utils/rank_zero_log.py
 torchtnt/utils/test_utils.py
 torchtnt/utils/timer.py
 torchtnt/utils/tqdm.py
 torchtnt/utils/version.py
 torchtnt/utils/data/__init__.py
```

