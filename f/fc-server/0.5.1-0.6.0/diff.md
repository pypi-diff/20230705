# Comparing `tmp/fc-server-0.5.1.tar.gz` & `tmp/fc-server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.5.1.tar", last modified: Thu May  4 06:09:39 2023, max compression
+gzip compressed data, was "dist/fc-server-0.6.0.tar", last modified: Wed Jul  5 06:32:29 2023, max compression
```

## Comparing `fc-server-0.5.1.tar` & `fc-server-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2535 2023-04-10 02:26:18.000000 fc-server-0.5.1/README.rst
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      614 2023-05-04 06:09:39.000000 fc-server-0.5.1/setup.cfg
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server.egg-info/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      109 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/requires.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        1 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/dependency_links.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      897 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/SOURCES.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/PKG-INFO
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       53 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/entry_points.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       20 2023-05-04 06:09:38.000000 fc-server-0.5.1/fc_server.egg-info/top_level.txt
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-04-10 02:26:18.000000 fc-server-0.5.1/LICENSE
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/config/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)       82 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/config/sample_lavacli.yaml
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      357 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/config/sample_cfg.yaml
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/plugins/
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/plugins/utils/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2359 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/utils/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     5185 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/utils/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/plugins/utils/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     7526 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/labgrid.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    17626 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/plugins/lava.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/plugins/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/core/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      681 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/logger.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)    11568 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/coordinator.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     6024 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/api_svr.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1951 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/decorators.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      929 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      623 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/plugin.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2828 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/core/config.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     1071 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/server.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/__init__.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_server/management/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      212 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/management/common.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-04-10 02:26:18.000000 fc-server-0.5.1/fc_server/management/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2498 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_server/management/cmd_online_lava_devices.py
-drwxrwxr-x   0 shubuntu1  (1000) shubuntu1  (1000)        0 2023-05-04 06:09:39.000000 fc-server-0.5.1/fc_common/
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)        6 2023-05-04 06:09:15.000000 fc-server-0.5.1/fc_common/VERSION
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      482 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_common/__init__.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      712 2023-05-04 03:23:04.000000 fc-server-0.5.1/fc_common/version.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)     2642 2023-05-04 06:09:15.000000 fc-server-0.5.1/setup.py
--rw-rw-r--   0 shubuntu1  (1000) shubuntu1  (1000)      715 2023-05-04 06:09:39.000000 fc-server-0.5.1/PKG-INFO
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-03-29 08:28:44.000000 fc-server-0.6.0/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:29.000000 fc-server-0.6.0/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2022-08-17 06:53:34.000000 fc-server-0.6.0/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-05 06:30:26.000000 fc-server-0.6.0/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-05 06:29:52.000000 fc-server-0.6.0/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_common/version.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/__init__.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/config/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/config/sample_cfg.yaml
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/config/sample_lavacli.yaml
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/core/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     6466 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/api_svr.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     4037 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    12182 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/coordinator.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/core/decorators.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/core/plugin.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/management/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-03-07 07:55:27.000000 fc-server-0.6.0/fc_server/management/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/management/cmd_online_lava_devices.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-06-30 05:19:57.000000 fc-server-0.6.0/fc_server/management/common.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/plugins/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-07-06 05:36:14.000000 fc-server-0.6.0/fc_server/plugins/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/lava.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server/plugins/utils/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2022-08-17 06:53:34.000000 fc-server-0.6.0/fc_server/plugins/utils/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/utils/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/plugins/utils/lava.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server/server.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-05 06:32:29.000000 fc-server-0.6.0/fc_server_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server_daemon/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1960 2023-06-30 05:20:06.000000 fc-server-0.6.0/fc_server_daemon/server_daemon.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-05 06:32:29.000000 fc-server-0.6.0/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3859 2023-07-05 06:29:52.000000 fc-server-0.6.0/setup.py
```

### Comparing `fc-server-0.5.1/README.rst` & `fc-server-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/setup.cfg` & `fc-server-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/fc_server.egg-info/SOURCES.txt` & `fc-server-0.6.0/fc_server.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 fc_common/VERSION
 fc_common/__init__.py
