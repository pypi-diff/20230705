# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731.tar", last modified: Wed May 24 19:28:40 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356.tar", last modified: Wed Jul  5 18:54:52 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-24 19:27:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-05-24 19:27:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-24 19:28:37.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 19:27:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      909 2023-05-24 19:27:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-24 19:27:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 19:28:40.249647 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-05-24 19:28:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-24 19:28:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 19:28:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-24 19:28:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-24 19:28:40.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:54:52.517141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 18:53:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-05 18:54:52.517141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-05 18:53:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 18:54:52.517141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-05 18:54:50.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:54:52.513141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:54:52.517141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 18:53:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      909 2023-07-05 18:53:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-05 18:53:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:54:52.517141 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-05 18:54:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-05 18:54:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:54:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 18:54:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-05 18:54:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230524192731
+Version: 1.0.0.dev20230705185356
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230524192731",
+  version="1.0.0.dev20230705185356",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230524192731
+Version: 1.0.0.dev20230705185356
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230524192731/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230705185356/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

