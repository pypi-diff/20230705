# Comparing `tmp/globus-compute-sdk-2.2.1.tar.gz` & `tmp/globus-compute-sdk-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.2.1.tar", last modified: Fri Jun 23 01:03:43 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.2.3a0.tar", last modified: Wed Jul  5 15:36:03 2023, max compression
```

## Comparing `globus-compute-sdk-2.2.1.tar` & `globus-compute-sdk-2.2.3a0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.700949 globus-compute-sdk-2.2.1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1819 2023-06-23 01:03:43.701006 globus-compute-sdk-2.2.1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.1/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.693707 globus-compute-sdk-2.2.1/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.694735 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.696785 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1276 2023-06-21 18:50:27.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.697351 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    27030 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46344 2023-06-05 19:33:47.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.699432 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     3012 2023-05-05 16:40:44.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.699716 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8443 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.700708 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      603 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1412 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7869 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     4848 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-05-08 21:56:13.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      832 2023-06-23 00:58:49.000000 globus-compute-sdk-2.2.1/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:43.694321 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1819 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1577 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      397 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-06-23 01:03:43.000000 globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-23 01:03:43.701241 globus-compute-sdk-2.2.1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3161 2023-06-21 18:50:25.000000 globus-compute-sdk-2.2.1/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.453345 globus-compute-sdk-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     1821 2023-07-05 15:36:03.453443 globus-compute-sdk-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      816 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/PyPI.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.445677 globus-compute-sdk-2.2.3a0/globus_compute_sdk/
+-rw-r--r--   0 yadu       (501) staff       (20)      433 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.446898 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/
+-rw-r--r--   0 yadu       (501) staff       (20)      320 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1921 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.448628 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1384 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.449560 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      648 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 yadu       (501) staff       (20)      724 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11458 2023-04-24 17:52:07.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2262 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 yadu       (501) staff       (20)    27050 2023-06-30 20:13:26.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2400 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 yadu       (501) staff       (20)    46344 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.451776 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 yadu       (501) staff       (20)      237 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1787 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 yadu       (501) staff       (20)      855 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 yadu       (501) staff       (20)      373 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 yadu       (501) staff       (20)      954 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7287 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)      710 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3012 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2190 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.452128 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 yadu       (501) staff       (20)      212 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1207 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 yadu       (501) staff       (20)     8561 2023-07-05 15:19:44.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.453067 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/
+-rw-r--r--   0 yadu       (501) staff       (20)      603 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1412 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7869 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 yadu       (501) staff       (20)     4848 2023-06-16 15:43:21.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/utils.py
+-rw-r--r--   0 yadu       (501) staff       (20)      834 2023-07-05 15:25:26.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:03.446516 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     1821 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     1577 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      397 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       19 2023-07-05 15:36:03.000000 globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-05 15:36:03.453803 globus-compute-sdk-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     3161 2023-06-12 16:33:52.000000 globus-compute-sdk-2.2.3a0/setup.py
```

### Comparing `globus-compute-sdk-2.2.1/LICENSE` & `globus-compute-sdk-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/PKG-INFO` & `globus-compute-sdk-2.2.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.1
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.1/PyPI.md` & `globus-compute-sdk-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/_environments.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,20 @@
         os.getenv("FUNCX_SDK_ENVIRONMENT", "production"),
     )
 
 
 def get_web_service_url(envname: str | None) -> str:
     env = envname or _get_envname()
     urls = {
-        "production": "https://compute.api.globus.org/v2",
-        "dev": "https://api.dev.funcx.org/v2",
-        "local": "http://localhost:5000/v2",
+        "production": "https://compute.api.globus.org",
+        "dev": "https://api.dev.funcx.org",
+        "local": "http://localhost:5000",
     }
     for test_env in ["sandbox", "test", "integration", "staging", "preview"]:
-        urls[test_env] = f"https://compute.api.{test_env}.globuscs.info/v2"
+        urls[test_env] = f"https://compute.api.{test_env}.globuscs.info"
 
     return urls.get(env, urls["production"])
 
 
 def get_web_socket_url(envname: str | None) -> str:
     env = envname or _get_envname()
     urls = {
@@ -34,7 +34,12 @@
     }
     return urls.get(env, urls["production"])
 
 
 def urls_might_mismatch(service_url: str, socket_url: str) -> bool:
     parsed_service, parsed_socket = urlparse(service_url), urlparse(socket_url)
     return parsed_service.hostname != parsed_socket.hostname
