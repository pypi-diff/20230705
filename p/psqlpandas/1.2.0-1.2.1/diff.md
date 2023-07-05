# Comparing `tmp/psqlpandas-1.2.0.tar.gz` & `tmp/psqlpandas-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.2.0.tar", max compression
+gzip compressed data, was "psqlpandas-1.2.1.tar", max compression
```

## Comparing `psqlpandas-1.2.0.tar` & `psqlpandas-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      900 2023-07-04 08:14:29.551749 psqlpandas-1.2.0/LICENSE
--rw-r--r--   0        0        0      199 2023-07-04 08:14:29.551749 psqlpandas-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-04 08:14:29.576748 psqlpandas-1.2.0/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 08:14:29.552749 psqlpandas-1.2.0/psqlpandas/__version__.py
--rw-r--r--   0        0        0     7944 2023-07-04 08:14:29.552749 psqlpandas-1.2.0/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-07-04 08:14:29.552749 psqlpandas-1.2.0/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     3065 2023-07-04 08:14:29.553749 psqlpandas-1.2.0/psqlpandas/tables.py
--rw-r--r--   0        0        0     1909 2023-07-04 08:14:29.553749 psqlpandas-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.2.0/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-05 10:36:15.858773 psqlpandas-1.2.1/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-05 10:36:15.859773 psqlpandas-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 10:36:15.883773 psqlpandas-1.2.1/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-05 10:36:15.859773 psqlpandas-1.2.1/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     7944 2023-07-05 10:36:15.860773 psqlpandas-1.2.1/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-07-05 10:36:15.860773 psqlpandas-1.2.1/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     3075 2023-07-05 10:36:15.860773 psqlpandas-1.2.1/psqlpandas/tables.py
+-rw-r--r--   0        0        0     1909 2023-07-05 10:36:15.860773 psqlpandas-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.2.1/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.2.1/PKG-INFO
```

### Comparing `psqlpandas-1.2.0/LICENSE` & `psqlpandas-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.0/psqlpandas/postgresql.py` & `psqlpandas-1.2.1/psqlpandas/postgresql.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.0/psqlpandas/tables.py` & `psqlpandas-1.2.1/psqlpandas/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     Args:
         table_info (Dict[str, object]): dictionary containing the table specifications
         db_connector (psql.PostgresqlDatabaseConnector): connector to the db
         data (pd.DataFrame): data
     """
 
-    if not initialize_table_checks():
+    if not initialize_table_checks(table_info):
         return False
 
     tablename = table_info["tablename"]
 
     # Drop table
     if table_info["drop_if_exists"]:
         db_connector.execute_sql_query(drop_table_query(tablename))
```

### Comparing `psqlpandas-1.2.0/pyproject.toml` & `psqlpandas-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.2.0"
+version = "1.2.1"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
```

### Comparing `psqlpandas-1.2.0/setup.py` & `psqlpandas-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-1.2.0/PKG-INFO` & `psqlpandas-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.2.0
+Version: 1.2.1
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

