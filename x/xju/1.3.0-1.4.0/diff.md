# Comparing `tmp/xju-1.3.0.tar.gz` & `tmp/xju-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-1.3.0.tar", last modified: Wed Jun 21 10:31:40 2023, max compression
+gzip compressed data, was "xju-1.4.0.tar", last modified: Wed Jul  5 10:32:10 2023, max compression
```

## Comparing `xju-1.3.0.tar` & `xju-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.132263 xju-1.3.0/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-06-21 10:31:39.000000 xju-1.3.0/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)     9044 2023-06-21 10:31:40.132263 xju-1.3.0/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     7508 2023-06-21 10:31:39.000000 xju-1.3.0/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1742 2023-06-21 10:31:39.000000 xju-1.3.0/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-06-21 10:31:40.132263 xju-1.3.0/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.124263 xju-1.3.0/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-1.3.0/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-1.3.0/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju/cmc/
--rwxr-xr-x   0 xju       (1001) xju       (1001)     9781 2023-06-20 09:48:20.000000 xju-1.3.0/src/xju/cmc/AsyncDict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-1.3.0/src/xju/cmc/AsyncOpt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.3.0/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-06-11 03:07:27.000000 xju-1.3.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.3.0/src/xju/cmc/Dict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-1.3.0/src/xju/cmc/Opt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.3.0/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    41771 2023-06-21 01:30:26.000000 xju-1.3.0/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6803 2023-06-19 11:23:59.000000 xju-1.3.0/src/xju/cmc/async_cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-1.3.0/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14657 2023-06-17 10:59:19.000000 xju-1.3.0/src/xju/cmc/cmclass.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.132263 xju-1.3.0/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.3.0/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.3.0/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.3.0/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.3.0/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.3.0/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.3.0/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.3.0/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.3.0/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.3.0/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.3.0/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.3.0/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.3.0/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.3.0/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.3.0/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.3.0/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.3.0/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    63268 2023-06-21 10:25:57.000000 xju-1.3.0/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    42007 2023-06-11 10:43:01.000000 xju-1.3.0/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.3.0/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.3.0/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.3.0/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.3.0/src/xju/misc.py.test
--r--r--r--   0 xju       (1001) xju       (1001)    22865 2023-06-11 07:25:02.000000 xju-1.3.0/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11796 2023-06-11 09:21:50.000000 xju-1.3.0/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.3.0/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.3.0/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.3.0/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.3.0/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:39.000000 xju-1.3.0/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.3.0/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.3.0/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.3.0/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.3.0/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7236 2023-06-21 01:02:08.000000 xju-1.3.0/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5202 2023-06-21 01:07:25.000000 xju-1.3.0/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-06-21 10:31:40.128263 xju-1.3.0/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)     9044 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1380 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-06-21 10:31:40.000000 xju-1.3.0/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-07-05 10:32:09.000000 xju-1.4.0/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)     9092 2023-07-05 10:32:10.205364 xju-1.4.0/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     7556 2023-07-05 10:32:09.000000 xju-1.4.0/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1742 2023-07-05 10:32:09.000000 xju-1.4.0/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-07-05 10:32:10.205364 xju-1.4.0/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.201364 xju-1.4.0/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.201364 xju-1.4.0/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-1.4.0/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-1.4.0/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju/cmc/
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     9781 2023-06-20 09:48:20.000000 xju-1.4.0/src/xju/cmc/AsyncDict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-1.4.0/src/xju/cmc/AsyncOpt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.4.0/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-06-11 03:07:27.000000 xju-1.4.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.4.0/src/xju/cmc/Dict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-1.4.0/src/xju/cmc/Opt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.4.0/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    41771 2023-06-21 01:30:26.000000 xju-1.4.0/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8562 2023-06-26 21:01:25.000000 xju-1.4.0/src/xju/cmc/async_cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-1.4.0/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14657 2023-06-17 10:59:19.000000 xju-1.4.0/src/xju/cmc/cmclass.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.4.0/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.4.0/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.4.0/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.4.0/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.4.0/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.4.0/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.4.0/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.4.0/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.4.0/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.4.0/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.4.0/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.4.0/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.4.0/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.4.0/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.4.0/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.4.0/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    70831 2023-07-03 10:56:25.000000 xju-1.4.0/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    45743 2023-07-03 10:53:19.000000 xju-1.4.0/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.4.0/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.4.0/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.4.0/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.4.0/src/xju/misc.py.test
+-r--r--r--   0 xju       (1001) xju       (1001)    22865 2023-06-11 07:25:02.000000 xju-1.4.0/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11796 2023-06-11 09:21:50.000000 xju-1.4.0/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.4.0/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.4.0/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.4.0/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.4.0/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:09.000000 xju-1.4.0/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.4.0/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.4.0/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.4.0/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.4.0/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7232 2023-07-02 10:20:30.000000 xju-1.4.0/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     5202 2023-06-21 01:07:25.000000 xju-1.4.0/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)     9092 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1380 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/top_level.txt
```

### Comparing `xju-1.3.0/MIT-LICENCE` & `xju-1.4.0/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/PKG-INFO` & `xju-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.3.0
+Version: 1.4.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -144,15 +144,15 @@
 * wrapper for subprocess.Popen that captures very common usage without the option-and-flag-warren of subprocess
 
 * see `xju/cmd.py.test <xju/cmd.py.test>`_ for sample code
 
 
 `xju.json_codec <xju/json_codec.py>`_
 
