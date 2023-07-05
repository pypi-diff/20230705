# Comparing `tmp/google-cloud-service-control-1.9.0.tar.gz` & `tmp/google-cloud-service-control-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-control-1.9.0.tar", last modified: Wed May 31 20:49:11 2023, max compression
+gzip compressed data, was "google-cloud-service-control-1.9.1.tar", last modified: Wed Jul  5 15:55:39 2023, max compression
```

## Comparing `google-cloud-service-control-1.9.0.tar` & `google-cloud-service-control-1.9.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4856 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3916 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.300694 google-cloud-service-control-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.300694 google-cloud-service-control-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/
--rw-rw-r--   0 root         (0)     1003     2516 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/
--rw-rw-r--   0 root         (0)     1003     1988 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2087 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/
--rw-rw-r--   0 root         (0)     1003      773 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    13162 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    21749 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6171 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12601 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12816 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12263 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.304695 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    17616 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    26029 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6933 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14785 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15029 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16877 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/
--rw-rw-r--   0 root         (0)     1003     1492 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6098 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/check_error.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/distribution.py
--rw-rw-r--   0 root         (0)     1003     4981 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/http_request.py
--rw-rw-r--   0 root         (0)     1003     8087 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/log_entry.py
--rw-rw-r--   0 root         (0)     1003     5091 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/metric_value.py
--rw-rw-r--   0 root         (0)     1003     7164 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/operation.py
--rw-rw-r--   0 root         (0)     1003    12336 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/quota_controller.py
--rw-rw-r--   0 root         (0)     1003    11573 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/
--rw-rw-r--   0 root         (0)     1003     1197 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1316 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.308696 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    18278 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    26691 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6933 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15302 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15546 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17091 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/
--rw-rw-r--   0 root         (0)     1003      895 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7316 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/
--rw-r--r--   0 root         (0)     1003     4856 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3777 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:11.000000 google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:11.316697 google-cloud-service-control-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2958 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    63977 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py
--rw-rw-r--   0 root         (0)     1003    74966 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_service_controller.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:11.312697 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    72840 2023-05-31 20:46:40.000000 google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/test_service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.810124 google-cloud-service-control-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:55:39.810124 google-cloud-service-control-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3880 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.794125 google-cloud-service-control-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.794125 google-cloud-service-control-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.798124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol/
+-rw-rw-r--   0 root         (0)     1003     2516 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.798124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/
+-rw-rw-r--   0 root         (0)     1003     1988 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2087 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.798124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.798124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13194 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21749 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6171 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12601 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12816 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12263 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17650 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26029 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6933 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14785 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15029 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16877 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1492 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6098 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/check_error.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/distribution.py
+-rw-rw-r--   0 root         (0)     1003     4981 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/http_request.py
+-rw-rw-r--   0 root         (0)     1003     8087 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/log_entry.py
+-rw-rw-r--   0 root         (0)     1003     5091 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/metric_value.py
+-rw-rw-r--   0 root         (0)     1003     7164 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/operation.py
+-rw-rw-r--   0 root         (0)     1003    12336 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/quota_controller.py
+-rw-rw-r--   0 root         (0)     1003    11573 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/
+-rw-rw-r--   0 root         (0)     1003     1197 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.802124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18312 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26691 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6933 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15302 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15546 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17091 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/types/
+-rw-rw-r--   0 root         (0)     1003      895 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7316 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/types/service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     4817 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3777 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:55:39.000000 google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:55:39.810124 google-cloud-service-control-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2955 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.806124 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    63977 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py
+-rw-rw-r--   0 root         (0)     1003    74966 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/test_service_controller.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:55:39.810124 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    72840 2023-07-05 15:46:59.000000 google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v2/test_service_controller.py
```

### Comparing `google-cloud-service-control-1.9.0/LICENSE` & `google-cloud-service-control-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/MANIFEST.in` & `google-cloud-service-control-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/PKG-INFO` & `google-cloud-service-control-1.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-control
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Service Control API client library
-Home-page: https://github.com/googleapis/python-service-control
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Service Control API
-=====================================
+Python Client for Service Control
+=================================
 
 |stable| |pypi| |versions|
 
-`Service Control API`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
+`Service Control`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
-.. _Service Control API: https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control: https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicecontrol/latest
 .. _Product Documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Control API.`_
+3. `Enable the Service Control.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Control API.:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Enable the Service Control.:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Control API
+-  Read the `Client Library Documentation`_ for Service Control
    to see other available methods on the client.
--  Read the `Service Control API Product documentation`_ to learn
+-  Read the `Service Control Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Control API Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-control-1.9.0/README.rst` & `google-cloud-service-control-1.9.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Service Control API
-=====================================
+Python Client for Service Control
+=================================
 
 |stable| |pypi| |versions|
 
-`Service Control API`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
+`Service Control`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
-.. _Service Control API: https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control: https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicecontrol/latest
 .. _Product Documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Control API.`_
+3. `Enable the Service Control.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Control API.:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Enable the Service Control.:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Control API
+-  Read the `Client Library Documentation`_ for Service Control
    to see other available methods on the client.
--  Read the `Service Control API Product documentation`_ to learn
+-  Read the `Service Control Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Control API Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol/gapic_version.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_metadata.json` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/gapic_version.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "QuotaControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/quota_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/async_client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ServiceControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/services/service_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/check_error.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/check_error.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/distribution.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/distribution.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/http_request.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/http_request.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/log_entry.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/log_entry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/metric_value.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/metric_value.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/operation.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/operation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/quota_controller.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/quota_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v1/types/service_controller.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v1/types/service_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_metadata.json` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/gapic_version.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/gapic_version.py`

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
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/async_client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,15 +431,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ServiceControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/client.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/services/service_controller/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/__init__.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google/cloud/servicecontrol_v2/types/service_controller.py` & `google-cloud-service-control-1.9.1/google/cloud/servicecontrol_v2/types/service_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/PKG-INFO` & `google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-control
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Service Control API client library
-Home-page: https://github.com/googleapis/python-service-control
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Service Control API
-=====================================
+Python Client for Service Control
+=================================
 
 |stable| |pypi| |versions|
 
-`Service Control API`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
+`Service Control`_:  is a foundational platform for creating, managing, securing, and consuming APIs and services across organizations. It is used by Google APIs, Cloud APIs, Cloud Endpoints, and API Gateway.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-service-control.svg
    :target: https://pypi.org/project/google-cloud-service-control/
-.. _Service Control API: https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control: https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/servicecontrol/latest
 .. _Product Documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Service Control API.`_
+3. `Enable the Service Control.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Service Control API.:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Enable the Service Control.:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-service-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Service Control API
+-  Read the `Client Library Documentation`_ for Service Control
    to see other available methods on the client.
--  Read the `Service Control API Product documentation`_ to learn
+-  Read the `Service Control Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Service Control API Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
+.. _Service Control Product documentation:  https://cloud.google.com/service-infrastructure/docs/overview/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-service-control-1.9.0/google_cloud_service_control.egg-info/SOURCES.txt` & `google-cloud-service-control-1.9.1/google_cloud_service_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/setup.py` & `google-cloud-service-control-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-service-control"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-service-control-1.9.0/tests/__init__.py` & `google-cloud-service-control-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/__init__.py` & `google-cloud-service-control-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/__init__.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/test_quota_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v1/test_service_controller.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v1/test_service_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/__init__.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-control-1.9.0/tests/unit/gapic/servicecontrol_v2/test_service_controller.py` & `google-cloud-service-control-1.9.1/tests/unit/gapic/servicecontrol_v2/test_service_controller.py`

 * *Files identical despite different names*

