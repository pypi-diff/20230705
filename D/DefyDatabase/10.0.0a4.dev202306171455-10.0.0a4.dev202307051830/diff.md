# Comparing `tmp/DefyDatabase-10.0.0a4.dev202306171455.tar.gz` & `tmp/DefyDatabase-10.0.0a4.dev202307051830.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202306171455.tar", last modified: Sat Jun 17 06:55:14 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a4.dev202307051830.tar", last modified: Wed Jul  5 10:28:54 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202306171455.tar` & `DefyDatabase-10.0.0a4.dev202307051830.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/
-drwxrwxrwx   0        0        0        0 2023-06-17 06:55:14.765924 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202306171455/README.md
--rw-rw-rw-   0        0        0     5625 2023-06-17 06:53:04.000000 DefyDatabase-10.0.0a4.dev202306171455/defy.py
--rw-rw-rw-   0        0        0       42 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202306171455/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:28:54.272289 DefyDatabase-10.0.0a4.dev202307051830/
+drwxrwxrwx   0        0        0        0 2023-07-05 10:28:54.271292 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 10:28:54.000000 DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-07-05 10:28:54.272289 DefyDatabase-10.0.0a4.dev202307051830/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202307051830/README.md
+-rw-rw-rw-   0        0        0     2757 2023-07-05 10:28:28.000000 DefyDatabase-10.0.0a4.dev202307051830/defy.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:28:54.273223 DefyDatabase-10.0.0a4.dev202307051830/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202307051830/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307051830/DefyDatabase.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202306171455
+Version: 10.0.0a4.dev202307051830
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171455/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202307051830/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202306171455
+Version: 10.0.0a4.dev202307051830
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171455/setup.py` & `DefyDatabase-10.0.0a4.dev202307051830/setup.py`

 * *Files identical despite different names*

