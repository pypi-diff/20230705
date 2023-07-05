# Comparing `tmp/scalable-pypeline-1.1.5.tar.gz` & `tmp/scalable-pypeline-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalable-pypeline-1.1.5.tar", last modified: Tue Apr 11 21:01:59 2023, max compression
+gzip compressed data, was "scalable-pypeline-1.2.0.tar", last modified: Wed Jul  5 20:20:02 2023, max compression
```

## Comparing `scalable-pypeline-1.1.5.tar` & `scalable-pypeline-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4270 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.847206 scalable-pypeline-1.1.5/pypeline/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11499 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10759 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/celery_beat.py
--rw-rw-rw-   0 root         (0) root         (0)     4191 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.848206 scalable-pypeline-1.1.5/pypeline/flask/
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.849206 scalable-pypeline-1.1.5/pypeline/flask/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8295 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/schedules.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5791 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/flask/flask_sermos.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/logging_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6763 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/pipeline_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7385 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/schedule_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    29081 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/sermos_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.851206 scalable-pypeline-1.1.5/pypeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13029 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/config_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/graph_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/module_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    33793 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/pypeline/utils/task_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.853206 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4687 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      541 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-11 21:01:59.000000 scalable-pypeline-1.1.5/scalable_pypeline.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-11 21:01:59.855207 scalable-pypeline-1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6355 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.841205 scalable-pypeline-1.1.5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:01:59.854206 scalable-pypeline-1.1.5/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-11 21:01:38.000000 scalable-pypeline-1.1.5/tests/fixtures/s3_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.250991 scalable-pypeline-1.2.0/pypeline/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9038 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/celery_beat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/flask/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/flask/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5791 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/flask_sermos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/logging_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/chained_task.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7385 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/schedule_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    17336 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/sermos_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.252991 scalable-pypeline-1.2.0/pypeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/config_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/graph_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/module_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22222 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/task_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-05 20:20:02.254991 scalable-pypeline-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.248991 scalable-pypeline-1.2.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.1.5/LICENSE` & `scalable-pypeline-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/PKG-INFO` & `scalable-pypeline-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.5
+Version: 1.2.0
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.1.5/README.md` & `scalable-pypeline-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/celery.py` & `scalable-pypeline-1.2.0/pypeline/celery.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 """ Configure and instantiate Celery
 """
 import os
 
-from pypeline.constants import DEFAULT_RETRY_TASK_MAX_TTL, DEFAULT_MAX_RETRY
-
 if os.environ.get('USE_GEVENT', "False").lower() == 'true':
     from gevent import monkey
     monkey.patch_all()
 
-import random
-import time
-
-from celery_dyrygent.tasks import register_workflow_processor
-
 import sys
 import logging
+from pypeline.pipeline.chained_task import ChainedTask
+from celery_dyrygent.tasks import register_workflow_processor
 from typing import List
 from celery import Celery
 from pypeline.logging_config import setup_logging
 from pypeline.utils.module_utils import SermosModuleLoader
-from pypeline.utils.task_utils import PipelineGenerator, PipelineResult, \
+from pypeline.utils.task_utils import PipelineResult, \
     get_service_config_for_worker
 from pypeline.extensions import sermos_config, sermos_client_version
 from pypeline import __version__
 
 logger = logging.getLogger('celery')
 ENABLE_TOOLS = str(os.environ.get('ENABLE_TOOLS', 'false')).lower() == 'true'
 CELERY_TASKS_ACK_LATE = str(os.environ.get('CELERY_TASKS_ACK_LATE', 'false')).lower() == 'true'
@@ -33,54 +28,14 @@
 
 setup_logging(app_version=__version__,
               client_version=sermos_client_version,
               default_level=LOG_LEVEL,
               overload_elasticsearch=OVERLOAD_ES,
               establish_logging_config=True)
 
-
-def pipeline_retry(event: dict):
-    """ Handle pipeline retry and deadletter logic.
-    """
-    access_key = event.get('access_key', None)
-    pipeline_id = event.get('pipeline_id', None)
-    execution_id = event.get('execution_id', None)
-    if pipeline_id is None or execution_id is None:
-        logger.error(f"Unable to retry pipeline {pipeline_id} / "
-                     f"execution {execution_id}.")
-        return False
-
-    # generate_chain() will return `None` if the pipeline has exceeded
-    # max retry count or other erorrs happen.
-    gen = PipelineGenerator(pipeline_id=pipeline_id,
-                            access_key=access_key,
-                            execution_id=execution_id,
-                            queue=event.get('queue', None),
-                            default_task_ttl=event.get('default_task_ttl',
-                                                       None),
-                            add_retry=event.get('add_retry', False),
-                            chain_payload=event.get('chain_payload', None))
-
-    if gen.good_to_go:
-        chain = gen.generate_chain()
-        if chain is not None:
-            # Exponential backoff
-            exponential_backoff = min((3 ** gen.pipeline_wrapper.retry_count) +
-                                      (random.randint(0, 1000) / 1000),
-                                      DEFAULT_RETRY_TASK_MAX_TTL)
-            logger.debug(f"Exponential backoff sleep {exponential_backoff}")
-            time.sleep(exponential_backoff)
-            # Kick it off again.
-            chain.apply_async()
-
-    logger.warning(f"Pipeline retry was invoked for {pipeline_id} "
-                   f"({execution_id})")
-    return True
-
-
 def task_chain_regulator(*args, **kwargs):
     """ Utility task to ensure celery properly waits between groups in a chain.
 
         For a chain(), if each element is a group() then celery does not
         properly adhere to the chain elements occurring sequentially. If you
         insert a task that is not a group() in between, though, then the
         chain operates as expected.
@@ -110,16 +65,14 @@
         self.config = config if config else {}
         self.celery = celery_instance
 
     def _get_default_tasks(self) -> List[dict]:
         """ Sermos provides default tasks that all workers should know about.
         """
         return [{
-            'handler': 'pypeline.celery.pipeline_retry'
-        }, {
             'handler': 'pypeline.celery.task_chain_regulator'
         }, {
             'handler': 'pypeline.celery.pipeline_success'
         }]
 
     def generate(self):
         """ Loads methods based on sermos config file and decorates them as
