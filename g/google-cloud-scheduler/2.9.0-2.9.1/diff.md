# Comparing `tmp/google-cloud-scheduler-2.9.0.tar.gz` & `tmp/google-cloud-scheduler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-scheduler-2.9.0.tar", last modified: Tue Jan 10 18:45:45 2023, max compression
+gzip compressed data, was "google-cloud-scheduler-2.9.1.tar", last modified: Mon Jan 23 16:11:35 2023, max compression
```

## Comparing `google-cloud-scheduler-2.9.0.tar` & `google-cloud-scheduler-2.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4837 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3915 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.571199 google-cloud-scheduler-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.571199 google-cloud-scheduler-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.575199 google-cloud-scheduler-2.9.0/google/cloud/scheduler/
--rw-rw-r--   0 root         (0)     1003     1881 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.575199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/
--rw-rw-r--   0 root         (0)     1003     1681 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2341 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/__init__.py
--rw-rw-r--   0 root         (0)     1003    46135 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/async_client.py
--rw-rw-r--   0 root         (0)     1003    55515 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/client.py
--rw-rw-r--   0 root         (0)     1003     5634 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9996 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20378 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20811 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/
--rw-rw-r--   0 root         (0)     1003     1403 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7712 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/cloudscheduler.py
--rw-rw-r--   0 root         (0)     1003    13476 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/job.py
--rw-rw-r--   0 root         (0)     1003    18915 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/target.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1681 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2351 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.579199 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.583200 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/__init__.py
--rw-rw-r--   0 root         (0)     1003    51357 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/async_client.py
--rw-rw-r--   0 root         (0)     1003    59975 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/client.py
--rw-rw-r--   0 root         (0)     1003     5679 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.583200 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11409 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22239 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22672 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.583200 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1403 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9516 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/cloudscheduler.py
--rw-rw-r--   0 root         (0)     1003    14773 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/job.py
--rw-rw-r--   0 root         (0)     1003    19799 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/target.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/
--rw-r--r--   0 root         (0)     1003     4837 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2714 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 18:45:45.000000 google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2982 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003      938 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   125824 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1/test_cloud_scheduler.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 18:45:45.587200 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   137957 2023-01-10 18:42:03.000000 google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1beta1/test_cloud_scheduler.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4837 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3915 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.285305 google-cloud-scheduler-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.285305 google-cloud-scheduler-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler/
+-rw-rw-r--   0 root         (0)     1003     1881 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/
+-rw-rw-r--   0 root         (0)     1003     1681 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2341 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46135 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/async_client.py
+-rw-rw-r--   0 root         (0)     1003    55541 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/client.py
+-rw-rw-r--   0 root         (0)     1003     5634 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9996 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20378 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20811 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.289307 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1403 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7712 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/cloudscheduler.py
+-rw-rw-r--   0 root         (0)     1003    14447 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/job.py
+-rw-rw-r--   0 root         (0)     1003    19313 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/target.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1681 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2351 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51357 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/async_client.py
+-rw-rw-r--   0 root         (0)     1003    60001 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/client.py
+-rw-rw-r--   0 root         (0)     1003     5679 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11409 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22239 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22672 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1403 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9516 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/cloudscheduler.py
+-rw-rw-r--   0 root         (0)     1003    15759 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/job.py
+-rw-rw-r--   0 root         (0)     1003    20197 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/target.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.293309 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/
+-rw-r--r--   0 root         (0)     1003     4837 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2714 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:11:35.000000 google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2982 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003      938 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   125824 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1/test_cloud_scheduler.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:11:35.297310 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   137957 2023-01-23 16:08:09.000000 google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1beta1/test_cloud_scheduler.py
```

### Comparing `google-cloud-scheduler-2.9.0/LICENSE` & `google-cloud-scheduler-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/MANIFEST.in` & `google-cloud-scheduler-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/PKG-INFO` & `google-cloud-scheduler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-scheduler
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Scheduler API client library
 Home-page: https://github.com/googleapis/python-scheduler
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-scheduler-2.9.0/README.rst` & `google-cloud-scheduler-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler/gapic_version.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/gapic_metadata.json` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/gapic_version.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/async_client.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/client.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1354,15 +1354,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CloudSchedulerClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/pagers.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/base.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc_asyncio.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/services/cloud_scheduler/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/cloudscheduler.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/job.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,40 +16,40 @@
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.scheduler_v1.types import target
+from google.cloud.scheduler_v1beta1.types import target
 
 __protobuf__ = proto.module(
-    package="google.cloud.scheduler.v1",
+    package="google.cloud.scheduler.v1beta1",
     manifest={
         "Job",
         "RetryConfig",
     },
 )
 
 
 class Job(proto.Message):
     r"""Configuration for a job.
-    The maximum allowed size for a job is 100KB.
+    The maximum allowed size for a job is 1MB.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Optionally caller-specified in
-            [CreateJob][google.cloud.scheduler.v1.CloudScheduler.CreateJob],
+            [CreateJob][google.cloud.scheduler.v1beta1.CloudScheduler.CreateJob],
             after which it becomes output only.
 
             The job name. For example:
             ``projects/PROJECT_ID/locations/LOCATION_ID/jobs/JOB_ID``.
 
             -  ``PROJECT_ID`` can contain letters ([A-Za-z]), numbers
                ([0-9]), hyphens (-), colons (:), or periods (.). For
@@ -62,109 +62,151 @@
                For more information, see
                https://cloud.google.com/about/locations/.
             -  ``JOB_ID`` can contain only letters ([A-Za-z]), numbers
                ([0-9]), hyphens (-), or underscores (_). The maximum
                length is 500 characters.
         description (str):
             Optionally caller-specified in
-            [CreateJob][google.cloud.scheduler.v1.CloudScheduler.CreateJob]
+            [CreateJob][google.cloud.scheduler.v1beta1.CloudScheduler.CreateJob]
             or
-            [UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob].
+            [UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob].
 
             A human-readable description for the job. This string must
             not contain more than 500 characters.
-        pubsub_target (google.cloud.scheduler_v1.types.PubsubTarget):
+        pubsub_target (google.cloud.scheduler_v1beta1.types.PubsubTarget):
             Pub/Sub target.
 
             This field is a member of `oneof`_ ``target``.
-        app_engine_http_target (google.cloud.scheduler_v1.types.AppEngineHttpTarget):
+        app_engine_http_target (google.cloud.scheduler_v1beta1.types.AppEngineHttpTarget):
             App Engine HTTP target.
 
             This field is a member of `oneof`_ ``target``.
-        http_target (google.cloud.scheduler_v1.types.HttpTarget):
+        http_target (google.cloud.scheduler_v1beta1.types.HttpTarget):
             HTTP target.
 
             This field is a member of `oneof`_ ``target``.
         schedule (str):
             Required, except when used with
-            [UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob].
+            [UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob].
 
             Describes the schedule on which the job will be executed.
 
             The schedule can be either of the following types:
 
-            -  `Crontab <http://en.wikipedia.org/wiki/Cron#Overview>`__
+            -  `Crontab <https://en.wikipedia.org/wiki/Cron#Overview>`__
             -  English-like
                `schedule <https://cloud.google.com/scheduler/docs/configuring/cron-job-schedules>`__
 
             As a general rule, execution ``n + 1`` of a job will not
             begin until execution ``n`` has finished. Cloud Scheduler
             will never allow two simultaneously outstanding executions.
             For example, this implies that if the ``n+1``\ th execution
             is scheduled to run at 16:00 but the ``n``\ th execution
             takes until 16:15, the ``n+1``\ th execution will not start
             until ``16:15``. A scheduled start time will be delayed if
             the previous execution has not ended when its scheduled time
             occurs.
 
             If
