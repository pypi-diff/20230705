# Comparing `tmp/melctl_client-5.5.1.tar.gz` & `tmp/melctl_client-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melctl_client-5.5.1.tar", last modified: Mon Apr 24 09:18:38 2023, max compression
+gzip compressed data, was "melctl_client-5.5.2.tar", last modified: Wed Jul  5 12:35:07 2023, max compression
```

## Comparing `melctl_client-5.5.1.tar` & `melctl_client-5.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-24 09:18:19.000000 melctl_client-5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 09:18:38.138778 melctl_client-5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 09:18:19.000000 melctl_client-5.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 09:18:38.000000 melctl_client-5.5.1/melctl_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 09:18:37.000000 melctl_client-5.5.1/melctl_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:18:38.138778 melctl_client-5.5.1/melctl_client_plugins/builtins/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/complete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-24 09:18:19.000000 melctl_client-5.5.1/melctl_client_plugins/builtins/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:18:38.138778 melctl_client-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 09:18:19.000000 melctl_client-5.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-05 12:34:59.000000 melctl_client-5.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-05 12:35:07.234079 melctl_client-5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 12:34:59.000000 melctl_client-5.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/melctl_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/melctl_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/melctl_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 12:35:07.000000 melctl_client-5.5.2/melctl_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/melctl_client_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:35:07.234079 melctl_client-5.5.2/melctl_client_plugins/builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-05 12:34:59.000000 melctl_client-5.5.2/melctl_client_plugins/builtins/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:35:07.234079 melctl_client-5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-05 12:34:59.000000 melctl_client-5.5.2/setup.py
```

### Comparing `melctl_client-5.5.1/LICENSE` & `melctl_client-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/PKG-INFO` & `melctl_client-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melctl_client
-Version: 5.5.1
+Version: 5.5.2
 Summary: Command-line client for LuxProvide API (MelCtl)
 Home-page: https://github.com/LuxProvide/melctl-client
 Author: jpclipffel
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 This package provides the base MelCtl command-line client.
```

### Comparing `melctl_client-5.5.1/melctl_client/__init__.py` & `melctl_client-5.5.2/melctl_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 __email__      = 'jean-philippe.clipffel@lxp.lu'
 __author__     = 'Jean-Philippe Clipffel <jean-philippe.clipffel@lxp.lu>'
 __license__    = 'BSD-3-Clause'
 __copyright__  = 'Copyright (c) 2023 LuxProvide S.A.'
 __maintainer__ = 'Jean-Philippe Clipffel'
 
 
-__version__ = '5.5.1'
+__version__ = '5.5.2'
 __version_name__ = 'Pedantic Santa'
```

### Comparing `melctl_client-5.5.1/melctl_client/__main__.py` & `melctl_client-5.5.2/melctl_client/__main__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client/commands.py` & `melctl_client-5.5.2/melctl_client/commands.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client/config.py` & `melctl_client-5.5.2/melctl_client/config.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client/hints.py` & `melctl_client-5.5.2/melctl_client/hints.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client/utils/__init__.py` & `melctl_client-5.5.2/melctl_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client.egg-info/PKG-INFO` & `melctl_client-5.5.2/melctl_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melctl-client
-Version: 5.5.1
+Version: 5.5.2
 Summary: Command-line client for LuxProvide API (MelCtl)
 Home-page: https://github.com/LuxProvide/melctl-client
 Author: jpclipffel
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 This package provides the base MelCtl command-line client.
```

### Comparing `melctl_client-5.5.1/melctl_client.egg-info/SOURCES.txt` & `melctl_client-5.5.2/melctl_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/__init__.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/complete.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/complete.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/conf.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/conf.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/login.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/login.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/ping.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/ping.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/melctl_client_plugins/builtins/version.py` & `melctl_client-5.5.2/melctl_client_plugins/builtins/version.py`

 * *Files identical despite different names*

### Comparing `melctl_client-5.5.1/setup.py` & `melctl_client-5.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             'melctl=melctl_client.__main__:main'
         ]
     },
     install_requires=[
         'requests >= 1.28',
         'tabulate >= 0.8',
         'pygments >= 2.12',
-        'pydantic[dotenv] >= 1.9',
+        'pydantic[dotenv] < 2',
         'pyyaml >= 6.0',
         'python-jose[cryptography] >= 3.3',
         # Library stubs
         'types-pyyaml',
         'types-tabulate',
         'types-pygments'
     ]
```

