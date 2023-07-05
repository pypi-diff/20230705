# Comparing `tmp/taskhawk-4.2.1.tar.gz` & `tmp/taskhawk-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskhawk-4.2.1.tar", last modified: Sat Jun  3 00:17:03 2023, max compression
+gzip compressed data, was "taskhawk-4.3.0.tar", last modified: Wed Jul  5 18:36:58 2023, max compression
```

## Comparing `taskhawk-4.2.1.tar` & `taskhawk-4.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070654 taskhawk-4.2.1/
--rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.2.1/CONTRIBUTORS.txt
--rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.2.1/LICENSE.md
--rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.2.1/MANIFEST.in
--rw-r--r--   0 maru       (501) staff       (20)     5395 2023-06-03 00:17:03.070708 taskhawk-4.2.1/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.2.1/README.rst
--rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.2.1/pyproject.toml
--rw-r--r--   0 maru       (501) staff       (20)      316 2023-06-03 00:17:03.070920 taskhawk-4.2.1/setup.cfg
--rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.2.1/setup.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.067542 taskhawk-4.2.1/taskhawk/
--rw-r--r--   0 maru       (501) staff       (20)      632 2023-06-03 00:17:01.000000 taskhawk-4.2.1/taskhawk/__init__.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.068911 taskhawk-4.2.1/taskhawk/backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     9886 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/backends/aws.py
--rw-r--r--   0 maru       (501) staff       (20)     6872 2022-11-30 05:33:20.000000 taskhawk-4.2.1/taskhawk/backends/base.py
--rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)    11346 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/backends/gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/import_utils.py
--rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/utils.py
--rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/commands.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.069021 taskhawk-4.2.1/taskhawk/conf/
--rw-r--r--   0 maru       (501) staff       (20)     6931 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/conf/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/consumer.py
--rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.2.1/taskhawk/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/models.py
--rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/publisher.py
--rw-r--r--   0 maru       (501) staff       (20)     7975 2022-04-13 05:43:22.000000 taskhawk-4.2.1/taskhawk/task_manager.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.068164 taskhawk-4.2.1/taskhawk.egg-info/
--rw-r--r--   0 maru       (501) staff       (20)     5395 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)      959 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/SOURCES.txt
--rw-r--r--   0 maru       (501) staff       (20)        1 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/dependency_links.txt
--rw-r--r--   0 maru       (501) staff       (20)      478 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/requires.txt
--rw-r--r--   0 maru       (501) staff       (20)        9 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/top_level.txt
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070083 taskhawk-4.2.1/tests/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.2.1/tests/conftest.py
--rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/settings.py
--rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.2.1/tests/tasks.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070535 taskhawk-4.2.1/tests/test_backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_backends/test_aws.py
--rw-r--r--   0 maru       (501) staff       (20)    10558 2021-07-06 19:19:15.000000 taskhawk-4.2.1/tests/test_backends/test_base.py
--rw-r--r--   0 maru       (501) staff       (20)    12496 2022-11-30 05:33:20.000000 taskhawk-4.2.1/tests/test_backends/test_gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_commands.py
--rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.2.1/tests/test_consumer.py
--rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_models.py
--rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_publisher.py
--rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_settings.py
--rw-r--r--   0 maru       (501) staff       (20)     8474 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789808 taskhawk-4.3.0/
+-rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.3.0/CONTRIBUTORS.txt
+-rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.3.0/LICENSE.md
+-rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.3.0/MANIFEST.in
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2023-07-05 18:36:58.789857 taskhawk-4.3.0/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.3.0/README.rst
+-rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.3.0/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      316 2023-07-05 18:36:58.790067 taskhawk-4.3.0/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.3.0/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.785872 taskhawk-4.3.0/taskhawk/
+-rw-r--r--   0 maru       (501) staff       (20)      632 2023-07-05 18:36:57.000000 taskhawk-4.3.0/taskhawk/__init__.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.787693 taskhawk-4.3.0/taskhawk/backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     9886 2023-06-03 00:08:40.000000 taskhawk-4.3.0/taskhawk/backends/aws.py
+-rw-r--r--   0 maru       (501) staff       (20)     6936 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/backends/base.py
+-rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)    11745 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/backends/gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/import_utils.py
+-rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.3.0/taskhawk/backends/utils.py
+-rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/commands.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.787853 taskhawk-4.3.0/taskhawk/conf/
+-rw-r--r--   0 maru       (501) staff       (20)     7020 2023-07-05 18:34:53.000000 taskhawk-4.3.0/taskhawk/conf/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.3.0/taskhawk/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/models.py
+-rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.3.0/taskhawk/publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)     7975 2022-04-13 05:43:22.000000 taskhawk-4.3.0/taskhawk/task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.786511 taskhawk-4.3.0/taskhawk.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)      959 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)      478 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        9 2023-07-05 18:36:58.000000 taskhawk-4.3.0/taskhawk.egg-info/top_level.txt
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789197 taskhawk-4.3.0/tests/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.3.0/tests/conftest.py
+-rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/settings.py
+-rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.3.0/tests/tasks.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-05 18:36:58.789689 taskhawk-4.3.0/tests/test_backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_backends/test_aws.py
+-rw-r--r--   0 maru       (501) staff       (20)    10558 2021-07-06 19:19:15.000000 taskhawk-4.3.0/tests/test_backends/test_base.py
+-rw-r--r--   0 maru       (501) staff       (20)    13090 2023-07-05 18:34:53.000000 taskhawk-4.3.0/tests/test_backends/test_gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_commands.py
+-rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.3.0/tests/test_consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_models.py
+-rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_settings.py
+-rw-r--r--   0 maru       (501) staff       (20)     8474 2020-03-12 19:54:19.000000 taskhawk-4.3.0/tests/test_task_manager.py
```

### Comparing `taskhawk-4.2.1/LICENSE.md` & `taskhawk-4.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/PKG-INFO` & `taskhawk-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.2.1
+Version: 4.3.0
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.2.1/README.rst` & `taskhawk-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/setup.py` & `taskhawk-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/__init__.py` & `taskhawk-4.3.0/taskhawk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~
 
 :copyright: (c) 2013-2017 by the Automatic Labs.
 """
 
 
 # semantic versioning (http://semver.org/)
-VERSION = '4.2.1'
+VERSION = '4.3.0'
 
 
 try:
     from .backends.aws import AWSMetadata  # noqa
 except ImportError:
     pass
 try:
```

### Comparing `taskhawk-4.2.1/taskhawk/backends/aws.py` & `taskhawk-4.3.0/taskhawk/backends/aws.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/backends/base.py` & `taskhawk-4.3.0/taskhawk/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
         log_published_message(message_body, result)
 
         return result
 
 
 class TaskhawkConsumerBaseBackend(TaskhawkBaseBackend):
+    def heartbeat_hook_kwargs(self) -> dict:
+        return {}
+
     @staticmethod
     def pre_process_hook_kwargs(queue_message) -> dict:
         return {}
 
     @staticmethod
     def post_process_hook_kwargs(queue_message) -> dict:
         return {}
```

### Comparing `taskhawk-4.2.1/taskhawk/backends/gcp.py` & `taskhawk-4.3.0/taskhawk/backends/gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,17 @@
                 f'taskhawk-{settings.TASKHAWK_QUEUE.lower()}{get_priority_suffix(priority)}{"-dlq" if dlq else ""}',
             )
             self._dlq_topic_path: str = pubsub_v1.PublisherClient.topic_path(
                 cloud_project,
                 f'taskhawk-{settings.TASKHAWK_QUEUE.lower()}{get_priority_suffix(priority)}-dlq',
             )
 
+    def heartbeat_hook_kwargs(self) -> dict:
+        return {"error_count": self.error_count}
+
     @property
     def publisher(self):
         if self._publisher is None:
             with _seed_credentials():
                 self._publisher = pubsub_v1.PublisherClient()
         return self._publisher
 
@@ -198,27 +201,29 @@
             messages = self.subscriber.pull(
                 subscription=self._subscription_path,
                 max_messages=num_messages,
                 retry=None,
                 timeout=settings.GOOGLE_PUBSUB_READ_TIMEOUT_S,
             ).received_messages
 
-            if self._error_count:
-                self._error_count = 0
+            self._error_count = 0
 
             return messages
         except DeadlineExceeded:
             logger.debug(f"Pulling deadline exceeded subscription={self._subscription_path}")
             return []
         except ServiceUnavailable as err:
             logger.debug(f"Service Unavailable while pulling exception={err}, subscription={self._subscription_path}")
             self._error_count += 1
             return []
+        finally:
+            self._call_heartbeat_hook()
 
     def process_message(self, queue_message: ReceivedMessage) -> None:
+        self._call_heartbeat_hook()
         self.message_handler(
             queue_message.message.data.decode(),
             GoogleMetadata(queue_message.ack_id, queue_message.message.publish_time, queue_message.delivery_attempt),
         )
 
     def delete_message(self, queue_message: ReceivedMessage) -> None:
         self.subscriber.acknowledge(subscription=self._subscription_path, ack_ids=[queue_message.ack_id])
@@ -238,14 +243,15 @@
         if settings.TASKHAWK_SYNC:
             return
         if visibility_timeout_s < 0 or visibility_timeout_s > 600:
             raise ValueError("Invalid visibility_timeout_s")
         self.subscriber.modify_ack_deadline(
             subscription=self._subscription_path, ack_ids=[metadata.ack_id], ack_deadline_seconds=visibility_timeout_s
         )
+        self._call_heartbeat_hook()
 
     def requeue_dead_letter(self, num_messages: int = 10, visibility_timeout: Optional[int] = None) -> None:
         """
         Re-queues everything in the Taskhawk DLQ back into the Taskhawk queue.
 
         :param num_messages: Maximum number of messages to fetch in one call. Defaults to 10.
         :param visibility_timeout: The number of seconds the message should remain invisible to other queue readers.
