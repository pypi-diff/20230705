# Comparing `tmp/globus-compute-endpoint-2.2.1.tar.gz` & `tmp/globus-compute-endpoint-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.2.1.tar", last modified: Fri Jun 23 01:03:56 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.2.3a0.tar", last modified: Wed Jul  5 15:36:21 2023, max compression
```

## Comparing `globus-compute-endpoint-2.2.1.tar` & `globus-compute-endpoint-2.2.3a0.tar`

### file list

```diff
@@ -1,82 +1,98 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.558050 globus-compute-endpoint-2.2.1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       83 2023-06-21 21:23:44.000000 globus-compute-endpoint-2.2.1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1838 2023-06-23 01:03:56.558134 globus-compute-endpoint-2.2.1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.1/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.544078 globus-compute-endpoint-2.2.1/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.547356 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.548441 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)      117 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.yaml
--rw-r--r--   0 lei        (501) staff       (20)     3447 2023-06-23 00:56:17.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.549176 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.549558 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.550769 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/
--rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/helper.py
--rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/process_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.550911 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.555338 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8499 2023-06-21 18:50:27.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.555614 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.556322 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.557235 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      804 2023-06-23 00:59:13.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.544803 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1838 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     3152 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      342 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-23 01:03:56.000000 globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-23 01:03:56.558447 globus-compute-endpoint-2.2.1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3683 2023-06-23 00:59:09.000000 globus-compute-endpoint-2.2.1/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-23 01:03:56.557776 globus-compute-endpoint-2.2.1/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.1/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.1/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.1/tests/utils.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.743182 globus-compute-endpoint-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       83 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     1840 2023-07-05 15:36:21.743282 globus-compute-endpoint-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      871 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/PyPI.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.723544 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)      131 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    16673 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.726804 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.728630 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 yadu       (501) staff       (20)       41 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6542 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 yadu       (501) staff       (20)      766 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 yadu       (501) staff       (20)      117 2023-06-16 15:43:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-r--r--   0 yadu       (501) staff       (20)     3522 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7326 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 yadu       (501) staff       (20)    27495 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 yadu       (501) staff       (20)    20355 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)    23242 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3075 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.730265 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 yadu       (501) staff       (20)      307 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      689 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11834 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3068 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 yadu       (501) staff       (20)    14076 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5184 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7275 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.730713 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 yadu       (501) staff       (20)     1017 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      110 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.731965 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/
+-rw-r--r--   0 yadu       (501) staff       (20)      241 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6257 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3721 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 yadu       (501) staff       (20)     4608 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/helper.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.735555 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1943 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/container_sched.py
+-rw-r--r--   0 yadu       (501) staff       (20)    34568 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/engine.py
+-rw-r--r--   0 yadu       (501) staff       (20)    49294 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange.py
+-rw-r--r--   0 yadu       (501) staff       (20)     9712 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 yadu       (501) staff       (20)      267 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 yadu       (501) staff       (20)    36121 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)     9295 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/messages.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7216 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker.py
+-rw-r--r--   0 yadu       (501) staff       (20)    19094 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker_map.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5427 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3715 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2020 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 yadu       (501) staff       (20)      220 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.735773 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/
+-rw-r--r--   0 yadu       (501) staff       (20)      141 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.736521 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      422 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 yadu       (501) staff       (20)     8499 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.737105 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/
+-rw-r--r--   0 yadu       (501) staff       (20)      115 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.738412 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    12926 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 yadu       (501) staff       (20)       50 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.740077 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 yadu       (501) staff       (20)      280 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7018 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5470 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6145 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1610 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 yadu       (501) staff       (20)      806 2023-07-05 15:23:57.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.724649 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     1840 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     3729 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      353 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      344 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       30 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-05 15:36:21.743746 globus-compute-endpoint-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     3679 2023-07-05 15:25:36.000000 globus-compute-endpoint-2.2.3a0/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.740942 globus-compute-endpoint-2.2.3a0/tests/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/tests/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2709 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/tests/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.741427 globus-compute-endpoint-2.2.3a0/tests/integration/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11428 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/tests/integration/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.741806 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1679 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.742133 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.742964 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2256 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2275 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1273 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1126 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/mock_executors.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2925 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.2.1/LICENSE` & `globus-compute-endpoint-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/PKG-INFO` & `globus-compute-endpoint-2.2.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.1
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.1/PyPI.md` & `globus-compute-endpoint-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,14 +91,20 @@
     multi_tenant : bool | None
         Designates the endpoint as a multi-tenant endpoint
         Default: None
 
     display_name : str | None
         The display name for the endpoint.  If None, defaults to name
         Default: None
+
+    endpoint_setup : str | None
+        Command or commands to be run during the endpoint initialization process.
+
+    endpoint_teardown : str | None
+        Command or commands to be run during the endpoint shutdown process.
     """
 
     def __init__(
         self,
         # Execution backed
         executors: list = _DEFAULT_EXECUTORS,
         # Connection info
@@ -108,14 +114,16 @@
         allowed_functions: list[str] | None = None,
         # Tuning info
         heartbeat_period=30,
         heartbeat_threshold=120,
         idle_heartbeats_soft=0,
         idle_heartbeats_hard=5760,  # Two days, divided by `heartbeat_period`
         detach_endpoint=True,
+        endpoint_setup: str | None = None,
+        endpoint_teardown: str | None = None,
         # Misc info
         display_name: str | None = None,
         # Logging info
         log_dir=None,
         stdout="./endpoint.log",
         stderr="./endpoint.log",
         **kwargs,
@@ -154,14 +162,17 @@
         # Tuning info
         self.heartbeat_period = heartbeat_period
         self.heartbeat_threshold = heartbeat_threshold
         self.idle_heartbeats_soft = int(max(0, idle_heartbeats_soft))
         self.idle_heartbeats_hard = int(max(0, idle_heartbeats_hard))
         self.detach_endpoint = detach_endpoint
 
+        self.endpoint_setup = endpoint_setup
+        self.endpoint_teardown = endpoint_teardown
+
         # Logging info
         self.log_dir = log_dir
         self.stdout = stdout
         self.stderr = stderr
 
         # Misc info
         self.display_name = display_name
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,16 @@
     multi_tenant: t.Optional[bool]
     allowed_functions: t.Optional[t.List[str]]
     heartbeat_period: t.Optional[int]
     heartbeat_threshold: t.Optional[int]
     idle_heartbeats_soft: t.Optional[int]
     idle_heartbeats_hard: t.Optional[int]
     detach_endpoint: t.Optional[bool]
+    endpoint_setup: t.Optional[str]
+    endpoint_teardown: t.Optional[str]
     log_dir: t.Optional[str]
     stdout: t.Optional[str]
     stderr: t.Optional[str]
 
     _validate_engine = _validate_params("engine")
 
     def dict(self, *args, **kwargs):
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import pathlib
 import pwd
 import re
 import shutil
 import signal
 import socket
+import subprocess
 import sys
 import typing
 import uuid
 
 import daemon
 import daemon.pidfile
 import psutil
@@ -261,14 +262,17 @@
             else:
                 log.info(
                     "A prior Endpoint instance appears to have been terminated without "
                     "proper cleanup. Cleaning up now."
                 )
                 Endpoint.pidfile_cleanup(endpoint_dir)
 
+        if endpoint_config.endpoint_setup:
+            Endpoint._run_command("endpoint_setup", endpoint_config.endpoint_setup)
+
         result_store = ResultStore(endpoint_dir=endpoint_dir)
 
         # Create a daemon context
         # If we are running a full detached daemon then we will send the output to
         # log files, otherwise we can piggy back on our stdout
         if endpoint_config.detach_endpoint:
             stdout: typing.TextIO = open(
@@ -470,14 +474,20 @@
             Endpoint.pidfile_cleanup(endpoint_dir)
             return
         elif not ep_status["exists"]:
             log.info(f"Endpoint <{ep_name}> is not active.")
             return
 
         log.debug(f"{ep_name} has a daemon.pid file")
+
+        if endpoint_config and endpoint_config.endpoint_teardown:
+            Endpoint._run_command(
+                "endpoint_teardown", endpoint_config.endpoint_teardown
+            )
+
         pid = int(pid_path.read_text().strip())
         try:
             log.debug(f"Signaling process: {pid}")
             # For all the processes, including the deamon and its descendants,
             # send SIGTERM, wait for 10s, and then SIGKILL any still alive.
             grace_period_s = 10
             parent = psutil.Process(pid)
@@ -721,7 +731,20 @@
         except Exception as e:
             log.warning(
                 f"Error when serializing config ({type(e).__name__}). Ignoring."
             )
             log.debug("Config serialization exception details", exc_info=e)
 
         return metadata
+
+    @staticmethod
+    def _run_command(name: str, command: str):
+        log.info(f"running {name} command: {command}")
+        completed_process = subprocess.run(command, shell=True, capture_output=True)
+
+        log.info(f"{name} stdout: {str(completed_process.stdout)}")
+        log.info(f"{name} stderr: {str(completed_process.stderr)}")
+
+        returncode = completed_process.returncode
+        if returncode:
+            log.error(f"{name} failed with exit code {returncode}")
+            exit(os.EX_CONFIG)
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import platform
 import queue
 import random
 import signal
 import sys
 import threading
 import time
-import typing as t
 
 # multiprocessing.Event is a method, not a class
 # to annotate, we need the "real" class
 # see: https://github.com/python/typeshed/issues/4266
 from multiprocessing.synchronize import Event as EventType
 
 import globus_compute_endpoint.endpoint.config
@@ -24,30 +23,24 @@
 from globus_compute_common.messagepack.message_types import (
     EPStatusReport,
     Result,
     ResultErrorDetails,
     Task,
 )
 from globus_compute_endpoint import __version__ as funcx_endpoint_version
-from globus_compute_endpoint.endpoint.messages_compat import (
-    convert_to_internaltask,
-    try_convert_to_messagepack,
-)
 from globus_compute_endpoint.endpoint.rabbit_mq import (
     ResultQueuePublisher,
     TaskQueueSubscriber,
 )
 from globus_compute_endpoint.endpoint.result_store import ResultStore
+from globus_compute_endpoint.engines.base import GlobusComputeEngineBase
 from globus_compute_endpoint.exception_handling import get_result_error_details
 from globus_compute_sdk import __version__ as funcx_sdk_version
 from parsl.version import VERSION as PARSL_VERSION
 
-if t.TYPE_CHECKING:
-    from globus_compute_endpoint.executors import HighThroughputExecutor
-
 log = logging.getLogger(__name__)
 
 
 class EndpointInterchange:
     """Interchange is a task orchestrator for distributed systems.
 
     1. Asynchronously queue large volume of tasks (>100K)
