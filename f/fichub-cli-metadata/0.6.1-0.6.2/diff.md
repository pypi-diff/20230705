# Comparing `tmp/fichub-cli-metadata-0.6.1.tar.gz` & `tmp/fichub-cli-metadata-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\Personal\Projects\Python\Others\fichub\fichub-cli\fichub-cli-contrib\fichub-cli-metadata\dist\.tmp-8gxrw85_\fichub-", last modified: Sun Jan 29 07:21:59 2023, max compression
+gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli-contrib\fichub-cli-metadata\dist\.tmp-ydaiioi8\f", last modified: Wed Jul  5 18:36:03 2023, max compression
```

## Comparing `fichub-cli-metadata-0.6.1.tar` & `fichub-cli-metadata-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:59.656711 fichub-cli-metadata-0.6.1/
--rw-rw-rw-   0        0        0    11357 2022-02-09 16:27:55.000000 fichub-cli-metadata-0.6.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5196 2023-01-29 07:21:59.656711 fichub-cli-metadata-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4656 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:59.618711 fichub-cli-metadata-0.6.1/fichub_cli_metadata/
--rw-rw-rw-   0        0        0      736 2023-01-29 07:21:15.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/__init__.py
--rw-rw-rw-   0        0        0     6746 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/cli.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:59.655710 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/
--rw-rw-rw-   0        0        0        0 2022-05-02 16:36:05.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/__init__.py
--rw-rw-rw-   0        0        0    10999 2023-01-29 07:20:31.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/crud.py
--rw-rw-rw-   0        0        0    20582 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/fetch_data.py
--rw-rw-rw-   0        0        0     1107 2022-03-18 14:02:06.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/logging.py
--rw-rw-rw-   0        0        0     1522 2023-01-29 07:18:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/models.py
--rw-rw-rw-   0        0        0     4264 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/processing.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:59.635710 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/
--rw-rw-rw-   0        0        0     5196 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-01-29 07:21:59.000000 fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2022-02-09 16:18:06.000000 fichub-cli-metadata-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-01-29 07:21:59.658711 fichub-cli-metadata-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-01-29 07:21:15.000000 fichub-cli-metadata-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.574312 fichub-cli-metadata-0.6.2/
+-rw-rw-rw-   0        0        0    11357 2022-02-09 16:27:55.000000 fichub-cli-metadata-0.6.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5196 2023-07-05 18:36:03.574312 fichub-cli-metadata-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4656 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.534311 fichub-cli-metadata-0.6.2/fichub_cli_metadata/
+-rw-rw-rw-   0        0        0      736 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/__init__.py
+-rw-rw-rw-   0        0        0     6493 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.572312 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-02 16:36:05.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/__init__.py
+-rw-rw-rw-   0        0        0    11124 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/crud.py
+-rw-rw-rw-   0        0        0    20582 2023-07-05 17:06:07.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/fetch_data.py
+-rw-rw-rw-   0        0        0     1138 2023-07-05 17:06:07.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/logging.py
+-rw-rw-rw-   0        0        0     1522 2023-06-19 06:33:58.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/models.py
+-rw-rw-rw-   0        0        0     4264 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/processing.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.564312 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/
+-rw-rw-rw-   0        0        0     5196 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2022-02-09 16:18:06.000000 fichub-cli-metadata-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-07-05 18:36:03.581311 fichub-cli-metadata-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.573312 fichub-cli-metadata-0.6.2/tests/
+-rw-rw-rw-   0        0        0     1360 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/tests/test_cli.py
```

### Comparing `fichub-cli-metadata-0.6.1/LICENSE.txt` & `fichub-cli-metadata-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.1/PKG-INFO` & `fichub-cli-metadata-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli-metadata
-Version: 0.6.1
+Version: 0.6.2
 Summary: A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli
 Home-page: https://github.com/fichub-cli-contrib/fichub-cli-metadata
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-metadata-0.6.1/README.md` & `fichub-cli-metadata-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/__init__.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # __version__ at the top to prevent ImportError: ... partially initialized module ...
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 from .cli import app  # entry_point
```

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/cli.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,19 +157,13 @@
 
     try:
         if fic.exit_status == 1:
             typer.echo(
                 Fore.RED +
                 "\nThe CLI ran into some errors! Check the console for the log messages!" + Style.RESET_ALL)
 
-        if os.path.exists("output.log"):
-            rm_output_log = typer.confirm(
-                Fore.BLUE+"Delete the output.log?", abort=False, show_default=True)
-            if rm_output_log is True:
-                os.remove("output.log")
-
         sys.exit(fic.exit_status)
 
     # FileNotFoundError: output.log doesnt exist, when run 1st time
     # UnboundLocalError: 'fic' is not assigned value for --version flag
     except (FileNotFoundError, UnboundLocalError):
         sys.exit(0)
```

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/crud.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/crud.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import json
 from datetime import datetime
 from tqdm import tqdm
 import sys
 import os
 from colorama import Fore
 from loguru import logger