@@ -283,7 +289,13 @@
                     self.delete_message(queue_message)
                 except Exception:
                     logger.exception(
                         'Exception in requeue message from {} to {}'.format(self._subscription_path, topic_path)
                     )
 
             logging.info("Re-queued {} messages".format(len(queue_messages)))
+
+    def _call_heartbeat_hook(self):
+        try:
+            settings.TASKHAWK_HEARTBEAT_HOOK(**self.heartbeat_hook_kwargs())
+        except Exception:
+            logger.exception('Exception in heartbeat hook')
```

### Comparing `taskhawk-4.2.1/taskhawk/backends/import_utils.py` & `taskhawk-4.3.0/taskhawk/backends/import_utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/backends/utils.py` & `taskhawk-4.3.0/taskhawk/backends/utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/commands.py` & `taskhawk-4.3.0/taskhawk/commands.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/conf/__init__.py` & `taskhawk-4.3.0/taskhawk/conf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,29 @@
     'AWS_SESSION_TOKEN': None,
     'GOOGLE_APPLICATION_CREDENTIALS': None,
     'GOOGLE_CLOUD_PROJECT': None,
     'GOOGLE_PUBSUB_READ_TIMEOUT_S': 20,
     'IS_LAMBDA_APP': False,
     'TASKHAWK_CONSUMER_BACKEND': None,
     'TASKHAWK_DEFAULT_HEADERS': 'taskhawk.conf.default_headers_hook',
