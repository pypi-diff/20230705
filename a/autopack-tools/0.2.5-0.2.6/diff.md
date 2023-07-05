# Comparing `tmp/autopack_tools-0.2.5.tar.gz` & `tmp/autopack_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.2.5.tar", max compression
+gzip compressed data, was "autopack_tools-0.2.6.tar", max compression
```

## Comparing `autopack_tools-0.2.5.tar` & `autopack_tools-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.5/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.5/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.5/autopack/VERSION
--rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.5/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.5/autopack/__main__.py
--rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.5/autopack/api.py
--rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.5/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.5/autopack/errors.py
--rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.5/autopack/get_pack.py
--rw-r--r--   0        0        0     3877 2023-07-04 01:58:56.151275 autopack_tools-0.2.5/autopack/installation.py
--rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.5/autopack/pack.py
--rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.5/autopack/pack_response.py
--rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.5/autopack/search.py
--rw-r--r--   0        0        0     2094 2023-07-04 01:58:55.758062 autopack_tools-0.2.5/autopack/selection.py
--rw-r--r--   0        0        0     4405 2023-07-04 01:58:56.161504 autopack_tools-0.2.5/autopack/utils.py
--rw-r--r--   0        0        0      911 2023-07-04 03:58:16.276805 autopack_tools-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2862 2023-07-02 21:31:24.435654 autopack_tools-0.2.6/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.2.6/autopack/VERSION
+-rw-r--r--   0        0        0        0 2023-06-30 20:06:04.842978 autopack_tools-0.2.6/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.2.6/autopack/__main__.py
+-rw-r--r--   0        0        0     2870 2023-07-04 00:01:05.734894 autopack_tools-0.2.6/autopack/api.py
+-rw-r--r--   0        0        0     1116 2023-07-03 23:59:48.436637 autopack_tools-0.2.6/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-06-29 18:48:28.424876 autopack_tools-0.2.6/autopack/errors.py
+-rw-r--r--   0        0        0     2698 2023-07-03 23:58:29.022022 autopack_tools-0.2.6/autopack/get_pack.py
+-rw-r--r--   0        0        0     3877 2023-07-05 01:53:52.116169 autopack_tools-0.2.6/autopack/installation.py
+-rw-r--r--   0        0        0     2921 2023-07-03 23:58:49.932953 autopack_tools-0.2.6/autopack/pack.py
+-rw-r--r--   0        0        0      676 2023-07-04 00:56:08.699966 autopack_tools-0.2.6/autopack/pack_response.py
+-rw-r--r--   0        0        0      455 2023-06-29 21:34:17.271996 autopack_tools-0.2.6/autopack/search.py
+-rw-r--r--   0        0        0     4016 2023-07-05 01:53:01.972972 autopack_tools-0.2.6/autopack/selection.py
+-rw-r--r--   0        0        0     4405 2023-07-05 01:53:52.129111 autopack_tools-0.2.6/autopack/utils.py
+-rw-r--r--   0        0        0      911 2023-07-05 02:01:03.148675 autopack_tools-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 autopack_tools-0.2.6/PKG-INFO
```

### Comparing `autopack_tools-0.2.5/LICENSE` & `autopack_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/README.md` & `autopack_tools-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/api.py` & `autopack_tools-0.2.6/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/cli.py` & `autopack_tools-0.2.6/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/get_pack.py` & `autopack_tools-0.2.6/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/installation.py` & `autopack_tools-0.2.6/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/pack.py` & `autopack_tools-0.2.6/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/pack_response.py` & `autopack_tools-0.2.6/autopack/pack_response.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/autopack/utils.py` & `autopack_tools-0.2.6/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.2.5/PKG-INFO` & `autopack_tools-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.2.5
+Version: 0.2.6
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

