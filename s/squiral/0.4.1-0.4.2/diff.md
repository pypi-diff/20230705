# Comparing `tmp/squiral-0.4.1.tar.gz` & `tmp/squiral-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squiral-0.4.1.tar", max compression
+gzip compressed data, was "squiral-0.4.2.tar", max compression
```

## Comparing `squiral-0.4.1.tar` & `squiral-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-04-21 17:22:00.053933 squiral-0.4.1/LICENSE
--rw-r--r--   0        0        0     3056 2023-04-21 17:22:00.053933 squiral-0.4.1/README.md
--rw-r--r--   0        0        0      531 2023-04-21 17:22:00.053933 squiral-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      184 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/__init__.py
--rw-r--r--   0        0        0      151 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/__main__.py
--rw-r--r--   0        0        0      744 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/main.py
--rw-r--r--   0        0        0     2464 2023-04-21 17:22:00.053933 squiral-0.4.1/squiral/squiral.py
--rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 squiral-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-04 22:47:30.784159 squiral-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3056 2023-07-04 22:47:30.784159 squiral-0.4.2/README.md
+-rw-r--r--   0        0        0      531 2023-07-04 22:47:30.784159 squiral-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-07-04 22:47:30.784159 squiral-0.4.2/squiral/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-04 22:47:30.788159 squiral-0.4.2/squiral/__main__.py
+-rw-r--r--   0        0        0      744 2023-07-04 22:47:30.788159 squiral-0.4.2/squiral/main.py
+-rw-r--r--   0        0        0     2464 2023-07-04 22:47:30.788159 squiral-0.4.2/squiral/squiral.py
+-rw-r--r--   0        0        0     3677 1970-01-01 00:00:00.000000 squiral-0.4.2/PKG-INFO
```

### Comparing `squiral-0.4.1/LICENSE` & `squiral-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squiral-0.4.1/README.md` & `squiral-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `squiral-0.4.1/pyproject.toml` & `squiral-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squiral"
-version = "0.4.1"
+version = "0.4.2"
 description = "squiral - square spiral"
 authors = ["SADIK KUZU <sadikkuzu@hotmail.com>"]
 homepage = "https://github.com/sadikkuzu/squiral"
 readme = "README.md"
 license = "MIT"
 packages = [{include = "squiral"}]
```

### Comparing `squiral-0.4.1/squiral/main.py` & `squiral-0.4.2/squiral/main.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.1/squiral/squiral.py` & `squiral-0.4.2/squiral/squiral.py`

 * *Files identical despite different names*

### Comparing `squiral-0.4.1/PKG-INFO` & `squiral-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squiral
-Version: 0.4.1
+Version: 0.4.2
 Summary: squiral - square spiral
 Home-page: https://github.com/sadikkuzu/squiral
 License: MIT
 Author: SADIK KUZU
 Author-email: sadikkuzu@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

