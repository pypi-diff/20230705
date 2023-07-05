# Comparing `tmp/hops-3.2.0.0.tar.gz` & `tmp/hops-3.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hops-3.2.0.0.tar", last modified: Thu Apr 13 09:39:39 2023, max compression
+gzip compressed data, was "dist/hops-3.3.0.0.tar", last modified: Wed Jul  5 13:07:22 2023, max compression
```

## Comparing `hops-3.2.0.0.tar` & `hops-3.3.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1795 2023-04-13 09:39:35.000000 hops-3.2.0.0/setup.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    14054 2023-04-13 09:39:35.000000 hops-3.2.0.0/README.rst
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       80 2023-04-13 09:39:39.000000 hops-3.2.0.0/setup.cfg
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1338 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/SOURCES.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        5 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/top_level.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/PKG-INFO
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      314 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/requires.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        1 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops.egg-info/dependency_links.txt
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-04-13 09:39:39.000000 hops-3.2.0.0/PKG-INFO
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3529 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/user.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17399 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/dataset.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3011 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/elasticsearch.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    26643 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/constants.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6851 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/kafka.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    31914 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/hdfs.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4608 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/pandas_helper.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6372 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/project.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5896 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/tensorboard.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1098 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/hive.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6902 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/numpy_helper.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7511 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/jobs.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    25975 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3549 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/devices.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/distribute/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      229 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation_client.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     8320 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5611 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5035 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/mirrored.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      245 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_client.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     9753 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/util/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/util/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    27081 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/util/experiment_utils.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5546 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/launcher.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/__init__.py
-drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:39.000000 hops-3.2.0.0/hops/experiment_impl/parallel/
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6171 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/random_search.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    22222 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/differential_evolution.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4463 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/experiment_impl/parallel/grid_search.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      169 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/__init__.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7717 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/tls.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17320 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/model.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    38651 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/serving.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      727 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/service_discovery.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      773 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/featurestore.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5313 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/secret.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      470 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/exceptions.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    20187 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/util.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5596 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/credentials_provider.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       24 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/version.py
--rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5732 2023-04-13 09:39:35.000000 hops-3.2.0.0/hops/xattr.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1795 2023-07-05 13:07:19.000000 hops-3.3.0.0/setup.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    14054 2023-07-05 13:07:19.000000 hops-3.3.0.0/README.rst
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       80 2023-07-05 13:07:22.000000 hops-3.3.0.0/setup.cfg
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1338 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        5 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/top_level.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/PKG-INFO
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      314 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/requires.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        1 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17016 2023-07-05 13:07:22.000000 hops-3.3.0.0/PKG-INFO
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3529 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/user.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17399 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/dataset.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3011 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/elasticsearch.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    26643 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/constants.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6851 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/kafka.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    31914 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/hdfs.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4608 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/pandas_helper.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6372 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/project.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5896 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/tensorboard.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     1098 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/hive.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6902 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/numpy_helper.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7511 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/jobs.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    25975 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     3549 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/devices.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops/experiment_impl/
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops/experiment_impl/distribute/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      229 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/mirrored_reservation_client.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     8320 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/mirrored_reservation.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5611 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/parameter_server.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5035 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/mirrored.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      245 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/parameter_server_client.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     9753 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops/experiment_impl/util/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/util/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    27081 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/util/experiment_utils.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5546 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/launcher.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/__init__.py
+drwxr-xr-x   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:22.000000 hops-3.3.0.0/hops/experiment_impl/parallel/
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)        0 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/parallel/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     6171 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/parallel/random_search.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    22222 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/parallel/differential_evolution.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     4463 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/experiment_impl/parallel/grid_search.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      169 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/__init__.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     7948 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/tls.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    17320 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/model.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    38651 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/serving.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      727 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/service_discovery.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      773 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/featurestore.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5313 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/secret.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)      470 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/exceptions.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)    21667 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/util.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5596 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/credentials_provider.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)       24 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/version.py
+-rw-r--r--   0 jenkinsmaster  (1006) jenkinsmaster  (1006)     5732 2023-07-05 13:07:19.000000 hops-3.3.0.0/hops/xattr.py
```

### Comparing `hops-3.2.0.0/setup.py` & `hops-3.3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/README.rst` & `hops-3.3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops.egg-info/SOURCES.txt` & `hops-3.3.0.0/hops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops.egg-info/PKG-INFO` & `hops-3.3.0.0/hops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hops
-Version: 3.2.0.0
+Version: 3.3.0.0
 Summary: Client library for interacting with Hopsworks, a full-stack platform for scale-out data science.
 Home-page: https://github.com/logicalclocks/hops-util-py
 Author: Robin Andersson
 Author-email: robin.eric.andersson@gmail.com
 License: Apache License 2.0
-Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.2.0.0.tar.gz
+Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.3.0.0.tar.gz
 Description: ============
         hops-util-py
         ============
         
         |Downloads| |PypiStatus| |PythonVersions|
         
         `hops-util-py` is a helper library for Hops that facilitates development by hiding the complexity of running applications, discovering services and interacting with HopsFS.
```

### Comparing `hops-3.2.0.0/PKG-INFO` & `hops-3.3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hops
-Version: 3.2.0.0
+Version: 3.3.0.0
 Summary: Client library for interacting with Hopsworks, a full-stack platform for scale-out data science.
 Home-page: https://github.com/logicalclocks/hops-util-py
 Author: Robin Andersson
 Author-email: robin.eric.andersson@gmail.com
 License: Apache License 2.0
-Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.2.0.0.tar.gz
+Download-URL: http://snurran.sics.se/hops/hops-util-py/hops-3.3.0.0.tar.gz
 Description: ============
         hops-util-py
         ============
         
         |Downloads| |PypiStatus| |PythonVersions|
         
         `hops-util-py` is a helper library for Hops that facilitates development by hiding the complexity of running applications, discovering services and interacting with HopsFS.
```

### Comparing `hops-3.2.0.0/hops/user.py` & `hops-3.3.0.0/hops/user.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/dataset.py` & `hops-3.3.0.0/hops/dataset.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/elasticsearch.py` & `hops-3.3.0.0/hops/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/constants.py` & `hops-3.3.0.0/hops/constants.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/kafka.py` & `hops-3.3.0.0/hops/kafka.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/hdfs.py` & `hops-3.3.0.0/hops/hdfs.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/pandas_helper.py` & `hops-3.3.0.0/hops/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/project.py` & `hops-3.3.0.0/hops/project.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/tensorboard.py` & `hops-3.3.0.0/hops/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/hive.py` & `hops-3.3.0.0/hops/hive.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/numpy_helper.py` & `hops-3.3.0.0/hops/numpy_helper.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/jobs.py` & `hops-3.3.0.0/hops/jobs.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment.py` & `hops-3.3.0.0/hops/experiment.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/devices.py` & `hops-3.3.0.0/hops/devices.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/distribute/mirrored_reservation.py` & `hops-3.3.0.0/hops/experiment_impl/distribute/mirrored_reservation.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server.py` & `hops-3.3.0.0/hops/experiment_impl/distribute/parameter_server.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/distribute/mirrored.py` & `hops-3.3.0.0/hops/experiment_impl/distribute/mirrored.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py` & `hops-3.3.0.0/hops/experiment_impl/distribute/parameter_server_reservation.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/util/experiment_utils.py` & `hops-3.3.0.0/hops/experiment_impl/util/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/launcher.py` & `hops-3.3.0.0/hops/experiment_impl/launcher.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/parallel/random_search.py` & `hops-3.3.0.0/hops/experiment_impl/parallel/random_search.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/parallel/differential_evolution.py` & `hops-3.3.0.0/hops/experiment_impl/parallel/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/experiment_impl/parallel/grid_search.py` & `hops-3.3.0.0/hops/experiment_impl/parallel/grid_search.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/tls.py` & `hops-3.3.0.0/hops/tls.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import string
 import base64
 import textwrap
 from hops import constants
 import os
 from pathlib import Path
+import tempfile
 
 try:
     import jks
 except:
     pass
 
 
@@ -21,15 +22,15 @@
 
     Returns:
         keystore path  
     """
     k_certificate = Path(constants.SSL_CONFIG.K_CERTIFICATE_CONFIG)
     if k_certificate.exists():
         return k_certificate
-    else: 
+    else:
         username = os.environ['HADOOP_USER_NAME']
         material_directory = Path(os.environ['MATERIAL_DIRECTORY'])
         return material_directory.joinpath(username + constants.SSL_CONFIG.KEYSTORE_SUFFIX)
 
 
 def get_key_store():
     return str(_get_key_store_path())
@@ -41,15 +42,15 @@
 
     Returns:
          truststore location 
     """
     t_certificate = Path(constants.SSL_CONFIG.T_CERTIFICATE_CONFIG)
     if t_certificate.exists():
         return str(t_certificate)