+fc_common/config.py
+fc_common/etcd.py
+fc_common/logger.py
 fc_common/version.py
 fc_server/__init__.py
 fc_server/server.py
 fc_server.egg-info/PKG-INFO
 fc_server.egg-info/SOURCES.txt
 fc_server.egg-info/dependency_links.txt
 fc_server.egg-info/entry_points.txt
@@ -16,18 +19,19 @@
 fc_server/config/sample_cfg.yaml
 fc_server/config/sample_lavacli.yaml
 fc_server/core/__init__.py
 fc_server/core/api_svr.py
 fc_server/core/config.py
 fc_server/core/coordinator.py
 fc_server/core/decorators.py
-fc_server/core/logger.py
 fc_server/core/plugin.py
 fc_server/management/__init__.py
 fc_server/management/cmd_online_lava_devices.py
 fc_server/management/common.py
 fc_server/plugins/__init__.py
 fc_server/plugins/labgrid.py
 fc_server/plugins/lava.py
 fc_server/plugins/utils/__init__.py
 fc_server/plugins/utils/labgrid.py
-fc_server/plugins/utils/lava.py
+fc_server/plugins/utils/lava.py
+fc_server_daemon/__init__.py
+fc_server_daemon/server_daemon.py
```

### Comparing `fc-server-0.5.1/fc_server.egg-info/PKG-INFO` & `fc-server-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: fc-server
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

### Comparing `fc-server-0.5.1/LICENSE` & `fc-server-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/fc_server/plugins/utils/labgrid.py` & `fc-server-0.6.0/fc_server/plugins/utils/labgrid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2022 NXP
+# Copyright 2022-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import logging
 import traceback
 
@@ -16,28 +16,28 @@
 
 class Labgrid(AsyncRunMixin):
     @which(
         "labgrid-client",
         "Use 'pip3 install labgrid-client' to install labgrid software please.",
     )
     def __init__(self):
-        pass
+        self.logger = logging.getLogger("fc_server")
 
     async def labgrid_get_places(self):
         cmd = "labgrid-client p"
         _, places, _ = await self._run_cmd(cmd)
         return places
 
     async def labgrid_get_reservations(self):
         cmd = "labgrid-client reservations"
         _, reservations_text, _ = await self._run_cmd(cmd)
         try:  # pylint: disable=too-many-nested-blocks
             reservations = yaml.load(reservations_text, Loader=yaml.FullLoader)
         except yaml.YAMLError:
-            logging.error(traceback.format_exc())
+            self.logger.error(traceback.format_exc())
             return
 
         return reservations
 
     async def labgrid_create_reservation(
         self, place, priority=None, wait=False, timeout=None
     ):
@@ -75,7 +75,19 @@
         token = ""
         place_info_lines = place_info_text.splitlines()
         for line in place_info_lines:
             if line.find("reservation") >= 0:
                 token = line.split(":")[-1].strip()
                 break
         return token
+
+    async def labgrid_get_place_owner(self, place):
+        cmd = f"labgrid-client -p {place} show"
+        _, place_info_text, _ = await self._run_cmd(cmd)
+
+        owner = ""
+        place_info_lines = place_info_text.splitlines()
+        for line in place_info_lines:
+            if line.find("acquired:") >= 0:
+                owner = line.split(":")[-1].strip()
+                break
+        return owner
```

### Comparing `fc-server-0.5.1/fc_server/plugins/utils/lava.py` & `fc-server-0.6.0/fc_server/plugins/utils/lava.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2022 NXP
+# Copyright 2022-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=no-member
 
 import asyncio
 import logging
