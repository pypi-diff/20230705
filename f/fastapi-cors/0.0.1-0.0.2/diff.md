# Comparing `tmp/fastapi-cors-0.0.1.tar.gz` & `tmp/fastapi-cors-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cors-0.0.1.tar", last modified: Tue Jul  4 22:27:36 2023, max compression
+gzip compressed data, was "fastapi-cors-0.0.2.tar", last modified: Tue Jul  4 22:53:51 2023, max compression
```

## Comparing `fastapi-cors-0.0.1.tar` & `fastapi-cors-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-07-04 22:27:10.130219 fastapi-cors-0.0.1/LICENSE
--rw-r--r--   0        0        0      121 2023-07-04 22:27:10.130219 fastapi-cors-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-04 22:27:10.130219 fastapi-cors-0.0.1/fastapi_cors/__init__.py
--rw-r--r--   0        0        0      813 2023-07-04 22:27:10.130219 fastapi-cors-0.0.1/fastapi_cors/env.py
--rw-r--r--   0        0        0     2056 2023-07-04 22:27:10.130219 fastapi-cors-0.0.1/fastapi_cors/main.py
--rw-r--r--   0        0        0     2249 2023-07-04 22:27:10.134219 fastapi-cors-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 fastapi-cors-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-04 22:53:22.212280 fastapi-cors-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2367 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/env.py
+-rw-r--r--   0        0        0     2056 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/main.py
+-rw-r--r--   0        0        0     2249 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 fastapi-cors-0.0.2/PKG-INFO
```

### Comparing `fastapi-cors-0.0.1/LICENSE` & `fastapi-cors-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.1/fastapi_cors/env.py` & `fastapi-cors-0.0.2/fastapi_cors/env.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.1/fastapi_cors/main.py` & `fastapi-cors-0.0.2/fastapi_cors/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.1/pyproject.toml` & `fastapi-cors-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 classifiers = [
     "Topic :: Software Development :: Code Generators",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/iancleary/fastapi-cors"
 Repository = "https://github.com/iancleary/fastapi-cors"
```

