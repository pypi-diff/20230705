# Comparing `tmp/dbt-glue-1.5.1.tar.gz` & `tmp/dbt-glue-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.5.1.tar", last modified: Mon Jul  3 08:14:25 2023, max compression
+gzip compressed data, was "dbt-glue-1.5.2.tar", last modified: Wed Jul  5 15:17:39 2023, max compression
```

## Comparing `dbt-glue-1.5.1.tar` & `dbt-glue-1.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.201209 dbt-glue-1.5.1/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-03 08:14:25.201053 dbt-glue-1.5.1/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.5.1/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194167 dbt-glue-1.5.1/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.193998 dbt-glue-1.5.1/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.196665 dbt-glue-1.5.1/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.1/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-03 08:13:38.000000 dbt-glue-1.5.1/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.1/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2524 2023-06-29 08:38:08.000000 dbt-glue-1.5.1/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.197480 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     9695 2023-07-03 08:12:14.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    36786 2023-06-29 09:26:37.000000 dbt-glue-1.5.1/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.1/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194221 dbt-glue-1.5.1/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198192 dbt-glue-1.5.1/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.1/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198349 dbt-glue-1.5.1/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.1/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.198687 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199159 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199493 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199670 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.1/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.194783 dbt-glue-1.5.1/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.199847 dbt-glue-1.5.1/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.1/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-03 08:14:25.200782 dbt-glue-1.5.1/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.1/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-03 08:14:25.000000 dbt-glue-1.5.1/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-03 08:14:25.201255 dbt-glue-1.5.1/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.1/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.215136 dbt-glue-1.5.2/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-05 15:17:39.214978 dbt-glue-1.5.2/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206639 dbt-glue-1.5.2/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206338 dbt-glue-1.5.2/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.209743 dbt-glue-1.5.2/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.2/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-07-05 12:00:28.000000 dbt-glue-1.5.2/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.2/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2585 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.210597 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     9695 2023-07-05 15:16:41.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8225 2023-07-05 15:09:54.000000 dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    38143 2023-07-05 15:12:32.000000 dbt-glue-1.5.2/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.2/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.206747 dbt-glue-1.5.2/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211117 dbt-glue-1.5.2/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.2/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211353 dbt-glue-1.5.2/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.2/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.211842 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.212517 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213072 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2023-07-05 12:59:31.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213235 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.2/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.207375 dbt-glue-1.5.2/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.213416 dbt-glue-1.5.2/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.2/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-07-05 15:17:39.214594 dbt-glue-1.5.2/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.2/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-07-05 15:17:39.000000 dbt-glue-1.5.2/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-07-05 15:17:39.215198 dbt-glue-1.5.2/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.2/setup.py
```

### Comparing `dbt-glue-1.5.1/LICENSE` & `dbt-glue-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/PKG-INFO` & `dbt-glue-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.1
+Version: 1.5.2
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -237,15 +237,15 @@
 | role_arn	                               | The ARN of the glue interactive session IAM role.	                                                                                                                                                                                                                                                |yes|
 | region	                                 | The AWS Region were you run the data pipeline.	                                                                                                                                                                                                                                                   |yes|
 | workers	                                | The number of workers of a defined workerType that are allocated when a job runs.	                                                                                                                                                                                                                |yes|
 | worker_type	                            | The type of predefined worker that is allocated when a job runs. Accepts a value of Standard, G.1X, or G.2X.	                                                                                                                                                                                     |yes|
 | schema	                                 | The schema used to organize data stored in Amazon S3.Additionally, is the database in AWS Lake Formation that stores metadata tables in the Data Catalog.	                                                                                                                                        |yes|
 | session_provisioning_timeout_in_seconds | The timeout in seconds for AWS Glue interactive session provisioning.	                                                                                                                                                                                                                            |yes|
 | location	                               | The Amazon S3 location of your target data.	                                                                                                                                                                                                                                                      |yes|
