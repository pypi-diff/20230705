# Comparing `tmp/rohmu-1.1.0.tar.gz` & `tmp/rohmu-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rohmu-1.1.0.tar", last modified: Thu Jun 15 10:17:15 2023, max compression
+gzip compressed data, was "rohmu-1.1.1.tar", last modified: Wed Jul  5 07:40:22 2023, max compression
```

## Comparing `rohmu-1.1.0.tar` & `rohmu-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.029233 rohmu-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-15 10:16:58.000000 rohmu-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-15 10:17:15.029233 rohmu-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-15 10:16:58.000000 rohmu-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 10:16:58.000000 rohmu-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/atomic_opener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/filewrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/inotify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/object_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/google.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/rohmufile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/snappyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/transfer_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/zstdfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-15 10:17:15.029233 rohmu-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-15 10:16:58.000000 rohmu-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.029233 rohmu-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_atomic_opener.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_from_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_inotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_rohmu_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_rohmufile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_transfer_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.899105 rohmu-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-05 07:40:13.000000 rohmu-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-05 07:40:22.899105 rohmu-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-05 07:40:13.000000 rohmu-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-05 07:40:13.000000 rohmu-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.883105 rohmu-1.1.1/rohmu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/atomic_opener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.887105 rohmu-1.1.1/rohmu/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/common/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.887105 rohmu-1.1.1/rohmu/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/delta/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/delta/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/filewrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/inotify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.887105 rohmu-1.1.1/rohmu/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/notifier/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/notifier/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/notifier/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/notifier/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.891105 rohmu-1.1.1/rohmu/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/object_storage/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/rohmufile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/snappyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/transfer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-05 07:40:13.000000 rohmu-1.1.1/rohmu/zstdfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.891105 rohmu-1.1.1/rohmu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-05 07:40:22.000000 rohmu-1.1.1/rohmu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-05 07:40:22.000000 rohmu-1.1.1/rohmu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:40:22.000000 rohmu-1.1.1/rohmu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 07:40:22.000000 rohmu-1.1.1/rohmu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 07:40:22.000000 rohmu-1.1.1/rohmu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-05 07:40:22.899105 rohmu-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-05 07:40:13.000000 rohmu-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:40:22.899105 rohmu-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_atomic_opener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_inotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_object_storage_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_rohmu_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_rohmufile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_transfer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-05 07:40:13.000000 rohmu-1.1.1/test/test_util.py
```

### Comparing `rohmu-1.1.0/LICENSE` & `rohmu-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/PKG-INFO` & `rohmu-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rohmu
-Version: 1.1.0
+Version: 1.1.1
 Summary: "Rohmu is a python library providing an interface to various cloud storage providers."
 Home-page: https://github.com/aiven/rohmu/
 License: Apache 2.0
 Platform: POSIX
 Platform: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rohmu-1.1.0/README.rst` & `rohmu-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/__init__.py` & `rohmu-1.1.1/rohmu/__init__.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/atomic_opener.py` & `rohmu-1.1.1/rohmu/atomic_opener.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/common/models.py` & `rohmu-1.1.1/rohmu/common/models.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/common/statsd.py` & `rohmu-1.1.1/rohmu/common/statsd.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/compat.py` & `rohmu-1.1.1/rohmu/compat.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/compressor.py` & `rohmu-1.1.1/rohmu/compressor.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/dates.py` & `rohmu-1.1.1/rohmu/dates.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/delta/common.py` & `rohmu-1.1.1/rohmu/delta/common.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/delta/snapshot.py` & `rohmu-1.1.1/rohmu/delta/snapshot.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/encryptor.py` & `rohmu-1.1.1/rohmu/encryptor.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/errors.py` & `rohmu-1.1.1/rohmu/errors.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/filewrap.py` & `rohmu-1.1.1/rohmu/filewrap.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/inotify.py` & `rohmu-1.1.1/rohmu/inotify.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/notifier/http.py` & `rohmu-1.1.1/rohmu/notifier/http.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/notifier/interface.py` & `rohmu-1.1.1/rohmu/notifier/interface.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/notifier/logger.py` & `rohmu-1.1.1/rohmu/notifier/logger.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/notifier/null.py` & `rohmu-1.1.1/rohmu/notifier/null.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/azure.py` & `rohmu-1.1.1/rohmu/object_storage/azure.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/base.py` & `rohmu-1.1.1/rohmu/object_storage/base.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/google.py` & `rohmu-1.1.1/rohmu/object_storage/google.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/local.py` & `rohmu-1.1.1/rohmu/object_storage/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,23 @@
     def _yield_object(self, key: str, full_path: str, with_metadata: bool) -> Iterator[IterKeyItem]:
         try:
             metadata = self._get_metadata_for_key(key)
         except FileNotFoundFromStorageError:
             return
         st = os.stat(full_path)
         last_modified = datetime.datetime.fromtimestamp(st.st_mtime, tz=datetime.timezone.utc)