+
+
+def remove_url_path(url: str):
+    parsed_url = urlparse(url)
+    return f"{parsed_url.scheme}://{parsed_url.netloc}"
```

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
         Returns
         -------
         int
             The port to connect to and a list of containers
         """
         data = {"endpoint_name": name, "description": description}
 
-        r = self.web_client.post("get_containers", data=data)
+        r = self.web_client.post("/v2/get_containers", data=data)
         return r.data["endpoint_uuid"], r.data["endpoint_containers"]
 
     @requires_login
     def get_container(self, container_uuid, container_type):
         """Get the details of a container for staging it locally.
 
         Parameters
@@ -552,15 +552,15 @@
         Returns
         -------
         dict
             The details of the containers to deploy
         """
         self.version_check()
 
-        r = self.web_client.get(f"containers/{container_uuid}/{container_type}")
+        r = self.web_client.get(f"/v2/containers/{container_uuid}/{container_type}")
         return r.data["container"]
 
     @requires_login
     def get_endpoint_status(self, endpoint_uuid):
         """Get the status reports for an endpoint.
 
         Parameters
@@ -688,15 +688,15 @@
         payload = {
             "name": name,
             "location": location,
             "description": description,
             "type": container_type,
         }
 
-        r = self.web_client.post("containers", data=payload)
+        r = self.web_client.post("/v2/containers", data=payload)
         return r.data["container_id"]
 
     @requires_login
     def build_container(self, container_spec):
         """
         Submit a request to build a docker image based on a container spec. This
         container build service is based on repo2docker, so the spec reflects features
@@ -717,19 +717,19 @@
             UUID of the container which can be used to register your function
 
         Raises
         ------
         ContainerBuildForbidden
             User is not in the globus group that protects the build
         """
-        r = self.web_client.post("containers/build", data=container_spec.to_json())
+        r = self.web_client.post("/v2/containers/build", data=container_spec.to_json())
         return r.data["container_id"]
 
     def get_container_build_status(self, container_id):
-        r = self.web_client.get(f"containers/build/{container_id}")
+        r = self.web_client.get(f"/v2/containers/build/{container_id}")
         if r.http_status == 200:
             return r["status"]
         elif r.http_status == 404:
             raise ValueError(f"Container ID {container_id} not found")
         else:
             message = (
                 f"Exception in fetching build status. HTTP Error Code "
```

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/sdk/web_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import json
 import typing as t
 import uuid
 
 import globus_sdk
 from globus_compute_common.sdk_version_sharing import user_agent_substring
-from globus_compute_sdk.sdk._environments import get_web_service_url
+from globus_compute_sdk.sdk._environments import get_web_service_url, remove_url_path
 from globus_compute_sdk.serialize import ComputeSerializer
 from globus_compute_sdk.version import __version__
 from globus_sdk.exc.api import GlobusAPIError
 
 ID_PARAM_T = t.Union[uuid.UUID, str]
 
 
@@ -87,41 +87,44 @@
         environment: t.Optional[str] = None,
         base_url: t.Optional[str] = None,
         app_name: t.Optional[str] = None,
         **kwargs,
     ):
         if base_url is None:
             base_url = get_web_service_url(environment)
+        base_url = remove_url_path(base_url)
+
         super().__init__(environment=environment, base_url=base_url, **kwargs)
+
         self._user_app_name = None
         self.user_app_name = app_name
 
     def get_version(self, *, service: str = "all") -> globus_sdk.GlobusHTTPResponse:
