# Comparing `tmp/google-cloud-support-0.1.0.tar.gz` & `tmp/google-cloud-support-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-support-0.1.0.tar", last modified: Fri May 12 16:05:38 2023, max compression
+gzip compressed data, was "google-cloud-support-0.1.1.tar", last modified: Wed Jul  5 15:56:11 2023, max compression
```

## Comparing `google-cloud-support-0.1.0.tar` & `google-cloud-support-0.1.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.411333 google-cloud-support-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4700 2023-05-12 16:05:38.411333 google-cloud-support-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3792 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.395328 google-cloud-support-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.395328 google-cloud-support-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.399330 google-cloud-support-0.1.0/google/cloud/support/
--rw-rw-r--   0 root         (0)     1003     3006 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.399330 google-cloud-support-0.1.0/google/cloud/support_v2/
--rw-rw-r--   0 root         (0)     1003     2475 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     5443 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       81 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.399330 google-cloud-support-0.1.0/google/cloud/support_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.399330 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/
--rw-rw-r--   0 root         (0)     1003      797 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    14846 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    24015 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/client.py
--rw-rw-r--   0 root         (0)     1003     5905 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.399330 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6463 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11913 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12125 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12544 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.403331 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/
--rw-rw-r--   0 root         (0)     1003      757 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41991 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    50928 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/client.py
--rw-rw-r--   0 root         (0)     1003    15886 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.403331 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10435 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20323 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20767 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    47467 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.403331 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    19094 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28516 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/client.py
--rw-rw-r--   0 root         (0)     1003     5767 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.403331 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6901 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13011 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13261 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17681 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/google/cloud/support_v2/types/
--rw-rw-r--   0 root         (0)     1003     1838 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2190 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/actor.py
--rw-rw-r--   0 root         (0)     1003     2469 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/attachment.py
--rw-rw-r--   0 root         (0)     1003     2749 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/attachment_service.py
--rw-rw-r--   0 root         (0)     1003     7691 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/case.py
--rw-rw-r--   0 root         (0)     1003    12647 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/case_service.py
--rw-rw-r--   0 root         (0)     1003     2281 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/comment.py
--rw-rw-r--   0 root         (0)     1003     3261 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/comment_service.py
--rw-rw-r--   0 root         (0)     1003     2281 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/google/cloud/support_v2/types/escalation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/google_cloud_support.egg-info/
--rw-r--r--   0 root         (0)     1003     4700 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3153 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-12 16:05:38.000000 google-cloud-support-0.1.0/google_cloud_support.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-05-12 16:05:38.411333 google-cloud-support-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2926 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-12 16:05:38.407332 google-cloud-support-0.1.0/tests/unit/gapic/support_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/gapic/support_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    83385 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_case_attachment_service.py
--rw-rw-r--   0 root         (0)     1003   210075 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_case_service.py
--rw-rw-r--   0 root         (0)     1003   100316 2023-05-12 16:02:57.000000 google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_comment_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.097107 google-cloud-support-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4700 2023-07-05 15:56:11.097107 google-cloud-support-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3792 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.085107 google-cloud-support-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.085107 google-cloud-support-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.085107 google-cloud-support-0.1.1/google/cloud/support/
+-rw-rw-r--   0 root         (0)     1003     3006 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.085107 google-cloud-support-0.1.1/google/cloud/support_v2/
+-rw-rw-r--   0 root         (0)     1003     2475 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5443 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       81 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.089107 google-cloud-support-0.1.1/google/cloud/support_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.089107 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14884 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    24015 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5905 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.089107 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6463 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11913 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12125 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12544 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.089107 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/
+-rw-rw-r--   0 root         (0)     1003      757 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42019 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    50928 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/client.py
+-rw-rw-r--   0 root         (0)     1003    15886 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.089107 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10435 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20323 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20767 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    47467 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19125 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28516 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5767 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6901 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13011 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13261 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17681 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/google/cloud/support_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1838 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2190 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/actor.py
+-rw-rw-r--   0 root         (0)     1003     2469 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/attachment.py
+-rw-rw-r--   0 root         (0)     1003     2749 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/attachment_service.py
+-rw-rw-r--   0 root         (0)     1003     7691 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/case.py
+-rw-rw-r--   0 root         (0)     1003    12647 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/case_service.py
+-rw-rw-r--   0 root         (0)     1003     2281 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/comment.py
+-rw-rw-r--   0 root         (0)     1003     3261 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/comment_service.py
+-rw-rw-r--   0 root         (0)     1003     2281 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/google/cloud/support_v2/types/escalation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/google_cloud_support.egg-info/
+-rw-r--r--   0 root         (0)     1003     4700 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3153 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:56:11.000000 google-cloud-support-0.1.1/google_cloud_support.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:56:11.097107 google-cloud-support-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2926 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.093107 google-cloud-support-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.097107 google-cloud-support-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:56:11.097107 google-cloud-support-0.1.1/tests/unit/gapic/support_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/gapic/support_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83584 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_case_attachment_service.py
+-rw-rw-r--   0 root         (0)     1003   210672 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_case_service.py
+-rw-rw-r--   0 root         (0)     1003   100515 2023-07-05 15:46:59.000000 google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_comment_service.py
```

### Comparing `google-cloud-support-0.1.0/LICENSE` & `google-cloud-support-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/MANIFEST.in` & `google-cloud-support-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/PKG-INFO` & `google-cloud-support-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-support
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Support API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-support-0.1.0/README.rst` & `google-cloud-support-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support/gapic_version.py` & `google-cloud-support-0.1.1/google/cloud/support/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/gapic_metadata.json` & `google-cloud-support-0.1.1/google/cloud/support_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/gapic_version.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/async_client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CaseAttachmentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/pagers.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/base.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/grpc.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/grpc_asyncio.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_attachment_service/transports/rest.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_attachment_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/async_client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1045,15 +1045,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CaseServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/pagers.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/base.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/grpc.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/grpc_asyncio.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/case_service/transports/rest.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/case_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/async_client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,15 +457,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "CommentServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/client.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/pagers.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/base.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/grpc.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/grpc_asyncio.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/services/comment_service/transports/rest.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/services/comment_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/__init__.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/actor.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/actor.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/attachment.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/attachment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/attachment_service.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/attachment_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/case.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/case.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/case_service.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/case_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/comment.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/comment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/comment_service.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/comment_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google/cloud/support_v2/types/escalation.py` & `google-cloud-support-0.1.1/google/cloud/support_v2/types/escalation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/google_cloud_support.egg-info/PKG-INFO` & `google-cloud-support-0.1.1/google_cloud_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-support
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Support API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-support-0.1.0/google_cloud_support.egg-info/SOURCES.txt` & `google-cloud-support-0.1.1/google_cloud_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/setup.py` & `google-cloud-support-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/tests/__init__.py` & `google-cloud-support-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/tests/unit/__init__.py` & `google-cloud-support-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-support-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/tests/unit/gapic/support_v2/__init__.py` & `google-cloud-support-0.1.1/tests/unit/gapic/support_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_case_attachment_service.py` & `google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_case_attachment_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1157,17 +1157,19 @@
                     attachment.Attachment(),
                     attachment.Attachment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_attachments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_case_service.py` & `google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_case_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1360,17 +1360,19 @@
                     case.Case(),
                     case.Case(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_cases(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1698,17 +1700,19 @@
                     case.Case(),
                     case.Case(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_cases(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2919,17 +2923,19 @@
                     case.CaseClassification(),
                     case.CaseClassification(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.search_case_classifications(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-support-0.1.0/tests/unit/gapic/support_v2/test_comment_service.py` & `google-cloud-support-0.1.1/tests/unit/gapic/support_v2/test_comment_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1114,17 +1114,19 @@
                     comment.Comment(),
                     comment.Comment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_comments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

