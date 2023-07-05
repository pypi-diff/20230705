# Comparing `tmp/DataPipelineExecutor-0.0.2.tar.gz` & `tmp/DataPipelineExecutor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataPipelineExecutor-0.0.2.tar", last modified: Wed Jul  5 09:21:25 2023, max compression
+gzip compressed data, was "DataPipelineExecutor-0.0.3.tar", last modified: Wed Jul  5 09:27:30 2023, max compression
```

## Comparing `DataPipelineExecutor-0.0.2.tar` & `DataPipelineExecutor-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 09:21:25.049319 DataPipelineExecutor-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-06-30 09:37:05.000000 DataPipelineExecutor-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2724 2023-07-05 09:21:25.047079 DataPipelineExecutor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2267 2023-07-05 09:16:38.000000 DataPipelineExecutor-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 09:21:25.049319 DataPipelineExecutor-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      586 2023-07-05 09:21:13.000000 DataPipelineExecutor-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 09:21:25.042305 DataPipelineExecutor-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 09:21:25.047079 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/
--rw-rw-rw-   0        0        0     2724 2023-07-05 09:21:24.000000 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-05 09:21:24.000000 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 09:21:24.000000 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-05 09:21:24.000000 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35008 2023-07-03 14:23:59.000000 DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.py
+drwxrwxrwx   0        0        0        0 2023-07-05 09:27:30.715887 DataPipelineExecutor-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-30 09:37:05.000000 DataPipelineExecutor-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2787 2023-07-05 09:27:30.715887 DataPipelineExecutor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2330 2023-07-05 09:27:22.000000 DataPipelineExecutor-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-05 09:27:30.715887 DataPipelineExecutor-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      586 2023-07-05 09:25:30.000000 DataPipelineExecutor-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 09:27:30.712377 DataPipelineExecutor-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 09:27:30.715887 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/
+-rw-rw-rw-   0        0        0     2787 2023-07-05 09:27:30.000000 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-05 09:27:30.000000 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 09:27:30.000000 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-05 09:27:30.000000 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35008 2023-07-03 14:23:59.000000 DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.py
```

### Comparing `DataPipelineExecutor-0.0.2/LICENSE.txt` & `DataPipelineExecutor-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DataPipelineExecutor-0.0.2/PKG-INFO` & `DataPipelineExecutor-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: DataPipelineExecutor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to execute Copy and Stored Procedure tasks on data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DataPipelineExecutor
 
-This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB). This tasks are completely configurable and the pipeline has followinf key features:
+This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB), and Executing a simple SQL Stored Procedure on the copied data. These tasks are completely configurable and the pipeline has following key features:
 - Restartability with configurability.
-- Logging - on tpop of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
+- Logging - on top of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
 
 ## Installation
 Use pip to install the package:
 
 ```shell
 pip install DataPipelineExecutor
 ```
@@ -29,15 +29,15 @@
 pip install azure-kusto-ingest
 pip install pyodbc
 pip install papermill
 ```
 
 ## Usage
 
-The to execute the pipelinem run the following:
+The to execute the pipeline run the following:
 ```shell
 import main from DataPipelineExecutor
 main('config.txt', 'logger.log')
 # OR
 main('config.txt')
 ```
```

### Comparing `DataPipelineExecutor-0.0.2/README.md` & `DataPipelineExecutor-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DataPipelineExecutor
 
-This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB). This tasks are completely configurable and the pipeline has followinf key features:
+This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB), and Executing a simple SQL Stored Procedure on the copied data. These tasks are completely configurable and the pipeline has following key features:
 - Restartability with configurability.
-- Logging - on tpop of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
+- Logging - on top of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
 
 ## Installation
 Use pip to install the package:
 
 ```shell
 pip install DataPipelineExecutor
 ```
@@ -19,15 +19,15 @@
 pip install azure-kusto-ingest
 pip install pyodbc
 pip install papermill
 ```
 
 ## Usage
 
-The to execute the pipelinem run the following:
+The to execute the pipeline run the following:
 ```shell
 import main from DataPipelineExecutor
 main('config.txt', 'logger.log')
 # OR
 main('config.txt')
 ```
```

### Comparing `DataPipelineExecutor-0.0.2/setup.py` & `DataPipelineExecutor-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='DataPipelineExecutor',
-    version='0.0.2',
+    version='0.0.3',
     description='A package to execute Copy and Stored Procedure tasks on data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=["DataPipelineExecutor"],
     package_dir={'':'src'},
     classifiers=(
         "Programming Language :: Python :: 3",
```

### Comparing `DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.egg-info/PKG-INFO` & `DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: DataPipelineExecutor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to execute Copy and Stored Procedure tasks on data
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DataPipelineExecutor
 
-This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB). This tasks are completely configurable and the pipeline has followinf key features:
+This package contains a pipeline which executes two tasks: Copying data from source (Kusto Cluster DB) to the sink (SQL Sever DB), and Executing a simple SQL Stored Procedure on the copied data. These tasks are completely configurable and the pipeline has following key features:
 - Restartability with configurability.
-- Logging - on tpop of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
+- Logging - on top of logging on console, you can pass a dedicated filepath as a parameter if you wish to store the logs. Otherwise a *logger.log* file will be created in the same directory and all logs will be stored there until deleted.
 
 ## Installation
 Use pip to install the package:
 
 ```shell
 pip install DataPipelineExecutor
 ```
@@ -29,15 +29,15 @@
 pip install azure-kusto-ingest
 pip install pyodbc
 pip install papermill
 ```
 
 ## Usage
 
-The to execute the pipelinem run the following:
+The to execute the pipeline run the following:
 ```shell
 import main from DataPipelineExecutor
 main('config.txt', 'logger.log')
 # OR
 main('config.txt')
 ```
```

### Comparing `DataPipelineExecutor-0.0.2/src/DataPipelineExecutor.py` & `DataPipelineExecutor-0.0.3/src/DataPipelineExecutor.py`

 * *Files identical despite different names*

