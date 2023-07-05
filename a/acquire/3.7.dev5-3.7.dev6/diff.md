# Comparing `tmp/acquire-3.7.dev5.tar.gz` & `tmp/acquire-3.7.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.7.dev5.tar", last modified: Tue Jun 27 07:48:27 2023, max compression
+gzip compressed data, was "acquire-3.7.dev6.tar", last modified: Wed Jul  5 13:27:49 2023, max compression
```

## Comparing `acquire-3.7.dev5.tar` & `acquire-3.7.dev6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.780567 acquire-3.7.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 07:48:11.000000 acquire-3.7.dev5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:11.000000 acquire-3.7.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:11.000000 acquire-3.7.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-27 07:48:27.780567 acquire-3.7.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-27 07:48:11.000000 acquire-3.7.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76017 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.780567 acquire-3.7.dev5/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-27 07:48:11.000000 acquire-3.7.dev5/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.776567 acquire-3.7.dev5/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:48:27.000000 acquire-3.7.dev5/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 07:48:17.000000 acquire-3.7.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:48:27.780567 acquire-3.7.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.780567 acquire-3.7.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:27.780567 acquire-3.7.dev5/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-27 07:48:11.000000 acquire-3.7.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.896515 acquire-3.7.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 13:27:33.000000 acquire-3.7.dev6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-05 13:27:33.000000 acquire-3.7.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 13:27:33.000000 acquire-3.7.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-05 13:27:49.896515 acquire-3.7.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-05 13:27:33.000000 acquire-3.7.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.888515 acquire-3.7.dev6/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76218 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.888515 acquire-3.7.dev6/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.888515 acquire-3.7.dev6/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.892515 acquire-3.7.dev6/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.892515 acquire-3.7.dev6/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.892515 acquire-3.7.dev6/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-05 13:27:33.000000 acquire-3.7.dev6/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.888515 acquire-3.7.dev6/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 13:27:49.000000 acquire-3.7.dev6/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 13:27:38.000000 acquire-3.7.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 13:27:49.896515 acquire-3.7.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.892515 acquire-3.7.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:27:49.892515 acquire-3.7.dev6/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-05 13:27:33.000000 acquire-3.7.dev6/tox.ini
```

### Comparing `acquire-3.7.dev5/LICENSE` & `acquire-3.7.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/PKG-INFO` & `acquire-3.7.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev5
+Version: 3.7.dev6
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev5/README.md` & `acquire-3.7.dev6/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/acquire.py` & `acquire-3.7.dev6/acquire/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,14 +556,16 @@
 
 @register_module("-t", "--tasks")
 class Tasks(Module):
     SPEC = [
         ("dir", "sysvol/windows/tasks"),
         ("dir", "sysvol/windows/system32/tasks"),
         ("dir", "sysvol/windows/syswow64/tasks"),
+        ("dir", "sysvol/windows/sysvol/domain/policies"),
+        ("dir", "sysvol/windows/system32/GroupPolicy/DataStore/"),
     ]
 
 
 @register_module("-nt", "--ntds")
 class NTDS(Module):
     SPEC = [
         ("dir", "sysvol/windows/NTDS"),
@@ -904,14 +906,16 @@
         ("dir", "AppData/Local/Symantec/Symantec Endpoint Protection/Logs", from_user_home),
         ("dir", "sysvol/Windows/System32/winevt/logs/Symantec Endpoint Protection Client.evtx"),
         ("glob", "sysvol/ProgramData/Symantec/Symantec Endpoint Protection/*/Data/CmnClnt/ccSubSDK"),
         ("glob", "sysvol/ProgramData/Symantec/Symantec Endpoint Protection/*/Data/registrationInfo.xml"),
         # TotalAV
         ("glob", "sysvol/Program Files*/TotalAV/logs"),
         ("dir", "sysvol/ProgramData/TotalAV/logs"),
+        # Trendmicro
+        ("glob", "sysvol/Program Files*/Trend Micro"),
         # VIPRE
         ("dir", "sysvol/ProgramData/VIPRE Business Agent/Logs"),
         ("dir", "AppData/Roaming/VIPRE Business", from_user_home),
         ("dir", "AppData/Roaming/GFI Software/AntiMalware/Logs", from_user_home),
         ("dir", "AppData/Roaming/Sunbelt Software/AntiMalware/Logs", from_user_home),
         # Webroot
         ("file", "sysvol/ProgramData/WRData/WRLog.log"),
```

### Comparing `acquire-3.7.dev5/acquire/collector.py` & `acquire-3.7.dev6/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/crypt.py` & `acquire-3.7.dev6/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/dynamic/windows/collect.py` & `acquire-3.7.dev6/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/dynamic/windows/handles.py` & `acquire-3.7.dev6/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/dynamic/windows/named_objects.py` & `acquire-3.7.dev6/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/dynamic/windows/ntdll.py` & `acquire-3.7.dev6/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/dynamic/windows/types.py` & `acquire-3.7.dev6/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/esxi.py` & `acquire-3.7.dev6/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/hashes.py` & `acquire-3.7.dev6/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/log.py` & `acquire-3.7.dev6/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/outputs/base.py` & `acquire-3.7.dev6/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/outputs/dir.py` & `acquire-3.7.dev6/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/outputs/tar.py` & `acquire-3.7.dev6/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/tools/decrypter.py` & `acquire-3.7.dev6/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/uploaders/minio.py` & `acquire-3.7.dev6/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/uploaders/plugin.py` & `acquire-3.7.dev6/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/uploaders/plugin_registry.py` & `acquire-3.7.dev6/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire/utils.py` & `acquire-3.7.dev6/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/acquire.egg-info/PKG-INFO` & `acquire-3.7.dev6/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev5
+Version: 3.7.dev6
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev5/acquire.egg-info/SOURCES.txt` & `acquire-3.7.dev6/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/pyproject.toml` & `acquire-3.7.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/conftest.py` & `acquire-3.7.dev6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/docs/Makefile` & `acquire-3.7.dev6/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/docs/conf.py` & `acquire-3.7.dev6/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_acquire_command.py` & `acquire-3.7.dev6/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_collector.py` & `acquire-3.7.dev6/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_decryptor_funcs.py` & `acquire-3.7.dev6/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_esxi_memory.py` & `acquire-3.7.dev6/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_file_sorting.py` & `acquire-3.7.dev6/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_minio_uploader.py` & `acquire-3.7.dev6/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_plugin.py` & `acquire-3.7.dev6/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tests/test_utils.py` & `acquire-3.7.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev5/tox.ini` & `acquire-3.7.dev6/tox.ini`

 * *Files identical despite different names*