@@ -143,23 +96,41 @@
         # registeredTasks list. This allows each worker to only attempt
         # bootstrapping those tasks that are relevant to the worker and not, for
         # example, attempt to import a package that's not used by this worker
         service = get_service_config_for_worker(self.config)
         if not service:
             return
         for task in service.get('registeredTasks', []):
+            pipeline_meta = None
+            for pipeline_key, pipeline in sermos_config['pipelines'].items():
+                pipeline_config = pipeline["config"]
+                pipeline_tasks = [t["handler"] for t in pipeline_config["taskDefinitions"].values()]
+                if task["handler"] in pipeline_tasks:
+                    pipeline_meta = pipeline_config["metadata"]
+                    break
+
             try:
                 worker_path = task['handler']  # Required, no default
 
                 tmp_handler = self.get_callable(worker_path)
 
                 # Decorate the method as a celery task along with a default
                 # queue if provided in config. Set ChainedTask as the base
                 # which allows chained tasks to pass kwargs correctly.
-                tmp_handler = self.celery.task(tmp_handler)
+                if pipeline_meta and pipeline_meta["maxRetry"] > 0:
+                    tmp_handler = self.celery.task(
+                        tmp_handler,
+                        autoretry_for=(Exception,),
+                        max_retries=pipeline_meta["maxRetry"],
+                        retry_backoff=pipeline_meta["retryBackoff"],
+                        retry_jitter=pipeline_meta["retryJitter"],
+                        retry_backoff_max=pipeline_meta["retryBackoffMax"]
+                    )
+                else:
+                    tmp_handler = self.celery.task(tmp_handler)
             except Exception as e:
                 logger.warning(f"Unable to add a task to celery: {e}")
         # Sermos provides default tasks that all workers should know about, add
         # them here.
         for task in self._get_default_tasks():
             tmp_handler = self.get_callable(task['handler'])
             tmp_handler = self.celery.task(tmp_handler)
@@ -169,48 +140,14 @@
     """ Configure Sermos-compatible Celery instance. Primarily this means
     compatibility with Pipelines and Scheduled Tasks through injecting the
     event kwarg. Also sets prebaked defaults that can be overloaded by user.
     """
     REDIS_URL = os.environ.get('REDIS_URL', 'redis://localhost:6379/0')
     CELERY_BROKER_URL = os.environ.get('CELERY_BROKER_URL', REDIS_URL)
     CELERY_RESULT_BACKEND = os.environ.get('CELERY_RESULT_BACKEND', REDIS_URL)
-    TaskBase = celery.Task
-
-    class ChainedTask(TaskBase):
-        """ A Celery Task that is used as the _base_ for all dynamically
-        generated tasks (by GenerateCeleryTasks().generate()). This injects
-        `event` into every task's signature, which allows pipelines to pass
-        event information easily through a chain.
-        """
-        abstract = True
-        autoretry_for = (Exception,)
-        max_retries = DEFAULT_MAX_RETRY
-        retry_backoff = True
-        retry_jitter = True
-
-        def __call__(self, *args, **kwargs):
-            """ Allow the return value of one task to update the kwargs of a
-                subsequent task if it's a dictionary. Important to the function
-                of a pipeline to allow event information to flow easily.
-            """
-            # Inject app context
-            if len(args) == 1 and isinstance(args[0], dict):
-                kwargs.update(args[0])
-                args = ()
-
-            # Event holds information used in PipelineRunWrapper and
-            # other areas.
-            if 'event' not in kwargs.keys():
-                kwargs['event'] = {}
-            # This is a special worker from dyrygent that orchestrates our
-            # pipelines.  It provides a patch in fix for celery's poor
-            # implementation of Canvas work-flows
-            if self.__name__ == 'workflow_processor':
-                kwargs.pop('event', None)
-            return super(ChainedTask, self).__call__(*args, **kwargs)
 
     celery.Task = ChainedTask
 
     # Configure the broker and tasks
     celery.conf.broker_url = CELERY_BROKER_URL
 
     # Use our custom database scheduler for dynamic celery beat updates.
@@ -226,15 +163,14 @@
       celery.conf.task_compression = PIPELINE_CHORD_COMPRESSION
 
     # NOTE: The broker URL may not be the best result backend. For example,
     # When using Rabbit as the broker (recommended), you should use Redis
     # as the result backend, as Rabbit has horrible support as backend.
     celery.conf.result_backend = CELERY_RESULT_BACKEND
     celery.conf.task_ignore_result = False  # Must not ignore for Chords
-    celery.conf.task_acks_late = False  # Check per worker
     celery.conf.result_expires = int(
         os.environ.get('CELERY_RESULT_EXPIRES', 10800))  # 3 hours by default
     celery.conf.broker_pool_limit = int(os.environ.get('BROKER_POOL_LIMIT',
                                                        10))
     celery.conf.worker_max_tasks_per_child = int(
         os.environ.get('MAX_TASKS_PER_CHILD', 100))
     celery.conf.task_soft_time_limit =\