-| query_timeout_in_seconds	               | The timeout in seconds for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
+| query_timeout_in_minutes	               | The timeout in minutes for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
 | idle_timeout	                           | The AWS Glue session idle timeout in minutes. (The session stops after being idle for the specified amount of time)	                                                                                                                                                                              |no|
 | glue_version	                           | The version of AWS Glue for this session to use. Currently, the only valid options are 2.0 and 3.0. The default value is 3.0.	                                                                                                                                                                    |no|
 | security_configuration	                 | The security configuration to use with this session.	                                                                                                                                                                                                                                             |no|
 | connections	                            | A comma-separated list of connections to use in the session.	                                                                                                                                                                                                                                     |no|
 | conf	                                   | Specific configuration used at the startup of the Glue Interactive Session (arg --conf)	                                                                                                                                                                                                          |no|
 | extra_py_files	                         | Extra python Libs that can be used by the interactive session.                                                                                                                                                                                                                                    |no|
 | delta_athena_prefix	                    | A prefix used to create Athena compatible tables for Delta tables	(if not specified, then no Athena compatible table will be created)                                                                                                                                                             |no|
```

### Comparing `dbt-glue-1.5.1/README.md` & `dbt-glue-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 | role_arn	                               | The ARN of the glue interactive session IAM role.	                                                                                                                                                                                                                                                |yes|
 | region	                                 | The AWS Region were you run the data pipeline.	                                                                                                                                                                                                                                                   |yes|
 | workers	                                | The number of workers of a defined workerType that are allocated when a job runs.	                                                                                                                                                                                                                |yes|
 | worker_type	                            | The type of predefined worker that is allocated when a job runs. Accepts a value of Standard, G.1X, or G.2X.	                                                                                                                                                                                     |yes|
 | schema	                                 | The schema used to organize data stored in Amazon S3.Additionally, is the database in AWS Lake Formation that stores metadata tables in the Data Catalog.	                                                                                                                                        |yes|
 | session_provisioning_timeout_in_seconds | The timeout in seconds for AWS Glue interactive session provisioning.	                                                                                                                                                                                                                            |yes|
 | location	                               | The Amazon S3 location of your target data.	                                                                                                                                                                                                                                                      |yes|
-| query_timeout_in_seconds	               | The timeout in seconds for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
+| query_timeout_in_minutes	               | The timeout in minutes for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
 | idle_timeout	                           | The AWS Glue session idle timeout in minutes. (The session stops after being idle for the specified amount of time)	                                                                                                                                                                              |no|
 | glue_version	                           | The version of AWS Glue for this session to use. Currently, the only valid options are 2.0 and 3.0. The default value is 3.0.	                                                                                                                                                                    |no|
 | security_configuration	                 | The security configuration to use with this session.	                                                                                                                                                                                                                                             |no|
 | connections	                            | A comma-separated list of connections to use in the session.	                                                                                                                                                                                                                                     |no|
 | conf	                                   | Specific configuration used at the startup of the Glue Interactive Session (arg --conf)	                                                                                                                                                                                                          |no|
 | extra_py_files	                         | Extra python Libs that can be used by the interactive session.                                                                                                                                                                                                                                    |no|
 | delta_athena_prefix	                    | A prefix used to create Athena compatible tables for Delta tables	(if not specified, then no Athena compatible table will be created)                                                                                                                                                             |no|
