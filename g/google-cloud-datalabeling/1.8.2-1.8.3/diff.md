# Comparing `tmp/google-cloud-datalabeling-1.8.2.tar.gz` & `tmp/google-cloud-datalabeling-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datalabeling-1.8.2.tar", last modified: Mon Mar 27 15:58:09 2023, max compression
+gzip compressed data, was "google-cloud-datalabeling-1.8.3.tar", last modified: Wed Jul  5 15:52:07 2023, max compression
```

## Comparing `google-cloud-datalabeling-1.8.2.tar` & `google-cloud-datalabeling-1.8.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.237980 google-cloud-datalabeling-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4838 2023-03-27 15:58:09.237980 google-cloud-datalabeling-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3907 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.225971 google-cloud-datalabeling-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.225971 google-cloud-datalabeling-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.225971 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/
--rw-rw-r--   0 root         (0)     1003     9419 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.229974 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/
--rw-rw-r--   0 root         (0)     1003     8912 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9306 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.229974 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.229974 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   184349 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   195409 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/client.py
--rw-rw-r--   0 root         (0)     1003    48808 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.229974 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    31057 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    54230 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    55484 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.233977 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     8542 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    25652 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/annotation.py
--rw-rw-r--   0 root         (0)     1003     3627 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/annotation_spec_set.py
--rw-rw-r--   0 root         (0)     1003    47418 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/data_labeling_service.py
--rw-rw-r--   0 root         (0)     1003     3675 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/data_payloads.py
--rw-rw-r--   0 root         (0)     1003    25783 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/dataset.py
--rw-rw-r--   0 root         (0)     1003    14432 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/evaluation.py
--rw-rw-r--   0 root         (0)     1003    19714 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/evaluation_job.py
--rw-rw-r--   0 root         (0)     1003    12746 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/human_annotation_config.py
--rw-rw-r--   0 root         (0)     1003     4627 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/instruction.py
--rw-rw-r--   0 root         (0)     1003    20469 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/operations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.233977 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/
--rw-r--r--   0 root         (0)     1003     4838 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2238 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:58:09.000000 google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:58:09.237980 google-cloud-datalabeling-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2947 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.233977 google-cloud-datalabeling-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.233977 google-cloud-datalabeling-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.237980 google-cloud-datalabeling-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:09.237980 google-cloud-datalabeling-1.8.2/tests/unit/gapic/datalabeling_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/tests/unit/gapic/datalabeling_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   429972 2023-03-27 15:55:50.000000 google-cloud-datalabeling-1.8.2/tests/unit/gapic/datalabeling_v1beta1/test_data_labeling_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.697077 google-cloud-datalabeling-1.8.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4802 2023-07-05 15:52:07.697077 google-cloud-datalabeling-1.8.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3871 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.685076 google-cloud-datalabeling-1.8.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.685076 google-cloud-datalabeling-1.8.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.685076 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/
+-rw-rw-r--   0 root         (0)     1003     9419 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.689077 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     8912 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9306 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.689077 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.689077 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   184385 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   195409 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/client.py
+-rw-rw-r--   0 root         (0)     1003    48808 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.689077 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31057 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    54230 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    55484 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     8542 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25652 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/annotation.py
+-rw-rw-r--   0 root         (0)     1003     3627 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/annotation_spec_set.py
+-rw-rw-r--   0 root         (0)     1003    47418 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/data_labeling_service.py
+-rw-rw-r--   0 root         (0)     1003     3675 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/data_payloads.py
+-rw-rw-r--   0 root         (0)     1003    25783 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003    14432 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/evaluation.py
+-rw-rw-r--   0 root         (0)     1003    19714 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/evaluation_job.py
+-rw-rw-r--   0 root         (0)     1003    12746 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/human_annotation_config.py
+-rw-rw-r--   0 root         (0)     1003     4627 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/instruction.py
+-rw-rw-r--   0 root         (0)     1003    20469 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/operations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/
+-rw-r--r--   0 root         (0)     1003     4802 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2238 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:07.000000 google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:52:07.697077 google-cloud-datalabeling-1.8.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2947 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:07.693076 google-cloud-datalabeling-1.8.3/tests/unit/gapic/datalabeling_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/tests/unit/gapic/datalabeling_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   431597 2023-07-05 15:46:58.000000 google-cloud-datalabeling-1.8.3/tests/unit/gapic/datalabeling_v1beta1/test_data_labeling_service.py
```

### Comparing `google-cloud-datalabeling-1.8.2/LICENSE` & `google-cloud-datalabeling-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/MANIFEST.in` & `google-cloud-datalabeling-1.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/PKG-INFO` & `google-cloud-datalabeling-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-datalabeling
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Datalabeling API client library
-Home-page: https://github.com/googleapis/python-datalabeling
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
 