@@ -27,19 +27,21 @@
 class Lava(AsyncRunMixin):
     @which("lavacli", "Use 'pip3 install lavacli' to install lava client please.")
     def __init__(self):
         self.identities = Config.frameworks_config["lava"]["identities"]
         self.device_description_prefix = "[FC]"
         self.lava_default_description = "Created automatically by LAVA."
 
+        self.logger = logging.getLogger("fc_server")
+
     @singledispatchmethod
     async def lava_maintenance_devices(
         self, *devices, desc=None
     ):  # pylint: disable=no-self-use, unused-argument
-        logging.error("unknown type")
+        self.logger.error("unknown type")
 
     @lava_maintenance_devices.register(str)
     @verify_cmd_results
     async def _(self, *devices, desc=None):
         cmd_list = []
         for device in devices:
             cmd = (
@@ -111,15 +113,15 @@
             one_batch_queued_jobs = []
             for queued_jobs_info in queued_jobs_infos:
                 try:
                     one_batch_queued_jobs += yaml.load(
                         queued_jobs_info[1], Loader=yaml.FullLoader
                     )
                 except yaml.YAMLError:
-                    logging.error(traceback.format_exc())
+                    self.logger.error(traceback.format_exc())
 
             queued_jobs += one_batch_queued_jobs
 
             if len(one_batch_queued_jobs) < batch_num * jobs_per_batch:
                 break
 
             seq += 1
@@ -129,39 +131,39 @@
     async def lava_get_job_info(self, job_id):
         cmd = f"lavacli -i {self.identities} jobs show {job_id} --yaml"
         _, job_info_text, _ = await self._run_cmd(cmd)
 
         try:
             job_info = yaml.load(job_info_text, Loader=yaml.FullLoader)
         except yaml.YAMLError:
-            logging.error(traceback.format_exc())
+            self.logger.error(traceback.format_exc())
             return
 
         return job_info
 
     async def lava_get_device_info(self, device):
         cmd = f"lavacli -i {self.identities} devices show {device} --yaml"
         _, device_info_text, _ = await self._run_cmd(cmd)
 
         try:
             device_info = yaml.load(device_info_text, Loader=yaml.FullLoader)
         except yaml.YAMLError:
-            logging.error(traceback.format_exc())
+            self.logger.error(traceback.format_exc())
             return
 
         return device_info
 
     async def lava_get_devices(self):
         cmd = f"lavacli -i {self.identities} devices list --yaml"
         _, devices_text, _ = await self._run_cmd(cmd)
 
         try:
             devices = yaml.load(devices_text, Loader=yaml.FullLoader)
         except yaml.YAMLError:
-            logging.error(traceback.format_exc())
+            self.logger.error(traceback.format_exc())
             return []
 
         return devices
 
     async def lava_cancel_job(self, job_id):
         cmd = f"lavacli -i {self.identities} jobs cancel {job_id}"
         await self._run_cmd(cmd)
```

### Comparing `fc-server-0.5.1/fc_server/plugins/labgrid.py` & `fc-server-0.6.0/fc_server/plugins/labgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import logging
 import os
@@ -31,50 +31,58 @@
         os.environ["LG_HOSTNAME"] = "fc"
         os.environ["LG_USERNAME"] = "fc"
 
         self.managed_resources = None
 
         self.seize_cache = {}  # cache to avoid busy seize
 
+        self.logger = logging.getLogger("fc_server")
+
     @safe_cache
     def __update_cache(self, cache_name, job_id, value):
         self.__dict__[cache_name][job_id] += value
 
     async def __labgrid_guard_reservation(self, resource):
-        logging.info("* [start] inject guard reservation for %s", resource)
+        self.logger.info("* [start] inject guard reservation for %s", resource)
         await self.labgrid_create_reservation(resource, priority=-100)
-        logging.info("* [done] inject guard reservation for %s", resource)
+        self.logger.info("* [done] inject guard reservation for %s", resource)
 
     async def __labgrid_fc_reservation(self, driver, resource):
         # let labgrid coordinator has chance to schedule
         await asyncio.sleep(10)
 
-        logging.info("* [start] inject fc reservation for %s", resource)
+        self.logger.info("* [start] inject fc reservation for %s", resource)
         await self.labgrid_create_reservation(resource, priority=100, wait=True)
         await self.labgrid_acquire_place(resource)
-        logging.info("* [done] inject fc reservation for %s", resource)
+        self.logger.info("* [done] inject fc reservation for %s", resource)
 
         await driver.return_resource(resource)
 
     async def __labgrid_init(self, resource):
         """
         Let FC take over by inject special reservation
         """
         reservations = await self.labgrid_get_reservations()
         if reservations:
             for _, v in reservations.items():  # pylint: disable=invalid-name
                 if v["filters"]["main"] == f"name={resource}":
-                    await self.labgrid_cancel_reservation(v["token"], quiet=True)
+                    await self.labgrid_cancel_reservation(v["token"])
 
-        await self.labgrid_release_place(resource, force=True, quiet=True)
+        await self.labgrid_release_place(resource, force=True)
         await self.labgrid_create_reservation(
             resource, priority=100, wait=True, timeout=20
         )
         await self.labgrid_acquire_place(resource)
 
+        # verify init effect
+        owner = await self.labgrid_get_place_owner(resource)
+        if owner != "fc/fc":
+            self.logger.info("- init %s failure", resource)
+            self.managed_resources.remove(resource)
+
     async def force_kick_off(self, resource):
         """
         Allow coordinator to seize labgrid resource
         """
 
         token = await self.labgrid_get_place_token(resource)
 
@@ -109,15 +117,22 @@
 
         async def switch_from_fc_to_labgrid(resource):
             # there is at most 10 seconds gap there if normal user release its acquired device
             # to avoid empty reservation during this period
             # inject a low priority system reservation
             await self.__labgrid_guard_reservation(resource)
 
-            await self.labgrid_cancel_reservation(managed_resources_tokens[resource])
+            reservation = managed_resources_tokens.get(resource, None)
+            if reservation:
+                await self.labgrid_cancel_reservation(reservation)
+            else:
+                self.logger.warning(
+                    "No reservation for %s found, this possible result in issue",
+                    resource,
+                )
             await self.labgrid_release_place(resource)
 
             # inject a high priority system reservation to let FC lock the device
             # after normal user finish using the device
             asyncio.create_task(self.__labgrid_fc_reservation(driver, resource))
 
         # query labgrid reservations
@@ -184,9 +199,10 @@
 
         places = await self.labgrid_get_places()
         self.managed_resources = [
             place.strip()
             for place in places.splitlines()
             if place.strip() in driver.managed_resources
         ]
+        candidated_init_resources = self.managed_resources.copy()
 
-        return [self.__labgrid_init(resource) for resource in self.managed_resources]
+        return [self.__labgrid_init(resource) for resource in candidated_init_resources]
```

### Comparing `fc-server-0.5.1/fc_server/plugins/lava.py` & `fc-server-0.6.0/fc_server/plugins/lava.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import logging
 
@@ -39,14 +39,16 @@
                 "submitter"
             ]
 
         self.scheduler_cache = {}  # cache to avoid busy scheduling
         self.seize_cache = {}  # cache to avoid busy seize
         self.job_tags_cache = {}  # cache to store job tags
 