```

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/connections.py` & `dbt-glue-1.5.2/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/credentials.py` & `dbt-glue-1.5.2/dbt/adapters/glue/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,28 @@
     region: str
     workers: int
     worker_type: str
     session_provisioning_timeout_in_seconds: int = 120
     location: Optional[str] = None
     extra_jars: Optional[str] = None
     idle_timeout: int = 10
-    query_timeout_in_seconds: int = 300
+    query_timeout_in_minutes: int = 300
     glue_version: Optional[str] = "3.0"
     security_configuration: Optional[str] = None
     connections: Optional[str] = None
     conf: Optional[str] = None
     extra_py_files: Optional[str] = None
     delta_athena_prefix: Optional[str] = None
     tags: Optional[str] = None
     database: Optional[str] # type: ignore
     seed_format: Optional[str] = "parquet"
     seed_mode: Optional[str] = "overwrite"
     default_arguments: Optional[str] = None
     iceberg_glue_commit_lock_table: Optional[str] = "myGlueLockTable"
+    use_interactive_session_role_for_api_calls: bool = False
 
     @property
     def type(self):
         return "glue"
 
     @property
     def unique_field(self):
@@ -62,15 +63,15 @@
             'workers',
             'worker_type',
             'session_provisioning_timeout_in_seconds',
             'schema',
             'location',
             'extra_jars',
             'idle_timeout',
-            'query_timeout_in_seconds',
+            'query_timeout_in_minutes',
             'glue_version',
             'security_configuration',
             'connections',
             'conf',
             'extra_py_files',
             'delta_athena_prefix',
             'tags',
```

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         if (self.credentials.extra_py_files is not None):
             args["--extra-py-files"] = f"{self.credentials.extra_py_files}"
 
         additional_args = {}
         additional_args["NumberOfWorkers"] = self.credentials.workers
         additional_args["WorkerType"] = self.credentials.worker_type
         additional_args["IdleTimeout"] = self.credentials.idle_timeout
-        additional_args["Timeout"] = self.credentials.query_timeout_in_seconds
+        additional_args["Timeout"] = self.credentials.query_timeout_in_minutes
         additional_args["RequestOrigin"] = 'dbt-glue'
         
         if (self.credentials.glue_version is not None):
             additional_args["GlueVersion"] = f"{self.credentials.glue_version}"
         
         if (self.credentials.security_configuration is not None):
             additional_args["SecurityConfiguration"] = f"{self.credentials.security_configuration}"
```

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.5.2/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dbt.contracts.connection import AdapterResponse
 from dbt import exceptions as dbterrors
 from dbt.adapters.glue.gluedbapi.commons import GlueStatement
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("Glue")
 
+
 class GlueCursorState:
     WAITING = "WAITING"
     RUNNING = "RUNNING"
     AVAILABLE = "AVAILABLE"
     CANCELLING = "CANCELLING"
     CANCELLED = "CANCELLED"
     TIMEOUT = "TIMEOUT"
@@ -114,26 +115,26 @@
                         logger.debug(f"chunks: {chunks}")
                         self.response = json.loads(chunks[0])
                         logger.debug(f"response: {response}")
                     except Exception as ex:
                         logger.error("Could not parse " + json.loads(chunks[0]), ex)
                         self.state = GlueCursorState.ERROR
             else:
-                error_message=f"Glue returned `{status}` for statement {self.statement_id} for code {self.code}, {output.get('ErrorName')}: {output.get('ErrorValue')}"
+                error_message = f"Glue returned `{status}` for statement {self.statement_id} for code {self.code}, {output.get('ErrorName')}: {output.get('ErrorValue')}"
                 if output.get('ErrorValue').find("is not a view"):
                     self.state = GlueCursorState.ERROR
                     logger.error(error_message)
                 else:
                     logger.debug(error_message)
                     raise dbterrors.DbtDatabaseError(msg=error_message)
 
         if self.state == GlueCursorState.ERROR:
             self._post()
             output = response.get("Statement", {}).get("Output", {})
-            error_message=f"Glue cursor returned `{output.get('Status')}` for statement {self.statement_id} for code {self.code}, {output.get('ErrorName')}: {output.get('ErrorValue')}"
+            error_message = f"Glue cursor returned `{output.get('Status')}` for statement {self.statement_id} for code {self.code}, {output.get('ErrorName')}: {output.get('ErrorValue')}"
             logger.debug(error_message)
             raise dbterrors.DbtDatabaseError(msg=error_message)
 
         if self.state in [GlueCursorState.CANCELLED, GlueCursorState.CANCELLING]:
             self._post()
             raise dbterrors.DbtDatabaseError(
                 msg=f"Statement {self.connection.session_id}.{self.statement_id} cancelled.")
@@ -141,15 +142,14 @@
         logger.debug("GlueCursor execute successfully")
         return self.response
 
     @property
     def columns(self):
         if self.response:
             return [column.get("name") for column in self.response.get("description")]
-        
 
     def fetchall(self):
         logger.debug("GlueCursor fetchall called")
         if self.closed:
             raise Exception("CursorClosed")
 
         if self.response:
```

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/impl.py` & `dbt-glue-1.5.2/dbt/adapters/glue/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,32 @@
 
     @classmethod
     def convert_datetime_type(cls, agate_table, col_idx):
         return "timestamp"
 
     def get_connection(self):
         connection: GlueConnectionManager = self.connections.get_thread_connection()
