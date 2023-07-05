# Comparing `tmp/anyio-3.7.0rc1.tar.gz` & `tmp/anyio-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyio-3.7.0rc1.tar", last modified: Thu May 18 16:06:13 2023, max compression
+gzip compressed data, was "anyio-3.7.1.tar", last modified: Wed Jul  5 16:44:41 2023, max compression
```

## Comparing `anyio-3.7.0rc1.tar` & `anyio-3.7.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/cancellation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/subprocesses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/threads.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/typedattrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34214 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.597363 anyio-3.7.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio/_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    30046 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_backends/_trio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/_core/_typedattr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/abc/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/abc/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/src/anyio/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/streams/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/src/anyio/to_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.601363 anyio-3.7.0rc1/src/anyio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 16:06:13.000000 anyio-3.7.0rc1/src/anyio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.605363 anyio-3.7.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:13.609362 anyio-3.7.0rc1/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/streams/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    51369 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_taskgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-18 16:06:01.000000 anyio-3.7.0rc1/tests/test_to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.469102 anyio-3.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 16:44:27.000000 anyio-3.7.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-05 16:44:27.000000 anyio-3.7.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 16:44:27.000000 anyio-3.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 16:44:27.000000 anyio-3.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 16:44:27.000000 anyio-3.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 16:44:27.000000 anyio-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:44:41.469102 anyio-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-05 16:44:27.000000 anyio-3.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.449102 anyio-3.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/cancellation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/subprocesses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/typedattrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-05 16:44:27.000000 anyio-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:44:41.469102 anyio-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio/_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67056 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30035 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/_trio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.457102 anyio-3.7.1/src/anyio/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_typedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.461102 anyio-3.7.1/src/anyio/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.461102 anyio-3.7.1/src/anyio/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.465102 anyio-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.469102 anyio-3.7.1/tests/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52196 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_taskgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_to_thread.py
```

### Comparing `anyio-3.7.0rc1/.github/workflows/publish.yml` & `anyio-3.7.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/.github/workflows/test.yml` & `anyio-3.7.1/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       run: pyright --verifytypes anyio
 
   test:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.8]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.9]
         include:
         - os: macos-latest
           python-version: "3.7"
         - os: macos-latest
           python-version: "3.11"
         - os: windows-latest
           python-version: "3.7"
@@ -41,18 +41,19 @@
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
         cache: pip
-        cache-dependency-path: setup.cfg
+        cache-dependency-path: pyproject.toml
     - name: Install dependencies
-      run: pip install .[test,trio] coveralls
+      run: pip install -e .[test] coveralls
     - name: Test with pytest
       run: coverage run -m pytest -v
       timeout-minutes: 5
       env:
         PYTEST_DISABLE_PLUGIN_AUTOLOAD: 1
     - name: Upload Coverage
       run: coveralls --service=github
```

### Comparing `anyio-3.7.0rc1/.pre-commit-config.yaml` & `anyio-3.7.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.265
+    rev: v0.0.277
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - trio-typing >= 0.8.0
           - packaging
```

### Comparing `anyio-3.7.0rc1/LICENSE` & `anyio-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/PKG-INFO` & `anyio-3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.0rc1
+Version: 3.7.1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyio-3.7.0rc1/README.rst` & `anyio-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/api.rst` & `anyio-3.7.1/docs/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 --------------------------------------------
 
 .. autofunction:: anyio.from_thread.run
 .. autofunction:: anyio.from_thread.run_sync
 .. autofunction:: anyio.from_thread.create_blocking_portal
 .. autofunction:: anyio.from_thread.start_blocking_portal
 
-.. autoclass:: anyio.abc.BlockingPortal
+.. autoclass:: anyio.from_thread.BlockingPortal
 
 Async file I/O
 --------------
 
 .. autofunction:: anyio.open_file
 .. autofunction:: anyio.wrap_file
 
@@ -131,14 +131,15 @@
 .. autofunction:: anyio.wait_socket_writable
 
 .. autoclass:: anyio.abc.SocketAttribute
 .. autoclass:: anyio.abc.SocketStream()
 .. autoclass:: anyio.abc.SocketListener()
 .. autoclass:: anyio.abc.UDPSocket()
 .. autoclass:: anyio.abc.ConnectedUDPSocket()
+.. autoclass:: anyio.abc.UNIXSocketStream()
 
 Subprocesses
 ------------
 
 .. autofunction:: anyio.run_process
 .. autofunction:: anyio.open_process
 
@@ -153,14 +154,15 @@
 .. autoclass:: anyio.Semaphore
 .. autoclass:: anyio.CapacityLimiter
 
 .. autoclass:: anyio.LockStatistics
 .. autoclass:: anyio.EventStatistics
 .. autoclass:: anyio.ConditionStatistics
 .. autoclass:: anyio.CapacityLimiterStatistics
+.. autoclass:: anyio.SemaphoreStatistics
 
 .. autofunction:: anyio.create_event
 .. autofunction:: anyio.create_lock
 .. autofunction:: anyio.create_condition
 .. autofunction:: anyio.create_semaphore
 .. autofunction:: anyio.create_capacity_limiter
