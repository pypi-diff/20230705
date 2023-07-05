# Comparing `tmp/google-cloud-data-qna-0.8.2.tar.gz` & `tmp/google-cloud-data-qna-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-data-qna-0.8.2.tar", last modified: Mon Oct 10 18:06:03 2022, max compression
+gzip compressed data, was "google-cloud-data-qna-0.9.0.tar", last modified: Thu Dec 15 22:57:12 2022, max compression
```

## Comparing `google-cloud-data-qna-0.8.2.tar` & `google-cloud-data-qna-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4359 2022-10-10 18:06:03.696539 google-cloud-data-qna-0.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3634 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.684543 google-cloud-data-qna-0.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.684543 google-cloud-data-qna-0.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna/
--rw-rw-r--   0 root         (0)     1003     2540 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna/__init__.py
--rw-rw-r--   0 root         (0)     1003       81 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/
--rw-rw-r--   0 root         (0)     1003     2142 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     3355 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       81 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/
--rw-rw-r--   0 root         (0)     1003      797 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14569 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    23145 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6256 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13835 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14060 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    14848 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.688542 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/
--rw-rw-r--   0 root         (0)     1003      773 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    33231 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    43751 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8194 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17282 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17626 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    34372 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     1763 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3288 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/annotated_string.py
--rw-rw-r--   0 root         (0)     1003     6234 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/auto_suggestion_service.py
--rw-rw-r--   0 root         (0)     1003    19063 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/question.py
--rw-rw-r--   0 root         (0)     1003     4067 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/question_service.py
--rw-rw-r--   0 root         (0)     1003     1780 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/user_feedback.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/
--rw-r--r--   0 root         (0)     1003     4359 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2394 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 18:06:03.000000 google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 18:06:03.696539 google-cloud-data-qna-0.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2223 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 18:06:03.692540 google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    67540 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/test_auto_suggestion_service.py
--rw-rw-r--   0 root         (0)     1003   160390 2022-10-10 18:02:41.000000 google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/test_question_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4489 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3634 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.847934 google-cloud-data-qna-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.847934 google-cloud-data-qna-0.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna/
+-rw-rw-r--   0 root         (0)     1003     2650 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     2252 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3355 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/
+-rw-rw-r--   0 root         (0)     1003      797 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14614 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    23300 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6140 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13935 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14147 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    14942 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.851935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/
+-rw-rw-r--   0 root         (0)     1003      773 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33572 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44162 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.855935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8078 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17382 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17713 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    34682 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.855935 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     1763 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3438 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/annotated_string.py
+-rw-rw-r--   0 root         (0)     1003     6527 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/auto_suggestion_service.py
+-rw-rw-r--   0 root         (0)     1003    20094 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/question.py
+-rw-rw-r--   0 root         (0)     1003     4251 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/question_service.py
+-rw-rw-r--   0 root         (0)     1003     1862 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/user_feedback.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.855935 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/
+-rw-r--r--   0 root         (0)     1003     4489 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2478 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 22:57:12.000000 google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2864 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:57:12.859936 google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67540 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/test_auto_suggestion_service.py
+-rw-rw-r--   0 root         (0)     1003   160390 2022-12-15 22:53:45.000000 google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/test_question_service.py
```

### Comparing `google-cloud-data-qna-0.8.2/LICENSE` & `google-cloud-data-qna-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/MANIFEST.in` & `google-cloud-data-qna-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/PKG-INFO` & `google-cloud-data-qna-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-data-qna
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Cloud Data Qna API client library
 Home-page: https://github.com/googleapis/python-data-qna
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Data QnA API
 ==============================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-data-qna-0.8.2/README.rst` & `google-cloud-data-qna-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.dataqna import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.dataqna_v1alpha.services.auto_suggestion_service.async_client import (
     AutoSuggestionServiceAsyncClient,
 )
 from google.cloud.dataqna_v1alpha.services.auto_suggestion_service.client import (
     AutoSuggestionServiceClient,
 )
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.dataqna import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.auto_suggestion_service import (
     AutoSuggestionServiceAsyncClient,
     AutoSuggestionServiceClient,
 )
 from .services.question_service import QuestionServiceAsyncClient, QuestionServiceClient
 from .types.annotated_string import AnnotatedString
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/gapic_metadata.json` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/async_client.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import auto_suggestion_service
@@ -226,17 +237,17 @@
         type(AutoSuggestionServiceClient).get_transport_class,
         type(AutoSuggestionServiceClient),
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, AutoSuggestionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto suggestion service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -272,18 +283,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def suggest_queries(
         self,
-        request: Union[auto_suggestion_service.SuggestQueriesRequest, dict] = None,
+        request: Optional[
+            Union[auto_suggestion_service.SuggestQueriesRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> auto_suggestion_service.SuggestQueriesResponse:
         r"""Gets a list of suggestions based on a prefix string.
         AutoSuggestion tolerance should be less than 1 second.
 
         .. code-block:: python
 
@@ -308,15 +321,15 @@
                 # Make the request
                 response = await client.suggest_queries(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.SuggestQueriesRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.SuggestQueriesRequest, dict]]):
                 The request object. Request for query suggestions.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -355,18 +368,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoSuggestionServiceAsyncClient",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/client.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import auto_suggestion_service
@@ -55,15 +67,15 @@
     )  # type: Dict[str, Type[AutoSuggestionServiceTransport]]
     _transport_registry["grpc"] = AutoSuggestionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = AutoSuggestionServiceGrpcAsyncIOTransport
     _transport_registry["rest"] = AutoSuggestionServiceRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[AutoSuggestionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -379,16 +391,16 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, AutoSuggestionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, AutoSuggestionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto suggestion service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -397,15 +409,15 @@
                 credentials from the environment.
             transport (Union[str, AutoSuggestionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
                 NOTE: "rest" transport functionality is currently in a
                 beta state (preview). We welcome your feedback via an
                 issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -427,14 +439,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -479,18 +492,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def suggest_queries(
         self,
-        request: Union[auto_suggestion_service.SuggestQueriesRequest, dict] = None,
+        request: Optional[
+            Union[auto_suggestion_service.SuggestQueriesRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> auto_suggestion_service.SuggestQueriesResponse:
         r"""Gets a list of suggestions based on a prefix string.
         AutoSuggestion tolerance should be less than 1 second.
 
         .. code-block:: python
 
@@ -570,18 +585,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoSuggestionServiceClient",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/base.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,40 +19,35 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 from google.cloud.dataqna_v1alpha.types import auto_suggestion_service
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class AutoSuggestionServiceTransport(abc.ABC):
     """Abstract transport class for AutoSuggestionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "dataqna.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc_asyncio.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers
-import google.auth  # type: ignore
+from google.api_core import gapic_v1, grpc_helpers_async
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import auto_suggestion_service
 
 from .base import DEFAULT_CLIENT_INFO, AutoSuggestionServiceTransport
+from .grpc import AutoSuggestionServiceGrpcTransport
 
 
-class AutoSuggestionServiceGrpcTransport(AutoSuggestionServiceTransport):
-    """gRPC backend transport for AutoSuggestionService.
+class AutoSuggestionServiceGrpcAsyncIOTransport(AutoSuggestionServiceTransport):
+    """gRPC AsyncIO backend transport for AutoSuggestionService.
 
     This stateless API provides automatic suggestions for natural
     language queries for the data sources in the provided project and
     location.
 
     The service provides a resourceless operation ``suggestQueries``
     that can be called to get a list of suggestions for a given
@@ -106,28 +107,72 @@
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "dataqna.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -139,17 +184,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -168,15 +214,15 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
@@ -188,15 +234,14 @@
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -242,81 +287,39 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
     def suggest_queries(
         self,
     ) -> Callable[
         [auto_suggestion_service.SuggestQueriesRequest],
-        auto_suggestion_service.SuggestQueriesResponse,
+        Awaitable[auto_suggestion_service.SuggestQueriesResponse],
     ]:
         r"""Return a callable for the suggest queries method over gRPC.
 
         Gets a list of suggestions based on a prefix string.
         AutoSuggestion tolerance should be less than 1 second.
 
         Returns:
             Callable[[~.SuggestQueriesRequest],
-                    ~.SuggestQueriesResponse]:
+                    Awaitable[~.SuggestQueriesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -325,15 +328,11 @@
                 "/google.cloud.dataqna.v1alpha.AutoSuggestionService/SuggestQueries",
                 request_serializer=auto_suggestion_service.SuggestQueriesRequest.serialize,
                 response_deserializer=auto_suggestion_service.SuggestQueriesResponse.deserialize,
             )
         return self._stubs["suggest_queries"]
 
     def close(self):
-        self.grpc_channel.close()
-
-    @property
-    def kind(self) -> str:
-        return "grpc"
+        return self.grpc_channel.close()
 
 
-__all__ = ("AutoSuggestionServiceGrpcTransport",)
+__all__ = ("AutoSuggestionServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc_asyncio.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import gapic_v1, grpc_helpers
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import auto_suggestion_service
 
 from .base import DEFAULT_CLIENT_INFO, AutoSuggestionServiceTransport
-from .grpc import AutoSuggestionServiceGrpcTransport
 
 
-class AutoSuggestionServiceGrpcAsyncIOTransport(AutoSuggestionServiceTransport):
-    """gRPC AsyncIO backend transport for AutoSuggestionService.
+class AutoSuggestionServiceGrpcTransport(AutoSuggestionServiceTransport):
+    """gRPC backend transport for AutoSuggestionService.
 
     This stateless API provides automatic suggestions for natural
     language queries for the data sources in the provided project and
     location.
 
     The service provides a resourceless operation ``suggestQueries``
     that can be called to get a list of suggestions for a given
@@ -107,73 +106,29 @@
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
@@ -184,18 +139,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -214,15 +168,15 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
@@ -234,14 +188,15 @@
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -287,39 +242,81 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "dataqna.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def suggest_queries(
         self,
     ) -> Callable[
         [auto_suggestion_service.SuggestQueriesRequest],
-        Awaitable[auto_suggestion_service.SuggestQueriesResponse],
+        auto_suggestion_service.SuggestQueriesResponse,
     ]:
         r"""Return a callable for the suggest queries method over gRPC.
 
         Gets a list of suggestions based on a prefix string.
         AutoSuggestion tolerance should be less than 1 second.
 
         Returns:
             Callable[[~.SuggestQueriesRequest],
-                    Awaitable[~.SuggestQueriesResponse]]:
+                    ~.SuggestQueriesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -328,11 +325,15 @@
                 "/google.cloud.dataqna.v1alpha.AutoSuggestionService/SuggestQueries",
                 request_serializer=auto_suggestion_service.SuggestQueriesRequest.serialize,
                 response_deserializer=auto_suggestion_service.SuggestQueriesResponse.deserialize,
             )
         return self._stubs["suggest_queries"]
 
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("AutoSuggestionServiceGrpcAsyncIOTransport",)
+__all__ = ("AutoSuggestionServiceGrpcTransport",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/rest.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,21 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the AutoSuggestionServiceRestTransport.
 
     .. code-block:: python
         class MyCustomAutoSuggestionServiceInterceptor(AutoSuggestionServiceRestInterceptor):
-            def pre_suggest_queries(request, metadata):
+            def pre_suggest_queries(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_suggest_queries(response):
+            def post_suggest_queries(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = AutoSuggestionServiceRestTransport(interceptor=MyCustomAutoSuggestionServiceInterceptor())
         client = AutoSuggestionServiceClient(transport=transport)
 
 
     """
 
@@ -195,18 +196,18 @@
     library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[AutoSuggestionServiceRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
@@ -290,15 +291,15 @@
             }
 
         def __call__(
             self,
             request: auto_suggestion_service.SuggestQueriesRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> auto_suggestion_service.SuggestQueriesResponse:
             r"""Call the suggest queries method over HTTP.
 
             Args:
                 request (~.auto_suggestion_service.SuggestQueriesRequest):
                     The request object. Request for query suggestions.
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/async_client.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import any_pb2  # type: ignore
@@ -183,17 +194,17 @@
     get_transport_class = functools.partial(
         type(QuestionServiceClient).get_transport_class, type(QuestionServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, QuestionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the question service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -229,19 +240,19 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def get_question(
         self,
-        request: Union[question_service.GetQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.GetQuestionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> question.Question:
         r"""Gets a previously created question.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -265,15 +276,15 @@
                 # Make the request
                 response = await client.get_question(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.GetQuestionRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.GetQuestionRequest, dict]]):
                 The request object. A request to get a previously
                 created question.
             name (:class:`str`):
                 Required. The unique identifier for the question.
                 Example: ``projects/foo/locations/bar/questions/1234``
 
                 This corresponds to the ``name`` field
@@ -334,20 +345,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_question(
         self,
-        request: Union[question_service.CreateQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.CreateQuestionRequest, dict]] = None,
         *,
-        parent: str = None,
-        question: gcd_question.Question = None,
+        parent: Optional[str] = None,
+        question: Optional[gcd_question.Question] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcd_question.Question:
         r"""Creates a question.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -376,15 +387,15 @@
                 # Make the request
                 response = await client.create_question(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.CreateQuestionRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.CreateQuestionRequest, dict]]):
                 The request object. Request to create a question
                 resource.
             parent (:class:`str`):
                 Required. The name of the project this data source
                 reference belongs to. Example:
                 ``projects/foo/locations/bar``
 
@@ -453,20 +464,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def execute_question(
         self,
-        request: Union[question_service.ExecuteQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.ExecuteQuestionRequest, dict]] = None,
         *,
-        name: str = None,
-        interpretation_index: int = None,
+        name: Optional[str] = None,
+        interpretation_index: Optional[int] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> question.Question:
         r"""Executes an interpretation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -491,15 +502,15 @@
                 # Make the request
                 response = await client.execute_question(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.ExecuteQuestionRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.ExecuteQuestionRequest, dict]]):
                 The request object. Request to execute an
                 interpretation.
             name (:class:`str`):
                 Required. The unique identifier for the question.
                 Example: ``projects/foo/locations/bar/questions/1234``
 
                 This corresponds to the ``name`` field
@@ -569,19 +580,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_user_feedback(
         self,
-        request: Union[question_service.GetUserFeedbackRequest, dict] = None,
+        request: Optional[Union[question_service.GetUserFeedbackRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> user_feedback.UserFeedback:
         r"""Gets previously created user feedback.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -605,15 +616,15 @@
                 # Make the request
                 response = await client.get_user_feedback(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.GetUserFeedbackRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.GetUserFeedbackRequest, dict]]):
                 The request object. Request to get user feedback.
             name (:class:`str`):
                 Required. The unique identifier for the user feedback.
                 User feedback is a singleton resource on a Question.
                 Example:
                 ``projects/foo/locations/bar/questions/1234/userFeedback``
 
@@ -670,20 +681,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_user_feedback(
         self,
-        request: Union[question_service.UpdateUserFeedbackRequest, dict] = None,
+        request: Optional[
+            Union[question_service.UpdateUserFeedbackRequest, dict]
+        ] = None,
         *,
-        user_feedback: gcd_user_feedback.UserFeedback = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        user_feedback: Optional[gcd_user_feedback.UserFeedback] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcd_user_feedback.UserFeedback:
         r"""Updates user feedback. This creates user feedback if
         there was none before (upsert).
 
         .. code-block:: python
 
@@ -711,15 +724,15 @@
                 # Make the request
                 response = await client.update_user_feedback(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.dataqna_v1alpha.types.UpdateUserFeedbackRequest, dict]):
+            request (Optional[Union[google.cloud.dataqna_v1alpha.types.UpdateUserFeedbackRequest, dict]]):
                 The request object. Request to updates user feedback.
             user_feedback (:class:`google.cloud.dataqna_v1alpha.types.UserFeedback`):
                 Required. The user feedback to
                 update. This can be called even if there
                 is no user feedback so far. The
                 feedback's name field is used to
                 identify the user feedback (and the
@@ -792,18 +805,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("QuestionServiceAsyncClient",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/client.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
+
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.protobuf import any_pb2  # type: ignore
@@ -63,15 +75,15 @@
     )  # type: Dict[str, Type[QuestionServiceTransport]]
     _transport_registry["grpc"] = QuestionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = QuestionServiceGrpcAsyncIOTransport
     _transport_registry["rest"] = QuestionServiceRestTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[QuestionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -377,16 +389,16 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, QuestionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, QuestionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the question service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -395,15 +407,15 @@
                 credentials from the environment.
             transport (Union[str, QuestionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
                 NOTE: "rest" transport functionality is currently in a
                 beta state (preview). We welcome your feedback via an
                 issue in this library's source repository.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -425,14 +437,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -477,19 +490,19 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def get_question(
         self,
-        request: Union[question_service.GetQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.GetQuestionRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> question.Question:
         r"""Gets a previously created question.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -582,20 +595,20 @@
         )
 
         # Done; return the response.
         return response
 
     def create_question(
         self,
-        request: Union[question_service.CreateQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.CreateQuestionRequest, dict]] = None,
         *,
-        parent: str = None,
-        question: gcd_question.Question = None,
+        parent: Optional[str] = None,
+        question: Optional[gcd_question.Question] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcd_question.Question:
         r"""Creates a question.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -701,20 +714,20 @@
         )
 
         # Done; return the response.
         return response
 
     def execute_question(
         self,
-        request: Union[question_service.ExecuteQuestionRequest, dict] = None,
+        request: Optional[Union[question_service.ExecuteQuestionRequest, dict]] = None,
         *,
-        name: str = None,
-        interpretation_index: int = None,
+        name: Optional[str] = None,
+        interpretation_index: Optional[int] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> question.Question:
         r"""Executes an interpretation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -817,19 +830,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_user_feedback(
         self,
-        request: Union[question_service.GetUserFeedbackRequest, dict] = None,
+        request: Optional[Union[question_service.GetUserFeedbackRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> user_feedback.UserFeedback:
         r"""Gets previously created user feedback.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -918,20 +931,22 @@
         )
 
         # Done; return the response.
         return response
 
     def update_user_feedback(
         self,
-        request: Union[question_service.UpdateUserFeedbackRequest, dict] = None,
+        request: Optional[
+            Union[question_service.UpdateUserFeedbackRequest, dict]
+        ] = None,
         *,
-        user_feedback: gcd_user_feedback.UserFeedback = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        user_feedback: Optional[gcd_user_feedback.UserFeedback] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gcd_user_feedback.UserFeedback:
         r"""Updates user feedback. This creates user feedback if
         there was none before (upsert).
 
         .. code-block:: python
 
@@ -1047,18 +1062,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("QuestionServiceClient",)
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/base.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,44 +19,39 @@
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
-import pkg_resources
 
+from google.cloud.dataqna_v1alpha import gapic_version as package_version
 from google.cloud.dataqna_v1alpha.types import user_feedback as gcd_user_feedback
 from google.cloud.dataqna_v1alpha.types import question
 from google.cloud.dataqna_v1alpha.types import question as gcd_question
 from google.cloud.dataqna_v1alpha.types import question_service
 from google.cloud.dataqna_v1alpha.types import user_feedback
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-dataqna",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class QuestionServiceTransport(abc.ABC):
     """Abstract transport class for QuestionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "dataqna.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,22 +62,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -196,16 +196,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc_asyncio.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -107,23 +107,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/services/question_service/transports/rest.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/services/question_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,48 +63,53 @@
     * Stripping extraneous information from responses
 
     These use cases and more can be enabled by injecting an
     instance of a custom subclass when constructing the QuestionServiceRestTransport.
 
     .. code-block:: python
         class MyCustomQuestionServiceInterceptor(QuestionServiceRestInterceptor):
-            def pre_create_question(request, metadata):
+            def pre_create_question(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_create_question(response):
+            def post_create_question(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_execute_question(request, metadata):
+            def pre_execute_question(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_execute_question(response):
+            def post_execute_question(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_get_question(request, metadata):
+            def pre_get_question(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_get_question(response):
+            def post_get_question(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_get_user_feedback(request, metadata):
+            def pre_get_user_feedback(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_get_user_feedback(response):
+            def post_get_user_feedback(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
-            def pre_update_user_feedback(request, metadata):
+            def pre_update_user_feedback(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
-            def post_update_user_feedback(response):
+            def post_update_user_feedback(self, response):
                 logging.log(f"Received response: {response}")
+                return response
 
         transport = QuestionServiceRestTransport(interceptor=MyCustomQuestionServiceInterceptor())
         client = QuestionServiceClient(transport=transport)
 
 
     """
 
@@ -259,18 +264,18 @@
     library's source repository. Thank you!
     """
 
     def __init__(
         self,
         *,
         host: str = "dataqna.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         url_scheme: str = "https",
         interceptor: Optional[QuestionServiceRestInterceptor] = None,
         api_audience: Optional[str] = None,
     ) -> None:
@@ -354,15 +359,15 @@
             }
 
         def __call__(
             self,
             request: question_service.CreateQuestionRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcd_question.Question:
             r"""Call the create question method over HTTP.
 
             Args:
                 request (~.question_service.CreateQuestionRequest):
                     The request object. Request to create a question
@@ -454,15 +459,15 @@
             }
 
         def __call__(
             self,
             request: question_service.ExecuteQuestionRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> question.Question:
             r"""Call the execute question method over HTTP.
 
             Args:
                 request (~.question_service.ExecuteQuestionRequest):
                     The request object. Request to execute an interpretation.
@@ -554,15 +559,15 @@
             }
 
         def __call__(
             self,
             request: question_service.GetQuestionRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> question.Question:
             r"""Call the get question method over HTTP.
 
             Args:
                 request (~.question_service.GetQuestionRequest):
                     The request object. A request to get a previously created
@@ -645,15 +650,15 @@
             }
 
         def __call__(
             self,
             request: question_service.GetUserFeedbackRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> user_feedback.UserFeedback:
             r"""Call the get user feedback method over HTTP.
 
             Args:
                 request (~.question_service.GetUserFeedbackRequest):
                     The request object. Request to get user feedback.
@@ -731,15 +736,15 @@
             }
 
         def __call__(
             self,
             request: question_service.UpdateUserFeedbackRequest,
             *,
             retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: float = None,
+            timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> gcd_user_feedback.UserFeedback:
             r"""Call the update user feedback method over HTTP.
 
             Args:
                 request (~.question_service.UpdateUserFeedbackRequest):
                     The request object. Request to updates user feedback.
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/__init__.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/annotated_string.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/annotated_string.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.dataqna.v1alpha",
     manifest={
         "AnnotatedString",
     },
@@ -56,15 +58,15 @@
     same, while semantic markups are different.
 
     Attributes:
         text_formatted (str):
             Text version of the string.
         html_formatted (str):
             HTML version of the string annotation.
-        markups (Sequence[google.cloud.dataqna_v1alpha.types.AnnotatedString.SemanticMarkup]):
+        markups (MutableSequence[google.cloud.dataqna_v1alpha.types.AnnotatedString.SemanticMarkup]):
             Semantic version of the string annotation.
     """
 
     class SemanticMarkupType(proto.Enum):
         r"""Semantic markup types."""
         MARKUP_TYPE_UNSPECIFIED = 0
         METRIC = 1
@@ -84,37 +86,37 @@
             start_char_index (int):
                 Unicode character index of the query.
             length (int):
                 The length (number of unicode characters) of
                 the markup substring.
         """
 
-        type_ = proto.Field(
+        type_: "AnnotatedString.SemanticMarkupType" = proto.Field(
             proto.ENUM,
             number=1,
             enum="AnnotatedString.SemanticMarkupType",
         )
-        start_char_index = proto.Field(
+        start_char_index: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        length = proto.Field(
+        length: int = proto.Field(
             proto.INT32,
             number=3,
         )
 
-    text_formatted = proto.Field(
+    text_formatted: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    html_formatted = proto.Field(
+    html_formatted: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    markups = proto.RepeatedField(
+    markups: MutableSequence[SemanticMarkup] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=SemanticMarkup,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/auto_suggestion_service.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/auto_suggestion_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import annotated_string
 
 __protobuf__ = proto.module(
     package="google.cloud.dataqna.v1alpha",
     manifest={
@@ -40,47 +42,47 @@
     r"""Request for query suggestions.
 
     Attributes:
         parent (str):
             Required. The parent of the suggestion query
             is the resource denoting the project and
             location.
-        scopes (Sequence[str]):
+        scopes (MutableSequence[str]):
             The scopes to which this search is restricted. The only
             supported scope pattern is
             ``//bigquery.googleapis.com/projects/{GCP-PROJECT-ID}/datasets/{DATASET-ID}/tables/{TABLE-ID}``.
         query (str):
             User query for which to generate suggestions.
             If the query is empty, zero state suggestions
             are returned. This allows UIs to display
             suggestions right away, helping the user to get
             a sense of what a query might look like.
-        suggestion_types (Sequence[google.cloud.dataqna_v1alpha.types.SuggestionType]):
+        suggestion_types (MutableSequence[google.cloud.dataqna_v1alpha.types.SuggestionType]):
             The requested suggestion type. Multiple
             suggestion types can be requested, but there is
             no guarantee that the service will return
             suggestions for each type. Suggestions for a
             requested type might rank lower than suggestions
             for other types and the service may decide to
             cut these suggestions off.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    scopes = proto.RepeatedField(
+    scopes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=2,
     )
-    query = proto.Field(
+    query: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    suggestion_types = proto.RepeatedField(
+    suggestion_types: MutableSequence["SuggestionType"] = proto.RepeatedField(
         proto.ENUM,
         number=4,
         enum="SuggestionType",
     )
 
 
 class Suggestion(proto.Message):
@@ -94,24 +96,24 @@
             ordering in UI. The score represents confidence in the
             suggestion where higher is better. All score values must be
             in the range [0, 1).
         suggestion_type (google.cloud.dataqna_v1alpha.types.SuggestionType):
             The type of the suggestion.
     """
 
-    suggestion_info = proto.Field(
+    suggestion_info: "SuggestionInfo" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="SuggestionInfo",
     )
-    ranking_score = proto.Field(
+    ranking_score: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
-    suggestion_type = proto.Field(
+    suggestion_type: "SuggestionType" = proto.Field(
         proto.ENUM,
         number=3,
         enum="SuggestionType",
     )
 
 
 class SuggestionInfo(proto.Message):
@@ -119,15 +121,15 @@
 
     Attributes:
         annotated_suggestion (google.cloud.dataqna_v1alpha.types.AnnotatedString):
             Annotations for the suggestion. This provides
             information about which part of the suggestion
             corresponds to what semantic meaning (e.g. a
             metric).
-        query_matches (Sequence[google.cloud.dataqna_v1alpha.types.SuggestionInfo.MatchInfo]):
+        query_matches (MutableSequence[google.cloud.dataqna_v1alpha.types.SuggestionInfo.MatchInfo]):
             Matches between user query and the annotated
             string.
     """
 
     class MatchInfo(proto.Message):
         r"""MatchInfo describes which part of suggestion matched with data in
         user typed query. This can be used to highlight matching parts in
@@ -159,44 +161,44 @@
                 Unicode character index of the string
                 annotation.
             length (int):
                 Count of unicode characters of this
                 substring.
         """
 
-        start_char_index = proto.Field(
+        start_char_index: int = proto.Field(
             proto.INT32,
             number=1,
         )
-        length = proto.Field(
+        length: int = proto.Field(
             proto.INT32,
             number=2,
         )
 
-    annotated_suggestion = proto.Field(
+    annotated_suggestion: annotated_string.AnnotatedString = proto.Field(
         proto.MESSAGE,
         number=1,
         message=annotated_string.AnnotatedString,
     )
-    query_matches = proto.RepeatedField(
+    query_matches: MutableSequence[MatchInfo] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=MatchInfo,
     )
 
 
 class SuggestQueriesResponse(proto.Message):
     r"""Response to SuggestQueries.
 
     Attributes:
-        suggestions (Sequence[google.cloud.dataqna_v1alpha.types.Suggestion]):
+        suggestions (MutableSequence[google.cloud.dataqna_v1alpha.types.Suggestion]):
             A list of suggestions.
     """
 
-    suggestions = proto.RepeatedField(
+    suggestions: MutableSequence["Suggestion"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="Suggestion",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/question.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/question.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import any_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import annotated_string
 
@@ -50,27 +52,27 @@
     retrieval status. A question cannot be modified.
 
     Attributes:
         name (str):
             Output only. Immutable. The unique identifier for the
             Question. The ID is server-generated. Example:
             ``projects/foo/locations/bar/questions/123``
-        scopes (Sequence[str]):
+        scopes (MutableSequence[str]):
             Required. Immutable. Scopes to be used for the question. A
             scope defines the relevant data set scope. It can be a
             reference to a specific data source or a collection of data
             sources. Currently, support is limited to a single BigQuery
             table. There must be exactly one ``scopes`` element.
 
             Example:
             ``//bigquery.googleapis.com/projects/test-project/datasets/foo/tables/bar``
         query (str):
             Required. Immutable. The query in natural
             language.
-        data_source_annotations (Sequence[str]):
+        data_source_annotations (MutableSequence[str]):
             A list of annotations to use instead of the
             default annotation of a data source (set in the
             data source reference resource). There must not
             be more than one annotation with the same data
             source reference.
         interpret_error (google.cloud.dataqna_v1alpha.types.InterpretError):
             An error field explaining why interpretation
@@ -79,15 +81,15 @@
             Note: This is different from getting a status
             error on the request itself. This is not a
             client or server error and the Question resource
             is still persisted, but the service could not
             interpret the question. Clients should present
             the error to the user so the user can rephrase
             the question.
-        interpretations (Sequence[google.cloud.dataqna_v1alpha.types.Interpretation]):
+        interpretations (MutableSequence[google.cloud.dataqna_v1alpha.types.Interpretation]):
             A list of interpretations for this question.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Time when the question was created.
         user_email (str):
             Output only. The e-mail address of the user
             that created this question.
         debug_flags (google.cloud.dataqna_v1alpha.types.DebugFlags):
@@ -97,55 +99,55 @@
             Top level debug information.
             This will be stored as the type
             DebugInformation. Using Any so clients don't
             need to pull in anything inside the debug
             message.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    scopes = proto.RepeatedField(
+    scopes: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=2,
     )
-    query = proto.Field(
+    query: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    data_source_annotations = proto.RepeatedField(
+    data_source_annotations: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=4,
     )
-    interpret_error = proto.Field(
+    interpret_error: "InterpretError" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="InterpretError",
     )
-    interpretations = proto.RepeatedField(
+    interpretations: MutableSequence["Interpretation"] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message="Interpretation",
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    user_email = proto.Field(
+    user_email: str = proto.Field(
         proto.STRING,
         number=8,
     )
-    debug_flags = proto.Field(
+    debug_flags: "DebugFlags" = proto.Field(
         proto.MESSAGE,
         number=9,
         message="DebugFlags",
     )
-    debug_info = proto.Field(
+    debug_info: any_pb2.Any = proto.Field(
         proto.MESSAGE,
         number=10,
         message=any_pb2.Any,
     )
 
 
 class InterpretError(proto.Message):
@@ -180,80 +182,82 @@
                 unsupported.
             incomplete_query_details (google.cloud.dataqna_v1alpha.types.InterpretError.InterpretIncompleteQueryDetails):
                 Populated if the query is incomplete.
             ambiguity_details (google.cloud.dataqna_v1alpha.types.InterpretError.InterpretAmbiguityDetails):
                 Populated if the query was too ambiguous.
         """
 
-        unsupported_details = proto.Field(
+        unsupported_details: "InterpretError.InterpretUnsupportedDetails" = proto.Field(
             proto.MESSAGE,
             number=1,
             message="InterpretError.InterpretUnsupportedDetails",
         )
-        incomplete_query_details = proto.Field(
-            proto.MESSAGE,
-            number=2,
-            message="InterpretError.InterpretIncompleteQueryDetails",
+        incomplete_query_details: "InterpretError.InterpretIncompleteQueryDetails" = (
+            proto.Field(
+                proto.MESSAGE,
+                number=2,
+                message="InterpretError.InterpretIncompleteQueryDetails",
+            )
         )
-        ambiguity_details = proto.Field(
+        ambiguity_details: "InterpretError.InterpretAmbiguityDetails" = proto.Field(
             proto.MESSAGE,
             number=3,
             message="InterpretError.InterpretAmbiguityDetails",
         )
 
     class InterpretUnsupportedDetails(proto.Message):
         r"""Details about unsupported parts in a query.
 
         Attributes:
-            operators (Sequence[str]):
+            operators (MutableSequence[str]):
                 Unsupported operators. For example: median.
-            intent (Sequence[str]):
+            intent (MutableSequence[str]):
                 Unsupported intents.
         """
 
-        operators = proto.RepeatedField(
+        operators: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
-        intent = proto.RepeatedField(
+        intent: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=2,
         )
 
     class InterpretIncompleteQueryDetails(proto.Message):
         r"""Details about an incomplete query.
 
         Attributes:
-            entities (Sequence[google.cloud.dataqna_v1alpha.types.InterpretEntity]):
+            entities (MutableSequence[google.cloud.dataqna_v1alpha.types.InterpretEntity]):
                 List of missing interpret entities.
         """
 
-        entities = proto.RepeatedField(
+        entities: MutableSequence["InterpretEntity"] = proto.RepeatedField(
             proto.ENUM,
             number=1,
             enum="InterpretEntity",
         )
 
     class InterpretAmbiguityDetails(proto.Message):
         r"""Details about a query that was too ambiguous. Currently, the
         message has no fields and its presence signals that there was
         ambiguity.
 
         """
 
-    message = proto.Field(
+    message: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    code = proto.Field(
+    code: InterpretErrorCode = proto.Field(
         proto.ENUM,
         number=2,
         enum=InterpretErrorCode,
     )
-    details = proto.Field(
+    details: InterpretErrorDetails = proto.Field(
         proto.MESSAGE,
         number=3,
         message=InterpretErrorDetails,
     )
 
 
 class ExecutionInfo(proto.Message):
@@ -279,30 +283,30 @@
         r"""Enum of possible job execution statuses."""
         JOB_EXECUTION_STATE_UNSPECIFIED = 0
         NOT_EXECUTED = 1
         RUNNING = 2
         SUCCEEDED = 3
         FAILED = 4
 
-    job_creation_status = proto.Field(
+    job_creation_status: status_pb2.Status = proto.Field(
         proto.MESSAGE,
         number=1,
         message=status_pb2.Status,
     )
-    job_execution_state = proto.Field(
+    job_execution_state: JobExecutionState = proto.Field(
         proto.ENUM,
         number=2,
         enum=JobExecutionState,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    bigquery_job = proto.Field(
+    bigquery_job: "BigQueryJob" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="BigQueryJob",
     )
 
 
 class BigQueryJob(proto.Message):
@@ -315,40 +319,40 @@
             The job ID.
         project_id (str):
             The project ID of the job.
         location (str):
             The location where the job is running.
     """
 
-    job_id = proto.Field(
+    job_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    project_id = proto.Field(
+    project_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    location = proto.Field(
+    location: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class Interpretation(proto.Message):
     r"""An interpretation of a natural language query.
 
     Attributes:
-        data_sources (Sequence[str]):
+        data_sources (MutableSequence[str]):
             List of data sources used in the current
             understanding.
         confidence (float):
             The level of confidence that one of the interpretations is
             correct. This is a value in the range [0, 1] where a value
             of 0.5 or below is to be considered a low confidence.
-        unused_phrases (Sequence[str]):
+        unused_phrases (MutableSequence[str]):
             A list of unused phrases. Clients should
             display a Did You Mean (DYM)  dialog if this is
             non-empty, even if this is the only
             interpretation.
         human_readable (google.cloud.dataqna_v1alpha.types.HumanReadable):
             Human readable representation of the query.
         interpretation_structure (google.cloud.dataqna_v1alpha.types.InterpretationStructure):
@@ -360,42 +364,42 @@
             to the backend.
         execution_info (google.cloud.dataqna_v1alpha.types.ExecutionInfo):
             Information about the backend response. This
             is populated only if execution of an
             interpretation was requested.
     """
 
-    data_sources = proto.RepeatedField(
+    data_sources: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
-    confidence = proto.Field(
+    confidence: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
-    unused_phrases = proto.RepeatedField(
+    unused_phrases: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
-    human_readable = proto.Field(
+    human_readable: "HumanReadable" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="HumanReadable",
     )
-    interpretation_structure = proto.Field(
+    interpretation_structure: "InterpretationStructure" = proto.Field(
         proto.MESSAGE,
         number=5,
         message="InterpretationStructure",
     )
-    data_query = proto.Field(
+    data_query: "DataQuery" = proto.Field(
         proto.MESSAGE,
         number=6,
         message="DataQuery",
     )
-    execution_info = proto.Field(
+    execution_info: "ExecutionInfo" = proto.Field(
         proto.MESSAGE,
         number=7,
         message="ExecutionInfo",
     )
 
 
 class DataQuery(proto.Message):
@@ -408,15 +412,15 @@
 
     Attributes:
         sql (str):
             The generated SQL query to be sent to the
             backend.
     """
 
-    sql = proto.Field(
+    sql: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class HumanReadable(proto.Message):
     r"""Human readable interpretation.
@@ -425,36 +429,36 @@
         generated_interpretation (google.cloud.dataqna_v1alpha.types.AnnotatedString):
             Generated query explaining the
             interpretation.
         original_question (google.cloud.dataqna_v1alpha.types.AnnotatedString):
             Annotations on the original query.
     """
 
-    generated_interpretation = proto.Field(
+    generated_interpretation: annotated_string.AnnotatedString = proto.Field(
         proto.MESSAGE,
         number=1,
         message=annotated_string.AnnotatedString,
     )
-    original_question = proto.Field(
+    original_question: annotated_string.AnnotatedString = proto.Field(
         proto.MESSAGE,
         number=2,
         message=annotated_string.AnnotatedString,
     )
 
 
 class InterpretationStructure(proto.Message):
     r"""Information about the interpretation structure that helps to
     understand and visualize the response.
 
     Attributes:
-        visualization_types (Sequence[google.cloud.dataqna_v1alpha.types.InterpretationStructure.VisualizationType]):
+        visualization_types (MutableSequence[google.cloud.dataqna_v1alpha.types.InterpretationStructure.VisualizationType]):
             List of possible visualization types to apply
             for this interpretation. The order has no
             relevance.
-        column_info (Sequence[google.cloud.dataqna_v1alpha.types.InterpretationStructure.ColumnInfo]):
+        column_info (MutableSequence[google.cloud.dataqna_v1alpha.types.InterpretationStructure.ColumnInfo]):
             Information about the output columns, that
             is, the columns that will be returned by the
             backend.
     """
 
     class VisualizationType(proto.Enum):
         r"""Enumeration of visualzation types to use for query response
@@ -483,29 +487,29 @@
                 backend. For example, the field name in the
                 schema provided in the query response in
                 BigQuery.
             display_name (str):
                 Human readable name of the output column.
         """
 
-        output_alias = proto.Field(
+        output_alias: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        display_name = proto.Field(
+        display_name: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
-    visualization_types = proto.RepeatedField(
+    visualization_types: MutableSequence[VisualizationType] = proto.RepeatedField(
         proto.ENUM,
         number=1,
         enum=VisualizationType,
     )
-    column_info = proto.RepeatedField(
+    column_info: MutableSequence[ColumnInfo] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=ColumnInfo,
     )
 
 
 class DebugFlags(proto.Message):
@@ -547,58 +551,58 @@
             Analyza.
         include_table_list (bool):
             Whether to include the table list.
         include_domain_list (bool):
             Whether to include the domain list.
     """
 
-    include_va_query = proto.Field(
+    include_va_query: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
-    include_nested_va_query = proto.Field(
+    include_nested_va_query: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
-    include_human_interpretation = proto.Field(
+    include_human_interpretation: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
-    include_aqua_debug_response = proto.Field(
+    include_aqua_debug_response: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
-    time_override = proto.Field(
+    time_override: int = proto.Field(
         proto.INT64,
         number=5,
     )
-    is_internal_google_user = proto.Field(
+    is_internal_google_user: bool = proto.Field(
         proto.BOOL,
         number=6,
     )
-    ignore_cache = proto.Field(
+    ignore_cache: bool = proto.Field(
         proto.BOOL,
         number=7,
     )
-    include_search_entities_rpc = proto.Field(
+    include_search_entities_rpc: bool = proto.Field(
         proto.BOOL,
         number=8,
     )
-    include_list_column_annotations_rpc = proto.Field(
+    include_list_column_annotations_rpc: bool = proto.Field(
         proto.BOOL,
         number=9,
     )
-    include_virtual_analyst_entities = proto.Field(
+    include_virtual_analyst_entities: bool = proto.Field(
         proto.BOOL,
         number=10,
     )
-    include_table_list = proto.Field(
+    include_table_list: bool = proto.Field(
         proto.BOOL,
         number=11,
     )
-    include_domain_list = proto.Field(
+    include_domain_list: bool = proto.Field(
         proto.BOOL,
         number=12,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/question_service.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/question_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 from google.protobuf import field_mask_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.dataqna_v1alpha.types import user_feedback as gcd_user_feedback
 from google.cloud.dataqna_v1alpha.types import question as gcd_question
 
 __protobuf__ = proto.module(
@@ -38,19 +40,19 @@
         name (str):
             Required. The unique identifier for the question. Example:
             ``projects/foo/locations/bar/questions/1234``
         read_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be retrieved.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    read_mask = proto.Field(
+    read_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class CreateQuestionRequest(proto.Message):
@@ -60,19 +62,19 @@
         parent (str):
             Required. The name of the project this data source reference
             belongs to. Example: ``projects/foo/locations/bar``
         question (google.cloud.dataqna_v1alpha.types.Question):
             Required. The question to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    question = proto.Field(
+    question: gcd_question.Question = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gcd_question.Question,
     )
 
 
 class ExecuteQuestionRequest(proto.Message):
@@ -83,19 +85,19 @@
             Required. The unique identifier for the question. Example:
             ``projects/foo/locations/bar/questions/1234``
         interpretation_index (int):
             Required. Index of the interpretation to
             execute.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    interpretation_index = proto.Field(
+    interpretation_index: int = proto.Field(
         proto.INT32,
         number=2,
     )
 
 
 class GetUserFeedbackRequest(proto.Message):
     r"""Request to get user feedback.
@@ -103,15 +105,15 @@
     Attributes:
         name (str):
             Required. The unique identifier for the user feedback. User
             feedback is a singleton resource on a Question. Example:
             ``projects/foo/locations/bar/questions/1234/userFeedback``
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateUserFeedbackRequest(proto.Message):
     r"""Request to updates user feedback.
@@ -123,20 +125,20 @@
             so far. The feedback's name field is used to
             identify the user feedback (and the
             corresponding question) to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The list of fields to be updated.
     """
 
-    user_feedback = proto.Field(
+    user_feedback: gcd_user_feedback.UserFeedback = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gcd_user_feedback.UserFeedback,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-data-qna-0.8.2/google/cloud/dataqna_v1alpha/types/user_feedback.py` & `google-cloud-data-qna-0.9.0/google/cloud/dataqna_v1alpha/types/user_feedback.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.dataqna.v1alpha",
     manifest={
         "UserFeedback",
     },
@@ -39,23 +41,23 @@
 
     class UserFeedbackRating(proto.Enum):
         r"""Enumeration of feedback ratings."""
         USER_FEEDBACK_RATING_UNSPECIFIED = 0
         POSITIVE = 1
         NEGATIVE = 2
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    free_form_feedback = proto.Field(
+    free_form_feedback: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    rating = proto.Field(
+    rating: UserFeedbackRating = proto.Field(
         proto.ENUM,
         number=3,
         enum=UserFeedbackRating,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/PKG-INFO` & `google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: google-cloud-data-qna
-Version: 0.8.2
+Version: 0.9.0
+Summary: Google Cloud Data Qna API client library
 Home-page: https://github.com/googleapis/python-data-qna
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Data QnA API
 ==============================
 
 |preview| |pypi| |versions|
```