-Python Client for Google Cloud Data Labeling API
-================================================
+Python Client for Google Cloud Data Labeling
+============================================
 
 |preview| |pypi| |versions|
 
-`Google Cloud Data Labeling API`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
+`Google Cloud Data Labeling`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
-.. _Google Cloud Data Labeling API: https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling: https://cloud.google.com/data-labeling/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datalabeling/latest
 .. _Product Documentation:  https://cloud.google.com/data-labeling/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Google Cloud Data Labeling API.`_
+3. `Enable the Google Cloud Data Labeling.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Google Cloud Data Labeling API.:  https://cloud.google.com/data-labeling/docs/
+.. _Enable the Google Cloud Data Labeling.:  https://cloud.google.com/data-labeling/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datalabeling
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Google Cloud Data Labeling API
+-  Read the `Client Library Documentation`_ for Google Cloud Data Labeling
    to see other available methods on the client.
--  Read the `Google Cloud Data Labeling API Product documentation`_ to learn
+-  Read the `Google Cloud Data Labeling Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Google Cloud Data Labeling API Product documentation:  https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling Product documentation:  https://cloud.google.com/data-labeling/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datalabeling-1.8.2/README.rst` & `google-cloud-datalabeling-1.8.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Google Cloud Data Labeling API
-================================================
+Python Client for Google Cloud Data Labeling
+============================================
 
 |preview| |pypi| |versions|
 
-`Google Cloud Data Labeling API`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
+`Google Cloud Data Labeling`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
-.. _Google Cloud Data Labeling API: https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling: https://cloud.google.com/data-labeling/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datalabeling/latest
 .. _Product Documentation:  https://cloud.google.com/data-labeling/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Google Cloud Data Labeling API.`_
+3. `Enable the Google Cloud Data Labeling.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Google Cloud Data Labeling API.:  https://cloud.google.com/data-labeling/docs/
+.. _Enable the Google Cloud Data Labeling.:  https://cloud.google.com/data-labeling/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datalabeling
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Google Cloud Data Labeling API
+-  Read the `Client Library Documentation`_ for Google Cloud Data Labeling
    to see other available methods on the client.
--  Read the `Google Cloud Data Labeling API Product documentation`_ to learn
+-  Read the `Google Cloud Data Labeling Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Google Cloud Data Labeling API Product documentation:  https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling Product documentation:  https://cloud.google.com/data-labeling/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling/gapic_version.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling/gapic_version.py`

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
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/gapic_metadata.json` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/gapic_version.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/gapic_version.py`

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
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/async_client.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4471,15 +4471,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "DataLabelingServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/client.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/pagers.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/base.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc_asyncio.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/services/data_labeling_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/__init__.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/annotation.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/annotation_spec_set.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/annotation_spec_set.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/data_labeling_service.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/data_labeling_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/data_payloads.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/data_payloads.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/dataset.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/dataset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/evaluation.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/evaluation_job.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/evaluation_job.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/human_annotation_config.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/human_annotation_config.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/instruction.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/instruction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google/cloud/datalabeling_v1beta1/types/operations.py` & `google-cloud-datalabeling-1.8.3/google/cloud/datalabeling_v1beta1/types/operations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/PKG-INFO` & `google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-datalabeling
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Datalabeling API client library
-Home-page: https://github.com/googleapis/python-datalabeling
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
 
-Python Client for Google Cloud Data Labeling API
-================================================
+Python Client for Google Cloud Data Labeling
+============================================
 
 |preview| |pypi| |versions|
 