-    else: 
+    else:
         username = os.environ['HADOOP_USER_NAME']
         material_directory = Path(os.environ['MATERIAL_DIRECTORY'])
         return str(material_directory.joinpath(username + constants.SSL_CONFIG.TRUSTSTORE_SUFFIX))
 
 
 def get_trust_store():
     return str(_get_trust_store_path())
@@ -75,15 +76,15 @@
 def get_key_store_cert():
     """
     Get keystore certificate from local container
 
     Returns:
         Certificate password
     """
-    cert_path = _get_key_store_path() 
+    cert_path = _get_key_store_path()
 
     if not cert_path.exists():
         raise AssertionError('k_certificate is not present in directory: {}'.format(str(cert_path)))
 
     # read as bytes, don't try to use utf-8 encoding
     with cert_path.open("rb") as f:
         key_store_cert = f.read()
@@ -161,15 +162,16 @@
 
     # Convert CA Certificates into PEM format and append to string
     for alias, c in ks.certs.items():
         ca_certs = ca_certs + _bytes_to_pem_str(c.cert, "CERTIFICATE")
     return private_keys_certs, private_keys, ca_certs
 
 
-def _write_pem(jks_key_store_path, jks_trust_store_path, keystore_pw, client_key_cert_path, client_key_path, ca_cert_path):
+def _write_pem(jks_key_store_path, jks_trust_store_path, keystore_pw, client_key_cert_path, client_key_path,
+               ca_cert_path):
     """
     Converts the JKS keystore, JKS truststore, and the root ca.pem
     client certificate, client key, and ca certificate
 
     Args:
     :jks_key_store_path: path to the JKS keystore
     :jks_trust_store_path: path to the JKS truststore
@@ -192,56 +194,65 @@
     """
     Get location of client certificate (PEM format) for the private key signed by trusted CA
     used for 2-way TLS authentication, for example with Kafka cluster
 
     Returns:
         string path to client certificate in PEM format
     """
-    certificate_path = Path(constants.SSL_CONFIG.PEM_CLIENT_CERTIFICATE_CONFIG)
-    if not certificate_path.exists(): 
+    certificate_path = pems_dir(constants.SSL_CONFIG.PEM_CLIENT_CERTIFICATE_CONFIG)
+    if not certificate_path.exists():
         _write_pems()
     return str(certificate_path)
 
 
 def get_client_key_location():
     """
     Get location of client private key (PEM format)
     used for for 2-way TLS authentication, for example with Kafka cluster
 
     Returns:
         string path to client private key in PEM format
     """
     # Convert JKS to PEMs if they don't exists already
-    key_path = Path(constants.SSL_CONFIG.PEM_CLIENT_KEY_CONFIG)
+    key_path = pems_dir(constants.SSL_CONFIG.PEM_CLIENT_KEY_CONFIG)
     if not key_path.exists():
         _write_pems()
     return str(key_path)
 
 
 def get_ca_chain_location():
     """
     Get location of chain of CA certificates (PEM format) that are required to validate the
     private key certificate of the client
     used for 2-way TLS authentication, for example with Kafka cluster
 
     Returns:
          string path to ca chain of certificate
     """
-    ca_chain_path = Path(constants.SSL_CONFIG.PEM_CA_CHAIN_CERTIFICATE_CONFIG) 
+    ca_chain_path = pems_dir(constants.SSL_CONFIG.PEM_CA_CHAIN_CERTIFICATE_CONFIG)
     if not ca_chain_path.exists():
         _write_pems()
     return str(ca_chain_path)
 
 
+def pems_dir(pem):
+    """
+    Get location of a pem file
+
+    Returns:
+         path to a pem file
+    """
+    pem_dir = Path(tempfile.gettempdir())
+    return pem_dir.joinpath(pem)
+
+
 def _write_pems():
     """
     Converts JKS keystore file into PEM to be compatible with Python libraries
     """
-    t_jks_path = get_trust_store() 
-    k_jks_path = get_key_store() 
-
-    client_certificate_path = Path(constants.SSL_CONFIG.PEM_CLIENT_CERTIFICATE_CONFIG)
-    client_key_path = Path(constants.SSL_CONFIG.PEM_CLIENT_KEY_CONFIG)
-    ca_chain_path = Path(constants.SSL_CONFIG.PEM_CA_CHAIN_CERTIFICATE_CONFIG)
+    t_jks_path = get_trust_store()
+    k_jks_path = get_key_store()
+    client_certificate_path = pems_dir(constants.SSL_CONFIG.PEM_CLIENT_CERTIFICATE_CONFIG)
+    client_key_path = pems_dir(constants.SSL_CONFIG.PEM_CLIENT_KEY_CONFIG)
+    ca_chain_path = pems_dir(constants.SSL_CONFIG.PEM_CA_CHAIN_CERTIFICATE_CONFIG)
 
     _write_pem(k_jks_path, t_jks_path, get_key_store_pwd(), client_certificate_path, client_key_path, ca_chain_path)
-
```

### Comparing `hops-3.2.0.0/hops/model.py` & `hops-3.3.0.0/hops/model.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/serving.py` & `hops-3.3.0.0/hops/serving.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/service_discovery.py` & `hops-3.3.0.0/hops/service_discovery.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/featurestore.py` & `hops-3.3.0.0/hops/featurestore.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/secret.py` & `hops-3.3.0.0/hops/secret.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/util.py` & `hops-3.3.0.0/hops/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from hops.exceptions import UnkownSecretStorageError, APIKeyFileNotFound
 import base64
 from socket import socket
 from json.decoder import JSONDecodeError
 from hops.exceptions import RestAPIError
 from hops.exceptions import APIKeyFileNotFound
 
+import logging
+from notebook.notebookapp import list_running_servers
 
 verify = None
 #! Needed for hops library backwards compatability
 try:
     import requests
     import urllib3
     urllib3.disable_warnings(urllib3.exceptions.SecurityWarning)
@@ -531,14 +533,45 @@
         :path (str): path where file is saved, including file name. e.g. /path/key-store.jks
     """
 
     with open(path, 'wb') as f:
         cert_b64 = base64.b64decode(b64_string)
         f.write(cert_b64)
 
