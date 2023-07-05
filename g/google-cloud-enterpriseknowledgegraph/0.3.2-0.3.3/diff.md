# Comparing `tmp/google-cloud-enterpriseknowledgegraph-0.3.2.tar.gz` & `tmp/google-cloud-enterpriseknowledgegraph-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-enterpriseknowledgegraph-0.3.2.tar", last modified: Mon Mar 27 14:58:40 2023, max compression
+gzip compressed data, was "google-cloud-enterpriseknowledgegraph-0.3.3.tar", last modified: Wed Jul  5 15:52:57 2023, max compression
```

## Comparing `google-cloud-enterpriseknowledgegraph-0.3.2.tar` & `google-cloud-enterpriseknowledgegraph-0.3.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4762 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3820 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.936420 google-cloud-enterpriseknowledgegraph-0.3.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.936420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.940420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/
--rw-rw-r--   0 root         (0)     1003     2766 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.940420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/
--rw-rw-r--   0 root         (0)     1003     2479 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4466 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       98 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.940420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.940420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/
--rw-rw-r--   0 root         (0)     1003      837 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    53318 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    65313 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/client.py
--rw-rw-r--   0 root         (0)     1003     6366 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.940420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/
--rw-rw-r--   0 root         (0)     1003     1665 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10745 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22144 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22646 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    54083 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/
--rw-rw-r--   0 root         (0)     1003     2051 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2203 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/job_state.py
--rw-rw-r--   0 root         (0)     1003     2587 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/operation_metadata.py
--rw-rw-r--   0 root         (0)     1003    25014 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/
--rw-r--r--   0 root         (0)     1003     4762 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2290 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:40.000000 google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2983 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:40.944420 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/enterpriseknowledgegraph_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/enterpriseknowledgegraph_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   246874 2023-03-27 14:55:35.000000 google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/enterpriseknowledgegraph_v1/test_enterprise_knowledge_graph_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4762 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3820 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.001373 google-cloud-enterpriseknowledgegraph-0.3.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.001373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/
+-rw-rw-r--   0 root         (0)     1003     2766 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/
+-rw-rw-r--   0 root         (0)     1003     2479 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4466 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       98 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/
+-rw-rw-r--   0 root         (0)     1003      837 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53366 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    65313 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6366 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1665 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10745 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22144 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22646 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    54083 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.005373 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2051 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2203 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/job_state.py
+-rw-rw-r--   0 root         (0)     1003     2587 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/operation_metadata.py
+-rw-rw-r--   0 root         (0)     1003    25014 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/
+-rw-r--r--   0 root         (0)     1003     4762 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2290 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:52:56.000000 google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2983 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:52:57.009373 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/enterpriseknowledgegraph_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/enterpriseknowledgegraph_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   247073 2023-07-05 15:46:58.000000 google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/enterpriseknowledgegraph_v1/test_enterprise_knowledge_graph_service.py
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/LICENSE` & `google-cloud-enterpriseknowledgegraph-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/MANIFEST.in` & `google-cloud-enterpriseknowledgegraph-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/PKG-INFO` & `google-cloud-enterpriseknowledgegraph-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-enterpriseknowledgegraph
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Cloud Enterpriseknowledgegraph API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/README.rst` & `google-cloud-enterpriseknowledgegraph-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph/gapic_version.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/gapic_metadata.json` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/gapic_version.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/async_client.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1248,15 +1248,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "EnterpriseKnowledgeGraphServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/client.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/pagers.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/base.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc_asyncio.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/rest.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/services/enterprise_knowledge_graph_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/job_state.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/job_state.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/operation_metadata.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/operation_metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google/cloud/enterpriseknowledgegraph_v1/types/service.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/google/cloud/enterpriseknowledgegraph_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/PKG-INFO` & `google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-enterpriseknowledgegraph
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Cloud Enterpriseknowledgegraph API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/google_cloud_enterpriseknowledgegraph.egg-info/SOURCES.txt` & `google-cloud-enterpriseknowledgegraph-0.3.3/google_cloud_enterpriseknowledgegraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/setup.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/tests/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/enterpriseknowledgegraph_v1/__init__.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/enterpriseknowledgegraph_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-enterpriseknowledgegraph-0.3.2/tests/unit/gapic/enterpriseknowledgegraph_v1/test_enterprise_knowledge_graph_service.py` & `google-cloud-enterpriseknowledgegraph-0.3.3/tests/unit/gapic/enterpriseknowledgegraph_v1/test_enterprise_knowledge_graph_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1723,17 +1723,19 @@
                     service.EntityReconciliationJob(),
                     service.EntityReconciliationJob(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_entity_reconciliation_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

