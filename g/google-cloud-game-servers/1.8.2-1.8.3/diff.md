# Comparing `tmp/google-cloud-game-servers-1.8.2.tar.gz` & `tmp/google-cloud-game-servers-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-game-servers-1.8.2.tar", last modified: Wed Apr  5 20:23:50 2023, max compression
+gzip compressed data, was "google-cloud-game-servers-1.8.3.tar", last modified: Wed Jul  5 15:47:59 2023, max compression
```

## Comparing `google-cloud-game-servers-1.8.2.tar` & `google-cloud-game-servers-1.8.3.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.136471 google-cloud-game-servers-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4557 2023-04-05 20:23:50.140472 google-cloud-game-servers-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3626 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.108467 google-cloud-game-servers-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.108467 google-cloud-game-servers-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.112467 google-cloud-game-servers-1.8.2/google/cloud/gaming/
--rw-rw-r--   0 root         (0)     1003     6016 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.112467 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/
--rw-rw-r--   0 root         (0)     1003     5441 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13495 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.112467 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.112467 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/
--rw-rw-r--   0 root         (0)     1003      813 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    48347 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57513 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/client.py
--rw-rw-r--   0 root         (0)     1003     6203 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.116468 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/
--rw-rw-r--   0 root         (0)     1003     1575 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11990 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22216 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22658 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    56107 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.116468 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    30530 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    39586 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/client.py
--rw-rw-r--   0 root         (0)     1003     6158 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.116468 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8583 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16767 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17111 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    31282 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.116468 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/
--rw-rw-r--   0 root         (0)     1003      825 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    55073 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    65065 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/client.py
--rw-rw-r--   0 root         (0)     1003     6419 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.120469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/
--rw-rw-r--   0 root         (0)     1003     1617 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12624 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24417 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24863 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    62938 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.120469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    37750 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    46562 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/client.py
--rw-rw-r--   0 root         (0)     1003     5584 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.120469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9370 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17770 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18129 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39537 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.120469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/
--rw-rw-r--   0 root         (0)     1003     4495 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16336 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    22970 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_clusters.py
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_clusters_service.py
--rw-rw-r--   0 root         (0)     1003     9588 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_configs.py
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_configs_service.py
--rw-rw-r--   0 root         (0)     1003    17474 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_deployments.py
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_deployments_service.py
--rw-rw-r--   0 root         (0)     1003     9403 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/realms.py
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/realms_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.124469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/
--rw-rw-r--   0 root         (0)     1003     5331 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    13503 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.124469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.124469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/
--rw-rw-r--   0 root         (0)     1003      813 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    48514 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57680 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/client.py
--rw-rw-r--   0 root         (0)     1003     6239 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.124469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/
--rw-rw-r--   0 root         (0)     1003     1575 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11998 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22252 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    22694 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    56163 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.124469 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    30562 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    39618 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/client.py
--rw-rw-r--   0 root         (0)     1003     6194 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.128470 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8591 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16787 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17131 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    31322 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.128470 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/
--rw-rw-r--   0 root         (0)     1003      825 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    55280 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    65272 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/client.py
--rw-rw-r--   0 root         (0)     1003     6455 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.128470 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/
--rw-rw-r--   0 root         (0)     1003     1617 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12632 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    24457 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    24903 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    62998 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.128470 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    37888 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    46700 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/client.py
--rw-rw-r--   0 root         (0)     1003     5620 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9378 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17798 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18157 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    39585 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     4381 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16395 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/common.py
--rw-rw-r--   0 root         (0)     1003    15754 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_clusters.py
--rw-rw-r--   0 root         (0)     1003      769 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_clusters_service.py
--rw-rw-r--   0 root         (0)     1003     9578 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_configs.py
--rw-rw-r--   0 root         (0)     1003      769 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_configs_service.py
--rw-rw-r--   0 root         (0)     1003    17533 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_deployments.py
--rw-rw-r--   0 root         (0)     1003      769 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_deployments_service.py
--rw-rw-r--   0 root         (0)     1003     9407 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/realms.py
--rw-rw-r--   0 root         (0)     1003      769 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/realms_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/
--rw-r--r--   0 root         (0)     1003     4557 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     8185 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-05 20:23:50.000000 google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-05 20:23:50.140472 google-cloud-game-servers-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2935 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.132471 google-cloud-game-servers-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.136471 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   223834 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_clusters_service.py
--rw-rw-r--   0 root         (0)     1003   148745 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_configs_service.py
--rw-rw-r--   0 root         (0)     1003   249597 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_deployments_service.py
--rw-rw-r--   0 root         (0)     1003   169232 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_realms_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-05 20:23:50.136471 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   220197 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_clusters_service.py
--rw-rw-r--   0 root         (0)     1003   148785 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_configs_service.py
--rw-rw-r--   0 root         (0)     1003   249649 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_deployments_service.py
--rw-rw-r--   0 root         (0)     1003   169276 2023-04-05 20:21:17.000000 google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_realms_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.301104 google-cloud-game-servers-1.8.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4557 2023-07-05 15:47:59.301104 google-cloud-game-servers-1.8.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3626 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.269106 google-cloud-game-servers-1.8.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.269106 google-cloud-game-servers-1.8.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.273106 google-cloud-game-servers-1.8.3/google/cloud/gaming/
+-rw-rw-r--   0 root         (0)     1003     6016 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.273106 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/
+-rw-rw-r--   0 root         (0)     1003     5441 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13495 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.273106 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.273106 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/
+-rw-rw-r--   0 root         (0)     1003      813 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48389 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57513 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6203 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.277105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1575 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11990 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22216 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22658 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    56107 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.277105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30571 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39586 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6158 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.277105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8583 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16767 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17111 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    31282 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.277105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/
+-rw-rw-r--   0 root         (0)     1003      825 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55118 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    65065 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6419 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.281105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1617 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12624 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24417 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24863 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    62938 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.281105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37780 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46562 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5584 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.281105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9370 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17770 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18129 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39537 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.285105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4495 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16336 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    22970 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_clusters.py
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_clusters_service.py
+-rw-rw-r--   0 root         (0)     1003     9588 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_configs.py
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_configs_service.py
+-rw-rw-r--   0 root         (0)     1003    17474 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_deployments.py
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_deployments_service.py
+-rw-rw-r--   0 root         (0)     1003     9403 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/realms.py
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/realms_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.285105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/
+-rw-rw-r--   0 root         (0)     1003     5331 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13503 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.285105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.285105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/
+-rw-rw-r--   0 root         (0)     1003      813 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    48556 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57680 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6239 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.285105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1575 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11998 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22252 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    22694 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    56163 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.289105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30603 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39618 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6194 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.289105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8591 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16787 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17131 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    31322 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.289105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/
+-rw-rw-r--   0 root         (0)     1003      825 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55325 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    65272 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6455 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.289105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1617 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12632 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    24457 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24903 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    62998 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.293105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    37918 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46700 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5620 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.293105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9378 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17798 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18157 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    39585 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.293105 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     4381 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16395 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/common.py
+-rw-rw-r--   0 root         (0)     1003    15754 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_clusters.py
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_clusters_service.py
+-rw-rw-r--   0 root         (0)     1003     9578 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_configs.py
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_configs_service.py
+-rw-rw-r--   0 root         (0)     1003    17533 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_deployments.py
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_deployments_service.py
+-rw-rw-r--   0 root         (0)     1003     9407 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/realms.py
+-rw-rw-r--   0 root         (0)     1003      769 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/realms_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.297104 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/
+-rw-r--r--   0 root         (0)     1003     4557 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     8185 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:47:59.000000 google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:47:59.301104 google-cloud-game-servers-1.8.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2935 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.297104 google-cloud-game-servers-1.8.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.297104 google-cloud-game-servers-1.8.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.297104 google-cloud-game-servers-1.8.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.297104 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   224033 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_clusters_service.py
+-rw-rw-r--   0 root         (0)     1003   148944 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_configs_service.py
+-rw-rw-r--   0 root         (0)     1003   249796 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_deployments_service.py
+-rw-rw-r--   0 root         (0)     1003   169431 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_realms_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:47:59.301104 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   220396 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_clusters_service.py
+-rw-rw-r--   0 root         (0)     1003   148984 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_configs_service.py
+-rw-rw-r--   0 root         (0)     1003   249848 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_deployments_service.py
+-rw-rw-r--   0 root         (0)     1003   169475 2023-07-05 15:45:06.000000 google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_realms_service.py
```

### Comparing `google-cloud-game-servers-1.8.2/LICENSE` & `google-cloud-game-servers-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/MANIFEST.in` & `google-cloud-game-servers-1.8.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/PKG-INFO` & `google-cloud-game-servers-1.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-game-servers
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Game Servers API client library
 Home-page: https://github.com/googleapis/python-game-servers
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-game-servers-1.8.2/README.rst` & `google-cloud-game-servers-1.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming/gapic_version.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming/gapic_version.py`

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
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/gapic_metadata.json` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/gapic_version.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/gapic_version.py`

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
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerClustersServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_clusters_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_clusters_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,15 +730,15 @@
             empty_pb2.Empty,
             metadata_type=common.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerConfigsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_configs_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_configs_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1320,15 +1320,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerDeploymentsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/game_server_deployments_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/game_server_deployments_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -946,15 +946,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RealmsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/services/realms_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/services/realms_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/common.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_clusters.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_clusters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_clusters_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_clusters_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_configs.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_configs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_configs_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_configs_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_deployments.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_deployments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/game_server_deployments_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/game_server_deployments_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/realms.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/realms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1/types/realms_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1/types/realms_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/gapic_metadata.json` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/gapic_version.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/gapic_version.py`

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
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.8.3"  # {x-release-please-version}
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1166,15 +1166,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerClustersServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_clusters_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
             empty_pb2.Empty,
             metadata_type=common.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerConfigsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_configs_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,15 +1327,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "GameServerDeploymentsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/game_server_deployments_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/async_client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,15 +948,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "RealmsServiceAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/client.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/pagers.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/base.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/grpc.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/grpc_asyncio.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/services/realms_service/transports/rest.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/services/realms_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/__init__.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/common.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_clusters.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_clusters.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_clusters_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_clusters_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_configs.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_configs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_configs_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_configs_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_deployments.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_deployments.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/game_server_deployments_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/game_server_deployments_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/realms.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/realms.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google/cloud/gaming_v1beta/types/realms_service.py` & `google-cloud-game-servers-1.8.3/google/cloud/gaming_v1beta/types/realms_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/PKG-INFO` & `google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-game-servers
-Version: 1.8.2
+Version: 1.8.3
 Summary: Google Cloud Game Servers API client library
 Home-page: https://github.com/googleapis/python-game-servers
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-game-servers-1.8.2/google_cloud_game_servers.egg-info/SOURCES.txt` & `google-cloud-game-servers-1.8.3/google_cloud_game_servers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/setup.py` & `google-cloud-game-servers-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/__init__.py` & `google-cloud-game-servers-1.8.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/__init__.py` & `google-cloud-game-servers-1.8.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/__init__.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/__init__.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_clusters_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_clusters_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,17 +1209,19 @@
                     game_server_clusters.GameServerCluster(),
                     game_server_clusters.GameServerCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_configs_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_configs_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,17 +1205,19 @@
                     game_server_configs.GameServerConfig(),
                     game_server_configs.GameServerConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_game_server_deployments_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_deployments_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.gaming_v1.services.game_server_deployments_service import (
+from google.cloud.gaming_v1beta.services.game_server_deployments_service import (
     GameServerDeploymentsServiceAsyncClient,
     GameServerDeploymentsServiceClient,
     pagers,
     transports,
 )
-from google.cloud.gaming_v1.types import common, game_server_deployments
+from google.cloud.gaming_v1beta.types import common, game_server_deployments
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -680,15 +680,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_game_server_deployments_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceGrpcTransport.__init__"
+        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = GameServerDeploymentsServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -1210,17 +1210,19 @@
                     game_server_deployments.GameServerDeployment(),
                     game_server_deployments.GameServerDeployment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_deployments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3383,15 +3385,15 @@
         client.list_game_server_deployments(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*}/gameServerDeployments"
+            "%s/v1beta/{parent=projects/*/locations/*}/gameServerDeployments"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_game_server_deployments_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -3728,15 +3730,15 @@
         client.get_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4040,15 +4042,15 @@
         client.create_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*}/gameServerDeployments"
+            "%s/v1beta/{parent=projects/*/locations/*}/gameServerDeployments"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4317,15 +4319,15 @@
         client.delete_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4622,15 +4624,15 @@
         client.update_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{game_server_deployment.name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1beta/{game_server_deployment.name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4916,15 +4918,15 @@
         client.get_game_server_deployment_rollout(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}/rollout"
+            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}/rollout"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_game_server_deployment_rollout_rest_flattened_error(
     transport: str = "rest",
@@ -5239,15 +5241,15 @@
         client.update_game_server_deployment_rollout(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{rollout.name=projects/*/locations/*/gameServerDeployments/*}/rollout"
+            "%s/v1beta/{rollout.name=projects/*/locations/*/gameServerDeployments/*}/rollout"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_game_server_deployment_rollout_rest_flattened_error(
     transport: str = "rest",
@@ -5912,15 +5914,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_game_server_deployments_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport.__init__"
+        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.GameServerDeploymentsServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -5958,15 +5960,15 @@
 
 
 def test_game_server_deployments_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
+        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.GameServerDeploymentsServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -5977,15 +5979,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_game_server_deployments_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
+        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.GameServerDeploymentsServiceTransport()
         adc.assert_called_once()
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1/test_realms_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_realms_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1127,17 +1127,19 @@
                     realms.Realm(),
                     realms.Realm(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_realms(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/__init__.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_clusters_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_clusters_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,17 +1209,19 @@
                     game_server_clusters.GameServerCluster(),
                     game_server_clusters.GameServerCluster(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_clusters(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_configs_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_game_server_configs_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1205,17 +1205,19 @@
                     game_server_configs.GameServerConfig(),
                     game_server_configs.GameServerConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_configs(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_game_server_deployments_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1/test_game_server_deployments_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.gaming_v1beta.services.game_server_deployments_service import (
+from google.cloud.gaming_v1.services.game_server_deployments_service import (
     GameServerDeploymentsServiceAsyncClient,
     GameServerDeploymentsServiceClient,
     pagers,
     transports,
 )
-from google.cloud.gaming_v1beta.types import common, game_server_deployments
+from google.cloud.gaming_v1.types import common, game_server_deployments
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -680,15 +680,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_game_server_deployments_service_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceGrpcTransport.__init__"
+        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = GameServerDeploymentsServiceClient(
             client_options={"api_endpoint": "squid.clam.whelk"}
         )
         grpc_transport.assert_called_once_with(
             credentials=None,
@@ -1210,17 +1210,19 @@
                     game_server_deployments.GameServerDeployment(),
                     game_server_deployments.GameServerDeployment(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_game_server_deployments(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
@@ -3383,15 +3385,15 @@
         client.list_game_server_deployments(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*}/gameServerDeployments"
+            "%s/v1/{parent=projects/*/locations/*}/gameServerDeployments"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_game_server_deployments_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -3728,15 +3730,15 @@
         client.get_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4040,15 +4042,15 @@
         client.create_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*}/gameServerDeployments"
+            "%s/v1/{parent=projects/*/locations/*}/gameServerDeployments"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4317,15 +4319,15 @@
         client.delete_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4622,15 +4624,15 @@
         client.update_game_server_deployment(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{game_server_deployment.name=projects/*/locations/*/gameServerDeployments/*}"
+            "%s/v1/{game_server_deployment.name=projects/*/locations/*/gameServerDeployments/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_game_server_deployment_rest_flattened_error(transport: str = "rest"):
     client = GameServerDeploymentsServiceClient(
@@ -4916,15 +4918,15 @@
         client.get_game_server_deployment_rollout(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/gameServerDeployments/*}/rollout"
+            "%s/v1/{name=projects/*/locations/*/gameServerDeployments/*}/rollout"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_game_server_deployment_rollout_rest_flattened_error(
     transport: str = "rest",
@@ -5239,15 +5241,15 @@
         client.update_game_server_deployment_rollout(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{rollout.name=projects/*/locations/*/gameServerDeployments/*}/rollout"
+            "%s/v1/{rollout.name=projects/*/locations/*/gameServerDeployments/*}/rollout"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_game_server_deployment_rollout_rest_flattened_error(
     transport: str = "rest",
@@ -5912,15 +5914,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_game_server_deployments_service_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport.__init__"
+        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.GameServerDeploymentsServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -5958,15 +5960,15 @@
 
 
 def test_game_server_deployments_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
+        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.GameServerDeploymentsServiceTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -5977,15 +5979,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_game_server_deployments_service_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.gaming_v1beta.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
+        "google.cloud.gaming_v1.services.game_server_deployments_service.transports.GameServerDeploymentsServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.GameServerDeploymentsServiceTransport()
         adc.assert_called_once()
```

### Comparing `google-cloud-game-servers-1.8.2/tests/unit/gapic/gaming_v1beta/test_realms_service.py` & `google-cloud-game-servers-1.8.3/tests/unit/gapic/gaming_v1beta/test_realms_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1127,17 +1127,19 @@
                     realms.Realm(),
                     realms.Realm(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
             await client.list_realms(request={})
-        ).pages:  # pragma: no branch
+        ).pages:
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
```

