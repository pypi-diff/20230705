# Comparing `tmp/dff-0.4.1.tar.gz` & `tmp/dff-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dff-0.4.1.tar", last modified: Mon Apr 24 14:28:32 2023, max compression
+gzip compressed data, was "dff-0.4.2.tar", last modified: Wed Jul  5 15:21:05 2023, max compression
```

## Comparing `dff-0.4.1.tar` & `dff-0.4.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-24 14:28:18.000000 dff-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-04-24 14:28:18.000000 dff-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 14:28:18.000000 dff-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-24 14:28:32.730352 dff-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-24 14:28:18.000000 dff-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 14:28:18.000000 dff-0.4.1/dff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/context_storages/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/protocols.json
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/shelve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/ydb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/messengers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/messengers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/messengers/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/service/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/script/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/script/conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/conditions/std_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/core/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/conditions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/slots/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/slots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/labels/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/labels/std_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/responses/std_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/cleanup_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/response_comparers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/toy_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/turn_caching/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/turn_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/turn_caching/singleton_turn_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:28:32.730352 dff-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-24 14:28:18.000000 dff-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-05 15:20:58.000000 dff-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-07-05 15:20:58.000000 dff-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-05 15:20:58.000000 dff-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-05 15:21:05.215838 dff-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-05 15:20:58.000000 dff-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.207835 dff-0.4.2/dff/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 15:20:58.000000 dff-0.4.2/dff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/context_storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/protocols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/shelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-05 15:20:58.000000 dff-0.4.2/dff/context_storages/ydb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/messengers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/messengers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/common/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/messengers/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/telegram/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/telegram/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/telegram/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-05 15:20:58.000000 dff-0.4.2/dff/messengers/telegram/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/pipeline/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/pipeline/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/pipeline/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/pipeline/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/service/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/service/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-05 15:20:58.000000 dff-0.4.2/dff/pipeline/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.211837 dff-0.4.2/dff/script/conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/conditions/std_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/extras/conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/extras/conditions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/extras/slots/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/extras/slots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/labels/std_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/script/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-05 15:20:58.000000 dff-0.4.2/dff/script/responses/std_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/utils/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/cleanup_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/response_comparers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/testing/toy_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/utils/turn_caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/turn_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/turn_caching/singleton_turn_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.215838 dff-0.4.2/dff/utils/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 15:20:58.000000 dff-0.4.2/dff/utils/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:21:05.207835 dff-0.4.2/dff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-05 15:21:05.000000 dff-0.4.2/dff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-05 15:21:05.000000 dff-0.4.2/dff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:21:05.000000 dff-0.4.2/dff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-05 15:21:05.000000 dff-0.4.2/dff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 15:21:05.000000 dff-0.4.2/dff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:21:05.215838 dff-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-05 15:20:58.000000 dff-0.4.2/setup.py
```

### Comparing `dff-0.4.1/CONTRIBUTING.md` & `dff-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/LICENSE` & `dff-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/PKG-INFO` & `dff-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dff
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Dialog Flow Framework (DFF) allows you to write conversational services.
 Home-page: https://github.com/deeppavlov/dialog_flow_framework
 Author: Denis Kuznetsov
 Author-email: kuznetsov.den.p@gmail.com
 Keywords: chatbots
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dff-0.4.1/README.md` & `dff-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/__init__.py` & `dff-0.4.2/dff/context_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/database.py` & `dff-0.4.2/dff/context_storages/database.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/json.py` & `dff-0.4.2/dff/context_storages/json.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/mongo.py` & `dff-0.4.2/dff/context_storages/mongo.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/pickle.py` & `dff-0.4.2/dff/context_storages/pickle.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/protocol.py` & `dff-0.4.2/dff/context_storages/protocol.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/protocols.json` & `dff-0.4.2/dff/context_storages/protocols.json`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/redis.py` & `dff-0.4.2/dff/context_storages/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Additionally, Redis can be used as a cache, message broker, and database, making it a versatile
 and powerful choice for data storage and management.
 """
 import json
 from typing import Hashable
 
 try:
-    from aioredis import Redis
+    from redis.asyncio import Redis
 
     redis_available = True
 except ImportError:
     redis_available = False
 
 from dff.script import Context
```

### Comparing `dff-0.4.1/dff/context_storages/shelve.py` & `dff-0.4.2/dff/context_storages/shelve.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/sql.py` & `dff-0.4.2/dff/context_storages/sql.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/context_storages/ydb.py` & `dff-0.4.2/dff/context_storages/ydb.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                     $queryContext
                 );
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            await (session.transaction(ydb.SerializableReadWrite())).execute(
+            await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 {"$queryId": str(key), "$queryContext": value.json()},
                 commit_tx=True,
             )
 
         return await self.pool.retry_operation(callee)
 
@@ -91,15 +91,15 @@
                 FROM {}
                 WHERE id = $queryId;
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            result_sets = await (session.transaction(ydb.SerializableReadWrite())).execute(
+            result_sets = await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 {
                     "$queryId": str(key),
                 },
                 commit_tx=True,
             )
             if result_sets[0].rows:
@@ -120,15 +120,15 @@
                     id = $queryId
                 ;
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            await (session.transaction(ydb.SerializableReadWrite())).execute(
+            await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 {"$queryId": str(key)},
                 commit_tx=True,
             )
 
         return await self.pool.retry_operation(callee)
 
@@ -146,15 +146,15 @@
                 FROM {}
                 WHERE id = $queryId;
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            result_sets = await (session.transaction(ydb.SerializableReadWrite())).execute(
+            result_sets = await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 {
                     "$queryId": str(key),
                 },
                 commit_tx=True,
             )
             return len(result_sets[0].rows) > 0
@@ -169,15 +169,15 @@
                     COUNT(*) as cnt
                 FROM {}
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            result_sets = await (session.transaction(ydb.SerializableReadWrite())).execute(
+            result_sets = await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 commit_tx=True,
             )
             return result_sets[0].rows[0].cnt
 
         return await self.pool.retry_operation(callee)
 
@@ -190,15 +190,15 @@
                 FROM {}
                 ;
                 """.format(
                 self.database, self.table_name
             )
             prepared_query = await session.prepare(query)
 
-            await (session.transaction(ydb.SerializableReadWrite())).execute(
+            await session.transaction(ydb.SerializableReadWrite()).execute(
                 prepared_query,
                 {},
                 commit_tx=True,
             )
 
         return await self.pool.retry_operation(callee)
```

### Comparing `dff-0.4.1/dff/messengers/common/interface.py` & `dff-0.4.2/dff/messengers/common/interface.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/messengers/common/types.py` & `dff-0.4.2/dff/messengers/common/types.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/messengers/telegram/interface.py` & `dff-0.4.2/dff/messengers/telegram/interface.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/messengers/telegram/message.py` & `dff-0.4.2/dff/messengers/telegram/message.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/messengers/telegram/messenger.py` & `dff-0.4.2/dff/messengers/telegram/messenger.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/messengers/telegram/utils.py` & `dff-0.4.2/dff/messengers/telegram/utils.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/pipeline/__init__.py` & `dff-0.4.2/dff/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/pipeline/conditions.py` & `dff-0.4.2/dff/pipeline/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,30 @@
     Condition that allows service execution, only if the other service was executed successfully.
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
     :param path: The path of the condition pipeline component.
     """
 
     def check_service_state(ctx: Context, _: Pipeline):