-            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
             > 0 and a job attempt fails, the job will be tried a total
             of
-            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
             times, with exponential backoff, until the next scheduled
             start time.
         time_zone (str):
             Specifies the time zone to be used in interpreting
-            [schedule][google.cloud.scheduler.v1.Job.schedule]. The
+            [schedule][google.cloud.scheduler.v1beta1.Job.schedule]. The
             value of this field must be a time zone name from the `tz
             database <http://en.wikipedia.org/wiki/Tz_database>`__.
 
             Note that some time zones include a provision for daylight
             savings time. The rules for daylight saving time are
             determined by the chosen tz. For UTC use the string "utc".
             If a time zone is not specified, the default will be in UTC
             (also known as GMT).
         user_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time of the job.
-        state (google.cloud.scheduler_v1.types.Job.State):
+        state (google.cloud.scheduler_v1beta1.types.Job.State):
             Output only. State of the job.
         status (google.rpc.status_pb2.Status):
             Output only. The response from the target for
             the last attempted execution.
         schedule_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The next time the job is
             scheduled. Note that this may be a retry of a
             previously failed attempt or the next execution
             time according to the schedule.
         last_attempt_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the last job attempt
             started.
-        retry_config (google.cloud.scheduler_v1.types.RetryConfig):
+        retry_config (google.cloud.scheduler_v1beta1.types.RetryConfig):
             Settings that determine the retry behavior.
         attempt_deadline (google.protobuf.duration_pb2.Duration):
             The deadline for job attempts. If the request handler does
             not respond by this deadline then the request is cancelled
             and the attempt is marked as a ``DEADLINE_EXCEEDED``
             failure. The failed attempt can be viewed in execution logs.
             Cloud Scheduler will retry the job according to the