```

### Comparing `scalable-pypeline-1.1.5/pypeline/celery_beat.py` & `scalable-pypeline-1.2.0/pypeline/celery_beat.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/constants.py` & `scalable-pypeline-1.2.0/pypeline/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import os
 from urllib.parse import urljoin
 
 API_PATH_V1 = '/api/v1'
 
 DEFAULT_RESULT_TTL = 86400  # seconds (1 day)
 DEFAULT_TASK_TTL = 60  # seconds (1 minute)
-DEFAULT_RETRY_TASK_MAX_TTL = 300
-DEFAULT_MAX_RETRY = 10
+DEFAULT_MAX_RETRY = 3
 DEFAULT_REGULATOR_TASK = 'pypeline.celery.task_chain_regulator'
 DEFAULT_SUCCESS_TASK = 'pypeline.celery.pipeline_success'
-DEFAULT_RETRY_TASK = 'pypeline.celery.pipeline_retry'
 
 CHAIN_SUCCESS_MSG = 'Chain built successfully ...'
 CHAIN_FAILURE_MSG = 'Chain failed to build ...'
 
 PIPELINE_RUN_WRAPPER_CACHE_KEY = 'sermos_{}_{}'  # pipeline_id + execution_id
 PIPELINE_RESULT_CACHE_KEY = 'sermos_result_{}'  # execution_id
 
@@ -48,14 +46,16 @@
 DEPLOYMENTS_URL = "{}deployments/{}"
 DEPLOYMENTS_DEPLOY_URL = "{}deployments/{}/deploy"
 DEPLOYMENTS_SERVICES_URL = "{}deployments/{}/services"
 DEPLOYMENTS_SERVICE_URL = "{}deployments/{}/services/{}"
 DEFAULT_AUTH_URL = urljoin(DEFAULT_BASE_URL, 'auth')
 USING_SERMOS_CLOUD = DEFAULT_BASE_URL != LOCAL_DEPLOYMENT_VALUE
 DEFAULT_CONFIG_RETRIEVAL_PAGE_SIZE = 25
+WORKFLOW_PROCESSOR_QUEUE = os.environ.get('WORKFLOW_PROCESSOR_QUEUE', 'default')
+
 # Default 'responses' dictionary when decorating endpoints with @api.doc()
 # Extend as necessary.
 API_DOC_RESPONSES = {
     200: {
         'code': 200,
         'description': 'Successful response.'
     },
```

### Comparing `scalable-pypeline-1.1.5/pypeline/extensions.py` & `scalable-pypeline-1.2.0/pypeline/extensions.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/__init__.py` & `scalable-pypeline-1.2.0/pypeline/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/api/pipelines.py` & `scalable-pypeline-1.2.0/pypeline/flask/api/pipelines.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from celery.canvas import _chain
 from celery_dyrygent.workflows import Workflow
 from flask import jsonify, request, abort
 from flask_smorest import Blueprint
 from flask.views import MethodView
 from marshmallow import Schema, fields
 from marshmallow.exceptions import ValidationError
-from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS, API_PATH_V1
+from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS, API_PATH_V1,\
+    WORKFLOW_PROCESSOR_QUEUE
 from pypeline.flask.decorators import require_accesskey
 from pypeline.flask.api.utils import chain_helper
 from pypeline.utils.task_utils import PipelineResult
 from pypeline.utils.config_utils import retrieve_latest_pipeline_config
 from pypeline.pipeline_config_schema import BasePipelineSchema, PipelineSchemaV1
 
 logger = logging.getLogger(__name__)
@@ -136,15 +137,14 @@
             ],
             tags=['Pipelines'])
     @bp.arguments(InvokePipelineSchema)
     @bp.response(InvokePipelineResponseSchema)
     def post(self, payload: dict, pipeline_id: str):
         """ Invoke a pipeline by it's ID; optionally provide pipeline arguments.
         """
-
         access_key = request.headers.get('accesskey')
         pipeline_config = retrieve_latest_pipeline_config(
             pipeline_id=pipeline_id, access_key=access_key)
 
         if pipeline_config is None:
             return abort(404)
 
@@ -160,17 +160,30 @@
                                access_key=access_key,
                                chain_payload=payload)
 
             if gen.chain is None:
                 abort(400, message=gen.loading_message)
 
             chain: _chain = gen.chain
-            wf: Workflow = Workflow()
+            wf: Workflow = Workflow({"queue": WORKFLOW_PROCESSOR_QUEUE})
             wf.add_celery_canvas(chain)
             wf.apply_async()
+
+            celery_task_status = []
+            for node in wf.nodes:
+                celery_task = dict(
+                    name=wf.nodes[node].signature.name,
+                    task_id=node,
+                    status="RUNNING",
+                    retries=0
+                )
+                celery_task_status.append(celery_task)
+
+            gen.pipeline_wrapper.celery_task_status = celery_task_status
+            gen.pipeline_wrapper.save_to_cache()
             retval['status'] = 'success'
             retval['execution_id'] = gen.execution_id
             # Initialize the cached result
             pr = PipelineResult(gen.execution_id, status='pending')
             pr.save()
 
         except Exception as e:
```

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/api/schedules.py` & `scalable-pypeline-1.2.0/pypeline/flask/api/schedules.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/api/utils.py` & `scalable-pypeline-1.2.0/pypeline/flask/api/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """ Utilities for Sermos APIs and interacting with Pipelines/Schedules
 """
 import logging
 from typing import Union
-from pypeline.utils.task_utils import PipelineGenerator
+
+from pypeline.pipeline.generator import PipelineGenerator
 
 logger = logging.getLogger(__name__)
 
 
 def chain_helper(pipeline_id: str,
                  access_key: Union[str, None] = None,
                  chain_payload: Union[dict, None] = None,
-                 add_retry: bool = True,
                  queue: Union[str, None] = None,
                  default_task_ttl: int = None):
     """ Helper method to generate a pipeline chain *with* error handling.
 
         Usage:
           my_chain = chain_helper('pipeline-name')
           my_chain.delay()
     """
     # Get our pipeline. The PipelineGenerator will use the PipelineRunWrapper
     # to cache this "run" of the pipeline.
     gen = PipelineGenerator(pipeline_id,
                             access_key=access_key,
                             queue=queue,
                             default_task_ttl=default_task_ttl,
-                            add_retry=add_retry,
                             chain_payload=chain_payload)
     if gen.good_to_go:
         # Generate our 'chain', which is the grouping of celery constructs that
         # allows our dag to run asynchronously and synchronously according to
         # the adjacency list defined in our pipeline configuration.
         gen.generate_chain()
```

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/decorators.py` & `scalable-pypeline-1.2.0/pypeline/flask/decorators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/flask/flask_sermos.py` & `scalable-pypeline-1.2.0/pypeline/flask/flask_sermos.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/generators.py` & `scalable-pypeline-1.2.0/pypeline/generators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/logging_config.py` & `scalable-pypeline-1.2.0/pypeline/logging_config.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/pipeline_config_schema.py` & `scalable-pypeline-1.2.0/pypeline/pipeline_config_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,23 +22,65 @@
     """
     queue = fields.String(required=True,
                           description="Default queue for all pipeline tasks.",
                           example="default-queue-name")
 
     maxRetry = fields.Integer(
         required=False,
-        description="Max number of retries for a pipeline.",
+        description="A number. Maximum number of retries before giving up. "
+                    "A value of None means task will retry forever. "
+                    "By default, this option is set to 3.",
         default=3,
         example=3)
 
     maxTtl = fields.Integer(required=False,
-                            description="Max TTL for a pipeline in seconds.",
+                            description="The soft time limit, in seconds, "
+                                        "for this task. When not set the "
+                                        "workers default is used.  The hard "
+                                        "time limit will be derived from this"
+                                        "field, by adding 10 seconds.",
                             default=60,
                             example=60)
 
+    retryBackoff = fields.Integer(
+        required=False,
+        description="A number. If this option is set , it is used as a delay"
+                    " factor. For example, if this option is set to 3, the"
+                    " first retry will delay 3 seconds, the second will delay"
+                    "  6 seconds, the third will delay 12 seconds, the fourth"
+                    " will delay 24 seconds, and so on. By default, this"
+                    " option is set to False, and autoretries will not"
+                    "  be delayed.",
+        default=3,
+        example=3)
+
+    retryJitter = fields.Boolean(
+        required=False,
+        description="A boolean. Jitter is used to introduce randomness into "
+                    "exponential backoff delays, to prevent all tasks in the "
+                    "queue from being executed simultaneously. If this option "
+                    "is set to True, the delay value calculated by "
+                    "retry_backoff is treated as a maximum, and the actual "
+                    "delay value will be a random number between zero and that "
+                    "maximum. By default, this option is set to True.",
+        default=False,
+        example=True)
+
+    retryBackoffMax = fields.Integer(
+        required=False,
+        description="A boolean. Jitter is used to introduce randomness into "
+                    "exponential backoff delays, to prevent all tasks in the "
+                    "queue from being executed simultaneously. If this option "
+                    "is set to True, the delay value calculated by "
+                    "retry_backoff is treated as a maximum, and the actual "
+                    "delay value will be a random number between zero and "
+                    "that maximum. By default, this option is set to True.",
+        default=600,
+        example=600)
+
 
 class TaskDefinitionsSchema(ExcludeUnknownSchema):
     """ Schema for a single task's configuration
     """
     handler = fields.String(required=True,
                             description="Path to the worker task definition",
                             example="client.workers.my_task")
@@ -47,22 +89,14 @@
                             description="Max TTL for a task in seconds.",
                             default=60,
                             example=60)
 
     queue = fields.String(required=False,
                           description="Non-default queue for this task.",
                           example="custom-queue-name")
-    # payload_args = fields.List(
-    #     fields.Dict(keys=fields.String(),
-    #                    values=fields.Nested(PayloadArgKwargSchema)))
-    # payload_kwargs = fields.List(
-    #     fields.Dict(keys=fields.String(),
-    #                    values=fields.Nested(PayloadArgKwargSchema)))
-    # model_version = fields.String()
-    # arbitrary other stuff passed to task?
 
 
 class PipelineConfigSchemaV1(Schema):
     """ Overall pipeline configuration schema
     """
     metadata = fields.Nested(
         MetadataSchema,
@@ -133,17 +167,18 @@
     @validates_schema
     def validate_pipeline(self, data, **kwargs):
         schema_version = data['schemaVersion']
         PipelineSchema = BasePipelineSchema.get_by_version(schema_version)
         schema = PipelineSchema(exclude=['name', 'description'])
         schema.load(data)
 
-class PipelineSchemaV1(BasePipelineSchema):
 
+class PipelineSchemaV1(BasePipelineSchema):
     __schema_version__ = 1
+
     class Meta:
         unknown = EXCLUDE
 
     config = fields.Nested(
         PipelineConfigSchemaV1,
         required=True,
         description="Metadata and configuration information for this pipeline."
@@ -175,15 +210,14 @@
         elif config_yaml is not None:
             self.config = yaml.safe_load(config_yaml)
 
         if schema_version is None:
             PipelineSchema = BasePipelineSchema.get_latest()
         else:
             PipelineSchema = BasePipelineSchema.get_by_version(schema_version)
-            
 
         self.is_valid = False
         self.validated_config = {}
         self.validation_errors = {}
         try:
             # https://github.com/marshmallow-code/marshmallow/issues/377
             # See issue above when migrating to marshmallow 3
```

### Comparing `scalable-pypeline-1.1.5/pypeline/schedule_config_schema.py` & `scalable-pypeline-1.2.0/pypeline/schedule_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/utils/config_utils.py` & `scalable-pypeline-1.2.0/pypeline/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/utils/graph_utils.py` & `scalable-pypeline-1.2.0/pypeline/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/utils/module_utils.py` & `scalable-pypeline-1.2.0/pypeline/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.1.5/pypeline/utils/task_utils.py` & `scalable-pypeline-1.2.0/pypeline/utils/task_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """ Utilities for running and managing tasks inside pipelines.
 """
 import os
 import logging
+import typing
 import uuid
 from typing import List, Any, Union
 from networkx.classes.digraph import DiGraph
-from celery import chain, signature, chord
+from celery import signature
 
 from pypeline.constants import DEFAULT_TASK_TTL, \
-    DEFAULT_REGULATOR_TASK, CHAIN_SUCCESS_MSG, CHAIN_FAILURE_MSG, \
-    PIPELINE_RUN_WRAPPER_CACHE_KEY, DEFAULT_SUCCESS_TASK, DEFAULT_RESULT_TTL, \
-    PIPELINE_RESULT_CACHE_KEY, DEFAULT_RETRY_TASK, DEFAULT_MAX_RETRY, \
-    DEFAULT_RETRY_TASK_MAX_TTL
-from pypeline.utils.graph_utils import get_execution_graph, get_chainable_tasks
-from pypeline.utils.config_utils import retrieve_latest_pipeline_config, \
-    load_json_config_from_redis, set_json_config_to_redis
+    PIPELINE_RUN_WRAPPER_CACHE_KEY, DEFAULT_RESULT_TTL, \
+    PIPELINE_RESULT_CACHE_KEY
+from pypeline.utils.graph_utils import get_execution_graph
+from pypeline.utils.config_utils import load_json_config_from_redis, set_json_config_to_redis
 from pypeline.pipeline_config_schema import PipelineConfigValidator
 
+
 logger = logging.getLogger(__name__)
 WORKER_NAME = os.environ.get('WORKER_NAME', None)
 
 
 def get_service_config_for_worker(sermos_config: dict,
                                   worker_name: str = None
                                   ) -> Union[dict, None]:
@@ -33,16 +32,15 @@
     if worker_name is None:
         worker_name = WORKER_NAME
     if worker_name is None:
         return None
 
     service_config = sermos_config.get('serviceConfig', [])
     for service in service_config:
-        if service['serviceType'] == 'celery-worker' and service[
-                'name'] == worker_name:
+        if service['name'] == worker_name:
             return service
 
     raise ValueError('Could not find a service config for worker '
                      f'`{worker_name}`. Make sure you have added the service in'
                      f' your sermos.yaml with `name: {worker_name}` and '
                      '`type: celery-worker`.')
 
@@ -77,39 +75,39 @@
         # First look on the pipeline configuration, if a max_ttl is specified,
         # then we're using that regardless.
         max_ttl = task_config.get('maxTtl', None)
 
         # If we still have None or 'default', set the default queue!
         if max_ttl in (None, 'default'):
             max_ttl = DEFAULT_TASK_TTL
-
+    task_id = str(uuid.uuid4())
     kwargs = {
         'event': {
             'access_key': access_key,
             'pipeline_id': pipeline_id,
-            'execution_id': execution_id
+            'execution_id': execution_id,
+            'task_id': task_id
         }
     }
     if custom_event_data is not None:
         kwargs['event'] = {**kwargs['event'], **custom_event_data}
 
-    # TODO where do we inject the 'event' data from sermos yaml schema?
-
     sig = signature(
         task_path,
         args=(),
         kwargs=kwargs,
         immutable=immutable,
-        task_id=str(uuid.uuid4()),
+        task_id=task_id,
         options={
             'queue': queue,
             'expires': 86400,  # Expire after 1 day. TODO make tunable.
             'soft_time_limit': max_ttl,
             'time_limit': max_ttl + 10,  # Add 10s buffer for cleanup
-        })
+        }
+    )
     return sig
 
 
 class PipelineRunWrapper:
     """ A wrapper for a single "run" of a Pipeline.
 
         A 'run' is defined as a single execution of a pipeline, a pipeline