+def notebook_post_save(relative_path):
+    """attach xattr after saving a notebook"""
+    logging.info("Attaching notebook configuration to file " + relative_path)
+    kernel_id = get_notebook_kernel_id(relative_path)
+    if kernel_id != "":
+        logging.info("Kernel id for {} is {}".format(relative_path, kernel_id))
+        try:
+            attach_jupyter_configuration_to_notebook(kernel_id)
+            logging.info("Notebook configuration successfully attached for file {} attached".format(relative_path))
+        except Exception as e:
+            logging.error("Failed to attach notebook configuration: " + str(e))
+    else:
+        logging.error("No kernel id found for notebook " + relative_path)
+    return
+
+def get_notebook_kernel_id(path):
+    """
+    Return the kernel_id of the jupyter notebook if it was opened or run.
+    """
+    if path != "":
+        for server in list_running_servers():
+            url = server['url'] + 'api/sessions?token=' + server.get('token', '')
+            req = requests.Request('GET', url)
+            prepped = session.prepare_request(req)
+            response = session.send(prepped, verify=verify, stream=False)
+            if response.ok:
+                for notebook_session in json.loads(response.content):
+                    if notebook_session['notebook']['path'] == path:
+                        return notebook_session['kernel']['id']
+    return ""
+
 def attach_jupyter_configuration_to_notebook(kernel_id):
     method = constants.HTTP_CONFIG.HTTP_PUT
     resource_url = constants.DELIMITERS.SLASH_DELIMITER + \
                    constants.REST_CONFIG.HOPSWORKS_REST_RESOURCE + constants.DELIMITERS.SLASH_DELIMITER + \
                    "project" + constants.DELIMITERS.SLASH_DELIMITER + os.environ["HOPSWORKS_PROJECT_ID"] + \
                    constants.DELIMITERS.SLASH_DELIMITER + "jupyter/attachConfiguration" + \
                    constants.DELIMITERS.SLASH_DELIMITER + os.environ["HADOOP_USER_NAME"] + \
```

### Comparing `hops-3.2.0.0/hops/credentials_provider.py` & `hops-3.3.0.0/hops/credentials_provider.py`

 * *Files identical despite different names*

### Comparing `hops-3.2.0.0/hops/xattr.py` & `hops-3.3.0.0/hops/xattr.py`

 * *Files identical despite different names*