-            [RetryConfig][google.cloud.scheduler.v1.RetryConfig].
+            [RetryConfig][google.cloud.scheduler.v1beta1.RetryConfig].
 
-            The allowed duration for this deadline is:
+            The default and the allowed values depend on the type of
+            target:
 
             -  For [HTTP
-               targets][google.cloud.scheduler.v1.Job.http_target],
-               between 15 seconds and 30 minutes.
+               targets][google.cloud.scheduler.v1beta1.Job.http_target],
+               the default is 3 minutes. The deadline must be in the
+               interval [15 seconds, 30 minutes].
+
             -  For [App Engine HTTP
-               targets][google.cloud.scheduler.v1.Job.app_engine_http_target],
-               between 15 seconds and 24 hours.
+               targets][google.cloud.scheduler.v1beta1.Job.app_engine_http_target],
+               0 indicates that the request has the default deadline.
+               The default deadline depends on the scaling type of the
+               service: 10 minutes for standard apps with automatic
+               scaling, 24 hours for standard apps with manual and basic
+               scaling, and 60 minutes for flex apps. If the request
+               deadline is set, it must be in the interval [15 seconds,
+               24 hours 15 seconds].
+
+            -  For [Pub/Sub
+               targets][google.cloud.scheduler.v1beta1.Job.pubsub_target],
+               this field is ignored.
+        legacy_app_engine_cron (bool):
+            Immutable. This field is used to manage the
+            legacy App Engine Cron jobs using the Cloud
+            Scheduler API. If the field is set to true, the
+            job will be considered a legacy job. Note that
+            App Engine Cron jobs have fewer features than
+            Cloud Scheduler jobs, e.g., are only limited to
+            App Engine targets.
     """
 
     class State(proto.Enum):
-        r"""State of the job."""
+        r"""State of the job.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            ENABLED (1):
+                The job is executing normally.
+            PAUSED (2):
+                The job is paused by the user. It will not execute. A user
+                can intentionally pause the job using
+                [PauseJobRequest][google.cloud.scheduler.v1beta1.PauseJobRequest].
+            DISABLED (3):
+                The job is disabled by the system due to
+                error. The user cannot directly set a job to be
+                disabled.
+            UPDATE_FAILED (4):
+                The job state resulting from a failed
+                [CloudScheduler.UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob]
+                operation. To recover a job from this state, retry
+                [CloudScheduler.UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob]
+                until a successful response is received.
+        """
         STATE_UNSPECIFIED = 0
         ENABLED = 1
         PAUSED = 2
         DISABLED = 3
         UPDATE_FAILED = 4
 
     name: str = proto.Field(
@@ -232,29 +274,33 @@
         message="RetryConfig",
     )
     attempt_deadline: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=22,
         message=duration_pb2.Duration,
     )
+    legacy_app_engine_cron: bool = proto.Field(
+        proto.BOOL,
+        number=23,
+    )
 
 
 class RetryConfig(proto.Message):
     r"""Settings that determine the retry behavior.
 
     By default, if a job does not complete successfully (meaning that an
     acknowledgement is not received from the handler, then it will be
     retried with exponential backoff according to the settings in
-    [RetryConfig][google.cloud.scheduler.v1.RetryConfig].
+    [RetryConfig][google.cloud.scheduler.v1beta1.RetryConfig].
 
     Attributes:
         retry_count (int):
             The number of attempts that the system will make to run a
             job using the exponential backoff procedure described by
-            [max_doublings][google.cloud.scheduler.v1.RetryConfig.max_doublings].
+            [max_doublings][google.cloud.scheduler.v1beta1.RetryConfig.max_doublings].
 
             The default value of retry_count is zero.
 
             If retry_count is zero, a job attempt will *not* be retried
             if it fails. Instead the Cloud Scheduler system will wait
             for the next scheduled execution time.
 
@@ -263,15 +309,15 @@
             backoff, retry_count times, or until the next scheduled
             execution time, whichever comes first.
 
             Values greater than 5 and negative values are not allowed.
         max_retry_duration (google.protobuf.duration_pb2.Duration):
             The time limit for retrying a failed job, measured from time
             when an execution was first attempted. If specified with
-            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count],
+            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count],
             the job will be retried until both limits are reached.
 
             The default value for max_retry_duration is zero, which
             means retry duration is unlimited.
         min_backoff_duration (google.protobuf.duration_pb2.Duration):
             The minimum amount of time to wait before
             retrying a job after it fails.