@@ -123,14 +121,15 @@
         representation of the full 'run' including retry count and any payload
         that should be accessible to any step in the chain. Remember, a pipeline
         is running asynchronously and, as such, each node in the graph operates
         independent the others, this allows for consistent coordination.
     """
     pipeline_id: str = None
     pipeline_config: dict = None  # Pipeline configuration in dictionary format
+    celery_task_status: dict = None # This tracks the state of tasks within the pipeline
     dag_config: dict = None
     execution_id: str = None
     current_event: dict = None  # For single task when from_event(). NOT cached.
     cache_key: str = None  # Set on init
     max_ttl: int = 60  # Overloaded when pipeline_config provided and it's set
     max_retry: int = 3  # Overloaded when pipeline_config provided and it's set
     retry_count: int = 0
@@ -183,15 +182,15 @@
         in the wrapper. Style convention switching is to keep with the naming
         convention of all yaml files following camelCase to conform with k8s
         and all local python variables being snake_case. This extraction of
         the yaml file variables to place onto the wrapper object is done
         during the .load() stage.
         """
         return ('pipeline_config', 'max_ttl', 'max_retry', 'retry_count',
-                'chain_payload', 'pipeline_id')
+                'chain_payload', 'pipeline_id', 'celery_task_status')
 
     def _load_from_cache(self, is_retry=False):
         """ Attempt to load this PipelineRunWrapper from cache.
         """
         logger.debug(f"Attempting to load {self.cache_key} from cache")
         try:
             cached_wrapper = load_json_config_from_redis(self.cache_key)