@@ -134,19 +127,20 @@
             "dir": os.getcwd(),
         }
         log.info(f"Platform info: {self.current_platform}")
 
         self.results_passthrough: queue.Queue[
             dict[str, bytes | str | None]
         ] = queue.Queue()
-        self.executor: HighThroughputExecutor = self.config.executors[0]
+        # Rename self.executor -> self.engine in second round
+        self.executor: GlobusComputeEngineBase = self.config.executors[0]
         self._test_start = False
 
-    def start_executor(self):
-        log.info("Starting Executor")
+    def start_engine(self):
+        log.info("Starting Engine")
         self.executor.start(
             results_passthrough=self.results_passthrough,
             endpoint_id=self.endpoint_id,
             run_dir=self.logdir,
         )
 
     def migrate_tasks_to_internal(
@@ -248,15 +242,15 @@
             ).start()
 
         log.info("Starting EndpointInterchange")
 
         # NOTE: currently we only start the executors once because
         # the current behavior is to keep them running decoupled while
         # the endpoint is waiting for reconnection
-        self.start_executor()
+        self.start_engine()
 
         while not self._kill_event.is_set():
             if self._reconnect_fail_counter >= self.reconnect_attempt_limit:
                 log.critical(
                     f"Failed {self._reconnect_fail_counter} consecutive times."
                     "  Shutting down."
                 )
@@ -358,15 +352,14 @@
                 log.debug("Exit process-stored-results thread.")
 
             def process_pending_tasks():
                 # Pull tasks from upstream (RMQ) and send them down the ZMQ pipe to the
                 # globus-compute-manager.  In terms of shutting down (or "rebooting")
                 # gracefully, iterate once a second whether or not a task has arrived.
                 nonlocal num_tasks_forwarded
-                ctype = executor.container_type
                 while not self._quiesce_event.is_set():
                     if self.time_to_quit:
                         self.stop()
                         continue  # nominally == break; but let event do it
                     try:
                         incoming_task = self.pending_task_queue.get(timeout=1)
                         task_msg = unpack(incoming_task)
@@ -377,27 +370,29 @@
                         continue
 
                     except Exception:
                         log.exception("Unhandled error processing incoming task")
                         continue
 
                     try:
-                        task = convert_to_internaltask(task_msg, ctype)
-                        executor.submit_raw(task)
+                        executor.submit(
+                            task_id=task_msg.task_id, packed_task=incoming_task
+                        )
                         num_tasks_forwarded += 1  # Safe given GIL
 
                     except Exception as exc:
                         log.exception(f"Failed to process {task_msg.task_id}")
                         code, msg = get_result_error_details()
                         failed_result = Result(
                             task_id=task_msg.task_id,
                             data=f"Failed to start task: {exc}",
                             error_details=ResultErrorDetails(
                                 code=code, user_message=msg
                             ),
+                            task_statuses=[],
                         )
                         res = {
                             "task_id": task_msg.task_id,
                             "message": pack(failed_result),
                         }
                         self.results_passthrough.put(res)
 
@@ -407,79 +402,45 @@
                 # Forward incoming results from the globus-compute-manager to the
                 # Globus Compute services. For graceful handling of shutdown
                 # (or "reboot"), wait up to a second or incoming results before
                 # iterating the loop regardless.
                 nonlocal num_results_forwarded
                 while not self._quiesce_event.is_set():
                     try:
-                        result = self.results_passthrough.get(timeout=1)
-                        task_id: str | None = result["task_id"]
-                        packed_result: bytes = result["message"]
+                        packed_message = self.results_passthrough.get(timeout=1)
+                        unpacked_message = unpack(packed_message)
 
                     except queue.Empty:
                         # Empty queue!  Let's see if we have any prior results to send
                         continue
 
                     except Exception as exc:
                         log.warning(
                             f"Invalid message received: no task_id.  Ignoring. {exc}"
                         )
                         continue
 
-                    try:
-                        # This either works or it doesn't; if it doesn't, then
-                        # serialize an exception and send _that_
-                        # will be a packed EPStatusReport or Result
-                        message = try_convert_to_messagepack(packed_result)
-
-                    except Exception as exc:
-                        if not task_id:
-                            log.exception(
-                                "Unable to parse result message; no task id, so"
-                                " likely a garbled EPStatusReport; ignoring"
-                            )
-                            continue
-
-                        log.exception(
-                            f"Unable to parse result message for task {task_id}."
-                            "   Marking task as failed."
-                        )
-
-                        err = f"[Task ID: {task_id}] ({exc.__class__.__name__}) {exc}"
-
-                        kwargs = {
-                            "task_id": task_id,
-                            "data": err,
-                            "error_details": ResultErrorDetails(
-                                code=0,
-                                user_message=(
-                                    "Endpoint failed to serialize."
-                                    f"  Exception text: {exc}"
-                                ),
-                            ),
-                        }
-                        message = pack(Result(**kwargs))
-
-                    if task_id:
-                        log.debug(f"Forwarding result for task {task_id}")
+                    task_id = None
+                    if isinstance(unpacked_message, Result):
+                        num_results_forwarded += 1
+                        task_id = unpacked_message.task_id
+                        log.debug("Forwarding result for task: %s", task_id)
 
                     try:
-                        results_publisher.publish(message)
-                        if task_id:
-                            num_results_forwarded += 1  # Safe given GIL
+                        results_publisher.publish(packed_message)
 
                     except Exception:
                         # Publishing didn't work -- quiesce and see if a simple restart
                         # fixes the issue.
                         self._quiesce_event.set()
 
                         log.exception("Something broke while forwarding results")
                         if task_id:
                             log.info("Storing result for later: %s", task_id)
-                            self.result_store[task_id] = packed_result
+                            self.result_store[task_id] = packed_message
                         continue  # just be explicit
 
                 log.debug("Exit process-pending-results thread.")
 
             stored_processor_thread = threading.Thread(
                 target=process_stored_results, name="Stored Result Handler"
             )
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,35 @@
 )
 from globus_compute_common.messagepack.message_types import Result as OutgoingResult
 from globus_compute_common.messagepack.message_types import (
     ResultErrorDetails as OutgoingResultErrorDetails,
 )
 from globus_compute_common.messagepack.message_types import Task as OutgoingTask
 from globus_compute_common.messagepack.message_types import TaskTransition
