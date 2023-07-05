# Comparing `tmp/risclog.zestreleaser.notify-1.0.2.tar.gz` & `tmp/risclog.zestreleaser.notify-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risclog.zestreleaser.notify-1.0.2.tar", last modified: Thu Apr  6 07:41:54 2023, max compression
+gzip compressed data, was "risclog.zestreleaser.notify-1.0.3.tar", last modified: Wed Jul  5 06:53:51 2023, max compression
```

## Comparing `risclog.zestreleaser.notify-1.0.2.tar` & `risclog.zestreleaser.notify-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:54.001439 risclog.zestreleaser.notify-1.0.2/
--rw-r--r--   0 sweh       (501) staff       (20)      162 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/AUTHORS.rst
--rw-r--r--   0 sweh       (501) staff       (20)      349 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/CHANGES.rst
--rw-r--r--   0 sweh       (501) staff       (20)     3601 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 sweh       (501) staff       (20)     1079 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/LICENSE
--rw-r--r--   0 sweh       (501) staff       (20)      513 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/MANIFEST.in
--rw-r--r--   0 sweh       (501) staff       (20)     2153 2023-04-06 07:41:54.001165 risclog.zestreleaser.notify-1.0.2/PKG-INFO
--rw-r--r--   0 sweh       (501) staff       (20)     1340 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/README.rst
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:53.998801 risclog.zestreleaser.notify-1.0.2/docs/
--rw-r--r--   0 sweh       (501) staff       (20)      628 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/Makefile
--rw-r--r--   0 sweh       (501) staff       (20)       28 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/authors.rst
--rwxr-xr-x   0 sweh       (501) staff       (20)     5173 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/conf.py
--rw-r--r--   0 sweh       (501) staff       (20)       33 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/contributing.rst
--rw-r--r--   0 sweh       (501) staff       (20)       28 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/history.rst
--rw-r--r--   0 sweh       (501) staff       (20)      341 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/index.rst
--rw-r--r--   0 sweh       (501) staff       (20)     1306 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/installation.rst
--rw-r--r--   0 sweh       (501) staff       (20)      789 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/make.bat
--rw-r--r--   0 sweh       (501) staff       (20)       27 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/readme.rst
--rw-r--r--   0 sweh       (501) staff       (20)      109 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/docs/usage.rst
--rw-r--r--   0 sweh       (501) staff       (20)     1043 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/pyproject.toml
--rw-r--r--   0 sweh       (501) staff       (20)       38 2023-04-06 07:41:54.001479 risclog.zestreleaser.notify-1.0.2/setup.cfg
--rw-r--r--   0 sweh       (501) staff       (20)     1895 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/setup.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:53.996225 risclog.zestreleaser.notify-1.0.2/src/
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:53.998921 risclog.zestreleaser.notify-1.0.2/src/risclog/
--rw-r--r--   0 sweh       (501) staff       (20)       56 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/__init__.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:54.000233 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/
--rw-r--r--   0 sweh       (501) staff       (20)       56 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/__init__.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:54.000670 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/
--rw-r--r--   0 sweh       (501) staff       (20)     1794 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/__init__.py
--rw-r--r--   0 sweh       (501) staff       (20)      244 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/config.py
--rw-r--r--   0 sweh       (501) staff       (20)      314 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/conftest.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:54.000910 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/tests/
--rw-r--r--   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/tests/__init__.py
--rw-r--r--   0 sweh       (501) staff       (20)      181 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/tests/test_config.py
-drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-04-06 07:41:54.000095 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/
--rw-r--r--   0 sweh       (501) staff       (20)     2153 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/PKG-INFO
--rw-r--r--   0 sweh       (501) staff       (20)     1004 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/SOURCES.txt
--rw-r--r--   0 sweh       (501) staff       (20)        1 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/dependency_links.txt
--rw-r--r--   0 sweh       (501) staff       (20)       75 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/entry_points.txt
--rw-r--r--   0 sweh       (501) staff       (20)       29 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/namespace_packages.txt
--rw-r--r--   0 sweh       (501) staff       (20)        1 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/not-zip-safe
--rw-r--r--   0 sweh       (501) staff       (20)      183 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/requires.txt
--rw-r--r--   0 sweh       (501) staff       (20)        8 2023-04-06 07:41:53.000000 risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/top_level.txt
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.513950 risclog.zestreleaser.notify-1.0.3/
+-rw-r--r--   0 sweh       (501) staff       (20)      162 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/AUTHORS.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      418 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/CHANGES.rst
+-rw-r--r--   0 sweh       (501) staff       (20)     3601 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 sweh       (501) staff       (20)     1079 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/LICENSE
+-rw-r--r--   0 sweh       (501) staff       (20)      513 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/MANIFEST.in
+-rw-r--r--   0 sweh       (501) staff       (20)     2153 2023-07-05 06:53:51.513811 risclog.zestreleaser.notify-1.0.3/PKG-INFO
+-rw-r--r--   0 sweh       (501) staff       (20)     1340 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/README.rst
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.511272 risclog.zestreleaser.notify-1.0.3/docs/
+-rw-r--r--   0 sweh       (501) staff       (20)      628 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/Makefile
+-rw-r--r--   0 sweh       (501) staff       (20)       28 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/authors.rst
+-rwxr-xr-x   0 sweh       (501) staff       (20)     5173 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/conf.py
+-rw-r--r--   0 sweh       (501) staff       (20)       33 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/contributing.rst
+-rw-r--r--   0 sweh       (501) staff       (20)       28 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/history.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      341 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/index.rst
+-rw-r--r--   0 sweh       (501) staff       (20)     1306 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/installation.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      789 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/make.bat
+-rw-r--r--   0 sweh       (501) staff       (20)       27 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/readme.rst
+-rw-r--r--   0 sweh       (501) staff       (20)      109 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/docs/usage.rst
+-rw-r--r--   0 sweh       (501) staff       (20)     1043 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/pyproject.toml
+-rw-r--r--   0 sweh       (501) staff       (20)       38 2023-07-05 06:53:51.513998 risclog.zestreleaser.notify-1.0.3/setup.cfg
+-rw-r--r--   0 sweh       (501) staff       (20)     1897 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/setup.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.508675 risclog.zestreleaser.notify-1.0.3/src/
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.511414 risclog.zestreleaser.notify-1.0.3/src/risclog/
+-rw-r--r--   0 sweh       (501) staff       (20)       56 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/__init__.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.512793 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/
+-rw-r--r--   0 sweh       (501) staff       (20)       56 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/__init__.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.513237 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/
+-rw-r--r--   0 sweh       (501) staff       (20)     1794 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/__init__.py
+-rw-r--r--   0 sweh       (501) staff       (20)      244 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/config.py
+-rw-r--r--   0 sweh       (501) staff       (20)      314 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/conftest.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.513522 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/tests/
+-rw-r--r--   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/tests/__init__.py
+-rw-r--r--   0 sweh       (501) staff       (20)      181 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/tests/test_config.py
+drwxr-xr-x   0 sweh       (501) staff       (20)        0 2023-07-05 06:53:51.512654 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/
+-rw-r--r--   0 sweh       (501) staff       (20)     2153 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/PKG-INFO
+-rw-r--r--   0 sweh       (501) staff       (20)     1004 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/SOURCES.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        1 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/dependency_links.txt
+-rw-r--r--   0 sweh       (501) staff       (20)       75 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/entry_points.txt
+-rw-r--r--   0 sweh       (501) staff       (20)       29 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/namespace_packages.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        1 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/not-zip-safe
+-rw-r--r--   0 sweh       (501) staff       (20)      185 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/requires.txt
+-rw-r--r--   0 sweh       (501) staff       (20)        8 2023-07-05 06:53:51.000000 risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/top_level.txt
```

### Comparing `risclog.zestreleaser.notify-1.0.2/CONTRIBUTING.rst` & `risclog.zestreleaser.notify-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/LICENSE` & `risclog.zestreleaser.notify-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/MANIFEST.in` & `risclog.zestreleaser.notify-1.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/PKG-INFO` & `risclog.zestreleaser.notify-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risclog.zestreleaser.notify
-Version: 1.0.2
+Version: 1.0.3
 Summary: Notify about new release in keybase channel.
 Home-page: https://github.com/risclog-solution/risclog.zestreleaser.notify
 Author: riscLOG Solution GmbH
 Author-email: info@risclog.de
 License: MIT license
 Keywords: risclog.zestreleaser.notify
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `risclog.zestreleaser.notify-1.0.2/README.rst` & `risclog.zestreleaser.notify-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/docs/Makefile` & `risclog.zestreleaser.notify-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/docs/conf.py` & `risclog.zestreleaser.notify-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/docs/installation.rst` & `risclog.zestreleaser.notify-1.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/docs/make.bat` & `risclog.zestreleaser.notify-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/pyproject.toml` & `risclog.zestreleaser.notify-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/setup.py` & `risclog.zestreleaser.notify-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description='Notify about new release in keybase channel.',
     install_requires=[
-        'pydantic[dotenv]',
+        'pydantic[dotenv]<2',
         # Add your dependencies here
         'zest.releaser >= 5.0',
         'requests',
         'six',
     ],
     extras_require={
         'docs': [
@@ -57,10 +57,10 @@
     include_package_data=True,
     keywords='risclog.zestreleaser.notify',
     name='risclog.zestreleaser.notify',
     packages=find_packages('src'),
     namespace_packages=['risclog', 'risclog.zestreleaser'],
     package_dir={'': 'src'},
     url='https://github.com/risclog-solution/risclog.zestreleaser.notify',
-    version='1.0.2',
+    version='1.0.3',
     zip_safe=False,
 )
```

### Comparing `risclog.zestreleaser.notify-1.0.2/src/risclog/zestreleaser/notify/__init__.py` & `risclog.zestreleaser.notify-1.0.3/src/risclog/zestreleaser/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/PKG-INFO` & `risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risclog.zestreleaser.notify
-Version: 1.0.2
+Version: 1.0.3
 Summary: Notify about new release in keybase channel.
 Home-page: https://github.com/risclog-solution/risclog.zestreleaser.notify
 Author: riscLOG Solution GmbH
 Author-email: info@risclog.de
 License: MIT license
 Keywords: risclog.zestreleaser.notify
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `risclog.zestreleaser.notify-1.0.2/src/risclog.zestreleaser.notify.egg-info/SOURCES.txt` & `risclog.zestreleaser.notify-1.0.3/src/risclog.zestreleaser.notify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

