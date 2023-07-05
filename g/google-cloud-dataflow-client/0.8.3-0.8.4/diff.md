# Comparing `tmp/google-cloud-dataflow-client-0.8.3.tar.gz` & `tmp/google-cloud-dataflow-client-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataflow-client-0.8.3.tar", last modified: Mon Mar 27 14:52:59 2023, max compression
+gzip compressed data, was "google-cloud-dataflow-client-0.8.4.tar", last modified: Wed Jul  5 15:16:45 2023, max compression
```

## Comparing `google-cloud-dataflow-client-0.8.3.tar` & `google-cloud-dataflow-client-0.8.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4564 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3637 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.835192 google-cloud-dataflow-client-0.8.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.835192 google-cloud-dataflow-client-0.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.839192 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/
--rw-rw-r--   0 root         (0)     1003     8007 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.839192 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/
--rw-rw-r--   0 root         (0)     1003     7053 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     9428 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.839192 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.839192 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/
--rw-rw-r--   0 root         (0)     1003      793 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    12688 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    21211 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.839192 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/
--rw-rw-r--   0 root         (0)     1003     1492 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6294 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11863 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12083 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12278 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.843193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/
--rw-rw-r--   0 root         (0)     1003      757 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003    33824 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/async_client.py
--rw-rw-r--   0 root         (0)     1003    43223 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/client.py
--rw-rw-r--   0 root         (0)     1003    10389 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.843193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8479 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19442 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19820 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    36767 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.843193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003    13690 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/async_client.py
--rw-rw-r--   0 root         (0)     1003    22243 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/client.py
--rw-rw-r--   0 root         (0)     1003     5841 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.843193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/
--rw-rw-r--   0 root         (0)     1003     1414 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6257 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12163 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12383 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12126 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.847193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003    21309 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/async_client.py
--rw-rw-r--   0 root         (0)     1003    30237 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/client.py
--rw-rw-r--   0 root         (0)     1003    10934 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.847193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7141 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14770 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15042 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    21886 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.847193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003    18767 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/async_client.py
--rw-rw-r--   0 root         (0)     1003    27635 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.847193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7127 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13911 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14190 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    21234 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.847193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/
--rw-rw-r--   0 root         (0)     1003      777 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    19005 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27889 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.851193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7116 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14002 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14281 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22022 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.851193 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     5912 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32670 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/environment.py
--rw-rw-r--   0 root         (0)     1003    50792 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/jobs.py
--rw-rw-r--   0 root         (0)     1003    12673 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/messages.py
--rw-rw-r--   0 root         (0)     1003    19950 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/metrics.py
--rw-rw-r--   0 root         (0)     1003     7051 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/snapshots.py
--rw-rw-r--   0 root         (0)     1003    15111 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/streaming.py
--rw-rw-r--   0 root         (0)     1003    36477 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/templates.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/
--rw-r--r--   0 root         (0)     1003     4564 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5425 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:52:59.000000 google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2946 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:52:59.855194 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003    65194 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_flex_templates_service.py
--rw-rw-r--   0 root         (0)     1003   185497 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_jobs_v1_beta3.py
--rw-rw-r--   0 root         (0)     1003    73163 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_messages_v1_beta3.py
--rw-rw-r--   0 root         (0)     1003   102572 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_metrics_v1_beta3.py
--rw-rw-r--   0 root         (0)     1003    85790 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_snapshots_v1_beta3.py
--rw-rw-r--   0 root         (0)     1003    90636 2023-03-27 14:50:26.000000 google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_templates_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.838859 google-cloud-dataflow-client-0.8.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4564 2023-07-05 15:16:45.838859 google-cloud-dataflow-client-0.8.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3637 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.818858 google-cloud-dataflow-client-0.8.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.818858 google-cloud-dataflow-client-0.8.4/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/
+-rw-rw-r--   0 root         (0)     1003     8007 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     7053 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9428 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/
+-rw-rw-r--   0 root         (0)     1003      793 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12725 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    21211 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1492 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6294 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11863 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12083 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12278 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.822858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/
+-rw-rw-r--   0 root         (0)     1003      757 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33852 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43223 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/client.py
+-rw-rw-r--   0 root         (0)     1003    10389 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.826858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8479 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19442 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19820 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    36767 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.826858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13722 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22243 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/client.py
+-rw-rw-r--   0 root         (0)     1003     5841 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.826858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6257 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12163 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12383 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12126 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.826858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21340 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/async_client.py
+-rw-rw-r--   0 root         (0)     1003    30237 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/client.py
+-rw-rw-r--   0 root         (0)     1003    10934 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.830858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7141 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14770 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15042 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    21886 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.830858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18800 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27635 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.830858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7127 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13911 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14190 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    21234 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.830858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/
+-rw-rw-r--   0 root         (0)     1003      777 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19038 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27889 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.830858 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7116 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14002 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14281 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22022 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     5912 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32670 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/environment.py
+-rw-rw-r--   0 root         (0)     1003    50792 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/jobs.py
+-rw-rw-r--   0 root         (0)     1003    12673 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/messages.py
+-rw-rw-r--   0 root         (0)     1003    19950 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/metrics.py
+-rw-rw-r--   0 root         (0)     1003     7051 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/snapshots.py
+-rw-rw-r--   0 root         (0)     1003    15111 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/streaming.py
+-rw-rw-r--   0 root         (0)     1003    36477 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/templates.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/
+-rw-r--r--   0 root         (0)     1003     4564 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5425 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:16:45.000000 google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:16:45.838859 google-cloud-dataflow-client-0.8.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2946 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:16:45.834859 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003    65194 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_flex_templates_service.py
+-rw-rw-r--   0 root         (0)     1003   185895 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_jobs_v1_beta3.py
+-rw-rw-r--   0 root         (0)     1003    73362 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_messages_v1_beta3.py
+-rw-rw-r--   0 root         (0)     1003   102970 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_metrics_v1_beta3.py
+-rw-rw-r--   0 root         (0)     1003    85790 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_snapshots_v1_beta3.py
+-rw-rw-r--   0 root         (0)     1003    90636 2023-07-05 15:14:23.000000 google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_templates_service.py
```

### Comparing `google-cloud-dataflow-client-0.8.3/LICENSE` & `google-cloud-dataflow-client-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/MANIFEST.in` & `google-cloud-dataflow-client-0.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/PKG-INFO` & `google-cloud-dataflow-client-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataflow-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Google Cloud Dataflow Client API client library
 Home-page: https://github.com/googleapis/python-dataflow-client
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-dataflow-client-0.8.3/README.rst` & `google-cloud-dataflow-client-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow/gapic_version.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow/gapic_version.py`

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
-__version__ = "0.8.3"  # {x-release-please-version}
+__version__ = "0.8.4"  # {x-release-please-version}
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/gapic_metadata.json` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/gapic_version.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/gapic_version.py`

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
-__version__ = "0.8.3"  # {x-release-please-version}
+__version__ = "0.8.4"  # {x-release-please-version}
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "FlexTemplatesServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/flex_templates_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "JobsV1Beta3AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/pagers.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/jobs_v1_beta3/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MessagesV1Beta3AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/pagers.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/messages_v1_beta3/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "MetricsV1Beta3AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/pagers.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/metrics_v1_beta3/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "SnapshotsV1Beta3AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/snapshots_v1_beta3/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/async_client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "TemplatesServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/client.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/base.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc_asyncio.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/services/templates_service/transports/rest.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/services/templates_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/__init__.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/environment.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/environment.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/jobs.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/jobs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/messages.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/messages.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/metrics.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/metrics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/snapshots.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/snapshots.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/streaming.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/streaming.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google/cloud/dataflow_v1beta3/types/templates.py` & `google-cloud-dataflow-client-0.8.4/google/cloud/dataflow_v1beta3/types/templates.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/PKG-INFO` & `google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataflow-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Google Cloud Dataflow Client API client library
 Home-page: https://github.com/googleapis/python-dataflow-client
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-dataflow-client-0.8.3/google_cloud_dataflow_client.egg-info/SOURCES.txt` & `google-cloud-dataflow-client-0.8.4/google_cloud_dataflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/setup.py` & `google-cloud-dataflow-client-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/__init__.py` & `google-cloud-dataflow-client-0.8.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/__init__.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/__init__.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/__init__.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_flex_templates_service.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_flex_templates_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_jobs_v1_beta3.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_jobs_v1_beta3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1631,17 +1631,19 @@
                     jobs.Job(),
                     jobs.Job(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1987,17 +1989,19 @@
                     jobs.Job(),
                     jobs.Job(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.aggregated_list_jobs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_messages_v1_beta3.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_messages_v1_beta3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1086,17 +1086,19 @@
                     messages.JobMessage(),
                     messages.JobMessage(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_job_messages(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_metrics_v1_beta3.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_metrics_v1_beta3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1210,17 +1210,19 @@
                     metrics.StageSummary(),
                     metrics.StageSummary(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.get_job_execution_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -1580,17 +1582,19 @@
                     metrics.WorkerDetails(),
                     metrics.WorkerDetails(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.get_stage_execution_details(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_snapshots_v1_beta3.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_snapshots_v1_beta3.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataflow-client-0.8.3/tests/unit/gapic/dataflow_v1beta3/test_templates_service.py` & `google-cloud-dataflow-client-0.8.4/tests/unit/gapic/dataflow_v1beta3/test_templates_service.py`

 * *Files identical despite different names*

