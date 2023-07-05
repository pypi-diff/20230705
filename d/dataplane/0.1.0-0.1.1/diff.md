# Comparing `tmp/dataplane-0.1.0.tar.gz` & `tmp/dataplane-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataplane-0.1.0.tar", last modified: Thu Mar 16 14:14:22 2023, max compression
+gzip compressed data, was "dataplane-0.1.1.tar", last modified: Wed Jul  5 20:20:23 2023, max compression
```

## Comparing `dataplane-0.1.0.tar` & `dataplane-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.674309 dataplane-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-16 14:13:41.000000 dataplane-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-16 14:14:22.674309 dataplane-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-16 14:13:41.000000 dataplane-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-16 14:14:04.000000 dataplane-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 14:14:22.674309 dataplane-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.666309 dataplane-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.666309 dataplane-0.1.0/src/dataplane/DataStorage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/DataStorage/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/DataStorage/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/DataStorage/s3/s3_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/DataStorage/s3/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/DataStorage/s3/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/DataStorage/s3/test_s3_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/Microsoft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/Microsoft/Teams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Teams/test_webhook_send.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/Teams/webhook_send.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/Microsoft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane/pipelinerun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.674309 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-16 14:13:41.000000 dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_s3_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:14:22.670309 dataplane-0.1.0/src/dataplane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-16 14:14:22.000000 dataplane-0.1.0/src/dataplane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-16 14:14:22.000000 dataplane-0.1.0/src/dataplane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:14:22.000000 dataplane-0.1.0/src/dataplane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 14:14:22.000000 dataplane-0.1.0/src/dataplane.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 20:19:36.000000 dataplane-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-05 20:20:23.345730 dataplane-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-05 20:19:36.000000 dataplane-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-05 20:20:04.000000 dataplane-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:20:23.345730 dataplane-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/dataplane/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/dataplane/DataStorage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/DataStorage/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/Teams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/test_webhook_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/webhook_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/pipelinerun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_s3_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/top_level.txt
```

### Comparing `dataplane-0.1.0/LICENSE` & `dataplane-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/PKG-INFO` & `dataplane-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataplane
-Version: 0.1.0
+Version: 0.1.1
 Summary: The data engineering library to build robust, reliable and on time data pipelines in Python.
 Author: Saul Frank, Dataplane, Inc.
 Project-URL: Homepage, https://dataplane.app
 Project-URL: Github, https://github.com/dataplane-app/dataplane-python-package
 Project-URL: Issues, https://github.com/dataplane-app/dataplane/issues
 Project-URL: Feedback, https://github.com/dataplane-app/dataplane/discussions
 Keywords: workflow,data-science,data,airflow,etl,dataplane,data-engineering,data-pipelines,datawarehouse,automation,data-analysis,scheduler
```

### Comparing `dataplane-0.1.0/README.md` & `dataplane-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/pyproject.toml` & `dataplane-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0", "redis>=1.0.0", "pandas>1.0.0", "requests>1.0.0", "boto3>1.0.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataplane"
-version = "0.1.0"
+version = "0.1.1"
 description = "The data engineering library to build robust, reliable and on time data pipelines in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: BSD License", "Operating System :: OS Independent",]
 keywords = [ "workflow", "data-science", "data", "airflow", "etl", "dataplane", "data-engineering", "data-pipelines", "datawarehouse", "automation", "data-analysis", "scheduler",]
 [[project.authors]]
 name = "Saul Frank"
```

### Comparing `dataplane-0.1.0/src/dataplane/DataStorage/s3/s3_download.py` & `dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 S3Client: Client for s3
 S3FilePath: /tmp/source.xlsx (needs UploadMethod="File")
 LocalFilePath: /General/hello.xlxs (where download method is File)
 Download Method: File or Object
 FilePath: /General/hello.xlxs
 """
 
-def s3_download(S3Client, Bucket,  S3FilePath, DownloadMethod="Object", LocalFilePath=""):
+def s3_download(S3Client, Bucket,  S3FilePath, DownloadMethod="Object", LocalFilePath="", ChecksumMode=''):
     
     from datetime import datetime
     from io import BytesIO
 
     # Start the timer
     start = datetime.now()
     
@@ -25,11 +25,14 @@
         with open(LocalFilePath, 'wb') as data:
             S3Client.download_fileobj(Bucket=Bucket, Key=S3FilePath, Fileobj=data)
 
         duration = datetime.now() - start
         return {"result":"OK", "duration": str(duration), "FilePath": LocalFilePath} 
 
     # Download S3 file content to object
-    objectGet = S3Client.get_object(Bucket=Bucket, Key=S3FilePath, ChecksumMode='ENABLED')["Body"].read()
+    if ChecksumMode=="ENABLED":
+        objectGet = S3Client.get_object(Bucket=Bucket, Key=S3FilePath, ChecksumMode='ENABLED')["Body"].read()
+    else:
+        objectGet = S3Client.get_object(Bucket=Bucket, Key=S3FilePath)["Body"].read()
     
     duration = datetime.now() - start
     return {"result":"OK", "duration": str(duration), "content": objectGet}
```

### Comparing `dataplane-0.1.0/src/dataplane/DataStorage/s3/s3_upload.py` & `dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_upload.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/DataStorage/s3/test_s3.py` & `dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/DataStorage/s3/test_s3_object.py` & `dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3_object.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Teams/test_webhook_send.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Teams/test_webhook_send.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/Microsoft/Teams/webhook_send.py` & `dataplane-0.1.1/src/dataplane/Microsoft/Teams/webhook_send.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/__init__.py` & `dataplane-0.1.1/src/dataplane/__init__.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/redis_store.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/redis_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_redis.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_redis.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane/pipelinerun/data_persist/test_s3_store.py` & `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_s3_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.0/src/dataplane.egg-info/PKG-INFO` & `dataplane-0.1.1/src/dataplane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataplane
-Version: 0.1.0
+Version: 0.1.1
 Summary: The data engineering library to build robust, reliable and on time data pipelines in Python.
 Author: Saul Frank, Dataplane, Inc.
 Project-URL: Homepage, https://dataplane.app
 Project-URL: Github, https://github.com/dataplane-app/dataplane-python-package
 Project-URL: Issues, https://github.com/dataplane-app/dataplane/issues
 Project-URL: Feedback, https://github.com/dataplane-app/dataplane/discussions
 Keywords: workflow,data-science,data,airflow,etl,dataplane,data-engineering,data-pipelines,datawarehouse,automation,data-analysis,scheduler
```

### Comparing `dataplane-0.1.0/src/dataplane.egg-info/SOURCES.txt` & `dataplane-0.1.1/src/dataplane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