-from globus_compute_endpoint.executors.high_throughput.messages import (
+from globus_compute_endpoint.engines.high_throughput.messages import (
     EPStatusReport as InternalEPStatusReport,
 )
-from globus_compute_endpoint.executors.high_throughput.messages import (
+from globus_compute_endpoint.engines.high_throughput.messages import (
     Task as InternalTask,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def convert_ep_status_report(
+    internal: InternalEPStatusReport,
+) -> OutgoingEPStatusReport:
+    messagepack_msg = OutgoingEPStatusReport(
+        endpoint_id=internal._header,
+        global_state=internal.global_state,
+        task_statuses=internal.task_statuses,
+    )
+    return messagepack_msg
+
+
 def try_convert_to_messagepack(message: bytes) -> bytes:
     try:
         unpacked = pickle.loads(message)
     except pickle.UnpicklingError:
         # message isn't pickled; assume that it's already in messagepack format
         return message
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,41 +113,55 @@
         self, shutdown_event: threading.Event, heartbeat_period_s: float
     ):
         while not shutdown_event.wait(timeout=heartbeat_period_s):
             status_report = self.get_status_report()
             packed = messagepack.pack(status_report)
             self.results_passthrough.put(packed)
 
-    def _future_done_callback(self, future: Future):
-        """Callback to post result to the passthrough queue
+    def _setup_future_done_callback(self, task_id: uuid.UUID, future: Future) -> None:
+        """
+        Set up the done() callback for the provided future.
+
+        The done callback handles
+        Callback to post result to the passthrough queue
         Parameters
         ----------
         future: Future for which the callback is triggerd
         """
 
-        if future.exception():
-            code, user_message = get_result_error_details()
-            error_details = {"code": code, "user_message": user_message}
-            exec_end = TaskTransition(
-                timestamp=time.time_ns(),
-                state=TaskState.EXEC_END,
-                actor=ActorName.WORKER,
-            )
-            result_message = dict(
-                task_id=future.task_id,  # type: ignore
-                data=get_error_string(),
-                exception=get_error_string(),
-                error_details=error_details,
-                task_statuses=[exec_end],  # We don't have any more info transitions
-            )
-            packed_result = messagepack.pack(Result(**result_message))
-        else:
-            packed_result = future.result()
+        exec_beg = TaskTransition(  # Reminder: used by *closure*, below
+            timestamp=time.time_ns(),
+            actor=ActorName.INTERCHANGE,
+            state=TaskState.WAITING_FOR_LAUNCH,
+        )
+
+        def _done_cb(f: Future):
+            if f.exception():
+                exc = f.exception()
+                code, user_message = get_result_error_details(exc)
+                error_details = {"code": code, "user_message": user_message}
+                exec_end = TaskTransition(
+                    timestamp=time.time_ns(),
+                    actor=ActorName.INTERCHANGE,
+                    state=TaskState.EXEC_END,
+                )
+                result_message = dict(
+                    task_id=task_id,
+                    data=get_error_string(exc=exc),
+                    exception=get_error_string(exc=exc),
+                    error_details=error_details,
+                    task_statuses=[exec_beg, exec_end],  # only transition info we have
+                )
+                packed_result = messagepack.pack(Result(**result_message))
+            else:
+                packed_result = f.result()
 
-        self.results_passthrough.put(packed_result)
+            self.results_passthrough.put(packed_result)
+
+        future.add_done_callback(_done_cb)
 
     @abstractmethod
     def _submit(
         self,
         func: t.Callable,
         *args: t.Any,
         **kwargs: t.Any,
@@ -162,15 +176,10 @@
         ----------
         packed_task: messagepack bytes buffer
         Returns
         -------
         future
         """
 
-        future: Future = self._submit(execute_task, packed_task)
-
-        # Executors mark futures are failed in the event of faults
-        # We need to tie the task_id info into the future to identify
-        # which tasks have failed
-        future.task_id = task_id  # type: ignore
-        future.add_done_callback(self._future_done_callback)
+        future = self._submit(execute_task, task_id, packed_task)
+        self._setup_future_done_callback(task_id, future)
         return future
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import logging
+import os
 import time
 import typing as t
 import uuid
 
 from globus_compute_common import messagepack
 from globus_compute_common.messagepack.message_types import Result, Task, TaskTransition
 from globus_compute_common.tasks import ActorName, TaskState
+from globus_compute_endpoint.engines.high_throughput.messages import Message
 from globus_compute_endpoint.exception_handling import (
     get_error_string,
     get_result_error_details,
 )
 from globus_compute_endpoint.exceptions import CouldNotExecuteUserTaskError
-from globus_compute_endpoint.executors.high_throughput.messages import Message
 from globus_compute_sdk.errors import MaxResultSizeExceeded
 from globus_compute_sdk.serialize import ComputeSerializer
+from parsl.app.python import timeout
 
 log = logging.getLogger(__name__)
 
 serializer = ComputeSerializer()
 
 
-def execute_task(task_body: bytes, result_size_limit: int = 10 * 1024 * 1024) -> bytes:
+def execute_task(
+    task_id: uuid.UUID, task_body: bytes, result_size_limit: int = 10 * 1024 * 1024
+) -> bytes:
     """Execute task is designed to enable any executor to execute a Task payload
     and return a Result payload, where the payload follows the globus-compute protocols
     This method is placed here to make serialization easy for executor classes
     Parameters
     ----------
     task_id: uuid string
     task_body: packed message as bytes
@@ -35,30 +39,30 @@
     """
     exec_start = TaskTransition(
         timestamp=time.time_ns(), state=TaskState.EXEC_START, actor=ActorName.WORKER
     )
 
     result_message: dict[
         str,
-        t.Union[uuid.UUID, str, tuple[str, str], list[TaskTransition], dict[str, str]],
-    ] = {}
+        uuid.UUID | str | tuple[str, str] | list[TaskTransition] | dict[str, str],
+    ]
 
     try:
-        task, task_buffer = _unpack_messagebody(task_body)
-        log.debug("executing task task_id='%s'", task.task_id)
+        _task, task_buffer = _unpack_messagebody(task_body)
+        log.debug("executing task task_id='%s'", task_id)
         result = _call_user_function(task_buffer, result_size_limit=result_size_limit)
         log.debug("Execution completed without exception")
-        result_message = dict(task_id=task.task_id, data=result)
+        result_message = dict(task_id=task_id, data=result)
 
     except Exception:
         log.exception("Caught an exception while executing user function")
         code, user_message = get_result_error_details()
         error_details = {"code": code, "user_message": user_message}
         result_message = dict(
-            task_id=task.task_id,
+            task_id=task_id,
             data=get_error_string(),
             exception=get_error_string(),
             error_details=error_details,
         )
 
     exec_end = TaskTransition(
         timestamp=time.time_ns(),
@@ -66,15 +70,15 @@
         actor=ActorName.WORKER,
     )
 
     result_message["task_statuses"] = [exec_start, exec_end]
 
     log.debug(
         "task %s completed in %d ns",
-        task.task_id,
+        task_id,
         (exec_end.timestamp - exec_start.timestamp),
     )
 
     return messagepack.pack(Result(**result_message))
 
 
 def _unpack_messagebody(message: bytes) -> t.Tuple[Task, str]:
@@ -114,15 +118,20 @@
     task_buffer: serialized buffer of (fn, args, kwargs)
     result_size_limit: size limit in bytes for results
     serializer: serializer for the buffers
     Returns
     -------
     Returns serialized result or throws exception.
     """
+    GC_TASK_TIMEOUT = max(0.0, float(os.environ.get("GC_TASK_TIMEOUT", 0.0)))
     f, args, kwargs = serializer.unpack_and_deserialize(task_buffer)
+    if GC_TASK_TIMEOUT > 0.0:
+        log.debug(f"Setting task timeout to GC_TASK_TIMEOUT={GC_TASK_TIMEOUT}s")
+        f = timeout(f, GC_TASK_TIMEOUT)
+
     result_data = f(*args, **kwargs)
     serialized_data = serializer.serialize(result_data)
 
     if len(serialized_data) > result_size_limit:
         raise MaxResultSizeExceeded(len(serialized_data), result_size_limit)
 
     return serialized_data
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/thread_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import multiprocessing
 import typing as t
 import uuid
 from concurrent.futures import Future
-from concurrent.futures import ProcessPoolExecutor as NativeExecutor
+from concurrent.futures import ThreadPoolExecutor as NativeExecutor
 from multiprocessing.queues import Queue as mpQueue
 
 import psutil
 from globus_compute_common.messagepack.message_types import (
     EPStatusReport,
     TaskTransition,
 )
@@ -17,19 +17,19 @@
     GlobusComputeEngineBase,
     ReportingThread,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class ProcessPoolEngine(GlobusComputeEngineBase):
+class ThreadPoolEngine(GlobusComputeEngineBase):
     def __init__(
         self,
         *args,
-        label: str = "ProcessPoolEngine",
+        label: str = "ThreadPoolEngine",
         heartbeat_period_s: float = 30.0,
         **kwargs,
     ):
         self.label = label
         self.executor = NativeExecutor(*args, **kwargs)
         self._status_report_thread = ReportingThread(
             target=self.report_status, args=[], reporting_period=heartbeat_period_s
@@ -48,15 +48,15 @@
         ----------
         endpoint_id: Endpoint UUID
         results_passthrough: Queue to which packed results will be posted
         run_dir Not used
         Returns
         -------
         """
-        assert endpoint_id, "ProcessPoolExecutor requires kwarg:endpoint_id at start"
+        assert endpoint_id, "ThreadPoolEngine requires kwarg:endpoint_id at start"
         self.endpoint_id = endpoint_id
         if results_passthrough:
             self.results_passthrough = results_passthrough
         assert self.results_passthrough
 
         # mypy think the thread can be none
         self._status_report_thread.start()
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exception_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,42 +19,46 @@
 
 INTERNAL_ERROR_CLASSES: tuple[type[Exception], ...] = (
     CouldNotExecuteUserTaskError,
     MaxResultSizeExceeded,
 )
 
 
-def _typed_excinfo() -> tuple[type[Exception], Exception, types.TracebackType]:
+def _typed_excinfo(
+    exc: Exception | None = None,
+) -> tuple[type[Exception], Exception, types.TracebackType]:
+    if exc:
+        return type(exc), exc, exc.__traceback__  # type: ignore
     return t.cast(
         t.Tuple[t.Type[Exception], Exception, types.TracebackType],
         sys.exc_info(),
     )
 
 
 def _inner_traceback(tb: types.TracebackType, levels: int = 2) -> types.TracebackType:
     while levels > 0:
         tb = tb.tb_next if tb.tb_next is not None else tb
         levels -= 1
     return tb
 
 
-def get_error_string(*, tb_levels: int = 2) -> str:
-    exc_info = _typed_excinfo()
+def get_error_string(*, exc: t.Any | None = None, tb_levels: int = 2) -> str:
+    exc_info = _typed_excinfo(exc)
     exc_type, exc, tb = exc_info
     if isinstance(exc, INTERNAL_ERROR_CLASSES):
         return repr(exc)
     return "".join(
         traceback.format_exception(
             exc_type, exc, _inner_traceback(tb, levels=tb_levels)
         )
     )
 
 
-def get_result_error_details() -> tuple[str, str]:
-    _, error, _ = _typed_excinfo()
+def get_result_error_details(exc: BaseException | None = None) -> tuple[str, str]:
+    _, error, _ = _typed_excinfo(exc)  # type: ignore
     # code, user_message
     if isinstance(error, INTERNAL_ERROR_CLASSES):
-        return (error.__class__.__name__, f"remote error: {error}")
+        return type(error).__name__, f"remote error: {error}"
     return (
         "RemoteExecutionError",
         "An error occurred during the execution of this task",
     )
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-"""HighThroughputExecutor builds on the Swift/T EMEWS architecture to use MPI for fast
-task distribution
-
-There's a slow but sure deviation from Parsl's Executor interface here, that needs
-to be addressed.
+"""HighThroughputEngine builds on Parsl's HighThroughputExecutor for execution
+of functions within containerized workers in a distributed setting.
 """
 from __future__ import annotations
 
 import concurrent.futures
 import ipaddress
 import logging
 import os
 import queue
 import threading
 import time
+import typing as t
 import uuid
+from concurrent.futures import Future
 from multiprocessing import Process
 
-import daemon
 import dill
-from globus_compute_endpoint.executors.high_throughput import interchange, zmq_pipes
-from globus_compute_endpoint.executors.high_throughput.mac_safe_queue import mpQueue
-from globus_compute_endpoint.executors.high_throughput.messages import (
+from globus_compute_common import messagepack
+from globus_compute_endpoint.endpoint.messages_compat import convert_ep_status_report
+from globus_compute_endpoint.engines.base import GlobusComputeEngineBase
+from globus_compute_endpoint.engines.helper import execute_task
+from globus_compute_endpoint.engines.high_throughput import interchange, zmq_pipes
+from globus_compute_endpoint.engines.high_throughput.mac_safe_queue import mpQueue
+from globus_compute_endpoint.engines.high_throughput.messages import (
     EPStatusReport,
     Heartbeat,
     HeartbeatReq,
     Task,
     TaskCancel,
 )
-from globus_compute_endpoint.logging_config import setup_logging
 from globus_compute_endpoint.strategies.simple import SimpleStrategy
 from globus_compute_sdk.serialize import ComputeSerializer
 from parsl.dataflow.error import ConfigurationError
 from parsl.executors.errors import BadMessage, ScalingFailed
 from parsl.providers import LocalProvider
 from parsl.utils import RepresentationMixin
 
-fx_serializer = ComputeSerializer()
-
-
-# TODO: YADU There's a bug here which causes some of the log messages to write out to
-# stderr
-# "logging" python3 self.stream.flush() OSError: [Errno 9] Bad file descriptor
+serializer = ComputeSerializer()
 
 log = logging.getLogger(__name__)
 
 
 BUFFER_THRESHOLD = 1024 * 1024
 ITEM_THRESHOLD = 1024
 
 
-class HighThroughputExecutor(RepresentationMixin):
-    """Executor designed for cluster-scale
+class HighThroughputEngine(GlobusComputeEngineBase, RepresentationMixin):
+    """Engine designed for cluster-scale
 
-    The HighThroughputExecutor system has the following components:
-      1. The HighThroughputExecutor instance which is run as part of the Parsl script.
+    The HighThroughputEngine system has the following components:
+      1. The HighThroughputEngine instance which is run as a client
       2. The Interchange which is acts as a load-balancing proxy between workers and
          Parsl
       3. The multiprocessing based worker pool which coordinates task execution over
          several cores on a node.
-      4. ZeroMQ pipes connect the HighThroughputExecutor, Interchange and the
+      4. ZeroMQ pipes connect the HighThroughputEngine, Interchange and the
          process_worker_pool
 
     Here is a diagram
 
     .. code:: python
 
 
-                        |  Data   |  Executor   |  Interchange  | External Process(es)
+                        |  Data   |  Engine     |  Interchange  | External Process(es)
                         |  Flow   |             |               |
                    Task | Kernel  |             |               |
                  +----->|-------->|------------>|->outgoing_q---|-> process_worker_pool
                  |      |         |             | batching      |    |         |
            Parsl<---Fut-|         |             | load-balancing|  result   exception
                      ^  |         |             | watchdogs     |    |         |
                      |  |         |   Q_mngmnt  |               |    V         V
@@ -93,15 +89,15 @@
         :class:`~parsl.providers.jetstream.jetstream.Jetstream`,
         :class:`~parsl.providers.local.local.Local`,
         :class:`~parsl.providers.sge.sge.GridEngine`,
         :class:`~parsl.providers.slurm.slurm.Slurm`, or
         :class:`~parsl.providers.torque.torque.Torque`.
 
     label : str
-        Label for this executor instance.
+        Label for this Engine instance.
 
     launch_cmd : str
         Command line string to launch the process_worker_pool from the provider. The
         command line string will be formatted with appropriate values for the following
         values: (
             debug,
             task_url,
@@ -113,15 +109,15 @@
             logdir,
         ).
         For example:
         launch_cmd="process_worker_pool.py {debug} -c {cores_per_worker} \
         --task_url={task_url} --result_url={result_url}"
 
     address : string
-        An address of the host on which the executor runs, which is reachable from the
+        An address of the host on which the engine runs, which is reachable from the
         network in which workers will be running. This can be either a hostname as
         returned by `hostname` or an IP address. Most login nodes on clusters have
         several network interfaces available, only some of which can be reached
         from the compute nodes. Some trial and error might be necessary to
         indentify what addresses are reachable from compute nodes.
 
     worker_ports : (int, int)
@@ -131,15 +127,15 @@
     worker_port_range : (int, int)
         Worker ports will be chosen between the two integers provided.
 
     interchange_port_range : (int, int)
         Port range used by Parsl to communicate with the Interchange.
 
     working_dir : str
-        Working dir to be used by the executor.
+        Working dir to be used by the engine.
 
     worker_debug : Bool
         Enables worker debug logging.
 
     cores_per_worker : float
         cores to be assigned to each worker. Oversubscription is possible
         by setting cores_per_worker < 1.0. Default=1
@@ -174,15 +170,15 @@
 
     heartbeat_period : int
         Number of seconds after which a heartbeat message indicating liveness is sent to
         the endpoint
         counterpart (interchange, manager). Default:30s
 
     poll_period : int
-        Timeout period to be used by the executor components in milliseconds.
+        Timeout period to be used by the engine components in milliseconds.
         Increasing poll_periods trades performance for cpu efficiency. Default: 10ms
 
     container_image : str
         Path or identfier to the container image to be used by the workers
 
     scheduler_mode: str
         Scheduling mode to be used by the node manager. Options: 'hard', 'soft'
@@ -198,15 +194,15 @@
         Container command strings to be added to associated container command.
         For example, singularity exec {container_cmd_options}
 
     task_status_queue : queue.Queue
         Queue to pass updates to task statuses back to the forwarder.
 
     strategy: Stategy Object
-        Specify the scaling strategy to use for this executor.
+        Specify the scaling strategy to use for this engine.
 
     launch_cmd: str
         Specify the launch command as using f-string format that will be used to specify
         command to launch managers. Default: None
 
     prefetch_capacity: int
         Number of tasks that can be fetched by managers in excess of available
@@ -219,15 +215,15 @@
         offers forked processes, and SlurmProvider interfaces to request
         resources from the Slurm batch scheduler.
         Default: LocalProvider
     """
 
     def __init__(
         self,
-        label="HighThroughputExecutor",
+        label="HighThroughputEngine",
         # NEW
         strategy=SimpleStrategy(),
         max_workers_per_node=float("inf"),
         mem_per_worker=None,
         launch_cmd=None,
         available_accelerators=None,
         # Container specific
@@ -253,15 +249,15 @@
         container_image=None,
         suppress_failure=True,
         run_dir=None,
         endpoint_id=None,
         passthrough=True,
         task_status_queue=None,
     ):
-        log.debug("Initializing HighThroughputExecutor")
+        log.debug("Initializing HighThroughputEngine")
         self.provider = provider
         self.label = label
         self.launch_cmd = launch_cmd
         self.worker_debug = worker_debug
         self.max_workers_per_node = max_workers_per_node
 
         # NEW
@@ -357,16 +353,16 @@
         *args,
         endpoint_id: uuid.UUID | None = None,
         run_dir: str | None = None,
         results_passthrough: queue.Queue[dict[str, bytes | str | None]] | None = None,
         **kwargs,
     ):
         """Create the Interchange process and connect to it."""
