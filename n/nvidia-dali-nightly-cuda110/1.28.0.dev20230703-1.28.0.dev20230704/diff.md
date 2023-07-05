# Comparing `tmp/nvidia-dali-nightly-cuda110-1.28.0.dev20230703.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.28.0.dev20230704.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.28.0.dev20230703.tar", last modified: Mon Jul  3 11:04:40 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.28.0.dev20230704.tar", last modified: Wed Jul  5 11:04:50 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230703.tar` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230704.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-03 11:04:40.615980 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 00:28:35.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-03 11:04:40.615980 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-03 11:04:40.615980 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-03 11:04:40.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-03 11:04:40.615980 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 00:28:35.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230703/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 11:04:50.468753 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-05 11:04:50.468753 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-05 11:04:50.468753 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-05 11:04:50.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-05 11:04:50.468753 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda110-1.28.0.dev20230704/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230703/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230704/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230703/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230704/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.28.0.dev20230703
+Version: 1.28.0.dev20230704
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230703/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230704/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.28.0.dev20230703
+Version: 1.28.0.dev20230704
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.28.0.dev20230703/setup.py` & `nvidia-dali-nightly-cuda110-1.28.0.dev20230704/setup.py`

 * *Files identical despite different names*
