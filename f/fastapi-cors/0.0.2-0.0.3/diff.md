# Comparing `tmp/fastapi-cors-0.0.2.tar.gz` & `tmp/fastapi-cors-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cors-0.0.2.tar", last modified: Tue Jul  4 22:53:51 2023, max compression
+gzip compressed data, was "fastapi-cors-0.0.3.tar", last modified: Tue Jul  4 22:58:44 2023, max compression
```

## Comparing `fastapi-cors-0.0.2.tar` & `fastapi-cors-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-07-04 22:53:22.212280 fastapi-cors-0.0.2/LICENSE
--rw-r--r--   0        0        0     2367 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/__init__.py
--rw-r--r--   0        0        0      813 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/env.py
--rw-r--r--   0        0        0     2056 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/fastapi_cors/main.py
--rw-r--r--   0        0        0     2249 2023-07-04 22:53:22.216281 fastapi-cors-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 fastapi-cors-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2497 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/fastapi_cors/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/fastapi_cors/env.py
+-rw-r--r--   0        0        0     2056 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/fastapi_cors/main.py
+-rw-r--r--   0        0        0     2249 2023-07-04 22:58:18.763231 fastapi-cors-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 fastapi-cors-0.0.3/PKG-INFO
```

### Comparing `fastapi-cors-0.0.2/LICENSE` & `fastapi-cors-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.2/README.md` & `fastapi-cors-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A simply scoped abstraction to provide CORS settings via environment variables to a Fastapi application.
 
 ## Usage
 
 ```python
 from fastapi import FastAPI
 
-# import (fastapi_cors.env) will read environment variables from .env
+# during this next line `fastapi_cors.env` will read environment variables from .env
 from fastapi_cors import CORS 
 
 app = FastAPI()
 
 CORS(app)
 ```
 
@@ -19,14 +19,18 @@
 
 A health check route is optionally added that displays these (but not other) environment variables.
 
 
 *If you want to disable it, use the code below*
 
 ```python
+
+from fastapi import FastAPI
+
+# during this next line `fastapi_cors.env` will read environment variables from .env
 from fastapi_cors import CORS 
 
 app = FastAPI()
 
 CORS(app, include_health_check=False)
 ```
```

### Comparing `fastapi-cors-0.0.2/fastapi_cors/env.py` & `fastapi-cors-0.0.3/fastapi_cors/env.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.2/fastapi_cors/main.py` & `fastapi-cors-0.0.3/fastapi_cors/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.2/pyproject.toml` & `fastapi-cors-0.0.3/pyproject.toml`

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
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/iancleary/fastapi-cors"
 Repository = "https://github.com/iancleary/fastapi-cors"
```

### Comparing `fastapi-cors-0.0.2/PKG-INFO` & `fastapi-cors-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_cors
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple env support of CORS settings for Fastapi applications
 License: MIT
 Keywords: cors,python,fastapi,environs
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,15 +20,15 @@
 A simply scoped abstraction to provide CORS settings via environment variables to a Fastapi application.
 
 ## Usage
 
 ```python
 from fastapi import FastAPI
 
-# import (fastapi_cors.env) will read environment variables from .env
+# during this next line `fastapi_cors.env` will read environment variables from .env
 from fastapi_cors import CORS 
 
 app = FastAPI()
 
 CORS(app)
 ```
 
@@ -36,14 +36,18 @@
 
 A health check route is optionally added that displays these (but not other) environment variables.
 
 
 *If you want to disable it, use the code below*
 
 ```python
+
+from fastapi import FastAPI
+
+# during this next line `fastapi_cors.env` will read environment variables from .env
 from fastapi_cors import CORS 
 
 app = FastAPI()
 
 CORS(app, include_health_check=False)
 ```
```