+    'TASKHAWK_HEARTBEAT_HOOK': 'taskhawk.conf.noop_hook',
     'TASKHAWK_PRE_PROCESS_HOOK': 'taskhawk.conf.noop_hook',
     'TASKHAWK_POST_PROCESS_HOOK': 'taskhawk.conf.noop_hook',
     'TASKHAWK_PUBLISHER_BACKEND': None,
     'TASKHAWK_PUBLISHER_GCP_BATCH_SETTINGS': (),
     'TASKHAWK_QUEUE': None,
     'TASKHAWK_SYNC': False,
     'TASKHAWK_TASK_CLASS': 'taskhawk.task_manager.Task',
 }
 
 
 # List of settings that may be in string import notation.
 _IMPORT_STRINGS = (
     'TASKHAWK_DEFAULT_HEADERS',
+    'TASKHAWK_HEARTBEAT_HOOK',
     'TASKHAWK_PRE_PROCESS_HOOK',
     'TASKHAWK_POST_PROCESS_HOOK',
     'TASKHAWK_TASK_CLASS',
 )
 
 
 def default_headers_hook(task, **kwargs):
```

### Comparing `taskhawk-4.2.1/taskhawk/consumer.py` & `taskhawk-4.3.0/taskhawk/consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/exceptions.py` & `taskhawk-4.3.0/taskhawk/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/models.py` & `taskhawk-4.3.0/taskhawk/models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/publisher.py` & `taskhawk-4.3.0/taskhawk/publisher.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk/task_manager.py` & `taskhawk-4.3.0/taskhawk/task_manager.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/taskhawk.egg-info/PKG-INFO` & `taskhawk-4.3.0/taskhawk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.2.1
+Version: 4.3.0
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.2.1/taskhawk.egg-info/SOURCES.txt` & `taskhawk-4.3.0/taskhawk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/conftest.py` & `taskhawk-4.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/tasks.py` & `taskhawk-4.3.0/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_backends/test_aws.py` & `taskhawk-4.3.0/tests/test_backends/test_aws.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_backends/test_base.py` & `taskhawk-4.3.0/tests/test_backends/test_base.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_backends/test_gcp.py` & `taskhawk-4.3.0/tests/test_backends/test_gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         assert funcy.project(mock_send_email.call_args[1], message.kwargs.keys()) == message.kwargs
         assert mock_send_email.call_args[1]['headers'] == message.headers
         assert mock_send_email.call_args[1]['metadata'] == message.metadata
 
 
 pre_process_hook = mock.MagicMock()
 post_process_hook = mock.MagicMock()
