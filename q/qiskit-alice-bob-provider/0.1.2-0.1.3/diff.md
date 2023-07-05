# Comparing `tmp/qiskit_alice_bob_provider-0.1.2.tar.gz` & `tmp/qiskit_alice_bob_provider-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.1.2.tar", last modified: Mon Jun 12 08:06:00 2023, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.1.3.tar", last modified: Wed Jul  5 08:21:02 2023, max compression
```

## Comparing `qiskit_alice_bob_provider-0.1.2.tar` & `qiskit_alice_bob_provider-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/LICENSE
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/README.md
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2108 2023-06-12 08:04:04.000000 qiskit_alice_bob_provider-0.1.2/pyproject.toml
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/__init__.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/__init__.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3681 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/client.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/jobs.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/targets.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5151 2023-06-09 14:28:03.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3186 2023-06-09 14:46:54.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/ensure_preparation_pass.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/errors.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/job.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2563 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-06-09 14:25:47.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/utils.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1124 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      317 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/setup.cfg
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/setup.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/tests/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/tests/test_against_real_server.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5145 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/tests/test_api.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1272 2023-06-09 14:26:04.000000 qiskit_alice_bob_provider-0.1.2/tests/test_ensure_preparation_pass.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/tests/test_translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/LICENSE
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/README.md
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2165 2023-07-05 08:20:43.000000 qiskit_alice_bob_provider-0.1.3/pyproject.toml
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/__init__.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/__init__.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3681 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/client.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/jobs.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/targets.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5151 2023-06-12 08:12:54.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3186 2023-06-12 08:12:54.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/ensure_preparation_pass.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/errors.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/job.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2563 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-06-09 14:25:47.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1124 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      325 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-07-05 08:21:02.000000 qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/setup.cfg
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/setup.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-07-05 08:21:02.252908 qiskit_alice_bob_provider-0.1.3/tests/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/tests/test_against_real_server.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5145 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.3/tests/test_api.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/tests/test_backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1272 2023-06-12 08:12:54.000000 qiskit_alice_bob_provider-0.1.3/tests/test_ensure_preparation_pass.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/tests/test_provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/tests/test_qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.3/tests/test_translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.3/tests/test_utils.py
```

### Comparing `qiskit_alice_bob_provider-0.1.2/LICENSE` & `qiskit_alice_bob_provider-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/PKG-INFO` & `qiskit_alice_bob_provider-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.2/README.md` & `qiskit_alice_bob_provider-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/pyproject.toml` & `qiskit_alice_bob_provider-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.1.2"
+version = "0.1.3"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 urls = {Homepage = "https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider", "Alice & Bob" = "https://alice-bob.com/"}
 requires-python = ">=3.7"
 dependencies = [
     "requests",
-    "qiskit-terra",
+    "qiskit-terra>=0.22.0",  # first version with backend transpiler plugins
     "qiskit-qir-alice-bob-fork",
     "tenacity"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.1.0",
```

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/__init__.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/client.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/jobs.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/targets.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/backend.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/ensure_preparation_pass.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/ensure_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/job.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/provider.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/translation_plugin.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/translation_plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/utils.py` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-alice-bob-provider
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.1.3/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_against_real_server.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_against_real_server.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_api.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_backend.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_ensure_preparation_pass.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_ensure_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.2/tests/test_translation_plugin.py` & `qiskit_alice_bob_provider-0.1.3/tests/test_translation_plugin.py`

 * *Files identical despite different names*