@@ -283,33 +329,33 @@
 
             The default value of this field is 1 hour.
         max_doublings (int):
             The time between retries will double ``max_doublings``
             times.
 
             A job's retry interval starts at
-            [min_backoff_duration][google.cloud.scheduler.v1.RetryConfig.min_backoff_duration],
+            [min_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.min_backoff_duration],
             then doubles ``max_doublings`` times, then increases
-            linearly, and finally retries retries at intervals of
-            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
+            linearly, and finally retries at intervals of
+            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
             up to
-            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
             times.
 
             For example, if
-            [min_backoff_duration][google.cloud.scheduler.v1.RetryConfig.min_backoff_duration]
+            [min_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.min_backoff_duration]
             is 10s,
-            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
+            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
             is 300s, and ``max_doublings`` is 3, then the a job will
             first be retried in 10s. The retry interval will double
             three times, and then increase linearly by 2^3 \* 10s.
             Finally, the job will retry at intervals of
-            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
+            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
             until the job has been attempted
-            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
             times. Thus, the requests will retry at 10s, 20s, 40s, 80s,
             160s, 240s, 300s, 300s, ....
 
             The default value of this field is 5.
     """
 
     retry_count: int = proto.Field(
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1/types/target.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,34 @@
         "OAuthToken",
         "OidcToken",
     },
 )
 
 
 class HttpMethod(proto.Enum):
-    r"""The HTTP method used to execute the job."""
+    r"""The HTTP method used to execute the job.
+
+    Values:
+        HTTP_METHOD_UNSPECIFIED (0):
+            HTTP method unspecified. Defaults to POST.
+        POST (1):
+            HTTP POST
+        GET (2):
+            HTTP GET
+        HEAD (3):
+            HTTP HEAD
+        PUT (4):
+            HTTP PUT
+        DELETE (5):
+            HTTP DELETE
+        PATCH (6):
+            HTTP PATCH
+        OPTIONS (7):
+            HTTP OPTIONS
+    """
     HTTP_METHOD_UNSPECIFIED = 0
     POST = 1
     GET = 2
     HEAD = 3
     PUT = 4
     DELETE = 5
     PATCH = 6
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/gapic_metadata.json` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/gapic_version.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/async_client.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/client.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1356,15 +1356,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "CloudSchedulerClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/pagers.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/base.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc_asyncio.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/services/cloud_scheduler/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/__init__.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/cloudscheduler.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/job.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1/types/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,40 +16,40 @@
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.scheduler_v1beta1.types import target
+from google.cloud.scheduler_v1.types import target
 
 __protobuf__ = proto.module(
-    package="google.cloud.scheduler.v1beta1",
+    package="google.cloud.scheduler.v1",
     manifest={
         "Job",
         "RetryConfig",
     },
 )
 
 
 class Job(proto.Message):
     r"""Configuration for a job.