@@ -211,14 +210,17 @@
                 logger.exception(e)
 
         if self.pipeline_config is None:
             raise ValueError("pipeline_config not set, invalid ...")
 
         return
 
+    def get_task_celery_status(self, task_id: type[uuid.uuid4()]) -> typing.Union[dict, None]:
+        return next(filter(lambda task: task["task_id"] == task_id, self.celery_task_status), None)
+
     def save_to_cache(self):
         """ Save current state of PipelineRunWrapper to cache, json serialized.
             Re-set the key's TTL
 
             TODO: Lock this so no race condition on concurrent steps.
         """
         logger.debug(f"Saving {self.cache_key} to cache")
@@ -273,15 +275,16 @@
                 # artifact of the caching process. We also explicitly skip
                 # pipeline_id, max_retry, and max_ttl keys because those are
                 # metadata keys in the pipeline_config and are camel case
                 # (pipelineId/maxRetry/maxTtl), we set them on this wrapper
                 # object purely for convenience and to provide logical defaults.
                 for key in self._cachable_keys:
                     if key in ('pipeline_config', 'pipeline_id', 'max_retry',
-                               'max_ttl', 'retry_count', 'chain_payload'):
+                               'max_retry', 'max_ttl', 'retry_count',
+                               'chain_payload', 'celery_task_status'):
                         continue
                     setattr(self, key, self.pipeline_config[key])
 
             # Validate pipeline config
             PipelineConfigValidator(config_dict=self.pipeline_config)
 
             # Initialize the actual pipeline configuration and execution graph
@@ -449,267 +452,14 @@
             'status': self.status,
             'result': self.result,
             'results': self.result,  # TODO Deprecate in future release
             'result_ttl': self.result_ttl
         }
 
 
