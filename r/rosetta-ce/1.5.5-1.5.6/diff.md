# Comparing `tmp/rosetta-ce-1.5.5.tar.gz` & `tmp/rosetta-ce-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.5.5.tar", last modified: Tue Jul  4 08:30:00 2023, max compression
+gzip compressed data, was "rosetta-ce-1.5.6.tar", last modified: Wed Jul  5 10:31:50 2023, max compression
```

## Comparing `rosetta-ce-1.5.5.tar` & `rosetta-ce-1.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.910155 rosetta-ce-1.5.5/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.5/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:30:00.909845 rosetta-ce-1.5.5/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.5/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.905484 rosetta-ce-1.5.5/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.5/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.907241 rosetta-ce-1.5.5/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.5/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)      269 2023-07-04 08:04:58.000000 rosetta-ce-1.5.5/rosetta/constants/attributes.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.5/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.5/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6478 2023-07-04 08:03:50.000000 rosetta-ce-1.5.5/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.5/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    44325 2023-07-04 08:28:39.000000 rosetta-ce-1.5.5/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    10463 2023-07-04 04:58:55.000000 rosetta-ce-1.5.5/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.908522 rosetta-ce-1.5.5/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      491 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-04 08:30:00.000000 rosetta-ce-1.5.5/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-04 08:30:00.910222 rosetta-ce-1.5.5/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-04 08:29:04.000000 rosetta-ce-1.5.5/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-04 08:30:00.909438 rosetta-ce-1.5.5/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.5/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.5/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.5/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-05 10:31:50.425996 rosetta-ce-1.5.6/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.5.6/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-05 10:31:50.425646 rosetta-ce-1.5.6/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.5.6/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-05 10:31:50.418707 rosetta-ce-1.5.6/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.5.6/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-05 10:31:50.421855 rosetta-ce-1.5.6/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.5.6/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)      269 2023-07-04 08:04:58.000000 rosetta-ce-1.5.6/rosetta/constants/attributes.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.5.6/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.5.6/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6478 2023-07-04 08:03:50.000000 rosetta-ce-1.5.6/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.5.6/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44997 2023-07-05 10:31:41.000000 rosetta-ce-1.5.6/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10463 2023-07-04 04:58:55.000000 rosetta-ce-1.5.6/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-05 10:31:50.423666 rosetta-ce-1.5.6/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-05 10:31:50.000000 rosetta-ce-1.5.6/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      491 2023-07-05 10:31:50.000000 rosetta-ce-1.5.6/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-05 10:31:50.000000 rosetta-ce-1.5.6/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-05 10:31:50.000000 rosetta-ce-1.5.6/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-05 10:31:50.000000 rosetta-ce-1.5.6/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-05 10:31:50.426038 rosetta-ce-1.5.6/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-05 10:31:41.000000 rosetta-ce-1.5.6/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-05 10:31:50.425067 rosetta-ce-1.5.6/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.5.6/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.5.6/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.5.6/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.5.5/LICENSE` & `rosetta-ce-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/PKG-INFO` & `rosetta-ce-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.5
+Version: 1.5.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.5/README.md` & `rosetta-ce-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta/constants/sensors.py` & `rosetta-ce-1.5.6/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta/constants/sources.py` & `rosetta-ce-1.5.6/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta/constants/systems.py` & `rosetta-ce-1.5.6/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta/rconverter.py` & `rosetta-ce-1.5.6/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta/rfaker.py` & `rosetta-ce-1.5.6/rosetta/rfaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
                  sender_email: Optional[list] = None, recipient_email: Optional[list] = None,
                  email_subject: Optional[list] = None, email_body: Optional[list] = None,
                  url: Optional[list] = None, source_port: Optional[list] = None, remote_port: Optional[list] = None,
                  protocol: Optional[list] = None, inbound_bytes: Optional[list] = None,
                  outbound_bytes: Optional[list] = None, app: Optional[list] = None, os: Optional[list] = None,
                  user: Optional[list] = None, cve: Optional[list] = None, file_name: Optional[list] = None,
                  file_hash: Optional[list] = None, win_cmd: Optional[list] = None, unix_cmd: Optional[list] = None,
-                 win_process: Optional[list] = None, unix_process: Optional[list] = None,
+                 win_process: Optional[list] = None, win_child_process: Optional[list] = None,
+                 unix_process: Optional[list] = None, unix_child_process: Optional[list] = None,
                  technique: Optional[list] = None, entry_type: Optional[list] = None, severity: Optional[list] = None,
                  sensor: Optional[list] = None, action: Optional[list] = None, event_id: Optional[list] = None,
                  error_code: Optional[list] = None, terms: Optional[list] = None, alert_types: Optional[list] = None,
                  alert_name: Optional[list] = None, incident_types: Optional[list] = None,
                  analysts: Optional[list] = None, action_status: Optional[list] = None):
         self.local_ip = local_ip
         self.remote_ip = remote_ip
@@ -70,15 +71,17 @@
         self.user = user
         self.cve = cve
         self.file_name = file_name
         self.file_hash = file_hash
         self.win_cmd = win_cmd
         self.unix_cmd = unix_cmd
         self.win_process = win_process
+        self.win_child_process = win_child_process
         self.unix_process = unix_process
+        self.unix_child_process = unix_child_process
         self.technique = technique
         self.entry_type = entry_type
         self.severity = severity
         self.sensor = sensor
         self.action = action
         self.event_id = event_id
         self.error_code = error_code
@@ -296,14 +299,17 @@
                 else faker.hostname()
         if field == "user":
             field_value = random.choice(observables.user) if observables and observables.user \
                 else faker.user_name()
         if field == "unix_process":
             field_value = random.choice(observables.unix_process) if observables and observables.unix_process \
                 else "sudo"
+        if field == "unix_child_process":
+            field_value = random.choice(observables.unix_child_process) if observables and \
+                                                                           observables.unix_child_process else "sudo"
         if field == "unix_cmd":
             field_value = random.choice(observables.unix_cmd) if observables and observables.unix_cmd \
                 else random.choice(UNIX_CMD)
         if field == "severity":
             field_value = random.choice(observables.severity) if observables and observables.severity \
                 else random.choice(SEVERITIES)
         if field == "local_ip":
@@ -402,14 +408,17 @@
                 else faker.random.randint(1, 999)
         if field == "win_process":
             field_value = random.choice(observables.win_process) if observables and observables.win_process \
                 else random.choice(WIN_PROCESSES)
         if field == "win_cmd":
             field_value = random.choice(observables.win_cmd) if observables and observables.win_cmd \
                 else random.choice(WINDOWS_CMD)
+        if field == "win_child_process":
+            field_value = random.choice(observables.win_child_process) if \
+                observables and observables.win_child_process else random.choice(WIN_PROCESSES)
         if field == "source_network_address":
             field_value = random.choice(observables.local_ip) if observables and observables.local_ip \
                 else faker.ipv4_private()
         if field == "file_name":
             field_value = random.choice(observables.file_name) if observables and observables.file_name \
                 else faker.file_name()
         if field == "cve_id":
```

### Comparing `rosetta-ce-1.5.5/rosetta/rsender.py` & `rosetta-ce-1.5.6/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.5.6/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.5.5
+Version: 1.5.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.5.5/setup.py` & `rosetta-ce-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.5.5",
+    version="1.5.6",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.5.5/tests/test_rconverter.py` & `rosetta-ce-1.5.6/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/tests/test_rfaker.py` & `rosetta-ce-1.5.6/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.5.5/tests/test_rsender.py` & `rosetta-ce-1.5.6/tests/test_rsender.py`

 * *Files identical despite different names*

