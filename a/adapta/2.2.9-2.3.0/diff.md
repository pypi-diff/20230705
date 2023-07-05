# Comparing `tmp/adapta-2.2.9.tar.gz` & `tmp/adapta-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.2.9.tar", max compression
+gzip compressed data, was "adapta-2.3.0.tar", max compression
```

## Comparing `adapta-2.2.9.tar` & `adapta-2.3.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10693 2023-05-26 07:49:00.485108 adapta-2.2.9/LICENSE
--rw-r--r--   0        0        0      666 2023-05-26 07:49:00.485108 adapta-2.2.9/README.md
--rw-r--r--   0        0        0      663 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-05-26 07:49:16.861319 adapta-2.2.9/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9167 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-05-26 07:49:00.485108 adapta-2.2.9/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     3820 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      732 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/schema_management/README.md
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/schema_management/__init__.py
--rw-r--r--   0        0        0     1219 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/schema_management/schema_entity.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/README.md
--rw-r--r--   0        0        0     1450 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     7396 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3454 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0     1952 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/security/clients/hashicorp_vault/token_client.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0      598 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6630 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/models/local.py
--rw-r--r--   0        0        0     1953 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0     2761 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/utils/README.md
--rw-r--r--   0        0        0      668 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/utils/__init__.py
--rw-r--r--   0        0        0     5161 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/utils/_common.py
--rw-r--r--   0        0        0     3815 2023-05-26 07:49:00.489108 adapta-2.2.9/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2210 2023-05-26 07:49:16.861319 adapta-2.2.9/pyproject.toml
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 adapta-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-07-05 09:27:26.020175 adapta-2.3.0/LICENSE
+-rw-r--r--   0        0        0      666 2023-07-05 09:27:26.020175 adapta-2.3.0/README.md
+-rw-r--r--   0        0        0      663 2023-07-05 09:27:26.020175 adapta-2.3.0/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-05 09:27:46.196101 adapta-2.3.0/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.020175 adapta-2.3.0/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9167 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     3820 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      732 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/README.md
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/__init__.py
+-rw-r--r--   0        0        0     1219 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/schema_management/schema_entity.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/__init__.py
+-rw-r--r--   0        0        0     2140 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/README.md
+-rw-r--r--   0        0        0     1450 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     8358 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0     1952 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/security/clients/hashicorp_vault/token_client.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0      598 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6630 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/models/local.py
+-rw-r--r--   0        0        0     1953 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     2761 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/README.md
+-rw-r--r--   0        0        0      668 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-07-05 09:27:26.024175 adapta-2.3.0/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3930 2023-07-05 09:27:26.028175 adapta-2.3.0/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2211 2023-07-05 09:27:46.196101 adapta-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 adapta-2.3.0/PKG-INFO
```

### Comparing `adapta-2.2.9/LICENSE` & `adapta-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/README.md` & `adapta-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/__init__.py` & `adapta-2.3.0/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/connectors/__init__.py` & `adapta-2.3.0/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/connectors/service_bus/__init__.py` & `adapta-2.3.0/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/connectors/service_bus/_connector.py` & `adapta-2.3.0/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/README.md` & `adapta-2.3.0/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/__init__.py` & `adapta-2.3.0/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/_base.py` & `adapta-2.3.0/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/_internal.py` & `adapta-2.3.0/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/handlers/__init__.py` & `adapta-2.3.0/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.3.0/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.3.0/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/models/__init__.py` & `adapta-2.3.0/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/models/_log_level.py` & `adapta-2.3.0/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/logs/models/_logs_metadata.py` & `adapta-2.3.0/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/metrics/__init__.py` & `adapta-2.3.0/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/metrics/_base.py` & `adapta-2.3.0/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/metrics/providers/README.md` & `adapta-2.3.0/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/metrics/providers/__init__.py` & `adapta-2.3.0/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/metrics/providers/datadog_provider.py` & `adapta-2.3.0/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/ml/__init__.py` & `adapta-2.3.0/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/ml/_model.py` & `adapta-2.3.0/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/ml/mlflow/__init__.py` & `adapta-2.3.0/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/ml/mlflow/_client.py` & `adapta-2.3.0/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/ml/mlflow/_functions.py` & `adapta-2.3.0/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/process_communication/__init__.py` & `adapta-2.3.0/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/process_communication/_models.py` & `adapta-2.3.0/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/schema_management/README.md` & `adapta-2.3.0/adapta/schema_management/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/schema_management/__init__.py` & `adapta-2.3.0/adapta/schema_management/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/schema_management/schema_entity.py` & `adapta-2.3.0/adapta/schema_management/schema_entity.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/__init__.py` & `adapta-2.3.0/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/README.md` & `adapta-2.3.0/adapta/security/clients/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 Currently supported:
 - HashiCorp Vault
 - Azure
 - Local (for unit tests)
 
 ## Azure Client
