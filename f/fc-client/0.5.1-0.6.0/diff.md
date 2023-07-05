# Comparing `tmp/fc-client-0.5.1.tar.gz` & `tmp/fc-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.5.1.tar", last modified: Thu May  4 06:09:39 2023, max compression
+gzip compressed data, was "dist/fc-client-0.6.0.tar", last modified: Wed Jul  5 06:32:30 2023, max compression
```

## Comparing `fc-client-0.5.1.tar` & `fc-client-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       35 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      318 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-client-0.5.1/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 06:09:39.000000 fc-client-0.5.1/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_client/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7005 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_client/client.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-client-0.5.1/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-client-0.5.1/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 06:09:15.000000 fc-client-0.5.1/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-client-0.5.1/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 06:09:15.000000 fc-client-0.5.1/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-client-0.5.1/PKG-INFO
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-0.6.0/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-03-29 08:28:44.000000 fc-client-0.6.0/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:30.000000 fc-client-0.6.0/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2022-08-17 06:53:34.000000 fc-client-0.6.0/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-0.6.0/fc_client/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    13952 2023-07-05 06:29:52.000000 fc-client-0.6.0/fc_client/client.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-0.6.0/fc_client.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:29.000000 fc-client-0.6.0/fc_client.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-05 06:32:30.000000 fc-client-0.6.0/fc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-05 06:32:29.000000 fc-client-0.6.0/fc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-05 06:32:29.000000 fc-client-0.6.0/fc_client.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       84 2023-07-05 06:32:29.000000 fc-client-0.6.0/fc_client.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-05 06:32:29.000000 fc-client-0.6.0/fc_client.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-0.6.0/fc_client_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-05 06:29:52.000000 fc-client-0.6.0/fc_client_daemon/client_daemon.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:30.000000 fc-client-0.6.0/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-05 06:30:26.000000 fc-client-0.6.0/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-06-30 05:19:57.000000 fc-client-0.6.0/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-06-30 05:20:06.000000 fc-client-0.6.0/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-06-30 05:20:06.000000 fc-client-0.6.0/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-05 06:29:52.000000 fc-client-0.6.0/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-06-30 05:19:57.000000 fc-client-0.6.0/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-05 06:32:30.000000 fc-client-0.6.0/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3859 2023-07-05 06:29:52.000000 fc-client-0.6.0/setup.py
```

### Comparing `fc-client-0.5.1/fc_client.egg-info/PKG-INFO` & `fc-client-0.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.5.1
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `fc-client-0.5.1/README.rst` & `fc-client-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.1/setup.cfg` & `fc-client-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.1/LICENSE` & `fc-client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.1/fc_common/version.py` & `fc-client-0.6.0/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.5.1/setup.py` & `fc-client-0.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import os
 import pathlib
+import signal
 import sys
 
 import pkg_resources
 from setuptools import Command, find_packages, setup
+from setuptools.command.install import install
 
 from fc_common.version import get_package_version
 
 
 class CleanCommand(Command):
     """Custom clean command to tidy up the project root."""
 
@@ -27,14 +29,27 @@
     def finalize_options(self):
         pass
 
     def run(self):  # pylint: disable=no-self-use
         os.system("rm -vrf ./build ./dist ./*.pyc ./*.tgz ./*.egg-info ./__pycache__")
 
 
+class InstallCommand(install):
+    """Custom install command to clear old client daemon"""
+
+    def run(self):
+        super().run()
+
+        pid_file = "/tmp/fc/fc_client_daemon.pid"
+        if os.path.exists(pid_file):
+            pid_path = pathlib.Path(pid_file)
+            pid = int(pid_path.read_text(encoding="utf-8").rstrip())
+            os.kill(pid, signal.SIGINT)
+
+
 def get_project_name():
     for dist in pkg_resources.AvailableDistributions():
         if dist.startswith("fc"):
             try:
                 pathlib.Path(__file__).relative_to(
                     pkg_resources.get_distribution(dist).location
                 )
@@ -56,15 +71,15 @@
     },
 }
 
 if PKG == "fc-server":
     setup(
         **common_setup,
         name="fc-server",
-        packages=find_packages(include=("fc_common", "fc_server*")),
+        packages=find_packages(include=("fc_common", "fc_server*", "fc_server_daemon")),
         package_data={
             "fc_common": ["VERSION"],
             "fc_server": ["config/sample_cfg.yaml", "config/sample_lavacli.yaml"],
         },
         entry_points={
             "console_scripts": [
                 "fc-server = fc_server.server:main",
@@ -73,14 +88,18 @@
         install_requires=[
             "aiohttp>=3.7.4.post0",
             "async-lru>=1.0.3",
             "flatdict>=4.0.1",
             "lavacli==1.2",
             "labgrid==23.0.1",
             "singledispatchmethod>=1.0",
+            "python-prctl",
+            "etcd3-fc",
+            "tenacity",
+            "protobuf==3.20.3",
         ],
     )
 elif PKG == "fc-guarder":
     setup(
         **common_setup,
         name="fc-guarder",
         packages=["fc_guarder"],
@@ -88,24 +107,45 @@
             "console_scripts": [
                 "fc-guarder = fc_guarder.guarder:main",
             ]
         },
         install_requires=[f"fc-server=={get_package_version()}"],
     )
 elif PKG == "fc-client":
+    common_setup["cmdclass"].update({"install": InstallCommand})
     setup(
         **common_setup,
         name="fc-client",
-        packages=["fc_common", "fc_client"],
+        packages=["fc_common", "fc_client", "fc_client_daemon"],
         package_data={
             "fc_common": ["VERSION"],
         },
         entry_points={
             "console_scripts": [
                 "fc-client = fc_client.client:main",
             ]
         },
         install_requires=[
             "prettytable>=2.2.1",
             "labgrid==23.0.1",
+            "python-daemon",
+            "etcd3-fc",
+            "tenacity",
+            "protobuf==3.20.3",
         ],
     )
+elif PKG == "fc-client-docker":
+    setup(
+        **common_setup,
+        name="fc-client-docker",
+        packages=["fc_common", "fc_client_docker"],
+        package_data={
+            "fc_common": ["VERSION"],
+            "fc_client_docker": ["fc_client_docker"],
+        },
+        entry_points={
+            "console_scripts": [
+                "fc-client-docker = fc_client_docker:main",
+            ]
+        },
+        python_requires=">=3",
+    )
```

### Comparing `fc-client-0.5.1/PKG-INFO` & `fc-client-0.6.0/fc_client.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.5.1
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
-
-UNKNOWN
-
```

