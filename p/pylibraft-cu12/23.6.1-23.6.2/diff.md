# Comparing `tmp/pylibraft-cu12-23.6.1.tar.gz` & `tmp/pylibraft-cu12-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibraft-cu12-23.6.1.tar", last modified: Wed Jun 14 14:37:03 2023, max compression
+gzip compressed data, was "pylibraft-cu12-23.6.2.tar", last modified: Wed Jul  5 19:19:04 2023, max compression
```

## Comparing `pylibraft-cu12-23.6.1.tar` & `pylibraft-cu12-23.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:37:03.139843 pylibraft-cu12-23.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 14:12:21.000000 pylibraft-cu12-23.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-14 14:37:03.139843 pylibraft-cu12-23.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 14:37:03.139843 pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 14:37:03.000000 pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 14:37:03.139843 pylibraft-cu12-23.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 14:12:21.000000 pylibraft-cu12-23.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 19:19:04.556778 pylibraft-cu12-23.6.2/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      446 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-13 15:37:00.000000 pylibraft-cu12-23.6.2/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-07-05 19:19:04.555778 pylibraft-cu12-23.6.2/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 19:19:04.554778 pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1604 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-05 19:19:04.000000 pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-05 19:19:04.556778 pylibraft-cu12-23.6.2/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-13 15:37:00.000000 pylibraft-cu12-23.6.2/setup.py
```

### Comparing `pylibraft-cu12-23.6.1/LICENSE.md` & `pylibraft-cu12-23.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylibraft-cu12-23.6.1/PKG-INFO` & `pylibraft-cu12-23.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibraft-cu12
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibraft-cu12-23.6.1/pylibraft_cu12.egg-info/PKG-INFO` & `pylibraft-cu12-23.6.2/pylibraft_cu12.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibraft-cu12
-Version: 23.6.1
+Version: 23.6.2
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `pylibraft-cu12-23.6.1/setup.py` & `pylibraft-cu12-23.6.2/setup.py`

 * *Files identical despite different names*

