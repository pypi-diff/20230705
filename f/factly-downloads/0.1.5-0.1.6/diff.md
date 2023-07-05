# Comparing `tmp/factly_downloads-0.1.5.tar.gz` & `tmp/factly_downloads-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factly_downloads-0.1.5.tar", max compression
+gzip compressed data, was "factly_downloads-0.1.6.tar", max compression
```

## Comparing `factly_downloads-0.1.5.tar` & `factly_downloads-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2022-09-27 06:09:49.263010 factly_downloads-0.1.5/factly/downloads/__init__.py
--rw-r--r--   0        0        0     8101 2022-12-26 17:49:42.136913 factly_downloads-0.1.5/factly/downloads/downloads.py
--rw-r--r--   0        0        0     5765 2022-12-26 17:49:42.137006 factly_downloads-0.1.5/factly/downloads/wasabi_bulk_upload.py
--rw-r--r--   0        0        0     2885 2022-12-26 17:49:42.137107 factly_downloads-0.1.5/factly/downloads/wasabi_download.py
--rw-r--r--   0        0        0     4664 2023-03-02 06:30:01.914166 factly_downloads-0.1.5/factly/downloads/wasabi_sync_download.py
--rw-r--r--   0        0        0     2543 2022-12-26 17:49:42.137216 factly_downloads-0.1.5/factly/downloads/wasabi_upload.py
--rw-r--r--   0        0        0      425 2023-03-02 06:31:57.192934 factly_downloads-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 factly_downloads-0.1.5/setup.py
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 factly_downloads-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2021-07-08 12:57:20.000000 factly_downloads-0.1.6/factly/downloads/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-05 06:01:19.625924 factly_downloads-0.1.6/factly/downloads/config.py
+-rw-r--r--   0        0        0     8101 2022-12-12 10:21:42.264225 factly_downloads-0.1.6/factly/downloads/downloads.py
+-rw-r--r--   0        0        0     5765 2022-12-12 10:21:42.264299 factly_downloads-0.1.6/factly/downloads/wasabi_bulk_upload.py
+-rw-r--r--   0        0        0     2885 2023-07-03 12:46:22.857714 factly_downloads-0.1.6/factly/downloads/wasabi_download.py
+-rw-r--r--   0        0        0     4180 2023-07-05 06:01:19.626098 factly_downloads-0.1.6/factly/downloads/wasabi_sync_download.py
+-rw-r--r--   0        0        0     2005 2023-07-05 06:01:19.626855 factly_downloads-0.1.6/factly/downloads/wasabi_upload.py
+-rw-r--r--   0        0        0      442 2023-07-05 06:03:51.370010 factly_downloads-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 factly_downloads-0.1.6/PKG-INFO
```

### Comparing `factly_downloads-0.1.5/factly/downloads/downloads.py` & `factly_downloads-0.1.6/factly/downloads/downloads.py`

 * *Files identical despite different names*

### Comparing `factly_downloads-0.1.5/factly/downloads/wasabi_bulk_upload.py` & `factly_downloads-0.1.6/factly/downloads/wasabi_bulk_upload.py`

 * *Files identical despite different names*

### Comparing `factly_downloads-0.1.5/factly/downloads/wasabi_download.py` & `factly_downloads-0.1.6/factly/downloads/wasabi_download.py`

 * *Files identical despite different names*

### Comparing `factly_downloads-0.1.5/factly/downloads/wasabi_sync_download.py` & `factly_downloads-0.1.6/factly/downloads/wasabi_sync_download.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,54 @@
+import datetime
 import logging
-
-# import json
 import os
 from pathlib import Path
 
 import boto3
 
-logging.basicConfig(level="INFO")
-# import asyncio
-
-
-def get_access_keys():
-    """
-    Summary: this function takes no arguments but provides wasabi access key and secret key
+from .config import Settings
 
-    Returns:
-        (String): it is a string tuple contains information of secret key and access key
-    """
-    try:
-        WASABI_ACCESS_KEY = os.environ["S3_ACCESS_KEY"]
-        WASABI_SECRET_KEY = os.environ["S3_SECRET_KEY"]
-    except Exception as e:
-        if "File" in str(e):
-            print(
-                "please configure wasabi_keys.cfg with 'key' and 'secret' key words"
-            )
-    return WASABI_ACCESS_KEY, WASABI_SECRET_KEY
+settings = Settings()
 
 
-def sync_files(
-    project_bucket_path, remote_directory_name, local_file_list, local_path
-):
+def sync_files(project_bucket_path, remote_directory_name, local_file_list, local_path):
     """
     Summary: it creates a replica in local by checking local files and wasabi files
 
     Args:
         project_bucket_path (s3 bucket object): _description_
         remote_directory_name (string): it describes the wasabi file path
         local_file_list (List): it is a list of files in local machine
     """
     # filtering the objects based on wasabi path
