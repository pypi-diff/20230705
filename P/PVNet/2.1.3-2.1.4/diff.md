# Comparing `tmp/PVNet-2.1.3.tar.gz` & `tmp/PVNet-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-2.1.3.tar", last modified: Tue Jun 27 14:07:03 2023, max compression
+gzip compressed data, was "PVNet-2.1.4.tar", last modified: Wed Jul  5 10:12:07 2023, max compression
```

## Comparing `PVNet-2.1.3.tar` & `PVNet-2.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:07:03.929233 PVNet-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-27 14:06:54.000000 PVNet-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 14:06:54.000000 PVNet-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 14:07:03.929233 PVNet-2.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:07:03.925233 PVNet-2.1.3/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 14:07:03.000000 PVNet-2.1.3/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 14:07:03.000000 PVNet-2.1.3/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:07:03.000000 PVNet-2.1.3/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-27 14:07:03.000000 PVNet-2.1.3/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 14:07:03.000000 PVNet-2.1.3/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-27 14:06:54.000000 PVNet-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:07:03.929233 PVNet-2.1.3/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-27 14:06:54.000000 PVNet-2.1.3/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-27 14:06:54.000000 PVNet-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 14:06:54.000000 PVNet-2.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-27 14:06:54.000000 PVNet-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:07:03.929233 PVNet-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-27 14:06:54.000000 PVNet-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:07:03.929233 PVNet-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:06:54.000000 PVNet-2.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-27 14:06:54.000000 PVNet-2.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 14:06:54.000000 PVNet-2.1.3/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:07.039581 PVNet-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 10:11:57.000000 PVNet-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 10:11:57.000000 PVNet-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 10:12:07.039581 PVNet-2.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:07.035581 PVNet-2.1.4/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 10:12:07.000000 PVNet-2.1.4/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-05 10:12:07.000000 PVNet-2.1.4/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:12:07.000000 PVNet-2.1.4/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 10:12:07.000000 PVNet-2.1.4/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:12:07.000000 PVNet-2.1.4/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-05 10:11:57.000000 PVNet-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:07.035581 PVNet-2.1.4/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-05 10:11:57.000000 PVNet-2.1.4/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-05 10:11:57.000000 PVNet-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 10:11:57.000000 PVNet-2.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 10:11:57.000000 PVNet-2.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:12:07.039581 PVNet-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-05 10:11:57.000000 PVNet-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:07.039581 PVNet-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:11:57.000000 PVNet-2.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-05 10:11:57.000000 PVNet-2.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-05 10:11:57.000000 PVNet-2.1.4/tests/test_app.py
```

### Comparing `PVNet-2.1.3/LICENSE` & `PVNet-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/PKG-INFO` & `PVNet-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.3
+Version: 2.1.4
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.3/PVNet.egg-info/PKG-INFO` & `PVNet-2.1.4/PVNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.3
+Version: 2.1.4
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.3/README.md` & `PVNet-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/pvnet/app.py` & `PVNet-2.1.4/pvnet/app.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/pvnet/callbacks.py` & `PVNet-2.1.4/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/pvnet/optimizers.py` & `PVNet-2.1.4/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/pvnet/training.py` & `PVNet-2.1.4/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/pvnet/utils.py` & `PVNet-2.1.4/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/setup.py` & `PVNet-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/tests/conftest.py` & `PVNet-2.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.3/tests/test_app.py` & `PVNet-2.1.4/tests/test_app.py`

 * *Files identical despite different names*

