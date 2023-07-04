# Comparing `tmp/raspberrypi_control-2.0.1.tar.gz` & `tmp/raspberrypi_control-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberrypi_control-2.0.1.tar", last modified: Tue Jul  4 22:37:24 2023, max compression
+gzip compressed data, was "raspberrypi_control-2.0.2.tar", last modified: Tue Jul  4 22:49:44 2023, max compression
```

## Comparing `raspberrypi_control-2.0.1.tar` & `raspberrypi_control-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:37:24.393149 raspberrypi_control-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 22:37:12.000000 raspberrypi_control-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:37:24.393149 raspberrypi_control-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 22:37:12.000000 raspberrypi_control-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 22:37:12.000000 raspberrypi_control-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:37:24.389149 raspberrypi_control-2.0.1/raspberrypi_control/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 22:37:12.000000 raspberrypi_control-2.0.1/raspberrypi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58113 2023-07-04 22:37:12.000000 raspberrypi_control-2.0.1/raspberrypi_control/raspberrypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:37:24.393149 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:37:24.000000 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:37:24.000000 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:37:24.000000 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 22:37:24.000000 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 22:37:24.000000 raspberrypi_control-2.0.1/raspberrypi_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:37:24.393149 raspberrypi_control-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.139421 raspberrypi_control-2.0.2/raspberrypi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/raspberrypi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58115 2023-07-04 22:49:34.000000 raspberrypi_control-2.0.2/raspberrypi_control/raspberrypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 22:49:44.000000 raspberrypi_control-2.0.2/raspberrypi_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:49:44.143421 raspberrypi_control-2.0.2/setup.cfg
```

### Comparing `raspberrypi_control-2.0.1/LICENSE` & `raspberrypi_control-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-2.0.1/PKG-INFO` & `raspberrypi_control-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi_control
-Version: 2.0.1
+Version: 2.0.2
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `raspberrypi_control-2.0.1/README.md` & `raspberrypi_control-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-2.0.1/pyproject.toml` & `raspberrypi_control-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspberrypi_control"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Geoloup Team", email="franckiebbb@gmail.com"},
 ]
 description = "Control Raspberrypi board with ssh and python"
 readme = "README.md"
 dependencies = [
     "requests",
```

### Comparing `raspberrypi_control-2.0.1/raspberrypi_control/raspberrypi.py` & `raspberrypi_control-2.0.2/raspberrypi_control/raspberrypi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1442,13 +1442,13 @@
             ssh_controller.connect()
             exit_code, output = ssh_controller.run(
                 command=command,
                 display=display,
                 capture=True
             )
             return output[-1]
-        else:
+        except:
             import os
             return  os.system(command)
     else:
         quit("You need to have a command... At run_command")
         return None
```

### Comparing `raspberrypi_control-2.0.1/raspberrypi_control.egg-info/PKG-INFO` & `raspberrypi_control-2.0.2/raspberrypi_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspberrypi-control
-Version: 2.0.1
+Version: 2.0.2
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

