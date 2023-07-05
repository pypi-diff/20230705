# Comparing `tmp/shaku-database-1.1.0.tar.gz` & `tmp/shaku-database-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.0.tar", last modified: Wed Jul  5 04:43:39 2023, max compression
+gzip compressed data, was "shaku-database-1.1.1.tar", last modified: Wed Jul  5 06:31:46 2023, max compression
```

## Comparing `shaku-database-1.1.0.tar` & `shaku-database-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.556316 shaku-database-1.1.0/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.0/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 04:43:39.556146 shaku-database-1.1.0/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.0/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.553777 shaku-database-1.1.0/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.0/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.554005 shaku-database-1.1.0/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.0/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.0/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.554283 shaku-database-1.1.0/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.0/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.0/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.554450 shaku-database-1.1.0/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.0/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.554705 shaku-database-1.1.0/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.0/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-05 02:21:08.000000 shaku-database-1.1.0/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.555041 shaku-database-1.1.0/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.0/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    10665 2023-07-05 04:33:12.000000 shaku-database-1.1.0/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-05 04:43:39.556360 shaku-database-1.1.0/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-05 04:42:32.000000 shaku-database-1.1.0/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 04:43:39.555812 shaku-database-1.1.0/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 04:43:39.000000 shaku-database-1.1.0/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      565 2023-07-05 04:43:39.000000 shaku-database-1.1.0/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-05 04:43:39.000000 shaku-database-1.1.0/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-05 04:43:39.000000 shaku-database-1.1.0/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-05 04:43:39.000000 shaku-database-1.1.0/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.632696 shaku-database-1.1.1/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.1/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 06:31:46.632506 shaku-database-1.1.1/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.1/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.630556 shaku-database-1.1.1/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.630780 shaku-database-1.1.1/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.1/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631016 shaku-database-1.1.1/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.1/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.1/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631160 shaku-database-1.1.1/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631383 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.631638 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-05 02:21:08.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    10772 2023-07-05 06:31:10.000000 shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-05 06:31:46.632734 shaku-database-1.1.1/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-05 06:31:11.000000 shaku-database-1.1.1/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-05 06:31:46.632312 shaku-database-1.1.1/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      565 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-05 06:31:46.000000 shaku-database-1.1.1/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.0/LICENSE` & `shaku-database-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/PKG-INFO` & `shaku-database-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.0/README.md` & `shaku-database-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/database/bigquery/util.py` & `shaku-database-1.1.1/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/database/cloud_sql/crud.py` & `shaku-database-1.1.1/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.1/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.1/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,27 +242,31 @@
                                                supportsAllDrives=True,
                                                includeItemsFromAllDrives=True,
                                                driveId=self.shared_drive_id, corpora='drive'
                                                ).execute()
             files = result.get('files', [])
 
             media = MediaIoBaseUpload(data_buffer, mimetype=mimetype, resumable=True)
-            file_metadata = {
-                'name': file_name,
-                'parents': [folder_id]
-            }
+
 
             if len(files) > 0:
+                file_metadata = {
+                    'name': file_name
+                }
                 # file already exists, update it
                 file_id = files[0].get('id')
                 print(f"'{file_name}' is existed, update it")
                 self.service.files().update(fileId=file_id, body=file_metadata, media_body=media, fields='id',
                                             supportsAllDrives=True).execute()
                 print(f"'{file_name}' is updated")
             else:
+                file_metadata = {
+                    'name': file_name,
+                    'parents': [folder_id]
+                }
                 self.service.files().create(body=file_metadata, media_body=media, fields='id',
                                             supportsAllDrives=True).execute()
 
                 print(f"'{file_name}' is saved")
 
         except Exception as e:
             raise f'An error occurred:{e}'
```

### Comparing `shaku-database-1.1.0/setup.py` & `shaku-database-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.0",
+    version="1.1.1",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.0/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.1/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.0
+Version: 1.1.1
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.0/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.1/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.0/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.1/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

