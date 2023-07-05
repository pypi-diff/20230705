# Comparing `tmp/remotemanager-0.8.1.tar.gz` & `tmp/remotemanager-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.8.1.tar", last modified: Fri Jun 30 20:01:15 2023, max compression
+gzip compressed data, was "remotemanager-0.8.2.tar", last modified: Wed Jul  5 08:46:33 2023, max compression
```

## Comparing `remotemanager-0.8.1.tar` & `remotemanager-0.8.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-30 20:01:15.851386 remotemanager-0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-30 09:39:29.000000 remotemanager-0.8.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.843386 remotemanager-0.8.1/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-30 09:39:29.000000 remotemanager-0.8.1/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.1/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-29 14:39:51.000000 remotemanager-0.8.1/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.1/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.1/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    25581 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48600 2023-06-30 14:09:28.000000 remotemanager-0.8.1/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    24686 2023-06-30 13:14:43.000000 remotemanager-0.8.1/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4920 2023-06-26 12:50:24.000000 remotemanager-0.8.1/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.1/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.1/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.1/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.1/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.1/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.1/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.1/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.1/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.1/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.1/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.851386 remotemanager-0.8.1/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.1/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 20:01:15.847386 remotemanager-0.8.1/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-30 20:01:15.000000 remotemanager-0.8.1/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 20:01:15.851386 remotemanager-0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.595770 remotemanager-0.8.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-05 08:46:33.591771 remotemanager-0.8.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.8.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-03 15:08:03.000000 remotemanager-0.8.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-03 15:08:03.000000 remotemanager-0.8.2/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.8.2/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12788 2023-06-29 14:39:51.000000 remotemanager-0.8.2/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.8.2/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.8.2/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    25712 2023-07-04 13:31:41.000000 remotemanager-0.8.2/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49554 2023-07-05 08:03:59.000000 remotemanager-0.8.2/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-06-26 08:49:48.000000 remotemanager-0.8.2/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    26063 2023-07-04 09:09:29.000000 remotemanager-0.8.2/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-07-03 15:08:03.000000 remotemanager-0.8.2/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.8.2/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.8.2/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.8.2/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.8.2/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.8.2/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.8.2/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.8.2/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-07-04 13:31:41.000000 remotemanager-0.8.2/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.8.2/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.8.2/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9435 2023-06-26 08:49:48.000000 remotemanager-0.8.2/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.591771 remotemanager-0.8.2/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.8.2/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:46:33.587771 remotemanager-0.8.2/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-05 08:46:33.000000 remotemanager-0.8.2/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:46:33.595770 remotemanager-0.8.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.8.2/setup.py
```

### Comparing `remotemanager-0.8.1/LICENSE` & `remotemanager-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/PKG-INFO` & `remotemanager-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.1
+Version: 0.8.2
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.1/README.md` & `remotemanager-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/pyproject.toml` & `remotemanager-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.8.1"
+current_version = "0.8.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.8.1/remotemanager/connection/cmd.py` & `remotemanager-0.8.2/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/computers/base.py` & `remotemanager-0.8.2/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/computers/example.py` & `remotemanager-0.8.2/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/computers/options.py` & `remotemanager-0.8.2/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/computers/parsers.py` & `remotemanager-0.8.2/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/testing_object.py` & `remotemanager-0.8.2/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/connection/url.py` & `remotemanager-0.8.2/remotemanager/connection/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -606,49 +606,50 @@
         """
 
         self._logger.info(f"performing stat on files: {files}")
         if local is None:
             local = self._parent.is_local
 
         files = ensure_list(files)
-        times, error = self._file_mtime(files, local, python, ignore_empty, dry_run)
+        times, error = self._file_mtime(files, local, python, dry_run)
 
         if dry_run:
             # in this instance "times" is simply the command
             return times
 
         self._logger.info("received:")
         self._logger.info(times)
         self._logger.info(error)
         output = {}
         for file in files:
             if file in times:
-                output[file] = times[file]
 
+                mtime = times[file][0]
+                fsize = times[file][1]
+                if ignore_empty and fsize == 0:
+                    output[file] = None
+                else:
+                    output[file] = mtime
             else:
                 output[file] = None
 
         return output
 
-    def _file_mtime(
-        self, files: list, local: bool, python: bool, ignore_empty: bool, dry_run: bool
-    ):
+    def _file_mtime(self, files: list, local: bool, python: bool, dry_run: bool):
         """
         Perform the "stat -c %Y" command on a list of files,
         returning the result. Uses a python command backup if this fails
 
         Args:
             files (list):
                 list of files to check
             local (bool):
                 force a local search
             python (bool):
                 force the python override
