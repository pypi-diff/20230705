# Comparing `tmp/ciscopykit-1.0.tar.gz` & `tmp/ciscopykit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.0.tar", last modified: Sun Jul  2 22:52:00 2023, max compression
+gzip compressed data, was "ciscopykit-1.1.tar", last modified: Wed Jul  5 00:06:56 2023, max compression
```

## Comparing `ciscopykit-1.0.tar` & `ciscopykit-1.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2023-07-02 22:52:00.660173 ciscopykit-1.0/
--rw-r--r--   0 vince      (501) staff       (20)       91 2023-07-02 22:51:04.000000 ciscopykit-1.0/MANIFEST.in
--rw-r--r--   0 vince      (501) staff       (20)      755 2023-07-02 22:52:00.659739 ciscopykit-1.0/PKG-INFO
--rw-r--r--   0 vince      (501) staff       (20)        0 2023-07-02 22:14:18.000000 ciscopykit-1.0/README.md
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2023-07-02 22:52:00.652338 ciscopykit-1.0/ciscopykit/
--rw-r--r--   0 vince      (501) staff       (20)        0 2023-07-02 22:10:09.000000 ciscopykit-1.0/ciscopykit/__init__.py
--rw-r--r--   0 vince      (501) staff       (20)      695 2023-07-02 22:21:56.000000 ciscopykit-1.0/ciscopykit/app.py
--rw-r--r--   0 vince      (501) staff       (20)     6428 2023-07-02 22:25:32.000000 ciscopykit-1.0/ciscopykit/device.py
--rw-r--r--   0 vince      (501) staff       (20)     2268 2023-07-02 22:31:47.000000 ciscopykit-1.0/ciscopykit/interface.py
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2023-07-02 22:52:00.658946 ciscopykit-1.0/ciscopykit/templates/
--rw-r--r--   0 vince      (501) staff       (20)        0 2023-07-02 22:10:09.000000 ciscopykit-1.0/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 vince      (501) staff       (20)        0 2023-07-02 22:52:00.657915 ciscopykit-1.0/ciscopykit.egg-info/
--rw-r--r--   0 vince      (501) staff       (20)      755 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 vince      (501) staff       (20)      359 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 vince      (501) staff       (20)        1 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 vince      (501) staff       (20)       59 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 vince      (501) staff       (20)       36 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 vince      (501) staff       (20)       11 2023-07-02 22:52:00.000000 ciscopykit-1.0/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 vince      (501) staff       (20)       38 2023-07-02 22:52:00.660387 ciscopykit-1.0/setup.cfg
--rw-r--r--   0 vince      (501) staff       (20)     1129 2023-07-02 22:48:56.000000 ciscopykit-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.486178 ciscopykit-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 00:06:41.000000 ciscopykit-1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-05 00:06:41.000000 ciscopykit-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 00:06:56.486178 ciscopykit-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-05 00:06:41.000000 ciscopykit-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.482177 ciscopykit-1.1/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.486178 ciscopykit-1.1/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:41.000000 ciscopykit-1.1/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:06:56.482177 ciscopykit-1.1/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 00:06:56.000000 ciscopykit-1.1/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:06:56.486178 ciscopykit-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-05 00:06:41.000000 ciscopykit-1.1/setup.py
```

### Comparing `ciscopykit-1.0/PKG-INFO` & `ciscopykit-1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.0
-Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 and Cisco Packet Tracer
+Version: 1.1
+Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/devinci-it/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE.md
 
-A network management toolkit for Cisco devices. It 
-provides classes and methods to manage network devices, interfaces, and 
-configurations.
+A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.
```

### Comparing `ciscopykit-1.0/ciscopykit/app.py` & `ciscopykit-1.1/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.0/ciscopykit/interface.py` & `ciscopykit-1.1/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.0/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-1.1/ciscopykit.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.0
-Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 and Cisco Packet Tracer
+Version: 1.1
+Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/devinci-it/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE.md
 
-A network management toolkit for Cisco devices. It 
-provides classes and methods to manage network devices, interfaces, and 
-configurations.
+A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.
```

### Comparing `ciscopykit-1.0/setup.py` & `ciscopykit-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.0',
+    version='1.1',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
-    description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 and Cisco Packet Tracer',
-    long_description='''A network management toolkit for Cisco devices. It 
-provides classes and methods to manage network devices, interfaces, and 
-configurations.''',
+    description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
+    long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/devinci-it/ciscopykit',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.11'
+
+
+
     ],
     install_requires=[
         'click',
         'networkx',
         'matplotlib',
         'ipaddress',
     ],
     entry_points={
         'console_scripts': [
             'ciscopykit = ciscopykit.entry_point:main',
         ],
     },
 )
-
```