+        self.logger = logging.getLogger("fc_server")
+
     @safe_cache
     def __update_cache(self, cache_name, job_id, value):
         self.__dict__[cache_name][job_id] += value
 
     async def __reset_possible_resource(self, driver, *possible_resources):
         """
         Maintenance all devices once devices finish scheduling.
@@ -184,23 +186,23 @@
         """
 
         device_info = await self.__get_device_info(resource, clear=True)
         if not device_info or device_info["current_job"]:
             return False, False
 
         if device_info["health"] == "Maintenance":
-            logging.info("%s default in maintenance.", resource)
+            self.logger.info("%s default in maintenance.", resource)
             return True, False
 
         if device_info["health"] == "Retired":
-            logging.info("%s default in retired.", resource)
+            self.logger.info("%s default in retired.", resource)
             return False, False
 
         # ask default framework disconnect this resource
-        logging.info("Disconnect %s from default framework", resource)
+        self.logger.info("Disconnect %s from default framework", resource)
         desc = await self.__get_device_description(resource)
         if not await self.lava_maintenance_devices(
             resource, desc=f"{self.device_description_prefix}{desc}"
         ):
             return False, False
 
         device_info = await self.__get_device_info(resource, clear=True)
@@ -211,15 +213,15 @@
 
     async def default_framework_connect(self, resource):
         """
         Default framework should realize this to let FC control the connect
         """
 
         # ask default framework connect this resource