-* encoding/decoding type-hinted dict/list/int/bool/None/float/str and classes to and from json
+* encoding/decoding type-hinted dict/list/int/bool/None/float/str/Enum and classes to and from json
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
@@ -188,14 +188,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
 - 1.2.13 xju.newtype eq/neq now follows python "you can compare apples to oranges", rely on mypy --strict-equality (which for what it's worth is broken at mypy 1.3.0)
```

### Comparing `xju-1.3.0/README.rst` & `xju-1.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 * wrapper for subprocess.Popen that captures very common usage without the option-and-flag-warren of subprocess
 
 * see `xju/cmd.py.test <xju/cmd.py.test>`_ for sample code
 
 
 `xju.json_codec <xju/json_codec.py>`_
 
-* encoding/decoding type-hinted dict/list/int/bool/None/float/str and classes to and from json
+* encoding/decoding type-hinted dict/list/int/bool/None/float/str/Enum and classes to and from json
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
@@ -167,14 +167,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
 - 1.2.13 xju.newtype eq/neq now follows python "you can compare apples to oranges", rely on mypy --strict-equality (which for what it's worth is broken at mypy 1.3.0)
```

### Comparing `xju-1.3.0/pyproject.toml` & `xju-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "1.3.0"
+version = "1.4.0"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `xju-1.3.0/src/xju/assert_.py` & `xju-1.4.0/src/xju/assert_.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/assert_.py.test` & `xju-1.4.0/src/xju/assert_.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/AsyncDict.py.test` & `xju-1.4.0/src/xju/cmc/AsyncDict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/AsyncOpt.py.test` & `xju-1.4.0/src/xju/cmc/AsyncOpt.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-1.4.0/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test` & `xju-1.4.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/Dict.py.test` & `xju-1.4.0/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/Opt.py.test` & `xju-1.4.0/src/xju/cmc/Opt.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-1.4.0/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/__init__.py` & `xju-1.4.0/src/xju/cmc/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/async_cmclass.py.test` & `xju-1.4.0/src/xju/cmc/async_cmclass.py.test`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,33 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 import sys
 import asyncio
+from dataclasses import dataclass, field
 from xju.assert_ import Assert
 from xju.xn import readable_repr, in_context
-from typing import Self
+from typing import Self, Awaitable, Generator
 from contextlib import AbstractContextManager, AbstractAsyncContextManager
 from xju.cmc import AsyncCM, async_cmclass
 
 _log:list[str]=[]
 
 def log(s: str) -> int:
     _log.append(s)
     print(s,file=sys.stderr)
     return len(_log)
 
+def extract_log() -> list[str]:
+    result=_log[:]
+    del _log[:]
+    return result
+
 class Resource:
     name: str
     entered_at: int|None = None
     exited_at: int|None = None
     ee: None|Exception
     xe: None|Exception
 
@@ -212,16 +218,55 @@
             pass
     except Exception as e:
         Assert(readable_repr(e))=='fred'
     else:
         assert False
         pass
     
-    Assert(_log)==[
+    Assert(extract_log())==[
         '+ aenter SA.A.a', '- aenter SA.A.a',
         '+ enter SA.A.b', '- enter SA.A.b',
         '+ aenter SA.A.c', 'E enter SA.A.c',
         '+ exit SA.A.b', '- exit SA.A.b',
         '+ aexit SA.A.a', '- aexit SA.A.a']
     pass
 
+async def async_init_dataclass_example() -> None:
+    async def some_async_function(x: int) -> str:
+        await asyncio.sleep(0.1)
+        return f"{x=}"
+    
+    @async_cmclass
+    @dataclass
+    class AsyncInit(AsyncCM):
+        # a class whose initialastion needs await statements
+        # python __init__() cannot be async, so use it to capture
+        # parameters p1, p2 and implement the asynchronous initialisation
+        # via __await__
+        p1: int
+        p2: list[str]
+
+        # attributes that will be initialised in an async "init" function
+        a: Resource = field(init=False)
+        b: int = field(init=False)
+        c: AsyncResource = field(init=False)
+
+        def __await__(self) -> Generator[None,None,'AsyncInit']:
+            """init AsyncInt asynchronously from parameters {self.p1=}, {self.p2=}
+               - this provides pseudo async __init__() i.e. await AsyncInit(x,y)
+               - do not call multiple times!"""
+            async def f() -> 'AsyncInit':
+                self.a=Resource(await some_async_function(self.p1), ee=None, xe=None)
+                self.b=self.p1 * len(self.p2)
+                self.c=AsyncResource('/'.join(self.p2), ee=None, xe=None)
+                return self
+            return f().__await__()
+
+        pass
+
+    async with await AsyncInit(6, ['fred','jock']):
+        Assert(extract_log())==['+ enter x=6', '- enter x=6', '+ aenter fred/jock', '- aenter fred/jock']
+        pass
+    Assert(extract_log())==['+ aexit fred/jock', '- aexit fred/jock', '+ exit x=6', '- exit x=6']
+
 asyncio.run(main())
+asyncio.run(async_init_dataclass_example())
```

### Comparing `xju-1.3.0/src/xju/cmc/cmc.py.test` & `xju-1.4.0/src/xju/cmc/cmc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/cmclass.py.test` & `xju-1.4.0/src/xju/cmc/cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/FileLock.py.test` & `xju-1.4.0/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/FileMode.py.test` & `xju-1.4.0/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/FilePosition.py.test` & `xju-1.4.0/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/FileReader.py.test` & `xju-1.4.0/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/FileWriter.py.test` & `xju-1.4.0/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/Pipe.py.test` & `xju-1.4.0/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-1.4.0/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/io/__init__.py` & `xju-1.4.0/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/perflog.py` & `xju-1.4.0/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/perflog.py.test` & `xju-1.4.0/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/signal.py` & `xju-1.4.0/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/signal.py.test` & `xju-1.4.0/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/tstore.py` & `xju-1.4.0/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmc/tstore.py.test` & `xju-1.4.0/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmd.py` & `xju-1.4.0/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/cmd.py.test` & `xju-1.4.0/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/json_codec.py` & `xju-1.4.0/src/xju/json_codec.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,23 +24,25 @@
 #   codec(Address).decode({'number':32, 'street': 'asler'})==Address(32,'asler')
 #   codec(Address).decode({'number':'42 biz', 'street': 'asler'})==Address('42 biz','asler')
 #   codec(Address).encode(Address(32,'asler'))=={'number':32, 'street': 'asler'}
 #
 # For examples see json_codec.py.test
 #
 from dataclasses import dataclass
-from xju.xn import Xn,in_context,in_function_context,readable_repr
+from xju.xn import Xn,in_context,in_function_context,readable_repr, AllFailed
 from typing import TypeVar, Generic, Type, cast, Any, Protocol, Self, Callable, get_type_hints
 from typing import Sequence, Literal, NewType
 from typing import _LiteralGenericAlias  # type: ignore  # mypy 1.1.1
 from typing import _UnionGenericAlias  # type: ignore  # mypy 1.1.1
 from typing import _GenericAlias  # type: ignore  # mypy 1.2.0
 from typing import get_origin,get_args, runtime_checkable
 from types import GenericAlias, UnionType, NoneType
 import xju.newtype
+from enum import Enum, EnumType, EnumMeta
+import json
 
 T=TypeVar('T')
 
 JsonType = None|bool|dict|list|float|str
 
 class TypeScriptUQNTag:pass
 class TypeScriptUQN(xju.newtype.Str[TypeScriptUQNTag]):pass
@@ -431,39 +433,38 @@
     def __init__(self,allowed_types, value_codecs):
         self.allowed_types=allowed_types
         self.value_codecs=value_codecs
         pass
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
         'encode {x!r} as one of {self.allowed_types}'
         try:
-            exceptions=[]
+            exceptions=list[BaseException]()
             for t, c in self.value_codecs.items():
                 try:
                     return c.encode(x,back_ref)
                 except Exception as e:
-                    exceptions.append( (t, e) )
+                    exceptions.append(in_context(f'decode as {t!r}'))
                     pass
                 pass
-            raise Exception(' and '.join([f'failed to encode as {t} because {e}' for t,e in exceptions]))
-                
+            raise AllFailed(exceptions)
         except Exception:
             raise in_function_context(UnionCodec.encode,vars()) from None
         pass
     def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> tuple:
         '''decode {x!r} as one of {self.allowed_types}'''
         try:
-            exceptions=[]
+            exceptions=list[BaseException]()
             for t, c in self.value_codecs.items():
                 try:
                     return c.decode(x,back_ref)
                 except Exception as e:
-                    exceptions.append( (t, e) )
+                    exceptions.append(in_context(f'decode as {t!r}'))
                     pass
                 pass
-            raise Exception(' and '.join([f'failed to decode as {t!r} because {e}' for t,e in exceptions]))
+            raise AllFailed(exceptions)
         except Exception:
             raise in_function_context(UnionCodec.decode,vars()) from None
         pass
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             "oneOf": [ codec.get_json_schema(definitions, self_ref) for codec in self.value_codecs.values() ]
         }
@@ -675,17 +676,15 @@
     def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewInt:
         if not isinstance(x, int):
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not an int')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
-        if self.t.__module__=='__main__':
-            return self.t.__name__
-        return f"{self.t.__module__}.{self.t.__name__}"
+        return get_type_fqn(self.t)
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'integer'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'number'
@@ -743,17 +742,15 @@
     def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewFloat:
         if type(x) is not float and type(x) is not int:
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not a float (or an int)')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
-        if self.t.__module__=='__main__':
-            return self.t.__name__
-        return f"{self.t.__module__}.{self.t.__name__}"
+        return get_type_fqn(self.t)
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'number'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'number'
@@ -811,17 +808,15 @@
     def decode(self, x:JsonType,back_ref:None|Callable[[JsonType],Any])->NewStr:
         if type(x) is not str:
             t=type(x)
             raise Exception(f'{x!r} (of type {t}) is not an str')
         return self.t(self.base_codec.decode(x,back_ref))
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
-        if self.t.__module__=='__main__':
-            return self.t.__name__
-        return f"{self.t.__module__}.{self.t.__name__}"
+        return get_type_fqn(self.t)
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             'description': self.get_type_fqn(),
             'type': 'string'
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         return 'string'
@@ -1087,17 +1082,15 @@
             except Exception:
                 raise in_context(f'init {self.t} with keyword arguments {attr_values}') from None
         except Exception:
             raise in_function_context(ClassCodec.decode,vars()) from None
         pass
     def get_type_fqn(self):
         '''get the fully qualified name of {self.t}'''
-        if self.t.__module__ == "__main__":
-            return self.t.__name__
-        return f'{self.t.__module__}.{self.t.__name__}'
+        return get_type_fqn(self.t)
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         if self.custom_codec is not None:
             return self.custom_codec.xju_json_codec_get_json_schema(definitions)
         fqn=self.get_type_fqn()
         self_ref=f'#/definitions/{fqn}'
         if not fqn in definitions:
             definitions[fqn]={
@@ -1186,14 +1179,171 @@
             return self.custom_codec.xju_json_codec_get_typescript_asa(expression,namespace)
         self.ensure_typescript_defs(namespace)
         fqn=self.get_type_fqn().split('.')
         fqn=self.get_type_fqn().split('.')
         return TypeScriptSourceCode('.'.join(fqn[0:-1]+[f"asInstanceOf{fqn[-1]}({expression})"]))
     pass
 
+@dataclass
+class EnumValueCodec:
+    t:EnumMeta
+    value:Enum
+    value_codec:CodecProto
+
+    def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
+        'encode {x!r} as a {self.t.__name__}.{self.value.name}'
+        try:
+            return self.value_codec.encode(x.value,back_ref)
+        except Exception:
+            raise in_function_context(EnumValueCodec.encode,vars()) from None
+        pass
+    def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> Enum:
+        'deocde {x!r} as {self.t.__name__}.{self.value.name}'
+        try:
+            value=self.value_codec.decode(x,back_ref)
+            if value != self.value.value:
+                raise Exception(f'{value!r} is not {self.value.value!r}')
+            return self.value
+        except Exception:
+            raise in_function_context(EnumValueCodec.decode,vars()) from None
+        pass
+    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        result = self.value_codec.get_json_schema(definitions,self_ref)
+        result.update({
+            'enum': [ self.value_codec.encode(self.value.value,None) ]
+        })
+        return result
+    def get_type_fqn(self):
+        '''get the fully qualified name of {self.t}'''
+        return get_type_fqn(self.t)
+    def typescript_type(self,back_refs:TypeScriptBackRefs|None) -> str:
+        return f'{self.get_type_fqn()}.{self.value.name}'
+    def typescript_value(self) -> TypeScriptSourceCode:
+        return TypeScriptSourceCode(json.dumps(self.value.value))
+    def ensure_typescript_defs(self,namespace)->None:
+        # EnumCodec supplies defs
+        pass
+    def get_typescript_isa(
+            self,
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace,
+            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        return TypeScriptSourceCode(f'({expression} === {self.typescript_type(back_refs)})')
+    def get_typescript_asa(
+            self,
+            expression:TypeScriptSourceCode,
+            namespace: TypeScriptNamespace,
+            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        tt=self.typescript_type(back_refs)
+        return TypeScriptSourceCode(
+            f"((v: any): {tt} => {{\n"
+            f"    if (v !== {tt}) throw new Error(`the ${{typeof v}} ${{v}} is not {tt}`);\n"
+            f"    return v as {tt};\n"
+            f"}})({expression})")
+    pass
+    
+class EnumCodec:
+    def __init__(self,t:EnumMeta, value_codecs:dict[str, EnumValueCodec]):
+        self.t=t
+        self.value_codecs=value_codecs
+        pass
+    def encode(self,x:Enum,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
+        'encode {self.t} value {x!r}'
+        try:
+            if not isinstance(x, self.t):
+                raise Exception(f'{x} (of type {x.__class__.__name__}) is not a {self.t.__name__}')
+            return self.value_codecs[x.name].encode(x,back_ref)
+        except Exception:
+            raise in_function_context(EnumCodec.encode,vars()) from None
+        pass
+    def decode(self,x,back_ref:None|Callable[[JsonType],Any]) -> Enum:
+        '''decode {x!r} as enum {self.t.__name__} value'''
+        try:
+            exceptions=list[BaseException]()
+            for n, c in self.value_codecs.items():
+                try:
+                    return c.decode(x,back_ref)
+                except Exception:
+                    exceptions.append(in_context(f'decode as {self.t.__name__}.{n}'))
+                    pass
+                pass
+            raise AllFailed(exceptions)
+        except Exception:
+            raise in_function_context(EnumCodec.decode,vars()) from None
+        pass
+    def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
+        return {
+            "oneOf": [
+                codec.get_json_schema(definitions, self_ref) for codec in self.value_codecs.values() ]
+        }
+    def get_type_fqn(self):
+        '''get the fully qualified name of {self.t}'''
+        return get_type_fqn(self.t)
+    def typescript_type(self,back_refs:TypeScriptBackRefs|None)->str:
+        return self.get_type_fqn()
+    def ensure_typescript_defs(self, namespace) -> None:
+        typescript_fqn=[TypeScriptUQN(_) for _ in self.get_type_fqn().split('.')]
+        target_namespace=namespace.get_namespace_of(typescript_fqn)
+        typescript_type_name=typescript_fqn[-1]
+        if typescript_type_name not in target_namespace.defs:
+            enum_value_codec:EnumValueCodec
+            target_namespace.defs[typescript_type_name]=TypeScriptSourceCode(
+                f"enum {typescript_type_name} {{\n"+
+                ',\n'.join([f'    {name} = {enum_value_codec.typescript_value().value()}'
+                         for name, enum_value_codec in self.value_codecs.items()])+
+                f'\n}};\n')
+            target_namespace.defs[TypeScriptUQN(f"asInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
+                f"function asInstanceOf{typescript_type_name}(v: any): {typescript_type_name}\n"
+                f"{{\n"
+                f"    return {indent(4,self.get_typescript_asa(TypeScriptSourceCode('v'),namespace,None))};\n"
+                f"}}")
+            target_namespace.defs[TypeScriptUQN(f"isInstanceOf{typescript_type_name}")]=TypeScriptSourceCode(
+                f"function isInstanceOf{typescript_type_name}(v:any): v is {typescript_type_name}\n"
+                f"{{\n"
+                f"    return {indent(4,self.get_typescript_isa(TypeScriptSourceCode('v'),namespace,None))};\n"
+                f"}}")
+        pass
+    def get_typescript_isa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        enum_value_codec:EnumValueCodec
+        isas=[' ||\n       '+indent(12,enum_value_codec.get_typescript_isa(TypeScriptSourceCode(f"v"),
+                                                                           namespace,back_refs))
+              for enum_value_codec in self.value_codecs.values()]
+        return TypeScriptSourceCode(
+            f"((v:any): v is {self.typescript_type(back_refs)}=>{{\n"
+            f"    return false" +
+            f"".join(isas) + ";\n"+
+            f"}})({expression})")
+    def get_typescript_asa(self,
+                           expression:TypeScriptSourceCode,
+                           namespace: TypeScriptNamespace,
+                           back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
+        enum_value_codec:EnumValueCodec
+        tt=self.typescript_type(back_refs)
+        asas=[f"    try{{\n"+
+              f"        {indent(8,enum_value_codec.get_typescript_asa(TypeScriptSourceCode('v'),namespace,back_refs))};\n"+
+              f"        return v as {tt};\n"+
+              f"    }}\n"+
+              f"    catch(e:any){{\n"+
+              f"        es.push(e.message);\n"+
+              f"    }};\n"
+              for enum_value_codec in self.value_codecs.values()]
+        return TypeScriptSourceCode(
+            f"((v: any): {tt} => {{try{{\n" +
+            f"    var es = new Array<string>();\n"+
+            "".join(asas)+
+            f"    throw new Error(es.join(' and '));\n"+
+            f"}}catch(e:any)\n"+
+            f"{{\n"+
+            f"    throw new Error(`${{v}} is not a {tt} because ${{e}}`);\n"+
+            f"}}}})({expression})")
+    pass
+
 class SelfCodec:
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]) -> JsonType:
         'encode {x} as a Self'
         try:
             assert back_ref is not None
             return back_ref(x)
         except Exception:
@@ -1230,15 +1380,15 @@
             expression:TypeScriptSourceCode,
             namespace: TypeScriptNamespace,
             back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         assert back_refs is not None
         return back_refs.asa_back_ref(expression)
     pass
     
-def _explodeSchema(t:type|NewType|TypeVar|GenericAlias|UnionType|_LiteralGenericAlias|_GenericAlias,
+def _explodeSchema(t:type|NewType|TypeVar|GenericAlias|UnionType|_LiteralGenericAlias|_GenericAlias|Enum|Type[Enum],
                    type_var_map:dict[TypeVar,Any]|None):
     '''explode type {t!r} into a tree of codecs using map {type_var_map} to resolve any generic type refs i.e. TypeVars'''
     try:
         if type(t) is TypeVar:
             assert type_var_map is not None
             assert t in type_var_map, type_var_map.keys()
             return _explodeSchema(type_var_map[t],type_var_map)
@@ -1281,15 +1431,21 @@
                 for type_var, value in
                 list((type_var_map or {}).items())+list(zip(get_origin(t).__parameters__, get_args(t)))
             }
             return ClassCodec(
                 get_origin(t),
                 { n: _explodeSchema(nt,local_type_var_map)
                   for n,nt in get_type_hints(get_origin(t)).items()})
-        assert isinstance(t,type), t
+        if type(t) is EnumType and issubclass(t, Enum):
+            return EnumCodec(
+                t,{name: _explodeSchema(vv,type_var_map)
+                   for name,vv in t.__members__.items()})
+        if isinstance(t,Enum):
+            return EnumValueCodec(t.__class__,t,_explodeSchema(type(t.value),type_var_map))
+        assert isinstance(t,type), (type(t), t)
         if issubclass(t,xju.newtype.Int):
             return NewIntCodec(t)
         if issubclass(t,xju.newtype.Float):
             return NewFloatCodec(t)
         if issubclass(t,xju.newtype.Str):
             return NewStrCodec(t)
         return ClassCodec(
@@ -1312,7 +1468,12 @@
     except:
         raise in_function_context(_explode_literal, vars())
     pass
 
 def indent(n: int, s:TypeScriptSourceCode)->str:
     lines=s.splitlines()
     return '\n'.join([lines[0].value()]+[(' '*n)+l.value() for l in lines[1:]])
+
+def get_type_fqn(t:type) -> str:
+    if t.__module__=='__main__':
+        return t.__name__
+    return f"{t.__module__}.{t.__name__}"
```

### Comparing `xju-1.3.0/src/xju/json_codec.py.test` & `xju-1.4.0/src/xju/json_codec.py.test`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from typing import cast, Type, Literal, Any, Self, NewType, Generic, TypeVar
 from types import NoneType
 from dataclasses import dataclass, field
 import re
 import sys
 import ipaddress
+from enum import Enum
 
 from xju.assert_ import Assert
 import xju.newtype
 from xju.xn import readable_repr
 from xju.time import Timestamp
 
 x:Any
@@ -301,14 +302,69 @@
     x=codec(Surname).encode(17) # type: ignore
 except Exception as e:
     Assert("17 is not a <class '__main__.Surname'>").isIn(str(e))
 else:
     assert False, x
     pass
 
+
+#enum support...
+
+class O(Enum):
+    a='fred'
+    b=7
+    pass
+
+#... member codecs...
+Assert(codec(O.a).decode('fred'))==O.a  # type: ignore
+Assert(codec(O.a).encode(O.a))=='fred'  # type: ignore
+try:
+    x=codec(O.a).decode(7)  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode 7 to a O.a because\nfailed to deocde 7 as O.a because\n7 (of type <class 'int'>) is not a <class 'str'>."
+else:
+    assert False, x
+try:
+    x=codec(O.a).decode('jock')  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode jock to a O.a because\nfailed to deocde 'jock' as O.a because\n'jock' is not 'fred'."
+else:
+    assert False, x
+try:
+    x=codec(O.a).encode(O.b)  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to encode <O.b: 7> as a O.a because\n7 is not a <class 'str'>."
+else:
+    assert False, x
+
+#... enum codec itself
+Assert(codec(O).decode('fred'))==O.a  # type: ignore
+Assert(codec(O).decode(7))==O.b  # type: ignore
+Assert(codec(O).encode(O.a))=='fred'  # type: ignore
+Assert(codec(O).encode(O.b))==7  # type: ignore
+try:
+    x=codec(O).decode(8)  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode 8 to a <enum 'O'> because\nfailed to decode 8 as enum O value because\n- failed to decode as O.a because\n  failed to deocde 8 as O.a because\n  8 (of type <class 'int'>) is not a <class 'str'>; and\n- failed to decode as O.b because\n  failed to deocde 8 as O.b because\n  8 is not 7."
+else:
+    assert False, x
+try:
+    x=codec(O).decode('jock')  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to decode jock to a <enum 'O'> because\nfailed to decode 'jock' as enum O value because\n- failed to decode as O.a because\n  failed to deocde 'jock' as O.a because\n  'jock' is not 'fred'; and\n- failed to decode as O.b because\n  failed to deocde 'jock' as O.b because\n  'jock' (of type <class 'str'>) is not a <class 'int'>."
+else:
+    assert False, x
+try:
+    x=codec(O).encode(7.1)  # type: ignore
+except Exception as e:
+    Assert(readable_repr(e))=="Failed to encode <enum 'O'> value 7.1 because\n7.1 (of type float) is not a O."
+else:
+    assert False, x
+    
+
 # type unions, e.g. str|int match either type
 
 #mypy 1.0.0 bug
 #union_codec=Codec[str|int](str|int)
 # says:
 #  error: Argument 1 to "Codec" has incompatible type "UnionType"; expected "Union[Type[str], Type[int]]"  [arg-type]
 
@@ -605,22 +661,22 @@
     assert False, x
     pass
 
 # decode wrong value
 try:
     x=codec(Literal['fred','ann']).decode('jock') # type: ignore
 except Exception as e:
-    Assert(readable_repr(e))=="Failed to decode jock to a typing.Literal['fred', 'ann'] because\nfailed to decode 'jock' as one of ('fred', 'ann') because\nfailed to decode as 'fred' because 'jock' is not 'fred' and failed to decode as 'ann' because 'jock' is not 'ann'."
+    Assert(readable_repr(e))=="Failed to decode jock to a typing.Literal['fred', 'ann'] because\nfailed to decode 'jock' as one of ('fred', 'ann') because\n- failed to decode as 'fred' because\n  'jock' is not 'fred'; and\n- failed to decode as 'ann' because\n  'jock' is not 'ann'."
 else:
     assert False, x
     pass
 try:
     x=codec(Literal[6,7]).decode(8) # type: ignore
 except Exception as e:
-    Assert(readable_repr(e))=="Failed to decode 8 to a typing.Literal[6, 7] because\nfailed to decode 8 as one of (6, 7) because\nfailed to decode as 6 because 8 is not 6 and failed to decode as 7 because 8 is not 7."
+    Assert(readable_repr(e))=="Failed to decode 8 to a typing.Literal[6, 7] because\nfailed to decode 8 as one of (6, 7) because\n- failed to decode as 6 because\n  8 is not 6; and\n- failed to decode as 7 because\n  8 is not 7."
 else:
     assert False, x
     pass
 try:
     x=codec(Literal[False]).decode(True) # type: ignore
 except Exception as e:
     Assert("True is not False").isIn(str(e))
@@ -747,16 +803,17 @@
 Assert(codec(AgeInYears).get_json_schema())=={'description': 'AgeInYears', 'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Street).get_json_schema())=={'description': 'Street', 'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Metres).get_json_schema())=={'description': 'Metres', 'type': 'number', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 
 Assert(codec(Literal['fred']).get_json_schema())=={'type': 'string', 'enum': ['fred'], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
-Assert(codec(Literal[7]).get_json_schema())=={'type': 'number', 'enum': [7], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(Literal[7,8]).get_json_schema())=={'oneOf': [{'type': 'number', 'enum': [7]}, {'type': 'number', 'enum': [8]}], '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema', 'definitions': {}} # type: ignore
 Assert(codec(Literal[False]).get_json_schema())=={'type': 'boolean', 'enum': [False], 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'} # type: ignore
+Assert(codec(O).get_json_schema())=={'oneOf': [{'type': 'string', 'enum': ['fred']}, {'type': 'integer', 'enum': [7]}], '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema', 'definitions': {}} # type: ignore
 
 Assert(codec(Address).get_json_schema())=={
     '$ref': '#/definitions/Address',
     '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema',
     'definitions':{
         'Address':{
             'description': 'Address',
@@ -879,14 +936,17 @@
         'postcode': 3365},Codec[Address](Address).get_json_schema())
     jsonschema.validate(
         {'shoots':[{'shoots':[1,2]},3]},
         Codec[Branch](Branch).get_json_schema())
     jsonschema.validate(
         {'shoots':[{'shoots':[1,2]},3]},
         Codec[Branch](Branch).get_json_schema())
+    jsonschema.validate(
+        'fred',
+        Codec(O.a).get_json_schema())  # type: ignore
     pass
 
 # internal: codecs' encode()s must verify correct type passed in, otherwise
 # UnionCodec encode try-each algorithm is invalid
 try:
     x=Codec[int](int).encode('fred') # type: ignore
 except Exception as e:
@@ -938,15 +998,15 @@
                         {'type': 'boolean'},
                         {'type': 'object'},
                         {'type': 'array'},
                         {'type': 'number'},
                         {'type': 'string'}]}}}}}
 
 
-# type hint string are supported, allowing forward-decls
+# type hint strings are supported, allowing forward-decls
 @dataclass
 class ShirtSize:
     size: 'SizeCode'
     pass
 
 Small=Literal['S']
 Large=Literal['L']
@@ -1081,50 +1141,95 @@
 timestamp_codec.ensure_typescript_defs(typescript_namespace)
 
 Assert(codec(IpV4Addr).get_typescript_isa(TypeScriptSourceCode('7'),typescript_namespace))==TypeScriptSourceCode("(typeof (7) == 'string')")
 Assert(codec(IpV4Addr).get_typescript_asa(TypeScriptSourceCode('7'),typescript_namespace))==TypeScriptSourceCode("""((v: any): string => {
     if (typeof v !== 'string') throw new Error(`${v} is not a string it is a ${typeof v}`);
     return v as string;
 })(7)""")
-       
+
+codec(O).ensure_typescript_defs(typescript_namespace)  # type: ignore
+
 # ... get_formatted_defs() generates the typescript source code:
 Assert(typescript_namespace.get_formatted_defs())==TypeScriptSourceCode(
     '''\
 namespace xju {
     export namespace time {
         export type Timestamp = {
             _Timestamp__value: number;
         };
         export function asInstanceOfTimestamp(v: any): xju.time.Timestamp
         {
             try{
                 if (Array.isArray(v)) throw new Error(`${v} is an array`);
                 if (v == null) throw new Error(`${v} is not an object it is null`);
-                if (typeof v !== \'object\') throw new Error(`${v} is not an object it is a ${typeof v}`);
+                if (typeof v !== 'object') throw new Error(`${v} is not an object it is a ${typeof v}`);
                 const attr_asa=function(name:string, asa:any):any{
                     try{
                         asa(v[name]);
                     }
                     catch(e:any){
                         throw new Error(`attribute ${name} is invalid because ${e}`);
                     }
                 }
-                attr_asa(\'_Timestamp__value\',(x:any)=>((v: any): number => {
-                    if (typeof v !== \'number\') throw new Error(`${v} is not a number it is a ${typeof v}`);
+                attr_asa('_Timestamp__value',(x:any)=>((v: any): number => {
+                    if (typeof v !== 'number') throw new Error(`${v} is not a number it is a ${typeof v}`);
                     return v as number;
                 })(x));
                 return v as xju.time.Timestamp;
             }
             catch(e:any){
                 throw new Error(`${v} is not a xju.time.Timestamp because ${e}`);
             }
         }
         export function isInstanceOfTimestamp(v:any): v is xju.time.Timestamp
         {
             return (
                 !Array.isArray(v) &&
-                v !== null &&        typeof v === \'object\' &&
-                (typeof (v["_Timestamp__value"]) == \'number\'))}
+                v !== null &&        typeof v === 'object' &&
+                (typeof (v["_Timestamp__value"]) == 'number'))}
     }
 }
-''')
+
+enum O {
+    a = "fred",
+    b = 7
+};
+
+function asInstanceOfO(v: any): O
+{
+    return ((v: any): O => {try{
+        var es = new Array<string>();
+        try{
+            ((v: any): O.a => {
+                if (v !== O.a) throw new Error(`the ${typeof v} ${v} is not O.a`);
+                return v as O.a;
+            })(v);
+            return v as O;
+        }
+        catch(e:any){
+            es.push(e.message);
+        };
+        try{
+            ((v: any): O.b => {
+                if (v !== O.b) throw new Error(`the ${typeof v} ${v} is not O.b`);
+                return v as O.b;
+            })(v);
+            return v as O;
+        }
+        catch(e:any){
+            es.push(e.message);
+        };
+        throw new Error(es.join(' and '));
+    }catch(e:any)
+    {
+        throw new Error(`${v} is not a O because ${e}`);
+    }})(v);
+}
+function isInstanceOfO(v:any): v is O
+{
+    return ((v:any): v is O=>{
+        return false ||
+           (v === O.a) ||
+           (v === O.b);
+    })(v);
+}''')
```

### Comparing `xju-1.3.0/src/xju/jsonschema.py` & `xju-1.4.0/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/jsonschema.py.test` & `xju-1.4.0/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/misc.py` & `xju-1.4.0/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/misc.py.test` & `xju-1.4.0/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/newtype.py` & `xju-1.4.0/src/xju/newtype.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/newtype.py.test` & `xju-1.4.0/src/xju/newtype.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/patch.py` & `xju-1.4.0/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/patch.py.test` & `xju-1.4.0/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/pq.py` & `xju-1.4.0/src/xju/pq.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/pq.py.test` & `xju-1.4.0/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/rfc2616.py` & `xju-1.4.0/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/rfc2616.py.test` & `xju-1.4.0/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/time.py` & `xju-1.4.0/src/xju/time.py`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/time.py.test` & `xju-1.4.0/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju/xn.py` & `xju-1.4.0/src/xju/xn.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     if s.endswith('.'): s=s[:-1]
     return s[0:1].lower()+s[1:]
 
 def indent(prefix:str,s:str)->str:
     '''prefix all but first line of s by specified prefix'''
     return s.replace('\n','\n'+prefix)
 
-class AllFailed(BaseException):
+class AllFailed(Exception):
     def __init__(self,causes:Sequence[BaseException])->None:
         self.causes=causes
         pass
     def __str__(self)->str:
         return ', and\n'.join([str(cause) for cause in self.causes])
     def xju_xn_readable_repr(self)->str:
         return '; and\n'.join(['- '+
```

### Comparing `xju-1.3.0/src/xju/xn.py.test` & `xju-1.4.0/src/xju/xn.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.3.0/src/xju.egg-info/PKG-INFO` & `xju-1.4.0/src/xju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.3.0
+Version: 1.4.0
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -144,15 +144,15 @@
 * wrapper for subprocess.Popen that captures very common usage without the option-and-flag-warren of subprocess
 
 * see `xju/cmd.py.test <xju/cmd.py.test>`_ for sample code
 
 
 `xju.json_codec <xju/json_codec.py>`_
 
-* encoding/decoding type-hinted dict/list/int/bool/None/float/str and classes to and from json
+* encoding/decoding type-hinted dict/list/int/bool/None/float/str/Enum and classes to and from json
 
 * designed to fit well with type checking
 
 * built in support for xju.newtype described above
 
 * generates json schema equivalent schemas for types
 
@@ -188,14 +188,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
 - 1.2.13 xju.newtype eq/neq now follows python "you can compare apples to oranges", rely on mypy --strict-equality (which for what it's worth is broken at mypy 1.3.0)
```

### Comparing `xju-1.3.0/src/xju.egg-info/SOURCES.txt` & `xju-1.4.0/src/xju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

