# Comparing `tmp/mdast_cli-2023.6.1.tar.gz` & `tmp/mdast_cli-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.6.1.tar", last modified: Tue Jun  6 14:47:12 2023, max compression
+gzip compressed data, was "mdast_cli-2023.7.1.tar", last modified: Wed Jul  5 14:26:48 2023, max compression
```

## Comparing `mdast_cli-2023.6.1.tar` & `mdast_cli-2023.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.333451 mdast_cli-2023.6.1/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.333451 mdast_cli-2023.6.1/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.333451 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.333451 mdast_cli-2023.6.1/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-06 14:47:12.000000 mdast_cli-2023.6.1/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 14:47:12.337451 mdast_cli-2023.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-06 14:46:54.000000 mdast_cli-2023.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3656 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15572 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.352256 mdast_cli-2023.7.1/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-05 14:26:48.000000 mdast_cli-2023.7.1/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 14:26:48.356256 mdast_cli-2023.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-05 14:26:23.000000 mdast_cli-2023.7.1/setup.py
```

### Comparing `mdast_cli-2023.6.1/PKG-INFO` & `mdast_cli-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast_cli
-Version: 2023.6.1
+Version: 2023.7.1
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.6.1/README.md` & `mdast_cli-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/app_center.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appgallery.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/firebase.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/firebase.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/google_play.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,16 @@
             if params.get("auth"):
                 ac2dmToken = params.get("auth")
             elif "error" in params:
                 if "NeedsBrowser" in params["error"]:
                     url = params.get('url') or 'https://accounts.google.com/b/0/DisplayUnlockCaptcha'
                     raise RuntimeError(f'Google Play - Error {params["error"]}. '
                                        f'Security check is needed, try to visit {url} to unlock.')
+                else:
+                    raise RuntimeError(f'Google Play - Error {params["error"]}.')
 
             self.gsfId = self.checkin(email, ac2dmToken)
             self.getAuthSubToken(email, encryptedPass)
             self.uploadDeviceConfig()
             logger.info(f'Google Play - gsfId: {self.gsfId}, authSubToken: {self.authSubToken}')
             logger.info('Google Play - You should copy these parameters and use them for next scans instead '
                         'of email and password:')
```

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.7.1/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/helpers/const.py` & `mdast_cli-2023.7.1/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli/mdast_scan.py` & `mdast_cli-2023.7.1/mdast_cli/mdast_scan.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.7.1/mdast_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdast-cli
-Version: 2023.6.1
+Version: 2023.7.1
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli-2023.6.1/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.7.1/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.7.1/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli_core/api.py` & `mdast_cli-2023.7.1/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli_core/base.py` & `mdast_cli-2023.7.1/mdast_cli_core/base.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/mdast_cli_core/token.py` & `mdast_cli-2023.7.1/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.6.1/setup.py` & `mdast_cli-2023.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.06.01',
+    version='2023.07.01',
 
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

