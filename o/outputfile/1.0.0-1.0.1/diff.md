# Comparing `tmp/outputfile-1.0.0.tar.gz` & `tmp/outputfile-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outputfile-1.0.0.tar", max compression
+gzip compressed data, was "outputfile-1.0.1.tar", max compression
```

## Comparing `outputfile-1.0.0.tar` & `outputfile-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-23 21:54:21.075670 outputfile-1.0.0/LICENSE
--rw-r--r--   0        0        0     1243 2023-06-23 21:54:21.075670 outputfile-1.0.0/README.md
--rw-r--r--   0        0        0    10498 2023-06-23 21:54:51.568201 outputfile-1.0.0/outputfile/__init__.py
--rw-r--r--   0        0        0     2124 2023-06-23 21:59:03.552588 outputfile-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 outputfile-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 06:57:34.116558 outputfile-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1243 2023-07-03 06:57:34.116558 outputfile-1.0.1/README.md
+-rw-r--r--   0        0        0    10498 2023-07-03 06:57:34.120558 outputfile-1.0.1/outputfile/__init__.py
+-rw-r--r--   0        0        0     2124 2023-07-03 06:57:34.120558 outputfile-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 outputfile-1.0.1/PKG-INFO
```

### Comparing `outputfile-1.0.0/LICENSE` & `outputfile-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `outputfile-1.0.0/README.md` & `outputfile-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `outputfile-1.0.0/outputfile/__init__.py` & `outputfile-1.0.1/outputfile/__init__.py`

 * *Files identical despite different names*

### Comparing `outputfile-1.0.0/pyproject.toml` & `outputfile-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "outputfile"
-version = "1.0.0"
+version = "1.0.1"
 description = "Timestamp Preserving Output File Writer"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `outputfile-1.0.0/PKG-INFO` & `outputfile-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outputfile
-Version: 1.0.0
+Version: 1.0.1
 Summary: Timestamp Preserving Output File Writer
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

