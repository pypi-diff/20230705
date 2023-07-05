# Comparing `tmp/pbu-1.0.3.tar.gz` & `tmp/pbu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbu-1.0.3.tar", last modified: Sat Apr  8 01:37:31 2023, max compression
+gzip compressed data, was "pbu-1.1.0.tar", last modified: Wed Jul  5 07:21:23 2023, max compression
```

## Comparing `pbu-1.0.3.tar` & `pbu-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-08 01:37:31.298100 pbu-1.0.3/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-04-08 01:37:31.298100 pbu-1.0.3/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.0.3/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-08 01:37:31.297100 pbu-1.0.3/pbu/
--rw-rw-r--   0 peter     (1000) peter     (1000)      751 2023-04-07 01:27:21.000000 pbu-1.0.3/pbu/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1733 2022-12-08 02:17:54.000000 pbu-1.0.3/pbu/app_config.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5997 2022-12-23 03:03:19.000000 pbu-1.0.3/pbu/basic_monitor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.0.3/pbu/constant_listing.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4383 2023-04-08 01:35:28.000000 pbu-1.0.3/pbu/datascience_util.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.0.3/pbu/date_time.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.0.3/pbu/default_options.py
--rw-r--r--   0 peter     (1000) peter     (1000)      993 2023-04-03 04:48:29.000000 pbu-1.0.3/pbu/files.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4687 2023-04-03 04:51:32.000000 pbu-1.0.3/pbu/json_document.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.0.3/pbu/json_wrapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.0.3/pbu/logger.py
--rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.0.3/pbu/paging.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1101 2021-02-28 01:50:33.000000 pbu-1.0.3/pbu/performance_logger.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.0.3/pbu/time_series.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-04-08 01:37:31.298100 pbu-1.0.3/pbu.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-04-08 01:37:31.000000 pbu-1.0.3/pbu.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      448 2023-04-08 01:37:31.000000 pbu-1.0.3/pbu.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-04-08 01:37:31.000000 pbu-1.0.3/pbu.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.0.3/pbu.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-04-08 01:37:31.000000 pbu-1.0.3/pbu.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-04-08 01:37:31.000000 pbu-1.0.3/pbu.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-04-08 01:37:31.298100 pbu-1.0.3/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-04-08 01:31:11.000000 pbu-1.0.3/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-05 07:21:23.030140 pbu-1.1.0/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.1.0/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/pbu/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      792 2023-07-05 05:55:01.000000 pbu-1.1.0/pbu/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1733 2022-12-08 02:17:54.000000 pbu-1.1.0/pbu/app_config.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6264 2023-07-05 06:07:23.000000 pbu-1.1.0/pbu/basic_monitor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.1.0/pbu/constant_listing.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4383 2023-04-08 01:50:06.000000 pbu-1.1.0/pbu/datascience_util.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.1.0/pbu/date_time.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      374 2023-07-05 06:00:07.000000 pbu-1.1.0/pbu/debug_object.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.1.0/pbu/default_options.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      993 2023-04-03 04:48:29.000000 pbu-1.1.0/pbu/files.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8739 2023-07-05 07:15:28.000000 pbu-1.1.0/pbu/json_document.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.1.0/pbu/json_wrapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.1.0/pbu/logger.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.1.0/pbu/paging.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1223 2023-04-11 09:50:57.000000 pbu-1.1.0/pbu/performance_logger.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.1.0/pbu/time_series.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/pbu.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      468 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.1.0/pbu.egg-info/not-zip-safe
+-rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-05 07:21:23.030140 pbu-1.1.0/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-07-05 07:11:36.000000 pbu-1.1.0/setup.py
```

### Comparing `pbu-1.0.3/PKG-INFO` & `pbu-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.0.3
+Version: 1.1.0
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.0.3/README.md` & `pbu-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/__init__.py` & `pbu-1.1.0/pbu/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 from pbu.constant_listing import ConstantListing
 from pbu.performance_logger import PerformanceLogger
 from pbu.date_time import combine_date_time, to_utc, to_timezone, set_timezone, DATE_FORMAT, DATETIME_FORMAT
 from pbu.datascience_util import weighted_mean, normalise, discretise
 from pbu.app_config import BasicConfig
 from pbu.json_document import JsonDocument, list_to_json, list_from_json
 from pbu.files import write_json, read_json
+from pbu.debug_object import DebugObject
```

### Comparing `pbu-1.0.3/pbu/app_config.py` & `pbu-1.1.0/pbu/app_config.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/basic_monitor.py` & `pbu-1.1.0/pbu/basic_monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import time
 from datetime import datetime