### Comparing `google-cloud-data-qna-0.8.2/google_cloud_data_qna.egg-info/SOURCES.txt` & `google-cloud-data-qna-0.9.0/google_cloud_data_qna.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/dataqna/__init__.py
+google/cloud/dataqna/gapic_version.py
 google/cloud/dataqna/py.typed
 google/cloud/dataqna_v1alpha/__init__.py
 google/cloud/dataqna_v1alpha/gapic_metadata.json
+google/cloud/dataqna_v1alpha/gapic_version.py
 google/cloud/dataqna_v1alpha/py.typed
 google/cloud/dataqna_v1alpha/services/__init__.py
 google/cloud/dataqna_v1alpha/services/auto_suggestion_service/__init__.py
 google/cloud/dataqna_v1alpha/services/auto_suggestion_service/async_client.py
 google/cloud/dataqna_v1alpha/services/auto_suggestion_service/client.py
 google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/__init__.py
 google/cloud/dataqna_v1alpha/services/auto_suggestion_service/transports/base.py
```

### Comparing `google-cloud-data-qna-0.8.2/tests/__init__.py` & `google-cloud-data-qna-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/tests/unit/__init__.py` & `google-cloud-data-qna-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/tests/unit/gapic/__init__.py` & `google-cloud-data-qna-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/__init__.py` & `google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/test_auto_suggestion_service.py` & `google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/test_auto_suggestion_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-data-qna-0.8.2/tests/unit/gapic/dataqna_v1alpha/test_question_service.py` & `google-cloud-data-qna-0.9.0/tests/unit/gapic/dataqna_v1alpha/test_question_service.py`

 * *Files identical despite different names*

