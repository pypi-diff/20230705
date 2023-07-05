# Comparing `tmp/repid-1.4.2.tar.gz` & `tmp/repid-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repid-1.4.2.tar", last modified: Wed Jul  5 09:15:24 2023, max compression
+gzip compressed data, was "repid-1.4.3.tar", last modified: Wed Jul  5 15:31:54 2023, max compression
```

## Comparing `repid-1.4.2.tar` & `repid-1.4.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1069 2023-07-05 09:14:59.090660 repid-1.4.2/LICENSE
--rw-r--r--   0        0        0     2589 2023-07-05 09:14:59.090660 repid-1.4.2/README.md
--rw-r--r--   0        0        0     4163 2023-07-05 09:15:24.536708 repid-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1138 2023-07-05 09:14:59.094660 repid-1.4.2/repid/__init__.py
--rw-r--r--   0        0        0     1552 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_asyncify.py
--rw-r--r--   0        0        0     5063 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_processor.py
--rw-r--r--   0        0        0     4061 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_runner.py
--rw-r--r--   0        0        0      434 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/__init__.py
--rw-r--r--   0        0        0      501 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/args_bucket_in_message_id.py
--rw-r--r--   0        0        0      272 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/dataclass_hacks.py
--rw-r--r--   0        0        0     1268 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/is_installed.py
--rw-r--r--   0        0        0     1012 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/json_encoder.py
--rw-r--r--   0        0        0      135 2023-07-05 09:14:59.094660 repid-1.4.2/repid/_utils/regex_validators.py
--rw-r--r--   0        0        0      504 2023-07-05 09:14:59.094660 repid-1.4.2/repid/actor.py
--rw-r--r--   0        0        0     2499 2023-07-05 09:14:59.094660 repid-1.4.2/repid/config.py
--rw-r--r--   0        0        0     4493 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connection.py
--rw-r--r--   0        0        0      761 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/__init__.py
--rw-r--r--   0        0        0     6594 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/abc.py
--rw-r--r--   0        0        0      314 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/dummy/__init__.py
--rw-r--r--   0        0        0      260 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/__init__.py
--rw-r--r--   0        0        0     1823 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/bucket_broker.py
--rw-r--r--   0        0        0     2766 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/consumer.py
--rw-r--r--   0        0        0     4093 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/message_broker.py
--rw-r--r--   0        0        0      860 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/in_memory/utils.py
--rw-r--r--   0        0        0       90 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/consumer.py
--rw-r--r--   0        0        0     7092 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/message_broker.py
--rw-r--r--   0        0        0      362 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/protocols.py
--rw-r--r--   0        0        0      910 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/rabbitmq/utils.py
--rw-r--r--   0        0        0      158 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/__init__.py
--rw-r--r--   0        0        0     1513 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/bucket_broker.py
--rw-r--r--   0        0        0     7593 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/consumer.py
--rw-r--r--   0        0        0     7609 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/message_broker.py
--rw-r--r--   0        0        0     3818 2023-07-05 09:14:59.094660 repid-1.4.2/repid/connections/redis/utils.py
--rw-r--r--   0        0        0     7133 2023-07-05 09:14:59.094660 repid-1.4.2/repid/converter.py
--rw-r--r--   0        0        0      355 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/__init__.py
--rw-r--r--   0        0        0     2276 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_buckets.py
--rw-r--r--   0        0        0      820 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_key.py
--rw-r--r--   0        0        0     5510 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/_parameters.py
--rw-r--r--   0        0        0       95 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/priorities.py
--rw-r--r--   0        0        0     3859 2023-07-05 09:14:59.094660 repid-1.4.2/repid/data/protocols.py
--rw-r--r--   0        0        0     3270 2023-07-05 09:14:59.094660 repid-1.4.2/repid/health_check_server.py
--rw-r--r--   0        0        0     7426 2023-07-05 09:14:59.094660 repid-1.4.2/repid/job.py
--rw-r--r--   0        0        0      546 2023-07-05 09:14:59.094660 repid-1.4.2/repid/logger.py
--rw-r--r--   0        0        0     1887 2023-07-05 09:14:59.094660 repid-1.4.2/repid/main.py
--rw-r--r--   0        0        0      257 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/__init__.py
--rw-r--r--   0        0        0      347 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/consts.py
--rw-r--r--   0        0        0     3696 2023-07-05 09:14:59.094660 repid-1.4.2/repid/middlewares/middleware.py
--rw-r--r--   0        0        0     3647 2023-07-05 09:14:59.098661 repid-1.4.2/repid/middlewares/wrapper.py
--rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/repid/py.typed
--rw-r--r--   0        0        0     1065 2023-07-05 09:14:59.098661 repid-1.4.2/repid/queue.py
--rw-r--r--   0        0        0     1319 2023-07-05 09:14:59.098661 repid-1.4.2/repid/retry_policy.py
--rw-r--r--   0        0        0     5022 2023-07-05 09:14:59.098661 repid-1.4.2/repid/router.py
--rw-r--r--   0        0        0      520 2023-07-05 09:14:59.098661 repid-1.4.2/repid/serializer.py
--rw-r--r--   0        0        0      845 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/__init__.py
--rw-r--r--   0        0        0     3184 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/modifiers.py
--rw-r--r--   0        0        0     6099 2023-07-05 09:14:59.098661 repid-1.4.2/repid/testing/plugin.py
--rw-r--r--   0        0        0     4726 2023-07-05 09:14:59.098661 repid-1.4.2/repid/worker.py
--rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1145 2023-07-05 09:14:59.098661 repid-1.4.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     3241 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     1337 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_buckets.py
--rw-r--r--   0        0        0     4335 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_consumer.py
--rw-r--r--   0        0        0     4003 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_default_flow.py
--rw-r--r--   0        0        0     1904 2023-07-05 09:14:59.098661 repid-1.4.2/tests/integration/test_no_messages_lost.py
--rw-r--r--   0        0        0      431 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_actor.py
--rw-r--r--   0        0        0     4620 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_config.py
--rw-r--r--   0        0        0     2986 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_connection.py
--rw-r--r--   0        0        0     3834 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_consumer.py
--rw-r--r--   0        0        0     2835 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_consumer_abc.py
--rw-r--r--   0        0        0    10230 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_default_data_models.py
--rw-r--r--   0        0        0     2110 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_health_check_server.py
--rw-r--r--   0        0        0     3004 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_hypothesis.py
--rw-r--r--   0        0        0     3591 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_job.py
--rw-r--r--   0        0        0     2298 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_json.py
--rw-r--r--   0        0        0     1366 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_main.py
--rw-r--r--   0        0        0     7842 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_middleware.py
--rw-r--r--   0        0        0     1097 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_multiprocessing.py
--rw-r--r--   0        0        0     7388 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_pydantic.py
--rw-r--r--   0        0        0     3819 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_pytest_plugin.py
--rw-r--r--   0        0        0      414 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_queue.py
--rw-r--r--   0        0        0     3180 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_router.py
--rw-r--r--   0        0        0      762 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_serializer.py
--rw-r--r--   0        0        0     1893 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_utils.py
--rw-r--r--   0        0        0     7633 2023-07-05 09:14:59.098661 repid-1.4.2/tests/test_worker.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-05 15:31:34.993182 repid-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2589 2023-07-05 15:31:34.993182 repid-1.4.3/README.md
+-rw-r--r--   0        0        0     4163 2023-07-05 15:31:54.241794 repid-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1138 2023-07-05 15:31:35.001182 repid-1.4.3/repid/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_asyncify.py
+-rw-r--r--   0        0        0     5063 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_processor.py
+-rw-r--r--   0        0        0     4061 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_runner.py
+-rw-r--r--   0        0        0      434 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/args_bucket_in_message_id.py
+-rw-r--r--   0        0        0      272 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/dataclass_hacks.py
+-rw-r--r--   0        0        0     1268 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/is_installed.py
+-rw-r--r--   0        0        0     1012 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/json_encoder.py
+-rw-r--r--   0        0        0      135 2023-07-05 15:31:35.001182 repid-1.4.3/repid/_utils/regex_validators.py
+-rw-r--r--   0        0        0      504 2023-07-05 15:31:35.001182 repid-1.4.3/repid/actor.py
+-rw-r--r--   0        0        0     2499 2023-07-05 15:31:35.001182 repid-1.4.3/repid/config.py
+-rw-r--r--   0        0        0     4493 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connection.py
+-rw-r--r--   0        0        0      761 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/__init__.py
+-rw-r--r--   0        0        0     6594 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/abc.py
+-rw-r--r--   0        0        0      314 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/dummy/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/in_memory/__init__.py
+-rw-r--r--   0        0        0     1823 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/in_memory/bucket_broker.py
+-rw-r--r--   0        0        0     2766 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/in_memory/consumer.py
+-rw-r--r--   0        0        0     4093 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/in_memory/message_broker.py
+-rw-r--r--   0        0        0      860 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/in_memory/utils.py
+-rw-r--r--   0        0        0       90 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/rabbitmq/consumer.py
+-rw-r--r--   0        0        0     7092 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/rabbitmq/message_broker.py
+-rw-r--r--   0        0        0      362 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/rabbitmq/protocols.py
+-rw-r--r--   0        0        0      910 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/rabbitmq/utils.py
+-rw-r--r--   0        0        0      158 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/redis/__init__.py
+-rw-r--r--   0        0        0     1513 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/redis/bucket_broker.py
+-rw-r--r--   0        0        0     7593 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/redis/consumer.py
+-rw-r--r--   0        0        0     7609 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/redis/message_broker.py
+-rw-r--r--   0        0        0     3818 2023-07-05 15:31:35.001182 repid-1.4.3/repid/connections/redis/utils.py
+-rw-r--r--   0        0        0     7133 2023-07-05 15:31:35.001182 repid-1.4.3/repid/converter.py
+-rw-r--r--   0        0        0      355 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/__init__.py
+-rw-r--r--   0        0        0     2276 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/_buckets.py
+-rw-r--r--   0        0        0      820 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/_key.py
+-rw-r--r--   0        0        0     5510 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/_parameters.py
+-rw-r--r--   0        0        0       95 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/priorities.py
+-rw-r--r--   0        0        0     3859 2023-07-05 15:31:35.001182 repid-1.4.3/repid/data/protocols.py
+-rw-r--r--   0        0        0     3421 2023-07-05 15:31:35.001182 repid-1.4.3/repid/health_check_server.py
+-rw-r--r--   0        0        0     7426 2023-07-05 15:31:35.001182 repid-1.4.3/repid/job.py
+-rw-r--r--   0        0        0      546 2023-07-05 15:31:35.001182 repid-1.4.3/repid/logger.py
+-rw-r--r--   0        0        0     1887 2023-07-05 15:31:35.001182 repid-1.4.3/repid/main.py
+-rw-r--r--   0        0        0      257 2023-07-05 15:31:35.001182 repid-1.4.3/repid/middlewares/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-05 15:31:35.001182 repid-1.4.3/repid/middlewares/consts.py
+-rw-r--r--   0        0        0     3696 2023-07-05 15:31:35.001182 repid-1.4.3/repid/middlewares/middleware.py
+-rw-r--r--   0        0        0     3647 2023-07-05 15:31:35.001182 repid-1.4.3/repid/middlewares/wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-05 15:31:35.001182 repid-1.4.3/repid/py.typed
+-rw-r--r--   0        0        0     1065 2023-07-05 15:31:35.001182 repid-1.4.3/repid/queue.py
+-rw-r--r--   0        0        0     1319 2023-07-05 15:31:35.001182 repid-1.4.3/repid/retry_policy.py
+-rw-r--r--   0        0        0     5022 2023-07-05 15:31:35.001182 repid-1.4.3/repid/router.py
+-rw-r--r--   0        0        0      520 2023-07-05 15:31:35.001182 repid-1.4.3/repid/serializer.py
+-rw-r--r--   0        0        0      845 2023-07-05 15:31:35.001182 repid-1.4.3/repid/testing/__init__.py
+-rw-r--r--   0        0        0     3184 2023-07-05 15:31:35.001182 repid-1.4.3/repid/testing/modifiers.py
+-rw-r--r--   0        0        0     6099 2023-07-05 15:31:35.001182 repid-1.4.3/repid/testing/plugin.py
+-rw-r--r--   0        0        0     4726 2023-07-05 15:31:35.001182 repid-1.4.3/repid/worker.py
+-rw-r--r--   0        0        0        0 2023-07-05 15:31:35.001182 repid-1.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1145 2023-07-05 15:31:35.001182 repid-1.4.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3241 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1337 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/test_buckets.py
+-rw-r--r--   0        0        0     4335 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/test_consumer.py
+-rw-r--r--   0        0        0     4003 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/test_default_flow.py
+-rw-r--r--   0        0        0     1904 2023-07-05 15:31:35.001182 repid-1.4.3/tests/integration/test_no_messages_lost.py
+-rw-r--r--   0        0        0      431 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_actor.py
+-rw-r--r--   0        0        0     4620 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_config.py
+-rw-r--r--   0        0        0     2986 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_connection.py
+-rw-r--r--   0        0        0     3834 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_consumer.py
+-rw-r--r--   0        0        0     2835 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_consumer_abc.py
+-rw-r--r--   0        0        0    10230 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_default_data_models.py
+-rw-r--r--   0        0        0     2110 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_health_check_server.py
+-rw-r--r--   0        0        0     3004 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_hypothesis.py
+-rw-r--r--   0        0        0     3591 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_job.py
+-rw-r--r--   0        0        0     2298 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_json.py
+-rw-r--r--   0        0        0     1366 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_main.py
+-rw-r--r--   0        0        0     7842 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_middleware.py
+-rw-r--r--   0        0        0     1097 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_multiprocessing.py
+-rw-r--r--   0        0        0     7388 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_pydantic.py
+-rw-r--r--   0        0        0     3819 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      414 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_queue.py
+-rw-r--r--   0        0        0     3180 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_router.py
+-rw-r--r--   0        0        0      762 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_serializer.py
+-rw-r--r--   0        0        0     1893 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_utils.py
+-rw-r--r--   0        0        0     7633 2023-07-05 15:31:35.001182 repid-1.4.3/tests/test_worker.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 repid-1.4.3/PKG-INFO
```

### Comparing `repid-1.4.2/LICENSE` & `repid-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/README.md` & `repid-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/pyproject.toml` & `repid-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "packaging>=22.0",
 ]
 description = "Repid framework: simple to use, fast to run and extensible to adopt job scheduler"
 dynamic = []
 name = "repid"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.4.2"
