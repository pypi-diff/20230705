# Comparing `tmp/django-rest-framework-client-0.7.0.tar.gz` & `tmp/django-rest-framework-client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-framework-client-0.7.0.tar", last modified: Tue May  9 04:02:04 2023, max compression
+gzip compressed data, was "django-rest-framework-client-0.8.0.tar", last modified: Wed Jul  5 00:20:30 2023, max compression
```

## Comparing `django-rest-framework-client-0.7.0.tar` & `django-rest-framework-client-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.726999 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 04:02:04.000000 django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.726999 django-rest-framework-client-0.7.0/drf_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/drf_client/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/drf_client/helpers/base_main.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 04:02:04.730999 django-rest-framework-client-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-09 04:01:49.000000 django-rest-framework-client-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 00:20:30.000000 django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/drf_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/drf_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/drf_client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/drf_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/drf_client/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/drf_client/helpers/base_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 00:20:30.611168 django-rest-framework-client-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-05 00:20:16.000000 django-rest-framework-client-0.8.0/setup.py
```

### Comparing `django-rest-framework-client-0.7.0/CHANGELOG.md` & `django-rest-framework-client-0.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+### v0.8.0 (2023-07-04)
+
+  * Remove support for Python 3.8.
+  * Add set of `raw_*` methods that do not process results.
+
 ### v0.7.0 (2023-05-08)
 
   * Migrated to Python 3.10, Python 2 is not supported anymore
   * Resource class methods respect additional `**kwargs` and `extra_headers` parameters and pass them on to the underlying `requests` methods
   * Fix to support `http://` schema in the server url
 
 ### v0.6.0 (2022-10-30)
```

### Comparing `django-rest-framework-client-0.7.0/LICENSE` & `django-rest-framework-client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-framework-client-0.7.0/PKG-INFO` & `django-rest-framework-client-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: django-rest-framework-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for a DjangoRestFramework based web site
 Home-page: https://github.com/dkarchmer/django-rest-framework-client
 Author: David Karchmer
 Author-email: dkarchmer@gmail.com
 License: MIT
 Keywords: django,djangorestframework,drf,rest-client
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Rest Framework Python API Package
 
