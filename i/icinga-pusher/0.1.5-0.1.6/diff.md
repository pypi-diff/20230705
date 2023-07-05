# Comparing `tmp/icinga_pusher-0.1.5.tar.gz` & `tmp/icinga_pusher-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icinga_pusher-0.1.5.tar", max compression
+gzip compressed data, was "icinga_pusher-0.1.6.tar", max compression
```

## Comparing `icinga_pusher-0.1.5.tar` & `icinga_pusher-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.5/README.md
--rw-r--r--   0        0        0     3012 2023-07-05 07:28:12.812974 icinga_pusher-0.1.5/icinga_pusher/__init__.py
--rw-r--r--   0        0        0      388 2023-07-05 07:28:32.582937 icinga_pusher-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-04 15:40:12.723695 icinga_pusher-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-04 15:40:12.727028 icinga_pusher-0.1.6/README.md
+-rw-r--r--   0        0        0     3044 2023-07-05 07:44:38.557646 icinga_pusher-0.1.6/icinga_pusher/__init__.py
+-rw-r--r--   0        0        0      388 2023-07-05 07:44:56.444349 icinga_pusher-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 icinga_pusher-0.1.6/PKG-INFO
```

### Comparing `icinga_pusher-0.1.5/LICENSE` & `icinga_pusher-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `icinga_pusher-0.1.5/icinga_pusher/__init__.py` & `icinga_pusher-0.1.6/icinga_pusher/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                                  json=data,
                                  headers=headers,
                                  verify=self.icinga.ssl_verify,
                                  auth=(self.icinga.username, self.icinga.password))
             resp.raise_for_status()
         except requests.exceptions.RequestException as e:
             logger.error(f"Could not set Icinga status of service {self.service}. {e}")
-            if hasattr(e, "response"):
+            if hasattr(e, "response") and hasattr(e.response, "text"):
                 logger.error(f"Response: {e.response.text}")
         else:
             logger.info(f"Sucessfully set Icinga status for service {self.service}")
 
 
 class Icinga(object):
     CHECK_OK = 0
```