-        return self.get("version", query_params={"service": service})
+        return self.get("/v2/version", query_params={"service": service})
 
     def get_taskgroup_tasks(
         self, task_group_id: ID_PARAM_T
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.get(f"/taskgroup/{task_group_id}")
+        return self.get(f"/v2/taskgroup/{task_group_id}")
 
     def get_task(self, task_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.get(f"tasks/{task_id}")
+        return self.get(f"/v2/tasks/{task_id}")
 
     def get_batch_status(
         self,
         task_ids: t.Iterable[ID_PARAM_T],
         *,
         additional_fields: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> globus_sdk.GlobusHTTPResponse:
         if isinstance(task_ids, str):
             task_ids = [task_ids]
         data = {"task_ids": [str(t) for t in task_ids]}
         if additional_fields is not None:
             data.update(additional_fields)
-        return self.post("/batch_status", data=data)
+        return self.post("/v2/batch_status", data=data)
 
     # the Client needs to send version information through BaseClient.app_name,
     # so that's overridden here to prevent direct manipulation. use user_app_name
     # instead to send any custom metadata through the User Agent request header
     @property
     def app_name(self) -> t.Optional[str]:
         return super().app_name
@@ -140,15 +143,15 @@
         self._user_app_name = value
         app_name = user_agent_substring(__version__)
         if value is not None:
             app_name += f"/{value}"
         globus_sdk.BaseClient.app_name.fset(self, app_name)
 
     def submit(self, batch: t.Dict[str, t.Any]) -> globus_sdk.GlobusHTTPResponse:
-        return self.post("submit", data=batch)
+        return self.post("/v2/submit", data=batch)
 
     def register_endpoint(
         self,
         endpoint_name: str,
         endpoint_id: ID_PARAM_T,
         *,
         metadata: t.Optional[dict] = None,
@@ -172,59 +175,59 @@
         if multi_tenant:
             data["multi_tenant"] = multi_tenant
 
         if metadata:
             data["metadata"] = metadata
         if additional_fields is not None:
             data.update(additional_fields)
-        return self.post("/endpoints", data=data)
+        return self.post("/v2/endpoints", data=data)
 
     def get_result_amqp_url(self) -> globus_sdk.GlobusHTTPResponse:
-        return self.get("get_amqp_result_connection_url")
+        return self.get("/v2/get_amqp_result_connection_url")
 
     def get_endpoint_status(
         self, endpoint_id: ID_PARAM_T
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.get(f"endpoints/{endpoint_id}/status")
+        return self.get(f"/v2/endpoints/{endpoint_id}/status")
 
     def get_endpoint_metadata(
         self, endpoint_id: ID_PARAM_T
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.get(f"endpoints/{endpoint_id}")
+        return self.get(f"/v2/endpoints/{endpoint_id}")
 
     def get_endpoints(self) -> globus_sdk.GlobusHTTPResponse:
-        return self.get("/endpoints")
+        return self.get("/v2/endpoints")
 
     def register_function(
         self,
         function_registration_data: t.Union[
             t.Dict[str, t.Any], FunctionRegistrationData
         ],
     ) -> globus_sdk.GlobusHTTPResponse:
         data = (
             function_registration_data.to_dict()
             if isinstance(function_registration_data, FunctionRegistrationData)
             else function_registration_data
         )
-        return self.post("/functions", data=data)
+        return self.post("/v2/functions", data=data)
 
     def get_whitelist(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.get(f"/endpoints/{endpoint_id}/whitelist")
+        return self.get(f"/v2/endpoints/{endpoint_id}/whitelist")
 
     def whitelist_add(
         self, endpoint_id: ID_PARAM_T, function_ids: t.Iterable[ID_PARAM_T]
     ) -> globus_sdk.GlobusHTTPResponse:
         if isinstance(function_ids, str):
             function_ids = [function_ids]
         data = {"func": [str(f) for f in function_ids]}
-        return self.post(f"/endpoints/{endpoint_id}/whitelist", data=data)
+        return self.post(f"/v2/endpoints/{endpoint_id}/whitelist", data=data)
 
     def whitelist_remove(
         self, endpoint_id: ID_PARAM_T, function_id: ID_PARAM_T
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.delete(f"/endpoints/{endpoint_id}/whitelist/{function_id}")
+        return self.delete(f"/v2/endpoints/{endpoint_id}/whitelist/{function_id}")
 
     def stop_endpoint(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(f"/endpoints/{endpoint_id}/lock", data={})
+        return self.post(f"/v2/endpoints/{endpoint_id}/lock", data={})
 
     def delete_endpoint(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.delete(f"/endpoints/{endpoint_id}")
+        return self.delete(f"/v2/endpoints/{endpoint_id}")
```

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/__init__.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk/version.py` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.1"
+__version__ = "2.2.3a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.1
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.1/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.2.3a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.1/setup.py` & `globus-compute-sdk-2.2.3a0/setup.py`

 * *Files identical despite different names*

