# Comparing `tmp/key_switcheroo-0.0.1.tar.gz` & `tmp/key_switcheroo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.1.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.2.tar", max compression
```

## Comparing `key_switcheroo-0.0.1.tar` & `key_switcheroo-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:58:38.586289 key_switcheroo-0.0.1/key_switcheroo/__init__.py
--rw-r--r--   0        0        0     1746 2023-07-05 16:58:39.506289 key_switcheroo-0.0.1/key_switcheroo/custom_keygen.py
--rw-r--r--   0        0        0        0 2023-07-05 16:58:29.416290 key_switcheroo-0.0.1/key_switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1507 2023-07-05 16:58:27.876290 key_switcheroo-0.0.1/key_switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     2296 2023-07-05 16:58:26.656290 key_switcheroo-0.0.1/key_switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 16:58:33.416289 key_switcheroo-0.0.1/key_switcheroo/server/__init__.py
--rw-r--r--   0        0        0     2921 2023-07-05 16:58:35.326289 key_switcheroo-0.0.1/key_switcheroo/server/data_stores.py
--rwxr-xr-x   0        0        0     1093 2023-07-05 16:58:36.466289 key_switcheroo-0.0.1/key_switcheroo/server/retrieve_public_keys.py
--rw-r--r--   0        0        0     5336 2023-07-05 16:58:37.606289 key_switcheroo-0.0.1/key_switcheroo/server/server.py
--rw-r--r--   0        0        0     1934 2023-07-05 16:58:40.626289 key_switcheroo-0.0.1/key_switcheroo/util.py
--rw-r--r--   0        0        0      486 2023-07-05 17:06:27.586164 key_switcheroo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:58:38.586289 key_switcheroo-0.0.2/key_switcheroo/__init__.py
+-rw-r--r--   0        0        0     1746 2023-07-05 16:58:39.506289 key_switcheroo-0.0.2/key_switcheroo/custom_keygen.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:58:29.416290 key_switcheroo-0.0.2/key_switcheroo/publisher/__init__.py
+-rw-r--r--   0        0        0     1507 2023-07-05 16:58:27.876290 key_switcheroo-0.0.2/key_switcheroo/publisher/__main__.py
+-rw-r--r--   0        0        0     2296 2023-07-05 16:58:26.656290 key_switcheroo-0.0.2/key_switcheroo/publisher/key_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:58:33.416289 key_switcheroo-0.0.2/key_switcheroo/server/__init__.py
+-rw-r--r--   0        0        0     2921 2023-07-05 16:58:35.326289 key_switcheroo-0.0.2/key_switcheroo/server/data_stores.py
+-rwxr-xr-x   0        0        0     1093 2023-07-05 16:58:36.466289 key_switcheroo-0.0.2/key_switcheroo/server/retrieve_public_keys.py
+-rw-r--r--   0        0        0     5336 2023-07-05 16:58:37.606289 key_switcheroo-0.0.2/key_switcheroo/server/server.py
+-rw-r--r--   0        0        0     1934 2023-07-05 16:58:40.626289 key_switcheroo-0.0.2/key_switcheroo/util.py
+-rw-r--r--   0        0        0      486 2023-07-05 17:06:27.586164 key_switcheroo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.2/PKG-INFO
```

### Comparing `key_switcheroo-0.0.1/key_switcheroo/custom_keygen.py` & `key_switcheroo-0.0.2/key_switcheroo/custom_keygen.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.2/key_switcheroo/publisher/__main__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/publisher/key_publisher.py` & `key_switcheroo-0.0.2/key_switcheroo/publisher/key_publisher.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/server/data_stores.py` & `key_switcheroo-0.0.2/key_switcheroo/server/data_stores.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/server/retrieve_public_keys.py` & `key_switcheroo-0.0.2/key_switcheroo/server/retrieve_public_keys.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/server/server.py` & `key_switcheroo-0.0.2/key_switcheroo/server/server.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/key_switcheroo/util.py` & `key_switcheroo-0.0.2/key_switcheroo/util.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.1/PKG-INFO` & `key_switcheroo-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

