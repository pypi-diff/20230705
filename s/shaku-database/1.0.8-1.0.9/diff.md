# Comparing `tmp/shaku-database-1.0.8.tar.gz` & `tmp/shaku-database-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.0.8.tar", last modified: Fri Jun 16 06:53:06 2023, max compression
+gzip compressed data, was "shaku-database-1.0.9.tar", last modified: Wed Jul  5 02:24:11 2023, max compression
```

## Comparing `shaku-database-1.0.8.tar` & `shaku-database-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.276641 shaku-database-1.0.8/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.8/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-16 06:53:06.276511 shaku-database-1.0.8/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.8/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.274500 shaku-database-1.0.8/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.8/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.274720 shaku-database-1.0.8/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.8/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-15 08:42:39.000000 shaku-database-1.0.8/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.275206 shaku-database-1.0.8/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.8/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.0.8/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.275551 shaku-database-1.0.8/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.8/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-06-08 02:35:46.000000 shaku-database-1.0.8/database/cloud_storage/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-06-16 06:53:06.276681 shaku-database-1.0.8/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1056 2023-06-16 06:51:54.000000 shaku-database-1.0.8/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-06-16 06:53:06.276317 shaku-database-1.0.8/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7160 2023-06-16 06:53:06.000000 shaku-database-1.0.8/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      416 2023-06-16 06:53:06.000000 shaku-database-1.0.8/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-06-16 06:53:06.000000 shaku-database-1.0.8/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)      417 2023-06-16 06:53:06.000000 shaku-database-1.0.8/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        9 2023-06-16 06:53:06.000000 shaku-database-1.0.8/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.050106 shaku-database-1.0.9/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.0.9/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 02:24:11.049895 shaku-database-1.0.9/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.0.9/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.047069 shaku-database-1.0.9/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.9/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.047325 shaku-database-1.0.9/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.9/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.0.9/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.047849 shaku-database-1.0.9/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.0.9/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.0.9/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.048223 shaku-database-1.0.9/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.0.9/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.048473 shaku-database-1.0.9/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.0.9/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-05 02:21:08.000000 shaku-database-1.0.9/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.048761 shaku-database-1.0.9/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.0.9/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    10665 2023-07-05 02:21:08.000000 shaku-database-1.0.9/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-05 02:24:11.050158 shaku-database-1.0.9/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1056 2023-07-05 02:24:09.000000 shaku-database-1.0.9/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:24:11.049533 shaku-database-1.0.9/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 02:24:11.000000 shaku-database-1.0.9/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      565 2023-07-05 02:24:11.000000 shaku-database-1.0.9/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-05 02:24:11.000000 shaku-database-1.0.9/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      546 2023-07-05 02:24:11.000000 shaku-database-1.0.9/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-05 02:24:11.000000 shaku-database-1.0.9/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.0.8/LICENSE` & `shaku-database-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.8/PKG-INFO` & `shaku-database-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.8
+Version: 1.0.9
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,19 @@
 Provides-Extra: pyarrow
 Provides-Extra: PyMySQL
 Provides-Extra: requests
 Provides-Extra: rsa
 Provides-Extra: setuptools
 Provides-Extra: six
 Provides-Extra: sqlalchemy
+Provides-Extra: chardet
+Provides-Extra: google-api-python-client
+Provides-Extra: google-auth-oauthlib
+Provides-Extra: google-auth-httplib2
+Provides-Extra: pathlib
 License-File: LICENSE
 
 # shaku_data_util
 
 
 
 ## Getting started
```

### Comparing `shaku-database-1.0.8/README.md` & `shaku-database-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.8/database/bigquery/util.py` & `shaku-database-1.0.9/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.8/database/cloud_sql/crud.py` & `shaku-database-1.0.9/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.8/database/cloud_storage/util.py` & `shaku-database-1.0.9/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.0.8/setup.py` & `shaku-database-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else "" for s
                     in requirements.split("\n")}
 setup(
     name="shaku-database",
-    version="1.0.8",
+    version="1.0.9",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.0.8/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.0.9/shaku_database.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.0.8
+Version: 1.0.9
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,14 +25,19 @@
 Provides-Extra: pyarrow
 Provides-Extra: PyMySQL
 Provides-Extra: requests
 Provides-Extra: rsa
 Provides-Extra: setuptools
 Provides-Extra: six
 Provides-Extra: sqlalchemy
+Provides-Extra: chardet
+Provides-Extra: google-api-python-client
+Provides-Extra: google-auth-oauthlib
+Provides-Extra: google-auth-httplib2
+Provides-Extra: pathlib
 License-File: LICENSE
 
 # shaku_data_util
 
 
 
 ## Getting started
```