-            ignore_empty (bool):
-                also check the filesize, ignoring empty files
             dry_run (bool):
                 print command only
 
         Returns:
             (list): list of file unix times
         """
         sep = ","
@@ -671,28 +672,26 @@
             times = {}
             for line in ret.stdout.split("\n"):
                 try:
                     fname = line.split(sep)[0]
                     mtime = int(float(line.split(sep)[1]))
                     fsize = int(float(line.split(sep)[2]))
 
-                    if ignore_empty and fsize == 0:
-                        continue
-                    times[fname] = mtime
+                    times[fname] = (mtime, fsize)
                 except IndexError:
                     pass
 
             return times, ret.stderr.split("\n"), ret.returncode, ret.stderr
 
         def pystat():
             self._logger.debug("attempting python stat on files")
             ex = f"""import os
 files={files}
 for f in files:
-\ttry: print(f'{{f}}{sep}{{os.stat(f).st_mtime}}')
+\ttry: print(f'{{f}}{sep}{{os.stat(f).st_mtime}}{sep}{{os.stat(f).st_size}}')
 \texcept FileNotFoundError: print(f)"""
 
             cmd = f'{self._parent.python} -c "{ex}"'
 
             ret = self._parent.cmd(
                 cmd, local=local, raise_errors=False, dry_run=dry_run
             )
@@ -700,15 +699,19 @@
             if dry_run:
                 return ret, None
 
             times = {}
             error = []
             for line in ret.stdout.split("\n"):
                 try:
-                    times[line.split(sep)[0]] = int(float(line.split(sep)[1]))
+                    fname = line.split(sep)[0]
+                    mtime = int(float(line.split(sep)[1]))
+                    fsize = int(float(line.split(sep)[2]))
+
+                    times[fname] = (mtime, fsize)
                 except IndexError:
                     error.append(line.strip())
 
             return times, error
 
         files = ensure_list(files)
```

### Comparing `remotemanager-0.8.1/remotemanager/dataset/dataset.py` & `remotemanager-0.8.2/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1034,15 +1034,21 @@
 
         Returns (bool):
             all(states)
         """
         return all([r == state for r in self.get_all_runner_states()])
 
     @property