-class PipelineGenerator(object):
-    """ Allows an API endpoint to generate a functional pipeline based on the
-        requested pipeline id. Allows API to then issue the tasks asynchronously
-        to initiate the pipeline. Thereafter, celery will monitor status and
-        handle success/failure modes so the API web worker can return
-        immediately.
-
-        The primary purpose is to unpack the pipeline config, create the
-        requisite cached entities to track pipeline progress, and apply the
-        chained pipeline tasks asynchronously so Celery can take over.
-
-        Usage:
-            gen = PipelineGenerator(pipeline_id)
-            chain = gen.generate_chain()
-            chain.on_error(custom_error_task.s())  # Optional add error handling
-            chain.delay()
-    """
-    def __init__(self,
-                 pipeline_id: str,
-                 access_key: str = None,
-                 execution_id: str = None,
-                 queue: str = None,
-                 default_task_ttl: int = None,
-                 regulator_queue: str = None,
-                 regulator_task: str = None,
-                 success_queue: str = None,
-                 success_task: str = None,
-                 retry_task: str = None,
-                 add_retry: bool = True,
-                 default_max_retry: int = None,
-                 chain_payload: dict = None):
-        super().__init__()
-        self.pipeline_id = pipeline_id
-        self.access_key = access_key
-
-        pipeline_config_api_resp = retrieve_latest_pipeline_config(
-            pipeline_id=self.pipeline_id, access_key=self.access_key)
-
-        if pipeline_config_api_resp is None:
-            raise ValueError("Unable to load Pipeline Configuration for "
-                             f"pipeline id: {self.pipeline_id} ...")
-
-        # The only part of the API response used for any 'pipeline config'
-        # is the `config` key. The API nests it under `config` to preserve
-        # ability to add additional detail at a later date.
-        self.pipeline_config = pipeline_config_api_resp.get('config', {})
-        schema_version = pipeline_config_api_resp.get('schemaVersion')
-        PipelineConfigValidator(config_dict=self.pipeline_config,
-                                schema_version=schema_version)
-
-        self.execution_id = execution_id  # UUID string
-        self.good_to_go = False  # Indicates initialization/loading success
-        self.loading_message = None  # Allows access to success/error messages
-        self.is_retry = False if self.execution_id is None else True
-        self.add_retry = add_retry
-        self.retry_task = retry_task\
-            if retry_task is not None else DEFAULT_RETRY_TASK
-
-        self.default_max_retry = default_max_retry \
-            if default_max_retry is not None else \
-            self.pipeline_config['metadata'].get('maxRetry', DEFAULT_MAX_RETRY)
-
-        # Queue on which to place tasks by default and default TTL per task
-        # These can be overridden in PipelineConfig.config['taskDefinitions']
-        self.queue = queue \
-            if queue is not None \
-            else self.pipeline_config['metadata']['queue']
-        self.default_task_ttl = default_task_ttl \
-            if default_task_ttl is not None else \
-            self.pipeline_config['metadata'].get('maxTtl', DEFAULT_TASK_TTL)
-
-        # See docstring in self._get_regulator()
-        self.regulator_queue = regulator_queue \
-            if regulator_queue is not None \
-            else self.pipeline_config['metadata']['queue']
-        self.regulator_task = regulator_task\
-            if regulator_task is not None else DEFAULT_REGULATOR_TASK
-
-        # See docstring in self._get_success_task()
-        self.success_queue = success_queue \
-            if success_queue is not None \
-            else self.pipeline_config['metadata']['queue']
-        self.success_task = success_task\
-            if success_task is not None else DEFAULT_SUCCESS_TASK
-
-        # Optional data to pass to each step in chain
-        self.chain_payload = chain_payload\
-            if chain_payload is not None else {}
-
-        self.pipeline_wrapper = None  # Allows access to the PipelineRunWrapper
-        self.chain = None  # Must be intentionally built with generate_chain()
-
-        try:
-            # Generate our wrapper for this pipeline_id / execution_id
-            self.pipeline_wrapper = PipelineRunWrapper(
-                pipeline_id=self.pipeline_id,
-                pipeline_config=self.pipeline_config,
-                execution_id=self.execution_id,
-                max_ttl=self.default_task_ttl,
-                max_retry=self.default_max_retry,
-                chain_payload=self.chain_payload)
-
-            # Loads pipeline config from remote or cache if it's already there
-            # `is_retry` will be True for any PipelineGenerator instantiated
-            # with an execution_id. This flag helps the wrapper increment the
-            # retry count and determine if this should be deadlettered.
-            # This step also saves the valid/initialized run wrapper to cache.
-            self.pipeline_wrapper.load(is_retry=self.is_retry)
-
-            # Set all variables that were established from the run wrapper
-            # initialization. Notably, default_task_ttl can be overloaded
-            # if the pipeline config has an explicit maxTtl set in metadata.
-            self.good_to_go = self.pipeline_wrapper.good_to_go
-            self.loading_message = self.pipeline_wrapper.loading_message
-            self.execution_id = self.pipeline_wrapper.execution_id
-
-        except Exception as e:
-            fail_msg = "Failed to load Pipeline for id {} ... {}".format(
-                self.pipeline_id, e)
-            self.loading_message = fail_msg
-            logger.error(fail_msg)
-            raise e
-
-    def _get_regulator(self):
-        """ Create a chain regulator celery task signature.
-
-            For a chain(), if each element is a group() then celery does not
-            properly adhere to the chain elements occurring sequentially. If you
-            insert a task that is not a group() in between, though, then the
-            chain operates as expected.
-        """
-        return signature(self.regulator_task,
-                         queue=self.regulator_queue,
-                         immutable=True)
-
-    def _get_success_task(self):
-        """ A final 'success' task that's added to the end of every pipeline.
-
-            This stores the 'success' state in the cached result. Users can
-            set other values by using TaskRunner().save_result()
-        """
-        return get_task_signature(task_path=self.success_task,
-                                  queue=self.success_queue,
-                                  pipeline_id=self.pipeline_id,
-                                  execution_id=self.execution_id)
-
-    def _get_retry_task(self):
-        """ The retry task will re-invoke a chain.
-        """
-        return get_task_signature(task_path=self.retry_task,
-                                  queue=self.queue,
-                                  access_key=self.access_key,
-                                  pipeline_id=self.pipeline_id,
-                                  execution_id=self.execution_id,
-                                  max_ttl=DEFAULT_RETRY_TASK_MAX_TTL,
-                                  custom_event_data={
-                                      'queue': self.queue,
-                                      'default_task_ttl':
-                                      self.default_task_ttl,
-                                      'add_retry': self.add_retry,
-                                      'chain_payload': self.chain_payload
-                                  })
-
-    def _get_signature(self, node):
-        """ Create a celery task signature based on a graph node.
-        """
-        metadata = self.pipeline_config['metadata']
-        node_config = self.pipeline_config['taskDefinitions'][node]
-
-        # Node config takes precedence, pipeline metadata as default
-        queue = node_config.get('queue', metadata['queue'])
-        max_ttl = node_config.get('maxTtl', metadata.get('maxTtl', None))
-
-        # Ensures task signatures include requisite information to retrieve
-        # PipelineRunWrapper from cache using the pipeline id, and execution id.
-        # We set immutable=True to ensure each client task can be defined
-        # with this specific signature (event)
-        # http://docs.celeryproject.org/en/master/userguide/canvas.html#immutability
-        return get_task_signature(task_path=node_config.get('handler'),
-                                  queue=queue,
-                                  access_key=self.access_key,
-                                  pipeline_id=self.pipeline_id,
-                                  execution_id=self.execution_id,
-                                  max_ttl=max_ttl,
-                                  immutable=True,
-                                  task_config=node_config)
-
-    def generate_chain(self):
-        """ Generate the full pipeline chain.
-        """
-        logger.debug(f'Starting Pipeline {self.pipeline_id}')
-
-        if not self.good_to_go:
-            logger.info("Chain deemed to be not good to go.")
-            if self.loading_message is None:
-                self.loading_message = CHAIN_FAILURE_MSG
-            return None
-
-        try:
-            # Create the task chain such that all concurrent tasks are grouped
-            # and all high level node groups are run serially
-            G = self.pipeline_wrapper.execution_graph
-
-            total_tasks = 0
-            pipeline_chain = []
-            chainable_tasks = get_chainable_tasks(G, None, [])
-
-            # Current chord+chain solution based on
-            # https://stackoverflow.com/questions/15123772/celery-chaining-groups-and-subtasks-out-of-order-execution
-            # Look also at last comment from Nov 7, 2017 here
-            # https://github.com/celery/celery/issues/3597
-            # Big outstanding bug in Celery related to failures in chords that
-            # results in really nasty log output. See
-            # https://github.com/celery/celery/issues/4834
-            for i, node_group in enumerate(chainable_tasks):
-                total_tasks += len(node_group)
-                this_group = []
-                for node in node_group:
-                    node_signature = self._get_signature(node)
-                    this_group.append(node_signature)
-
-                if len(this_group) <= 1:
-                    this_group.append(self._get_regulator())
-
-                the_chord = chord(header=this_group,
-                                  body=self._get_regulator())
-
-                pipeline_chain.append(the_chord)
-
-            # Add a 'finished/success' task to the end of all pipelines
-            pipeline_chain.append(
-                chord(header=self._get_success_task(),
-                      body=self._get_regulator()))
-
-            the_chain = chain(*pipeline_chain)
-
-            # Add retry
-            if self.add_retry:
-                the_chain.link_error(self._get_retry_task())
-
-            self.loading_message = CHAIN_SUCCESS_MSG
-
-            self.chain = the_chain
-        except Exception as e:
-            self.loading_message = CHAIN_FAILURE_MSG + " {}".format(e)
-            logger.exception(e)
-            the_chain = None
-
-        self.chain = the_chain
-
-        return the_chain
-
-
 class TaskRunner:
     """ Run tasks in Sermos
     """
     @classmethod
     def save_result(cls):
         """ Save a task result
         """
