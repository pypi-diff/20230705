# Comparing `tmp/stc-geck-1.2.2.tar.gz` & `tmp/stc-geck-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.2.tar", last modified: Mon Jul  3 18:44:53 2023, max compression
+gzip compressed data, was "stc-geck-1.2.3.tar", last modified: Wed Jul  5 10:26:26 2023, max compression
```

## Comparing `stc-geck-1.2.2.tar` & `stc-geck-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.117548 stc-geck-1.2.2/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.2/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:44:53.117309 stc-geck-1.2.2/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-04-25 17:50:47.000000 stc-geck-1.2.2/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-03 18:44:43.000000 stc-geck-1.2.2/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-03 15:18:02.000000 stc-geck-1.2.2/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-03 18:44:53.117642 stc-geck-1.2.2/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.115074 stc-geck-1.2.2/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)     6140 2023-07-03 18:42:15.000000 stc-geck-1.2.2/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     6106 2023-07-03 18:38:08.000000 stc-geck-1.2.2/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.2/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-03 18:44:53.116931 stc-geck-1.2.2/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      344 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      300 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-03 18:44:53.000000 stc-geck-1.2.2/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 10:26:26.825326 stc-geck-1.2.3/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.3/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 10:26:26.824023 stc-geck-1.2.3/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.3/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-05 09:12:39.000000 stc-geck-1.2.3/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       82 2023-07-05 09:12:47.000000 stc-geck-1.2.3/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 10:26:26.825899 stc-geck-1.2.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 10:26:26.807716 stc-geck-1.2.3/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)      891 2023-07-05 08:35:32.000000 stc-geck-1.2.3/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-03 19:42:55.000000 stc-geck-1.2.3/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6106 2023-07-03 18:38:08.000000 stc-geck-1.2.3/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.3/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 10:26:26.821723 stc-geck-1.2.3/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       83 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-05 10:26:26.000000 stc-geck-1.2.3/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.2/pyproject.toml` & `stc-geck-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.2"
+version = "1.2.3"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.2/stc_geck/cli.py` & `stc-geck-1.2.3/stc_geck/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,35 +130,35 @@
         async with self.geck as geck:
             return await geck.create_ipfs_directory(self.index_name, output_car, query, limit, name_template)
 
 
 async def stc_geck_cli(
     ipfs_http_endpoint: str = 'http://127.0.0.1:8080',
     ipfs_data_directory: str = '/ipns/standard-template-construct.org/data/',
-    index_alias: str = 'nexus_science',
+    index_name: str = 'nexus_science',
     grpc_api_endpoint: str = '127.0.0.1:37082',
     embed: bool = True,
     timeout: int = 600,
     debug: bool = False,
 ):
     """
     :param ipfs_http_endpoint: IPFS HTTP API Endpoint
     :param ipfs_data_directory: path to the directory with index
-    :param index_alias: `nexus_free` (non-classified content) or `nexus_science` (similar to Crossref)
+    :param index_name: `nexus_free` (non-classified content) or `nexus_science` (similar to Crossref)
     :param grpc_api_endpoint: port used for Summa
     :param embed: setup embedded Summa server
     :param timeout: timeout for requests to IPFS
     :param debug: add debugging output
     :return:
     """
     logging.basicConfig(stream=sys.stdout, level=logging.INFO if debug else logging.ERROR)
     stc_geck_client = StcGeckCli(
         ipfs_http_endpoint=ipfs_http_endpoint,
         ipfs_data_directory=ipfs_data_directory,
-        index_alias=index_alias,
+        index_name=index_name,
         grpc_api_endpoint=grpc_api_endpoint,
         embed=embed,
         timeout=timeout,
     )
     return {
         'search': stc_geck_client.search,
         'download': stc_geck_client.download,
```

### Comparing `stc-geck-1.2.2/stc_geck/client.py` & `stc-geck-1.2.3/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.2/stc_geck/utils.py` & `stc-geck-1.2.3/stc_geck/utils.py`

 * *Files identical despite different names*

