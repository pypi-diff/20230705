# Comparing `tmp/git_remote_oracle-0.0.1.tar.gz` & `tmp/git_remote_oracle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_remote_oracle-0.0.1.tar", last modified: Sun Jul  2 13:27:29 2023, max compression
+gzip compressed data, was "git_remote_oracle-0.0.2.tar", last modified: Wed Jul  5 15:02:02 2023, max compression
```

## Comparing `git_remote_oracle-0.0.1.tar` & `git_remote_oracle-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:27:29.462969 git_remote_oracle-0.0.1/
--rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git_remote_oracle-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-02 13:27:29.462969 git_remote_oracle-0.0.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      233 2023-07-02 09:48:14.000000 git_remote_oracle-0.0.1/README.md
--rwxr-xr-x   0 root         (0) root         (0)      709 2023-07-02 13:22:49.000000 git_remote_oracle-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 13:27:29.462969 git_remote_oracle-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:27:29.452969 git_remote_oracle-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:27:29.462969 git_remote_oracle-0.0.1/src/git_remote_oracle/
--rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git_remote_oracle-0.0.1/src/git_remote_oracle/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7724 2023-07-02 13:15:57.000000 git_remote_oracle-0.0.1/src/git_remote_oracle/git_remote_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 13:27:29.462969 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-02 13:27:29.000000 git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/
+-rwxr-xr-x   0 root         (0) root         (0)     1066 2023-06-24 07:23:36.000000 git_remote_oracle-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      233 2023-07-02 09:48:14.000000 git_remote_oracle-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 15:02:02.000000 git_remote_oracle-0.0.2/git_remote_oracle.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)      764 2023-07-05 14:58:34.000000 git_remote_oracle-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.703360 git_remote_oracle-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 15:02:02.713360 git_remote_oracle-0.0.2/src/git_remote_oracle/
+-rwxr-xr-x   0 root         (0) root         (0)      113 2023-07-02 13:25:58.000000 git_remote_oracle-0.0.2/src/git_remote_oracle/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7868 2023-07-03 15:40:27.000000 git_remote_oracle-0.0.2/src/git_remote_oracle/git_remote_oracle.py
```

### Comparing `git_remote_oracle-0.0.1/LICENSE` & `git_remote_oracle-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_remote_oracle-0.0.1/PKG-INFO` & `git_remote_oracle-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_remote_oracle
-Version: 0.0.1
+Version: 0.0.2
 Summary: A git remote helper to pull package source from oracle database.
 Author-email: CrazyT <crazyt2019+gro@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/git-remote-oracle
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/git-remote-oracle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `git_remote_oracle-0.0.1/pyproject.toml` & `git_remote_oracle-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61"]
 
 [project]
 name = "git_remote_oracle"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="CrazyT", email="crazyt2019+gro@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -21,8 +21,11 @@
 ]
 
 [project.scripts]
 git-remote-oracle = "git_remote_oracle:main_cli"
 
 [project.urls]
 "Homepage" = "https://github.com/TheCrazyT/git-remote-oracle"
-"Bug Tracker" = "https://github.com/TheCrazyT/git-remote-oracle/issues"
+"Bug Tracker" = "https://github.com/TheCrazyT/git-remote-oracle/issues"
+
+[tool.setuptools.packages.find]
+exclude = ["*.ipynb"]
```

### Comparing `git_remote_oracle-0.0.1/src/git_remote_oracle/git_remote_oracle.py` & `git_remote_oracle-0.0.2/src/git_remote_oracle/git_remote_oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,43 +149,50 @@
     with open(last_ddl_path, 'r') as f:
       last_ddl = f.read()
       last_ddl_time = datetime.strptime(last_ddl, DATETIME_FORMAT)
   dbg(f"last_ddl_time: {last_ddl_time}")
   file_list = []
   qry = """
     SELECT 
-      OBJECT_ID,
-      OBJECT_NAME,
-      OWNER,
-      OBJECT_TYPE,
-      DBMS_METADATA.GET_DDL(REPLACE(object_type,' ','_'), object_name, UPPER(:2)) AS DDL
+      object_id,
+      object_name,
+      owner,
+      object_type,
+      DBMS_METADATA.GET_DDL(REPLACE(DECODE(
+							object_type,
+							'PACKAGE','PACKAGE SPEC',
+							'TYPE','TYPE SPEC',
+							'JOB','PROCOBJ',
+							object_type 
+						),' ','_'), object_name, UPPER(:2)) AS DDL
     FROM all_objects
     WHERE 
-      lower(OWNER) = lower(:1)
-      AND OBJECT_TYPE IN (
+      lower(owner) = lower(:1)
+      AND object_type IN (
         'PACKAGE',
         'PACKAGE BODY',
+        'TRIGGER',
         'VIEW',
         'TABLE',
         'PROCEDURE',
         'FUNCTION',
         'INDEX',
         'TYPE',
         'TYPE BODY',
         'SYNONYM',
-        -- 'JOB',
+        'JOB',
         'JAVA SOURCE',
         'JAVA RESOURCE'
       )
-      AND SHARING <> 'METADATA LINK'
-      AND LAST_DDL_TIME > :3
-      AND GENERATED = 'N'
-      AND TEMPORARY = 'N'
-      AND ORACLE_MAINTAINED = 'N'
-    ORDER BY OBJECT_ID
+      AND sharing <> 'METADATA LINK'
+      AND last_ddl_time > :3
+      AND generated = 'N'
+      AND temporary = 'N'
+      AND oracle_maintained = 'N'
+    ORDER BY object_id
     """
   dbg(f"qry: {qry}")
   for object_id, object_name, owner, object_type, ddl in cursor.execute(qry, [schema, username, last_ddl_time]):
     #print(object_name)
     #print(ddl)
     ddl_str = ddl.read()
     dbg(f"object_name: {object_name}")
```

### Comparing `git_remote_oracle-0.0.1/src/git_remote_oracle.egg-info/PKG-INFO` & `git_remote_oracle-0.0.2/git_remote_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-remote-oracle
-Version: 0.0.1
+Version: 0.0.2
 Summary: A git remote helper to pull package source from oracle database.
 Author-email: CrazyT <crazyt2019+gro@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/git-remote-oracle
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/git-remote-oracle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