-        state = ctx.framework_states[PIPELINE_STATE_KEY].get(path, ComponentExecutionState.NOT_RUN.name)
+        state = ctx.framework_states[PIPELINE_STATE_KEY].get(path, ComponentExecutionState.NOT_RUN)
         return ComponentExecutionState[state] == ComponentExecutionState.FINISHED
 
     return check_service_state
 
 
-def not_condition(function: StartConditionCheckerFunction) -> StartConditionCheckerFunction:
+def not_condition(func: StartConditionCheckerFunction) -> StartConditionCheckerFunction:
     """
     Condition that returns opposite boolean value to the one returned by incoming function.
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
-    :param function: The function to return opposite of.
+    :param func: The function to return opposite of.
     """
 
     def not_function(ctx: Context, pipeline: Pipeline):
-        return not function(ctx, pipeline)
+        return not func(ctx, pipeline)
 
     return not_function
 
 
 def aggregate_condition(
     aggregator: StartConditionCheckerAggregationFunction, *functions: StartConditionCheckerFunction
 ) -> StartConditionCheckerFunction:
@@ -66,15 +66,15 @@
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
     :param aggregator: The function that accepts list of booleans and returns a single boolean.
     :param functions: Functions to aggregate.
     """
 
     def aggregation_function(ctx: Context, pipeline: Pipeline):
-        return aggregator([function(ctx, pipeline) for function in functions])
+        return aggregator([func(ctx, pipeline) for func in functions])
 
     return aggregation_function
 
 
 def all_condition(*functions: StartConditionCheckerFunction) -> StartConditionCheckerFunction:
     """
     Condition that returns `True` only if all incoming functions return `True`.
```

### Comparing `dff-0.4.1/dff/pipeline/pipeline/actor.py` & `dff-0.4.2/dff/pipeline/pipeline/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 
         # NB! The following API is highly experimental and may be removed at ANY time WITHOUT FURTHER NOTICE!!
         self._clean_turn_cache = True
 
     def __call__(
         self, pipeline: Pipeline, ctx: Optional[Union[Context, dict, str]] = None, *args, **kwargs
     ) -> Union[Context, dict, str]:
-
         # context init
         ctx = self._context_init(ctx, *args, **kwargs)
         self._run_handlers(ctx, pipeline, ActorStage.CONTEXT_INIT, *args, **kwargs)
 
         # get previous node
         ctx = self._get_previous_node(ctx, *args, **kwargs)
         self._run_handlers(ctx, pipeline, ActorStage.GET_PREVIOUS_NODE, *args, **kwargs)
@@ -285,15 +284,15 @@
         transition_info: str = "",
         *args,
         **kwargs,
     ) -> Optional[NodeLabel3Type]:
         true_labels = []
         for label, condition in transitions.items():
             if self.condition_handler(condition, ctx, pipeline, *args, **kwargs):
-                if isinstance(label, Callable):
+                if callable(label):
                     label = label(ctx, pipeline, *args, **kwargs)
                     # TODO: explicit handling of errors
                     if label is None:
                         continue
                 label = normalize_label(label, flow_label)
                 true_labels += [label]
         true_labels = [
@@ -303,16 +302,16 @@
             for label in true_labels
         ]
         true_labels.sort(key=lambda label: -label[2])
         true_label = true_labels[0] if true_labels else None
         logger.debug(f"{transition_info} transitions sorted by priority = {true_labels}")
         return true_label
 
-    def _run_handlers(self, ctx, pipeline: Pipeline, actor_stade: ActorStage, *args, **kwargs):
-        [handler(ctx, pipeline, *args, **kwargs) for handler in self.handlers.get(actor_stade, [])]
+    def _run_handlers(self, ctx, pipeline: Pipeline, actor_stage: ActorStage, *args, **kwargs):
+        [handler(ctx, pipeline, *args, **kwargs) for handler in self.handlers.get(actor_stage, [])]
 
     def _choose_label(
         self, specific_label: Optional[NodeLabel3Type], general_label: Optional[NodeLabel3Type]
     ) -> NodeLabel3Type:
         if all([specific_label, general_label]):
             chosen_label = specific_label if specific_label[2] >= general_label[2] else general_label
         elif any([specific_label, general_label]):
@@ -336,15 +335,15 @@
 
         error_msgs = []
         for flow_label, node_label, label, condition in zip(flow_labels, node_labels, labels, conditions):
             ctx = Context()
             ctx.validation = True
             ctx.add_request(Message(text="text"))
 
-            label = label(ctx, pipeline) if isinstance(label, Callable) else normalize_label(label, flow_label)
+            label = label(ctx, pipeline) if callable(label) else normalize_label(label, flow_label)
 
             # validate labeling
             try:
                 node = self.script[label[0]][label[1]]
             except Exception as exc:
                 msg = (
                     f"Could not find node with label={label}, "
```

### Comparing `dff-0.4.1/dff/pipeline/pipeline/component.py` & `dff-0.4.2/dff/pipeline/pipeline/component.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,29 +66,38 @@
         timeout: Optional[float] = None,
         requested_async_flag: Optional[bool] = None,
         calculated_async_flag: bool = False,
         start_condition: Optional[StartConditionCheckerFunction] = None,
         name: Optional[str] = None,
         path: Optional[str] = None,
     ):
-        #: Maximum component execution time (in seconds),
-        #: if it exceeds this time, it is interrupted (for asynchronous only!).
         self.timeout = timeout
-        #: Requested asynchronous property; if not defined, :py:attr:`~requested_async_flag` is used instead.
+        """
+        Maximum component execution time (in seconds),
+        if it exceeds this time, it is interrupted (for asynchronous only!).
+        """
         self.requested_async_flag = requested_async_flag
-        #: Calculated asynchronous property, whether the component can be asynchronous or not.
+        """Requested asynchronous property; if not defined, :py:attr:`~requested_async_flag` is used instead."""
         self.calculated_async_flag = calculated_async_flag
-        #: Component start condition that is invoked before each component execution;
-        #: component is executed only if it returns `True`.
+        """Calculated asynchronous property, whether the component can be asynchronous or not."""
         self.start_condition = always_start_condition if start_condition is None else start_condition
