# Comparing `tmp/LinuxRecycle-1.9.4.tar.gz` & `tmp/LinuxRecycle-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinuxRecycle-1.9.4.tar", last modified: Wed Jul  5 07:05:46 2023, max compression
+gzip compressed data, was "LinuxRecycle-1.9.5.tar", last modified: Wed Jul  5 07:10:18 2023, max compression
```

## Comparing `LinuxRecycle-1.9.4.tar` & `LinuxRecycle-1.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/
--rwxr-xr-x   0 maxx      (1000) research  (1001)    35149 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/LICENSE
-drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.090639 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/
--rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/PKG-INFO
--rw-r--r--   0 maxx      (1000) research  (1001)      546 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/SOURCES.txt
--rw-r--r--   0 maxx      (1000) research  (1001)        1 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/dependency_links.txt
--rw-r--r--   0 maxx      (1000) research  (1001)      168 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/entry_points.txt
--rw-r--r--   0 maxx      (1000) research  (1001)       10 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/requires.txt
--rw-r--r--   0 maxx      (1000) research  (1001)       13 2023-07-05 07:05:45.000000 LinuxRecycle-1.9.4/LinuxRecycle.egg-info/top_level.txt
--rwxr-xr-x   0 maxx      (1000) research  (1001)       47 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/MANIFEST.in
--rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/PKG-INFO
--rwxr-xr-x   0 maxx      (1000) research  (1001)     1530 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/README.md
-drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:05:46.092639 LinuxRecycle-1.9.4/linuxrecycle/
--rw-r--r--   0 maxx      (1000) research  (1001)     2223 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/AutoRegularTask.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     4984 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/DB.py
--rw-r--r--   0 maxx      (1000) research  (1001)      520 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/__init__.py
--rw-r--r--   0 maxx      (1000) research  (1001)      591 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/argv.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     2648 2023-07-05 06:50:50.000000 LinuxRecycle-1.9.4/linuxrecycle/auto_clear.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     2163 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/config.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     1489 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/main.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     2958 2023-07-05 06:50:34.000000 LinuxRecycle-1.9.4/linuxrecycle/oper.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     1332 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/printDB.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     1211 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/recover.py
--rw-r--r--   0 maxx      (1000) research  (1001)      642 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/setCrontab.py
--rwxr-xr-x   0 maxx      (1000) research  (1001)     2271 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.4/linuxrecycle/trashInfo.py
--rw-r--r--   0 maxx      (1000) research  (1001)       38 2023-07-05 07:05:46.093639 LinuxRecycle-1.9.4/setup.cfg
--rwxr-xr-x   0 maxx      (1000) research  (1001)     1510 2023-07-05 07:05:44.000000 LinuxRecycle-1.9.4/setup.py
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:10:18.727990 LinuxRecycle-1.9.5/
+-rwxr-xr-x   0 maxx      (1000) research  (1001)    35149 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/LICENSE
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:10:18.725990 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/
+-rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/PKG-INFO
+-rw-r--r--   0 maxx      (1000) research  (1001)      546 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/SOURCES.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)        1 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/dependency_links.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)      168 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/entry_points.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)       10 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/requires.txt
+-rw-r--r--   0 maxx      (1000) research  (1001)       13 2023-07-05 07:10:18.000000 LinuxRecycle-1.9.5/LinuxRecycle.egg-info/top_level.txt
+-rwxr-xr-x   0 maxx      (1000) research  (1001)       47 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/MANIFEST.in
+-rw-r--r--   0 maxx      (1000) research  (1001)     5209 2023-07-05 07:10:18.727990 LinuxRecycle-1.9.5/PKG-INFO
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1530 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/README.md
+drwxr-xr-x   0 maxx      (1000) research  (1001)        0 2023-07-05 07:10:18.727990 LinuxRecycle-1.9.5/linuxrecycle/
+-rw-r--r--   0 maxx      (1000) research  (1001)     2223 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/AutoRegularTask.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     4984 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/DB.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      520 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/__init__.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      591 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/argv.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2648 2023-07-05 06:50:50.000000 LinuxRecycle-1.9.5/linuxrecycle/auto_clear.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2163 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/config.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1489 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/main.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2958 2023-07-05 06:50:34.000000 LinuxRecycle-1.9.5/linuxrecycle/oper.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1332 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/printDB.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1211 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/recover.py
+-rw-r--r--   0 maxx      (1000) research  (1001)      642 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/setCrontab.py
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     2271 2023-02-03 08:11:03.000000 LinuxRecycle-1.9.5/linuxrecycle/trashInfo.py
+-rw-r--r--   0 maxx      (1000) research  (1001)       38 2023-07-05 07:10:18.728990 LinuxRecycle-1.9.5/setup.cfg
+-rwxr-xr-x   0 maxx      (1000) research  (1001)     1462 2023-07-05 07:10:11.000000 LinuxRecycle-1.9.5/setup.py
```

### Comparing `LinuxRecycle-1.9.4/LICENSE` & `LinuxRecycle-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/LinuxRecycle.egg-info/PKG-INFO` & `LinuxRecycle-1.9.5/LinuxRecycle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinuxRecycle
-Version: 1.9.4
+Version: 1.9.5
 Summary: A recycle system for linux
 Author: Xin-Xin Ma
 License: GPL
 Project-URL: Source, https://github.com/xxmawhu/LinuxRecycle
 License-File: LICENSE
 
 qnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbd
```

### Comparing `LinuxRecycle-1.9.4/LinuxRecycle.egg-info/SOURCES.txt` & `LinuxRecycle-1.9.5/LinuxRecycle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/PKG-INFO` & `LinuxRecycle-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinuxRecycle
-Version: 1.9.4
+Version: 1.9.5
 Summary: A recycle system for linux
 Author: Xin-Xin Ma
 License: GPL
 Project-URL: Source, https://github.com/xxmawhu/LinuxRecycle
 License-File: LICENSE
 
 qnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbdqnmbd
```

### Comparing `LinuxRecycle-1.9.4/README.md` & `LinuxRecycle-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/AutoRegularTask.py` & `LinuxRecycle-1.9.5/linuxrecycle/AutoRegularTask.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/DB.py` & `LinuxRecycle-1.9.5/linuxrecycle/DB.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/__init__.py` & `LinuxRecycle-1.9.5/linuxrecycle/__init__.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/argv.py` & `LinuxRecycle-1.9.5/linuxrecycle/argv.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/auto_clear.py` & `LinuxRecycle-1.9.5/linuxrecycle/auto_clear.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/config.py` & `LinuxRecycle-1.9.5/linuxrecycle/config.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/main.py` & `LinuxRecycle-1.9.5/linuxrecycle/main.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/oper.py` & `LinuxRecycle-1.9.5/linuxrecycle/oper.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/printDB.py` & `LinuxRecycle-1.9.5/linuxrecycle/printDB.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/recover.py` & `LinuxRecycle-1.9.5/linuxrecycle/recover.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/setCrontab.py` & `LinuxRecycle-1.9.5/linuxrecycle/setCrontab.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/linuxrecycle/trashInfo.py` & `LinuxRecycle-1.9.5/linuxrecycle/trashInfo.py`

 * *Files identical despite different names*

### Comparing `LinuxRecycle-1.9.4/setup.py` & `LinuxRecycle-1.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # ====================================================
 
 from setuptools import setup
 from setuptools import find_packages
 import sys
 import os
 
-m_version = '1.9.4'
+m_version = '1.9.5'
 
 if sys.argv[1] == "publish":
     os.system("python3 setup.py sdist")
     os.system("python3 setup.py bdist_wheel")
-    os.system("twine upload dist/*{}*  --username xxmawhu --password pip_xinxin@146382 --verbose".format(m_version))
+    os.system("twine upload dist/*{}*  --verbose".format(m_version))
 else:
     setup(
         name='LinuxRecycle',
         version=m_version,
         author='Xin-Xin Ma',
         description="A recycle system for linux",
         description_content_type="text/markdown",
```