```

### Comparing `anyio-3.7.0rc1/docs/basics.rst` & `anyio-3.7.1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/cancellation.rst` & `anyio-3.7.1/docs/cancellation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 Networked operations can often take a long time, and you usually want to set up some kind of a
 timeout to ensure that your application doesn't stall forever. There are two principal ways to do
 this: :func:`~move_on_after` and :func:`~fail_after`. Both are used as synchronous
 context managers. The difference between these two is that the former simply exits the context
 block prematurely on a timeout, while the other raises a :exc:`TimeoutError`.
 
 Both methods create a new cancel scope, and you can check the deadline by accessing the
-:attr:`~.abc.CancelScope.deadline` attribute. Note, however, that an outer cancel scope may
-have an earlier deadline than your current cancel scope. To check the actual deadline, you can use
-the :func:`~current_effective_deadline` function.
+:attr:`~.CancelScope.deadline` attribute. Note, however, that an outer cancel scope
+may have an earlier deadline than your current cancel scope. To check the actual
+deadline, you can use the :func:`~current_effective_deadline` function.
 
 Here's how you typically use timeouts::
 
     from anyio import create_task_group, move_on_after, sleep, run
 
 
     async def main():
```

### Comparing `anyio-3.7.0rc1/docs/conf.py` & `anyio-3.7.1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx_autodoc_typehints",
+    "sphinxcontrib.jquery",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "AnyIO"
 author = "Alex Grönholm"
@@ -23,13 +24,14 @@
 release = v.public
 
 language = "en"
 
 exclude_patterns = ["_build"]
 pygments_style = "sphinx"
 autodoc_default_options = {"members": True, "show-inheritance": True}
+autodoc_mock_imports = ["_typeshed"]
 todo_include_todos = False
 
 html_theme = "sphinx_rtd_theme"
 htmlhelp_basename = "anyiodoc"
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
```

### Comparing `anyio-3.7.0rc1/docs/contributing.rst` & `anyio-3.7.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/faq.rst` & `anyio-3.7.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/fileio.rst` & `anyio-3.7.1/docs/fileio.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 Asynchronous path operations
 ----------------------------
 
 AnyIO provides an asynchronous version of the :class:`pathlib.Path` class. It differs with the
 original in a number of ways:
 