-        #: Component name (should be unique in single :py:class:`~pipeline.service.group.ServiceGroup`),
-        #: should not be blank or contain '.' symbol.
+        """
+        Component start condition that is invoked before each component execution;
+        component is executed only if it returns `True`.
+        """
         self.name = name
-        #: Вot-separated path to component (should be is universally unique).
+        """
+        Component name (should be unique in single :py:class:`~pipeline.service.group.ServiceGroup`),
+        should not be blank or contain '.' symbol.
+        """
         self.path = path
+        """
+        Dot-separated path to component (is universally unique).
+        This attribute is set in :py:func:`~dff.pipeline.pipeline.utils.finalize_service_group`.
+        """
 
         self.before_handler = BeforeHandler([] if before_handler is None else before_handler)
         self.after_handler = AfterHandler([] if after_handler is None else after_handler)
 
         if name is not None and (name == "" or "." in name):
             raise Exception(f"User defined service name shouldn't be blank or contain '.' (service: {name})!")
 
@@ -102,29 +111,27 @@
 
         :param ctx: :py:class:`~.Context` to keep state in.
         :param value: State to set.
         :return: `None`
         """
         if PIPELINE_STATE_KEY not in ctx.framework_states:
             ctx.framework_states[PIPELINE_STATE_KEY] = {}
-        ctx.framework_states[PIPELINE_STATE_KEY][self.path] = value.name
+        ctx.framework_states[PIPELINE_STATE_KEY][self.path] = value
 
     def get_state(self, ctx: Context, default: Optional[ComponentExecutionState] = None) -> ComponentExecutionState:
         """
         Method for component runtime state getting, state is preserved in `ctx.framework_states` dict,
         in subdict, dedicated to this library.
 
         :param ctx: :py:class:`~.Context` to get state from.
         :param default: Default to return if no record found
             (usually it's :py:attr:`~.pipeline.types.ComponentExecutionState.NOT_RUN`).
         :return: :py:class:`~pipeline.types.ComponentExecutionState` of this service or default if not found.
         """
-        return ComponentExecutionState[
-            ctx.framework_states[PIPELINE_STATE_KEY].get(self.path, default if default is not None else None)
-        ]
+        return ctx.framework_states[PIPELINE_STATE_KEY].get(self.path, default if default is not None else None)
 
     @property
     def asynchronous(self) -> bool:
         """
         Property, that indicates, whether this component is synchronous or asynchronous.
         It is calculated according to the following rules:
 
@@ -149,15 +156,15 @@
         if extra_handler is None:
             return
         try:
             extra_handler_result = await extra_handler(ctx, pipeline, self._get_runtime_info(ctx))
             if extra_handler.asynchronous and isinstance(extra_handler_result, Awaitable):
                 await extra_handler_result
         except asyncio.TimeoutError:
-            logger.warning(f"{type(self).__name__} '{self.name}' {extra_handler.stage.name} extra handler timed out!")
+            logger.warning(f"{type(self).__name__} '{self.name}' {extra_handler.stage} extra handler timed out!")
 
     @abc.abstractmethod
     async def _run(self, ctx: Context, pipeline: Optional[Pipeline] = None) -> Optional[Context]:
         """
         A method for running pipeline component, it is overridden in all its children.
         This method is run after the component's timeout is set (if needed).
 
@@ -200,23 +207,23 @@
 
     def _get_runtime_info(self, ctx: Context) -> ServiceRuntimeInfo:
         """
         Method for retrieving runtime info about this component.
 
         :param ctx: Current dialog :py:class:`~.Context`.
         :return: :py:class:`~.dff.script.typing.ServiceRuntimeInfo`
-            dict where all not set fields are replaced with `[None]`.
+            object where all not set fields are replaced with `[None]`.
         """
-        return {
-            "name": self.name if self.name is not None else "[None]",
-            "path": self.path if self.path is not None else "[None]",
-            "timeout": self.timeout,
-            "asynchronous": self.asynchronous,
-            "execution_state": copy.deepcopy(ctx.framework_states[PIPELINE_STATE_KEY]),
-        }
+        return ServiceRuntimeInfo(
+            name=self.name if self.name is not None else "[None]",
+            path=self.path if self.path is not None else "[None]",
+            timeout=self.timeout,
+            asynchronous=self.asynchronous,
+            execution_state=copy.deepcopy(ctx.framework_states[PIPELINE_STATE_KEY]),
+        )
 
     @property
     def info_dict(self) -> dict:
         """
         Property for retrieving info dictionary about this component.
         All not set fields there are replaced with `[None]`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dff-0.4.1/dff/pipeline/pipeline/pipeline.py` & `dff-0.4.2/dff/pipeline/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/pipeline/pipeline/utils.py` & `dff-0.4.2/dff/pipeline/pipeline/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Utils
 -----
 The Utils module contains several service functions that are commonly used throughout the framework.
 These functions provide a variety of utility functionality.
 """
 import collections
-from typing import Union, List, Callable
+from typing import Union, List
 from inspect import isfunction
 
 from ..service.service import Service
 from ..service.group import ServiceGroup
 
 
 def pretty_format_component_info_dict(
@@ -73,15 +73,15 @@
 
     :param service: Service to be renamed.
     :param collisions: Services in the same service group as service.
     :return: Generated name
     """
     if isinstance(service, Service) and isinstance(service.handler, str) and service.handler == "ACTOR":
         base_name = "actor"
-    elif isinstance(service, Service) and isinstance(service.handler, Callable):
+    elif isinstance(service, Service) and callable(service.handler):
         if isfunction(service.handler):
             base_name = service.handler.__name__
         else:
             base_name = service.handler.__class__.__name__
     elif isinstance(service, ServiceGroup):
         base_name = "service_group"
     else:
@@ -97,14 +97,17 @@
     """
     Function that iterates through a service group (and all its subgroups),
     finalizing component's names and paths in it.
     Components are renamed only if user didn't set a name for them. Their paths are also generated here.
     It also searches for "ACTOR" in the group, throwing exception if no actor or multiple actors found.
 
     :param service_group: Service group to resolve name collisions in.
+    :param path:
+        A prefix for component paths -- path of `component` is equal to `{path}.{component.name}`.
+        Defaults to ".".
     """
     actor = False
     names_counter = collections.Counter([component.name for component in service_group.components])
     for component in service_group.components:
         if component.name is None:
             component.name = rename_component_incrementing(component, service_group.components)
         elif names_counter[component.name] > 1:
```

### Comparing `dff-0.4.1/dff/pipeline/service/extra.py` & `dff-0.4.2/dff/pipeline/service/extra.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 import logging
 import inspect
 from typing import Optional, List, ForwardRef
 
 from dff.script import Context
 
 from .utils import collect_defined_constructor_parameters_to_dict, _get_attrs_with_updates, wrap_sync_function_in_async
-from ..types import ServiceRuntimeInfo, ExtraHandlerType, ExtraHandlerBuilder, ExtraHandlerFunction
+from ..types import (
+    ServiceRuntimeInfo,
+    ExtraHandlerType,
+    ExtraHandlerBuilder,
+    ExtraHandlerFunction,
+    ExtraHandlerRuntimeInfo,
+)
 
 logger = logging.getLogger(__name__)
 
 Pipeline = ForwardRef("Pipeline")
 
 
 class _ComponentExtraHandler:
@@ -59,15 +65,15 @@
         elif isinstance(functions, dict):
             functions.update(overridden_parameters)
             self.__init__(**functions)
         elif isinstance(functions, List):
             self.functions = functions
             self.timeout = timeout
             self.requested_async_flag = asynchronous
-            self.calculated_async_flag = all([asyncio.iscoroutinefunction(function) for function in self.functions])
+            self.calculated_async_flag = all([asyncio.iscoroutinefunction(func) for func in self.functions])
             self.stage = stage
         else:
             raise Exception(f"Unknown type for {type(self).__name__} {functions}")
 
     @property
     def asynchronous(self) -> bool:
         """
@@ -83,36 +89,28 @@
         - | If component **can't** be asynchronous and :py:attr:`~requested_async_flag` is `True`,
             an Exception is thrown in constructor.
 
         """
         return self.calculated_async_flag if self.requested_async_flag is None else self.requested_async_flag
 
     async def _run_function(
-        self, function: ExtraHandlerFunction, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo
+        self, func: ExtraHandlerFunction, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo
     ):
-        handler_params = len(inspect.signature(function).parameters)
+        handler_params = len(inspect.signature(func).parameters)
         if handler_params == 1:
-            await wrap_sync_function_in_async(function, ctx)
+            await wrap_sync_function_in_async(func, ctx)
         elif handler_params == 2:
-            await wrap_sync_function_in_async(function, ctx, pipeline)
+            await wrap_sync_function_in_async(func, ctx, pipeline)
         elif handler_params == 3:
-            await wrap_sync_function_in_async(
-                function,
-                ctx,
-                pipeline,
-                {
-                    "function": function,
-                    "stage": self.stage,
-                    "component": component_info,
-                },
-            )
+            extra_handler_runtime_info = ExtraHandlerRuntimeInfo(func=func, stage=self.stage, component=component_info)
+            await wrap_sync_function_in_async(func, ctx, pipeline, extra_handler_runtime_info)
         else:
             raise Exception(
-                f"Too many parameters required for component {component_info['name']} {self.stage.name}"
-                f" wrapper handler '{function.__name__}': {handler_params}!"
+                f"Too many parameters required for component {component_info.name} {self.stage}"
+                f" wrapper handler '{func.__name__}': {handler_params}!"
             )
 
     async def _run(self, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo):
         """
         Method for executing one of the wrapper functions (before or after).
         If the function is not set, nothing happens.
 
@@ -120,26 +118,24 @@
         :param ctx: current dialog context.
         :param pipeline: the current pipeline.
         :param component_info: associated component's info dictionary.
         :return: `None`
         """
 
         if self.asynchronous:
-            futures = [self._run_function(function, ctx, pipeline, component_info) for function in self.functions]
-            for function, future in zip(self.functions, asyncio.as_completed(futures)):
+            futures = [self._run_function(func, ctx, pipeline, component_info) for func in self.functions]
+            for func, future in zip(self.functions, asyncio.as_completed(futures)):
                 try:
                     await future
                 except asyncio.TimeoutError:
-                    logger.warning(
-                        f"Component {component_info['name']} {self.stage.name} wrapper '{function.__name__}' timed out!"
-                    )
+                    logger.warning(f"Component {component_info.name} {self.stage} wrapper '{func.__name__}' timed out!")
 
         else:
-            for function in self.functions:
-                await self._run_function(function, ctx, pipeline, component_info)
+            for func in self.functions:
+                await self._run_function(func, ctx, pipeline, component_info)
 
     async def __call__(self, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo):
         """
         A method for calling pipeline components.
         It sets up timeout if this component is asynchronous and executes it using `_run` method.
 
         :param ctx: (required) Current dialog `Context`.
@@ -161,15 +157,15 @@
         :return: Info dict, containing its fields as well as its type.
             All not set fields there are replaced with `None`.
         """
         return {
             "type": type(self).__name__,
             "timeout": self.timeout,
             "asynchronous": self.asynchronous,
-            "functions": [function.__name__ for function in self.functions],
+            "functions": [func.__name__ for func in self.functions],
         }
 
 
 class BeforeHandler(_ComponentExtraHandler):
     """
     A handler for extra functions that are executed before the component's main function.
```

### Comparing `dff-0.4.1/dff/pipeline/service/group.py` & `dff-0.4.2/dff/pipeline/service/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,14 @@
         Services are created from services and dictionaries.
         ServiceGroups are created from service groups and lists.
 
         :param services: ServiceGroupBuilder object (a `ServiceGroup` instance or a list).
         :type services: :py:data:`~.ServiceGroupBuilder`
         :return: List of services and service groups.
         """
-        handled_services = []
+        handled_services: List[Union[Service, "ServiceGroup"]] = []
         for service in services:
             if isinstance(service, List) or isinstance(service, ServiceGroup):
                 handled_services.append(ServiceGroup(service))
             else:
                 handled_services.append(Service(service))
         return handled_services
```

### Comparing `dff-0.4.1/dff/pipeline/service/service.py` & `dff-0.4.2/dff/pipeline/service/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Actor wrapping service can be synchronous only.
 """
 # TODO: change last sentence, when actor will be asynchronous
 
 import logging
 import asyncio
 import inspect
-from typing import Optional, Callable, ForwardRef
+from typing import Optional, ForwardRef
 
 from dff.script import Context
 
 from .utils import wrap_sync_function_in_async, collect_defined_constructor_parameters_to_dict, _get_attrs_with_updates
 from ..types import (
     ServiceBuilder,
     StartConditionCheckerFunction,
@@ -81,15 +81,15 @@
                         "calculated_async_flag",
                         "path",
                     ),
                     {"requested_async_flag": "asynchronous"},
                     overridden_parameters,
                 )
             )
-        elif isinstance(handler, Callable) or isinstance(handler, str) and handler == "ACTOR":
+        elif callable(handler) or isinstance(handler, str) and handler == "ACTOR":
             self.handler = handler
             super(Service, self).__init__(
                 before_handler,
                 after_handler,
                 timeout,
                 asynchronous,
                 asyncio.iscoroutinefunction(handler),
@@ -176,25 +176,26 @@
         else:
             await self._run_as_service(ctx, pipeline)
 
         await self.run_extra_handler(ExtraHandlerType.AFTER, ctx, pipeline)
 
         if isinstance(self.handler, str) and self.handler == "ACTOR":
             return ctx
+        return None
 
     @property
     def info_dict(self) -> dict:
         """
         See `Component.info_dict` property.
         Adds `handler` key to base info dictionary.
         """
         representation = super(Service, self).info_dict
         if isinstance(self.handler, str) and self.handler == "ACTOR":
             service_representation = "Instance of Actor"
-        elif isinstance(self.handler, Callable):
+        elif callable(self.handler):
             service_representation = f"Callable '{self.handler.__name__}'"
         else:
             service_representation = "[Unknown]"
         representation.update({"handler": service_representation})
         return representation
```

### Comparing `dff-0.4.1/dff/pipeline/service/utils.py` & `dff-0.4.2/dff/pipeline/service/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 The Utility Functions module contains several utility functions that are commonly used throughout the DFF.
 These functions provide a variety of utility functionality.
 """
 import asyncio
 from typing import Callable, Any, Optional, Tuple, Mapping
 
 
-async def wrap_sync_function_in_async(function: Callable, *args, **kwargs) -> Any:
+async def wrap_sync_function_in_async(func: Callable, *args, **kwargs) -> Any:
     """
     Utility function, that wraps both functions and coroutines in coroutines.
-    Invokes `function` if it is just a callable and awaits, if this is a coroutine.
+    Invokes `func` if it is just a callable and awaits, if this is a coroutine.
 
-    :param function: Callable to wrap.
+    :param func: Callable to wrap.
     :param \\*args: Function args.
     :param \\**kwargs: Function kwargs.
     :return: What function returns.
     """
-    if asyncio.iscoroutinefunction(function):
-        return await function(*args, **kwargs)
+    if asyncio.iscoroutinefunction(func):
+        return await func(*args, **kwargs)
     else:
-        return function(*args, **kwargs)
+        return func(*args, **kwargs)
 
 
 def _get_attrs_with_updates(
     obj: object,
     drop_attrs: Optional[Tuple[str, ...]] = None,
     replace_attrs: Optional[Mapping[str, str]] = None,
     add_attrs: Optional[Mapping[str, Any]] = None,
```

### Comparing `dff-0.4.1/dff/pipeline/types.py` & `dff-0.4.2/dff/pipeline/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,83 +2,85 @@
 Types
 -----
 The Types module contains several classes and special types that are used throughout the `DFF Pipeline`.
 The classes and special types in this module can include data models,
 data structures, and other types that are defined for type hinting.
 """
 from abc import ABC
-from enum import unique, Enum, auto
-from typing import Callable, Union, Awaitable, Dict, List, Optional, NewType, Iterable
+from enum import unique, Enum
+from typing import Callable, Union, Awaitable, Dict, List, Optional, NewType, Iterable, Any
 
 from dff.context_storages import DBContextStorage
 from dff.script import Context, ActorStage, NodeLabel2Type, Script
 from typing_extensions import NotRequired, TypedDict, TypeAlias
+from pydantic import BaseModel
 
 
-_ForwardPipeline = NewType("Pipeline", None)
-_ForwardPipelineComponent = NewType("PipelineComponent", None)
+_ForwardPipeline = NewType("Pipeline", Any)
+_ForwardPipelineComponent = NewType("PipelineComponent", Any)
 _ForwardService = NewType("Service", _ForwardPipelineComponent)
-_ForwardServiceBuilder = NewType("ServiceBuilder", None)
+_ForwardServiceBuilder = NewType("ServiceBuilder", Any)
 _ForwardServiceGroup = NewType("ServiceGroup", _ForwardPipelineComponent)
-_ForwardComponentExtraHandler = NewType("_ComponentExtraHandler", None)
+_ForwardComponentExtraHandler = NewType("_ComponentExtraHandler", Any)
 _ForwardProvider = NewType("ABCProvider", ABC)
-_ForwardExtraHandlerFunction = NewType("ExtraHandlerFunction", None)
+_ForwardExtraHandlerRuntimeInfo = NewType("ExtraHandlerRuntimeInfo", Any)
 
 
 @unique
-class ComponentExecutionState(Enum):
+class ComponentExecutionState(str, Enum):
     """
     Enum, representing pipeline component execution state.
     These states are stored in `ctx.framework_keys[PIPELINE_STATE_KEY]`,
     that should always be requested with `NOT_RUN` being default fallback.
     Following states are supported:
 
     - NOT_RUN: component has not been executed yet (the default one),
     - RUNNING: component is currently being executed,
     - FINISHED: component executed successfully,
     - FAILED: component execution failed.
     """
 
-    NOT_RUN = auto()
-    RUNNING = auto()
-    FINISHED = auto()
-    FAILED = auto()
+    NOT_RUN = "NOT_RUN"
+    RUNNING = "RUNNING"
+    FINISHED = "FINISHED"
+    FAILED = "FAILED"
 
 
 @unique
-class GlobalExtraHandlerType(Enum):
+class GlobalExtraHandlerType(str, Enum):
     """
     Enum, representing types of global wrappers, that can be set applied for a pipeline.
     The following types are supported:
 
     - BEFORE_ALL: function called before each pipeline call,
     - BEFORE: function called before each component,
     - AFTER: function called after each component,
     - AFTER_ALL: function called after each pipeline call.
     """
 
-    BEFORE_ALL = auto()
-    BEFORE = auto()
-    AFTER = auto()
-    AFTER_ALL = auto()
+    BEFORE_ALL = "BEFORE_ALL"
+    BEFORE = "BEFORE"
+    AFTER = "AFTER"
+    AFTER_ALL = "AFTER_ALL"
 
 
 @unique
-class ExtraHandlerType(Enum):
+class ExtraHandlerType(str, Enum):
     """
-    Enum, representing wrapper type, pre- or postprocessing.
+    Enum, representing wrapper execution stage: before or after the wrapped function.
     The following types are supported:
 
-    - PREPROCESSING: wrapper function called before component,
-    - POSTPROCESSING: wrapper function called after component.
+    - UNDEFINED: wrapper function with undetermined execution stage,
+    - BEFORE: wrapper function called before component,
+    - AFTER: wrapper function called after component.
     """
 
-    UNDEFINED = auto()
-    BEFORE = auto()
-    AFTER = auto()
+    UNDEFINED = "UNDEFINED"
+    BEFORE = "BEFORE"
+    AFTER = "AFTER"
 
 
 PIPELINE_STATE_KEY = "PIPELINE"
 """
 PIPELINE: storage for services and groups execution status.
 Should be used in `ctx.framework_keys[PIPELINE_STATE_KEY]`.
 """
@@ -103,69 +105,65 @@
 A function type used during global wrappers initialization to determine
 whether wrapper should be applied to component with given path or not.
 Checks components path to be in whitelist (if defined) and not to be in blacklist (if defined).
 Accepts str (component path), returns boolean (whether wrapper should be applied).
 """
 
 
-ServiceRuntimeInfo: TypeAlias = TypedDict(
-    "ServiceRuntimeInfo",
-    {
-        "name": str,
-        "path": str,
-        "timeout": Optional[float],
-        "asynchronous": bool,
-        "execution_state": Dict[str, ComponentExecutionState],
-    },
-)
+class ServiceRuntimeInfo(BaseModel):
+    name: str
+    path: str
+    timeout: Optional[float]
+    asynchronous: bool
+    execution_state: Dict[str, ComponentExecutionState]
+
+
 """
-Type of dictionary, that is passed to components in runtime.
+Type of object, that is passed to components in runtime.
 Contains current component info (`name`, `path`, `timeout`, `asynchronous`).
 Also contains `execution_state` - a dictionary,
-containing other pipeline components execution stats mapped to their paths.
+containing execution states of other components mapped to their paths.
 """
 
 
-ExtraHandlerRuntimeInfo: TypeAlias = TypedDict(
-    "ExtraHandlerRuntimeInfo",
-    {
-        "function": _ForwardExtraHandlerFunction,
-        "stage": ExtraHandlerType,
-        "component": ServiceRuntimeInfo,
-    },
-)
+ExtraHandlerFunction: TypeAlias = Union[
+    Callable[[Context], Any],
+    Callable[[Context, _ForwardPipeline], Any],
+    Callable[[Context, _ForwardPipeline, _ForwardExtraHandlerRuntimeInfo], Any],
+]
 """
-Type of dictionary, that is passed to wrappers in runtime.
-Contains current wrapper info (`name`, `stage`).
-Also contains `component` - runtime info dictionary of the component this wrapper is attached to.
+A function type for creating wrappers (before and after functions).
+Can accept current dialog context, pipeline, and current wrapper info.
 """
 
 
-ExtraHandlerFunction: TypeAlias = Union[
-    Callable[[Context], None],
-    Callable[[Context, _ForwardPipeline], None],
-    Callable[[Context, _ForwardPipeline, ExtraHandlerRuntimeInfo], None],
-]
+class ExtraHandlerRuntimeInfo(BaseModel):
+    func: ExtraHandlerFunction
+    stage: ExtraHandlerType
+    component: ServiceRuntimeInfo
+
+
 """
-A function type for creating wrappers (before and after functions).
-Can accept current dialog context, pipeline, and current wrapper info dictionary.
+Type of object, that is passed to wrappers in runtime.
+Contains current wrapper info (`name`, `stage`).
+Also contains `component` - runtime info of the component this wrapper is attached to.
 """
 
 
 ServiceFunction: TypeAlias = Union[
     Callable[[Context], None],
     Callable[[Context], Awaitable[None]],
     Callable[[Context, _ForwardPipeline], None],
     Callable[[Context, _ForwardPipeline], Awaitable[None]],
     Callable[[Context, _ForwardPipeline, ServiceRuntimeInfo], None],
     Callable[[Context, _ForwardPipeline, ServiceRuntimeInfo], Awaitable[None]],
 ]
 """
 A function type for creating service handlers.
-Can accept current dialog context, pipeline, and current service info dictionary.
+Can accept current dialog context, pipeline, and current service info.
 Can be both synchronous and asynchronous.
 """
 
 
 ExtraHandlerBuilder: TypeAlias = Union[
     _ForwardComponentExtraHandler,
     TypedDict(
```

### Comparing `dff-0.4.1/dff/script/__init__.py` & `dff-0.4.2/dff/script/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 )
 from .core.normalization import (
     normalize_label,
     normalize_condition,
     normalize_transitions,
     normalize_response,
     normalize_processing,
-    normalize_keywords,
     normalize_script,
 )
 from .core.script import Node, Script
 from .core.types import (
     LabelType,
     NodeLabel1Type,
     NodeLabel2Type,
```

### Comparing `dff-0.4.1/dff/script/conditions/std_conditions.py` & `dff-0.4.2/dff/script/conditions/std_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 def check_cond_seq(cond_seq: list):
     """
     Check if the list consists only of Callables.
 
     :param cond_seq: List of conditions to check.
     """
     for cond in cond_seq:
-        if not isinstance(cond, Callable):
+        if not callable(cond):
             raise TypeError(f"{cond_seq} has to consist of callable objects")
 
 
 _any = any
 """
 _any is an alias for any.
 """
```

### Comparing `dff-0.4.1/dff/script/core/context.py` & `dff-0.4.2/dff/script/core/context.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/script/core/keywords.py` & `dff-0.4.2/dff/script/core/keywords.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Keywords
 --------
 Keywords are used to define the dialog graph, which is the structure of a conversation.
 They are used to determine all nodes in the script and to assign python objects and python functions for nodes.
 
 """
-from enum import Enum, auto
+from enum import Enum
 
 
-class Keywords(Enum):
+class Keywords(str, Enum):
     """
     Keywords used to define the dialog script (:py:class:`~dff.script.Script`).
     The data type `dict` is used to describe the scenario.
     `Enums` of this class are used as keys in this `dict`.
     Different keys correspond to the different value types aimed at different purposes.
 
     Enums:
@@ -76,21 +76,22 @@
 
         where `"PRE_TRANSITIONS_PROC_i"` is an arbitrary name of the preprocessing stage in the pipeline.
         The order of `pre_transitions_proc_func_i` calls is defined by the order
         in which the preprocessing `dict` is defined.
 
     """
 
-    GLOBAL = auto()
-    LOCAL = auto()
-    TRANSITIONS = auto()
-    RESPONSE = auto()
-    MISC = auto()
-    PRE_RESPONSE_PROCESSING = auto()
-    PRE_TRANSITIONS_PROCESSING = auto()
+    GLOBAL = "global"
+    LOCAL = "local"
+    TRANSITIONS = "transitions"
+    RESPONSE = "response"
+    MISC = "misc"
+    PRE_RESPONSE_PROCESSING = "pre_response_processing"
+    PRE_TRANSITIONS_PROCESSING = "pre_transitions_processing"
+    PROCESSING = "pre_transitions_processing"
 
 
 # Redefine shortcuts
 GLOBAL = Keywords.GLOBAL
 LOCAL = Keywords.LOCAL
 TRANSITIONS = Keywords.TRANSITIONS
 RESPONSE = Keywords.RESPONSE
```

### Comparing `dff-0.4.1/dff/script/core/message.py` & `dff-0.4.2/dff/script/core/message.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/script/core/normalization.py` & `dff-0.4.2/dff/script/core/normalization.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,48 +5,49 @@
 that is suitable for script and actor execution process.
 This module contains a basic set of functions for normalizing data in a dialog script.
 """
 import logging
 
 from typing import Union, Callable, Any, Dict, Optional, ForwardRef
 
-from .keywords import GLOBAL, Keywords
+from .keywords import Keywords
 from .context import Context
 from .types import NodeLabel3Type, NodeLabelType, ConditionType, LabelType
 from .message import Message
 
 from pydantic import validate_arguments
 
 logger = logging.getLogger(__name__)
 
 Pipeline = ForwardRef("Pipeline")
 
 
-@validate_arguments
 def normalize_label(label: NodeLabelType, default_flow_label: LabelType = "") -> Union[Callable, NodeLabel3Type]:
     """
     The function that is used for normalization of
     :py:const:`default_flow_label <dff.script.NodeLabelType>`.
 
     :param label: If label is Callable the function is wrapped into try/except
         and normalization is used on the result of the function call with the name label.
     :param default_flow_label: flow_label is used if label does not contain flow_label.
     :return: Result of the label normalization,
         if Callable is returned, the normalized result is returned.
     """
-    if isinstance(label, Callable):
+    if callable(label):
 
         def get_label_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
             try:
                 new_label = label(ctx, pipeline, *args, **kwargs)
                 new_label = normalize_label(new_label, default_flow_label)
                 flow_label, node_label, _ = new_label
                 node = pipeline.script.get(flow_label, {}).get(node_label)
                 if not node:
                     raise Exception(f"Unknown transitions {new_label} for pipeline.script={pipeline.script}")
+                if node_label in [Keywords.LOCAL, Keywords.GLOBAL]:
+                    raise Exception(f"Invalid transition: can't transition to {flow_label}:{node_label}")
             except Exception as exc:
                 new_label = None
                 logger.error(f"Exception {exc} of function {label}", exc_info=exc)
             return new_label
 
         return get_label_handler  # create wrap to get uniq key for dictionary
     elif isinstance(label, str) or isinstance(label, Keywords):
@@ -57,23 +58,22 @@
         flow_label = label[0] or default_flow_label
         return (flow_label, label[-1], float("-inf"))
     elif isinstance(label, tuple) and len(label) == 3:
         flow_label = label[0] or default_flow_label
         return (flow_label, label[1], label[2])
 
 
-@validate_arguments
 def normalize_condition(condition: ConditionType) -> Callable:
     """
     The function that is used to normalize `condition`
 
     :param condition: Condition to normalize.
     :return: The function condition wrapped into the try/except.
     """
-    if isinstance(condition, Callable):
+    if callable(condition):
 
         def callable_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
             try:
                 return condition(ctx, pipeline, *args, **kwargs)
             except Exception as exc:
                 logger.error(f"Exception {exc} of function {condition}", exc_info=exc)
                 return False
@@ -100,15 +100,15 @@
     """
     This function is used to normalize response, if response Callable, it is returned, otherwise
     response is wrapped to the function and this function is returned.
 
     :param response: Response to normalize.
     :return: Function that returns callable response.
     """
-    if isinstance(response, Callable):
+    if callable(response):
         return response
     else:
         if response is None:
             result = Message()
         elif isinstance(response, Message):
             result = response
         else:
@@ -143,59 +143,21 @@
                     )
             return ctx
 
         return processing_handler
 
 
 @validate_arguments
-def map_deprecated_key(key: str) -> str:
-    """
-    This function is used to map deprecated keyword to new one.
-
-    :param key: A keyword of a node.
-    :return: A mapped keyword of a node.
-    """
-    if key == "processing":
-        logger.warning(
-            "Use the new key 'PRE_RESPONSE_PROCESSING instead of the deprecated key 'PROCESSING',"
-            " which will be removed in future versions."
-        )
-        return "pre_response_processing"
-    return key
-
-
-@validate_arguments
-def normalize_keywords(
-    script: Dict[LabelType, Dict[LabelType, Dict[Keywords, Any]]]
-) -> Dict[LabelType, Dict[LabelType, Dict[str, Any]]]:
-    """
-    This function is used to normalize keywords in the script.
-
-    :param script: :py:class:`.Script`, containing all transitions between states based in the keywords.
-    :return: :py:class:`.Script` with the normalized keywords.
-    """
-
-    script = {
-        flow_label: {
-            node_label: {map_deprecated_key(key.name.lower()): val for key, val in node.items()}
-            for node_label, node in flow.items()
-        }
-        for flow_label, flow in script.items()
-    }
-    return script
-
-
-@validate_arguments
 def normalize_script(script: Dict[LabelType, Any]) -> Dict[LabelType, Dict[LabelType, Dict[str, Any]]]:
     """
     This function normalizes :py:class:`.Script`: it returns dict where the GLOBAL node is moved
     into the flow with the GLOBAL name. The function returns the structure
 
     `{GLOBAL: {...NODE...}, ...}` -> `{GLOBAL: {GLOBAL: {...NODE...}}, ...}`.
 
     :param script: :py:class:`.Script` that describes the dialog scenario.
     :return: Normalized :py:class:`.Script`.
     """
     if isinstance(script, dict):
-        if GLOBAL in script and all([isinstance(item, Keywords) for item in script[GLOBAL].keys()]):
-            script[GLOBAL] = {GLOBAL: script[GLOBAL]}
-    return normalize_keywords(script)
+        if Keywords.GLOBAL in script and all([isinstance(item, Keywords) for item in script[Keywords.GLOBAL].keys()]):
+            script[Keywords.GLOBAL] = {Keywords.GLOBAL: script[Keywords.GLOBAL]}
+    return script
```

### Comparing `dff-0.4.1/dff/script/core/script.py` & `dff-0.4.2/dff/script/core/script.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/script/core/types.py` & `dff-0.4.2/dff/script/core/types.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/script/labels/std_labels.py` & `dff-0.4.2/dff/script/labels/std_labels.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/script/responses/std_responses.py` & `dff-0.4.2/dff/script/responses/std_responses.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/testing/cleanup_db.py` & `dff-0.4.2/dff/utils/testing/cleanup_db.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/testing/common.py` & `dff-0.4.2/dff/utils/testing/common.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/testing/response_comparers.py` & `dff-0.4.2/dff/utils/testing/response_comparers.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/testing/telegram.py` & `dff-0.4.2/dff/utils/testing/telegram.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/testing/toy_script.py` & `dff-0.4.2/dff/utils/testing/toy_script.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff/utils/turn_caching/singleton_turn_caching.py` & `dff-0.4.2/dff/utils/turn_caching/singleton_turn_caching.py`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/dff.egg-info/PKG-INFO` & `dff-0.4.2/dff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dff
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Dialog Flow Framework (DFF) allows you to write conversational services.
 Home-page: https://github.com/deeppavlov/dialog_flow_framework
 Author: Denis Kuznetsov
 Author-email: kuznetsov.den.p@gmail.com
 Keywords: chatbots
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dff-0.4.1/dff.egg-info/SOURCES.txt` & `dff-0.4.2/dff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dff-0.4.1/setup.py` & `dff-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,65 +23,64 @@
     for req_list in req_lists:
         for req in req_list:
             result.add(req)
     return list(result)
 
 
 core = [
-    "pydantic>=1.8.2",
-    "nest_asyncio>=1.5.5",
-    "typing_extensions>=4.0.0",
+    "pydantic<2.0",
+    "nest-asyncio",
+    "typing-extensions",
 ]
 
 async_files_dependencies = [
-    "aiofiles>=22.1.0",
+    "aiofiles",
 ]
 
 redis_dependencies = [
-    "aioredis>=2.0.1",
+    "redis",
 ]
 
 mongodb_dependencies = [
-    "motor>=3.1.1",
+    "motor",
 ]
 
 _sql_dependencies = [
-    "sqlalchemy[asyncio]>=2.0.2",
+    "sqlalchemy[asyncio]",
 ]
 
 sqlite_dependencies = merge_req_lists(
     _sql_dependencies,
     [
-        "aiosqlite>=0.18.0",
-        "sqlalchemy[asyncio]>=1.4.27",
+        "aiosqlite",
     ],
 )
 
 mysql_dependencies = merge_req_lists(
     _sql_dependencies,
     [
-        "asyncmy>=0.2.5",
-        "cryptography>=36.0.2",
+        "asyncmy",
+        "cryptography",
     ],
 )
 
 postgresql_dependencies = merge_req_lists(
     _sql_dependencies,
     [
-        "asyncpg>=0.27.0",
+        "asyncpg",
     ],
 )
 
 ydb_dependencies = [
-    "ydb~=2.5.0",
-    "six>=1.16.0",
+    "ydb",
+    "six",
 ]
 
 telegram_dependencies = [
-    "pytelegrambotapi==4.5.1",
+    "pytelegrambotapi",
 ]
 
 full = merge_req_lists(
     core,
     async_files_dependencies,
     sqlite_dependencies,
     redis_dependencies,
@@ -89,72 +88,74 @@
     mysql_dependencies,
     postgresql_dependencies,
     ydb_dependencies,
     telegram_dependencies,
 )
 
 requests_requirements = [
-    "requests>=2.28.1",
+    "requests==2.31.0",
 ]
 
 test_requirements = merge_req_lists(
     [
-        "pytest >=7.2.1,<8.0.0",
-        "pytest-cov >=4.0.0,<5.0.0",
-        "pytest-asyncio >=0.14.0,<0.15.0",
-        "flake8 >=3.8.3,<4.0.0",
-        "click<=8.0.4",
-        "black ==20.8b1",
-        "isort >=5.0.6,<6.0.0",
-        "flask[async]>=2.1.2",
-        "psutil>=5.9.1",
-        "telethon>=1.27.0,<2.0",
-        "anyio>=3.6.2",
-        "fastapi>=0.95.1",
-        "idna>=3.4",
-        "sniffio>=1.3.0",
-        "starlette>=0.26.1",
-        "h11>=0.14.0",
-        "uvicorn>=0.21.1",
-        "websockets>=11.0",
+        "pytest==7.3.1",
+        "pytest-cov==4.1.0",
+        "pytest-asyncio==0.21.0",
+        "flake8==6.0.0; python_version>'3.7'",
+        "flake8==3.9.2; python_version=='3.7'",
+        "click==8.1.3",
+        "black==23.3.0",
+        "isort==5.12.0; python_version>'3.7'",
+        "isort==5.11.5; python_version=='3.7'",
+        "flask[async]==2.3.2; python_version>'3.7'",
+        "flask[async]==2.2.3; python_version=='3.7'",
+        "psutil==5.9.5",
+        "telethon==1.28.5",
+        "fastapi==0.97.0",
+        "uvicorn==0.22.0",
+        "websockets==11.0.2",
+        "locust==2.15",
+        "streamlit~=1.23.1",
+        "streamlit-chat~=0.1.1",
     ],
     requests_requirements,
 )
 
 tests_full = merge_req_lists(
     full,
     test_requirements,
 )
 
 doc = merge_req_lists(
     [
-        "sphinx<6",
-        "pydata_sphinx_theme>=0.12.0",
+        "sphinx==7.0.1; python_version>'3.7'",
+        "sphinx==5.3.0; python_version=='3.7'",
+        "pydata-sphinx-theme==0.13.3",
         "sphinxcontrib-apidoc==0.3.0",
-        "sphinxcontrib-httpdomain>=1.8.0",
+        "sphinxcontrib-httpdomain==1.8.0",
         "sphinxcontrib-katex==0.9.0",
-        "sphinx-favicon>=1.0.1",
-        "sphinx_copybutton>=0.5",
-        "sphinx_gallery==0.7.0",
-        "sphinx-autodoc-typehints>=1.19.4",
-        "nbsphinx>=0.8.9",
-        "jupytext>=1.14.1",
-        "jupyter>=1.0.0",
+        "sphinx-favicon==1.0.1",
+        "sphinx-copybutton==0.5.2",
+        "sphinx-gallery==0.13.0",
+        "sphinx-autodoc-typehints==1.23.0",
+        "nbsphinx==0.9.1",
+        "jupytext==1.14.5",
+        "jupyter==1.0.0",
     ],
     requests_requirements,
 )
 
 devel = [
-    "bump2version>=1.0.1",
-    "build==0.7.0",
+    "bump2version==1.0.1",
+    "build==0.10.0",
     "twine==4.0.0",
 ]
 
 mypy_dependencies = [
-    "mypy==0.950",
+    "mypy==1.3.0",
 ]
 
 devel_full = merge_req_lists(
     tests_full,
     doc,
     devel,
     mypy_dependencies,
@@ -178,37 +179,34 @@
     "devel": devel,  # dependencies for development
     "doc": doc,  # dependencies for documentation
     "devel_full": devel_full,  # full dependencies for development (all options above)
 }
 
 setup(
     name="dff",
-    version="0.4.1",
+    version="0.4.2",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deeppavlov/dialog_flow_framework",
     author="Denis Kuznetsov",
     author_email="kuznetsov.den.p@gmail.com",
-    classifiers=[  # Optional
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
+    classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3 :: Only",
     ],
-    keywords="chatbots",  # Optional
-    packages=find_packages(where="."),  # Required
+    keywords="chatbots",
+    packages=find_packages(where="."),
     include_package_data=True,
     python_requires=">=3.7, <4",
-    install_requires=core,  # Optional
+    install_requires=core,
     test_suite="tests",
     extras_require=EXTRA_DEPENDENCIES,
 )
```

