# Comparing `tmp/google-cloud-run-0.8.0.tar.gz` & `tmp/google-cloud-run-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-run-0.8.0.tar", last modified: Wed May 31 18:48:12 2023, max compression
+gzip compressed data, was "google-cloud-run-0.8.1.tar", last modified: Wed Jul  5 15:19:42 2023, max compression
```

## Comparing `google-cloud-run-0.8.0.tar` & `google-cloud-run-0.8.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4478 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3587 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.357279 google-cloud-run-0.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.357279 google-cloud-run-0.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run/
--rw-rw-r--   0 root         (0)     1003     4984 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/
--rw-rw-r--   0 root         (0)     1003     4323 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    11056 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/
--rw-rw-r--   0 root         (0)     1003      753 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32592 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/async_client.py
--rw-rw-r--   0 root         (0)     1003    44778 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/client.py
--rw-rw-r--   0 root         (0)     1003     5724 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.361281 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/
--rw-rw-r--   0 root         (0)     1003     1344 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8120 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17896 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18214 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38178 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/
--rw-rw-r--   0 root         (0)     1003      729 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/__init__.py
--rw-rw-r--   0 root         (0)     1003    62817 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/async_client.py
--rw-rw-r--   0 root         (0)     1003    75369 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/client.py
--rw-rw-r--   0 root         (0)     1003     5454 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/
--rw-rw-r--   0 root         (0)     1003     1260 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10638 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24322 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24783 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    74496 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/
--rw-rw-r--   0 root         (0)     1003      749 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/__init__.py
--rw-rw-r--   0 root         (0)     1003    32604 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/async_client.py
--rw-rw-r--   0 root         (0)     1003    45650 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/client.py
--rw-rw-r--   0 root         (0)     1003     5679 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/
--rw-rw-r--   0 root         (0)     1003     1330 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8080 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17882 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18199 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    38188 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.365282 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/
--rw-rw-r--   0 root         (0)     1003      745 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/__init__.py
--rw-rw-r--   0 root         (0)     1003    61130 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/async_client.py
--rw-rw-r--   0 root         (0)     1003    74285 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/client.py
--rw-rw-r--   0 root         (0)     1003     5634 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/
--rw-rw-r--   0 root         (0)     1003     1316 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11098 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23863 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24318 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    70819 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/
--rw-rw-r--   0 root         (0)     1003      733 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/__init__.py
--rw-rw-r--   0 root         (0)     1003    27294 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/async_client.py
--rw-rw-r--   0 root         (0)     1003    40166 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/client.py
--rw-rw-r--   0 root         (0)     1003     5499 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.369283 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/
--rw-rw-r--   0 root         (0)     1003     1274 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7324 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15918 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16151 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30148 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/google/cloud/run_v2/types/
--rw-rw-r--   0 root         (0)     1003     3581 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10542 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/condition.py
--rw-rw-r--   0 root         (0)     1003    13565 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/execution.py
--rw-rw-r--   0 root         (0)     1003     4307 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/execution_template.py
--rw-rw-r--   0 root         (0)     1003    18011 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/job.py
--rw-rw-r--   0 root         (0)     1003    23222 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/k8s_min.py
--rw-rw-r--   0 root         (0)     1003    14333 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/revision.py
--rw-rw-r--   0 root         (0)     1003     6438 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/revision_template.py
--rw-rw-r--   0 root         (0)     1003    19791 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/service.py
--rw-rw-r--   0 root         (0)     1003    13995 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/task.py
--rw-rw-r--   0 root         (0)     1003     4207 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/task_template.py
--rw-rw-r--   0 root         (0)     1003     3750 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/traffic_target.py
--rw-rw-r--   0 root         (0)     1003     5608 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/google/cloud/run_v2/types/vendor_settings.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/google_cloud_run.egg-info/
--rw-r--r--   0 root         (0)     1003     4478 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3882 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-05-31 18:48:12.000000 google-cloud-run-0.8.0/google_cloud_run.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2952 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.373284 google-cloud-run-0.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 18:48:12.377286 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   153250 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_executions.py
--rw-rw-r--   0 root         (0)     1003   261385 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_jobs.py
--rw-rw-r--   0 root         (0)     1003   150387 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_revisions.py
--rw-rw-r--   0 root         (0)     1003   246727 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_services.py
--rw-rw-r--   0 root         (0)     1003   131193 2023-05-31 18:46:03.000000 google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.059746 google-cloud-run-0.8.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4478 2023-07-05 15:19:42.059746 google-cloud-run-0.8.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3587 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.039753 google-cloud-run-0.8.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.039753 google-cloud-run-0.8.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.043752 google-cloud-run-0.8.1/google/cloud/run/
+-rw-rw-r--   0 root         (0)     1003     4984 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.043752 google-cloud-run-0.8.1/google/cloud/run_v2/
+-rw-rw-r--   0 root         (0)     1003     4323 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11056 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.043752 google-cloud-run-0.8.1/google/cloud/run_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.043752 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/
+-rw-rw-r--   0 root         (0)     1003      753 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32619 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44778 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/client.py
+-rw-rw-r--   0 root         (0)     1003     5724 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.043752 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/
+-rw-rw-r--   0 root         (0)     1003     1344 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8120 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17896 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18214 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38166 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.047750 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/
+-rw-rw-r--   0 root         (0)     1003      729 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62838 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75369 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/client.py
+-rw-rw-r--   0 root         (0)     1003     5454 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.047750 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/
+-rw-rw-r--   0 root         (0)     1003     1260 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10638 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24322 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24783 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    74484 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.047750 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/
+-rw-rw-r--   0 root         (0)     1003      749 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32630 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/async_client.py
+-rw-rw-r--   0 root         (0)     1003    45650 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/client.py
+-rw-rw-r--   0 root         (0)     1003     5679 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.047750 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8080 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17882 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18199 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    38176 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.051749 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/
+-rw-rw-r--   0 root         (0)     1003      745 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61155 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74285 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/client.py
+-rw-rw-r--   0 root         (0)     1003     5634 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.051749 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/
+-rw-rw-r--   0 root         (0)     1003     1316 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11098 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23863 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24318 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    70807 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.051749 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/
+-rw-rw-r--   0 root         (0)     1003      733 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27316 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40166 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/client.py
+-rw-rw-r--   0 root         (0)     1003     5499 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.051749 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/
+-rw-rw-r--   0 root         (0)     1003     1274 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7324 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15918 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16151 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30136 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.055748 google-cloud-run-0.8.1/google/cloud/run_v2/types/
+-rw-rw-r--   0 root         (0)     1003     3581 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10542 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/condition.py
+-rw-rw-r--   0 root         (0)     1003    13565 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/execution.py
+-rw-rw-r--   0 root         (0)     1003     4307 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/execution_template.py
+-rw-rw-r--   0 root         (0)     1003    18011 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/job.py
+-rw-rw-r--   0 root         (0)     1003    23222 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/k8s_min.py
+-rw-rw-r--   0 root         (0)     1003    14333 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/revision.py
+-rw-rw-r--   0 root         (0)     1003     6438 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/revision_template.py
+-rw-rw-r--   0 root         (0)     1003    19791 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/service.py
+-rw-rw-r--   0 root         (0)     1003    13995 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/task.py
+-rw-rw-r--   0 root         (0)     1003     4207 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/task_template.py
+-rw-rw-r--   0 root         (0)     1003     3750 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/traffic_target.py
+-rw-rw-r--   0 root         (0)     1003     5608 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/google/cloud/run_v2/types/vendor_settings.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.055748 google-cloud-run-0.8.1/google_cloud_run.egg-info/
+-rw-r--r--   0 root         (0)     1003     4478 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3882 2023-07-05 15:19:42.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:19:41.000000 google-cloud-run-0.8.1/google_cloud_run.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:19:42.059746 google-cloud-run-0.8.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2952 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.055748 google-cloud-run-0.8.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.055748 google-cloud-run-0.8.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.055748 google-cloud-run-0.8.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:19:42.059746 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   153449 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_executions.py
+-rw-rw-r--   0 root         (0)     1003   261584 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_jobs.py
+-rw-rw-r--   0 root         (0)     1003   150586 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_revisions.py
+-rw-rw-r--   0 root         (0)     1003   246926 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_services.py
+-rw-rw-r--   0 root         (0)     1003   131392 2023-07-05 15:17:42.000000 google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_tasks.py
```

### Comparing `google-cloud-run-0.8.0/LICENSE` & `google-cloud-run-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/MANIFEST.in` & `google-cloud-run-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/PKG-INFO` & `google-cloud-run-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.8.0
+Version: 0.8.1
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-run-0.8.0/README.rst` & `google-cloud-run-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run/gapic_version.py` & `google-cloud-run-0.8.1/google/cloud/run/gapic_version.py`

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
-__version__ = "0.8.0"  # {x-release-please-version}
+__version__ = "0.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/gapic_metadata.json` & `google-cloud-run-0.8.1/google/cloud/run_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/gapic_version.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/gapic_version.py`

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
-__version__ = "0.8.0"  # {x-release-please-version}
+__version__ = "0.8.1"  # {x-release-please-version}
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/async_client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -792,15 +792,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ExecutionsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/pagers.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/base.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/executions/transports/rest.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/executions/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -940,15 +940,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_wait_operation(request, metadata)
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

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/async_client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1538,15 +1538,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "JobsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/pagers.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/base.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/jobs/transports/rest.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/jobs/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1869,15 +1869,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_wait_operation(request, metadata)
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

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/async_client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,15 +791,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RevisionsAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/pagers.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/base.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/revisions/transports/rest.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/revisions/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,15 +939,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_wait_operation(request, metadata)
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

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/async_client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1465,15 +1465,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "ServicesAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/pagers.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/base.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/grpc_asyncio.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/services/transports/rest.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/services/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1755,15 +1755,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_wait_operation(request, metadata)
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

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/async_client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,15 +663,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "TasksAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/client.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/pagers.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/base.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/services/tasks/transports/rest.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/services/tasks/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,15 +738,15 @@
                 },
             ]
 
             request, metadata = self._interceptor.pre_wait_operation(request, metadata)
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

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/__init__.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/condition.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/condition.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/execution.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/execution.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/execution_template.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/execution_template.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/job.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/job.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/k8s_min.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/k8s_min.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/revision.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/revision.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/revision_template.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/revision_template.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/service.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/task.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/task.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/task_template.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/task_template.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/traffic_target.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/traffic_target.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google/cloud/run_v2/types/vendor_settings.py` & `google-cloud-run-0.8.1/google/cloud/run_v2/types/vendor_settings.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/google_cloud_run.egg-info/PKG-INFO` & `google-cloud-run-0.8.1/google_cloud_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-run
-Version: 0.8.0
+Version: 0.8.1
 Summary: Google Cloud Run API client library
 Home-page: https://github.com/googleapis/python-run
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-run-0.8.0/google_cloud_run.egg-info/SOURCES.txt` & `google-cloud-run-0.8.1/google_cloud_run.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/setup.py` & `google-cloud-run-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/tests/__init__.py` & `google-cloud-run-0.8.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/tests/unit/__init__.py` & `google-cloud-run-0.8.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/__init__.py` & `google-cloud-run-0.8.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/__init__.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_executions.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_executions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1392,17 +1392,19 @@
                     execution.Execution(),
                     execution.Execution(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_executions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_jobs.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1591,17 +1591,19 @@
                     job.Job(),
                     job.Job(),
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
```

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_revisions.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_revisions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,17 +1326,19 @@
                     revision.Revision(),
                     revision.Revision(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_revisions(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_services.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -1529,17 +1529,19 @@
                     service.Service(),
                     service.Service(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_services(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-run-0.8.0/tests/unit/gapic/run_v2/test_tasks.py` & `google-cloud-run-0.8.1/tests/unit/gapic/run_v2/test_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1364,17 +1364,19 @@
                     task.Task(),
                     task.Task(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_tasks(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

