# Comparing `tmp/stc-geck-1.2.4.tar.gz` & `tmp/stc-geck-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.4.tar", last modified: Wed Jul  5 19:33:08 2023, max compression
+gzip compressed data, was "stc-geck-1.2.5.tar", last modified: Wed Jul  5 19:35:12 2023, max compression
```

## Comparing `stc-geck-1.2.4.tar` & `stc-geck-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:33:08.732862 stc-geck-1.2.4/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.4/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:33:08.732543 stc-geck-1.2.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.4/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-05 16:21:06.000000 stc-geck-1.2.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.2.4/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 19:33:08.732956 stc-geck-1.2.4/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:33:08.728733 stc-geck-1.2.4/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)      891 2023-07-05 08:35:32.000000 stc-geck-1.2.4/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.2.4/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5949 2023-07-05 18:55:54.000000 stc-geck-1.2.4/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.4/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:33:08.731887 stc-geck-1.2.4/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-05 19:33:08.000000 stc-geck-1.2.4/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.061931 stc-geck-1.2.5/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.5/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:35:12.061662 stc-geck-1.2.5/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.5/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-05 19:34:52.000000 stc-geck-1.2.5/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.2.5/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 19:35:12.062031 stc-geck-1.2.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.059336 stc-geck-1.2.5/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)      891 2023-07-05 08:35:32.000000 stc-geck-1.2.5/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.2.5/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5949 2023-07-05 19:34:46.000000 stc-geck-1.2.5/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.5/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.061118 stc-geck-1.2.5/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.4/PKG-INFO` & `stc-geck-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.4
+Version: 1.2.5
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.2.4/pyproject.toml` & `stc-geck-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.4"
+version = "1.2.5"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.4/stc_geck/advices.py` & `stc-geck-1.2.5/stc_geck/advices.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.4/stc_geck/cli.py` & `stc-geck-1.2.5/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.4/stc_geck/client.py` & `stc-geck-1.2.5/stc_geck/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         self.temp_dir = None
 
     async def start(self):
         self.temp_dir = tempfile.TemporaryDirectory()
         if self.embed:
             server_config = get_config()
             server_config['api']['grpc_endpoint'] = self.grpc_api_endpoint
-            server_config['home_path'] = self.temp_dir.name
+            server_config['data_path'] = self.temp_dir.name
             server_config['log_path'] = self.temp_dir.name
             for index_name in self.index_names:
                 query_parser_config = {
                     'default_fields': ['abstract', 'title']
                 }
                 full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index_name + '/'
                 headers_template = {'range': 'bytes={start}-{end}'}
```

### Comparing `stc-geck-1.2.4/stc_geck/utils.py` & `stc-geck-1.2.5/stc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.4/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.2.5/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.4
+Version: 1.2.5
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

