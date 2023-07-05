# Comparing `tmp/trailml-1.0.1.tar.gz` & `tmp/trailml-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailml-1.0.1.tar", last modified: Thu Jun 29 12:19:21 2023, max compression
+gzip compressed data, was "trailml-1.0.2.tar", last modified: Wed Jul  5 14:04:05 2023, max compression
```

## Comparing `trailml-1.0.1.tar` & `trailml-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.589105 trailml-1.0.1/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-06-29 12:19:21.588973 trailml-1.0.1/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.1/README.md
--rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-06-29 12:15:25.000000 trailml-1.0.1/pyproject.toml
--rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-06-29 12:19:21.589156 trailml-1.0.1/setup.cfg
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.585160 trailml-1.0.1/src/
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.585943 trailml-1.0.1/src/trail/
--rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/__init__.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.586633 trailml-1.0.1/src/trail/libconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      235 2023-06-05 14:32:13.000000 trailml-1.0.1/src/trail/libconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-30 16:59:12.000000 trailml-1.0.1/src/trail/libconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)    10795 2023-06-22 15:45:14.000000 trailml-1.0.1/src/trail/trail.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.587845 trailml-1.0.1/src/trail/userconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/exceptions.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.588755 trailml-1.0.1/src/trailml.egg-info/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/requires.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.047338 trailml-1.0.2/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-05 14:04:05.047181 trailml-1.0.2/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.2/README.md
+-rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-07-05 14:02:41.000000 trailml-1.0.2/pyproject.toml
+-rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-07-05 14:04:05.047392 trailml-1.0.2/setup.cfg
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.043511 trailml-1.0.2/src/
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.044316 trailml-1.0.2/src/trail/
+-rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/__init__.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.045110 trailml-1.0.2/src/trail/libconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      194 2023-07-05 12:36:48.000000 trailml-1.0.2/src/trail/libconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-30 16:59:12.000000 trailml-1.0.2/src/trail/libconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)    10765 2023-07-05 13:35:09.000000 trailml-1.0.2/src/trail/trail.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.046086 trailml-1.0.2/src/trail/userconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.2/src/trail/userconfig/exceptions.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-07-05 14:04:05.046964 trailml-1.0.2/src/trailml.egg-info/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/requires.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-07-05 14:04:05.000000 trailml-1.0.2/src/trailml.egg-info/top_level.txt
```

### Comparing `trailml-1.0.1/PKG-INFO` & `trailml-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.1
+Version: 1.0.2
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trailml-1.0.1/README.md` & `trailml-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trailml-1.0.1/pyproject.toml` & `trailml-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trailml"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Trail ML", email="python@trail-ml.com" },
 ]
 description = "Trail ML library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `trailml-1.0.1/src/trail/trail.py` & `trailml-1.0.2/src/trail/trail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import base64
-from collections import defaultdict
-import json
 import os.path
 import signal
 import sys
+from collections import defaultdict
 from typing import Union
 
 import mlflow
 import pyrebase
 import requests
-from gql import gql, Client
+from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.exceptions import TransportQueryError
 from mlflow.entities import Run
 from mlflow.tracking import MlflowClient
 
 from .libconfig import libconfig
 from .userconfig import userconfig
@@ -22,16 +21,16 @@
 class Trail:
     ADD_EXPERIMENT_MUTATION = """
         mutation (
             $projectId: String!,
             $parentExperimentId: String!,
             $title: String!,
             $comments: String!,
-            $instanceRunParameters: JSONString!,
-            $instanceRunMetrics: JSONString!,
+            $instanceRunParameters: GenericScalar!,
+            $instanceRunMetrics: GenericScalar!,
             $instanceRunComplete: Boolean!
             $hypothesis: String,
             $metricsHistoryEntries: [MetricsHistoryInput]
         ) {
             addExperiment(
                 projectId: $projectId,
                 parentExperimentId: $parentExperimentId,
@@ -149,16 +148,16 @@
 
     def put_artifact(
             self,
             src:  Union[str, bytes],
             name: str,
             tags: Union[str, list, None]
     ):
-        """Queues an artifact for upload to Trail. The artifact is uploaded when
-        leaving the `with Trail` block.
+        """Queues an artifact for upload to Trail.
+        The artifact is uploaded when leaving the `with Trail` block.
         The `src` parameter can be either a string or a bytes object. In case
         of a string, it is assumed to be a path to a file. In case of a bytes
         object, it is assumed to be the raw data of the artifact.
 
         :param src: The artifact path or bytes to upload
         :param name: The name of the artifact
         :param tags: A single tag or a list of tags
@@ -222,16 +221,16 @@
             result = self.client.execute(
                 document=gql(self.ADD_EXPERIMENT_MUTATION),
                 variable_values={
                     'projectId': self.project_id,
                     'parentExperimentId': self.parent_experiment_id,
                     'title': self.experiment_title,
                     'comments': '',
-                    'instanceRunParameters': json.dumps(converted_params),
-                    'instanceRunMetrics': json.dumps(run.data.metrics),
+                    'instanceRunParameters': converted_params,
+                    'instanceRunMetrics': run.data.metrics,
                     'instanceRunComplete': self.is_complete,
                     'hypothesis': self.hypothesis,
                     'metricsHistoryEntries': self.get_metric_history_data(
                         run_id=run_id
                     ),
                 },
             )
@@ -266,16 +265,16 @@
                 self._upload_artifact(
                     data=data,
                     name=name,
                     tags=tags,
                 )
         except TransportQueryError:
             print(
-                'Error uploading experiment artifacts to Trail. Please contact '
-                'us if the problem persists.',
+                'Error uploading experiment artifacts to Trail. Please contact'
+                ' us if the problem persists.',
                 file=sys.stderr
             )
 
     def get_metric_history_data(self, run_id):
         client = mlflow.tracking.MlflowClient()
         run = mlflow.active_run()
         mlflowrun = mlflow.get_run(run_id=run.info.run_id)  # type: ignore
```

### Comparing `trailml-1.0.1/src/trail/userconfig/__init__.py` & `trailml-1.0.2/src/trail/userconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.1/src/trail/userconfig/config.py` & `trailml-1.0.2/src/trail/userconfig/config.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.1/src/trail/userconfig/exceptions.py` & `trailml-1.0.2/src/trail/userconfig/exceptions.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.1/src/trailml.egg-info/PKG-INFO` & `trailml-1.0.2/src/trailml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.1
+Version: 1.0.2
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