-There are few important notes on the usage of this client for retrieving storage account credentials via `connect_storage` method. This method is also used by `delta_lake` loaders, thus it is important to understand how to configure your environment and account. 
+There are few important notes on the usage of this client for retrieving storage account credentials via `connect_storage` method. This method is also used by `delta_lake` loaders, thus it is important to understand how to configure your environment and account. The client supports several methods for obtaining credentials, which are listed below in order of preference:
 
-1. Environment Variables: The method first checks for mapped environment variables in a format `f'PROTEUS__{STORAGEACCOUNTNAME}_AZURE_STORAGE_ACCOUNT_KEY'`, and if found, returns the account name and key.
+1. Azure Token: If the `PROTEUS__USE_AZURE_CREDENTIAL` environment variable is set, the method returns a token retrieved from Azure AD with the correct scope, and account name.
 
-Note that this gives your client full write access on the account.
+For the issued tokens to work, this method requires user to have **exactly** `Storage Blob Data Reader` IAM role on the **storage account** or **container**. Please note that even being account owner does not work.
 
 2. Azure Credentials: If environment variables are not found, the method checks for Azure service principal credentials in the environment variables in the form of `AZURE_CLIENT_SECRET` or `PROTEUS__AZURE_CLIENT_SECRET`. If found, it returns the client ID, client secret, tenant ID, and account name.
 
 For the issued tokens to work, this method requires user to have **exactly** `Storage Blob Data Reader` IAM role on the **storage account** or **container**. Please note that even being account owner does not work.
 
-3. Azure Token: If the `PROTEUS__USE_AZURE_CREDENTIAL` environment variable is set, the method returns a token retrieved from Azure AD with the correct scope, and account name.
+3. Environment Variables (Legacy): The method first checks for mapped environment variables in a format `f'PROTEUS__{STORAGEACCOUNTNAME}_AZURE_STORAGE_ACCOUNT_KEY'`, and if found, returns the account name and key.
 
-For the issued tokens to work, this method requires user to have **exactly** `Storage Blob Data Reader` IAM role on the **storage account** or **container**. Please note that even being account owner does not work.
+Note that this gives your client full write access on the account.
 
-4. Auto-Discovery: If none of the above options work, the method auto-discovers the storage account using the ARM API and returns the account name and key. If `set_env` is True, it also sets the environment variables for the account name and key.
+4. Auto-Discovery (Legacy - DO NOT USE): If none of the above options work, the method auto-discovers the storage account using the ARM API and returns the account name and key. If `set_env` is True, it also sets the environment variables for the account name and key.
 
 This method requires user to have `Reader and Data Access` IAM role on the **storage account**.
 
-If none of the above options work, the method raises a ValueError.
+If none of the above options work, the method raises a ValueError.
```

### Comparing `adapta-2.2.9/adapta/security/clients/__init__.py` & `adapta-2.3.0/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/_azure_client.py` & `adapta-2.3.0/adapta/security/clients/_azure_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -152,25 +152,40 @@
         raise ValueError(f"Can't find credentials for an account {adls_path.account}")
 
     def get_credentials(self) -> DefaultAzureCredential:
         return _get_azure_credentials()
 
     def get_pyarrow_filesystem(self, path: DataPath, connection_options: Optional[Dict[str, str]] = None) -> FileSystem:
         def select_file_system(options: Optional[Dict[str, str]], account_name: str) -> AzureBlobFileSystem:
-            if not options:
+            if not options and "PROTEUS__USE_AZURE_CREDENTIAL" in os.environ:
                 return AzureBlobFileSystem(account_name=account_name, anon=False)
 