-        logging.info("Connect %s to default framework", resource)
+        self.logger.info("Connect %s to default framework", resource)
         desc = await self.__get_device_description(resource)
         return await self.lava_online_devices(
             resource, desc=desc.split(self.device_description_prefix)[-1]
         )
 
     async def schedule(
         self, driver
@@ -302,15 +304,15 @@
                         ]
 
         # category devices
         managed_resources_category = {"available": {}, "non-available": {}}
         devices = await self.lava_get_devices()
 
         if not devices:
-            logging.warning(
+            self.logger.warning(
                 "No device fetched from lava server, delay to next scheduling slot"
             )
             return
 
         if driver.is_default_framework(self):
             async for _ in schedule_prepare():
                 pass
@@ -341,15 +343,15 @@
         # get devices suitable for queued jobs
         queued_jobs.reverse()
         for queued_job in queued_jobs:
             job_id = queued_job["id"]
 
             # delay issue job to next scheduling slot
             if job_id not in self.job_tags_cache:
-                logging.warning("Job %s delayed to next scheduling slot", job_id)
+                self.logger.warning("Job %s delayed to next scheduling slot", job_id)
                 continue
 
             candidated_available_devices = managed_resources_category["available"].get(
                 queued_job["requested_device_type"], []
             )
 
             candidated_available_resources = []
@@ -412,15 +414,15 @@
 
         # let lava dispatch
         if possible_resources:
             for possible_resource in possible_resources:
                 driver.accept_resource(possible_resource, self)
 
             if not driver.is_default_framework(self):
-                logging.info("Online devices to schedule lava jobs.")
+                self.logger.info("Online devices to schedule lava jobs.")
                 await self.lava_online_devices(*possible_resources)
 
             # cleanup
             asyncio.create_task(
                 self.__reset_possible_resource(driver, *possible_resources)
             )
```

### Comparing `fc-server-0.5.1/fc_server/core/coordinator.py` & `fc-server-0.6.0/fc_server/core/coordinator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import logging
 import sys
 from importlib import import_module
 
 from fc_server.core.api_svr import ApiSvr
 from fc_server.core.config import Config
 from fc_server.core.decorators import check_priority_scheduler
+from fc_server_daemon.server_daemon import ServerDaemon
 
 
 class Coordinator:
     """
     FC coordinator which used to coordinate status among different frameworks
     """
 
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self):
+        self.logger = logging.getLogger("fc_server")
+
         self.__framework_plugins = [
             import_module("fc_server.plugins." + framework).Plugin(
                 Config.frameworks_config[framework]
             )
             for framework in Config.registered_frameworks
         ]
 
@@ -37,28 +40,28 @@
 
         self.__framework_seize_strategies = {
             framework: Config.frameworks_config[framework].get("seize", True)
             for framework in Config.registered_frameworks
         }
 
         if Config.default_framework:
