# Comparing `tmp/nc_py_api-0.0.21.tar.gz` & `tmp/nc_py_api-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.21.tar", last modified: Mon Jul  3 20:47:18 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.22.tar", last modified: Wed Jul  5 10:24:16 2023, max compression
```

## Comparing `nc_py_api-0.0.21.tar` & `nc_py_api-0.0.22.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.208260 nc_py_api-0.0.21/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12320 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-03 20:47:18.000000 nc_py_api-0.0.21/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 20:47:10.000000 nc_py_api-0.0.21/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-03 20:47:18.212260 nc_py_api-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-03 20:47:01.000000 nc_py_api-0.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12320 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-05 10:24:16.000000 nc_py_api-0.0.22/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 10:24:09.000000 nc_py_api-0.0.22/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-05 10:24:16.651228 nc_py_api-0.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-05 10:24:01.000000 nc_py_api-0.0.22/setup.py
```

### Comparing `nc_py_api-0.0.21/LICENSE` & `nc_py_api-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/PKG-INFO` & `nc_py_api-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc_py_api
-Version: 0.0.21
+Version: 0.0.22
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.21/README.md` & `nc_py_api-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/_session.py` & `nc_py_api-0.0.22/nc_py_api/_session.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.22/nc_py_api/appconfig_preferences_ex.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/apps.py` & `nc_py_api-0.0.22/nc_py_api/apps.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/constants.py` & `nc_py_api-0.0.22/nc_py_api/constants.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/exceptions.py` & `nc_py_api-0.0.22/nc_py_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/files.py` & `nc_py_api-0.0.22/nc_py_api/files.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.22/nc_py_api/integration_fastapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,7 +33,13 @@
     @fast_api_app.put("/enabled")
     def enabled_handler(
         enabled: bool,
         nc: Annotated[NextcloudApp, Depends(nc_app)],
     ):
         r = callback(enabled, nc)
         return JSONResponse(content={"error": r}, status_code=200)
+
+
+def enable_heartbeat(fast_api_app: FastAPI):
+    @fast_api_app.get("/heartbeat")
+    def heartbeat_handler():
+        return JSONResponse(content={"status": "ok"}, status_code=200)
```

### Comparing `nc_py_api-0.0.21/nc_py_api/misc.py` & `nc_py_api-0.0.22/nc_py_api/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/nextcloud.py` & `nc_py_api-0.0.22/nc_py_api/nextcloud.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/preferences.py` & `nc_py_api-0.0.22/nc_py_api/preferences.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/theming.py` & `nc_py_api-0.0.22/nc_py_api/theming.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.22/nc_py_api/ui_files_actions_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/users.py` & `nc_py_api-0.0.22/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/users_groups.py` & `nc_py_api-0.0.22/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/users_status.py` & `nc_py_api-0.0.22/nc_py_api/users_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api/weather_status.py` & `nc_py_api-0.0.22/nc_py_api/weather_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.22/nc_py_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nc-py-api
-Version: 0.0.21
+Version: 0.0.22
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
 License: Apache License 3.0
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
```

### Comparing `nc_py_api-0.0.21/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.22/nc_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/pyproject.toml` & `nc_py_api-0.0.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.21/setup.cfg` & `nc_py_api-0.0.22/setup.cfg`

 * *Files identical despite different names*

