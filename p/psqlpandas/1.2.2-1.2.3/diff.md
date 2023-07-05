# Comparing `tmp/psqlpandas-1.2.2.tar.gz` & `tmp/psqlpandas-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.2.2.tar", max compression
+gzip compressed data, was "psqlpandas-1.2.3.tar", max compression
```

## Comparing `psqlpandas-1.2.2.tar` & `psqlpandas-1.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      900 2023-07-05 10:43:11.118842 psqlpandas-1.2.2/LICENSE
--rw-r--r--   0        0        0      199 2023-07-05 10:43:11.118842 psqlpandas-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-05 10:43:11.142842 psqlpandas-1.2.2/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 10:43:11.119842 psqlpandas-1.2.2/psqlpandas/__version__.py
--rw-r--r--   0        0        0     7944 2023-07-05 10:43:11.119842 psqlpandas-1.2.2/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-07-05 10:43:11.119842 psqlpandas-1.2.2/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     3091 2023-07-05 10:43:11.120842 psqlpandas-1.2.2/psqlpandas/tables.py
--rw-r--r--   0        0        0     1909 2023-07-05 10:43:11.120842 psqlpandas-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.2.2/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-05 11:04:01.409203 psqlpandas-1.2.3/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-05 11:04:01.409203 psqlpandas-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 11:04:01.434203 psqlpandas-1.2.3/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     7939 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     3091 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/psqlpandas/tables.py
+-rw-r--r--   0        0        0     1909 2023-07-05 11:04:01.410203 psqlpandas-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 psqlpandas-1.2.3/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 psqlpandas-1.2.3/PKG-INFO
```

### Comparing `psqlpandas-1.2.2/LICENSE` & `psqlpandas-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.2/psqlpandas/postgresql.py` & `psqlpandas-1.2.3/psqlpandas/postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         # Update if there are data already
         if replace:
             # Query from https://wiki.postgresql.org/wiki/Retrieve_primary_key_columns
             primary_keys_sql = (
                 f"SELECT a.attname FROM pg_index i JOIN pg_attribute a ON a.attrelid = i.indrelid AND "
                 f"a.attnum = ANY(i.indkey) WHERE i.indrelid = '{tablename}'::regclass AND i.indisprimary;"
             )
-            primary_keys = list(self.read_from_db(primary_keys_sql))
+            primary_keys = list(self.read_df(primary_keys_sql))
             columns_to_update = [x for x in df_columns if x not in primary_keys]
             insertsql = (
                 insertsql
                 + " ON CONFLICT ON CONSTRAINT "
                 + tablename
                 + "_pkey DO UPDATE SET ("
                 + ",".join([column for column in columns_to_update])
```

### Comparing `psqlpandas-1.2.2/psqlpandas/tables.py` & `psqlpandas-1.2.3/psqlpandas/tables.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.2/pyproject.toml` & `psqlpandas-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.2.2"
+version = "1.2.3"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
```

### Comparing `psqlpandas-1.2.2/setup.py` & `psqlpandas-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.24.2,<2.0.0',
  'pandas>=2.0.1,<3.0.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '1.2.2',
+    'version': '1.2.3',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-1.2.2/PKG-INFO` & `psqlpandas-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.2.2
+Version: 1.2.3
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

