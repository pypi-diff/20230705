# Comparing `tmp/tarn-0.8.0.tar.gz` & `tmp/tarn-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.8.0.tar", last modified: Sat Jun 24 14:47:56 2023, max compression
+gzip compressed data, was "tarn-0.9.0.tar", last modified: Wed Jul  5 00:25:25 2023, max compression
```

## Comparing `tarn-0.8.0.tar` & `tarn-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-24 14:47:54.000000 tarn-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-24 14:47:54.000000 tarn-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-24 14:47:56.973829 tarn-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-24 14:47:54.000000 tarn-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-24 14:47:54.000000 tarn-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 14:47:54.000000 tarn-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:47:56.973829 tarn-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-24 14:47:54.000000 tarn-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.973829 tarn-0.8.0/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-24 14:47:54.000000 tarn-0.8.0/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:47:56.969829 tarn-0.8.0/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-24 14:47:56.000000 tarn-0.8.0/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.652315 tarn-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-05 00:25:22.000000 tarn-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 00:25:22.000000 tarn-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 00:25:25.652315 tarn-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 00:25:22.000000 tarn-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-05 00:25:22.000000 tarn-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 00:25:22.000000 tarn-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:25:25.652315 tarn-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 00:25:22.000000 tarn-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.640314 tarn-0.9.0/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.644314 tarn-0.9.0/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.644314 tarn-0.9.0/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.648315 tarn-0.9.0/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.648315 tarn-0.9.0/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.648315 tarn-0.9.0/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.648315 tarn-0.9.0/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.648315 tarn-0.9.0/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-05 00:25:22.000000 tarn-0.9.0/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:25:25.644314 tarn-0.9.0/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 00:25:25.000000 tarn-0.9.0/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 00:25:25.000000 tarn-0.9.0/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:25:25.000000 tarn-0.9.0/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-05 00:25:25.000000 tarn-0.9.0/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 00:25:25.000000 tarn-0.9.0/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.8.0/LICENSE` & `tarn-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/PKG-INFO` & `tarn-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.8.0
+Version: 0.9.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A hashmap-based storage on local and remote disks
 
 # Install
```

### Comparing `tarn-0.8.0/README.md` & `tarn-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/pyproject.toml` & `tarn-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = 'tarn'
 dynamic = ['version', 'dependencies']
 description = 'A hashmap-based storage on local and remote disks'
 readme = 'README.md'