-* Operations that perform disk I/O (like :meth:`~pathlib.Path.read_bytes``) are run in a worker
+* Operations that perform disk I/O (like :meth:`~pathlib.Path.read_bytes`) are run in a worker
   thread and thus require an ``await``
 * Methods like :meth:`~pathlib.Path.glob` return an asynchronous iterator that yields asynchronous
   :class:`~.Path` objects
 * Properties and methods that normally return :class:`pathlib.Path` objects return :class:`~.Path`
   objects instead
 * Methods and properties from the Python 3.10 API are available on all versions
 * Use as a context manager is not supported, as it is deprecated in pathlib
```

### Comparing `anyio-3.7.0rc1/docs/migration.rst` & `anyio-3.7.1/docs/migration.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #. to better serve use cases where synchronous callbacks are used by third party libraries
 #. to better match the API of trio_
 
 The following functions and methods were changed:
 
 * :func:`current_time`
 * :func:`current_effective_deadline`
-* :meth:`CancelScope.cancel() <.abc.CancelScope.cancel>`
+* :meth:`CancelScope.cancel() <.CancelScope.cancel>`
 * :meth:`CapacityLimiter.acquire_nowait`
 * :meth:`CapacityLimiter.acquire_on_behalf_of_nowait`
 * :meth:`Condition.release`
 * :meth:`Event.set`
 * :func:`get_current_task`
 * :func:`get_running_tasks`
 * :meth:`Lock.release`
@@ -36,33 +36,33 @@
 When migrating to AnyIO 3, simply remove the ``await`` from each call to these.
 
 .. note:: For backwards compatibility reasons, :func:`current_time`,
           :func:`current_effective_deadline` and :func:`get_running_tasks` return objects which are
           awaitable versions of their original types (:class:`float` and :class:`list`,
           respectively). These awaitable versions are subclasses of the original types so they
           should behave as their originals, but if you absolutely need the pristine original types,
-          you can either use :func:`maybe_async` or ``float()`` / ``list()`` on the returned
+          you can either use ``maybe_async`` or ``float()`` / ``list()`` on the returned
           value as appropriate.
 
 The following async context managers changed to regular context managers:
 
 * :func:`fail_after`
 * :func:`move_on_after`
-* :func:`open_cancel_scope` (now just ``CancelScope()``)
+* ``open_cancel_scope()`` (now just ``CancelScope()``)
 
 When migrating, just change ``async with`` into a plain ``with``.
 
 With the exception of
 :meth:`MemoryObjectReceiveStream.receive_nowait() <.streams.memory.MemoryObjectReceiveStream.receive_nowait>`,
 all of them can still be used like before – they will raise :exc:`DeprecationWarning` when used
 this way on AnyIO 3, however.
 
 If you're writing a library that needs to be compatible with both major releases, you will need
-to use the compatibility functions added in AnyIO 2.2: :func:`maybe_async` and
-:func:`maybe_async_cm`. These will let you safely use functions/methods and context managers
+to use the compatibility functions added in AnyIO 2.2: ``maybe_async()`` and
+``maybe_async_cm()``. These will let you safely use functions/methods and context managers
 (respectively) regardless of which major release is currently installed.
 
 Example 1 – setting an event::
 
     from anyio.abc import Event
     from anyio import maybe_async
 
@@ -80,19 +80,19 @@
             ...
 
 .. _trio: https://github.com/python-trio/trio
 
 Starting tasks
 --------------
 
-The :meth:`TaskGroup.spawn` coroutine method has been deprecated in favor of the synchronous
-method :meth:`TaskGroup.start_soon` (which mirrors ``start_soon()`` in trio's nurseries). If you're
-fully migrating to AnyIO 3, simply switch to calling the new method (and remove the ``await``).
+The ``TaskGroup.spawn()`` coroutine method has been deprecated in favor of the synchronous
+method :meth:`.TaskGroup.start_soon` (which mirrors ``start_soon()`` in trio's nurseries).
+If you're fully migrating to AnyIO 3, simply switch to calling the new method (and remove the ``await``).
 
-If your code needs to work with both AnyIO 2 and 3, you can keep using :meth:`~TaskGroup.spawn`
+If your code needs to work with both AnyIO 2 and 3, you can keep using ``TaskGroup.spawn()``
 (until AnyIO 4) and suppress the deprecation warning::
 
     import warnings
 
     async def foo():
         async with create_task_group() as tg:
             with warnings.catch_warnings():
@@ -105,26 +105,26 @@
 
     from anyio import sleep
     from anyio.from_thread import start_blocking_portal
 
     with start_blocking_portal() as portal:
         portal.call(sleep, 1)
 
-As with :meth:`TaskGroup.spawn`, the :meth:`BlockingPortal.spawn_task` method has also been renamed
-to :meth:`~BlockingPortal.start_task_soon`, so as to be consistent with task groups.
+As with ``TaskGroup.spawn()``, the ``BlockingPortal.spawn_task()`` method has also been renamed
+to :meth:`~from_thread.BlockingPortal.start_task_soon`, so as to be consistent with task groups.
 
-The :func:`create_blocking_portal` factory function was also deprecated in favor of instantiating
-:class:`BlockingPortal` directly.
+The ``create_blocking_portal()`` factory function was also deprecated in favor of instantiating
+:class:`~from_thread.BlockingPortal` directly.
 
 For code requiring cross compatibility, catching the deprecation warning (as above) should work.
 
 Synchronization primitives
 --------------------------
 
-Synchronization primitive factories (:func:`create_event` etc.) were deprecated in favor of
+Synchronization primitive factories (``create_event()`` etc.) were deprecated in favor of
 instantiating the classes directly. So convert code like this::
 
     from anyio import create_event
 
     async def main():
         event = create_event()
```

### Comparing `anyio-3.7.0rc1/docs/networking.rst` & `anyio-3.7.1/docs/networking.rst`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 .. note:: The UNIX socket listener does not remove the socket it creates, so you may need to delete
           them manually.
 
 Sending and receiving file descriptors
 ++++++++++++++++++++++++++++++++++++++
 
 UNIX sockets can be used to pass open file descriptors (sockets and files) to another process.
-The receiving end can then use either :func:`os.fdopen` or :func:`socket.socket` to get a usable
+The receiving end can then use either :func:`os.fdopen` or :class:`socket.socket` to get a usable
 file or socket object, respectively.
 
 The following is an example where a client connects to a UNIX socket server and receives the
 descriptor of a file opened on the server, reads the contents of the file and then prints them on
 standard output.
 
 Client::
```

### Comparing `anyio-3.7.0rc1/docs/signals.rst` & `anyio-3.7.1/docs/signals.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                     return
                 elif signum == signal.SIGHUP:
                     print('Reloading configuration')
 
     run(main)
 
 .. note:: Signal handlers can only be installed in the main thread, so they will not work when the
-    event loop is being run through :func:`~start_blocking_portal`, for instance.
+    event loop is being run through :class:`~.from_thread.BlockingPortal`, for instance.
 
 .. note:: Windows does not natively support signals so do not rely on this in a cross platform
     application.
 
 Handling KeyboardInterrupt and SystemExit
 -----------------------------------------
```

### Comparing `anyio-3.7.0rc1/docs/streams.rst` & `anyio-3.7.1/docs/streams.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/subprocesses.rst` & `anyio-3.7.1/docs/subprocesses.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/support.rst` & `anyio-3.7.1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/synchronization.rst` & `anyio-3.7.1/docs/synchronization.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/tasks.rst` & `anyio-3.7.1/docs/tasks.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/testing.rst` & `anyio-3.7.1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/threads.rst` & `anyio-3.7.1/docs/threads.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 Calling asynchronous code from an external thread
 -------------------------------------------------
 
 If you need to run async code from a thread that is not a worker thread spawned by the event loop,
 you need a *blocking portal*. This needs to be obtained from within the event loop thread.
 
 One way to do this is to start a new event loop with a portal, using
-:func:`~start_blocking_portal` (which takes mostly the same arguments as :func:`~run`::
+:class:`~from_thread.start_blocking_portal` (which takes mostly the same arguments as :func:`~run`::
 
     from anyio.from_thread import start_blocking_portal
 
 
     with start_blocking_portal(backend='trio') as portal:
         portal.call(...)
 
@@ -189,15 +189,15 @@
 When calling asynchronous code from worker threads, context is again copied to the task that calls
 the target function in the event loop thread.
 
 Adjusting the default maximum worker thread count
 -------------------------------------------------
 
 The default AnyIO worker thread limiter has a value of **40**, meaning that any calls
-to :func:`.to_thread.run` without an explicit ``limiter`` argument will cause a maximum
+to :func:`.to_thread.run_sync` without an explicit ``limiter`` argument will cause a maximum
 of 40 threads to be spawned. You can adjust this limit like this::
 
     from anyio import to_thread
 
     async def foo():
         # Set the maximum number of worker threads to 60
         to_thread.current_default_thread_limiter().total_tokens = 60
```

### Comparing `anyio-3.7.0rc1/docs/typedattrs.rst` & `anyio-3.7.1/docs/typedattrs.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/docs/versionhistory.rst` & `anyio-3.7.1/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
-**3.7.0rc1**
+**3.7.1**
+
+- Fixed sending large buffers via UNIX stream sockets on asyncio
+- Fixed several minor documentation issues (broken links to classes, missing classes or
+  attributes)
+
+**3.7.0**
 
 - Dropped support for Python 3.6
 - Improved type annotations:
 
   - Several functions and methods that were previously annotated as accepting
     ``Coroutine[Any, Any, Any]`` as the return type of the callable have been amended to
     accept ``Awaitable[Any]`` instead, to allow a slightly broader set of coroutine-like
```

### Comparing `anyio-3.7.0rc1/pyproject.toml` & `anyio-3.7.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Framework :: AnyIO",
+    "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -46,20 +47,21 @@
     "mock >= 4; python_version < '3.8'",
     "coverage[toml] >= 4.5",
     "hypothesis >= 4.0",
     "psutil >= 5.9",
     "pytest >= 7.0",
     "pytest-mock >= 3.6.1",
     "trustme",
-    "uvloop >= 0.17; platform_python_implementation == 'CPython' and platform_system != 'Windows'",
+    "uvloop >= 0.17; python_version < '3.12' and platform_python_implementation == 'CPython' and platform_system != 'Windows'",
 ]
 doc = [
     "packaging",
-    "Sphinx >= 6.1.0",
-    "sphinx_rtd_theme",
+    "Sphinx",
+    "sphinx-rtd-theme >= 1.2.2",
+    "sphinxcontrib-jquery",
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
 
 [project.entry-points]
 pytest11 = {anyio = "anyio.pytest_plugin"}
 
 [tool.setuptools_scm]
@@ -97,14 +99,17 @@
 addopts = "-rsx --tb=short --strict-config --strict-markers -p anyio -p no:asyncio -p no:trio"
 testpaths = ["tests"]
 # Ignore resource warnings due to a CPython/Windows bug (https://bugs.python.org/issue44428)
 filterwarnings = [
     "error",
     "ignore:unclosed <socket.socket.*:ResourceWarning",
     "ignore:unclosed transport <_ProactorSocketTransport.*:ResourceWarning",
+    "ignore:ast.Str is deprecated:DeprecationWarning",
+    "ignore:Attribute s is deprecated:DeprecationWarning",
+    "ignore:ast.NameConstant is deprecated:DeprecationWarning",
     # Workaround for Python 3.9.7 (see https://bugs.python.org/issue45097)
     "ignore:The loop argument is deprecated since Python 3\\.8, and scheduled for removal in Python 3\\.10\\.:DeprecationWarning:asyncio",
 ]
 markers = [
     "network: marks tests as requiring Internet access",
 ]
 
@@ -114,36 +119,33 @@
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-minversion = 4.0.0
 envlist = pre-commit, py37, py38, py39, py310, py311, pypy3
 skip_missing_interpreters = true
+minversion = 4.4.3
 
 [testenv]
 depends = pre-commit
 package = editable
 commands = coverage run -m pytest {posargs}
-extras =
-    test
-    trio
+extras = test
 
 [testenv:pre-commit]
 depends =
 basepython = python3
 package = skip
 deps = pre-commit
 commands = pre-commit run --all-files
 
 [testenv:pyright]
 deps = pyright
 commands = pyright --verifytypes anyio
-package = editable
 
 [testenv:docs]
 depends =
 extras = doc
-commands = sphinx-build docs build/sphinx
+commands = sphinx-build -W docs build/sphinx
 """
```

### Comparing `anyio-3.7.0rc1/src/anyio/__init__.py` & `anyio-3.7.1/src/anyio/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_backends/_asyncio.py` & `anyio-3.7.1/src/anyio/_backends/_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     IO,
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Collection,
     Coroutine,
-    Deque,
     Generator,
     Iterable,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
@@ -756,15 +755,15 @@
 class WorkerThread(Thread):
     MAX_IDLE_TIME = 10  # seconds
 
     def __init__(
         self,
         root_task: asyncio.Task,
         workers: set[WorkerThread],
-        idle_workers: Deque[WorkerThread],
+        idle_workers: deque[WorkerThread],
     ):
         super().__init__(name="AnyIO worker thread")
         self.root_task = root_task
         self.workers = workers
         self.idle_workers = idle_workers
         self.loop = root_task._loop
         self.queue: Queue[
@@ -822,15 +821,15 @@
         self.workers.discard(self)
         try:
             self.idle_workers.remove(self)
         except ValueError:
             pass
 
 
-_threadpool_idle_workers: RunVar[Deque[WorkerThread]] = RunVar(
+_threadpool_idle_workers: RunVar[deque[WorkerThread]] = RunVar(
     "_threadpool_idle_workers"
 )
 _threadpool_workers: RunVar[set[WorkerThread]] = RunVar("_threadpool_workers")
 
 
 async def run_sync_in_worker_thread(
     func: Callable[..., T_Retval],
@@ -1110,15 +1109,15 @@
 
 #
 # Sockets and networking
 #
 
 
 class StreamProtocol(asyncio.Protocol):
-    read_queue: Deque[bytes]
+    read_queue: deque[bytes]
     read_event: asyncio.Event
     write_event: asyncio.Event
     exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque()
         self.read_event = asyncio.Event()
@@ -1146,15 +1145,15 @@
         self.write_event = asyncio.Event()
 
     def resume_writing(self) -> None:
         self.write_event.set()
 
 
 class DatagramProtocol(asyncio.DatagramProtocol):
-    read_queue: Deque[tuple[bytes, IPSockAddrType]]
+    read_queue: deque[tuple[bytes, IPSockAddrType]]
     read_event: asyncio.Event
     write_event: asyncio.Event
     exception: Exception | None = None
 
     def connection_made(self, transport: asyncio.BaseTransport) -> None:
         self.read_queue = deque(maxlen=100)  # arbitrary value
         self.read_event = asyncio.Event()
@@ -1326,15 +1325,15 @@
     async def send(self, item: bytes) -> None:
         loop = get_running_loop()
         await checkpoint()
         with self._send_guard:
             view = memoryview(item)
             while view:
                 try:
-                    bytes_sent = self.__raw_socket.send(item)
+                    bytes_sent = self.__raw_socket.send(view)
                 except BlockingIOError:
                     await self._wait_until_writable(loop)
                 except OSError as exc:
                     if self._closing:
                         raise ClosedResourceError from None
                     else:
                         raise BrokenResourceError from exc
@@ -1921,15 +1920,15 @@
 #
 
 
 class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
     def __init__(self, signals: tuple[int, ...]):
         self._signals = signals
         self._loop = get_running_loop()
-        self._signal_queue: Deque[int] = deque()
+        self._signal_queue: deque[int] = deque()
         self._future: asyncio.Future = asyncio.Future()
         self._handled_signals: set[int] = set()
 
     def _deliver(self, signum: int) -> None:
         self._signal_queue.append(signum)
         if not self._future.done():
             self._future.set_result(None)
```

### Comparing `anyio-3.7.0rc1/src/anyio/_backends/_trio.py` & `anyio-3.7.1/src/anyio/_backends/_trio.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     Any,
     AsyncGenerator,
     AsyncIterator,
     Awaitable,
     Callable,
     Collection,
     Coroutine,
-    Deque,
     Generic,
     Iterable,
     Mapping,
     NoReturn,
     Sequence,
     TypeVar,
     cast,
@@ -905,15 +904,15 @@
 
 class TestRunner(abc.TestRunner):
     def __init__(self, **options: Any) -> None:
         from collections import deque
         from queue import Queue
 
         self._call_queue: Queue[Callable[..., object]] = Queue()
-        self._result_queue: Deque[Outcome] = deque()
+        self._result_queue: deque[Outcome] = deque()
         self._stop_event: trio.Event | None = None
         self._nursery: trio.Nursery | None = None
         self._options = options
 
     async def _trio_main(self) -> None:
         self._stop_event = trio.Event()
         async with trio.open_nursery() as self._nursery:
```

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_compat.py` & `anyio-3.7.1/src/anyio/_core/_compat.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_eventloop.py` & `anyio-3.7.1/src/anyio/_core/_eventloop.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_exceptions.py` & `anyio-3.7.1/src/anyio/_core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_fileio.py` & `anyio-3.7.1/src/anyio/_core/_fileio.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_signals.py` & `anyio-3.7.1/src/anyio/_core/_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_sockets.py` & `anyio-3.7.1/src/anyio/_core/_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_streams.py` & `anyio-3.7.1/src/anyio/_core/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_subprocesses.py` & `anyio-3.7.1/src/anyio/_core/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_synchronization.py` & `anyio-3.7.1/src/anyio/_core/_synchronization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import dataclass
 from types import TracebackType
-from typing import Deque
 from warnings import warn
 
 from ..lowlevel import cancel_shielded_checkpoint, checkpoint, checkpoint_if_cancelled
 from ._compat import DeprecatedAwaitable
 from ._eventloop import get_asynclib
 from ._exceptions import BusyResourceError, WouldBlock
 from ._tasks import CancelScope
@@ -101,15 +100,15 @@
         raise NotImplementedError
 
 
 class Lock:
     _owner_task: TaskInfo | None = None
 
     def __init__(self) -> None:
-        self._waiters: Deque[tuple[TaskInfo, Event]] = deque()
+        self._waiters: deque[tuple[TaskInfo, Event]] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
@@ -146,15 +145,15 @@
                 self.release()
                 raise
 
     def acquire_nowait(self) -> None:
         """
         Acquire the lock, without blocking.
 
-        :raises ~WouldBlock: if the operation would block
+        :raises ~anyio.WouldBlock: if the operation would block
 
         """
         task = get_current_task()
         if self._owner_task == task:
             raise RuntimeError("Attempted to acquire an already held Lock")
 
         if self._owner_task is not None:
@@ -189,15 +188,15 @@
 
 
 class Condition:
     _owner_task: TaskInfo | None = None
 
     def __init__(self, lock: Lock | None = None):
         self._lock = lock or Lock()
-        self._waiters: Deque[Event] = deque()
+        self._waiters: deque[Event] = deque()
 
     async def __aenter__(self) -> None:
         await self.acquire()
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
@@ -215,15 +214,15 @@
         await self._lock.acquire()
         self._owner_task = get_current_task()
 
     def acquire_nowait(self) -> None:
         """
         Acquire the underlying lock, without blocking.
 
-        :raises ~WouldBlock: if the operation would block
+        :raises ~anyio.WouldBlock: if the operation would block
 
         """
         self._lock.acquire_nowait()
         self._owner_task = get_current_task()
 
     def release(self) -> DeprecatedAwaitable:
         """Release the underlying lock."""
@@ -291,15 +290,15 @@
             if max_value < initial_value:
                 raise ValueError(
                     "max_value must be equal to or higher than initial_value"
                 )
 
         self._value = initial_value
         self._max_value = max_value
-        self._waiters: Deque[Event] = deque()
+        self._waiters: deque[Event] = deque()
 
     async def __aenter__(self) -> Semaphore:
         await self.acquire()
         return self
 
     async def __aexit__(
         self,
@@ -333,15 +332,15 @@
                 self.release()
                 raise
 
     def acquire_nowait(self) -> None:
         """
         Acquire the underlying lock, without blocking.
 
-        :raises ~WouldBlock: if the operation would block
+        :raises ~anyio.WouldBlock: if the operation would block
 
         """
         if self._value == 0:
             raise WouldBlock
 
         self._value -= 1
```

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_tasks.py` & `anyio-3.7.1/src/anyio/_core/_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
     Create a context manager which raises a :class:`TimeoutError` if does not finish in time.
 
     :param delay: maximum allowed time (in seconds) before raising the exception, or ``None`` to
         disable the timeout
     :param shield: ``True`` to shield the cancel scope from external cancellation
     :return: a context manager that yields a cancel scope
-    :rtype: :class:`~typing.ContextManager`\\[:class:`~anyio.abc.CancelScope`\\]
+    :rtype: :class:`~typing.ContextManager`\\[:class:`~anyio.CancelScope`\\]
 
     """
     deadline = (
         (get_asynclib().current_time() + delay) if delay is not None else math.inf
     )
     cancel_scope = get_asynclib().CancelScope(deadline=deadline, shield=shield)
     return FailAfterContextManager(cancel_scope)
```

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_testing.py` & `anyio-3.7.1/src/anyio/_core/_testing.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/_core/_typedattr.py` & `anyio-3.7.1/src/anyio/_core/_typedattr.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/__init__.py` & `anyio-3.7.1/src/anyio/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_resources.py` & `anyio-3.7.1/src/anyio/abc/_resources.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_sockets.py` & `anyio-3.7.1/src/anyio/abc/_sockets.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_streams.py` & `anyio-3.7.1/src/anyio/abc/_streams.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_subprocesses.py` & `anyio-3.7.1/src/anyio/abc/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_tasks.py` & `anyio-3.7.1/src/anyio/abc/_tasks.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/abc/_testing.py` & `anyio-3.7.1/src/anyio/abc/_testing.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/from_thread.py` & `anyio-3.7.1/src/anyio/from_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,18 +346,19 @@
 
         The task will be run inside a cancel scope which can be cancelled by cancelling the
         returned future.
 
         :param func: the target function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
-        :return: a future that resolves with the return value of the callable if the task completes
-            successfully, or with the exception raised in the task
-        :raises RuntimeError: if the portal is not running or if this method is called from within
-            the event loop thread
+        :return: a future that resolves with the return value of the callable if the
+            task completes successfully, or with the exception raised in the task
+        :raises RuntimeError: if the portal is not running or if this method is called
+            from within the event loop thread
+        :rtype: concurrent.futures.Future[T_Retval]
 
         .. versionadded:: 3.0
 
         """
         self._check_running()
         f: Future = Future()
         self._spawn_task_from_thread(func, args, {}, name, f)
@@ -365,21 +366,23 @@
 
     def start_task(
         self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> tuple[Future[Any], Any]:
         """
         Start a task in the portal's task group and wait until it signals for readiness.
 
-        This method works the same way as :meth:`TaskGroup.start`.
+        This method works the same way as :meth:`.abc.TaskGroup.start`.
 
         :param func: the target function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
-        :return: a tuple of (future, task_status_value) where the ``task_status_value`` is the
-            value passed to ``task_status.started()`` from within the target function
+        :return: a tuple of (future, task_status_value) where the ``task_status_value``
+            is the value passed to ``task_status.started()`` from within the target
+            function
+        :rtype: tuple[concurrent.futures.Future[Any], Any]
 
         .. versionadded:: 3.0
 
         """
 
         def task_done(future: Future) -> None:
             if not task_status_future.done():
```

### Comparing `anyio-3.7.0rc1/src/anyio/lowlevel.py` & `anyio-3.7.1/src/anyio/lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/pytest_plugin.py` & `anyio-3.7.1/src/anyio/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/streams/buffered.py` & `anyio-3.7.1/src/anyio/streams/buffered.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/streams/file.py` & `anyio-3.7.1/src/anyio/streams/file.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/streams/memory.py` & `anyio-3.7.1/src/anyio/streams/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections import OrderedDict, deque
 from dataclasses import dataclass, field
 from types import TracebackType
-from typing import Deque, Generic, NamedTuple, TypeVar
+from typing import Generic, NamedTuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
     get_cancelled_exc_class,
@@ -31,15 +31,15 @@
     #: number of tasks blocked on :meth:`MemoryObjectReceiveStream.receive`
     tasks_waiting_receive: int
 
 
 @dataclass(eq=False)
 class MemoryObjectStreamState(Generic[T_Item]):
     max_buffer_size: float = field()
-    buffer: Deque[T_Item] = field(init=False, default_factory=deque)
+    buffer: deque[T_Item] = field(init=False, default_factory=deque)
     open_send_channels: int = field(init=False, default=0)
     open_receive_channels: int = field(init=False, default=0)
     waiting_receivers: OrderedDict[Event, list[T_Item]] = field(
         init=False, default_factory=OrderedDict
     )
     waiting_senders: OrderedDict[Event, T_Item] = field(
         init=False, default_factory=OrderedDict
```

### Comparing `anyio-3.7.0rc1/src/anyio/streams/stapled.py` & `anyio-3.7.1/src/anyio/streams/stapled.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/streams/text.py` & `anyio-3.7.1/src/anyio/streams/text.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio/streams/tls.py` & `anyio-3.7.1/src/anyio/streams/tls.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,28 @@
 
     #: the selected ALPN protocol
     alpn_protocol: str | None = typed_attribute()
     #: the channel binding for type ``tls-unique``
     channel_binding_tls_unique: bytes = typed_attribute()
     #: the selected cipher
     cipher: tuple[str, str, int] = typed_attribute()
-    #: the peer certificate in dictionary form (see :meth:`ssl.SSLSocket.getpeercert` for more
-    #: information)
+    #: the peer certificate in dictionary form (see :meth:`ssl.SSLSocket.getpeercert`
+    #: for more information)
     peer_certificate: dict[str, str | _PCTRTTT | _PCTRTT] | None = typed_attribute()
     #: the peer certificate in binary form
     peer_certificate_binary: bytes | None = typed_attribute()
     #: ``True`` if this is the server side of the connection
     server_side: bool = typed_attribute()
     #: ciphers shared by the client during the TLS handshake (``None`` if this is the
     #: client side)
     shared_ciphers: list[tuple[str, str, int]] | None = typed_attribute()
     #: the :class:`~ssl.SSLObject` used for encryption
     ssl_object: ssl.SSLObject = typed_attribute()
-    #: ``True`` if this stream does (and expects) a closing TLS handshake when the stream is being
-    #: closed
+    #: ``True`` if this stream does (and expects) a closing TLS handshake when the
+    #: stream is being closed
     standard_compatible: bool = typed_attribute()
     #: the TLS protocol version (e.g. ``TLSv1.2``)
     tls_version: str = typed_attribute()
 
 
 @dataclass(eq=False)
 class TLSStream(ByteStream):
@@ -79,21 +79,21 @@
     ) -> TLSStream:
         """
         Wrap an existing stream with Transport Layer Security.
 
         This performs a TLS handshake with the peer.
 
         :param transport_stream: a bytes-transporting stream to wrap
-        :param server_side: ``True`` if this is the server side of the connection, ``False`` if
-            this is the client side (if omitted, will be set to ``False`` if ``hostname`` has been
-            provided, ``False`` otherwise). Used only to create a default context when an explicit
-            context has not been provided.
+        :param server_side: ``True`` if this is the server side of the connection,
+            ``False`` if this is the client side (if omitted, will be set to ``False``
+            if ``hostname`` has been provided, ``False`` otherwise). Used only to create
+            a default context when an explicit context has not been provided.
         :param hostname: host name of the peer (if host name checking is desired)
-        :param ssl_context: the SSLContext object to use (if not provided, a secure default will be
-            created)
+        :param ssl_context: the SSLContext object to use (if not provided, a secure
+            default will be created)
         :param standard_compatible: if ``False``, skip the closing handshake when closing the
             connection, and don't raise an exception if the peer does the same
         :raises ~ssl.SSLError: if the TLS handshake fails
 
         """
         if server_side is None:
             server_side = not hostname
@@ -259,22 +259,22 @@
     listener: Listener[Any]
     ssl_context: ssl.SSLContext
     standard_compatible: bool = True
     handshake_timeout: float = 30
 
     @staticmethod
     async def handle_handshake_error(exc: BaseException, stream: AnyByteStream) -> None:
-        f"""
+        """
         Handle an exception raised during the TLS handshake.
 
         This method does 3 things:
 
         #. Forcefully closes the original stream
-        #. Logs the exception (unless it was a cancellation exception) using the ``{__name__}``
-           logger
+        #. Logs the exception (unless it was a cancellation exception) using the
+           ``anyio.streams.tls`` logger
         #. Reraises the exception if it was a base exception or a cancellation exception
 
         :param exc: the exception
         :param stream: the original stream
 
         """
         await aclose_forcefully(stream)
```

### Comparing `anyio-3.7.0rc1/src/anyio/to_process.py` & `anyio-3.7.1/src/anyio/to_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import os
 import pickle
 import subprocess
 import sys
 from collections import deque
 from importlib.util import module_from_spec, spec_from_file_location
-from typing import Callable, Deque, TypeVar, cast
+from typing import Callable, TypeVar, cast
 
 from ._core._eventloop import current_time, get_asynclib, get_cancelled_exc_class
 from ._core._exceptions import BrokenWorkerProcess
 from ._core._subprocesses import open_process
 from ._core._synchronization import CapacityLimiter
 from ._core._tasks import CancelScope, fail_after
 from .abc import ByteReceiveStream, ByteSendStream, Process
 from .lowlevel import RunVar, checkpoint_if_cancelled
 from .streams.buffered import BufferedByteReceiveStream
 
 WORKER_MAX_IDLE_TIME = 300  # 5 minutes
 
 T_Retval = TypeVar("T_Retval")
 _process_pool_workers: RunVar[set[Process]] = RunVar("_process_pool_workers")
-_process_pool_idle_workers: RunVar[Deque[tuple[Process, float]]] = RunVar(
+_process_pool_idle_workers: RunVar[deque[tuple[Process, float]]] = RunVar(
     "_process_pool_idle_workers"
 )
 _default_process_limiter: RunVar[CapacityLimiter] = RunVar("_default_process_limiter")
 
 
 async def run_sync(
     func: Callable[..., T_Retval],
```

### Comparing `anyio-3.7.0rc1/src/anyio/to_thread.py` & `anyio-3.7.1/src/anyio/to_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/src/anyio.egg-info/PKG-INFO` & `anyio-3.7.1/src/anyio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.0rc1
+Version: 3.7.1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyio-3.7.0rc1/src/anyio.egg-info/SOURCES.txt` & `anyio-3.7.1/src/anyio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/conftest.py` & `anyio-3.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/streams/test_buffered.py` & `anyio-3.7.1/tests/streams/test_buffered.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/streams/test_file.py` & `anyio-3.7.1/tests/streams/test_file.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/streams/test_memory.py` & `anyio-3.7.1/tests/streams/test_memory.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/streams/test_stapled.py` & `anyio-3.7.1/tests/streams/test_stapled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import InitVar, dataclass, field
-from typing import Deque, Iterable, TypeVar
+from typing import Iterable, TypeVar
 
 import pytest
 
 from anyio import ClosedResourceError, EndOfStream
 from anyio.abc import (
     ByteReceiveStream,
     ByteSendStream,
@@ -99,15 +99,15 @@
 
 T_Item = TypeVar("T_Item")
 
 
 @dataclass
 class DummyObjectReceiveStream(ObjectReceiveStream[T_Item]):
     data: InitVar[Iterable[T_Item]]
-    buffer: Deque[T_Item] = field(init=False)
+    buffer: deque[T_Item] = field(init=False)
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self, data: Iterable[T_Item]) -> None:
         self.buffer = deque(data)
 
     async def receive(self) -> T_Item:
         if self._closed:
```

### Comparing `anyio-3.7.0rc1/tests/streams/test_text.py` & `anyio-3.7.1/tests/streams/test_text.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/streams/test_tls.py` & `anyio-3.7.1/tests/streams/test_tls.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_compat.py` & `anyio-3.7.1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_debugging.py` & `anyio-3.7.1/tests/test_debugging.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_eventloop.py` & `anyio-3.7.1/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_fileio.py` & `anyio-3.7.1/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_from_thread.py` & `anyio-3.7.1/tests/test_from_thread.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_lowlevel.py` & `anyio-3.7.1/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_pytest_plugin.py` & `anyio-3.7.1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_signals.py` & `anyio-3.7.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_sockets.py` & `anyio-3.7.1/tests/test_sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,35 +748,63 @@
             request = client.recv(100)
             client.sendall(request[::-1])
             response = await stream.receive()
             client.close()
 
         assert response == b"halb"
 
-    async def test_send_large_buffer(
+    async def test_receive_large_buffer(
         self, server_sock: socket.socket, socket_path: Path
     ) -> None:
         def serve() -> None:
             client, _ = server_sock.accept()
             client.sendall(buffer)
             client.close()
 
         buffer = (
-            b"\xff" * 1024 * 1024
+            b"\xff" * 1024 * 512 + b"\x00" * 1024 * 512
         )  # should exceed the maximum kernel send buffer size
         async with await connect_unix(socket_path) as stream:
             thread = Thread(target=serve, daemon=True)
             thread.start()
             response = b""
             while len(response) < len(buffer):
                 response += await stream.receive()
 
         thread.join()
         assert response == buffer
 
+    async def test_send_large_buffer(
+        self, server_sock: socket.socket, socket_path: Path
+    ) -> None:
+        response = b""
+
+        def serve() -> None:
+            nonlocal response
+            client, _ = server_sock.accept()
+            while True:
+                data = client.recv(1024)
+                if not data:
+                    break
+
+                response += data
+
+            client.close()
+
+        buffer = (
+            b"\xff" * 1024 * 512 + b"\x00" * 1024 * 512
+        )  # should exceed the maximum kernel send buffer size
+        async with await connect_unix(socket_path) as stream:
+            thread = Thread(target=serve, daemon=True)
+            thread.start()
+            await stream.send(buffer)
+
+        thread.join()
+        assert response == buffer
+
     async def test_receive_fds(
         self, server_sock: socket.socket, socket_path: Path, tmp_path: Path
     ) -> None:
         def serve() -> None:
             path1 = tmp_path / "file1"
             path2 = tmp_path / "file2"
             path1.write_text("Hello, ")
```

### Comparing `anyio-3.7.0rc1/tests/test_subprocesses.py` & `anyio-3.7.1/tests/test_subprocesses.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_synchronization.py` & `anyio-3.7.1/tests/test_synchronization.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_taskgroups.py` & `anyio-3.7.1/tests/test_taskgroups.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_to_process.py` & `anyio-3.7.1/tests/test_to_process.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.0rc1/tests/test_to_thread.py` & `anyio-3.7.1/tests/test_to_thread.py`

 * *Files identical despite different names*

