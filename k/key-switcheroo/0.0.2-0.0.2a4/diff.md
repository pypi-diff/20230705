# Comparing `tmp/key_switcheroo-0.0.2.tar.gz` & `tmp/key_switcheroo-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.2.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.2a4.tar", max compression
```

## Comparing `key_switcheroo-0.0.2.tar` & `key_switcheroo-0.0.2a4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:58:38.586289 key_switcheroo-0.0.2/key_switcheroo/__init__.py
--rw-r--r--   0        0        0     1746 2023-07-05 16:58:39.506289 key_switcheroo-0.0.2/key_switcheroo/custom_keygen.py
--rw-r--r--   0        0        0        0 2023-07-05 16:58:29.416290 key_switcheroo-0.0.2/key_switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1507 2023-07-05 16:58:27.876290 key_switcheroo-0.0.2/key_switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     2296 2023-07-05 16:58:26.656290 key_switcheroo-0.0.2/key_switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 16:58:33.416289 key_switcheroo-0.0.2/key_switcheroo/server/__init__.py
--rw-r--r--   0        0        0     2921 2023-07-05 16:58:35.326289 key_switcheroo-0.0.2/key_switcheroo/server/data_stores.py
--rwxr-xr-x   0        0        0     1093 2023-07-05 16:58:36.466289 key_switcheroo-0.0.2/key_switcheroo/server/retrieve_public_keys.py
--rw-r--r--   0        0        0     5336 2023-07-05 16:58:37.606289 key_switcheroo-0.0.2/key_switcheroo/server/server.py
--rw-r--r--   0        0        0     1934 2023-07-05 16:58:40.626289 key_switcheroo-0.0.2/key_switcheroo/util.py
--rw-r--r--   0        0        0      486 2023-07-05 17:06:27.586164 key_switcheroo-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.2a4/README.md
+-rw-r--r--   0        0        0      540 2023-07-05 18:00:34.125340 key_switcheroo-0.0.2a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:24.365289 key_switcheroo-0.0.2a4/switcheroo/__init__.py
+-rw-r--r--   0        0        0     1746 2023-07-05 18:03:24.725289 key_switcheroo-0.0.2a4/switcheroo/custom_keygen.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:25.015289 key_switcheroo-0.0.2a4/switcheroo/publisher/__init__.py
+-rw-r--r--   0        0        0     1503 2023-07-05 18:03:25.365289 key_switcheroo-0.0.2a4/switcheroo/publisher/__main__.py
+-rw-r--r--   0        0        0     2288 2023-07-05 18:03:25.575289 key_switcheroo-0.0.2a4/switcheroo/publisher/key_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-05 18:03:25.865289 key_switcheroo-0.0.2a4/switcheroo/server/__init__.py
+-rw-r--r--   0        0        0     2917 2023-07-05 18:03:26.145289 key_switcheroo-0.0.2a4/switcheroo/server/data_stores.py
+-rwxr-xr-x   0        0        0     1093 2023-07-05 18:03:26.535289 key_switcheroo-0.0.2a4/switcheroo/server/retrieve_public_keys.py
+-rw-r--r--   0        0        0     5324 2023-07-05 18:03:27.025288 key_switcheroo-0.0.2a4/switcheroo/server/server.py
+-rw-r--r--   0        0        0     1934 2023-07-05 18:03:27.585288 key_switcheroo-0.0.2a4/switcheroo/util.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 key_switcheroo-0.0.2a4/PKG-INFO
```

### Comparing `key_switcheroo-0.0.2/key_switcheroo/custom_keygen.py` & `key_switcheroo-0.0.2a4/switcheroo/custom_keygen.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.2/key_switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.2a4/switcheroo/publisher/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from argparse import ArgumentParser
-from key_switcheroo.publisher.key_publisher import LocalPublisher, S3Publisher
+from switcheroo.publisher.key_publisher import LocalPublisher, S3Publisher
 
 
 def create_argument_parser() -> ArgumentParser:
     argument_parser = ArgumentParser(
         prog="key_publisher",
         description="Creates public/private SSH keys and publishes "
         + "the public key either locally or to S3 (default is S3)",
```

### Comparing `key_switcheroo-0.0.2/key_switcheroo/publisher/key_publisher.py` & `key_switcheroo-0.0.2a4/switcheroo/publisher/key_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
 import os
 import shutil
 import boto3
-from key_switcheroo.custom_keygen import (
+from switcheroo.custom_keygen import (
     generate_private_public_key_in_file,
     generate_private_public_key,
 )
-from key_switcheroo.util import get_user_path, get_username
+from switcheroo.util import get_user_path, get_username
 
 
 def _ensure_ssh_home_exists():
     ssh_home = f"{get_user_path()}/.ssh"
     if not os.path.isdir(ssh_home):
         os.makedirs(ssh_home)
```

### Comparing `key_switcheroo-0.0.2/key_switcheroo/server/data_stores.py` & `key_switcheroo-0.0.2a4/switcheroo/server/data_stores.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 "Data stores that specifies where a Server stores its keys"
 import os
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 import boto3
-from key_switcheroo.util import get_user_path
+from switcheroo.util import get_user_path
 
 
 class DataStore(ABC):
     "A server uses a DataStore to get public keys from somewhere."
 
     @abstractmethod
     def get_sshd_config_line(self):
```

### Comparing `key_switcheroo-0.0.2/key_switcheroo/server/retrieve_public_keys.py` & `key_switcheroo-0.0.2a4/switcheroo/server/retrieve_public_keys.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.2/key_switcheroo/server/server.py` & `key_switcheroo-0.0.2a4/switcheroo/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Callable
 import os
 import asyncio
 import pathlib
 import subprocess
 from asyncio.subprocess import Process
 from tempfile import NamedTemporaryFile
-from key_switcheroo.server.data_stores import DataStore
-from key_switcheroo.util import get_open_port
-from key_switcheroo.util import get_user_path, get_username
+from switcheroo.server.data_stores import DataStore
+from switcheroo.util import get_open_port
+from switcheroo.util import get_user_path, get_username
 
 
 class Server:
     "Wrapper for SSH Server. Takes a DataStore to determine where to look for keys"
 
     def __init__(
         self,
```

### Comparing `key_switcheroo-0.0.2/key_switcheroo/util.py` & `key_switcheroo-0.0.2a4/switcheroo/util.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.2/PKG-INFO` & `key_switcheroo-0.0.2a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.2
+Version: 0.0.2a4
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