@@ -733,15 +483,14 @@
                 queue (str): The queue on which to place this task.
                     Ensure there are workers available to accept work on
                     that queue.
                 max_ttl (int): Optional. Max time to live for the issued task.
                     If not specified, system default is used.
         """
         try:
-            # TODO consider whether to add access key/deployment id here
             worker = get_task_signature(task_path=task_path,
                                         queue=queue,
                                         max_ttl=max_ttl,
                                         custom_event_data=task_payload)
             worker.delay()
         except Exception as e:
             logger.error(f"Failed to publish work ... {e}")
@@ -785,15 +534,15 @@
             if len(task_payload_list) > 0:
                 for idx in range(len(task_payload_list)):
                     if idx % max_per_task == 0:
                         custom_event_data = {
                             grouping_key:
                             task_payload_list[idx:idx + max_per_task]
                         }
-                        # TODO consider whether to add access key/deployment id here
+
                         worker = get_task_signature(
                             task_path=task_path,
                             queue=queue,
                             max_ttl=max_ttl,
                             custom_event_data=custom_event_data)
                         worker.delay()
         except Exception as e:
```

### Comparing `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/PKG-INFO` & `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.1.5
+Version: 1.2.0
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/SOURCES.txt` & `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 pypeline/flask/__init__.py
 pypeline/flask/decorators.py
 pypeline/flask/flask_sermos.py
 pypeline/flask/api/__init__.py
 pypeline/flask/api/pipelines.py
 pypeline/flask/api/schedules.py
 pypeline/flask/api/utils.py
+pypeline/pipeline/__init__.py
+pypeline/pipeline/chained_task.py
+pypeline/pipeline/generator.py
 pypeline/utils/__init__.py
 pypeline/utils/config_utils.py
 pypeline/utils/graph_utils.py
 pypeline/utils/module_utils.py
 pypeline/utils/task_utils.py
 scalable_pypeline.egg-info/PKG-INFO
 scalable_pypeline.egg-info/SOURCES.txt
```

### Comparing `scalable-pypeline-1.1.5/scalable_pypeline.egg-info/requires.txt` & `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 [dev]
 honcho>=1.0.1
 awscli>=1.11
 pylint>=2.5.3
 pip-licenses
 
 [flask]
-Flask>=1.1.1
-flask-smorest>=0.23.0
+Werkzeug==2.0.3
+Flask<2,>=1.1.2
+flask-smorest<0.29,>=0.23.0
+Jinja2==3.0.3
 
 [test]
 pytest-cov<3,>=2.6.1
 tox<4,>=3.14.1
 mock<2,>=1
-moto<2,>=1.3.16
+moto>=1.3.16
 responses<0.11,>=0.10.16
 fakeredis<3,>=2.10.3
 importlib-metadata<5,>=4.12
 
 [web]
 gunicorn
-gevent
+gevent<22,>=21.12.0
 
 [workers]
 celery[redis]<6,>=5.1.2
 networkx>=2.4
```

### Comparing `scalable-pypeline-1.1.5/setup.py` & `scalable-pypeline-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,27 +161,31 @@
     packages=packages,
     include_package_data=True,
     cmdclass=cmdclass,
     ext_modules=ext_modules,
     install_requires=install_requires,
     extras_require={
         'build': ['wheel', 'twine'],
-        'flask':
-        ['Flask>=1.1.1', 'flask-smorest>=0.23.0'],
-        'web': ['gunicorn', 'gevent'],
+        'flask': [
+            'Werkzeug==2.0.3',
+            'Flask>=1.1.2,<2',
+            'flask-smorest>=0.23.0,<0.29',
+            'Jinja2==3.0.3',
+        ],
+        'web': ['gunicorn', 'gevent>=21.12.0,<22'],
         'workers': [
             "celery[redis]>=5.1.2,<6",
             'networkx>=2.4',
         ],
         'dev':['honcho>=1.0.1', 'awscli>=1.11', 'pylint>=2.5.3', 'pip-licenses'],
         'test': [
             'pytest-cov>=2.6.1,<3',
             'tox>=3.14.1,<4',
             'mock>=1,<2',
-            'moto>=1.3.16,<2',
+            'moto>=1.3.16',
             'responses>=0.10.16,<0.11',
             'fakeredis>=2.10.3,<3',
             'importlib-metadata>=4.12,<5'
         ]
     },
     entry_points="""
     [console_scripts]
```

### Comparing `scalable-pypeline-1.1.5/tests/fixtures/s3_fixtures.py` & `scalable-pypeline-1.2.0/tests/fixtures/s3_fixtures.py`

 * *Files identical despite different names*

