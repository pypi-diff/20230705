# Comparing `tmp/google-cloud-error-reporting-1.9.1.tar.gz` & `tmp/google-cloud-error-reporting-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-error-reporting-1.9.1.tar", last modified: Mon Mar 27 16:05:18 2023, max compression
+gzip compressed data, was "google-cloud-error-reporting-1.9.2.tar", last modified: Wed Jul  5 15:47:19 2023, max compression
```

## Comparing `google-cloud-error-reporting-1.9.1.tar` & `google-cloud-error-reporting-1.9.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4977 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4037 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.133415 google-cloud-error-reporting-1.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.133415 google-cloud-error-reporting-1.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/
--rw-rw-r--   0 root         (0)     1003      992 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/__init__.py
--rw-rw-r--   0 root         (0)     1003     2724 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/_gapic.py
--rw-rw-r--   0 root         (0)     1003     3697 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/_logging.py
--rw-rw-r--   0 root         (0)     1003    15137 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/client.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/gapic_version.py
--rw-rw-r--   0 root         (0)     1003     1716 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/util.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/
--rw-rw-r--   0 root         (0)     1003     3298 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3694 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    18022 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27150 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/
--rw-rw-r--   0 root         (0)     1003     1460 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6507 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12975 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13219 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17291 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.137415 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25344 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    34628 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/client.py
--rw-rw-r--   0 root         (0)     1003    11197 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.141416 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/
--rw-rw-r--   0 root         (0)     1003     1460 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7132 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14290 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14551 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22579 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.141416 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15182 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23750 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.141416 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/
--rw-rw-r--   0 root         (0)     1003     1496 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6168 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12571 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12781 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12873 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.141416 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1932 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11034 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003     2021 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/error_group_service.py
--rw-rw-r--   0 root         (0)     1003    20438 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/error_stats_service.py
--rw-rw-r--   0 root         (0)     1003     5065 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/report_errors_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/
--rw-r--r--   0 root         (0)     1003     4977 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3843 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      354 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:05:18.000000 google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3059 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.133415 google-cloud-error-reporting-1.9.1/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/system/gapic/v1beta1/
--rw-rw-r--   0 root         (0)     1003     1610 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/system/gapic/v1beta1/test_system_report_errors_service_v1beta1.py
--rw-rw-r--   0 root         (0)     1003     4354 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/system/test_system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:05:18.145417 google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    91348 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_error_group_service.py
--rw-rw-r--   0 root         (0)     1003   131082 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_error_stats_service.py
--rw-rw-r--   0 root         (0)     1003    76270 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_report_errors_service.py
--rw-rw-r--   0 root         (0)     1003     2867 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/test__gapic.py
--rw-rw-r--   0 root         (0)     1003     2812 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/test__logging.py
--rw-rw-r--   0 root         (0)     1003     8161 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003     1672 2023-03-27 16:03:22.000000 google-cloud-error-reporting-1.9.1/tests/unit/test_util.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4977 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4037 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.966860 google-cloud-error-reporting-1.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.966860 google-cloud-error-reporting-1.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.970859 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/
+-rw-rw-r--   0 root         (0)     1003      992 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2724 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/_gapic.py
+-rw-rw-r--   0 root         (0)     1003     3697 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/_logging.py
+-rw-rw-r--   0 root         (0)     1003    15137 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/client.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003     1716 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/util.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     3298 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3694 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18056 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27150 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1460 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6507 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12975 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13219 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17291 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25378 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    34628 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11197 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.974858 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1460 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7132 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14290 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14551 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22579 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15218 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23750 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1496 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6168 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12571 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12781 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12873 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1932 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11034 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     2021 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/error_group_service.py
+-rw-rw-r--   0 root         (0)     1003    20438 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/error_stats_service.py
+-rw-rw-r--   0 root         (0)     1003     5065 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/report_errors_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/
+-rw-r--r--   0 root         (0)     1003     4977 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3843 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      354 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:47:19.000000 google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3059 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.970859 google-cloud-error-reporting-1.9.2/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.978857 google-cloud-error-reporting-1.9.2/tests/system/gapic/v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1610 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/system/gapic/v1beta1/test_system_report_errors_service_v1beta1.py
+-rw-rw-r--   0 root         (0)     1003     4354 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/system/test_system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:19.982856 google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91348 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_error_group_service.py
+-rw-rw-r--   0 root         (0)     1003   131480 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_error_stats_service.py
+-rw-rw-r--   0 root         (0)     1003    76270 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_report_errors_service.py
+-rw-rw-r--   0 root         (0)     1003     2867 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/test__gapic.py
+-rw-rw-r--   0 root         (0)     1003     2812 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/test__logging.py
+-rw-rw-r--   0 root         (0)     1003     8161 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003     1672 2023-07-05 15:45:11.000000 google-cloud-error-reporting-1.9.2/tests/unit/test_util.py
```

### Comparing `google-cloud-error-reporting-1.9.1/LICENSE` & `google-cloud-error-reporting-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/MANIFEST.in` & `google-cloud-error-reporting-1.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/PKG-INFO` & `google-cloud-error-reporting-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-error-reporting
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Error Reporting API client library
 Home-page: https://github.com/googleapis/python-error-reporting
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-error-reporting-1.9.1/README.rst` & `google-cloud-error-reporting-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/_gapic.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/_gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/_logging.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/_logging.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/gapic_version.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/error_reporting/util.py` & `google-cloud-error-reporting-1.9.2/google/cloud/error_reporting/util.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/gapic_metadata.json` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/gapic_version.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.1"  # {x-release-please-version}
+__version__ = "1.9.2"  # {x-release-please-version}
```

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/async_client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ErrorGroupServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/base.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc_asyncio.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/rest.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_group_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/async_client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -593,15 +593,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ErrorStatsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/pagers.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/base.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc_asyncio.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/rest.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/error_stats_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/async_client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ReportErrorsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/client.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/base.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc_asyncio.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/rest.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/services/report_errors_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/__init__.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/common.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/error_group_service.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/error_group_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/error_stats_service.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/error_stats_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google/cloud/errorreporting_v1beta1/types/report_errors_service.py` & `google-cloud-error-reporting-1.9.2/google/cloud/errorreporting_v1beta1/types/report_errors_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/PKG-INFO` & `google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-error-reporting
-Version: 1.9.1
+Version: 1.9.2
 Summary: Google Cloud Error Reporting API client library
 Home-page: https://github.com/googleapis/python-error-reporting
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-error-reporting-1.9.1/google_cloud_error_reporting.egg-info/SOURCES.txt` & `google-cloud-error-reporting-1.9.2/google_cloud_error_reporting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/setup.py` & `google-cloud-error-reporting-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/__init__.py` & `google-cloud-error-reporting-1.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/system/gapic/v1beta1/test_system_report_errors_service_v1beta1.py` & `google-cloud-error-reporting-1.9.2/tests/system/gapic/v1beta1/test_system_report_errors_service_v1beta1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/system/test_system.py` & `google-cloud-error-reporting-1.9.2/tests/system/test_system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/__init__.py` & `google-cloud-error-reporting-1.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/gapic/__init__.py` & `google-cloud-error-reporting-1.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/__init__.py` & `google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_error_group_service.py` & `google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_error_group_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_error_stats_service.py` & `google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_error_stats_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1174,17 +1174,19 @@
                     error_stats_service.ErrorGroupStats(),
                     error_stats_service.ErrorGroupStats(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_group_stats(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1604,17 +1606,19 @@
                     common.ErrorEvent(),
                     common.ErrorEvent(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_events(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/gapic/errorreporting_v1beta1/test_report_errors_service.py` & `google-cloud-error-reporting-1.9.2/tests/unit/gapic/errorreporting_v1beta1/test_report_errors_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/test__gapic.py` & `google-cloud-error-reporting-1.9.2/tests/unit/test__gapic.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/test__logging.py` & `google-cloud-error-reporting-1.9.2/tests/unit/test__logging.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/test_client.py` & `google-cloud-error-reporting-1.9.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-error-reporting-1.9.1/tests/unit/test_util.py` & `google-cloud-error-reporting-1.9.2/tests/unit/test_util.py`

 * *Files identical despite different names*