-    The maximum allowed size for a job is 1MB.
+    The maximum allowed size for a job is 100KB.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Optionally caller-specified in
-            [CreateJob][google.cloud.scheduler.v1beta1.CloudScheduler.CreateJob],
+            [CreateJob][google.cloud.scheduler.v1.CloudScheduler.CreateJob],
             after which it becomes output only.
 
             The job name. For example:
             ``projects/PROJECT_ID/locations/LOCATION_ID/jobs/JOB_ID``.
 
             -  ``PROJECT_ID`` can contain letters ([A-Za-z]), numbers
                ([0-9]), hyphens (-), colons (:), or periods (.). For
@@ -62,130 +62,130 @@
                For more information, see
                https://cloud.google.com/about/locations/.
             -  ``JOB_ID`` can contain only letters ([A-Za-z]), numbers
                ([0-9]), hyphens (-), or underscores (_). The maximum
                length is 500 characters.
         description (str):
             Optionally caller-specified in
-            [CreateJob][google.cloud.scheduler.v1beta1.CloudScheduler.CreateJob]
+            [CreateJob][google.cloud.scheduler.v1.CloudScheduler.CreateJob]
             or
-            [UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob].
+            [UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob].
 
             A human-readable description for the job. This string must
             not contain more than 500 characters.
-        pubsub_target (google.cloud.scheduler_v1beta1.types.PubsubTarget):
+        pubsub_target (google.cloud.scheduler_v1.types.PubsubTarget):
             Pub/Sub target.
 
             This field is a member of `oneof`_ ``target``.
-        app_engine_http_target (google.cloud.scheduler_v1beta1.types.AppEngineHttpTarget):
+        app_engine_http_target (google.cloud.scheduler_v1.types.AppEngineHttpTarget):
             App Engine HTTP target.
 
             This field is a member of `oneof`_ ``target``.
-        http_target (google.cloud.scheduler_v1beta1.types.HttpTarget):
+        http_target (google.cloud.scheduler_v1.types.HttpTarget):
             HTTP target.
 
             This field is a member of `oneof`_ ``target``.
         schedule (str):
             Required, except when used with
-            [UpdateJob][google.cloud.scheduler.v1beta1.CloudScheduler.UpdateJob].
+            [UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob].
 
             Describes the schedule on which the job will be executed.
 
             The schedule can be either of the following types:
 
-            -  `Crontab <https://en.wikipedia.org/wiki/Cron#Overview>`__
+            -  `Crontab <http://en.wikipedia.org/wiki/Cron#Overview>`__
             -  English-like
                `schedule <https://cloud.google.com/scheduler/docs/configuring/cron-job-schedules>`__
 
             As a general rule, execution ``n + 1`` of a job will not
             begin until execution ``n`` has finished. Cloud Scheduler
             will never allow two simultaneously outstanding executions.
             For example, this implies that if the ``n+1``\ th execution
             is scheduled to run at 16:00 but the ``n``\ th execution
             takes until 16:15, the ``n+1``\ th execution will not start
             until ``16:15``. A scheduled start time will be delayed if
             the previous execution has not ended when its scheduled time
             occurs.
 
             If
-            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
             > 0 and a job attempt fails, the job will be tried a total
             of
-            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
             times, with exponential backoff, until the next scheduled
             start time.
         time_zone (str):
             Specifies the time zone to be used in interpreting
-            [schedule][google.cloud.scheduler.v1beta1.Job.schedule]. The
+            [schedule][google.cloud.scheduler.v1.Job.schedule]. The
             value of this field must be a time zone name from the `tz
             database <http://en.wikipedia.org/wiki/Tz_database>`__.
 
             Note that some time zones include a provision for daylight
             savings time. The rules for daylight saving time are
             determined by the chosen tz. For UTC use the string "utc".
             If a time zone is not specified, the default will be in UTC
             (also known as GMT).
         user_update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The creation time of the job.
-        state (google.cloud.scheduler_v1beta1.types.Job.State):
+        state (google.cloud.scheduler_v1.types.Job.State):
             Output only. State of the job.
         status (google.rpc.status_pb2.Status):
             Output only. The response from the target for
             the last attempted execution.
         schedule_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The next time the job is
             scheduled. Note that this may be a retry of a
             previously failed attempt or the next execution
             time according to the schedule.
         last_attempt_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the last job attempt
             started.
