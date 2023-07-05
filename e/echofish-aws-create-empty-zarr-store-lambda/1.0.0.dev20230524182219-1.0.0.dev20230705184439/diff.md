# Comparing `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219.tar.gz` & `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219.tar", last modified: Wed May 24 18:23:25 2023, max compression
+gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar", last modified: Wed Jul  5 18:45:35 2023, max compression
```

## Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219.tar` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-24 18:22:12.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2534 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2161 2023-05-24 18:22:12.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      733 2023-05-24 18:23:22.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 18:22:12.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12014 2023-05-24 18:22:12.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-24 18:22:12.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 18:23:25.642152 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2534 2023-05-24 18:23:25.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-24 18:23:25.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 18:23:25.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-24 18:23:25.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-24 18:23:25.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      733 2023-07-05 18:45:32.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.720362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.720362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12014 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/LICENSE` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230524182219
+Version: 1.0.0.dev20230705184439
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/README.md` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/setup.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-create-empty-zarr-store-lambda",
-  version="1.0.0.dev20230524182219",
+  version="1.0.0.dev20230705184439",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230524182219
+Version: 1.0.0.dev20230705184439
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230524182219/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