-            logging.info("Default framework: %s", Config.default_framework)
+            self.logger.info("Default framework: %s", Config.default_framework)
             for framework in self.__framework_plugins:
                 if framework.__module__.split(".")[-1] == Config.default_framework:
                     self.__default_framework_plugin = framework
                     if not hasattr(
                         self.__default_framework_plugin, "default_framework_disconnect"
                     ) or not hasattr(
                         self.__default_framework_plugin, "default_framework_connect"
                     ):
-                        logging.fatal(
+                        self.logger.fatal(
                             "Fatal: specified default framework doesn't realize next interfaces:"
                         )
-                        logging.fatal("  - default_framework_disconnect")
-                        logging.fatal("  - default_framework_connect")
+                        self.logger.fatal("  - default_framework_disconnect")
+                        self.logger.fatal("  - default_framework_connect")
                         sys.exit(1)
                     break
 
         self.__managed_resources_status = {}
         self.__managed_disconnect_resources = []
         self.__managed_issue_disconnect_resources = []
 
@@ -67,28 +70,28 @@
 
         # assure no seize for this job when already a seize for this job there
         self.coordinating_job_records = {}
 
         # record timeout task for seized status
         self.seized_status_timeout_records = {}
 
-        logging.info("FC managed resource list:")
-        logging.info(Config.managed_resources)
+        self.logger.info("FC managed resource list:")
+        self.logger.info(Config.managed_resources)
 
     async def __init_frameworks(self):
-        logging.info("Start to init following frameworks:")
+        self.logger.info("Start to init following frameworks:")
 
         init_tasks = []
         for framework in self.__framework_plugins:
-            logging.info("  - %s", framework.__module__)
+            self.logger.info("  - %s", framework.__module__)
             init_tasks += await framework.init(self)
 
         await asyncio.gather(*init_tasks)
 
-        logging.info("Framework coordinator ready.")
+        self.logger.info("Framework coordinator ready.")
 
     async def __managed_issue_resources_connect(self):
         for resource in self.__managed_issue_disconnect_resources:
             if await self.__default_framework_plugin.default_framework_connect(
                 resource
             ):
                 self.__managed_issue_disconnect_resources.remove(resource)
@@ -105,15 +108,15 @@
                     await framework.schedule(self)
                 framework.schedule_tick += 1
 
             await asyncio.sleep(1)
 
     async def __action(self):
         await self.__init_frameworks()
-        await ApiSvr(self).start(Config.api_server["port"])
+        await ApiSvr(self).start(**Config.api_server)
         await self.__schedule_frameworks()
 
     @property
     def priority_scheduler(self):
         return Config.priority_scheduler
 
     @property
@@ -201,27 +204,27 @@
 
     def is_seized_job(self, job_id):
         # pylint: disable=consider-iterating-dictionary
         return job_id in list(self.coordinating_job_records.keys())
 
     async def __seized_status_timeout(self, resource):
         await asyncio.sleep(90)
-        logging.info("* %s seized status be reset to fc due to timeout", resource)
+        self.logger.info("* %s seized status be reset to fc due to timeout", resource)
         self.reset_resource(resource)
 
     @check_priority_scheduler()
     async def coordinate_resources(self, context, job_id, *candidated_resources):
         """
         Seize resource from low priority framework
         """
 
         if not candidated_resources:
             return []
 
-        logging.info(
+        self.logger.info(
             "[start] seize resource requirement from %s for %s",
             context.__module__.split(".")[-1],
             job_id,
         )
 
         candidated_seized_resources = [
             candidated_resource
@@ -245,15 +248,15 @@
                     framework.__module__.split(".")[-1]
                     == self.managed_resources_status[candidated_seized_resource]
                 ):
                     self.__set_resource_status(
                         candidated_seized_resource,
                         context.__module__.split(".")[-1] + "_seizing",
                     )
-                    logging.info(
+                    self.logger.info(
                         "Force kick off the resource %s.", candidated_seized_resource
                     )
                     await framework.force_kick_off(candidated_seized_resource)
                     self.__set_resource_status(
                         candidated_seized_resource,
                         context.__module__.split(".")[-1] + "_seized",
                     )
@@ -265,25 +268,25 @@
                     self.seized_status_timeout_records[
                         candidated_seized_resource
                     ] = timeout_task
 
                     break
             low_priority_resources.append(candidated_seized_resource)
 
-        logging.info(
+        self.logger.info(
             "[done] seize resource requirement from %s for %s",
             context.__module__.split(".")[-1],
             job_id,
         )
 
         return high_priority_resources + low_priority_resources
 
     def __set_resource_status(self, resource, status):
         self.__managed_resources_status[resource] = status
-        logging.info("* %s now belongs to %s", resource, status)
+        self.logger.info("* %s now belongs to %s", resource, status)
 
     async def return_resource(self, resource):
         if (
             self.__managed_resources_status.get(resource, "")
             in Config.registered_frameworks
         ):
             self.__set_resource_status(resource, "fc")
@@ -308,8 +311,18 @@
     def retire_resource(self, resource):
         self.__set_resource_status(resource, "retired")
 
     def reset_resource(self, resource):
         self.__set_resource_status(resource, "fc")
 
     def start(self):
+        if Config.cluster["enable"]:
+            daemon_paras = {
+                "etcd": Config.cluster["etcd"],
+                "instance_name": Config.cluster["instance_name"],
+                "fc": f"http://{Config.api_server['ip']}:{Config.api_server['port']}",
+                "lg": Config.frameworks_config["labgrid"]["lg_crossbar"],
+                "devices": Config.managed_resources,
+            }
+            ServerDaemon(daemon_paras).run()
+
         asyncio.run(self.__action())
```

### Comparing `fc-server-0.5.1/fc_server/core/api_svr.py` & `fc-server-0.6.0/fc_server/core/api_svr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import logging
 from contextlib import suppress
@@ -21,14 +21,15 @@
     """
     Rest api server
     """
 
     def __init__(self, context):
         self.context = context
         self.external_info_tool = Config.api_server.get("external_info_tool", "")
+        self.logger = logging.getLogger("fc_server")
 
     @staticmethod
     def friendly_status(status):
         with suppress(Exception):
             return Config.frameworks_config[status]["friendly_status"]
         return status
 
@@ -149,22 +150,33 @@
                 continue
 
             if booking_text[anchor:].split(" ")[0] in Config.managed_resources:
                 bookings_text_list.append(booking_text)
 
         return web.Response(text="\n".join(bookings_text_list))
 
-    async def start(self, port):
+    async def start(self, **svr_args):
         app = web.Application()
+
+        access_logger = logging.getLogger("aiohttp.access")
+        access_logger.setLevel(logging.INFO)
+        handler = logging.StreamHandler()
+        s_format = logging.Formatter(
+            fmt="%(asctime)s %(message)s",
+            datefmt="%Y-%m-%d %H:%M:%S",
+        )
+        handler.setFormatter(s_format)
+        access_logger.addHandler(handler)
+
         app.add_routes([web.get("/ping", self.pong)])
         app.add_routes([web.get("/booking", self.booking)])
         app.add_routes([web.get("/resource", self.resource_status)])
         app.add_routes([web.get("/resource/{res}", self.resource_status)])
 
         app_runner = web.AppRunner(app)
         await app_runner.setup()
 
-        api_interface = "0.0.0.0"
-        api_port = port
+        api_interface = svr_args["ip"]
+        api_port = svr_args["port"]
         loop = asyncio.get_event_loop()
         await loop.create_server(app_runner.server, api_interface, api_port)
-        logging.info("Api Server ready at http://%s:%d.", api_interface, api_port)
+        self.logger.info("Api Server ready at http://%s:%d.", api_interface, api_port)
```

### Comparing `fc-server-0.5.1/fc_server/core/decorators.py` & `fc-server-0.6.0/fc_server/core/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import logging
 from functools import wraps
 
+logger = logging.getLogger("fc_server")
+
 
 def safe_cache(func):
     @wraps(func)
     def decorator(*args):
         if args[2] not in args[0].__dict__[args[1]]:
             args[0].__dict__[args[1]][args[2]] = []
         return func(*args)
@@ -65,14 +67,14 @@
     async def decorator(*args, desc=None):
         results, cmd_list = await func(*args, desc=desc)
 
         i = 0
         for result in results:
             device_update_response = result[1]
             if device_update_response != "":
-                logging.error(cmd_list[i])
-                logging.error(device_update_response)
+                logger.error(cmd_list[i])
+                logger.error(device_update_response)
                 return False
             i += 1
         return True
 
     return decorator
```

### Comparing `fc-server-0.5.1/fc_server/core/__init__.py` & `fc-server-0.6.0/fc_server/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import asyncio
 import os
 
+from fc_common.logger import Logger
 from fc_server.core.config import Config
-from fc_server.core.logger import Logger
 
 fc_path = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-Logger.init(fc_path)
+Logger.init("fc_server", "fc_server.log")
 Config.parse(fc_path)
 
 
 class AsyncRunMixin:  # pylint: disable=too-few-public-methods
     """
     Mixin for async subprocess call
     """
@@ -24,12 +24,12 @@
     async def _run_cmd(self, cmd):  # pylint: disable=no-self-use
         proc = await asyncio.create_subprocess_shell(
             cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
         )
         stdout, stderr = await proc.communicate()
 
         if proc.returncode != 0:
-            print(f"[{cmd!r} exited with {proc.returncode}]")
+            print(f"{cmd!r}:\n  - exited with {proc.returncode}")
         if stderr:
-            print(f"[{cmd!r} stderr]\n{stderr.decode()}")
+            print(f"  - {stderr.decode()}")
 
         return proc.returncode, stdout.decode(), stderr.decode()
```

### Comparing `fc-server-0.5.1/fc_server/core/plugin.py` & `fc-server-0.6.0/fc_server/core/plugin.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/fc_server/server.py` & `fc-server-0.6.0/fc_server/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# Copyright 2021-2022 NXP
+# Copyright 2021-2023 NXP
 #
 # SPDX-License-Identifier: MIT
 
 
 import logging
 
 from fc_common.version import get_runtime_version
@@ -17,15 +17,16 @@
 ______                                           _    _____                     _ _             _
 |  ___|                                         | |  /  __ \                   | (_)           | |
 | |_ _ __ __ _ _ __ ___   _____      _____  _ __| | _| /  \/ ___   ___  _ __ __| |_ _ __   __ _| |_ ___  _ __
 |  _| '__/ _` | '_ ` _ \ / _ \ \ /\ / / _ \| '__| |/ / |    / _ \ / _ \| '__/ _` | | '_ \ / _` | __/ _ \| '__|
 | | | | | (_| | | | | | |  __/\ V  V / (_) | |  |   <| \__/\ (_) | (_) | | | (_| | | | | | (_| | || (_) | |
 \_| |_|  \__,_|_| |_| |_|\___| \_/\_/ \___/|_|  |_|\_\\____/\___/ \___/|_|  \__,_|_|_| |_|\__,_|\__\___/|_|
     """
-    logging.info(product_text)
-    logging.info("VERSION: %s", get_runtime_version("fc-server"))
+    logger = logging.getLogger("fc_server")
+    logger.info(product_text)
+    logger.info("VERSION: %s", get_runtime_version("fc-server"))
 
     Coordinator().start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fc-server-0.5.1/fc_server/management/cmd_online_lava_devices.py` & `fc-server-0.6.0/fc_server/management/cmd_online_lava_devices.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/fc_common/version.py` & `fc-server-0.6.0/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.5.1/setup.py` & `fc-server-0.6.0/setup.py`

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

### Comparing `fc-server-0.5.1/PKG-INFO` & `fc-server-0.6.0/fc_server.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: fc-server
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