-    def last_run(self):
+    def last_run(self) -> [int, None]:
+        """
+        Returns the unix time of the last _run call
+
+        Returns:
+            (int): unix time of last  _run call, or None if impossible
+        """
         if self._last_run > 0:
             return self._last_run
         return None
 
     def run(
         self,
         force: bool = False,
@@ -1116,15 +1122,14 @@
         master_scripts = {}
         any_file_written = False
         asynchronous = None
         for runner in self.runners:
             if not runner._assess_run(**temp_args):
                 continue
 
-            runner.state = Runner._submit_status["initial"]
             runner._write_runfile(self)
             any_file_written = True
 
             self._logger.info("writing script with run args:")
             self._logger.info(format_iterable(runner.run_args))
 
             script = self._script_sub(avoid_nodes, **runner.run_args)
@@ -1153,14 +1158,15 @@
 
             for file in runner.extra_files["send"]:
                 self.transport.queue_for_push(
                     os.path.split(file)[1], os.path.split(file)[0], runner.remote_dir
                 )
 
             runners_to_update.append(runner.uuid)
+            runner.state = "staged"
 
         if not any_file_written:
             return self._run_finalise()
 
         cmds = []
         i = 0
         for remote, lines in master_scripts.items():
@@ -1184,19 +1190,18 @@
 
             # send a repo for each new remote dir
             # TODO this should ideally be reduced to just _one_
             self._write_to_repo(self.local_dir, remote)
 
         if not dry_run:
             self.transport.transfer()
-            self.set_runner_states("files copied to remote", runners_to_update)
+            self.set_runner_states("submit pending", runners_to_update)
             if self.is_child:
                 self._logger.info(f"{self} is child, returning")
                 return self._run_finalise()
-            self.set_runner_states(Runner._submit_status["final"], runners_to_update)
             for cmd in cmds:
                 self._run_cmds.append(self.url.cmd(cmd, asynchronous=asynchronous))
         else:
             self.transport.wipe_transfers()
             for cmd in cmds:
                 self._logger.important(f"launch command: {cmd}")
             self.set_runner_states("dry run", runners_to_update)
@@ -1418,14 +1423,16 @@
                     submission time for the runner
 
             Returns:
                 bool
             """
             if not mtime:
                 return False
+            if last_sub is None:
+                return False
             if mtime >= last_sub:
                 return True
             return False
 
         for runner in self.runners:
             # if we've already decided this runner, ignore it
             if ret[runner.uuid] is not None:
@@ -1455,29 +1462,61 @@
         Check if `all` runners have finished
 
         Returns (bool):
             True if all runners have completed their runs
         """
         return all(self.is_finished)
 
-    def wait(self, interval: int = 10, timeout: int = None) -> None:
+    def wait(
+        self, interval: int = 10, timeout: int = None, watch: bool = False
+    ) -> None:
         """
-        Block run until completion, checking every `interval` seconds
+        Watch the calculation, printing updates as runners complete
 
         Args:
-            interval (int):
+            interval:
                 check interval time in seconds
-            timeout (int):
-                maximum time to wait (s)
+            timeout:
+                maximum time to wait in seconds
+            watch:
+                print an updating table of runner states
+
+        Returns:
+
         """
+        if watch:
+            from IPython.display import clear_output
+
         t0 = time.time()
-        while not all(self._is_finished(verbose=False)):
+
+        states = self._is_finished(verbose=False)
+        while not all(states):
             time.sleep(interval)
 
-            if timeout is not None and time.time() - t0 > timeout:
+            states = self._is_finished(verbose=False)
+
+            if watch:
+                clear_output(wait=True)
+                print(
+                    f"watching {len(self.runners)} runners, with a {interval}s interval"
+                )
+
+                if timeout:
+                    print(f"will time out if t > {timeout}")
+
+            dt = time.time() - t0
+
+            if watch:
+                print(f"t={dt:.2f}")
+
+                for runner, state in zip(self.runners, states):
+                    statetxt = "completed" if state else "running..."
+                    print(f"{runner.name}, {statetxt}")
+
+            if timeout is not None and dt > timeout:
                 raise RuntimeError("wait timed out")
 
     @property
     def results(self) -> list:
         """
         Access the results of the runners
```

### Comparing `remotemanager-0.8.1/remotemanager/dataset/dependency.py` & `remotemanager-0.8.2/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/dataset/runner.py` & `remotemanager-0.8.2/remotemanager/dataset/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,14 @@
     """
 
     _defaults = {"skip": True}
 
     _default_local_dir = "temp_runner_local"
     _default_remote_dir = "temp_runner_remote"
 
-    _submit_status = {
-        "initial": "creating files and submitting...",
-        "final": "command executed remotely",
-    }
-
     _args_replaced_key = "~serialised_args~"
 
     _do_not_package = ["_serialiser", "_parent", "_database"]
 
     def __init__(
         self,
         arguments: dict,
@@ -105,15 +100,17 @@
         self._runner_uuid = generate_uuid(format_iterable(uuid_slug))
         self._uuid = generate_uuid(self._runner_uuid + str(self.parent.uuid))
 
         self._logger.info(f"new runner (id {self.uuid}) created")
 
         self._args = arguments
         self._state_time = None
-        self._last_submitted = -1
+        self._last_submitted = None
+        self._last_resultfile = 0
+        self._last_errorfile = 0
         self._state = None
         self._extension = "yaml"
 
         self._dependency_info = {}
 
         self._dbfile = dbfile
 
@@ -388,24 +385,28 @@
             return timestamp
 
         finished = False
         # first try read results
         timestamp = check_file_mtime(self.resultfile.local)
         if timestamp > 0:
             mtime = datetime.fromtimestamp(timestamp)
-            self.insert_history(mtime, "resultfile created remotely")
+            if timestamp != self._last_resultfile:
+                self.insert_history(mtime, "resultfile created remotely")
+            self._last_resultfile = timestamp
 
             self.result = self.parent.serialiser.load(self.resultfile.local)
             finished = True
 
         # do the same for the error
         timestamp = check_file_mtime(self.errorfile.local)
         if timestamp > 0:
             mtime = datetime.fromtimestamp(timestamp)
-            self.insert_history(mtime, "errorfile created remotely")
+            if timestamp != self._last_errorfile:
+                self.insert_history(mtime, "errorfile created remotely")
+            self._last_errorfile = timestamp
 
             with open(self.errorfile.local, "r") as o:
                 error = o.read().strip()
 
             if error != "":
                 self._logger.runtime("valid error found, storing")
                 self.error = error.split("\n")[-1]
@@ -462,15 +463,15 @@
         Creates and sets the error property
 
         Args:
             error:
                 run error string
         """
         self._error = error
-        self.state = "completed"
+        self.state = "failed"
 
     def clear_result(self) -> None:
         """
         Removes any results, and sets the state to "result wiped"
         """
         if hasattr(self, "_result"):
             del self._result
@@ -497,15 +498,15 @@
                 self._logger.info("Done")
             except FileNotFoundError:
                 self._logger.info("file not found")
 
         remove_file(self.resultfile.local)
         remove_file(self.resultfile.remote)
 
-        self.state = "result wiped"
+        self.state = "reset"
 
     @property
     def state(self) -> str:
         """
         Returns the most recent runner state
         """
         return self._state
@@ -518,17 +519,18 @@
 
         t = int(time.time())
         state_time = datetime.fromtimestamp(t)
 
         self.insert_history(state_time, newstate)
         self._state_time = t
 
-        if newstate == Runner._submit_status["final"]:
+        if newstate == "submit pending":
+            self._logger.runtime(f"updating last submitted to {t}")
             self._last_submitted = t
-        self._state = newstate
+        self._state = RunnerState(newstate)
 
     @property
     def last_updated(self) -> int:
         """
         Time that this runner state last changed
         """
         return self._state_time
@@ -586,15 +588,15 @@
         timekey = f"{base_timekey}/{idx}"
         while timekey in self._history:
             idx += 1
 
             timekey = f"{base_timekey}/{idx}"
 
         self._logger.info(
-            f"({timekey}) updating runner {self.short_uuid} state -> {newstate}"
+            f"({timekey}) updating runner {self.short_uuid} history -> {newstate}"
         )
         self._history[timekey] = newstate
 
     def run(self, dry_run: bool = False, **kwargs) -> None:
         """
         Perform a manual run
 
@@ -613,38 +615,38 @@
         if not self._assess_run(**self._run_options):
             return None
 
         if os.name == "nt" and parent.url.is_local:
             raise RuntimeError(localwinerror)
 
         self._manual_run = True  # set internal flag for a manual run
-        self.state = Runner._submit_status["initial"]
         self._write_runfile(parent)
 
         parent.transport.queue_for_push(
             self.runfile.name, self.local_dir, self.remote_dir
         )
 
         script = parent._script_sub(**self.run_args)
 
         self._write_script(parent.url.python, script)
+        self.state = "staged"
 
         parent.transport.queue_for_push(
             self.jobscript.name, self.jobscript.local_dir, self.jobscript.remote_dir
         )
 
         cmd = (
             f"cd {self.jobscript.remote_dir} &&"
             f" {parent.url.submitter} {self.jobscript.name}"
         )
 
         if not dry_run:
             parent.transport.transfer()
             parent.url.cmd(cmd, asynchronous=False)
-            self.state = Runner._submit_status["final"]
+            self.state = "submit pending"
         else:
             parent.transport.wipe_transfers()
             self._logger.important(f"launch command: {cmd}")
             self.state = "dry run"
 
     def _assess_run(self, **kwargs) -> bool:
 
@@ -661,23 +663,22 @@
         self._logger.info(format_iterable(self.run_args))
         self._logger.info(f"current state is {self.state}")
 
         if self.run_option("force", False):
             self._logger.warning("force running")
             return True
 
-        if self.state == Runner._submit_status["final"]:
-            self._logger.warning("skipping already submitted run")
-            return False
-
-        # old skip test unpacks a runner from the database
         if self.is_finished and self.run_option("skip", True):
             self._logger.warning("skipping already completed run")
             return False
 
+        if self.state >= "submit pending" and self.run_option("skip", True):
+            self._logger.warning("skipping already submitted run")
+            return False
+
         self._logger.important("checks passed, running")
         return True
 
     def _write_runfile(self, dataset, write_file: bool = True) -> str:
         """
         Writes the python file which actually runs the function
 
@@ -720,17 +721,14 @@
         output = "\n".join(runscript)
         if write_file:
             if not os.path.isdir(self.local_dir):
                 self._logger.info(f"creating local dir {self.local_dir}")
                 os.makedirs(self.local_dir)
             with open(self.runfile.local, "w+") as o:
                 o.write(output)
-            self.state = "runfile written"
-        else:
-            self.state = "runfile write skipped"
 
         return output
 
     def _write_script(self, python: str, script, write_file: bool = True) -> str:
         """
         Writes the jobscript for this runner
 
@@ -768,17 +766,14 @@
         output = "\n".join(tmp)
         if write_file:
             self._logger.info(f"writing run script to {path}")
             with open(path, "w+") as o:
                 o.write(output)
                 # Make sure the script ends with a line break
                 o.write("\n")
-            self.state = "jobscript written"
-        else:
-            self.state = "jobscript write skipped"
 
         return output
 
     @property
     def is_finished(self) -> bool:
         """
         Attempts to determine if this runner has completed its run
@@ -829,7 +824,72 @@
         """
         Display the run arguments
 
         Returns:
             (dict) run_args
         """
         return self._run_options
+
+
+class RunnerState(SendableMixin):
+    """
+    State tracker for a runner
+    """
+
+    _states = {
+        "created": 0,
+        "staged": 1,
+        "reset": 1,
+        "dry run": 1,
+        "submit pending": 2,
+        "submitted": 3,
+        "running": 4,
+        "completed": 5,
+        "failed": 5,
+    }
+
+    def __init__(self, state: str = None):
+        self.state = state
+
+    def __str__(self):
+        if self.state is None:
+            return "None"
+        return self.state
+
+    def __repr__(self):
+        return f"RunnerState({self.state})"
+
+    @property
+    def state(self):
+        return self._state
+
+    @state.setter
+    def state(self, state):
+        if state not in RunnerState._states:
+            raise ValueError(f"invalid state; {state}")
+
+        self._state = state
+
+    @property
+    def value(self):
+        return RunnerState._states[self.state]
+
+    def _prepare_compare(self, other):
+        if not isinstance(other, RunnerState):
+            other = RunnerState(other)
+
+        return other.value
+
+    def __eq__(self, other):
+        return self.value == self._prepare_compare(other)
+
+    def __lt__(self, other):
+        return self.value < self._prepare_compare(other)
+
+    def __gt__(self, other):
+        return self.value > self._prepare_compare(other)
+
+    def __le__(self, other):
+        return self.value <= self._prepare_compare(other)
+
+    def __ge__(self, other):
+        return self.value >= self._prepare_compare(other)
```

### Comparing `remotemanager-0.8.1/remotemanager/jupyter/magic.py` & `remotemanager-0.8.2/remotemanager/jupyter/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
         fargs = self.extract_in_scope(",".join(sargs), local_ns)
         fstr = self.parse_line(cell_actual, list(fargs), spull)
 
         self._logger.info(f"generated function string {fstr}")
         self._logger.info(f"Dataset args: {args}")
         self._logger.info(f"Function args: {fargs}")
 
-        run_skip = args.pop("skip", True)
+        run_skip = args.pop("skip", False)
         # Build the runner and run
-        ds = Dataset(function=fstr, skip=True, **args)
+        ds = Dataset(function=fstr, skip=False, **args)
         ds.append_run(args=fargs)
         ds.run(skip=run_skip)
 
         for cmd in ds.run_cmds:
             if cmd.stderr:
                 raise RuntimeError(f"error detected in magic run: " f"{cmd.stderr}")
         Quiet.state = True
```

### Comparing `remotemanager-0.8.1/remotemanager/logging/__init__.py` & `remotemanager-0.8.2/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/logging/log.py` & `remotemanager-0.8.2/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/logging/utils.py` & `remotemanager-0.8.2/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/logging/verbosity.py` & `remotemanager-0.8.2/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/serialisation/__init__.py` & `remotemanager-0.8.2/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/serialisation/serial.py` & `remotemanager-0.8.2/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.8.2/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.8.2/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/storage/database.py` & `remotemanager-0.8.2/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/storage/function.py` & `remotemanager-0.8.2/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/storage/remotefunction.py` & `remotemanager-0.8.2/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/storage/sendablemixin.py` & `remotemanager-0.8.2/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/transport/cp.py` & `remotemanager-0.8.2/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/transport/rsync.py` & `remotemanager-0.8.2/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/transport/scp.py` & `remotemanager-0.8.2/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/transport/transport.py` & `remotemanager-0.8.2/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/utils/__init__.py` & `remotemanager-0.8.2/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/utils/flags.py` & `remotemanager-0.8.2/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager/utils/version.py` & `remotemanager-0.8.2/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.8.1/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.8.2/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.8.1
+Version: 0.8.2
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.8.1/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.8.2/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