+            if not options and f"PROTEUS__{account_name.upper()}_AZURE_STORAGE_ACCOUNT_KEY" in os.environ:
+                return AzureBlobFileSystem(
+                    account_name=account_name,
+                    account_key=os.getenv(f"PROTEUS__{account_name.upper()}_AZURE_STORAGE_ACCOUNT_KEY"),
+                )
+
+            if not options and ("AZURE_CLIENT_SECRET" in os.environ or "PROTEUS__AZURE_CLIENT_SECRET" in os.environ):
+                return AzureBlobFileSystem(
+                    account_name=account_name,
+                    client_id=os.getenv("AZURE_CLIENT_ID") or os.getenv("PROTEUS__AZURE_CLIENT_ID"),
+                    client_secret=os.getenv("AZURE_CLIENT_SECRET") or os.getenv("PROTEUS__AZURE_CLIENT_SECRET"),
+                    tenant_id=os.getenv("AZURE_TENANT_ID") or os.getenv("PROTEUS__AZURE_TENANT_ID"),
+                )
+
             if options.get("AZURE_STORAGE_ACCOUNT_KEY", None):
                 return AzureBlobFileSystem(
                     account_name=account_name,
                     account_key=options["AZURE_STORAGE_ACCOUNT_KEY"],
                 )
 
             if options.get("AZURE_CLIENT_SECRET", None):
                 return AzureBlobFileSystem(
+                    account_name=account_name,
                     client_id=options["AZURE_CLIENT_ID"],
                     client_secret=options["AZURE_CLIENT_SECRET"],
                     tenant_id=options["AZURE_TENANT_ID"],
                 )
 
             raise ValueError(f"Unsupported connection options have been provided: {connection_options}")
```

### Comparing `adapta-2.2.9/adapta/security/clients/_base.py` & `adapta-2.3.0/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/_local_client.py` & `adapta-2.3.0/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.3.0/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.3.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.3.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.3.0/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/security/clients/hashicorp_vault/token_client.py` & `adapta-2.3.0/adapta/security/clients/hashicorp_vault/token_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/__init__.py` & `adapta-2.3.0/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/blob/README.md` & `adapta-2.3.0/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/blob/__init__.py` & `adapta-2.3.0/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/blob/azure_storage_client.py` & `adapta-2.3.0/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/blob/base.py` & `adapta-2.3.0/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/cache/__init__.py` & `adapta-2.3.0/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/cache/_base.py` & `adapta-2.3.0/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/cache/redis_cache.py` & `adapta-2.3.0/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/README.md` & `adapta-2.3.0/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/__init__.py` & `adapta-2.3.0/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/azure_sql.py` & `adapta-2.3.0/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/models/__init__.py` & `adapta-2.3.0/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/models/_models.py` & `adapta-2.3.0/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/odbc.py` & `adapta-2.3.0/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/database/trino_sql.py` & `adapta-2.3.0/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/delta_lake/README.md` & `adapta-2.3.0/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/delta_lake/__init__.py` & `adapta-2.3.0/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/delta_lake/_functions.py` & `adapta-2.3.0/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/delta_lake/_models.py` & `adapta-2.3.0/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/__init__.py` & `adapta-2.3.0/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/azure.py` & `adapta-2.3.0/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/base.py` & `adapta-2.3.0/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/format.py` & `adapta-2.3.0/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/hive.py` & `adapta-2.3.0/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/models/local.py` & `adapta-2.3.0/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/secrets/README.md` & `adapta-2.3.0/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/secrets/__init__.py` & `adapta-2.3.0/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/secrets/_base.py` & `adapta-2.3.0/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.3.0/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.3.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/utils/README.md` & `adapta-2.3.0/adapta/utils/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/utils/__init__.py` & `adapta-2.3.0/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.2.9/adapta/utils/_common.py` & `adapta-2.3.0/adapta/utils/_common.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 import math
 import os
 import sys
 
 import time
 from collections import namedtuple
 from functools import partial
-from typing import List, Optional, Dict, Any, Tuple
+from typing import List, Optional, Dict, Any, Tuple, Union
 
+import pandas
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 if sys.platform != "win32":
     import resource
 
@@ -151,7 +152,33 @@
                 )
 
                 yield memory_limit_bytes
             else:
                 raise ValueError("Specify either memory_limit_percentage or memory_limit_bytes")
         finally:
             resource.setrlimit(resource.RLIMIT_AS, (total_mem_bytes, total_mem_bytes))
+
+
+def map_column_names(
+    dataframe: pandas.DataFrame,
+    column_map: Dict[str, str],
+    default_values: Optional[Dict[str, Union[str, int, float]]] = None,
+    drop_missing: bool = True,
+) -> pandas.DataFrame:
+    """
+    Maps a dataframe from one nomenclature to another. Original dataframe is not mutated.
+
+    :param dataframe: Dataframe to be mapped.
+    :param column_map: A dictionary mapping old column names to new.
+    :param default_values: If a column is not present in the dataframe
+    a default value mapping can be given, by mapping a column name it a value.
+    :param drop_missing: A boolean value to control if columns should be
+    dropped if the columns are present in the dataframe but not the column_map.
+    """
+    default_values = default_values or {}
+    # Only columns in the map are mapped
+    kept_columns = list(set(column_map.keys()) & set(dataframe.columns)) if drop_missing else dataframe.columns
+    dataframe = dataframe[kept_columns].rename(columns=column_map, errors="ignore")
+    # Only use default values for columns not present in the dataframe
+    default_values = {k: v for (k, v) in default_values.items() if k not in dataframe.columns}
+    dataframe[list(default_values.keys())] = list(default_values.values())
+    return dataframe
```

### Comparing `adapta-2.2.9/adapta/utils/concurrent_task_runner.py` & `adapta-2.3.0/adapta/utils/concurrent_task_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 #  limitations under the License.
 #
 
 import concurrent
 import os
 import sys
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Callable, Any, List, TypeVar, Generic, Optional, Dict
 
 T = TypeVar("T")
 
 
 @dataclass
 class Executable(Generic[T]):
     """
     A single executable function with arguments, ready to run if invoked.
     """
 
     func: Callable[[...], T]