+heartbeat_hook = mock.MagicMock()
 
 
 @pytest.fixture(name='reset_mocks')
 def _reset_mocks():
     yield
     pre_process_hook.reset_mock()
     post_process_hook.reset_mock()
@@ -245,14 +246,17 @@
         gcp_consumer.subscriber.acknowledge.assert_called_once_with(
             subscription=gcp_consumer._subscription_path, ack_ids=[queue_message.ack_id]
         )
         pre_process_hook.assert_called_once_with(google_pubsub_message=queue_message)
         post_process_hook.assert_called_once_with(google_pubsub_message=queue_message)
 
     def test_error_count_increments(self, mock_pubsub_v1, gcp_settings, gcp_consumer):
+        settings.clear_cache()
+        gcp_settings.TASKHAWK_HEARTBEAT_HOOK = 'tests.test_backends.test_gcp.heartbeat_hook'
+        heartbeat_hook.reset_mock()
         assert gcp_consumer.error_count == 0
 
         gcp_consumer.subscriber.pull.side_effect = ServiceUnavailable("Service Unavailable")
 
         gcp_consumer.pull_messages(num_messages=1)
         assert gcp_consumer.error_count == 1
 
@@ -269,16 +273,20 @@
                     max_messages=1,
                     retry=None,
                     timeout=gcp_settings.GOOGLE_PUBSUB_READ_TIMEOUT_S,
                 )
                 for _ in range(3)
             ]
         )
+        heartbeat_hook.assert_has_calls([mock.call(error_count=1), mock.call(error_count=2), mock.call(error_count=3)])
 
     def test_error_count_resets(self, mock_pubsub_v1, gcp_settings, gcp_consumer):
+        settings.clear_cache()
+        gcp_settings.TASKHAWK_HEARTBEAT_HOOK = 'tests.test_backends.test_gcp.heartbeat_hook'
+        heartbeat_hook.reset_mock()
         gcp_consumer.subscriber.pull.side_effect = ServiceUnavailable("Service Unavailable")
 
         gcp_consumer.pull_messages(num_messages=1)
         assert gcp_consumer.error_count == 1
 
         gcp_consumer.pull_messages(num_messages=1)
         assert gcp_consumer.error_count == 2
@@ -295,7 +303,8 @@
                     max_messages=1,
                     retry=None,
                     timeout=gcp_settings.GOOGLE_PUBSUB_READ_TIMEOUT_S,
                 )
                 for _ in range(3)
             ]
         )
+        heartbeat_hook.assert_has_calls([mock.call(error_count=1), mock.call(error_count=2), mock.call(error_count=0)])
```

### Comparing `taskhawk-4.2.1/tests/test_consumer.py` & `taskhawk-4.3.0/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_models.py` & `taskhawk-4.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_settings.py` & `taskhawk-4.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.1/tests/test_task_manager.py` & `taskhawk-4.3.0/tests/test_task_manager.py`

 * *Files identical despite different names*