-        assert run_dir, "GCExecutor requires kwarg:run_dir at start"
-        assert endpoint_id, "GCExecutor requires kwarg:endpoint_id at start"
+        assert run_dir, "HighThroughputEngine requires kwarg:run_dir at start"
+        assert endpoint_id, "HighThroughputEngine requires kwarg:endpoint_id at start"
         self.run_dir = run_dir
         self.endpoint_id = endpoint_id
 
         self.outgoing_q = zmq_pipes.TasksOutgoing(
             "127.0.0.1", self.interchange_port_range
         )
         self.incoming_q = zmq_pipes.ResultsIncoming(
@@ -377,22 +373,22 @@
         )
 
         self.is_alive = True
 
         if self.passthrough is True:
             if results_passthrough is None:
                 raise Exception(
-                    "Executors configured in passthrough mode, must be started with"
+                    "Engines configured in passthrough mode, must be started with"
                     "a multiprocessing queue for results_passthrough"
                 )
             self.results_passthrough = results_passthrough
-            log.debug(f"Executor:{self.label} starting in results_passthrough mode")
+            log.debug(f"Engine:{self.label} starting in results_passthrough mode")
 
-        self._executor_bad_state = threading.Event()
-        self._executor_exception = None
+        self._engine_bad_state = threading.Event()
+        self._engine_exception: t.Optional[Exception] = None
         self._start_queue_management_thread()
 
         log.info("Attempting local interchange start")
         self._start_local_interchange_process()
         log.info(
             "Started local interchange with ports: %s. %s",
             self.worker_task_port,
@@ -401,31 +397,31 @@
 
         log.debug(f"Created management thread: {self._queue_management_thread}")
 
         if self.provider:
             pass
         else:
             self._scaling_enabled = False
-            log.debug("Starting HighThroughputExecutor with no provider")
+            log.debug("Starting HighThroughputEngine with no provider")
 
         return self.outgoing_q.port, self.incoming_q.port, self.command_client.port
 
     def _start_local_interchange_process(self):
         """Starts the interchange process locally
 
         Starts the interchange process locally and uses an internal command queue to
         get the worker task and result ports that the interchange has bound to.
         """
         comm_q = mpQueue(maxsize=10)
         self.queue_proc = Process(
             target=interchange.starter,
-            name="Executor-Interchange",
+            name="Engine-Interchange",
             args=(comm_q,),
             kwargs={
-                "client_address": "127.0.0.1",  # executor and ix are on the same node
+                "client_address": "127.0.0.1",  # engine and ix are on the same node
                 "client_ports": (
                     self.outgoing_q.port,
                     self.incoming_q.port,
                     self.command_client.port,
                 ),
                 "provider": self.provider,
                 "strategy": self.strategy,
@@ -472,14 +468,18 @@
         self.worker_task_port, self.worker_result_port = msg
 
         self.worker_task_url = f"tcp://{self.address}:{self.worker_task_port}"
         self.worker_result_url = "tcp://{}:{}".format(
             self.address, self.worker_result_port
         )
 
+    def get_status_report(self) -> EPStatusReport:
+        """HTEX Interchange reports EPStatusReport periodically"""
+        raise NotImplementedError
+
     def _queue_management_worker(self):
         """Listen to the queue for task status messages and handle them.
 
         Depending on the message, tasks will be updated with results, exceptions,
         or updates. It expects the following messages:
 
         .. code:: python
@@ -507,15 +507,15 @@
                "started"  : tstamp
             }
 
         The `None` message is a die request.
         """
         log.debug("queue management worker starting")
 
-        while self.is_alive and not self._executor_bad_state.is_set():
+        while self.is_alive and not self._engine_bad_state.is_set():
             try:
                 msgs = self.incoming_q.get(timeout=1)
 
             except queue.Empty:
                 log.debug("queue empty")
                 # Timed out.
                 continue
@@ -530,18 +530,19 @@
 
             else:
                 if msgs is None:
                     log.debug("Got None, exiting")
                     return
 
                 elif isinstance(msgs, EPStatusReport):
-                    log.debug(f"Received EPStatusReport {msgs}")
+                    log.debug(f"Received {msgs!r}")
                     if self.passthrough:
+                        external_ep_status = convert_ep_status_report(msgs)
                         self.results_passthrough.put(
-                            {"task_id": None, "message": dill.dumps(msgs)}
+                            messagepack.pack(external_ep_status)
                         )
 
                 else:
                     log.debug("Unpacking results")
                     for serialized_msg in msgs:
                         try:
                             msg = dill.loads(serialized_msg)
@@ -555,29 +556,30 @@
                             )
 
                         if tid == -1 and "exception" in msg:
                             # TODO: This could be handled better we are
                             # essentially shutting down the client with little
                             # indication to the user.
                             log.warning(
-                                "Executor shutting down due to fatal "
+                                "Engine shutting down due to fatal "
                                 "exception from interchange"
                             )
-                            self._executor_exception = fx_serializer.deserialize(
+                            self._engine_exception = serializer.deserialize(
                                 msg["exception"]
                             )
-                            log.exception(f"Exception: {self._executor_exception}")
+                            log.exception(f"Exception: {self._engine_exception}")
                             # Set bad state to prevent new tasks from being submitted
-                            self._executor_bad_state.set()
+                            self._engine_bad_state.set()
                             # We set all current tasks to this exception to make sure
                             # that this is raised in the main context.
+                            # YADU: Report failure on all pending tasks
                             for task_id in self.tasks:
                                 try:
                                     self.tasks[task_id].set_exception(
-                                        self._executor_exception
+                                        self._engine_exception
                                     )
                                 except concurrent.futures.InvalidStateError:
                                     # Task was already cancelled, the exception can be
                                     # ignored
                                     log.debug(
                                         f"Task:{task_id} result couldn't be set. "
                                         "Already in terminal state"
@@ -585,23 +587,17 @@
                             break
 
                         if self.passthrough is True:
                             log.debug(f"Pushing results for task:{tid}")
                             # we are only interested in actual task ids here, not
                             # identifiers for other message types
                             sent_task_id = tid if isinstance(tid, str) else None
-                            x = self.results_passthrough.put(
-                                {"task_id": sent_task_id, "message": serialized_msg}
-                            )
-                            log.debug(f"task:{tid} ret value: {x}")
-                            log.debug(
-                                "task:%s items in queue: %s",
-                                tid,
-                                self.results_passthrough.qsize(),
-                            )
+                            packed_result = self._convert_result_to_outgoing(msg)
+                            self.results_passthrough.put(packed_result)
+                            self.tasks[sent_task_id].set_result(packed_result)
                             continue
 
                         try:
                             task_fut = self.tasks.pop(tid)
                         except KeyError:
                             # This is triggered when the result of a cancelled task is
                             # returned
@@ -609,39 +605,45 @@
                             log.warning(
                                 f"Task:{tid} not found in tasks table\n"
                                 "Task likely was cancelled and removed."
                             )
                             continue
 
                         if "result" in msg:
-                            result = fx_serializer.deserialize(msg["result"])
+                            result = serializer.deserialize(msg["result"])
                             try:
                                 task_fut.set_result(result)
                             except concurrent.futures.InvalidStateError:
                                 log.debug(
                                     f"Task:{tid} result couldn't be set. "
                                     "Already in terminal state"
                                 )
                         elif "exception" in msg:
-                            exception = fx_serializer.deserialize(msg["exception"])
+                            exception = serializer.deserialize(msg["exception"])
                             try:
                                 task_fut.set_result(exception)
                             except concurrent.futures.InvalidStateError:
                                 log.debug(
                                     f"Task:{tid} result couldn't be set. "
                                     "Already in terminal state"
                                 )
                         else:
                             raise BadMessage(
                                 "Message received is neither result or exception"
                             )
 
         log.info("queue management worker finished")
 
-    # When the executor gets lost, the weakref callback will wake up
+    def _convert_result_to_outgoing(self, msg: dict[str, t.Union[str, bytes]]) -> bytes:
+        """The messagepacked result should be in the result dict in the data field"""
+        # The data body already is packed on the worker
+        assert isinstance(msg["data"], bytes)
+        return msg["data"]
+
+    # When the engine gets lost, the weakref callback will wake up
     # the queue management thread.
     def weakref_cb(self, q=None):
         """We do not use this yet."""
         q.put(None)
 
     def _start_queue_management_thread(self):
         """Method to start the management thread as a daemon.
@@ -695,58 +697,44 @@
 
     @property
     def connected_workers(self):
         workers = self.command_client.run("MANAGERS")
         log.debug(f"Got managers: {workers}")
         return workers
 
-    def submit(
-        self, func, *args, container_id: str = "RAW", task_id: str = None, **kwargs
-    ):
-        """Submits the function and it's params for execution."""
-        self._task_counter += 1
-        if task_id is None:
-            task_id = self._task_counter
-        task_id = str(task_id)
-
-        fn_code = fx_serializer.serialize(func)
-        ser_code = fx_serializer.pack_buffers([fn_code])
-        ser_params = fx_serializer.pack_buffers(
-            [fx_serializer.serialize(args), fx_serializer.serialize(kwargs)]
-        )
-        payload = Task(task_id, container_id, ser_code + ser_params)
-
-        self.submit_raw(payload.pack())
-        self.tasks[task_id] = HTEXFuture(self)
-        self.tasks[task_id].task_id = task_id
+    def _submit(self, func: t.Callable, *args: t.Any, **kwargs: t.Any) -> Future:
+        raise RuntimeError("Invalid attempt to _submit()")
 
-        return self.tasks[task_id]
-
-    def submit_raw(self, packed_task):
-        """Submits work to the the outgoing_q.
-
-        The outgoing_q is an external process listens on this
-        queue for new work. This method behaves like a
-        submit call as described in the `Python docs \
-        <https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor>`_
+    def submit(self, task_id: uuid.UUID, packed_task: bytes) -> HTEXFuture:
+        """Submits a messagepacked.Task for execution
 
         Parameters
         ----------
         Packed Task (messages.Task) - A packed Task object which contains task_id,
         container_id, and serialized fn, args, kwargs packages.
 
         Returns:
               Submit status
         """
-        log.debug(f"Submitting raw task : {packed_task}")
-        if self._executor_bad_state.is_set():
-            raise self._executor_exception
+        if self._engine_bad_state.is_set():
+            # If the flag is set the exception body must exist
+            raise self._engine_exception  # type: ignore
 
-        # Submit task to queue
-        return self.outgoing_q.put(packed_task)
+        self._task_counter += 1
+
+        task_id_str = str(task_id)
+        future = HTEXFuture(self, task_id_str)
+        self.tasks[task_id_str] = future
+
+        ser = serializer.serialize((execute_task, [task_id, packed_task], {}))
+        payload = Task(task_id_str, "RAW", ser).pack()
+        assert self.outgoing_q  # Placate mypy
+        self.outgoing_q.put(payload)
+
+        return future
 
     def _get_block_and_job_ids(self):
         # Not using self.blocks.keys() and self.blocks.values() simultaneously
         # The dictionary may be changed during invoking this function
         # As scale_in and scale_out are invoked in multiple threads
         block_ids = list(self.blocks.keys())
         job_ids = []  # types: List[Any]
@@ -822,88 +810,83 @@
         status = []
         if self.provider:
             status = self.provider.status(self.blocks)
 
         return status
 
     def shutdown(self, hub=True, targets="all", block=False):
-        """Shutdown the executor, including all workers and controllers.
+        """Shutdown the Engine, including all workers and controllers.
 
         This is not implemented.
 
         Kwargs:
             - hub (Bool): Whether the hub should be shutdown, Default:True,
             - targets (list of ints| 'all'): List of block id's to kill, Default:'all'
             - block (Bool): To block for confirmations or not
 
         Raises:
              NotImplementedError
         """
 
-        log.info("Attempting HighThroughputExecutor shutdown")
+        log.info("Attempting HighThroughputEngine shutdown")
         # self.outgoing_q.close()
         # self.incoming_q.close()
         if self.queue_proc:
             try:
                 self.queue_proc.terminate()
             except AttributeError:
-                log.info("Executor interchange terminate skipped due to wrong context")
+                log.info("Engine interchange terminate skipped due to wrong context")
             except Exception:
                 log.exception("Terminating the interchange failed")
-        log.info("Finished HighThroughputExecutor shutdown attempt")
+        log.info("Finished HighThroughputEngine shutdown attempt")
         return True
 
-    def _cancel(self, future):
-        """Attempt cancelling a task tracked by the future by requesting
-        cancellation from the interchange. Task cancellation is attempted
-        only if the future is cancellable i.e not already in a terminal
-        state. This relies on the executor not setting the task to a running
-        state, and the task only tracking pending, and completed states.
+    def cancel_task(self, task_id: uuid.UUID | str) -> bool:
+        """
+        Attempt to cancel the task `task_id` by requesting cancellation
+        from the interchange.  Task cancellation is attempted only if the
+        future is cancellable (i.e., not already in a terminal state).  This
+        relies on the Engine not setting the task to a running state, and the
+        task only tracking pending, and completed states.
 
         Parameters
         ----------
-        future
+        task_id
 
         Returns
         -------
         Bool
         """
 
-        ret_value = future._cancel()
+        log.debug("Send TaskCancel to interchange (%s)", task_id)
         log.debug("Sending cancel of task_id:{future.task_id} to interchange")
-        if ret_value is True:
-            self.command_client.run(TaskCancel(future.task_id))
-            log.debug("Sent TaskCancel to interchange")
-        return ret_value
+        # TODO: Doesn't yet return a bool ...
+        assert self.command_client
+        return self.command_client.run(TaskCancel(str(task_id)))
 
 
 CANCELLED = "CANCELLED"
 CANCELLED_AND_NOTIFIED = "CANCELLED_AND_NOTIFIED"
 FINISHED = "FINISHED"
 
 
 class HTEXFuture(concurrent.futures.Future):
-    def __init__(self, executor):
+    __slots__ = ("engine", "task_id")
+
+    def __init__(self, engine: HighThroughputEngine, task_id: str):
         super().__init__()
-        self.executor = executor
+        self.engine = engine
+        self.task_id = task_id
 
     def cancel(self):
         raise NotImplementedError(
             f"{self.__class__} does not implement cancel() "
             "try using best_effort_cancel()"
         )
 
-    def _cancel(self):
-        """Should be invoked only by the executor
-        Returns
-        -------
-        Bool
-        """
-        return super().cancel()
-
     def best_effort_cancel(self):
         """Attempt to cancel the function.
 
         If the function has finished running, the task cannot be cancelled
         and the method will return False.
         If the function is yet to start or is running, cancellation will be
         attempted without guarantees, and the method will return True.
@@ -912,25 +895,8 @@
         function will not execute at all, but it does guarantee that the
         future will be in a cancelled state.
 
         Returns
         -------
         Bool
         """
-        return self.executor._cancel(self)
-
-
-def executor_starter(htex, logdir, endpoint_id):
-    stdout = open(os.path.join(logdir, f"executor.{endpoint_id}.stdout"), "w")
-    stderr = open(os.path.join(logdir, f"executor.{endpoint_id}.stderr"), "w")
-
-    logdir = os.path.abspath(logdir)
-    with daemon.DaemonContext(stdout=stdout, stderr=stderr):
-        print("cwd: ", os.getcwd())
-        setup_logging(
-            logfile=os.path.join(logdir, f"executor.{endpoint_id}.log"),
-            console_enabled=False,
-        )
-        htex.start()
-
-    stdout.close()
-    stderr.close()
+        return self.engine.cancel_task(self.task_id)
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 from collections import defaultdict
 
 import daemon
 import dill
 import zmq
 from globus_compute_common.messagepack.message_types import TaskTransition
 from globus_compute_common.tasks import ActorName, TaskState
-from globus_compute_endpoint.exception_handling import (
-    get_error_string,
-    get_result_error_details,
-)
-from globus_compute_endpoint.executors.high_throughput.interchange_task_dispatch import (  # noqa: E501
+from globus_compute_endpoint.engines.high_throughput.interchange_task_dispatch import (  # noqa: E501
     naive_interchange_task_dispatch,
 )
-from globus_compute_endpoint.executors.high_throughput.messages import (
+from globus_compute_endpoint.engines.high_throughput.messages import (
     BadCommand,
     EPStatusReport,
     Heartbeat,
     Message,
     MessageType,
 )
+from globus_compute_endpoint.exception_handling import (
+    get_error_string,
+    get_result_error_details,
+)
 from globus_compute_endpoint.logging_config import ComputeLogger
 from globus_compute_sdk.sdk.utils import chunk_by
 from globus_compute_sdk.serialize import ComputeSerializer
 from parsl.version import VERSION as PARSL_VERSION
 
 if t.TYPE_CHECKING:
     import multiprocessing as mp
@@ -61,15 +61,15 @@
         return f"Task failure due to loss of manager {self.worker_id}"
 
     def __str__(self):
         return self.__repr__()
 
 
 class BadRegistration(Exception):
-    """A new Manager tried to join the executor with a BadRegistration message"""
+    """A new Manager tried to join the Engine with a BadRegistration message"""
 
     def __init__(self, worker_id, critical=False):
         self.worker_id = worker_id
         self.tstamp = time.time()
         self.handled = "critical" if critical else "suppressed"
 
     def __repr__(self):
@@ -553,28 +553,28 @@
             self._ready_manager_queue[manager]["active"] = False
 
     def _status_report_loop(self, kill_event, status_report_queue: queue.Queue):
         log.info(f"Endpoint id: {self.endpoint_id}")
 
         def _enqueue_status_report(ep_state: dict, task_states: dict):
             try:
-                msg = EPStatusReport(self.endpoint_id, ep_state, dict(task_states))
+                msg = EPStatusReport(str(self.endpoint_id), ep_state, dict(task_states))
                 status_report_queue.put(msg.pack())
             except Exception:
                 log.exception("Unable to create or send EP status report.")
                 log.debug("Attempted to send chunk: %s", tsd_chunk)
                 # ignoring so that the thread continues; "it's just a status"
 
         while True:
             with self._task_status_delta_lock:
                 task_status_deltas = copy.deepcopy(self.task_status_deltas)
                 self.task_status_deltas.clear()
 
             log.debug(
-                "Cleared task deltas (%s); sending status report to executor.",
+                "Cleared task deltas (%s); sending status report to Engine.",
                 len(task_status_deltas),
             )
 
             # For multi-chunk reports ("lots-o-tasks"), the state won't change *that*
             # much each iteration, so cache the result
             global_state = self.get_global_state_for_status_report()
 
@@ -956,48 +956,31 @@
                             "Got container switch count: %s",
                             self.container_switch_count,
                         )
                     except Exception:
                         pass
                     if len(b_messages):
                         log.info(f"Got {len(b_messages)} result items in batch")
-                        with self._task_status_delta_lock:
-                            for idx, b_message in enumerate(b_messages):
-                                r = dill.loads(b_message)
-                                tid = r["task_id"]
-
-                                log.debug(
-                                    "Received task result %s (from %s)", tid, manager
-                                )
-                                task_container = self.containers[r["container_id"]]
-                                log.debug(
-                                    "Removing for manager: %s from %s",
-                                    manager,
-                                    self._ready_manager_queue,
-                                )
-
-                                mdata["tasks"][task_container].remove(tid)
-
-                                # Transfer any outstanding task statuses to the
-                                # result message
-                                if tid in self.task_status_deltas:
-                                    r["task_statuses"] += self.task_status_deltas[tid]
-                                    del self.task_status_deltas[tid]
-                                    b_messages[idx] = dill.dumps(r)
-                                    log.debug(
-                                        "Transferring statuses for %s: %s",
-                                        tid,
-                                        r["task_statuses"],
-                                    )
+                        for idx, b_message in enumerate(b_messages):
+                            r = dill.loads(b_message)
+                            tid = r["task_id"]
+
+                            log.debug("Received task result %s (from %s)", tid, manager)
+                            task_container = self.containers[r["container_id"]]
+                            log.debug(
+                                "Removing for manager: %s from %s",
+                                manager,
+                                self._ready_manager_queue,
+                            )
+
+                            mdata["tasks"][task_container].remove(tid)
+                            b_messages[idx] = dill.dumps(r)
 
                         mdata["total_tasks"] -= len(b_messages)
 
-                    # TODO: handle this with a Task message or something?
-                    # previously used this; switched to mono-message,
-                    # self.results_outgoing.send_multipart(b_messages)
                     self.results_outgoing.send(dill.dumps(b_messages))
                     interesting_managers.add(manager)
 
                     log.debug(f"Current tasks: {mdata['tasks']}")
                 log.debug("leaving results_incoming section")
 
             # Send status reports from this main thread to avoid thread-safety on zmq
@@ -1169,15 +1152,15 @@
 
         return status
 
 
 def starter(comm_q: mp.Queue, *args, **kwargs) -> None:
     """Start the interchange process
 
-    The executor is expected to call this function. The args, kwargs match that of the
+    The Engine is expected to call this function. The args, kwargs match that of the
     Interchange.__init__
     """
     ic = None
     try:
         ic = Interchange(*args, **kwargs)
         comm_q.put((ic.worker_task_port, ic.worker_result_port))
     finally:
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from typing import Any
 
 import dill
 import psutil
 import zmq
 from globus_compute_common.messagepack.message_types import TaskTransition
 from globus_compute_common.tasks import ActorName, TaskState
-from globus_compute_endpoint.exception_handling import (
-    get_error_string,
-    get_result_error_details,
-)
-from globus_compute_endpoint.executors.high_throughput.container_sched import (
+from globus_compute_endpoint.engines.high_throughput.container_sched import (
     naive_scheduler,
 )
-from globus_compute_endpoint.executors.high_throughput.mac_safe_queue import mpQueue
-from globus_compute_endpoint.executors.high_throughput.messages import (
+from globus_compute_endpoint.engines.high_throughput.mac_safe_queue import mpQueue
+from globus_compute_endpoint.engines.high_throughput.messages import (
     ManagerStatusReport,
     Message,
     Task,
 )
-from globus_compute_endpoint.executors.high_throughput.worker_map import WorkerMap
+from globus_compute_endpoint.engines.high_throughput.worker_map import WorkerMap
+from globus_compute_endpoint.exception_handling import (
+    get_error_string,
+    get_result_error_details,
+)
 from globus_compute_endpoint.logging_config import ComputeLogger, setup_logging
 from parsl.version import VERSION as PARSL_VERSION
 
 RESULT_TAG = 10
 TASK_REQUEST_TAG = 11
 HEARTBEAT_CODE = (2**32) - 1
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,19 @@
 
     def __init__(self, endpoint_id, global_state, task_statuses):
         super().__init__()
         self._header = uuid.UUID(endpoint_id).bytes
         self.global_state = global_state
         self.task_statuses = task_statuses
 
+    def __repr__(self):
+        name = type(self).__name__
+        ep_id = uuid.UUID(bytes=self._header)
+        return f"{name}(ep:{ep_id}; task count:{len(self.task_statuses)})"
+
     @classmethod
     def unpack(cls, msg):
         endpoint_id = str(uuid.UUID(bytes=msg[:16]))
         msg = msg[16:]
         jsonified = msg.decode("ascii")
         global_state, statuses = json.loads(jsonified)
         task_statuses = defaultdict(list)
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import os
 import signal
 import sys
-import time
+import typing as t
 
 import dill
 import zmq
 from globus_compute_common import messagepack
-from globus_compute_common.messagepack.message_types import TaskTransition
-from globus_compute_common.tasks import ActorName, TaskState
+from globus_compute_common.messagepack.message_types import Result as OutgoingResult
+from globus_compute_common.messagepack.message_types import (
+    ResultErrorDetails as OutgoingResultErrorDetails,
+)
+from globus_compute_endpoint.engines.high_throughput.messages import Message
 from globus_compute_endpoint.exception_handling import (
     get_error_string,
     get_result_error_details,
 )
-from globus_compute_endpoint.exceptions import CouldNotExecuteUserTaskError
-from globus_compute_endpoint.executors.high_throughput.messages import Message
 from globus_compute_endpoint.logging_config import setup_logging
-from globus_compute_sdk.errors import MaxResultSizeExceeded
 from globus_compute_sdk.serialize import ComputeSerializer
-from parsl.app.python import timeout
 
 log = logging.getLogger(__name__)
 
 DEFAULT_RESULT_SIZE_LIMIT_MB = 10
 DEFAULT_RESULT_SIZE_LIMIT_B = DEFAULT_RESULT_SIZE_LIMIT_MB * 1024 * 1024
 
 
@@ -109,93 +108,58 @@
                 log.info("[KILL] -- Worker KILL message received! ")
                 # send a "worker die" message back to the manager
                 self.task_socket.send_multipart([b"WRKR_DIE", b""])
                 log.info(f"*** WORKER {self.worker_id} ABOUT TO DIE ***")
                 # Kill the worker after accepting death in message to manager.
                 sys.exit()
             else:
-                result = self.execute_task(task_id, msg)
+                result = self._worker_execute_task(task_id, msg)
                 result["container_id"] = container_id
                 log.debug("Sending result")
                 # send bytes over the socket back to the manager
                 self.task_socket.send_multipart([b"TASK_RET", dill.dumps(result)])
 
         log.warning("Broke out of the loop... dying")
 
-    def execute_task(self, task_id: str, task_body: bytes) -> dict:
-        log.debug("executing task task_id='%s'", task_id)
-        exec_start = TaskTransition(
-            timestamp=time.time_ns(), state=TaskState.EXEC_START, actor=ActorName.WORKER
+    def compose_exception_message(self, task_id: str) -> bytes:
+        code, user_message = get_result_error_details()
+        outgoing_result = OutgoingResult(
+            task_id=task_id,
+            data=get_error_string(),
+            error_details=OutgoingResultErrorDetails(
+                code=code,
+                user_message=user_message,
+            ),
         )
+        return messagepack.pack(outgoing_result)
 
+    def _worker_execute_task(
+        self, task_id: str, msg: bytes
+    ) -> dict[str, t.Union[str, bytes]]:
+        result_message: dict[str, t.Union[str, bytes]] = {"task_id": task_id}
         try:
-            result = self.call_user_function(task_body)
-        except Exception:
-            log.exception("Caught an exception while executing user function")
-            result_message: dict[
-                str, str | tuple[str, str] | list[TaskTransition]
-            ] = dict(
-                task_id=task_id,
-                exception=get_error_string(),
-                error_details=get_result_error_details(),
-            )
-
-        else:
-            log.debug("Execution completed without exception")
-            result_message = dict(task_id=task_id, data=result)
-
-        exec_end = TaskTransition(
-            timestamp=time.time_ns(),
-            state=TaskState.EXEC_END,
-            actor=ActorName.WORKER,
-        )
+            # Unwrap HTEX's Task packing
+            task_message = Message.unpack(msg)
+            serialized_fn_package = task_message.task_buffer.decode()
+
+            # Deserialize HTEX Engines' wrapping of
+            # execute_task, messagepack_payload)
+            function, args, kwargs = self.deserialize(serialized_fn_package)
+
+            # Execute
+            serialized_result: bytes = function(*args, **kwargs)
+            result_message["data"] = serialized_result
 
-        result_message["task_statuses"] = [exec_start, exec_end]
+        except Exception:
+            log.exception("Failed to execute task")
+            serialized_error = self.compose_exception_message(task_id)
+            result_message["data"] = serialized_error
 
-        log.debug(
-            "task %s completed in %d ns",
-            task_id,
-            (exec_end.timestamp - exec_start.timestamp),
-        )
         return result_message
 
-    def call_user_function(self, message: bytes) -> str:
-        """Deserialize the buffer and execute the task.
-
-        Returns the result or throws exception.
-        """
-        # try to unpack it as a messagepack message
-        try:
-            task = messagepack.unpack(message)
-            if not isinstance(task, messagepack.message_types.Task):
-                raise CouldNotExecuteUserTaskError(
-                    f"wrong type of message in worker: {type(task)}"
-                )
-            task_data = task.task_buffer
-        # on parse errors, failover to trying the "legacy" message reading
-        except (
-            messagepack.InvalidMessageError,
-            messagepack.UnrecognizedProtocolVersion,
-        ):
-            task = Message.unpack(message)
-            task_data = task.task_buffer.decode("utf-8")  # type: ignore[attr-defined]
-
-        f, args, kwargs = self.serializer.unpack_and_deserialize(task_data)
-        GC_TASK_TIMEOUT = max(0.0, float(os.environ.get("GC_TASK_TIMEOUT", 0.0)))
-        if GC_TASK_TIMEOUT > 0.0:
-            log.debug(f"Setting task timeout to GC_TASK_TIMEOUT={GC_TASK_TIMEOUT}s")
-            f = timeout(f, GC_TASK_TIMEOUT)
-        result_data = f(*args, **kwargs)
-        serialized_data = self.serialize(result_data)
-
-        if len(serialized_data) > self.result_size_limit:
-            raise MaxResultSizeExceeded(len(serialized_data), self.result_size_limit)
-
-        return serialized_data
-
 
 def cli_run():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-w", "--worker_id", required=True, help="ID of worker from process_worker_pool"
     )
     parser.add_argument(
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import logging
 import time
 
 import dill
 import zmq
-from globus_compute_endpoint.executors.high_throughput.messages import Message
+from globus_compute_endpoint.engines.high_throughput.messages import Message
 
 log = logging.getLogger(__name__)
 
 
 class CommandClient:
     """CommandClient"""
 
@@ -48,15 +48,15 @@
 
     def close(self):
         self.zmq_socket.close()
         self.context.term()
 
 
 class TasksOutgoing:
-    """Outgoing task queue from the executor to the Interchange"""
+    """Outgoing task queue from the Engine to the Interchange"""
 
     def __init__(self, ip_address, port_range):
         """
         Parameters
         ----------
 
         ip_address: str
@@ -123,15 +123,15 @@
 
     def close(self):
         self.zmq_socket.close()
         self.context.term()
 
 
 class ResultsIncoming:
-    """Incoming results queue from the Interchange to the executor"""
+    """Incoming results queue from the Interchange to the Engine"""
 
     def __init__(self, ip_address, port_range):
         """
         Parameters
         ----------
 
         ip_address: str
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.1"
+__version__ = "2.2.3a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.2.1/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.1
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.1/setup.py` & `globus-compute-endpoint-2.2.3a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.2.1",
+    "globus-compute-sdk==2.2.3a0",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
@@ -79,19 +79,19 @@
         "Topic :: Scientific/Engineering",
     ],
     keywords=["Globus Compute", "FaaS", "Function Serving"],
     entry_points={
         "console_scripts": [
             "globus-compute-endpoint=globus_compute_endpoint.cli:cli_run",
             "globus-compute-interchange"
-            "=globus_compute_endpoint.executors.high_throughput.interchange:cli_run",
+            "=globus_compute_endpoint.engines.high_throughput.interchange:cli_run",
             "globus-compute-manager"
-            "=globus_compute_endpoint.executors.high_throughput.manager:cli_run",
+            "=globus_compute_endpoint.engines.high_throughput.manager:cli_run",
             "globus-compute-worker"
-            "=globus_compute_endpoint.executors.high_throughput.worker:cli_run",
+            "=globus_compute_endpoint.engines.high_throughput.worker:cli_run",
         ]
     },
     include_package_data=True,
     author="Globus Compute Team",
     author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
```

### Comparing `globus-compute-endpoint-2.2.1/tests/conftest.py` & `globus-compute-endpoint-2.2.3a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.1/tests/utils.py` & `globus-compute-endpoint-2.2.3a0/tests/utils.py`

 * *Files identical despite different names*