-requires-python = '>=3.6'
+requires-python = '>=3.7'
 license = { file = 'LICENSE' }
 keywords = ['storage', 'cache', 'invalidation']
 authors = [
-    { name = 'Max', email = 'max@ira-labs.com' }
+    { name = 'Max', email = 'max@ira-labs.com' },
+    { name = 'Talgat', email = 't.saparov@ira-labs.com' },
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
@@ -43,18 +44,15 @@
 # E203: spaces around complex variables in slices are pep-right
 # F401: unused imports in __init__.py-s
 # I251: allow absolute imports in upper files
 # B019: @lru_cache for static methods is fine
 # B008: calling the function as default value is just part of the typer's interface
 # C408: for identifier-like fields dict(x=y) is just more concise
 ignore = ["W503", "E203", "B019", "B028", "C408"]
-per-file-ignores = [
-    "**/__init__.py:F401",
-    "tests/*:I251",
-]
+per-file-ignores = ["**/__init__.py:F401", "tests/*:I251"]
 max-line-length = 120
 banned-modules = "tarn.* = Use relative imports"
 
 [tool.isort]
 line_length = 120
 profile = 'black'
 combine_as_imports = true
```

### Comparing `tarn-0.8.0/setup.py` & `tarn-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import runpy
 from pathlib import Path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 classifiers = [
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
@@ -35,9 +35,9 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/neuro-ml/tarn',
     download_url='https://github.com/neuro-ml/tarn/archive/v%s.tar.gz' % version,
     keywords=['storage', 'cache', 'invalidation'],
     classifiers=classifiers,
     install_requires=requirements,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```

### Comparing `tarn-0.8.0/tarn/cache/storage.py` & `tarn-0.9.0/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/compat.py` & `tarn-0.9.0/tarn/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,70 @@
-import errno
+import filecmp
 import os
-import platform
-import shutil
-import stat
+from contextlib import contextmanager
+from io import BytesIO
 from pathlib import Path
-from tempfile import SpooledTemporaryFile as _SpooledTemporaryFile
-from typing import Any, Union
+from typing import BinaryIO, Union
+
+from .compat import set_path_attrs
+from .interface import Key, Value  # noqa
+
+# TODO: legacy
+PathLike = Union[Path, str]
+
+
+def to_read_only(path: Path, permissions, group):
+    adjust_permissions(path, permissions, group, read_only=True)
+
+
+def adjust_permissions(path: Path, permissions, group, read_only: bool = False):
+    if read_only:
+        permissions = 0o444 & permissions
+
+    set_path_attrs(path, permissions, group)
 
-try:
-    from typing import Protocol
-except ImportError:
-    Protocol = object
-try:
-    from gzip import BadGzipFile
-except ImportError:
-    BadGzipFile = OSError
-try:
-    from typing import Self
-except ImportError:
-    Self = Any
-
-try:
-    from mypy_boto3_s3 import S3Client
-except ImportError:
-    S3Client = Any
-
-from .interface import PathOrStr
-
-if platform.system() == 'Windows':
-    def rmtree(path, ignore_errors=False):
-        # source: https://docs.python.org/3.10/library/shutil.html#rmtree-example
-        def remove_readonly(func, p, _):
-            os.chmod(p, stat.S_IWRITE)
-            func(p)
-
-        shutil.rmtree(path, ignore_errors=ignore_errors, onerror=remove_readonly)
-
-
-    def get_path_group(path: PathOrStr) -> Union[int, None]:
-        pass
-
-
-    def remove_file(path: PathOrStr):
-        os.chmod(path, stat.S_IWRITE)
-        os.remove(path)
-
-else:
-    rmtree = shutil.rmtree
-    remove_file = os.remove
-
-
-    def get_path_group(path: PathOrStr) -> Union[int, None]:
-        return Path(path).stat().st_gid
-
-if hasattr(_SpooledTemporaryFile, 'seekable'):
-    SpooledTemporaryFile = _SpooledTemporaryFile
-else:
-    class SpooledTemporaryFile(_SpooledTemporaryFile):
-        def seekable(self) -> bool:
-            return True
 
+def get_size(file: Path) -> int:
+    return file.stat().st_size
 
-def set_path_attrs(path: Path, permissions: Union[int, None] = None, group: Union[str, int, None] = None):
-    if permissions is not None:
-        path.chmod(permissions)
-    if group is not None:
-        shutil.chown(path, group=group)
-
-
-def copy_file(source: PathOrStr, destination: PathOrStr):
-    # in Python>=3.8 the sendfile call is used, which apparently may fail
-    try:
-        shutil.copyfile(source, destination)
-    except OSError as e:
-        # BlockingIOError -> fallback to slow copy
-        if e.errno != errno.EWOULDBLOCK:
-            raise
-
-        with open(source, 'rb') as src, open(destination, 'wb') as dst:
-            shutil.copyfileobj(src, dst)
 
+def mkdir(path: Path, permissions: Union[int, None], group: Union[str, int, None],
+          parents: bool = False, exist_ok: bool = False):
+    path.mkdir(parents=parents, exist_ok=exist_ok)
+    set_path_attrs(path, permissions, group)
+
+
+def create_folders(path: Path, permissions, group):
+    if not path.exists():
+        create_folders(path.parent, permissions, group)
+        mkdir(path, permissions, group, exist_ok=True)
+
+
+# TODO: need functions that return bool
+
+def match_files(first: Path, second: Path):
+    if not filecmp.cmp(first, second, shallow=False):
+        raise ValueError(f'Files do not match: {first} vs {second}')
+
+
+def match_buffers(first: BinaryIO, second: BinaryIO, context: str):
+    bufsize = 8 * 1024
+    while True:
+        b1 = first.read(bufsize)
+        b2 = second.read(bufsize)
+        if b1 != b2:
+            raise ValueError(f'Buffers do not match: {context}')
+        if not b1:
+            return True
 
-class HashAlgorithm(Protocol):
-    digest_size: int
 
-    def update(self, chunk: bytes) -> None:
-        pass
+@contextmanager
+def value_to_buffer(value: Union[Value, bytes]):
+    if isinstance(value, bytes):
+        yield BytesIO(value)
+
+    elif isinstance(value, (str, os.PathLike)):
+        with open(value, 'rb') as file:
+            yield file
 
-    def digest(self) -> bytes:
-        pass
+    else:
+        yield value
```

### Comparing `tarn-0.8.0/tarn/config.py` & `tarn-0.9.0/tarn/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 import hashlib
 import io
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, Sequence, Tuple, Union
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import humanfriendly
-from pydantic import BaseModel, Extra, root_validator, validator
+from pydantic import Field
 from yaml import safe_dump, safe_load
 
-from .compat import get_path_group
+from .compat import field_validator, get_path_group, model_validator, model_validate, model_dump, NoExtra
 from .interface import PathOrStr
 from .tools import DummyLabels, DummyLocker, DummySize, DummyUsage, LabelsStorage, Locker, SizeTracker, UsageTracker
 from .utils import mkdir
 
 CONFIG_NAME = 'config.yml'
 
 
-class _NoExtra(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-
-class HashConfig(_NoExtra):
+class HashConfig(NoExtra):
     name: str
     kwargs: Dict[str, Any] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode='before')
     def normalize_kwargs(cls, values):
-        alias = 'kwargs'
-        required = {field.alias for field in cls.__fields__.values() if field.alias != alias}
-
         kwargs = {}
         for field_name in list(values):
-            if field_name not in required:
+            if field_name not in ('name', 'kwargs'):
                 kwargs[field_name] = values.pop(field_name)
 
-        values[alias] = kwargs
+        values['kwargs'] = kwargs
         return values
 
+    def model_dump(self, **kwargs):
+        real = super().model_dump(**kwargs)
+        kwargs = real.pop('kwargs')
+        real.update(kwargs)
+        return real
+
     def dict(self, **kwargs):
         real = super().dict(**kwargs)
         kwargs = real.pop('kwargs')
         real.update(kwargs)
         return real
 
     def build(self):
         cls = getattr(hashlib, self.name)
         if self.kwargs:
             cls = partial(cls, **self.kwargs)
         return cls
 
 
-class ToolConfig(_NoExtra):
+class ToolConfig(NoExtra):
     name: str
     args: Tuple = ()
-    kwargs: Dict[str, Any] = None
+    kwargs: Optional[Dict[str, Any]] = None
 
-    @validator('kwargs', always=True)
+    @field_validator('kwargs', always=True)
     def normalize_kwargs(cls, v):
         if v is None:
             return {}
         return v
 
 
-class StorageConfig(_NoExtra):
+class StorageConfig(NoExtra):
     hash: HashConfig
-    levels: Sequence[int] = None
-    locker: ToolConfig = None
-    size: ToolConfig = None
-    usage: ToolConfig = None
-    labels: ToolConfig = None
+    levels: Optional[Sequence[int]] = Field(None, validate_default=True)
+    locker: Optional[ToolConfig] = None
+    size: Optional[ToolConfig] = None
+    usage: Optional[ToolConfig] = None
+    labels: Optional[ToolConfig] = None
     free_disk_size: Union[int, str] = 0
-    max_size: Union[int, str] = None
-    version: str = None
+    max_size: Optional[Union[int, str]] = None
 
     @staticmethod
     def _make(base, dummy, config, *args):
         if config is None:
             return dummy(*args)
         cls = find_subclass(base, config.name)
         return cls(*args, *config.args, **config.kwargs)
@@ -89,44 +86,46 @@
 
     def make_usage(self, root: Path) -> UsageTracker:
         return self._make(UsageTracker, DummyUsage, self.usage, root)
 
     def make_labels(self, root: Path) -> LabelsStorage:
         return self._make(LabelsStorage, DummyLabels, self.labels, root)
 
-    @validator('free_disk_size', 'max_size')
+    @field_validator('free_disk_size', 'max_size')
     def to_size(cls, v):
         return parse_size(v)
 
-    @validator('hash', 'locker', 'usage', 'labels', pre=True)
+    @field_validator('hash', 'locker', 'usage', 'labels', mode='before')
     def normalize_tools(cls, v):
         if isinstance(v, str):
             v = {'name': v}
         return v
 
-    @validator('levels', always=True)
+    @field_validator('levels', always=True)
     def normalize_levels(cls, v, values):
         # default levels are [1, n - 1]
+        if not isinstance(values, dict):
+            values = values.data
         if v is None:
             v = 1, values['hash'].build()().digest_size - 1
         return v
 
 
 def root_params(root: Path):
     stat = root.stat()
     return stat.st_mode & 0o777, get_path_group(root)
 
 
 def load_config_buffer(data: str) -> StorageConfig:
-    return StorageConfig.parse_obj(safe_load(io.StringIO(data)))
+    return model_validate(StorageConfig, safe_load(io.StringIO(data)))
 
 
 def load_config(root: PathOrStr) -> StorageConfig:
     with open(Path(root) / CONFIG_NAME) as file:
-        return StorageConfig.parse_obj(safe_load(file))
+        return model_validate(StorageConfig, safe_load(file))
 
 
 def parse_size(x):
     if isinstance(x, int):
         return x
     if isinstance(x, str):
         return humanfriendly.parse_size(x)
@@ -144,8 +143,8 @@
 
 def init_storage(config: StorageConfig, root: PathOrStr, *,
                  permissions: Union[int, None] = None, group: Union[str, int, None] = None, exist_ok: bool = False):
     root = Path(root)
     mkdir(root, permissions, group, parents=True, exist_ok=exist_ok)
 
     with open(root / CONFIG_NAME, 'w') as file:
-        safe_dump(config.dict(), file)
+        safe_dump(model_dump(config), file)
```

### Comparing `tarn-0.8.0/tarn/digest.py` & `tarn-0.9.0/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/interface.py` & `tarn-0.9.0/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/local/storage.py` & `tarn-0.9.0/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/disk_dict.py` & `tarn-0.9.0/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/fanout.py` & `tarn-0.9.0/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/interface.py` & `tarn-0.9.0/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/levels.py` & `tarn-0.9.0/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/nginx.py` & `tarn-0.9.0/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/location/scp.py` & `tarn-0.9.0/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/pickler/compat.py` & `tarn-0.9.0/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/pickler/interface.py` & `tarn-0.9.0/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/pool/hash_key.py` & `tarn-0.9.0/tarn/pool/hash_key.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from io import BytesIO
 import os
 from contextlib import contextmanager
+from io import BytesIO
 from pathlib import Path
 from typing import Any, Callable, ContextManager, Iterable, Optional, Sequence, Tuple, Type, Union
 
 from ..compat import HashAlgorithm
 from ..digest import digest_value
 from ..exceptions import ReadError, WriteError
 from ..interface import Key, Keys, MaybeLabels, MaybeValue, PathOrStr, Value
```

### Comparing `tarn-0.8.0/tarn/pool/pickle_key.py` & `tarn-0.9.0/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/serializers.py` & `tarn-0.9.0/tarn/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-
 import inspect
 import json
-from pathlib import Path
 import pickle
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import suppress
 from functools import partial
 from gzip import GzipFile
 from pathlib import Path
```

### Comparing `tarn-0.8.0/tarn/tools/labels.py` & `tarn-0.9.0/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/tools/locker.py` & `tarn-0.9.0/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/tools/size.py` & `tarn-0.9.0/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn/tools/usage.py` & `tarn-0.9.0/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.8.0/tarn.egg-info/PKG-INFO` & `tarn-0.9.0/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.8.0
+Version: 0.9.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 A hashmap-based storage on local and remote disks
 
 # Install
```

### Comparing `tarn-0.8.0/tarn.egg-info/SOURCES.txt` & `tarn-0.9.0/tarn.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 tarn/local/storage.py
 tarn/location/__init__.py
 tarn/location/disk_dict.py
 tarn/location/fanout.py
 tarn/location/interface.py
 tarn/location/levels.py
 tarn/location/nginx.py
+tarn/location/redis.py
 tarn/location/s3.py
 tarn/location/scp.py
 tarn/pickler/__init__.py
 tarn/pickler/compat.py
 tarn/pickler/interface.py
 tarn/pool/__init__.py
 tarn/pool/hash_key.py
```

