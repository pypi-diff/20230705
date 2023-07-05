# Comparing `tmp/repid-1.4.1.tar.gz` & `tmp/repid-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.4.1.tar", last modified: Sat Jul  1 09:57:27 2023, max compression
+gzip compressed data, was "repid-1.4.2.tar", last modified: Wed Jul  5 09:15:24 2023, max compression
```

## Comparing `repid-1.4.1.tar` & `repid-1.4.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1069 2023-07-01 09:57:07.325157 repid-1.4.1/LICENSE
--rw-r--r--   0        0        0     2589 2023-07-01 09:57:07.325157 repid-1.4.1/README.md
--rw-r--r--   0        0        0     4041 2023-07-01 09:57:27.797185 repid-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1138 2023-07-01 09:57:07.329157 repid-1.4.1/repid/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_asyncify.py
--rw-r--r--   0        0        0     5063 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_runner.py
--rw-r--r--   0        0        0      434 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/__init__.py
--rw-r--r--   0        0        0      501 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/args_bucket_in_message_id.py
--rw-r--r--   0        0        0      272 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/dataclass_hacks.py
--rw-r--r--   0        0        0     1268 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/is_installed.py
--rw-r--r--   0        0        0     1012 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/json_encoder.py
--rw-r--r--   0        0        0      135 2023-07-01 09:57:07.329157 repid-1.4.1/repid/_utils/regex_validators.py
--rw-r--r--   0        0        0      504 2023-07-01 09:57:07.329157 repid-1.4.1/repid/actor.py
--rw-r--r--   0        0        0     2499 2023-07-01 09:57:07.329157 repid-1.4.1/repid/config.py
--rw-r--r--   0        0        0     4525 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connection.py
--rw-r--r--   0        0        0      761 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     2766 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      860 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7092 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-07-01 09:57:07.329157 repid-1.4.1/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     7136 2023-07-01 09:57:07.329157 repid-1.4.1/repid/converter.py
--rw-r--r--   0        0        0      355 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/__init__.py
--rw-r--r--   0        0        0     2276 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_buckets.py
--rw-r--r--   0        0        0      820 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_key.py
--rw-r--r--   0        0        0     5510 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/priorities.py
--rw-r--r--   0        0        0     3859 2023-07-01 09:57:07.329157 repid-1.4.1/repid/data/protocols.py
--rw-r--r--   0        0        0     3270 2023-07-01 09:57:07.329157 repid-1.4.1/repid/health_check_server.py
--rw-r--r--   0        0        0     7426 2023-07-01 09:57:07.333157 repid-1.4.1/repid/job.py
--rw-r--r--   0        0        0      546 2023-07-01 09:57:07.333157 repid-1.4.1/repid/logger.py
--rw-r--r--   0        0        0     1887 2023-07-01 09:57:07.333157 repid-1.4.1/repid/main.py
--rw-r--r--   0        0        0      257 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3696 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-07-01 09:57:07.333157 repid-1.4.1/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/repid/py.typed
--rw-r--r--   0        0        0     1065 2023-07-01 09:57:07.333157 repid-1.4.1/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-07-01 09:57:07.333157 repid-1.4.1/repid/retry_policy.py
--rw-r--r--   0        0        0     5022 2023-07-01 09:57:07.333157 repid-1.4.1/repid/router.py
--rw-r--r--   0        0        0      520 2023-07-01 09:57:07.333157 repid-1.4.1/repid/serializer.py
--rw-r--r--   0        0        0      845 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/__init__.py
--rw-r--r--   0        0        0     3184 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6099 2023-07-01 09:57:07.333157 repid-1.4.1/repid/testing/plugin.py
--rw-r--r--   0        0        0     4726 2023-07-01 09:57:07.333157 repid-1.4.1/repid/worker.py
--rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1145 2023-07-01 09:57:07.333157 repid-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-07-01 09:57:07.333157 repid-1.4.1/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_actor.py
--rw-r--r--   0        0        0     4620 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_config.py
--rw-r--r--   0        0        0     2986 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_connection.py
--rw-r--r--   0        0        0     3834 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10230 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_default_data_models.py
--rw-r--r--   0        0        0     2110 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_health_check_server.py
--rw-r--r--   0        0        0     3004 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_job.py
--rw-r--r--   0        0        0     2298 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_json.py
--rw-r--r--   0        0        0     1366 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     7388 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_queue.py
--rw-r--r--   0        0        0     3180 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_router.py
--rw-r--r--   0        0        0      762 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_serializer.py
--rw-r--r--   0        0        0     1893 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     7633 2023-07-01 09:57:07.333157 repid-1.4.1/tests/test_worker.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-05 09:14:59.090660 repid-1.4.2/LICENSE
+-rw-r--r--   0        0        0     2589 2023-07-05 09:14:59.090660 repid-1.4.2/README.md
+-rw-r--r--   0        0        0     4163 2023-07-05 09:15:24.536708 repid-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1138 2023-07-05 09:14:59.094660 repid-1.4.2/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_asyncify.py
+-rw-r--r--   0        0        0     5063 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_runner.py
+-rw-r--r--   0        0        0      434 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0     1268 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0     1012 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      504 2023-07-05 09:14:59.094660 repid-1.4.2/repid/actor.py
+-rw-r--r--   0        0        0     2499 2023-07-05 09:14:59.094660 repid-1.4.2/repid/config.py
+-rw-r--r--   0        0        0     4493 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connection.py
+-rw-r--r--   0        0        0      761 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     2766 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      860 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7092 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     7133 2023-07-05 09:14:59.094660 repid-1.4.2/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_key.py
+-rw-r--r--   0        0        0     5510 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/priorities.py
+-rw-r--r--   0        0        0     3859 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/protocols.py
+-rw-r--r--   0        0        0     3270 2023-07-05 09:14:59.094660 repid-1.4.2/repid/health_check_server.py
+-rw-r--r--   0        0        0     7426 2023-07-05 09:14:59.094660 repid-1.4.2/repid/job.py
+-rw-r--r--   0        0        0      546 2023-07-05 09:14:59.094660 repid-1.4.2/repid/logger.py
+-rw-r--r--   0        0        0     1887 2023-07-05 09:14:59.094660 repid-1.4.2/repid/main.py
+-rw-r--r--   0        0        0      257 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3696 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-07-05 09:14:59.098661 repid-1.4.2/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/repid/py.typed
+-rw-r--r--   0        0        0     1065 2023-07-05 09:14:59.098661 repid-1.4.2/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-07-05 09:14:59.098661 repid-1.4.2/repid/retry_policy.py
+-rw-r--r--   0        0        0     5022 2023-07-05 09:14:59.098661 repid-1.4.2/repid/router.py
+-rw-r--r--   0        0        0      520 2023-07-05 09:14:59.098661 repid-1.4.2/repid/serializer.py
+-rw-r--r--   0        0        0      845 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6099 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/plugin.py
+-rw-r--r--   0        0        0     4726 2023-07-05 09:14:59.098661 repid-1.4.2/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1145 2023-07-05 09:14:59.098661 repid-1.4.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_actor.py
+-rw-r--r--   0        0        0     4620 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10230 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     2110 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_health_check_server.py
+-rw-r--r--   0        0        0     3004 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_job.py
+-rw-r--r--   0        0        0     2298 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_json.py
+-rw-r--r--   0        0        0     1366 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7388 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_router.py
+-rw-r--r--   0        0        0      762 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_serializer.py
+-rw-r--r--   0        0        0     1893 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     7633 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_worker.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.2/PKG-INFO
```

### Comparing `repid-1.4.1/LICENSE` & `repid-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/README.md` & `repid-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/pyproject.toml` & `repid-1.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.4.1"
+version = "1.4.2"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
 
