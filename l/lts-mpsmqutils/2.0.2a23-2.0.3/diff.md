# Comparing `tmp/lts-mpsmqutils-2.0.2a23.tar.gz` & `tmp/lts-mpsmqutils-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a23.tar", last modified: Thu Jun 29 16:05:48 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.3.tar", last modified: Wed Jul  5 16:12:37 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a23.tar` & `lts-mpsmqutils-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-29 16:05:48.947859 lts-mpsmqutils-2.0.2a23/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-29 16:05:48.947329 lts-mpsmqutils-2.0.2a23/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a23/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-29 16:05:48.938145 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-29 16:05:48.000000 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-29 16:05:48.000000 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-29 16:05:48.000000 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-29 16:05:48.000000 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-29 16:05:48.000000 lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-29 16:05:48.940584 lts-mpsmqutils-2.0.2a23/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     1075 2023-06-08 19:03:56.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    25679 2023-06-28 20:58:30.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-29 16:04:19.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-29 16:05:48.946129 lts-mpsmqutils-2.0.2a23/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a23/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-29 16:05:48.948025 lts-mpsmqutils-2.0.2a23/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-29 16:03:40.000000 lts-mpsmqutils-2.0.2a23/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-07-05 16:12:37.695328 lts-mpsmqutils-2.0.3/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6649 2023-07-05 16:12:37.694863 lts-mpsmqutils-2.0.3/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.3/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-07-05 16:12:37.690590 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6649 2023-07-05 16:12:37.000000 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-07-05 16:12:37.000000 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-07-05 16:12:37.000000 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-07-05 16:12:37.000000 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-07-05 16:12:37.000000 lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-07-05 16:12:37.692967 lts-mpsmqutils-2.0.3/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.3/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     1075 2023-07-05 16:08:23.000000 lts-mpsmqutils-2.0.3/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    25653 2023-07-05 16:08:23.000000 lts-mpsmqutils-2.0.3/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-07-05 16:08:23.000000 lts-mpsmqutils-2.0.3/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-07-05 16:12:37.693909 lts-mpsmqutils-2.0.3/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.3/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.3/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-07-05 16:12:37.695512 lts-mpsmqutils-2.0.3/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      896 2023-07-05 16:08:42.000000 lts-mpsmqutils-2.0.3/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a23/PKG-INFO` & `lts-mpsmqutils-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a23
+Version: 2.0.3
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a23/README.md` & `lts-mpsmqutils-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a23/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.3/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a23
+Version: 2.0.3
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a23/mpsmqutils/log_wrapper.py` & `lts-mpsmqutils-2.0.3/mpsmqutils/log_wrapper.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a23/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.3/mpsmqutils/messagehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,14 @@
 
     def handle_message(self):
         logger.debug("************************ MQUTILS MQLISTENER - HANDLE_MESSAGE *******************************")
         # headers, body = frame.headers, frame.body
         logger.info('handling message "%s"' % self.message)
 
         category = self.message.get("category", "ingest")
-        # task_management
         task_success = False
         job_ticket_id = self.message.get('job_ticket_id')
         logger.info('job_ticket_id {}'.format(job_ticket_id))
         try:
             job_tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
         except Exception as e:
             import traceback
```

### Comparing `lts-mpsmqutils-2.0.2a23/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.3/mpsmqutils/mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a23/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.3/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a23/setup.py` & `lts-mpsmqutils-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a23",
+    version="2.0.3",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

