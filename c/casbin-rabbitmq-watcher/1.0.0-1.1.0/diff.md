# Comparing `tmp/casbin-rabbitmq-watcher-1.0.0.tar.gz` & `tmp/casbin-rabbitmq-watcher-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin-rabbitmq-watcher-1.0.0.tar", last modified: Wed Jul  5 02:49:59 2023, max compression
+gzip compressed data, was "casbin-rabbitmq-watcher-1.1.0.tar", last modified: Wed Jul  5 04:05:19 2023, max compression
```

## Comparing `casbin-rabbitmq-watcher-1.0.0.tar` & `casbin-rabbitmq-watcher-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:49:59.062805 casbin-rabbitmq-watcher-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-05 02:49:59.062805 casbin-rabbitmq-watcher-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:49:59.062805 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:49:59.062805 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-05 02:49:59.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 02:49:59.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:49:59.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 02:49:59.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 02:49:59.000000 casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 02:49:59.066805 casbin-rabbitmq-watcher-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:49:59.062805 casbin-rabbitmq-watcher-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-05 02:49:27.000000 casbin-rabbitmq-watcher-1.0.0/tests/test_rabbit_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-05 04:05:19.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 04:05:19.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 04:05:19.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 04:05:19.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 04:05:19.000000 casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 04:05:19.527621 casbin-rabbitmq-watcher-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-05 04:04:44.000000 casbin-rabbitmq-watcher-1.1.0/tests/test_rabbit_watcher.py
```

### Comparing `casbin-rabbitmq-watcher-1.0.0/LICENSE` & `casbin-rabbitmq-watcher-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin-rabbitmq-watcher-1.0.0/PKG-INFO` & `casbin-rabbitmq-watcher-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-rabbitmq-watcher
-Version: 1.0.0
+Version: 1.1.0
 Summary: Casbin role watcher to be used for monitoring updates to policies for PyCasbin
 Home-page: https://github.com/pycasbin/rabbitmq-watcher
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Rabbitmq,casbin-watcher,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rabbitmq-watcher
 
-[![tests](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml)
+[![build](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/rabbitmq-watcher/badge.svg)](https://coveralls.io/github/pycasbin/rabbitmq-watcher)
 [![Version](https://img.shields.io/pypi/v/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Download](https://img.shields.io/pypi/dm/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
 
 Rabbitmq Watcher is the rabbitmq watcher for pycasbin. With this library, Casbin can synchronize the policy with the database in multiple enforcer instances.
```

### Comparing `casbin-rabbitmq-watcher-1.0.0/README.md` & `casbin-rabbitmq-watcher-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # rabbitmq-watcher
 
-[![tests](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml)
+[![build](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/rabbitmq-watcher/badge.svg)](https://coveralls.io/github/pycasbin/rabbitmq-watcher)
 [![Version](https://img.shields.io/pypi/v/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Download](https://img.shields.io/pypi/dm/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
 
 Rabbitmq Watcher is the rabbitmq watcher for pycasbin. With this library, Casbin can synchronize the policy with the database in multiple enforcer instances.
@@ -45,8 +45,8 @@
 
 ## Getting Help
 
 - [Casbin](https://github.com/casbin/pycasbin)
 
 ## License
 
-This project is under Apache 2.0 License. See the [LICENSE](LICENSE) file for the full license text.
+This project is under Apache 2.0 License. See the [LICENSE](LICENSE) file for the full license text.
```

### Comparing `casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher/watcher.py` & `casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher/watcher.py`

 * *Files identical despite different names*

### Comparing `casbin-rabbitmq-watcher-1.0.0/casbin_rabbitmq_watcher.egg-info/PKG-INFO` & `casbin-rabbitmq-watcher-1.1.0/casbin_rabbitmq_watcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-rabbitmq-watcher
-Version: 1.0.0
+Version: 1.1.0
 Summary: Casbin role watcher to be used for monitoring updates to policies for PyCasbin
 Home-page: https://github.com/pycasbin/rabbitmq-watcher
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Rabbitmq,casbin-watcher,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rabbitmq-watcher
 
-[![tests](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/release.yml)
+[![build](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml/badge.svg)](https://github.com/pycasbin/rabbitmq-watcher/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/rabbitmq-watcher/badge.svg)](https://coveralls.io/github/pycasbin/rabbitmq-watcher)
 [![Version](https://img.shields.io/pypi/v/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Download](https://img.shields.io/pypi/dm/casbin-rabbitmq-watcher.svg)](https://pypi.org/project/casbin-rabbitmq-watcher/)
 [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/casbin/lobby)
 
 Rabbitmq Watcher is the rabbitmq watcher for pycasbin. With this library, Casbin can synchronize the policy with the database in multiple enforcer instances.
```

### Comparing `casbin-rabbitmq-watcher-1.0.0/setup.py` & `casbin-rabbitmq-watcher-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `casbin-rabbitmq-watcher-1.0.0/tests/test_rabbit_watcher.py` & `casbin-rabbitmq-watcher-1.1.0/tests/test_rabbit_watcher.py`

 * *Files identical despite different names*