-        retry_config (google.cloud.scheduler_v1beta1.types.RetryConfig):
+        retry_config (google.cloud.scheduler_v1.types.RetryConfig):
             Settings that determine the retry behavior.
         attempt_deadline (google.protobuf.duration_pb2.Duration):
             The deadline for job attempts. If the request handler does
             not respond by this deadline then the request is cancelled
             and the attempt is marked as a ``DEADLINE_EXCEEDED``
             failure. The failed attempt can be viewed in execution logs.
             Cloud Scheduler will retry the job according to the
-            [RetryConfig][google.cloud.scheduler.v1beta1.RetryConfig].
+            [RetryConfig][google.cloud.scheduler.v1.RetryConfig].
 
-            The default and the allowed values depend on the type of
-            target:
+            The allowed duration for this deadline is:
 
             -  For [HTTP
-               targets][google.cloud.scheduler.v1beta1.Job.http_target],
-               the default is 3 minutes. The deadline must be in the
-               interval [15 seconds, 30 minutes].
-
+               targets][google.cloud.scheduler.v1.Job.http_target],
+               between 15 seconds and 30 minutes.
             -  For [App Engine HTTP
-               targets][google.cloud.scheduler.v1beta1.Job.app_engine_http_target],
-               0 indicates that the request has the default deadline.
-               The default deadline depends on the scaling type of the
-               service: 10 minutes for standard apps with automatic
-               scaling, 24 hours for standard apps with manual and basic
-               scaling, and 60 minutes for flex apps. If the request
-               deadline is set, it must be in the interval [15 seconds,
-               24 hours 15 seconds].
-
-            -  For [Pub/Sub
-               targets][google.cloud.scheduler.v1beta1.Job.pubsub_target],
-               this field is ignored.
-        legacy_app_engine_cron (bool):
-            Immutable. This field is used to manage the
-            legacy App Engine Cron jobs using the Cloud
-            Scheduler API. If the field is set to true, the
-            job will be considered a legacy job. Note that
-            App Engine Cron jobs have fewer features than
-            Cloud Scheduler jobs, e.g., are only limited to
-            App Engine targets.
+               targets][google.cloud.scheduler.v1.Job.app_engine_http_target],
+               between 15 seconds and 24 hours.
     """
 
     class State(proto.Enum):
-        r"""State of the job."""
+        r"""State of the job.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                Unspecified state.
+            ENABLED (1):
+                The job is executing normally.
+            PAUSED (2):
+                The job is paused by the user. It will not execute. A user
+                can intentionally pause the job using
+                [PauseJobRequest][google.cloud.scheduler.v1.PauseJobRequest].
+            DISABLED (3):
+                The job is disabled by the system due to
+                error. The user cannot directly set a job to be
+                disabled.
+            UPDATE_FAILED (4):
+                The job state resulting from a failed
+                [CloudScheduler.UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob]
+                operation. To recover a job from this state, retry
+                [CloudScheduler.UpdateJob][google.cloud.scheduler.v1.CloudScheduler.UpdateJob]
+                until a successful response is received.
+        """
         STATE_UNSPECIFIED = 0
         ENABLED = 1
         PAUSED = 2
         DISABLED = 3
         UPDATE_FAILED = 4
 
     name: str = proto.Field(
@@ -253,33 +253,29 @@
         message="RetryConfig",
     )
     attempt_deadline: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=22,
         message=duration_pb2.Duration,
     )
-    legacy_app_engine_cron: bool = proto.Field(
-        proto.BOOL,
-        number=23,
-    )
 
 
 class RetryConfig(proto.Message):
     r"""Settings that determine the retry behavior.
 
     By default, if a job does not complete successfully (meaning that an
     acknowledgement is not received from the handler, then it will be
     retried with exponential backoff according to the settings in
-    [RetryConfig][google.cloud.scheduler.v1beta1.RetryConfig].
+    [RetryConfig][google.cloud.scheduler.v1.RetryConfig].
 
     Attributes:
         retry_count (int):
             The number of attempts that the system will make to run a
             job using the exponential backoff procedure described by
-            [max_doublings][google.cloud.scheduler.v1beta1.RetryConfig.max_doublings].
+            [max_doublings][google.cloud.scheduler.v1.RetryConfig.max_doublings].
 
             The default value of retry_count is zero.
 
             If retry_count is zero, a job attempt will *not* be retried
             if it fails. Instead the Cloud Scheduler system will wait
             for the next scheduled execution time.
 
@@ -288,15 +284,15 @@
             backoff, retry_count times, or until the next scheduled
             execution time, whichever comes first.
 
             Values greater than 5 and negative values are not allowed.
         max_retry_duration (google.protobuf.duration_pb2.Duration):
             The time limit for retrying a failed job, measured from time
             when an execution was first attempted. If specified with
-            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count],
+            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count],
             the job will be retried until both limits are reached.
 
             The default value for max_retry_duration is zero, which
             means retry duration is unlimited.
         min_backoff_duration (google.protobuf.duration_pb2.Duration):
             The minimum amount of time to wait before
             retrying a job after it fails.