+from sqlalchemy.sql import text
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.orm import Session
 from platformdirs import PlatformDirs
 
 from . import models
 from .processing import get_ins_query, sql_to_json
 from .logging import db_not_found_log
@@ -142,15 +143,15 @@
 def add_fichub_id_column(db: Session, db_backup, debug: bool):
     """ To add a column AFTER an existing column
     """
 
     drop_TempFichubMetadata(db)
     col_exists = False
     try:
-        col_exists = db.execute("SELECT fichub_id from fichub_metadata;")
+        col_exists = db.execute(text("SELECT fichub_id from fichub_metadata;"))
         col_exists = True
     except OperationalError as e:
         if debug:
             logger.error(e)
         pass
     if not col_exists:
         tqdm.write(
@@ -158,29 +159,29 @@
         # backup the db before migrating the data
         db_backup("pre.migration")
 
         if debug:
             logger.info("Migration: adding fichub_id column")
         tqdm.write(Fore.GREEN + "Migration: adding fichub_id column")
 
-        db.execute("ALTER TABLE fichub_metadata RENAME TO TempFichubMetadata;")
-        db.execute("CREATE TABLE fichub_metadata(id INTEGER NOT NULL, fichub_id VARCHAR(255),title VARCHAR(255), author VARCHAR(255), chapters INTEGER, created VARCHAR(255), description VARCHAR(255), rated VARCHAR(255), language VARCHAR(255), genre VARCHAR(255), characters VARCHAR(255), reviews INTEGER, favs INTEGER, follows INTEGER, status VARCHAR(255), words INTEGER, last_updated VARCHAR(255), source VARCHAR(255), PRIMARY KEY(id))")
-        db.execute("INSERT INTO fichub_metadata (id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words, last_updated, source ) SELECT id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words,last_updated, source FROM TempFichubMetadata;")
-        db.execute("DROP TABLE TempFichubMetadata;")
+        db.execute(text("ALTER TABLE fichub_metadata RENAME TO TempFichubMetadata;"))
+        db.execute(text("CREATE TABLE fichub_metadata(id INTEGER NOT NULL, fichub_id VARCHAR(255),title VARCHAR(255), author VARCHAR(255), chapters INTEGER, created VARCHAR(255), description VARCHAR(255), rated VARCHAR(255), language VARCHAR(255), genre VARCHAR(255), characters VARCHAR(255), reviews INTEGER, favs INTEGER, follows INTEGER, status VARCHAR(255), words INTEGER, last_updated VARCHAR(255), source VARCHAR(255), PRIMARY KEY(id));"))
+        db.execute(text("INSERT INTO fichub_metadata (id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words, last_updated, source ) SELECT id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words,last_updated, source FROM TempFichubMetadata;"))
+        db.execute(text("DROP TABLE TempFichubMetadata;"))
         db.commit()
 
 
 def add_db_last_updated_column(db: Session, db_backup, debug: bool):
     """ To add a column AFTER an existing column
     """
 
     drop_TempFichubMetadata(db)
     col_exists = False
     try:
-        db.execute("SELECT db_last_updated from fichub_metadata;")
+        db.execute(text("SELECT db_last_updated from fichub_metadata;"))
         col_exists = True
     except OperationalError as e:
         if debug:
             logger.error(e)
         pass
     if not col_exists:
         tqdm.write(
@@ -188,28 +189,28 @@
         # backup the db before migrating the data
         db_backup("pre.migration")
 
         if debug:
             logger.info("Migration: adding db_last_updated column")
         tqdm.write(Fore.GREEN + "Migration: adding db_last_updated column")
 
-        db.execute("ALTER TABLE fichub_metadata RENAME TO TempFichubMetadata;")
-        db.execute("CREATE TABLE fichub_metadata(id INTEGER NOT NULL, fichub_id VARCHAR(255), title VARCHAR(255), author VARCHAR(255), chapters INTEGER, created VARCHAR(255), description VARCHAR(255), rated VARCHAR(255), language VARCHAR(255), genre VARCHAR(255), characters VARCHAR(255), reviews INTEGER, favs INTEGER, follows INTEGER, status VARCHAR(255), words INTEGER, fic_last_updated VARCHAR(255), db_last_updated VARCHAR(255), source VARCHAR(255), PRIMARY KEY(id))")
-        db.execute("INSERT INTO fichub_metadata (id, fichub_id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status,  words, fic_last_updated, source ) SELECT id, fichub_id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words, last_updated, source FROM TempFichubMetadata;")
-        db.execute("DROP TABLE TempFichubMetadata;")
+        db.execute(text("ALTER TABLE fichub_metadata RENAME TO TempFichubMetadata;"))
+        db.execute(text("CREATE TABLE fichub_metadata(id INTEGER NOT NULL, fichub_id VARCHAR(255), title VARCHAR(255), author VARCHAR(255), chapters INTEGER, created VARCHAR(255), description VARCHAR(255), rated VARCHAR(255), language VARCHAR(255), genre VARCHAR(255), characters VARCHAR(255), reviews INTEGER, favs INTEGER, follows INTEGER, status VARCHAR(255), words INTEGER, fic_last_updated VARCHAR(255), db_last_updated VARCHAR(255), source VARCHAR(255), PRIMARY KEY(id));"))
+        db.execute(text("INSERT INTO fichub_metadata (id, fichub_id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status,  words, fic_last_updated, source ) SELECT id, fichub_id, title, author, chapters, created, description, rated, language, genre, characters, reviews, favs, follows, status, words, last_updated, source FROM TempFichubMetadata;"))
+        db.execute(text("DROP TABLE TempFichubMetadata;"))
         db.commit()
 
 def add_rawExtendedMeta_columns(db: Session, db_backup, debug: bool):
     """ To add fic_id, author_id, author_url, fandom columns
     """
     cols_list = ['fic_id','author_id','author_url','fandom']
     for col in cols_list:
         col_exists = False
         try:
-            db.execute(f"SELECT {col} from fichub_metadata;")
+            db.execute(text(f"SELECT {col} from fichub_metadata;"))
             col_exists = True
         except OperationalError as e:
             if debug:
                 logger.error(e)
             pass
         if not col_exists:
             tqdm.write(
@@ -217,26 +218,26 @@
             # backup the db before migrating the data
             db_backup("pre.migration")
 
             if debug:
                 logger.info(f"Migration: adding {col} column")
             tqdm.write(Fore.GREEN + f"Migration: adding {col} column")
 
-            db.execute(f"ALTER TABLE fichub_metadata ADD {col} TEXT DEFAULT '';")
+            db.execute(text(f"ALTER TABLE fichub_metadata ADD {col} TEXT DEFAULT '';"))
         db.commit()
 
 
 
 def rename_favs_column(db: Session, db_backup, debug: bool):
     """ To rename favs column to favorites
     """
 
     col_exists = False
     try:
-        db.execute("SELECT favorites from fichub_metadata;")
+        db.execute(text("SELECT favorites from fichub_metadata;"))
         col_exists = True
     except OperationalError as e:
         if debug:
             logger.error(e)
         pass
     if not col_exists:
         tqdm.write(
@@ -244,16 +245,16 @@
         # backup the db before migrating the data
         db_backup("pre.migration")
 
         if debug:
             logger.info("Migration: renaming favs column to favorites")
         tqdm.write(Fore.GREEN + "Migration: renaming favs column to favorites")
 
-        db.execute("ALTER TABLE fichub_metadata RENAME COLUMN favs TO favorites;")
+        db.execute(text("ALTER TABLE fichub_metadata RENAME COLUMN favs TO favorites;"))
         db.commit()
 
 
 def drop_TempFichubMetadata(db: Session):
     try:
-        db.execute("DROP TABLE TempFichubMetadata;")
+        db.execute(text("DROP TABLE TempFichubMetadata;"))
     except OperationalError:
         pass
```

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/fetch_data.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/fetch_data.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/logging.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/logging.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright 2022 Arbaaz Laskar
-
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-
-#   http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from colorama import Fore
-from loguru import logger
-from tqdm import tqdm
-
-
-def meta_fetched_log(debug: bool, url: str):
-    if debug:
-        logger.info(f"Metadata fetched for {url}")
-    tqdm.write(Fore.GREEN + f"Metadata fetched for {url}")
-
-
-def db_not_found_log(debug: bool, input_db: str):
-    if debug:
-        logger.error(
-            f"Unable to open database file: '{input_db}'\nPlease recheck the filename!")
-    tqdm.write(
-        Fore.RED + f"Unable to open database file: '{input_db}'\nPlease recheck the filename!")
+# Copyright 2022 Arbaaz Laskar
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from colorama import Fore
+from loguru import logger
+from tqdm import tqdm
+
+
+def meta_fetched_log(debug: bool, url: str):
+    if debug:
+        logger.info(f"Metadata fetched for {url}")
+    tqdm.write(Fore.GREEN + f"Metadata fetched for {url}")
+
+
+def db_not_found_log(debug: bool, input_db: str):
+    if debug:
+        logger.error(
+            f"Unable to open database file: '{input_db}'\nPlease recheck the filename!")
+    tqdm.write(
+        Fore.RED + f"Unable to open database file: '{input_db}'\nPlease recheck the filename!")
```

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/models.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/models.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata/utils/processing.py` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/processing.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/PKG-INFO` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli-metadata
-Version: 0.6.1
+Version: 0.6.2
 Summary: A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli
 Home-page: https://github.com/fichub-cli-contrib/fichub-cli-metadata
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-metadata-0.6.1/fichub_cli_metadata.egg-info/SOURCES.txt` & `fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 fichub_cli_metadata.egg-info/requires.txt
 fichub_cli_metadata.egg-info/top_level.txt
 fichub_cli_metadata/utils/__init__.py
 fichub_cli_metadata/utils/crud.py
 fichub_cli_metadata/utils/fetch_data.py
 fichub_cli_metadata/utils/logging.py
 fichub_cli_metadata/utils/models.py
-fichub_cli_metadata/utils/processing.py
+fichub_cli_metadata/utils/processing.py
+tests/test_cli.py
```

### Comparing `fichub-cli-metadata-0.6.1/setup.py` & `fichub-cli-metadata-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     name='fichub-cli-metadata',
     author='Arbaaz Laskar',
     author_email="arzkar.dev@gmail.com",
     description="A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.6.1',
+    version='0.6.2',
     license='Apache License',
     url="https://github.com/fichub-cli-contrib/fichub-cli-metadata",
     packages=find_packages(
         include=['fichub_cli_metadata', 'fichub_cli_metadata.*']),
     include_package_data=True,
     install_requires=[
         'fichub-cli>=0.8.2',
```

