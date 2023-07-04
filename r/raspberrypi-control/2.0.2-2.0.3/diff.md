# Comparing `tmp/raspberrypi_control-2.0.2.tar.gz` & `tmp/raspberrypi_control-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberrypi_control-2.0.2.tar", last modified: Tue Jul  4 22:49:44 2023, max compression
+gzip compressed data, was "raspberrypi_control-2.0.3.tar", last modified: Tue Jul  4 22:59:25 2023, max compression
```

## Comparing `raspberrypi_control-2.0.2.tar` & `raspberrypi_control-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.139421 raspberrypi_control-2.0.2/raspberrypi_control/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/raspberrypi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58115 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/raspberrypi_control/raspberrypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/raspberrypi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/raspberrypi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58549 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/raspberrypi_control/raspberrypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/setup.cfg
```

### Comparing `raspberrypi_control-2.0.2/LICENSE` & `raspberrypi_control-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-2.0.2/PKG-INFO` & `raspberrypi_control-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi_control
-Version: 2.0.2
+Version: 2.0.3
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `raspberrypi_control-2.0.2/README.md` & `raspberrypi_control-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-2.0.2/pyproject.toml` & `raspberrypi_control-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspberrypi_control"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Geoloup Team", email="franckiebbb@gmail.com"},
 ]
 description = "Control Raspberrypi board with ssh and python"
 readme = "README.md"
 dependencies = [
     "requests",
```

### Comparing `raspberrypi_control-2.0.2/raspberrypi_control/raspberrypi.py` & `raspberrypi_control-2.0.3/raspberrypi_control/raspberrypi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1150,30 +1150,32 @@
             return wrapper
 
 
 raspberrypi_prep = "192.168.0.10"
 raspberrypi_prep_max = "9"
 raspberrypi_prep_timeout = 1
 raspberrypi_ip = 0
+raspberrypi_info = list()
 
 
 def raspberry_command(add=False):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 global raspberrypi_prep
+                global raspberrypi_info
                 global imported
                 global function_to_add
                 HOST_IP = raspberrypi().local(raspberrypi_prep)
-                SSH_PWD = "geoloup"
+                SSH_PWD = raspberrypi_info[0]
                 ssh_controller = ssh.SSHController(
                     host=HOST_IP,
                     user="geoloup",
-                    ssh_password=SSH_PWD
+                    ssh_password=raspberrypi_info[1]
                 )
                 ssh_controller.connect()
                 import inspect
                 func_content = inspect.getsource(func)
                 func_content = func_content.splitlines(True)
                 func_contentl = list()
                 ft = 0
@@ -1378,20 +1380,21 @@
 
 
 class raspberrypi:
     global raspberrypi_prep_timeout
 
     @timeout(raspberrypi_prep_timeout, default=False)
     def check(self, hoip):
+        global raspberrypi_info
         HOST_IP = hoip
-        SSH_PWD = "geoloup"
+        SSH_PWD = raspberrypi_info[1]
 
         ssh_controller = ssh.SSHController(
             host=HOST_IP,
-            user="geoloup",
+            user=raspberrypi_info[0],
             ssh_password=SSH_PWD
         )
         ssh_controller.connect()
         try:
             ssh_controller.run(
                 command="ls"
             )
@@ -1423,24 +1426,31 @@
                 if raspberrypi().check(hoip):
                     raspberrypi_ip = hoip
                     break
                 else:
                     continue
         res = raspberrypi_ip
         return res
-
+    
+    def set_raspberry_info(self,user_name,password):
+        global raspberrypi_info
+        raspberrypi_info = list()
+        raspberrypi_info.append(user_name)
+        raspberrypi_info.append(password)
 
 def run_command(command=None,display=False):
     if not command == None:
         global raspberrypi_prep
+        global raspberrypi_info
+        SSH_PWD = "geoloup"
         HOST_IP = raspberrypi().local(raspberrypi_prep)
         ssh_controller = ssh.SSHController(
             host=HOST_IP,
-            user="geoloup",
-        ssh_password=SSH_PWD
+            user=raspberrypi_info[0],
+            ssh_password=raspberrypi_info[1]
         )
         try:
             ssh_controller.connect()
             exit_code, output = ssh_controller.run(
                 command=command,
                 display=display,
                 capture=True
```

### Comparing `raspberrypi_control-2.0.2/raspberrypi_control.egg-info/PKG-INFO` & `raspberrypi_control-2.0.3/raspberrypi_control.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi-control
-Version: 2.0.2
+Version: 2.0.3
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

