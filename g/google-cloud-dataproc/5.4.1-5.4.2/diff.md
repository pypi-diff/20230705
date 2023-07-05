# Comparing `tmp/google-cloud-dataproc-5.4.1.tar.gz` & `tmp/google-cloud-dataproc-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataproc-5.4.1.tar", last modified: Mon Mar 27 15:32:20 2023, max compression
+gzip compressed data, was "google-cloud-dataproc-5.4.2.tar", last modified: Wed Jul  5 15:07:01 2023, max compression
```

## Comparing `google-cloud-dataproc-5.4.1.tar` & `google-cloud-dataproc-5.4.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.353186 google-cloud-dataproc-5.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4620 2023-03-27 15:32:20.353186 google-cloud-dataproc-5.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3701 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.325185 google-cloud-dataproc-5.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.329185 google-cloud-dataproc-5.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.329185 google-cloud-dataproc-5.4.1/google/cloud/dataproc/
--rw-rw-r--   0 root         (0)     1003    15051 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.333185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/
--rw-rw-r--   0 root         (0)     1003    11355 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    15797 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.333185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.333185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    56139 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    64864 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     6171 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.333185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1566 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11320 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24453 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24765 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    64141 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.333185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/
--rw-rw-r--   0 root         (0)     1003      773 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    48391 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    58292 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5645 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.337185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1432 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9285 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22939 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23286 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    57650 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.337185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    80421 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    89325 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5692 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.337185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1460 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13322 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28663 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29113 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    80130 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.337185 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    67530 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    74242 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/client.py
--rw-rw-r--   0 root         (0)     1003     5512 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.341186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13052 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26071 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26482 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    72122 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.341186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/
--rw-rw-r--   0 root         (0)     1003      789 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/__init__.py
--rw-rw-r--   0 root         (0)     1003    46611 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/async_client.py
--rw-rw-r--   0 root         (0)     1003    55885 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.341186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/
--rw-rw-r--   0 root         (0)     1003     1496 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8990 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22495 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22822 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    54976 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.341186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/
--rw-rw-r--   0 root         (0)     1003      805 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    73251 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    82170 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/client.py
--rw-rw-r--   0 root         (0)     1003     6101 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.345186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/
--rw-rw-r--   0 root         (0)     1003     1552 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13977 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30186 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30591 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    78756 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.345186 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/
--rw-rw-r--   0 root         (0)     1003     7071 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16523 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/autoscaling_policies.py
--rw-rw-r--   0 root         (0)     1003    20835 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/batches.py
--rw-rw-r--   0 root         (0)     1003    81651 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/clusters.py
--rw-rw-r--   0 root         (0)     1003    56007 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/jobs.py
--rw-rw-r--   0 root         (0)     1003     6061 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/node_groups.py
--rw-rw-r--   0 root         (0)     1003     9425 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/operations.py
--rw-rw-r--   0 root         (0)     1003    27760 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/shared.py
--rw-rw-r--   0 root         (0)     1003    38762 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/workflow_templates.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/
--rw-r--r--   0 root         (0)     1003     4620 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5438 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:32:20.000000 google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:32:20.353186 google-cloud-dataproc-5.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2972 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.329185 google-cloud-dataproc-5.4.1/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.329185 google-cloud-dataproc-5.4.1/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0)     1003     1109 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/system/gapic/v1/test_system_cluster_controller_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:32:20.349186 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   221572 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py
--rw-rw-r--   0 root         (0)     1003   196734 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_batch_controller.py
--rw-rw-r--   0 root         (0)     1003   300884 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_cluster_controller.py
--rw-rw-r--   0 root         (0)     1003   256532 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_job_controller.py
--rw-rw-r--   0 root         (0)     1003   169636 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_node_group_controller.py
--rw-rw-r--   0 root         (0)     1003   332826 2023-03-27 15:30:15.000000 google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4620 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3701 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.643207 google-cloud-dataproc-5.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.643207 google-cloud-dataproc-5.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc/
+-rw-rw-r--   0 root         (0)     1003    15051 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/
+-rw-rw-r--   0 root         (0)     1003    11355 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15797 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56180 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    64864 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6171 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1566 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11320 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24453 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24765 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    64105 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/
+-rw-rw-r--   0 root         (0)     1003      773 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48423 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58292 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5645 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.651207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1432 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9285 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22939 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23286 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    57614 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/
+-rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    80455 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    89325 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5692 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1460 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13322 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28663 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29113 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    80094 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    67560 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74242 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/client.py
+-rw-rw-r--   0 root         (0)     1003     5512 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13052 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26071 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26482 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    72086 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.655207 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46647 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/async_client.py
+-rw-rw-r--   0 root         (0)     1003    55885 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/
+-rw-rw-r--   0 root         (0)     1003     1496 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8990 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22495 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22822 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    54940 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/
+-rw-rw-r--   0 root         (0)     1003      805 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73291 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    82170 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6101 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.659206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1552 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13977 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30186 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30591 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    78720 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/
+-rw-rw-r--   0 root         (0)     1003     7071 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16523 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/autoscaling_policies.py
+-rw-rw-r--   0 root         (0)     1003    20835 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/batches.py
+-rw-rw-r--   0 root         (0)     1003    81651 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/clusters.py
+-rw-rw-r--   0 root         (0)     1003    56007 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/jobs.py
+-rw-rw-r--   0 root         (0)     1003     6061 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/node_groups.py
+-rw-rw-r--   0 root         (0)     1003     9425 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/operations.py
+-rw-rw-r--   0 root         (0)     1003    27760 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/shared.py
+-rw-rw-r--   0 root         (0)     1003    38762 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/workflow_templates.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/
+-rw-r--r--   0 root         (0)     1003     4620 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5438 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:07:01.000000 google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2972 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.647207 google-cloud-dataproc-5.4.2/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0)     1003     1109 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/system/gapic/v1/test_system_cluster_controller_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.663206 google-cloud-dataproc-5.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:07:01.667206 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   220145 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py
+-rw-rw-r--   0 root         (0)     1003   196675 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_batch_controller.py
+-rw-rw-r--   0 root         (0)     1003   301083 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_cluster_controller.py
+-rw-rw-r--   0 root         (0)     1003   256059 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_job_controller.py
+-rw-rw-r--   0 root         (0)     1003   169636 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_node_group_controller.py
+-rw-rw-r--   0 root         (0)     1003   333025 2023-07-05 15:05:05.000000 google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py
```

### Comparing `google-cloud-dataproc-5.4.1/LICENSE` & `google-cloud-dataproc-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/MANIFEST.in` & `google-cloud-dataproc-5.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/PKG-INFO` & `google-cloud-dataproc-5.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc
-Version: 5.4.1
+Version: 5.4.2
 Summary: Google Cloud Dataproc API client library
 Home-page: https://github.com/googleapis/python-dataproc
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataproc-5.4.1/README.rst` & `google-cloud-dataproc-5.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc/gapic_version.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "5.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/gapic_metadata.json` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/gapic_version.py` & `google-cloud-dataproc-5.4.2/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "5.4.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/__init__.py` & `google-cloud-dataproc-5.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1364,15 +1364,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "AutoscalingPolicyServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/autoscaling_policy_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1084,15 +1084,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1184,15 +1184,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1286,15 +1286,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1189,15 +1189,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "BatchControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/pagers.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/batch_controller/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -941,15 +941,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1041,15 +1041,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1143,15 +1143,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1980,15 +1980,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ClusterControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/pagers.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/cluster_controller/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1519,15 +1519,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1619,15 +1619,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1721,15 +1721,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1693,15 +1693,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "JobControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/pagers.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/job_controller/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/job_controller/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1321,15 +1321,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1421,15 +1421,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1523,15 +1523,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1125,15 +1125,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "NodeGroupControllerAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/node_group_controller/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -869,15 +869,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -969,15 +969,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1071,15 +1071,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1769,15 +1769,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "WorkflowTemplateServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/client.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/services/workflow_template_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1459,15 +1459,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1559,15 +1559,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
@@ -1661,15 +1661,15 @@
 
             request, metadata = self._interceptor.pre_test_iam_permissions(
                 request, metadata
             )
             request_kwargs = json_format.MessageToDict(request)
             transcoded_request = path_template.transcode(http_options, **request_kwargs)
 