@@ -109,41 +109,41 @@
 [tool.pdm.build]
 includes = [
     "repid",
 ]
 
 [tool.pdm.dev-dependencies]
 docs = [
-    "mkdocs-material",
-    "mike",
-    "mkdocs-glightbox",
+    "mkdocs-material>=9.1.16",
+    "mike>=1.1.2",
+    "mkdocs-glightbox>=0.3.4",
     "setuptools>=65.5.1",
 ]
 format = [
-    "black",
+    "black>=23.3.0",
 ]
 lint = [
-    "mypy",
-    "types-redis",
-    "types-croniter",
-    "ruff",
+    "mypy>=1.4.1",
+    "types-redis>=4.6.0.0",
+    "types-croniter>=1.4.0.0",
+    "ruff>=0.0.275",
 ]
 pre-commit = [
-    "pre-commit",
+    "pre-commit>=3.3.3",
 ]
 tests = [
-    "pytest",
-    "pytest-asyncio",
-    "pytest-pretty",
-    "pytest-clarity",
-    "pytest-lazy-fixture",
-    "pytest-docker-tools",
+    "pytest>=7.3.2",
+    "pytest-asyncio>=0.21.0",
+    "pytest-pretty>=1.2.0",
+    "pytest-clarity>=1.0.1",
+    "pytest-lazy-fixture>=0.6.3",
+    "pytest-docker-tools>=3.1.3",
     "pytest-timeout>=2.1.0",
     "coverage[toml]>=7.2.7",
-    "hypothesis",
+    "hypothesis>=6.79.1",
     "httpx>=0.24.1",
 ]
 
 [tool.pdm.scripts]
 erase-coverage = "coverage erase"
 only-test = "coverage run -m pytest --diff-symbols --hypothesis-verbosity=normal tests/"
 report-coverage = "coverage report --no-skip-covered --show-missing"
```

### Comparing `repid-1.4.1/repid/__init__.py` & `repid-1.4.2/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/_asyncify.py` & `repid-1.4.2/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/_processor.py` & `repid-1.4.2/repid/_processor.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/_runner.py` & `repid-1.4.2/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/_utils/is_installed.py` & `repid-1.4.2/repid/_utils/is_installed.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/_utils/json_encoder.py` & `repid-1.4.2/repid/_utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/config.py` & `repid-1.4.2/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connection.py` & `repid-1.4.2/repid/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,30 @@
                     self.message_broker,
                     self.args_bucket_broker,
                     self.results_bucket_broker,
                 ]
                 if broker is not None
             ],
         )