-`Google Cloud Data Labeling API`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
+`Google Cloud Data Labeling`_: is a service that lets you work with human labelers to generate highly accurate labels for a collection of data that you can use to train your machine learning models.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-datalabeling.svg
    :target: https://pypi.org/project/google-cloud-datalabeling/
-.. _Google Cloud Data Labeling API: https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling: https://cloud.google.com/data-labeling/docs/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/datalabeling/latest
 .. _Product Documentation:  https://cloud.google.com/data-labeling/docs/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Google Cloud Data Labeling API.`_
+3. `Enable the Google Cloud Data Labeling.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Google Cloud Data Labeling API.:  https://cloud.google.com/data-labeling/docs/
+.. _Enable the Google Cloud Data Labeling.:  https://cloud.google.com/data-labeling/docs/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-datalabeling
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Google Cloud Data Labeling API
+-  Read the `Client Library Documentation`_ for Google Cloud Data Labeling
    to see other available methods on the client.
--  Read the `Google Cloud Data Labeling API Product documentation`_ to learn
+-  Read the `Google Cloud Data Labeling Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Google Cloud Data Labeling API Product documentation:  https://cloud.google.com/data-labeling/docs/
+.. _Google Cloud Data Labeling Product documentation:  https://cloud.google.com/data-labeling/docs/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-datalabeling-1.8.2/google_cloud_datalabeling.egg-info/SOURCES.txt` & `google-cloud-datalabeling-1.8.3/google_cloud_datalabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/setup.py` & `google-cloud-datalabeling-1.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-datalabeling"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-datalabeling-1.8.2/tests/__init__.py` & `google-cloud-datalabeling-1.8.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/tests/unit/__init__.py` & `google-cloud-datalabeling-1.8.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/tests/unit/gapic/__init__.py` & `google-cloud-datalabeling-1.8.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/tests/unit/gapic/datalabeling_v1beta1/__init__.py` & `google-cloud-datalabeling-1.8.3/tests/unit/gapic/datalabeling_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datalabeling-1.8.2/tests/unit/gapic/datalabeling_v1beta1/test_data_labeling_service.py` & `google-cloud-datalabeling-1.8.3/tests/unit/gapic/datalabeling_v1beta1/test_data_labeling_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1651,17 +1651,19 @@
                     dataset.Dataset(),
                     dataset.Dataset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_datasets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2420,15 +2422,14 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_data_item), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = dataset.DataItem(
             name="name_value",
-            image_payload=data_payloads.ImagePayload(mime_type="mime_type_value"),
         )
         response = client.get_data_item(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == data_labeling_service.GetDataItemRequest()
@@ -3051,17 +3052,19 @@
                     dataset.DataItem(),
                     dataset.DataItem(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_data_items(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3785,17 +3788,19 @@
                     dataset.AnnotatedDataset(),
                     dataset.AnnotatedDataset(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_annotated_datasets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -4742,15 +4747,14 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_example), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = dataset.Example(
             name="name_value",
-            image_payload=data_payloads.ImagePayload(mime_type="mime_type_value"),
         )
         response = client.get_example(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == data_labeling_service.GetExampleRequest()
@@ -5383,17 +5387,19 @@
                     dataset.Example(),
                     dataset.Example(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_examples(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -6376,17 +6382,19 @@
                     annotation_spec_set.AnnotationSpecSet(),
                     annotation_spec_set.AnnotationSpecSet(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_annotation_spec_sets(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -7564,17 +7572,19 @@
                     instruction.Instruction(),
                     instruction.Instruction(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_instructions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8499,17 +8509,19 @@
                     evaluation.Evaluation(),
                     evaluation.Evaluation(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_evaluations(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -8954,17 +8966,19 @@
                     data_labeling_service.SearchExampleComparisonsResponse.ExampleComparison(),
                     data_labeling_service.SearchExampleComparisonsResponse.ExampleComparison(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_example_comparisons(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -10945,17 +10959,19 @@
                     evaluation_job.EvaluationJob(),
                     evaluation_job.EvaluationJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_evaluation_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
```