-            body = json.loads(json.dumps(transcoded_request["body"]))
+            body = json.dumps(transcoded_request["body"])
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
 
             # Jsonify the query params
             query_params = json.loads(json.dumps(transcoded_request["query_params"]))
 
             # Send the request
```

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/__init__.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/autoscaling_policies.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/autoscaling_policies.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/batches.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/batches.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/clusters.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/clusters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/jobs.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/jobs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/node_groups.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/node_groups.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/operations.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/operations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/shared.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/shared.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google/cloud/dataproc_v1/types/workflow_templates.py` & `google-cloud-dataproc-5.4.2/google/cloud/dataproc_v1/types/workflow_templates.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/PKG-INFO` & `google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc
-Version: 5.4.1
+Version: 5.4.2
 Summary: Google Cloud Dataproc API client library
 Home-page: https://github.com/googleapis/python-dataproc
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataproc-5.4.1/google_cloud_dataproc.egg-info/SOURCES.txt` & `google-cloud-dataproc-5.4.2/google_cloud_dataproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/setup.py` & `google-cloud-dataproc-5.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/tests/__init__.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/tests/system/gapic/v1/test_system_cluster_controller_v1.py` & `google-cloud-dataproc-5.4.2/tests/system/gapic/v1/test_system_cluster_controller_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/__init__.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_autoscaling_policy_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,19 +787,14 @@
     with mock.patch.object(
         type(client.transport.create_autoscaling_policy), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
         response = client.create_autoscaling_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == autoscaling_policies.CreateAutoscalingPolicyRequest()
@@ -1053,19 +1048,14 @@
     with mock.patch.object(
         type(client.transport.update_autoscaling_policy), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
         response = client.update_autoscaling_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == autoscaling_policies.UpdateAutoscalingPolicyRequest()
@@ -1309,19 +1299,14 @@
     with mock.patch.object(
         type(client.transport.get_autoscaling_policy), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
         response = client.get_autoscaling_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == autoscaling_policies.GetAutoscalingPolicyRequest()
@@ -1979,17 +1964,19 @@
                     autoscaling_policies.AutoscalingPolicy(),
                     autoscaling_policies.AutoscalingPolicy(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_autoscaling_policies(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2262,19 +2249,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = autoscaling_policies.AutoscalingPolicy.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2589,19 +2571,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = autoscaling_policies.AutoscalingPolicy.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -2890,19 +2867,14 @@
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = autoscaling_policies.AutoscalingPolicy(
             id="id_value",
             name="name_value",
-            basic_algorithm=autoscaling_policies.BasicAutoscalingAlgorithm(
-                yarn_config=autoscaling_policies.BasicYarnAutoscalingConfig(
-                    graceful_decommission_timeout=duration_pb2.Duration(seconds=751)
-                )
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = autoscaling_policies.AutoscalingPolicy.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_batch_controller.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_batch_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,17 +1011,14 @@
         call.return_value = batches.Batch(
             name="name_value",
             uuid="uuid_value",
             state=batches.Batch.State.PENDING,
             state_message="state_message_value",
             creator="creator_value",
             operation="operation_value",
-            pyspark_batch=batches.PySparkBatch(
-                main_python_file_uri="main_python_file_uri_value"
-            ),
         )
         response = client.get_batch(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == batches.GetBatchRequest()
@@ -1647,17 +1644,19 @@
                     batches.Batch(),
                     batches.Batch(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_batches(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -2339,17 +2338,14 @@
         return_value = batches.Batch(
             name="name_value",
             uuid="uuid_value",
             state=batches.Batch.State.PENDING,
             state_message="state_message_value",
             creator="creator_value",
             operation="operation_value",
-            pyspark_batch=batches.PySparkBatch(
-                main_python_file_uri="main_python_file_uri_value"
-            ),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = batches.Batch.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_cluster_controller.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_cluster_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -2509,17 +2509,19 @@
                     clusters.Cluster(),
                     clusters.Cluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_job_controller.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_job_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -735,15 +735,14 @@
     with mock.patch.object(type(client.transport.submit_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
         response = client.submit_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == jobs.SubmitJobRequest()
@@ -1260,15 +1259,14 @@
     with mock.patch.object(type(client.transport.get_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
         response = client.get_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == jobs.GetJobRequest()
@@ -1939,17 +1937,19 @@
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
@@ -1972,15 +1972,14 @@
     with mock.patch.object(type(client.transport.update_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
         response = client.update_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == jobs.UpdateJobRequest()
@@ -2137,15 +2136,14 @@
     with mock.patch.object(type(client.transport.cancel_job), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
         response = client.cancel_job(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == jobs.CancelJobRequest()
@@ -2646,15 +2644,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = jobs.Job.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3212,15 +3209,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = jobs.Job.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -3970,15 +3966,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = jobs.Job.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -4316,15 +4311,14 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = jobs.Job(
             driver_output_resource_uri="driver_output_resource_uri_value",
             driver_control_files_uri="driver_control_files_uri_value",
             job_uuid="job_uuid_value",
             done=True,
-            hadoop_job=jobs.HadoopJob(main_jar_file_uri="main_jar_file_uri_value"),
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = jobs.Job.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
```

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_node_group_controller.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_node_group_controller.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-5.4.1/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py` & `google-cloud-dataproc-5.4.2/tests/unit/gapic/dataproc_v1/test_workflow_template_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -2480,17 +2480,19 @@
                     workflow_templates.WorkflowTemplate(),
                     workflow_templates.WorkflowTemplate(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_workflow_templates(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