+version = "1.4.3"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pytest11]
 repid = "repid.testing.plugin"
```

### Comparing `repid-1.4.2/repid/__init__.py` & `repid-1.4.3/repid/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/_asyncify.py` & `repid-1.4.3/repid/_asyncify.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/_processor.py` & `repid-1.4.3/repid/_processor.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/_runner.py` & `repid-1.4.3/repid/_runner.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/_utils/is_installed.py` & `repid-1.4.3/repid/_utils/is_installed.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/_utils/json_encoder.py` & `repid-1.4.3/repid/_utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/config.py` & `repid-1.4.3/repid/config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connection.py` & `repid-1.4.3/repid/connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/__init__.py` & `repid-1.4.3/repid/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/abc.py` & `repid-1.4.3/repid/connections/abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/in_memory/bucket_broker.py` & `repid-1.4.3/repid/connections/in_memory/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/in_memory/consumer.py` & `repid-1.4.3/repid/connections/in_memory/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/in_memory/message_broker.py` & `repid-1.4.3/repid/connections/in_memory/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/in_memory/utils.py` & `repid-1.4.3/repid/connections/in_memory/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/rabbitmq/consumer.py` & `repid-1.4.3/repid/connections/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/rabbitmq/message_broker.py` & `repid-1.4.3/repid/connections/rabbitmq/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/rabbitmq/utils.py` & `repid-1.4.3/repid/connections/rabbitmq/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/redis/bucket_broker.py` & `repid-1.4.3/repid/connections/redis/bucket_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/redis/consumer.py` & `repid-1.4.3/repid/connections/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/redis/message_broker.py` & `repid-1.4.3/repid/connections/redis/message_broker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/connections/redis/utils.py` & `repid-1.4.3/repid/connections/redis/utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/converter.py` & `repid-1.4.3/repid/converter.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/data/_buckets.py` & `repid-1.4.3/repid/data/_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/data/_key.py` & `repid-1.4.3/repid/data/_key.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/data/_parameters.py` & `repid-1.4.3/repid/data/_parameters.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/data/protocols.py` & `repid-1.4.3/repid/data/protocols.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/health_check_server.py` & `repid-1.4.3/repid/health_check_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import asyncio
+import time
 from dataclasses import asdict, dataclass
 from enum import IntEnum
