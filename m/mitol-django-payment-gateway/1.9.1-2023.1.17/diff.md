# Comparing `tmp/mitol-django-payment-gateway-1.9.1.tar.gz` & `tmp/mitol-django-payment-gateway-2023.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-payment-gateway-1.9.1.tar", last modified: Mon Feb 13 13:26:43 2023, max compression
+gzip compressed data, was "mitol-django-payment-gateway-2023.1.17.tar", last modified: Wed Jul  5 16:16:56 2023, max compression
```

## Comparing `mitol-django-payment-gateway-1.9.1.tar` & `mitol-django-payment-gateway-2023.1.17.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.761960 mitol-django-payment-gateway-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7821 2023-02-13 13:26:43.757959 mitol-django-payment-gateway-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.757959 mitol-django-payment-gateway-1.9.1/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.757959 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/
--rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34982 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/payment_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.757959 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/settings/cybersource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 13:26:43.757959 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7821 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-13 13:26:43.761960 mitol-django-payment-gateway-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     8676 2023-02-13 13:26:43.000000 mitol-django-payment-gateway-1.9.1/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.996655 mitol-django-payment-gateway-2023.1.17/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     7825 2023-07-05 16:16:56.996655 mitol-django-payment-gateway-2023.1.17/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      748 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.993322 mitol-django-payment-gateway-2023.1.17/mitol/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       56 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.993322 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1294 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/CHANGELOG.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     7317 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/README.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      171 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    34982 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/api.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      845 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/apps.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      893 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/constants.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1032 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/exceptions.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      705 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/payment_utils.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/py.typed
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.993322 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/settings/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/settings/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2053 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/settings/cybersource.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.993322 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     7825 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      811 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       90 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/zip-safe
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-05 16:16:56.996655 mitol-django-payment-gateway-2023.1.17/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     8673 2023-07-05 16:16:55.000000 mitol-django-payment-gateway-2023.1.17/setup.py
```

### Comparing `mitol-django-payment-gateway-1.9.1/PKG-INFO` & `mitol-django-payment-gateway-2023.1.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-payment-gateway
-Version: 1.9.1
+Version: 2023.1.17
 Summary: Django application to handle payment processing
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-payment_gateway
 ---
 
 This is the Open Learning Django Payment Gateway app. Its purpose is to wrap up payments and refunds processing in a reasonably generic and pluggable way, so that payment and refund processing is relatively straight-forward to implement in a given app.
```

### Comparing `mitol-django-payment-gateway-1.9.1/backend_shim.py` & `mitol-django-payment-gateway-2023.1.17/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/CHANGELOG.md` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+and this project uses date-based versioning.
 
+<!-- scriv-insert-here -->
 ## [1.9.0] - 2023-02-10
 
 ### Changed
 - Adds transaction search and lookup to the CyberSource payment gateway.
 
 ## [1.8.0] - 2023-01-17
```

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/README.md` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/api.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/apps.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/apps.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/constants.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/constants.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/exceptions.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/payment_utils.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/payment_utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol/payment_gateway/settings/cybersource.py` & `mitol-django-payment-gateway-2023.1.17/mitol/payment_gateway/settings/cybersource.py`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/PKG-INFO` & `mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-payment-gateway
-Version: 1.9.1
+Version: 2023.1.17
 Summary: Django application to handle payment processing
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-payment_gateway
 ---
 
 This is the Open Learning Django Payment Gateway app. Its purpose is to wrap up payments and refunds processing in a reasonably generic and pluggable way, so that payment and refund processing is relatively straight-forward to implement in a given app.
```

### Comparing `mitol-django-payment-gateway-1.9.1/mitol_django_payment_gateway.egg-info/SOURCES.txt` & `mitol-django-payment-gateway-2023.1.17/mitol_django_payment_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-payment-gateway-1.9.1/setup.py` & `mitol-django-payment-gateway-2023.1.17/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     'description': 'Django application to handle payment processing',
     'install_requires': (
         'cybersource-rest-client-python>=0.0.36',
         'django<4.0,>=2.2.12',
-        'mitol-django-common~=2.7.0',
+        'mitol-django-common',
         'setuptools',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-payment_gateway
 ---
 
 This is the Open Learning Django Payment Gateway app. Its purpose is to wrap up payments and refunds processing in a reasonably generic and pluggable way, so that payment and refund processing is relatively straight-forward to implement in a given app. 
@@ -153,11 +153,11 @@
         ),
     },
     'packages': (
         'mitol',
         'mitol.payment_gateway',
         'mitol.payment_gateway.settings',
     ),
-    'python_requires': '>=3.7',
-    'version': '1.9.1',
+    'python_requires': '>=3.8',
+    'version': '2023.1.17',
     'zip_safe': True,
 })
```

