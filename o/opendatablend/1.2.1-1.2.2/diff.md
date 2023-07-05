# Comparing `tmp/opendatablend-1.2.1.tar.gz` & `tmp/opendatablend-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendatablend-1.2.1.tar", last modified: Fri Apr 15 16:44:48 2022, max compression
+gzip compressed data, was "opendatablend-1.2.2.tar", last modified: Wed Jul  5 07:47:47 2023, max compression
```

## Comparing `opendatablend-1.2.1.tar` & `opendatablend-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-15 16:44:48.454396 opendatablend-1.2.1/
--rw-rw-rw-   0        0        0     1110 2021-07-06 22:59:46.000000 opendatablend-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     8903 2022-04-15 16:44:48.456400 opendatablend-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8280 2022-04-15 16:43:19.000000 opendatablend-1.2.1/README.md
--rw-rw-rw-   0        0        0      108 2021-07-06 22:59:46.000000 opendatablend-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      854 2022-04-15 16:44:48.464384 opendatablend-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-15 16:44:48.355253 opendatablend-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-04-15 16:44:48.371370 opendatablend-1.2.1/src/opendatablend/
--rw-rw-rw-   0        0        0       48 2021-07-06 22:59:46.000000 opendatablend-1.2.1/src/opendatablend/__init__.py
--rw-rw-rw-   0        0        0    16615 2022-04-15 16:40:50.000000 opendatablend-1.2.1/src/opendatablend/opendatablend.py
-drwxrwxrwx   0        0        0        0 2022-04-15 16:44:48.448380 opendatablend-1.2.1/src/opendatablend.egg-info/
--rw-rw-rw-   0        0        0     8903 2022-04-15 16:44:46.000000 opendatablend-1.2.1/src/opendatablend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2022-04-15 16:44:48.000000 opendatablend-1.2.1/src/opendatablend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-15 16:44:46.000000 opendatablend-1.2.1/src/opendatablend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-04-15 16:44:47.000000 opendatablend-1.2.1/src/opendatablend.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-04-15 16:44:47.000000 opendatablend-1.2.1/src/opendatablend.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.866522 opendatablend-1.2.2/
+-rw-rw-rw-   0        0        0     1110 2021-07-06 22:59:46.000000 opendatablend-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     8862 2023-07-05 07:47:47.868525 opendatablend-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8280 2022-04-15 16:48:40.000000 opendatablend-1.2.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-07-06 22:59:46.000000 opendatablend-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      861 2023-07-05 07:47:47.876170 opendatablend-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.703982 opendatablend-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.767272 opendatablend-1.2.2/src/opendatablend/
+-rw-rw-rw-   0        0        0       48 2021-07-06 22:59:46.000000 opendatablend-1.2.2/src/opendatablend/__init__.py
+-rw-rw-rw-   0        0        0    16623 2023-07-05 07:38:24.000000 opendatablend-1.2.2/src/opendatablend/opendatablend.py
+drwxrwxrwx   0        0        0        0 2023-07-05 07:47:47.862507 opendatablend-1.2.2/src/opendatablend.egg-info/
+-rw-rw-rw-   0        0        0     8862 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-05 07:47:47.000000 opendatablend-1.2.2/src/opendatablend.egg-info/top_level.txt
```

### Comparing `opendatablend-1.2.1/LICENSE` & `opendatablend-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opendatablend-1.2.1/PKG-INFO` & `opendatablend-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: opendatablend
-Version: 1.2.1
+Version: 1.2.2
 Summary: The fastest way to get data from the Open Data Blend Dataset API
 Home-page: https://github.com/opendatablend/opendatablend-py
 Author: Open Data Blend
 Author-email: info@opendatablend.io
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/opendatablend/opendatablend-py/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://raw.githubusercontent.com/opendatablend/opendatablend-py/master/images/odblogo.png "Open Data Blend")
 
 # Open Data Blend for Python
 
@@ -219,9 +217,7 @@
 print(output.data_file_name)
 print(output.metadata_file_name)
 ```
 
 ## Additional Examples
 
 For more in-depth examples, see the [examples](https://github.com/opendatablend/opendatablend-py/tree/master/examples) folder.
-
-
```