-    if (
-        len(
-            list(
-                project_bucket_path.objects.filter(
-                    Prefix=remote_directory_name
-                )
+    if len(list(project_bucket_path.objects.filter(Prefix=remote_directory_name))) != 0:
+        for obj in project_bucket_path.objects.filter(Prefix=remote_directory_name):
+            # check if wasabi file exist in local or not and which is latest
+            exists_local = (
+                str(obj.key).split(f"{remote_directory_name}")[-1] in local_file_list
             )
-        )
-        != 0
-    ):
-        for obj in project_bucket_path.objects.filter(
-            Prefix=remote_directory_name
-        ):
-            # check if wasabi file exist in local or not
-            if (
-                str(obj.key).split(f"{remote_directory_name}")[-1]
-                in local_file_list
-            ):
-                logging.info(" - File exist in local")
+            lastest_on_local = False
+            if exists_local:
+                lastest_on_local = (
+                    datetime.datetime.fromtimestamp(
+                        os.stat(Path(local_path / str(obj.key))).st_mtime
+                    )
+                    > obj.last_modified
+                )
+                logging.info(" - File exist in local and but has new version on s3")
+                if lastest_on_local:
+                    logging.info(" - File exist in local and is latest")
             else:
                 if obj.size != 0:
                     logging.info(" - File does not exist in local")
                     output_file = get_directory(
                         obj.key, local_path, remote_directory_name
                     )
-                    logging.info(
-                        f" Downloading file {obj.key} to {str(output_file)}"
-                    )
-                    project_bucket_path.download_file(
-                        Filename=output_file, Key=obj.key
-                    )
+                    logging.info(f" Downloading file {obj.key} to {str(output_file)}")
+                    project_bucket_path.download_file(Filename=output_file, Key=obj.key)
                 else:
                     logging.info("--skipping file as it is of size zero")
     else:
         logging.info(" - Please check wasabi_path for existence")
     return
 
 
@@ -84,22 +58,15 @@
 
     Args:
         file_path (String): it is the wasabi file path
 
     Returns:
         output_file (String): it is the output file path
     """
-    if (
-        len(
-            file_path.split(f"{remote_directory_name}")[-1]
-            .strip("/")
-            .split("/")
-        )
-        > 1
-    ):
+    if len(file_path.split(f"{remote_directory_name}")[-1].strip("/").split("/")) > 1:
         local_path = (
             local_path
             + "/"
             + "/".join(
                 file_path.split(f"{remote_directory_name}")[-1]
                 .strip("/")
                 .split("/")[:-1]
@@ -120,29 +87,25 @@
         wasabi_path (String): wasabi path
         local_path (String): local folder path
     """
     # handling improper input
     wasabi_path = wasabi_path.strip("/")
     local_path = local_path.strip("/")
     local_path = "/" + local_path
-    # Read Access Key and Secret Key
-    WASABI_ACCESS_KEY, WASABI_SECRET_KEY = get_access_keys()
+
     # starting wasabi session
     session = boto3.Session(
-        aws_access_key_id=WASABI_ACCESS_KEY,
-        aws_secret_access_key=WASABI_SECRET_KEY,
+        aws_access_key_id=settings.S3_ACCESS_KEY,
+        aws_secret_access_key=settings.S3_SECRET_KEY,
+        region_name=settings.S3_REGION,
     )
     s3 = session.resource(
-        "s3", endpoint_url="https://s3.eu-central-1.wasabisys.com"
+        "s3", endpoint_url=settings.S3_HOST, region_name=settings.S3_REGION
     )
     project_bucket_path = s3.Bucket(bucket_name)
     remote_directory_name = wasabi_path
     # checking local files
     local_path_file = list(Path(local_path).glob("**/*.*"))
     # creating file list
-    local_file_list = [
-        str(i).split(f"{local_path}")[-1] for i in local_path_file
-    ]
-    sync_files(
-        project_bucket_path, remote_directory_name, local_file_list, local_path
-    )
+    local_file_list = [str(i).split(f"{local_path}")[-1] for i in local_path_file]
+    sync_files(project_bucket_path, remote_directory_name, local_file_list, local_path)
     return True
```

### Comparing `factly_downloads-0.1.5/factly/downloads/wasabi_upload.py` & `factly_downloads-0.1.6/factly/downloads/wasabi_upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,62 @@
-import json
-import os
-import sys
+import logging
 
 import boto3
-from botocore.exceptions import NoCredentialsError
 
+from .config import Settings
 
-def wasabi_upload(
-    bucket_name, wasabi_path, local_file_path, access_tokens=None, s3_host=None
-):
+
+def validate_bucket_name(base_name: str) -> str:
+    """Functionality to add prefix "stag" to Project base name while creating bucket
+
+    Args:
+        base_name (str): Project Name; example: "cricket"
+
+    Returns:
+        str: Project name with prefix stag-; example: "stag-cricket"
     """
-    function to upload files from local to wasabi
+    if not base_name.startswith("stag-"):
+        base_name = f"stag-{base_name}"
+    return base_name
+
+
+settings = Settings()
+
+
+def wasabi_upload(bucket_name: str, wasabi_path: str, local_file_path: str):
+    """Functionality to upload a file to wasabi cloud, using file path
+
+    Args:
+        bucket_name (str): Bucket name to upload file to, usually project name, example: "cricket"
+        wasabi_path (str): Location in wasabi to store. Recommended to use the same as local file path
+        local_file_path (str): Local file path inside the Projects data directory, example: "cricket/2021/01/01/20210101-123456.csv"
     """
-    if access_tokens is None:
-        try:
-            if os.environ["S3_ACCESS_KEY"] and os.environ["S3_SECRET_KEY"]:
-                WASABI_ACCESS_KEY = os.environ["S3_ACCESS_KEY"]
-                WASABI_SECRET_KEY = os.environ["S3_SECRET_KEY"]
-        except KeyError:
-            print(
-                "environment variables S3_ACCESS_KEY or S3_SECRET_KEY is not set."
-            )
-            sys.exit(1)
-    else:
-        with open(access_tokens, "r") as wasabi_keys:
-            wasabi = json.load(wasabi_keys)
-            WASABI_ACCESS_KEY = wasabi["key"]
-            WASABI_SECRET_KEY = wasabi["secret"]
-    if s3_host is None:
-        try:
-            if os.environ["S3_HOST"]:
-                S3_HOST = os.environ["S3_HOST"]
-        except KeyError:
-            print("environment variables S3_HOST is not set.")
-            sys.exit(1)
-    else:
-        S3_HOST = s3_host
-    # Creating a Session on Wasabi
-    # mentioning the endpoint to wasabi, this is insane
-    session = boto3.Session(
-        aws_access_key_id=WASABI_ACCESS_KEY,
-        aws_secret_access_key=WASABI_SECRET_KEY,
+    # validate bucket name
+    bucket_name = validate_bucket_name(bucket_name)
+
+    s3 = boto3.client(
+        "s3",
+        aws_access_key_id=settings.S3_ACCESS_KEY,
+        aws_secret_access_key=settings.S3_SECRET_KEY,
+        endpoint_url=settings.S3_HOST,
     )
-    s3 = session.resource("s3", endpoint_url=S3_HOST)
-    """
-    This next command will create a new bucket for the dataset that we are wroking on
-    """
-    # for bucket in s3.buckets.all():
-    #     if bucket.name == bucket_name:
-    #         print(bucket_name + " bucket already exists")
-    #         wasabi_bucket = bucket_name
-    #         pass
-    #     else:
-    wasabi_bucket = s3.create_bucket(Bucket=bucket_name)
-
-    def upload_to_wasabi(file_name, bucket, data):
-        """
-        Function to upload a dataset on to the wasabi cloud
-        """
-        try:
-            s3.Bucket(bucket).put_object(Key=file_name, Body=data)
-            print("Upload Successful")
-            return True
-        except FileNotFoundError:
-            print("The file was not found")
-            return False
-        except NoCredentialsError:
-            print("Credentials not available")
-            return False
-
-    data = open(local_file_path, "rb")
-    wasabi_bucket = bucket_name
-    # invoking the upload function to wasabi or amazon s3.
-    upload_to_wasabi(wasabi_path, wasabi_bucket, data)
-    print("file uploaded to wasabi on this path: ", wasabi_path)
+
+    # Check if the bucket exists
+    bucket_exists = False
+    try:
+        s3.head_bucket(Bucket=bucket_name)
+        bucket_exists = True
+    except Exception as e:
+        logging.info(f"Bucket does not exist: {e}")
+
+    # Create the bucket if it doesn't exist
+    if not bucket_exists:
+        logging.info(f"Creating bucket: {bucket_name}")
+        s3.create_bucket(Bucket=bucket_name)
+        logging.info(f"Bucket created: {bucket_name}")
+
+    # Upload the file to the S3 bucket
+    logging.info(f"Bucket name: {bucket_name}")
+    logging.info(f"Uploading file: {local_file_path}")
+    logging.info(f"Wasabi File path: {wasabi_path}")
+    s3.upload_file(local_file_path, bucket_name, wasabi_path)
+    logging.info("File uploaded successfully.")
```

