# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230705193219.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar", last modified: Thu Jun  1 15:36:46 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230705193219.tar", last modified: Wed Jul  5 19:33:01 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-01 15:36:44.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11349 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:33:01.098815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 19:32:15.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-05 19:33:01.098815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-07-05 19:32:15.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 19:33:01.098815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-05 19:32:58.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:33:01.094815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:33:01.094815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 19:32:15.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11873 2023-07-05 19:32:15.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-07-05 19:32:15.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:33:01.098815 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-05 19:33:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-05 19:33:01.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 19:33:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-05 19:33:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 19:33:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230601153606
+Version: 1.0.0.dev20230705193219
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230601153606",
+  version="1.0.0.dev20230705193219",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 import os
 import re
 import boto3
 # import logging
 import numpy as np
 import botocore
-from botocore.config import Config
 import pandas as pd
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 
+# https://ncei-wcsd-archive.s3.amazonaws.com/index.html
+BUCKET_NAME = 'noaa-wcsd-pds'
+
+session = boto3.Session()
+
+dynamodb = session.client(service_name='dynamodb')
+
+max_pool_connections = 64
+client_config = botocore.config.Config(max_pool_connections=max_pool_connections)
+s3 = session.client(service_name='s3', config=client_config)
+
+# logging.basicConfig(level=logging.DEBUG)
+# logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+# Name of dynamoDB table to hold cruise level details
+INDEX_EK60_TABLE_NAME = 'noaa-wcsd-pds-index-ek60'
+
+
 class LambdaExecutor:
 
     def __init__(self, index_ek60_table_name, bucket_name, calibration_bucket, calibration_key):
         self.index_ek60_table_name = index_ek60_table_name
         self.bucket_name = bucket_name
         self.calibration_bucket = calibration_bucket
         self.calibration_key = calibration_key
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230705193219/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230601153606
+Version: 1.0.0.dev20230705193219
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

