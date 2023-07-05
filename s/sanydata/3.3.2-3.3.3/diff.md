# Comparing `tmp/sanydata-3.3.2.tar.gz` & `tmp/sanydata-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanydata-3.3.2.tar", last modified: Tue Jun 20 08:31:04 2023, max compression
+gzip compressed data, was "sanydata-3.3.3.tar", last modified: Wed Jul  5 03:00:07 2023, max compression
```

## Comparing `sanydata-3.3.2.tar` & `sanydata-3.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.596533 sanydata-3.3.2/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-20 08:31:04.596272 sanydata-3.3.2/PKG-INFO
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.592195 sanydata-3.3.2/sanydata/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.2/sanydata/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)   120883 2023-06-20 08:30:08.000000 sanydata-3.3.2/sanydata/datatools.py
--rw-r--r--   0 thao       (501) staff       (20)   102791 2023-06-20 08:22:53.000000 sanydata-3.3.2/sanydata/model_data_message_pb2.py
--rw-r--r--   0 thao       (501) staff       (20)    22020 2023-06-20 08:22:53.000000 sanydata-3.3.2/sanydata/model_data_message_pb2_grpc.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.593492 sanydata-3.3.2/sanydata.egg-info/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-06-20 08:31:03.000000 sanydata-3.3.2/sanydata.egg-info/PKG-INFO
--rw-r--r--   0 thao       (501) staff       (20)      371 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/SOURCES.txt
--rw-r--r--   0 thao       (501) staff       (20)        1 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/dependency_links.txt
--rw-r--r--   0 thao       (501) staff       (20)      130 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/requires.txt
--rw-r--r--   0 thao       (501) staff       (20)       15 2023-06-20 08:31:04.000000 sanydata-3.3.2/sanydata.egg-info/top_level.txt
--rw-r--r--   0 thao       (501) staff       (20)       38 2023-06-20 08:31:04.596627 sanydata-3.3.2/setup.cfg
--rw-r--r--   0 thao       (501) staff       (20)      999 2023-06-20 08:26:47.000000 sanydata-3.3.2/setup.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-06-20 08:31:04.595485 sanydata-3.3.2/utils/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.2/utils/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.2/utils/cos_handler.py
--rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.2/utils/file_operation.py
--rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.2/utils/local_handler.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-07-05 03:00:07.752013 sanydata-3.3.3/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-07-05 03:00:07.751794 sanydata-3.3.3/PKG-INFO
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-07-05 03:00:07.747538 sanydata-3.3.3/sanydata/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.3/sanydata/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)   120883 2023-06-20 08:30:08.000000 sanydata-3.3.3/sanydata/datatools.py
+-rw-r--r--   0 thao       (501) staff       (20)   102791 2023-06-20 08:22:53.000000 sanydata-3.3.3/sanydata/model_data_message_pb2.py
+-rw-r--r--   0 thao       (501) staff       (20)    22020 2023-06-20 08:22:53.000000 sanydata-3.3.3/sanydata/model_data_message_pb2_grpc.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-07-05 03:00:07.749027 sanydata-3.3.3/sanydata.egg-info/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-07-05 03:00:07.000000 sanydata-3.3.3/sanydata.egg-info/PKG-INFO
+-rw-r--r--   0 thao       (501) staff       (20)      371 2023-07-05 03:00:07.000000 sanydata-3.3.3/sanydata.egg-info/SOURCES.txt
+-rw-r--r--   0 thao       (501) staff       (20)        1 2023-07-05 03:00:07.000000 sanydata-3.3.3/sanydata.egg-info/dependency_links.txt
+-rw-r--r--   0 thao       (501) staff       (20)      147 2023-07-05 03:00:07.000000 sanydata-3.3.3/sanydata.egg-info/requires.txt
+-rw-r--r--   0 thao       (501) staff       (20)       15 2023-07-05 03:00:07.000000 sanydata-3.3.3/sanydata.egg-info/top_level.txt
+-rw-r--r--   0 thao       (501) staff       (20)       38 2023-07-05 03:00:07.752093 sanydata-3.3.3/setup.cfg
+-rw-r--r--   0 thao       (501) staff       (20)     1019 2023-07-05 02:59:04.000000 sanydata-3.3.3/setup.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-07-05 03:00:07.751147 sanydata-3.3.3/utils/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.3/utils/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.3/utils/cos_handler.py
+-rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.3/utils/file_operation.py
+-rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.3/utils/local_handler.py
```

### Comparing `sanydata-3.3.2/sanydata/datatools.py` & `sanydata-3.3.3/sanydata/datatools.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.2/sanydata/model_data_message_pb2.py` & `sanydata-3.3.3/sanydata/model_data_message_pb2.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.2/sanydata/model_data_message_pb2_grpc.py` & `sanydata-3.3.3/sanydata/model_data_message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.2/setup.py` & `sanydata-3.3.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 import sys
 import importlib
 
 importlib.reload(sys)
 
 setup(
     name="sanydata",
-    version="3.3.2",
+    version="3.3.3",
     keywords=["pip", "sanydata", "thao"],
     description="get data and get wind farm information",
     long_description="get data and get wind farm information",
     license="MIT Licence",
 
     url="http://gitlab.sanywind.net/sanydata/sanydata",
     author="thao",
     author_email="thao92@126.com",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=['grpcio', 'grpcio-tools', 'gql', 'pandas', 'elasticsearch',
                       'requests', 'requests_toolbelt', 'cos-python-sdk-v5', 'pyarrow', 'hdfs',
-                      'python-logstash', 'sentry_sdk']
+                      'python-logstash', 'sentry_sdk', 'protobuf==3.19.0']
 )
```

### Comparing `sanydata-3.3.2/utils/cos_handler.py` & `sanydata-3.3.3/utils/cos_handler.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.2/utils/file_operation.py` & `sanydata-3.3.3/utils/file_operation.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.3.2/utils/local_handler.py` & `sanydata-3.3.3/utils/local_handler.py`

 * *Files identical despite different names*