-[![Build Status](https://travis-ci.org/dkarchmer/django-rest-framework-client.svg?branch=master)](https://travis-ci.org/dkarchmer/django-rest-framework-client)
 [![PyPI version](https://img.shields.io/pypi/v/django-rest-framework-client.svg)](https://pypi.python.org/pypi/django-rest-framework-client)
 
 A python library for interacting with any Django web server base on django-rest-framework
 
 Package is based on https://github.com/samgiles/slumber, but enhanced to support tokens and other features.
 
 ## Features
@@ -41,15 +39,15 @@
 
 * Support for custom methods (e.g. ``/ap1/v1/object/custom/`)
 
 ## Requirements
 
 restframeworkclient requires the following modules.
 
-    * Python 3.7+
+    * Python 3.9+
     * requests
 
 ## Installation
 
 ```bash
 python3 -m venv ~/.virtualenv/drf_client
 source ~/.virtualenv/drf_client/bin/activate
```

### Comparing `django-rest-framework-client-0.7.0/README.md` & `django-rest-framework-client-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Django Rest Framework Python API Package
 
-[![Build Status](https://travis-ci.org/dkarchmer/django-rest-framework-client.svg?branch=master)](https://travis-ci.org/dkarchmer/django-rest-framework-client)
 [![PyPI version](https://img.shields.io/pypi/v/django-rest-framework-client.svg)](https://pypi.python.org/pypi/django-rest-framework-client)
 
 A python library for interacting with any Django web server base on django-rest-framework
 
 Package is based on https://github.com/samgiles/slumber, but enhanced to support tokens and other features.
 
 ## Features
@@ -17,15 +16,15 @@
 
 * Support for custom methods (e.g. ``/ap1/v1/object/custom/`)
 
 ## Requirements
 
 restframeworkclient requires the following modules.
 
-    * Python 3.7+
+    * Python 3.9+
     * requests
 
 ## Installation
 
 ```bash
 python3 -m venv ~/.virtualenv/drf_client
 source ~/.virtualenv/drf_client/bin/activate
```

### Comparing `django-rest-framework-client-0.7.0/django_rest_framework_client.egg-info/PKG-INFO` & `django-rest-framework-client-0.8.0/django_rest_framework_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: django-rest-framework-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for a DjangoRestFramework based web site
 Home-page: https://github.com/dkarchmer/django-rest-framework-client
 Author: David Karchmer
 Author-email: dkarchmer@gmail.com
 License: MIT
 Keywords: django,djangorestframework,drf,rest-client
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Rest Framework Python API Package
 
-[![Build Status](https://travis-ci.org/dkarchmer/django-rest-framework-client.svg?branch=master)](https://travis-ci.org/dkarchmer/django-rest-framework-client)
 [![PyPI version](https://img.shields.io/pypi/v/django-rest-framework-client.svg)](https://pypi.python.org/pypi/django-rest-framework-client)
 
 A python library for interacting with any Django web server base on django-rest-framework
 
 Package is based on https://github.com/samgiles/slumber, but enhanced to support tokens and other features.
 
 ## Features
@@ -41,15 +39,15 @@
 
 * Support for custom methods (e.g. ``/ap1/v1/object/custom/`)
 
 ## Requirements
 
 restframeworkclient requires the following modules.
 
-    * Python 3.7+
+    * Python 3.9+
     * requests
 
 ## Installation
 
 ```bash
 python3 -m venv ~/.virtualenv/drf_client
 source ~/.virtualenv/drf_client/bin/activate
```

### Comparing `django-rest-framework-client-0.7.0/drf_client/connection.py` & `django-rest-framework-client-0.8.0/drf_client/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -170,49 +170,74 @@
             if not "token" in self._store:
                 raise RestBaseException('No Token')
             authorization_str = self._options['TOKEN_FORMAT'].format(token=self._store["token"])
             headers['Authorization'] = authorization_str
 
         return headers
 
-    def get(self, extra_headers: dict = None, **kwargs):
+    def raw_get(self, extra_headers: dict = None, **kwargs):
+        """Call get and return raw request respond."""
         args = None
         if 'extra' in kwargs:
             args = kwargs['extra']
         headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.get(self.url(args), headers=headers)
+        return requests.get(self.url(args), headers=headers)
+
+    def get(self, extra_headers: dict = None, **kwargs):
+        """Call get and process respond."""
+        resp = self.raw_get(extra_headers, **kwargs)
         return self._process_response(resp)
 
-    def post(self, data: dict = None, extra_headers: dict = None, **kwargs):
+    def raw_post(self, data: dict = None, extra_headers: dict = None, **kwargs):
+        """Call requests post and return raw respond."""
         payload = json.dumps(data) if data and "files" not in kwargs else data
         headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.post(self.url(), data=payload, headers=headers, **kwargs)
+        return requests.post(self.url(), data=payload, headers=headers, **kwargs)
+
+    def post(self, data: dict = None, extra_headers: dict = None, **kwargs):
+        """Call post and process respond."""
+        resp = self.raw_post(data, extra_headers, **kwargs)
         return self._process_response(resp)
 
-    def patch(self, data=None, extra_headers: dict = None, **kwargs):
+    def raw_patch(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call patch and return raw request respond."""
         payload = json.dumps(data) if data and "files" not in kwargs else data
         headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.patch(self.url(), data=payload, headers=headers, **kwargs)
+        return requests.patch(self.url(), data=payload, headers=headers, **kwargs)
+
+    def patch(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call patch and process respond."""
+        resp = self.raw_patch(data, extra_headers, **kwargs)
         return self._process_response(resp)
 
-    def put(self, data=None, extra_headers: dict = None, **kwargs):
+    def raw_put(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call Put and return raw request respond."""
         payload = json.dumps(data) if data and "files" not in kwargs else data
         headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.put(self.url(), data=payload, headers=headers, **kwargs)
+        return requests.put(self.url(), data=payload, headers=headers, **kwargs)
+
+    def put(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call Put and process respond."""
+        resp = self.raw_put(data, extra_headers, **kwargs)
         return self._process_response(resp)
 
-    def delete(self, data=None, extra_headers: dict = None, **kwargs):
+    def raw_delete(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call Delete and return raw request respond."""
         payload = json.dumps(data) if data and "files" not in kwargs else data
         headers = self._get_headers() | extra_headers if extra_headers else self._get_headers()
 
-        resp = requests.delete(self.url(), data=payload, headers=headers, **kwargs)
+        return requests.delete(self.url(), data=payload, headers=headers, **kwargs)
+
+    def delete(self, data=None, extra_headers: dict = None, **kwargs):
+        """Call Delete and process respond. Return True if ok"""
+        resp = self.raw_delete(data, extra_headers, **kwargs)
         if 200 <= resp.status_code <= 299:
             if resp.status_code == 204:
                 return True
             else:
                 return True  # @@@ Should this really be True?
         else:
             return False
```

### Comparing `django-rest-framework-client-0.7.0/drf_client/exceptions.py` & `django-rest-framework-client-0.8.0/drf_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-client-0.7.0/drf_client/helpers/base_main.py` & `django-rest-framework-client-0.8.0/drf_client/helpers/base_main.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-client-0.7.0/setup.py` & `django-rest-framework-client-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='django-rest-framework-client',
-    version='0.7.0',
+    version='0.8.0',
     description='Python client for a DjangoRestFramework based web site',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/dkarchmer/django-rest-framework-client',
     author='David Karchmer',
     author_email="dkarchmer@gmail.com",
     license='MIT',
@@ -24,15 +24,14 @@
         'requests',
     ],
     python_requires=">=3.10,<4",
     keywords=["django", "djangorestframework", "drf", "rest-client",],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