### Comparing `opendatablend-1.2.1/README.md` & `opendatablend-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `opendatablend-1.2.1/setup.cfg` & `opendatablend-1.2.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 7065 6e64 6174 6162 6c65 6e64   = opendatablend
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 310d 0a61 7574 686f 7220 3d20 4f70 656e  1..author = Open
+00000030: 320d 0a61 7574 686f 7220 3d20 4f70 656e  2..author = Open
 00000040: 2044 6174 6120 426c 656e 640d 0a61 7574   Data Blend..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 696e 666f  hor_email = info
 00000060: 406f 7065 6e64 6174 6162 6c65 6e64 2e69  @opendatablend.i
 00000070: 6f0d 0a64 6573 6372 6970 7469 6f6e 203d  o..description =
 00000080: 2054 6865 2066 6173 7465 7374 2077 6179   The fastest way
 00000090: 2074 6f20 6765 7420 6461 7461 2066 726f   to get data fro
 000000a0: 6d20 7468 6520 4f70 656e 2044 6174 6120  m the Open Data 
@@ -33,22 +33,22 @@
 00000200: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
 00000210: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 00000220: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
 00000230: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 00000240: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 00000250: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000260: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000270: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
+00000270: 7265 7320 3d20 3e3d 332e 370d 0a69 6e73  res = >=3.7..ins
 00000280: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
 00000290: 0d0a 0961 7a75 7265 2d73 746f 7261 6765  ...azure-storage
 000002a0: 2d62 6c6f 623e 3d31 322e 3130 2e30 0d0a  -blob>=12.10.0..
 000002b0: 0962 6f74 6f33 0d0a 0962 6f74 6f63 6f72  .boto3...botocor
 000002c0: 650d 0a09 676f 6f67 6c65 2d63 6c6f 7564  e...google-cloud
 000002d0: 2d73 746f 7261 6765 3e3d 322e 332e 300d  -storage>=2.3.0.
 000002e0: 0a09 6672 6963 7469 6f6e 6c65 7373 3e3d  ..frictionless>=
-000002f0: 342e 302e 300d 0a09 7265 7175 6573 7473  4.0.0...requests
-00000300: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000310: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000320: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000330: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000340: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000350: 2030 0d0a 0d0a                            0....
+000002f0: 342e 302e 302c 3c35 2e30 2e30 0d0a 0972  4.0.0,<5.0.0...r
+00000300: 6571 7565 7374 730d 0a0d 0a5b 6f70 7469  equests....[opti
+00000310: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000320: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000330: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000340: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000350: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `opendatablend-1.2.1/src/opendatablend/opendatablend.py` & `opendatablend-1.2.2/src/opendatablend/opendatablend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import errno
 from io import BytesIO
 from frictionless import Package
 import requests
 from azure.storage.blob import BlobServiceClient, BlobClient, ContainerClient, __version__
 import boto3
 from botocore.client import ClientError
 from google.cloud import storage
@@ -62,15 +63,15 @@
 def cache_data_file_to_local_file_system(data_file, access_key, data_file_name):
 
     # Create the directory for the data file if it doesn't exist
     if not os.path.exists(os.path.dirname(data_file_name)):
         try:
             os.makedirs(os.path.dirname(data_file_name))
         except OSError as ex:
-            if ex.errno != os.errno.EEXIST:
+            if ex.errno != errno.EEXIST:
                 raise
 
     # Only download the data file if it doesn't exist
     if not os.path.exists(data_file_name):
         if access_key != '':
             data_file_download_path = data_file.path + '?accesskey=' + access_key
         else:
@@ -239,15 +240,15 @@
 def cache_dataset_metadata_to_local_file_system(metadata_data_file_snapshot_path, metadata_file_name):
 
     # Create the directory for the dataset metadata file if it doesn't exist
     if not os.path.exists(os.path.dirname(metadata_file_name)):
         try:
             os.makedirs(os.path.dirname(metadata_file_name))
         except OSError as ex:
-            if ex.errno != os.errno.EEXIST:
+            if ex.errno != errno.EEXIST:
                 raise
 
     # Download the dataset metadata file if it doesn't exist
     if not os.path.exists(metadata_file_name):
         data = requests.get(metadata_data_file_snapshot_path)
 
         open(metadata_file_name, 'wb').write(data.content)
```

### Comparing `opendatablend-1.2.1/src/opendatablend.egg-info/PKG-INFO` & `opendatablend-1.2.2/src/opendatablend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: opendatablend
-Version: 1.2.1
+Version: 1.2.2
 Summary: The fastest way to get data from the Open Data Blend Dataset API
 Home-page: https://github.com/opendatablend/opendatablend-py
 Author: Open Data Blend
 Author-email: info@opendatablend.io
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/opendatablend/opendatablend-py/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://raw.githubusercontent.com/opendatablend/opendatablend-py/master/images/odblogo.png "Open Data Blend")
 
 # Open Data Blend for Python
 
@@ -219,9 +217,7 @@
 print(output.data_file_name)
 print(output.metadata_file_name)
 ```
 
 ## Additional Examples
 
 For more in-depth examples, see the [examples](https://github.com/opendatablend/opendatablend-py/tree/master/examples) folder.
-
-
```