-        session: GlueConnection = connection.handle
-        client = boto3.client("glue", region_name=session.credentials.region)
+        glueSession: GlueConnection = connection.handle
+        if glueSession.credentials.role_arn is not None:
+            if glueSession.credentials.use_interactive_session_role_for_api_calls is True:
+                sts_client = boto3.client('sts')
+                assumed_role_object = sts_client.assume_role(
+                    RoleArn=glueSession.credentials.role_arn,
+                    RoleSessionName="dbt"
+                )
+                credentials = assumed_role_object['Credentials']
+                session = boto3.Session(
+                    aws_access_key_id=credentials['AccessKeyId'],
+                    aws_secret_access_key=credentials['SecretAccessKey'],
+                    aws_session_token=credentials['SessionToken']
+                )
 
-        return session, client
+        client = boto3.client("glue", region_name=glueSession.credentials.region)
+
+        return glueSession, client
 
     def list_schemas(self, database: str) -> List[str]:
         session, client = self.get_connection()
         responseGetDatabases = client.get_databases()
         databaseList = responseGetDatabases['DatabaseList']
         schemas = []
         for databaseDict in databaseList:
@@ -199,35 +213,53 @@
                 .config(f"spark.sql.catalog.glue_catalog.catalog-impl", "org.apache.iceberg.aws.glue.GlueCatalog") \
                 .config(f"spark.sql.catalog.glue_catalog.io-impl", "org.apache.iceberg.aws.s3.S3FileIO") \
                 .config(f"spark.sql.catalog.glue_catalog.lock-impl", "org.apache.iceberg.aws.glue.DynamoLockManager") \
                 .config(f"spark.sql.catalog.glue_catalog.lock.table", dynamodb_table) \
                 .config("spark.sql.extensions", "org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions") \
                 .getOrCreate()
             SqlWrapper2.execute("""describe glue_catalog.{relation.schema}.{relation.name}""")'''
-        else : 
+        else:
             code = f'''describe {relation.schema}.{relation.identifier}'''
         columns = []
         try:
-            session.cursor().execute(code)
-            for record in session.cursor().fetchall():
+            response = session.cursor().execute(code)
+            records = self.fetch_all_response(response)
+
+            for record in records:
                 column = Column(column=record[0], dtype=record[1])
                 if record[0][:1] != "#":
                     if column not in columns:
                         columns.append(column)
+
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueGetColumnsInRelationFailed") from e
         except Exception as e:
             logger.error(e)
 
+        logger.debug("columns before strip:")
+        logger.debug(columns)
         # strip hudi metadata columns.
         columns = [x for x in columns
                    if x.name not in self.HUDI_METADATA_COLUMNS]
 
+        logger.debug("columns after strip:")
+        logger.debug(columns)
+
         return columns
-    
+
+    def fetch_all_response(self, response):
+        records = []
+        obj_columns = [column.get("name") for column in response.get("description")]
+        for item in response.get("results", []):
+            record = []
+            for column in obj_columns:
+                record.append(item.get("data", {}).get(column, None))
+            records.append(record)
+        return records
+
     def set_table_properties(self, table_properties):
         if table_properties=='empty':
             return ""
         else:
             table_properties_formatted = []
             for key in table_properties : 
                 table_properties_formatted.append("'" + key + "'='" + table_properties[key] + "'")
@@ -243,16 +275,17 @@
         return ' AND '.join(['t.{} = s.{}'.format(field, field) for field in merge_key])
             
     @available
     def duplicate_view(self, from_relation: BaseRelation, to_relation: BaseRelation, ):
         session, client = self.get_connection()
         code = f'''SHOW CREATE TABLE {from_relation.schema}.{from_relation.identifier}'''
         try:
-            session.cursor().execute(code)
-            for record in session.cursor().fetchall():
+            response = session.cursor().execute(code)
+            records = self.fetch_all_response(response)
+            for record in records:
                 create_view_statement = record[0]
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueDuplicateViewFailed") from e
         except Exception as e:
             logger.error(e)
         target_query = create_view_statement.replace(from_relation.schema, to_relation.schema)
         target_query = target_query.replace(from_relation.identifier, to_relation.identifier)
```

### Comparing `dbt-glue-1.5.1/dbt/adapters/glue/relation.py` & `dbt-glue-1.5.2/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% macro get_insert_overwrite_sql(source_relation, target_relation) %}
-    {%- set dest_columns = adapter.get_columns_in_relation(target_relation) -%}
+    {%- set dest_columns = adapter.get_columns_in_relation(source_relation) -%}
     {%- set dest_cols_csv = dest_columns | map(attribute='name') | join(', ') -%}
     set hive.exec.dynamic.partition.mode=nonstrict
     dbt_next_query
     insert overwrite table {{ target_relation }}
     {{ partition_cols(label="partition") }}
     select {{dest_cols_csv}} from {{ source_relation }}
 {% endmacro %}
```

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.5.2/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.5.2/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.5.2/dbt_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.5.1
+Version: 1.5.2
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -237,15 +237,15 @@
 | role_arn	                               | The ARN of the glue interactive session IAM role.	                                                                                                                                                                                                                                                |yes|
 | region	                                 | The AWS Region were you run the data pipeline.	                                                                                                                                                                                                                                                   |yes|
 | workers	                                | The number of workers of a defined workerType that are allocated when a job runs.	                                                                                                                                                                                                                |yes|
 | worker_type	                            | The type of predefined worker that is allocated when a job runs. Accepts a value of Standard, G.1X, or G.2X.	                                                                                                                                                                                     |yes|
 | schema	                                 | The schema used to organize data stored in Amazon S3.Additionally, is the database in AWS Lake Formation that stores metadata tables in the Data Catalog.	                                                                                                                                        |yes|
 | session_provisioning_timeout_in_seconds | The timeout in seconds for AWS Glue interactive session provisioning.	                                                                                                                                                                                                                            |yes|
 | location	                               | The Amazon S3 location of your target data.	                                                                                                                                                                                                                                                      |yes|
-| query_timeout_in_seconds	               | The timeout in seconds for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
+| query_timeout_in_minutes	               | The timeout in minutes for a signle query. Default is 300                                                                                                                                                                                                                                         |no|
 | idle_timeout	                           | The AWS Glue session idle timeout in minutes. (The session stops after being idle for the specified amount of time)	                                                                                                                                                                              |no|
 | glue_version	                           | The version of AWS Glue for this session to use. Currently, the only valid options are 2.0 and 3.0. The default value is 3.0.	                                                                                                                                                                    |no|
 | security_configuration	                 | The security configuration to use with this session.	                                                                                                                                                                                                                                             |no|
 | connections	                            | A comma-separated list of connections to use in the session.	                                                                                                                                                                                                                                     |no|
 | conf	                                   | Specific configuration used at the startup of the Glue Interactive Session (arg --conf)	                                                                                                                                                                                                          |no|
 | extra_py_files	                         | Extra python Libs that can be used by the interactive session.                                                                                                                                                                                                                                    |no|
 | delta_athena_prefix	                    | A prefix used to create Athena compatible tables for Delta tables	(if not specified, then no Athena compatible table will be created)                                                                                                                                                             |no|
```

### Comparing `dbt-glue-1.5.1/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.5.2/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.5.1/setup.py` & `dbt-glue-1.5.2/setup.py`

 * *Files identical despite different names*