+from typing import Optional
 from abc import ABC, abstractmethod
 from pbu.logger import Logger
 from pbu.constant_listing import ConstantListing
+from pbu.debug_object import DebugObject
 
 
 class JobStatus(ConstantListing):
     CREATED = "CREATED"
     QUEUED = "QUEUED"
     PENDING = "PENDING"
     RUNNING = "RUNNING"
@@ -16,24 +18,27 @@
     STALLED = "STALLED"
     SUCCESS = "SUCCESS"
     ERROR = "ERROR"
     PAUSED = "PAUSED"
     RESUMED = "RESUMED"
 
 
-class BasicMonitor(ABC):
+class BasicMonitor(ABC, DebugObject):
     """
     Abstract base class (ABC) for all monitors containing base functionality for lifecycle and meta information.
     """
 
-    def __init__(self, monitor_id, wait_time, run_interval=False, custom_logger=None, ping_interval=60):
+    def __init__(self, monitor_id: str, wait_time: int, run_interval: bool = False,
+                 custom_logger: Optional[Logger] = None, ping_interval: int = 60, debug: bool = False,
+                 debug_logger: Optional[Logger] = None):
         """
         Super constructor invoked from implementing sub-classes of this class
         providing interfaces start, track_success and track_error
         """
+        super().__init__(debug, debug_logger)
         # set meta flags
         self.active = False
         self.finished = False
         self.started = False
 
         # store parameters
         self.monitor_id = monitor_id
```

### Comparing `pbu-1.0.3/pbu/datascience_util.py` & `pbu-1.1.0/pbu/datascience_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 
 def discretise(value: Union[float, int], precision: Union[float, int] = 1, floor=False,
                ceil=False) -> Union[float, int]:
     """
     This function will round the given value to the nearest multiple of the given precision. There are 2 boolean flags
     available that can force the function to return the lower or upper boundary of a precision interval. If neither is
-    set, the function will return the mid point of the interval.
+    set, the function will return the mid-point of the interval.
     :param value: the value to discretise
     :param precision: the precision to use for the discretisation
     :param floor: a boolean flag indicating whether the lower boundary of the precision interval should be returned
     :param ceil: a boolean flag indicating whether the upper boundary of the precision interval should be returned
     :return: the discretised value
     """
     if value is None:
```

### Comparing `pbu-1.0.3/pbu/date_time.py` & `pbu-1.1.0/pbu/date_time.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/default_options.py` & `pbu-1.1.0/pbu/default_options.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/files.py` & `pbu-1.1.0/pbu/files.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/json_wrapper.py` & `pbu-1.1.0/pbu/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/logger.py` & `pbu-1.1.0/pbu/logger.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu/performance_logger.py` & `pbu-1.1.0/pbu/performance_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from datetime import datetime, timedelta
 from logging import Logger
 
 
 class PerformanceLogger:
-    def __init__(self):
+    def __init__(self, logger=None):
         self.start_time = datetime.now()
         self.last_checkpoint = None
+        self.logger = logger
 
     def start(self):
         self.start_time = datetime.now()
 
     def checkpoint(self, message: str = None, logger: Logger = None):
         start_time = self.last_checkpoint if self.last_checkpoint is not None else self.start_time
         now = datetime.now()
         duration = now - start_time
-        PerformanceLogger._log_message(duration, message, logger)
+        PerformanceLogger._log_message(duration, message, logger if self.logger is None else self.logger)
         self.last_checkpoint = now
 
     def finish(self, message: str = None, logger: Logger = None):
         duration = datetime.now() - self.start_time
-        PerformanceLogger._log_message(duration, message, logger)
+        PerformanceLogger._log_message(duration, message, logger if self.logger is None else self.logger)
 
     @staticmethod
     def _log_message(duration: timedelta, message: str = None, logger: Logger = None):
         if message is None:
             return
 
         print_string = f"{message} took {duration}"
```

### Comparing `pbu-1.0.3/pbu/time_series.py` & `pbu-1.1.0/pbu/time_series.py`

 * *Files identical despite different names*

### Comparing `pbu-1.0.3/pbu.egg-info/PKG-INFO` & `pbu-1.1.0/pbu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.0.3
+Version: 1.1.0
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.0.3/setup.py` & `pbu-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="pbu",
-      version="1.0.3",
+      version="1.1.0",
       description="Basic Utility module for the Python programming language",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/ilfrich/python-basic-utils",
       author="Peter Ilfrich",
       author_email="das-peter@gmx.de",
       license="Apache-2.0",
```