+from wsgiref.handlers import format_date_time
 
 from repid._utils import FROZEN_DATACLASS, SLOTS_DATACLASS
 from repid.logger import logger
 
 
 @dataclass(**FROZEN_DATACLASS, **SLOTS_DATACLASS)
 class HealthCheckServerSettings:
@@ -79,13 +81,18 @@
         response = self.handle_request(method, path)
 
         self.transport.write(response.encode())
         self.transport.close()
 
     def handle_request(self, method: str, path: str) -> str:
         if method == "GET" and path == self.endpoint_name:
-            return (
-                f"HTTP/1.1 {self.status.value} {self.status.name}\r\n"
-                f"Content-Type: text/plain\r\n\r\n"
-                f"{self.status.value} {self.status.name}"
-            )
-        return "HTTP/1.1 404 Not Found\r\nContent-Type: text/plain\r\n\r\n404 Not Found"
+            content = f"{self.status.value} {self.status.name}"
+        else:
+            content = "404 Not Found"
+        return (
+            f"HTTP/1.1 {content}\r\n"
+            f"Date: {format_date_time(time.time())}\r\n"
+            f"Content-Type: text/plain\r\n"
+            f"Content-Length: {len(content)}\r\n"
+            f"Connection: close\r\n\r\n"
+            f"{content}"
+        )
```

### Comparing `repid-1.4.2/repid/job.py` & `repid-1.4.3/repid/job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/logger.py` & `repid-1.4.3/repid/logger.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/main.py` & `repid-1.4.3/repid/main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/middlewares/middleware.py` & `repid-1.4.3/repid/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/middlewares/wrapper.py` & `repid-1.4.3/repid/middlewares/wrapper.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/queue.py` & `repid-1.4.3/repid/queue.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/retry_policy.py` & `repid-1.4.3/repid/retry_policy.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/router.py` & `repid-1.4.3/repid/router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/serializer.py` & `repid-1.4.3/repid/serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/testing/__init__.py` & `repid-1.4.3/repid/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/testing/modifiers.py` & `repid-1.4.3/repid/testing/modifiers.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/testing/plugin.py` & `repid-1.4.3/repid/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/repid/worker.py` & `repid-1.4.3/repid/worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/conftest.py` & `repid-1.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/integration/conftest.py` & `repid-1.4.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/integration/test_buckets.py` & `repid-1.4.3/tests/integration/test_buckets.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/integration/test_consumer.py` & `repid-1.4.3/tests/integration/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/integration/test_default_flow.py` & `repid-1.4.3/tests/integration/test_default_flow.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/integration/test_no_messages_lost.py` & `repid-1.4.3/tests/integration/test_no_messages_lost.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_config.py` & `repid-1.4.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_connection.py` & `repid-1.4.3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_consumer.py` & `repid-1.4.3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_consumer_abc.py` & `repid-1.4.3/tests/test_consumer_abc.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_default_data_models.py` & `repid-1.4.3/tests/test_default_data_models.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_health_check_server.py` & `repid-1.4.3/tests/test_health_check_server.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_hypothesis.py` & `repid-1.4.3/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_job.py` & `repid-1.4.3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_json.py` & `repid-1.4.3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_main.py` & `repid-1.4.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_middleware.py` & `repid-1.4.3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_multiprocessing.py` & `repid-1.4.3/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_pydantic.py` & `repid-1.4.3/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_pytest_plugin.py` & `repid-1.4.3/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_router.py` & `repid-1.4.3/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_serializer.py` & `repid-1.4.3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_utils.py` & `repid-1.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/tests/test_worker.py` & `repid-1.4.3/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `repid-1.4.2/PKG-INFO` & `repid-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repid
-Version: 1.4.2
+Version: 1.4.3
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
-Metadata-Version: 2.1 Name: repid Version: 1.4.2 Summary: Repid framework:
+Metadata-Version: 2.1 Name: repid Version: 1.4.3 Summary: Repid framework:
 simple to use, fast to run and extensible to adopt job scheduler Author-Email:
 aleksul
 aleksul.space> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

