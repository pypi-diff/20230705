# Comparing `tmp/pasqal-cloud-0.3.2.tar.gz` & `tmp/pasqal-cloud-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.3.2.tar", last modified: Mon Jul  3 13:26:26 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.3.tar", last modified: Wed Jul  5 14:05:54 2023, max compression
```

## Comparing `pasqal-cloud-0.3.2.tar` & `pasqal-cloud-0.3.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 13:26:26.413693 pasqal-cloud-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.3.2/LICENSE` & `pasqal-cloud-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/PKG-INFO` & `pasqal-cloud-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.2
+Version: 0.3.3
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.2/README.md` & `pasqal-cloud-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.3/pasqal_cloud/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 import time
 from typing import Any, Dict, List, Optional
 from warnings import warn
 
 from pasqal_cloud.authentication import TokenProvider
 from pasqal_cloud.batch import Batch, RESULT_POLLING_INTERVAL
 from pasqal_cloud.client import Client
-from pasqal_cloud.device import BaseConfig
-from pasqal_cloud.device import EmulatorType
-from pasqal_cloud.endpoints import Auth0Conf, Endpoints, PASQAL_ENDPOINTS, AUTH0_CONFIG
+from pasqal_cloud.device import BaseConfig, EmulatorType
+from pasqal_cloud.endpoints import AUTH0_CONFIG, Auth0Conf, Endpoints, PASQAL_ENDPOINTS
 from pasqal_cloud.job import Job
 
 
 class SDK:
     _client: Client
 
     def __init__(
@@ -45,33 +44,33 @@
         To authenticate to PASQAL Cloud, you have to provide either an
         email/password combination or a TokenProvider instance.
         You may omit the password, you will then be prompted to enter one.
 
         Args:
             username: email of the user to login as.
             password: password of the user to login as.
-            token_provider: The token provider is an alternative log-in method not for human users.
+            token_provider: The token provider is an alternative log-in method \
+                not for human users.
             webhook: Webhook where the job results are automatically sent to.
             endpoints: Endpoints targeted of the public apis.
             auth0: Auth0Config object to define the auth0 tenant to target.
             project_id: ID of the owner project of the batch.
             group_id (deprecated): Use project_id instead.
         """
 
-        # Ticket (#622), to be removed, used to avoid a breaking change during the group to project renaming
+        # Ticket (#622), to be removed,
+        # used to avoid a breaking change during the group to project renaming
         if not project_id:
             if not group_id:
                 raise TypeError(
                     "Either a 'group_id' or 'project_id' has to be given as argument"
                 )
             warn(
-                (
-                    "The parameter 'group_id' is deprecated, from now on use"
-                    " 'project_id' instead"
-                ),
+                "The parameter 'group_id' is deprecated, from now on use"
+                " 'project_id' instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
             project_id = group_id
 
         self._client = Client(
             project_id=project_id,
@@ -102,23 +101,25 @@
             jobs: List of jobs to be added to the batch at creation.
                 (#TODO: Make optional after Iroise MVP)
             emulator: The type of emulator to use,
               If set to None, the device_type will be set to the one
               stored in the serialized sequence
             configuration: A dictionary with extra configuration for the emulators
                 that accept it.
-            wait: Whether to wait for the batch to be done
+            wait: Whether to wait for the batch to be done and fetch results
+            fetch_results (Deprecated): Whether to wait for the batch to be done and fetch results
 
 
         Returns:
             Batch: The new batch that has been created in the database.
         """
         if fetch_results:
             warn(
-                ("The parameter fetch_results has no effect and is deprecated."),
+                "Argument `fetch_results` is deprecated and will be removed in a future"
+                " version. Please use argument `wait` instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         req = {
             "sequence_builder": serialized_sequence,
             "webhook": self.webhook,
@@ -133,15 +134,15 @@
         # The configuration field is only added in the case
         # it's requested
         if configuration:
             req.update({"configuration": configuration.to_dict()})  # type: ignore
 
         batch_rsp = self._client._send_batch(req)
         batch_id = batch_rsp["id"]
-        if wait:
+        if wait or fetch_results:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 batch_rsp = self._client._get_batch(batch_id)
 
         batch = Batch(**batch_rsp, _client=self._client)
 
         self.batches[batch.id] = batch
@@ -154,15 +155,16 @@
             id: ID of the batch.
 
         Returns:
             Batch: the batch stored in the PCS database.
         """
         if fetch_results:
             warn(
-                ("The parameter fetch_results has no effect and is deprecated."),
+                "Argument `fetch_results` is deprecated and will be removed in a future"
+                " version. Results are fetched anyway with this function.",
                 DeprecationWarning,
                 stacklevel=2,
             )
         batch_rsp = self._client._get_batch(id)
         batch = Batch(**batch_rsp, _client=self._client)
         self.batches[batch.id] = batch
         return batch
```

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.3/pasqal_cloud/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.3/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.3/pasqal_cloud/batch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import time
 from typing import Any, Dict, Optional, Type, Union
 
 from pydantic import BaseModel, Extra, root_validator, validator
 
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import EmulatorType
-from pasqal_cloud.device.configuration import (
-    BaseConfig,
-    EmuFreeConfig,
-    EmuTNConfig,
-)
+from pasqal_cloud.device.configuration import BaseConfig, EmuFreeConfig, EmuTNConfig
 from pasqal_cloud.job import Job
 
 RESULT_POLLING_INTERVAL = 2  # seconds
 
 
 class Batch(BaseModel):
     """Class to load batch data return by the API.
@@ -27,15 +23,16 @@
         - created_at: Timestamp of the creation of the batch.
         - updated_at: Timestamp of the last update of the batch.
         - device_type: Type of device to run the batch on.
         - project_id: ID of the owner project of the batch.
         - id: Unique identifier for the batch.
         - user_id: Unique identifier of the user that created the batch.
         - priority: Level of priority of the batch.
-        - status: Status of the batch. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
+        - status: Status of the batch. Possible values are: \
+            PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - webhook: Webhook where the job results are automatically sent to.
         - _client: A Client instance to connect to PCS.
         - sequence_builder: Pulser sequence of the batch.
         - start_datetime: Timestamp of the time the batch was sent to the QPU.
         - end_datetime: Timestamp of when the batch process was finished.
         - device_status: Status of the device where the batch is running.
         - jobs: Dictionary of all the jobs added to the batch.
@@ -119,27 +116,31 @@
         if wait:
             while job.status in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 job_rsp = self._client._get_job(job.id)
                 job = Job(**job_rsp)
         return job
 
-    def declare_complete(self, wait: bool = False) -> Dict[str, Any]:
+    def declare_complete(
+        self, wait: bool = False, fetch_results: bool = False
+    ) -> Dict[str, Any]:
         """Declare to PCS that the batch is complete.
 
         Args:
-            wait: Whether to wait for the batch to be done.
+            wait: Whether to wait for the batch to be done and fetch results.
+            fetch_results (Deprecated): Whether to wait for the batch \
+                to be done and fetch results.
 
         A batch that is complete awaits no extra jobs. All jobs previously added
         will be executed before the batch is terminated. When all its jobs are done,
         the complete batch is unassigned to its running device.
         """
         batch_rsp = self._client._complete_batch(self.id)
         self.complete = True
-        if wait:
+        if wait or fetch_results:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 batch_rsp = self._client._get_batch(
                     self.id,
                 )
             for job_rsp in batch_rsp["jobs"]:
                 self.jobs[job_rsp["id"]] = Job(**job_rsp)
```

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/client.py` & `pasqal-cloud-0.3.3/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.3/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.3/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/job.py` & `pasqal-cloud-0.3.3/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.3/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.3/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.2
+Version: 0.3.3
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.3.2/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.3/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/sdk/setup.py` & `pasqal-cloud-0.3.3/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/setup.py` & `pasqal-cloud-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/conftest.py` & `pasqal-cloud-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_batch.py` & `pasqal-cloud-0.3.3/tests/test_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
-from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
-from pasqal_cloud import SDK, Batch, Job
+from pasqal_cloud import Batch, Job, SDK
 from pasqal_cloud.device import BaseConfig, EmuFreeConfig, EmulatorType, EmuTNConfig
+from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
 
 class TestBatch:
     @pytest.fixture(autouse=True)
     @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
@@ -37,18 +37,22 @@
         assert batch.id == self.batch_id
         assert batch.sequence_builder == self.pulser_sequence
         # TODO: Remove after IROISE MVP
         assert batch.complete
         assert batch.jobs[self.job_id].batch_id == batch.id
         assert batch.jobs[self.job_id].runs == self.n_job_runs
 
-    def test_create_batch_and_wait(self, request_mock):
+    @pytest.mark.parametrize("wait,fetch_results", [(True, False), (False, True)])
+    def test_create_batch_and_wait(self, request_mock, wait, fetch_results):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
         batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence, jobs=[job], wait=True
+            serialized_sequence=self.pulser_sequence,
+            jobs=[job],
+            wait=wait,
+            fetch_results=fetch_results,
         )
         assert (
             batch.id == "00000000-0000-0000-0000-000000000001"
         )  # the batch_id used in the mock data
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
         assert batch.jobs
```

### Comparing `pasqal-cloud-0.3.2/tests/test_client.py` & `pasqal-cloud-0.3.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.3.3/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_config.py` & `pasqal-cloud-0.3.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_device_specs.py` & `pasqal-cloud-0.3.3/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.3/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_job.py` & `pasqal-cloud-0.3.3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.2/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.3/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