-        object.__setattr__(self, "is_open", True)  # noqa: FBT003
+        object.__setattr__(self, "is_open", True)
 
     async def disconnect(self) -> None:
         """Disconnect from all set brokers. Marks connection as closed."""
         await asyncio.gather(
             *[
                 broker.disconnect()
                 for broker in [
                     self.message_broker,
                     self.args_bucket_broker,
                     self.results_bucket_broker,
                 ]
                 if broker is not None
             ],
         )
-        object.__setattr__(self, "is_open", False)  # noqa: FBT003
+        object.__setattr__(self, "is_open", False)
 
     @property
     def _ab(self) -> "BucketBrokerT":
         """For internal use.
 
         Shortcut to get args bucket broker or raise an error, if it isn't set.
         """
```

### Comparing `repid-1.4.1/repid/connections/__init__.py` & `repid-1.4.2/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/abc.py` & `repid-1.4.2/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/in_memory/bucket_broker.py` & `repid-1.4.2/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/in_memory/consumer.py` & `repid-1.4.2/repid/connections/in_memory/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/in_memory/message_broker.py` & `repid-1.4.2/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/in_memory/utils.py` & `repid-1.4.2/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/rabbitmq/consumer.py` & `repid-1.4.2/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/rabbitmq/message_broker.py` & `repid-1.4.2/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/rabbitmq/utils.py` & `repid-1.4.2/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/redis/bucket_broker.py` & `repid-1.4.2/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/redis/consumer.py` & `repid-1.4.2/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/redis/message_broker.py` & `repid-1.4.2/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/connections/redis/utils.py` & `repid-1.4.2/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/converter.py` & `repid-1.4.2/repid/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 raise ValueError("*args and **kwargs are unsupported")
 
         self.input_pydantic_model: BaseModel = create_model(  # type: ignore[call-overload]
             f"{fn.__name__}_input_repid_model",
             **{
                 p.name: (
                     p.annotation if p.annotation is not inspect.Parameter.empty else Any,
-                    p.default if p.annotation is not inspect.Parameter.empty else Field(),
+                    p.default if p.default is not inspect.Parameter.empty else Field(),
                 )
                 for p in signature.parameters.values()
             },
         )
 
         self.validate_output = True
         if (
```

### Comparing `repid-1.4.1/repid/data/_buckets.py` & `repid-1.4.2/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/data/_key.py` & `repid-1.4.2/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/data/_parameters.py` & `repid-1.4.2/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/data/protocols.py` & `repid-1.4.2/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/health_check_server.py` & `repid-1.4.2/repid/health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/job.py` & `repid-1.4.2/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/logger.py` & `repid-1.4.2/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/main.py` & `repid-1.4.2/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/middlewares/middleware.py` & `repid-1.4.2/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/middlewares/wrapper.py` & `repid-1.4.2/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/queue.py` & `repid-1.4.2/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/retry_policy.py` & `repid-1.4.2/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/router.py` & `repid-1.4.2/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/serializer.py` & `repid-1.4.2/repid/serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/testing/__init__.py` & `repid-1.4.2/repid/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/testing/modifiers.py` & `repid-1.4.2/repid/testing/modifiers.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/testing/plugin.py` & `repid-1.4.2/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/repid/worker.py` & `repid-1.4.2/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/conftest.py` & `repid-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/integration/conftest.py` & `repid-1.4.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/integration/test_buckets.py` & `repid-1.4.2/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/integration/test_consumer.py` & `repid-1.4.2/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/integration/test_default_flow.py` & `repid-1.4.2/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/integration/test_no_messages_lost.py` & `repid-1.4.2/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_config.py` & `repid-1.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_connection.py` & `repid-1.4.2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_consumer.py` & `repid-1.4.2/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_consumer_abc.py` & `repid-1.4.2/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_default_data_models.py` & `repid-1.4.2/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_health_check_server.py` & `repid-1.4.2/tests/test_health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_hypothesis.py` & `repid-1.4.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_job.py` & `repid-1.4.2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_json.py` & `repid-1.4.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_main.py` & `repid-1.4.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_middleware.py` & `repid-1.4.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_multiprocessing.py` & `repid-1.4.2/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_pydantic.py` & `repid-1.4.2/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_pytest_plugin.py` & `repid-1.4.2/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_router.py` & `repid-1.4.2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_serializer.py` & `repid-1.4.2/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_utils.py` & `repid-1.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/tests/test_worker.py` & `repid-1.4.2/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.1/PKG-INFO` & `repid-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.4.1
+Version: 1.4.2
 Summary: Repid framework: simple to use, fast to run and extensible to adopt job scheduler
 Author-Email: aleksul <me@aleksul.space>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repid Version: 1.4.1 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.4.2 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