@@ -308,33 +304,33 @@
 
             The default value of this field is 1 hour.
         max_doublings (int):
             The time between retries will double ``max_doublings``
             times.
 
             A job's retry interval starts at
-            [min_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.min_backoff_duration],
+            [min_backoff_duration][google.cloud.scheduler.v1.RetryConfig.min_backoff_duration],
             then doubles ``max_doublings`` times, then increases
-            linearly, and finally retries at intervals of
-            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
+            linearly, and finally retries retries at intervals of
+            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
             up to
-            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
             times.
 
             For example, if
-            [min_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.min_backoff_duration]
+            [min_backoff_duration][google.cloud.scheduler.v1.RetryConfig.min_backoff_duration]
             is 10s,
-            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
+            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
             is 300s, and ``max_doublings`` is 3, then the a job will
             first be retried in 10s. The retry interval will double
             three times, and then increase linearly by 2^3 \* 10s.
             Finally, the job will retry at intervals of
-            [max_backoff_duration][google.cloud.scheduler.v1beta1.RetryConfig.max_backoff_duration]
+            [max_backoff_duration][google.cloud.scheduler.v1.RetryConfig.max_backoff_duration]
             until the job has been attempted
-            [retry_count][google.cloud.scheduler.v1beta1.RetryConfig.retry_count]
+            [retry_count][google.cloud.scheduler.v1.RetryConfig.retry_count]
             times. Thus, the requests will retry at 10s, 20s, 40s, 80s,
             160s, 240s, 300s, 300s, ....
 
             The default value of this field is 5.
     """
 
     retry_count: int = proto.Field(
```

### Comparing `google-cloud-scheduler-2.9.0/google/cloud/scheduler_v1beta1/types/target.py` & `google-cloud-scheduler-2.9.1/google/cloud/scheduler_v1beta1/types/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,34 @@
         "OAuthToken",
         "OidcToken",
     },
 )
 
 
 class HttpMethod(proto.Enum):
-    r"""The HTTP method used to execute the job."""
+    r"""The HTTP method used to execute the job.
+
+    Values:
+        HTTP_METHOD_UNSPECIFIED (0):
+            HTTP method unspecified. Defaults to POST.
+        POST (1):
+            HTTP POST
+        GET (2):
+            HTTP GET
+        HEAD (3):
+            HTTP HEAD
+        PUT (4):
+            HTTP PUT
+        DELETE (5):
+            HTTP DELETE
+        PATCH (6):
+            HTTP PATCH
+        OPTIONS (7):
+            HTTP OPTIONS
+    """
     HTTP_METHOD_UNSPECIFIED = 0
     POST = 1
     GET = 2
     HEAD = 3
     PUT = 4
     DELETE = 5
     PATCH = 6
```

### Comparing `google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/PKG-INFO` & `google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-scheduler
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Scheduler API client library
 Home-page: https://github.com/googleapis/python-scheduler
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-scheduler-2.9.0/google_cloud_scheduler.egg-info/SOURCES.txt` & `google-cloud-scheduler-2.9.1/google_cloud_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/setup.py` & `google-cloud-scheduler-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/__init__.py` & `google-cloud-scheduler-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/system.py` & `google-cloud-scheduler-2.9.1/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/__init__.py` & `google-cloud-scheduler-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-scheduler-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1/__init__.py` & `google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1/test_cloud_scheduler.py` & `google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1/test_cloud_scheduler.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1beta1/__init__.py` & `google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-scheduler-2.9.0/tests/unit/gapic/scheduler_v1beta1/test_cloud_scheduler.py` & `google-cloud-scheduler-2.9.1/tests/unit/gapic/scheduler_v1beta1/test_cloud_scheduler.py`

 * *Files identical despite different names*

