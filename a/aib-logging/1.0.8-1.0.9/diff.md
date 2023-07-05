# Comparing `tmp/aib_logging-1.0.8.tar.gz` & `tmp/aib_logging-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-1.0.8.tar", last modified: Mon May 29 10:21:20 2023, max compression
+gzip compressed data, was "aib_logging-1.0.9.tar", last modified: Wed Jul  5 13:02:36 2023, max compression
```

## Comparing `aib_logging-1.0.8.tar` & `aib_logging-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.731631 aib_logging-1.0.8/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.8/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-29 10:21:20.731631 aib_logging-1.0.8/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.8/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-29 10:20:59.000000 aib_logging-1.0.8/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-29 10:21:20.731631 aib_logging-1.0.8/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.724630 aib_logging-1.0.8/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.728630 aib_logging-1.0.8/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.8/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14590 2023-05-29 10:20:53.000000 aib_logging-1.0.8/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.730631 aib_logging-1.0.8/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       28 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-07-05 13:02:36.246021 aib_logging-1.0.9/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.9/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      615 2023-07-05 13:02:36.246021 aib_logging-1.0.9/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.9/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      748 2023-07-05 13:01:52.000000 aib_logging-1.0.9/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-07-05 13:02:36.246021 aib_logging-1.0.9/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-07-05 13:02:36.235020 aib_logging-1.0.9/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-07-05 13:02:36.244021 aib_logging-1.0.9/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.9/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    15829 2023-07-05 13:00:45.000000 aib_logging-1.0.9/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-07-05 13:02:36.246021 aib_logging-1.0.9/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      615 2023-07-05 13:02:36.000000 aib_logging-1.0.9/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-07-05 13:02:36.000000 aib_logging-1.0.9/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-07-05 13:02:36.000000 aib_logging-1.0.9/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       28 2023-07-05 13:02:36.000000 aib_logging-1.0.9/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-07-05 13:02:36.000000 aib_logging-1.0.9/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-1.0.8/LICENSE.txt` & `aib_logging-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.8/pyproject.toml` & `aib_logging-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
+  { name="karim ramzy", email="karimatefhenry@gmail.com"},
+  { name="muhammad badawy", email="muhammad.i.badawy@gmail.com"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `aib_logging-1.0.8/src/aib_logging/logger.py` & `aib_logging-1.0.9/src/aib_logging/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         CREATE="Create"
         UPDATE="Update"
         DELETE="Delete"
         UPLOAD="Upload"
         READ="Read"
         MODEL_SCORE="Model_Score"
         DATA_STAT="Data_statistics"
+        GIT_COMMIT="git_commit"
         OTHER="Other"
     
     class Severities(Enum):
         INFO="INFO"
         WARNING="WARNING"
         ERROR="ERROR"
 
@@ -386,8 +387,48 @@
             "extra_labels":extra_labels,
             "message":msg,
             "object":object
         }
         for key, value in kwargs.items():
                 payload[key]=value
         # Send the Log request
+        self.logger.log_struct(payload, severity=severity.value)
+
+    def git_commit_log(
+        self,
+        msg:str,
+        category:Categories=Categories.DATA,
+        action:Actions=Actions.GIT_COMMIT,
+        severity:Severities=Severities.INFO,
+        commit_user:str ="",
+        commit_message:str="",
+        commit_date:str="",
+        commit_additions:str="",
+        commit_url:str="",
+        extra_labels:list=[],
+        object:dict={},
+        **kwargs
+        ):
+
+ 
+
+        import inspect
+        payload={
+            "pipeline_run_name":self.pipeline_name,
+            "component_name": inspect.stack()[1].function,
+            "project":self.project,
+            "region":self.region,
+            "category":category.value,
+            "action":action.value,
+            "commit_user":commit_user,
+            "commit_message":commit_message,
+            "commit_date":commit_date,
+            "commit_additions":commit_additions,
+            "commit_url":commit_url,
+            "extra_labels":extra_labels,
+            "message":msg,
+            "object":object
+        }
+        for key, value in kwargs.items():
+                payload[key]=value
+        # Send the Log request
         self.logger.log_struct(payload, severity=severity.value)
```

