# Comparing `tmp/citybrain-official-0.7.tar.gz` & `tmp/citybrain-official-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citybrain-official-0.7.tar", last modified: Mon Jul  3 09:00:01 2023, max compression
+gzip compressed data, was "citybrain-official-0.8.tar", last modified: Wed Jul  5 02:59:46 2023, max compression
```

## Comparing `citybrain-official-0.7.tar` & `citybrain-official-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.087763 citybrain-official-0.7/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.7/LICENSE
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 09:00:01.087552 citybrain-official-0.7/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.7/README.md
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.086265 citybrain-official-0.7/citybrain_official/
--rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.7/citybrain_official/__init__.py
--rw-r--r--   0 mabingtao   (501) staff       (20)     5480 2023-07-03 08:59:12.000000 citybrain-official-0.7/citybrain_official/client.py
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.087261 citybrain-official-0.7/citybrain_official.egg-info/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/SOURCES.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/dependency_links.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/requires.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/top_level.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-03 09:00:01.087826 citybrain-official-0.7/setup.cfg
--rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-03 08:59:47.000000 citybrain-official-0.7/setup.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.378987 citybrain-official-0.8/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.8/LICENSE
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-05 02:59:46.378797 citybrain-official-0.8/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.8/README.md
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.377430 citybrain-official-0.8/citybrain_official/
+-rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.8/citybrain_official/__init__.py
+-rw-r--r--   0 mabingtao   (501) staff       (20)     5505 2023-07-05 02:58:47.000000 citybrain-official-0.8/citybrain_official/client.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-05 02:59:46.378522 citybrain-official-0.8/citybrain_official.egg-info/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/SOURCES.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/dependency_links.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/requires.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-05 02:59:46.000000 citybrain-official-0.8/citybrain_official.egg-info/top_level.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-05 02:59:46.379060 citybrain-official-0.8/setup.cfg
+-rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-05 02:59:11.000000 citybrain-official-0.8/setup.py
```

### Comparing `citybrain-official-0.7/LICENSE` & `citybrain-official-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.7/PKG-INFO` & `citybrain-official-0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.7
+Version: 0.8
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citybrain-official-0.7/README.md` & `citybrain-official-0.8/README.md`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.7/citybrain_official/client.py` & `citybrain-official-0.8/citybrain_official/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 __DEFAULT_ODPS_DATA_ADDRESS = "170DD61338021000"
 
 endpoint: str = ""
 
 def __get_endpoint() -> str:
     if endpoint != '':
         return endpoint
-    envEndpoint = os.getenv('ENDPOINT')
+    envEndpoint = os.getenv('CITYBRAIN_DATA_ENDPOINT')
     if envEndpoint is not None and envEndpoint != '':
         return envEndpoint
     return __DEFAULT_ENDPOINT
 
 
 def __get_odps_dataaddress(dataAddress: str) -> str:
     if dataAddress != '':
         return dataAddress
-    envODPSDataAddress = os.getenv('ODPS_DATA_ADDRESS')
+    envODPSDataAddress = os.getenv('CITYBRAIN_ODPS_DATA_ADDRESS')
     if envODPSDataAddress is not None and envODPSDataAddress != '':
         return envODPSDataAddress
     return __DEFAULT_ODPS_DATA_ADDRESS
 
 def retrieve_raw(dataAddress: str = '', sql: str = '') -> any:
     if sql == '':
         if dataAddress == '':
```

### Comparing `citybrain-official-0.7/citybrain_official.egg-info/PKG-INFO` & `citybrain-official-0.8/citybrain_official.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.7
+Version: 0.8
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