-    args: List[Any]
     alias: str
+    args: List[Any] = field(default_factory=list)
+    kwargs: Dict[str, Any] = field(default_factory=dict)
 
 
 class ConcurrentTaskRunner(Generic[T]):
     """
      Provides parallel execution capability for a list of given functions.
 
       my_funcs = [Executable(func=my_func1, args=[arg1, .., argN], alias='task1'),..]
@@ -82,15 +83,15 @@
         runner_pool = (
             ProcessPoolExecutor(max_workers=worker_count)
             if self._use_processes
             else ThreadPoolExecutor(max_workers=worker_count)
         )
         with runner_pool:
             return {
-                executable.alias: runner_pool.submit(executable.func, *executable.args)
+                executable.alias: runner_pool.submit(executable.func, *executable.args, **executable.kwargs)
                 for executable in self._func_list
             }
 
     def lazy(self) -> Dict[str, concurrent.futures.Future]:
         """
          Executes the function list without explicitly collecting the results, allowing them to be retrieved by the client
          when needed.
```

### Comparing `adapta-2.2.9/pyproject.toml` & `adapta-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "adapta"
-version = "2.2.9"
+version = "2.3.0"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 requests = "^2.26"
 backoff = "^2.2"
 cryptography = "~36.0"
-pandas = { version = ">=1.5,^2.0.0", extras = ["performance"] }
+pandas = { version = ">=2.0.0,<3.0", extras = ["performance"] }
 pyarrow = ">=7.0"
 dataclasses-json = "~0.5.7"
 
 deltalake = { version = "~0.8.1", optional = true }
 
 azure-identity = { version = "~1.7", optional = true }
 azure-storage-blob = { version = ">12.7.0,<=12.16.0", optional = true }
@@ -28,15 +28,15 @@
 
 datadog = { version = "~0.44.0", optional = true }
 datadog-api-client = { version = "~1.12.0", optional = true }
 
 SQLAlchemy = { version = "~1.4", optional = true }
 pyodbc = { version = "~4.0", optional = true }
 
-mlflow-skinny = { version = "~1.28", optional = true }
+mlflow-skinny = { version = "~2.4.1", optional = true }
 
 redis = { version = "~4.4.0", optional = true, extras = ['hiredis'] }
 
 hvac = { version = "0.11.2", optional = true }
 
 fsspec = { version = "2022.8.2" }
```

### Comparing `adapta-2.2.9/PKG-INFO` & `adapta-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.2.9
+Version: 2.3.0
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
@@ -33,16 +33,16 @@
 Requires-Dist: cryptography (>=36.0,<36.1)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: datadog (>=0.44.0,<0.45.0) ; extra == "datadog"
 Requires-Dist: datadog-api-client (>=1.12.0,<1.13.0) ; extra == "datadog"
 Requires-Dist: deltalake (>=0.8.1,<0.9.0) ; extra == "storage"
 Requires-Dist: fsspec (==2022.8.2)
 Requires-Dist: hvac (==0.11.2) ; extra == "hashicorp"
-Requires-Dist: mlflow-skinny (>=1.28,<1.29) ; extra == "ml"
-Requires-Dist: pandas[performance] (>=2.0.0,<3.0.0)
+Requires-Dist: mlflow-skinny (>=2.4.1,<2.5.0) ; extra == "ml"
+Requires-Dist: pandas[performance] (>=2.0.0,<3.0)
 Requires-Dist: pyarrow (>=7.0)
 Requires-Dist: pyodbc (>=4.0,<4.1) ; extra == "databases"
 Requires-Dist: redis[hiredis] (>=4.4.0,<4.5.0) ; extra == "caching"
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: trino[sqlalchemy] (==0.319.0) ; extra == "trino"
 Project-URL: Repository, https://github.com/SneaksAndData/adapta
 Description-Content-Type: text/markdown
```

