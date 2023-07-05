# Comparing `tmp/segment-guard-0.0.2.tar.gz` & `tmp/segment-guard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-guard-0.0.2.tar", last modified: Mon Jul  3 13:25:39 2023, max compression
+gzip compressed data, was "segment-guard-0.0.3.tar", last modified: Wed Jul  5 07:35:25 2023, max compression
```

## Comparing `segment-guard-0.0.2.tar` & `segment-guard-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 segment-guard-0.0.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2023-07-03 13:25:39.256354 segment-guard-0.0.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      294 2023-07-03 11:27:11.000000 segment-guard-0.0.2/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1056 2023-07-03 11:32:23.000000 segment-guard-0.0.2/pyproject.toml
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/segment_guard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       52 2023-06-21 13:56:24.000000 segment-guard-0.0.2/segment_guard/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5828 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/detection.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-06-30 11:10:59.000000 segment-guard-0.0.2/segment_guard/embedding_utils.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/explanation.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7979 2023-07-03 13:18:08.000000 segment-guard-0.0.2/segment_guard/segment_guard.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/segment_guard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      413 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      232 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-03 13:25:39.256354 segment-guard-0.0.2/setup.cfg
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4385 2023-07-03 11:25:32.000000 segment-guard-0.0.2/tests/test_segment_guard.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:35:25.944138 segment-guard-0.0.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      345 2023-07-05 07:35:25.944138 segment-guard-0.0.3/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      158 2023-07-05 07:34:16.000000 segment-guard-0.0.3/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-05 07:35:25.944138 segment-guard-0.0.3/segment_guard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      345 2023-07-05 07:35:25.000000 segment-guard-0.0.3/segment_guard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      202 2023-07-05 07:35:25.000000 segment-guard-0.0.3/segment_guard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-05 07:35:25.000000 segment-guard-0.0.3/segment_guard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-05 07:35:25.000000 segment-guard-0.0.3/segment_guard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-05 07:35:25.000000 segment-guard-0.0.3/segment_guard.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-05 07:35:25.944138 segment-guard-0.0.3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      545 2023-07-05 07:34:16.000000 segment-guard-0.0.3/setup.py
```