+        md5 = metadata.get(INTERNAL_METADATA_KEY_HASH)
         yield IterKeyItem(
             type=KEY_TYPE_OBJECT,
             value={
                 "name": key,
                 "size": st.st_size,
                 "last_modified": last_modified,
-                "md5": metadata[INTERNAL_METADATA_KEY_HASH],
                 "metadata": self._filter_metadata(metadata) if with_metadata else None,
+                **({"md5": md5} if md5 else {}),
             },
         )
 
     def iter_key(
         self, key: str, *, with_metadata: bool = True, deep: bool = False, include_key: bool = False
     ) -> Iterator[IterKeyItem]:
         target_path = self.format_key_for_backend(key.strip("/"))
```

### Comparing `rohmu-1.1.0/rohmu/object_storage/s3.py` & `rohmu-1.1.1/rohmu/object_storage/s3.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/sftp.py` & `rohmu-1.1.1/rohmu/object_storage/sftp.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/object_storage/swift.py` & `rohmu-1.1.1/rohmu/object_storage/swift.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/rohmufile.py` & `rohmu-1.1.1/rohmu/rohmufile.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/snappyfile.py` & `rohmu-1.1.1/rohmu/snappyfile.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/transfer_pool.py` & `rohmu-1.1.1/rohmu/transfer_pool.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/typing.py` & `rohmu-1.1.1/rohmu/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,24 @@
 from __future__ import annotations
 
 from types import TracebackType
-from typing import Any, Dict, Optional, Type, TYPE_CHECKING, Union
-
-try:
-    from typing import Protocol
-except ImportError:
-    from typing_extensions import Protocol  # type: ignore [assignment]
-
-try:
-    # Remove when dropping support for Python 3.7
-    from pickle import PickleBuffer
-except ImportError:
-    PickleBuffer = bytes  # type: ignore [misc,assignment]
-import mmap
+from typing import Any, Dict, Optional, Protocol, Type, TYPE_CHECKING, Union
+from typing_extensions import Buffer
 
 if TYPE_CHECKING:
     from array import array
     from os import PathLike
 
     import ctypes
 
 Metadata = Dict[str, Any]
 
 AnyPath = Union[str, bytes, "PathLike[str]", "PathLike[bytes]"]
 
-BinaryData = Union[
-    bytes,
-    bytearray,
-    memoryview,
-    "array[Any]",
-    mmap.mmap,
-    "ctypes._CData",
-    PickleBuffer,
-]
+BinaryData = Buffer
 
 StrOrPathLike = Union[str, "PathLike[str]"]
 
 
 class HasFileno(Protocol):
     def fileno(self) -> int:
         ...
```

### Comparing `rohmu-1.1.0/rohmu/util.py` & `rohmu-1.1.1/rohmu/util.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu/zstdfile.py` & `rohmu-1.1.1/rohmu/zstdfile.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/rohmu.egg-info/PKG-INFO` & `rohmu-1.1.1/rohmu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rohmu
-Version: 1.1.0
+Version: 1.1.1
 Summary: "Rohmu is a python library providing an interface to various cloud storage providers."
 Home-page: https://github.com/aiven/rohmu/
 License: Apache 2.0
 Platform: POSIX
 Platform: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rohmu-1.1.0/rohmu.egg-info/SOURCES.txt` & `rohmu-1.1.1/rohmu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/setup.cfg` & `rohmu-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_atomic_opener.py` & `rohmu-1.1.1/test/test_atomic_opener.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_compressor.py` & `rohmu-1.1.1/test/test_compressor.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_dates.py` & `rohmu-1.1.1/test/test_dates.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_encryptor.py` & `rohmu-1.1.1/test/test_encryptor.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_from_model.py` & `rohmu-1.1.1/test/test_from_model.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_inotify.py` & `rohmu-1.1.1/test/test_inotify.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_object_storage_azure.py` & `rohmu-1.1.1/test/test_object_storage_azure.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_object_storage_google.py` & `rohmu-1.1.1/test/test_object_storage_google.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_object_storage_s3.py` & `rohmu-1.1.1/test/test_object_storage_s3.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_object_storage_sftp.py` & `rohmu-1.1.1/test/test_object_storage_sftp.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_object_storage_swift.py` & `rohmu-1.1.1/test/test_object_storage_swift.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_rohmu_dates.py` & `rohmu-1.1.1/test/test_rohmu_dates.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_rohmufile.py` & `rohmu-1.1.1/test/test_rohmufile.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_statsd.py` & `rohmu-1.1.1/test/test_statsd.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_storage.py` & `rohmu-1.1.1/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.1.0/test/test_transfer_pool.py` & `rohmu-1.1.1/test/test_transfer_pool.py`

 * *Files identical despite different names*

