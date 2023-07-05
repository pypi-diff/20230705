# Comparing `tmp/pipelinewise-tap-mysql-1.5.4.tar.gz` & `tmp/pipelinewise-tap-mysql-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-mysql-1.5.4.tar", last modified: Mon May 22 15:06:18 2023, max compression
+gzip compressed data, was "pipelinewise-tap-mysql-1.5.5.tar", last modified: Wed Jul  5 10:04:32 2023, max compression
```

## Comparing `pipelinewise-tap-mysql-1.5.4.tar` & `pipelinewise-tap-mysql-1.5.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/tap_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/discover_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/binlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:32.012774 pipelinewise-tap-mysql-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-07-05 10:04:32.012774 pipelinewise-tap-mysql-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:32.008774 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 10:04:31.000000 pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:04:32.012774 pipelinewise-tap-mysql-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:32.008774 pipelinewise-tap-mysql-1.5.5/tap_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/discover_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:32.012774 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/binlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-05 10:04:23.000000 pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/incremental.py
```

### Comparing `pipelinewise-tap-mysql-1.5.4/LICENSE` & `pipelinewise-tap-mysql-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/PKG-INFO` & `pipelinewise-tap-mysql-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.4
+Version: 1.5.5
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `pipelinewise-tap-mysql-1.5.4/README.md` & `pipelinewise-tap-mysql-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/PKG-INFO` & `pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.4
+Version: 1.5.5
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/SOURCES.txt` & `pipelinewise-tap-mysql-1.5.5/pipelinewise_tap_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/setup.py` & `pipelinewise-tap-mysql-1.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pipelinewise-tap-mysql',
-      version='1.5.4',
+      version='1.5.5',
       description='Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-mysql',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=['tap_mysql'],
       install_requires=[
           'pendulum==2.1.2',
           'pipelinewise-singer-python==1.*',
-          'PyMySQL==1.0.2',
+          'PyMySQL==1.1.*',
           'mysql-replication==0.40',
-          'plpygis==0.2.0',
+          'plpygis==0.2.1',
           'tzlocal==2.1',
       ],
       extras_require={
           'test': [
               'nose==1.3.*',
               'pylint==2.13.2',
               'nose-cov==1.6'
```

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/__init__.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/connection.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/connection.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/discover_utils.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/discover_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/stream_utils.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/binlog.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/binlog.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/common.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/full_table.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/incremental.py` & `pipelinewise-tap-mysql-1.5.5/tap_mysql/sync_strategies/incremental.py`

 * *Files identical despite different names*

