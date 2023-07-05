# Comparing `tmp/cephes4py-0.0.2.tar.gz` & `tmp/cephes4py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cephes4py-0.0.2.tar", last modified: Wed Jul  5 10:53:49 2023, max compression
+gzip compressed data, was "cephes4py-0.0.3.tar", last modified: Wed Jul  5 13:35:13 2023, max compression
```

## Comparing `cephes4py-0.0.2.tar` & `cephes4py-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 10:53:49.861669 cephes4py-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1076 2023-07-03 10:15:34.000000 cephes4py-0.0.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-05 10:41:05.000000 cephes4py-0.0.2/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4195 2023-07-05 10:53:49.861669 cephes4py-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-07-05 08:37:35.000000 cephes4py-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 10:53:49.861669 cephes4py-0.0.2/cephes4py/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8563 2023-07-05 09:10:05.000000 cephes4py-0.0.2/cephes4py/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      434 2023-07-04 06:10:05.000000 cephes4py-0.0.2/cephes4py/_test.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4705 2023-07-05 10:52:08.000000 cephes4py-0.0.2/cephes4py/build_hcephes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5346 2023-07-03 19:20:37.000000 cephes4py-0.0.2/cephes4py/interface.h
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 10:53:49.861669 cephes4py-0.0.2/cephes4py.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4195 2023-07-05 10:53:49.000000 cephes4py-0.0.2/cephes4py.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      334 2023-07-05 10:53:49.000000 cephes4py-0.0.2/cephes4py.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-05 10:53:49.000000 cephes4py-0.0.2/cephes4py.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-05 09:06:24.000000 cephes4py-0.0.2/cephes4py.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-07-05 10:53:49.000000 cephes4py-0.0.2/cephes4py.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       35 2023-07-05 10:53:49.000000 cephes4py-0.0.2/cephes4py.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      948 2023-07-05 10:53:49.861669 cephes4py-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      376 2023-07-05 10:51:53.000000 cephes4py-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 13:35:13.860717 cephes4py-0.0.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1076 2023-07-03 10:15:34.000000 cephes4py-0.0.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-07-05 10:41:05.000000 cephes4py-0.0.3/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4195 2023-07-05 13:35:13.860717 cephes4py-0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3462 2023-07-05 08:37:35.000000 cephes4py-0.0.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 13:35:13.856717 cephes4py-0.0.3/cephes4py/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8563 2023-07-05 09:10:05.000000 cephes4py-0.0.3/cephes4py/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      434 2023-07-04 06:10:05.000000 cephes4py-0.0.3/cephes4py/_test.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4705 2023-07-05 10:52:08.000000 cephes4py-0.0.3/cephes4py/build_hcephes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5346 2023-07-03 19:20:37.000000 cephes4py-0.0.3/cephes4py/interface.h
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-05 13:35:13.860717 cephes4py-0.0.3/cephes4py.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4195 2023-07-05 13:35:13.000000 cephes4py-0.0.3/cephes4py.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      334 2023-07-05 13:35:13.000000 cephes4py-0.0.3/cephes4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-05 13:35:13.000000 cephes4py-0.0.3/cephes4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-05 09:06:24.000000 cephes4py-0.0.3/cephes4py.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-07-05 13:35:13.000000 cephes4py-0.0.3/cephes4py.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       35 2023-07-05 13:35:13.000000 cephes4py-0.0.3/cephes4py.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      948 2023-07-05 13:35:13.860717 cephes4py-0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      386 2023-07-05 13:34:07.000000 cephes4py-0.0.3/setup.py
```

### Comparing `cephes4py-0.0.2/LICENSE` & `cephes4py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cephes4py-0.0.2/PKG-INFO` & `cephes4py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cephes4py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Numba-friendly Python bindings to Cephes math library
 Home-page: https://github.com/jonmest/cephes4py
 Download-URL: https://github.com/limix/ncephes
 Author: Jon Cavallie Mester
 Author-email: jonmester3@gmail.com
 Maintainer: Jon Cavallie Mester
 Maintainer-email: jonmester3@gmail.com
```

### Comparing `cephes4py-0.0.2/README.md` & `cephes4py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cephes4py-0.0.2/cephes4py/__init__.py` & `cephes4py-0.0.3/cephes4py/__init__.py`

 * *Files identical despite different names*

### Comparing `cephes4py-0.0.2/cephes4py/build_hcephes.py` & `cephes4py-0.0.3/cephes4py/build_hcephes.py`

 * *Files identical despite different names*

### Comparing `cephes4py-0.0.2/cephes4py/interface.h` & `cephes4py-0.0.3/cephes4py/interface.h`

 * *Files identical despite different names*

### Comparing `cephes4py-0.0.2/cephes4py.egg-info/PKG-INFO` & `cephes4py-0.0.3/cephes4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cephes4py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Numba-friendly Python bindings to Cephes math library
 Home-page: https://github.com/jonmest/cephes4py
 Download-URL: https://github.com/limix/ncephes
 Author: Jon Cavallie Mester
 Author-email: jonmester3@gmail.com
 Maintainer: Jon Cavallie Mester
 Maintainer-email: jonmester3@gmail.com
```

### Comparing `cephes4py-0.0.2/setup.cfg` & `cephes4py-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cephes4py
-version = 0.0.2
+version = 0.0.3
 author = Jon Cavallie Mester
 author_email = jonmester3@gmail.com
 classifiers = 
 	Development Status :: 1 - Planning
 	Environment :: Console
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

