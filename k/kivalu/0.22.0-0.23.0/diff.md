# Comparing `tmp/kivalu-0.22.0.tar.gz` & `tmp/kivalu-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivalu-0.22.0.tar", last modified: Sat Jun 24 13:55:15 2023, max compression
+gzip compressed data, was "kivalu-0.23.0.tar", last modified: Wed Jul  5 04:40:27 2023, max compression
```

## Comparing `kivalu-0.22.0.tar` & `kivalu-0.23.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-07 10:57:06.000000 kivalu-0.22.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-06-24 13:55:15.850455 kivalu-0.22.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/kivalu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13483 2023-06-24 11:24:20.000000 kivalu-0.22.0/kivalu/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/kivalu.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-06-24 13:55:15.000000 kivalu-0.22.0/kivalu.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/scripts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-07 10:57:06.000000 kivalu-0.22.0/scripts/kivalu-setup
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-24 13:55:15.850455 kivalu-0.22.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-06-24 11:39:05.000000 kivalu-0.22.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-24 13:55:15.850455 kivalu-0.22.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2023-05-12 16:53:14.000000 kivalu-0.22.0/tests/test_argumentparser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9095 2023-06-24 11:24:21.000000 kivalu-0.22.0/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1017 2023-05-12 16:53:14.000000 kivalu-0.22.0/tests/test_main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-05-07 10:57:06.000000 kivalu-0.22.0/tests/test_server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:40:27.761867 kivalu-0.23.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1061 2023-05-07 10:57:06.000000 kivalu-0.23.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-07-05 04:40:27.761867 kivalu-0.23.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:40:27.761867 kivalu-0.23.0/kivalu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13989 2023-07-05 04:32:22.000000 kivalu-0.23.0/kivalu/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:40:27.761867 kivalu-0.23.0/kivalu.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-07-05 04:40:27.000000 kivalu-0.23.0/kivalu.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-05 04:40:27.000000 kivalu-0.23.0/kivalu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-05 04:40:27.000000 kivalu-0.23.0/kivalu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-07-05 04:40:27.000000 kivalu-0.23.0/kivalu.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-05 04:40:27.000000 kivalu-0.23.0/kivalu.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:40:27.761867 kivalu-0.23.0/scripts/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       52 2023-05-07 10:57:06.000000 kivalu-0.23.0/scripts/kivalu-setup
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-05 04:40:27.761867 kivalu-0.23.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-07-05 04:39:21.000000 kivalu-0.23.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-05 04:40:27.761867 kivalu-0.23.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1100 2023-05-12 16:53:14.000000 kivalu-0.23.0/tests/test_argumentparser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2023-07-05 04:32:21.000000 kivalu-0.23.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1017 2023-05-12 16:53:14.000000 kivalu-0.23.0/tests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2203 2023-05-07 10:57:06.000000 kivalu-0.23.0/tests/test_server.py
```

### Comparing `kivalu-0.22.0/LICENSE` & `kivalu-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kivalu-0.22.0/PKG-INFO` & `kivalu-0.23.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.22.0
+Version: 0.23.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.22.0/kivalu/__init__.py` & `kivalu-0.23.0/kivalu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import argparse
+import datetime
 import http.server
 import json
 import threading
 from pathlib import Path
 from typing import List, Optional, Any
 
 import jinja2
@@ -108,14 +109,15 @@
         self.jinja_environment.globals[URL] = self.url
         self.jinja_environment.globals[FAILOVER] = self.failover
         self.jinja_environment.globals[LEVELS] = self.levels
         self.jinja_environment.globals.update(self.extra_vars)
         self.jinja_environment.globals["configuration"] = json.dumps({URL: self.url, FAILOVER: self.failover, LEVELS: self.levels, EXTRA_VARS: self.extra_vars, TIMEOUT: self.timeout, CACHE: self.cache})
         self.jinja_environment.filters["get"] = self.get
         self.jinja_environment.filters["read"] = read
+        self.jinja_environment.filters["now"] = now
 
         # http requests setup
         self.http_session = requests_cache.CachedSession(backend="memory", expire_after=cache)
 
     def get(self, key: str, default: str = "", template: bool = True, strip: bool = True, extra_vars: dict = None) -> str:
         """
         Fetches the value of a provided key from the server.
@@ -234,14 +236,26 @@
 
     try:
         return Path(path).read_text(encoding=encoding)
     except IOError:
         return ""
 
 
+def now(pattern: str) -> str:
+    """
+    Filter for the Jinja templating engine, that formats the current datetime with the given pattern.
+    Visit https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes for more information about the format codes.
+
+    :param pattern: formatting pattern
+    :return: the current datetime as a formatted string
+    """
+
+    return datetime.datetime.now().strftime(pattern)
+
+
 def build_argument_parser(*args: Any, **kwargs: Any) -> argparse.ArgumentParser:
     """
     Builds an ArgumentParser that can be used to share a common Client CLI syntax.
 
     :param args: arguments of the ArgumentParser constructor
     :param kwargs: keyword arguments of the ArgumentParser constructor
     :return: the customized ArgumentParser
```

### Comparing `kivalu-0.22.0/kivalu.egg-info/PKG-INFO` & `kivalu-0.23.0/kivalu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivalu
-Version: 0.22.0
+Version: 0.23.0
 Summary: Nested key-value system with built-in inheritance and templating, designed for configuration management
 Home-page: https://zebr0.io/projects/kivalu
 Download-URL: https://gitlab.com/zebr0/kivalu
 Author: Thomas JOUANNOT
 Author-email: mazerty@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kivalu-0.22.0/setup.py` & `kivalu-0.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="kivalu",
-    version="0.22.0",
+    version="0.23.0",
     description="Nested key-value system with built-in inheritance and templating, designed for configuration management",
     long_description="TODO",
     long_description_content_type="text/markdown",
     author="Thomas JOUANNOT",
     author_email="mazerty@gmail.com",
     url="https://zebr0.io/projects/kivalu",
     download_url="https://gitlab.com/zebr0/kivalu",
```

### Comparing `kivalu-0.22.0/tests/test_argumentparser.py` & `kivalu-0.23.0/tests/test_argumentparser.py`

 * *Files identical despite different names*

### Comparing `kivalu-0.22.0/tests/test_client.py` & `kivalu-0.23.0/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import http.server
 import time
 from pathlib import Path
 
 import jinja2.exceptions
 import pytest
 import requests.exceptions
@@ -142,14 +143,21 @@
 def test_read_ko(tmp_path, server):
     server.data = {"template": "{{ '" + str(tmp_path.joinpath("unknown_file")) + "' | read }}"}
     client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""))
 
     assert client.get("template") == ""
 
 
+def test_now(server):
+    server.data = {"template": '{{ "%Y-%m-%d" | now }}'}
+    client = kivalu.Client(url="http://127.0.0.1:8000", configuration_file=Path(""))
+
+    assert client.get("template") == datetime.datetime.now().strftime("%Y-%m-%d")
+
+
 def test_timeout():
     class TimeoutRequestHandler(http.server.BaseHTTPRequestHandler):
         def do_GET(self):
             time.sleep(0.2)
             self.send_response(404)
             self.end_headers()
```

### Comparing `kivalu-0.22.0/tests/test_main.py` & `kivalu-0.23.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `kivalu-0.22.0/tests/test_server.py` & `kivalu-0.23.0/tests/test_server.py`

 * *Files identical despite different names*

