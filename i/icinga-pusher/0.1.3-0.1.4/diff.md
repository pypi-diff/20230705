# Comparing `tmp/icinga_pusher-0.1.3.tar.gz` & `tmp/icinga_pusher-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icinga_pusher-0.1.3.tar", max compression
+gzip compressed data, was "icinga_pusher-0.1.4.tar", max compression
```

## Comparing `icinga_pusher-0.1.3.tar` & `icinga_pusher-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.3/README.md
--rw-r--r--   0        0        0     2910 2023-07-04 15:40:12.727028 icinga_pusher-0.1.3/icinga_pusher/__init__.py
--rw-r--r--   0        0        0      388 2023-07-04 17:24:49.400246 icinga_pusher-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.4/README.md
+-rw-r--r--   0        0        0     2941 2023-07-05 07:18:27.726873 icinga_pusher-0.1.4/icinga_pusher/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-05 07:18:50.280101 icinga_pusher-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.4/PKG-INFO
```

### Comparing `icinga_pusher-0.1.3/LICENSE` & `icinga_pusher-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icinga_pusher-0.1.3/icinga_pusher/__init__.py` & `icinga_pusher-0.1.4/icinga_pusher/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import os
 import requests
 import logging
 from typing import Optional
 
-logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger("icinga_pusher")
+logger.setLevel(logging.INFO)
 
 ICINGA_DRY_RUN = "ICINGA_DRY_RUN"
 
 
 class IcingaService(object):
 
     def __init__(self, icinga, mon_host, service):
         self.icinga = icinga
         self.mon_host = mon_host
         self.service = service
 
     def push_state(self, exit_status: int, plugin_output: str, performance_data: Optional[list] = None):
 
         if ICINGA_DRY_RUN in os.environ:
-            logging.debug("Env ICINGA_DRY_RUN is set. Not pushing Icinga state")
+            logger.debug("Env ICINGA_DRY_RUN is set. Not pushing Icinga state")
             return
 
         if type(exit_status) != int:
             raise TypeError(f"exit_status must be an int ({exit_status=})")
 
         headers = {
             "Accept": "application/json",
@@ -45,17 +46,17 @@
             resp = requests.post(f"{self.icinga.hostname}:5665/v1/actions/process-check-result",
                                  json=data,
                                  headers=headers,
                                  verify=self.icinga.ssl_verify,
                                  auth=(self.icinga.username, self.icinga.password))
             resp.raise_for_status()
         except requests.exceptions.RequestException as e:
-            logging.error(f"Could not set Icinga status of service {self.service}. {e}. Response: {e.response.text}")
+            logger.error(f"Could not set Icinga status of service {self.service}. {e}. Response: {e.response.text}")
         else:
-            logging.info(f"Sucessfully set Icinga status for service {self.service}")
+            logger.info(f"Sucessfully set Icinga status for service {self.service}")
 
 
 class Icinga(object):
     CHECK_OK = 0
     CHECK_WARNING = 1
     CHECK_CRITICAL = 2
     CHECK_UNKNOWN = 3
```

