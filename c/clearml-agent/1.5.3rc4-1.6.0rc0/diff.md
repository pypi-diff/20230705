# Comparing `tmp/clearml_agent-1.5.3rc4-py3-none-any.whl.zip` & `tmp/clearml_agent-1.6.0rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,131 +1,135 @@
-Zip file size: 403035 bytes, number of entries: 129
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-15 07:28 clearml_agent/__init__.py
--rw-r--r--  2.0 unx     2891 b- defN 23-Jun-15 07:28 clearml_agent/__main__.py
--rw-r--r--  2.0 unx     2410 b- defN 23-Jun-15 07:28 clearml_agent/complete.py
--rw-r--r--  2.0 unx      736 b- defN 23-Jun-15 07:28 clearml_agent/config.py
--rw-r--r--  2.0 unx    11218 b- defN 23-Jun-15 07:28 clearml_agent/definitions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-Jun-15 07:28 clearml_agent/errors.py
--rw-r--r--  2.0 unx    15942 b- defN 23-Jun-15 07:28 clearml_agent/session.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-15 07:28 clearml_agent/version.py
--rw-r--r--  2.0 unx      123 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/__init__.py
--rw-r--r--  2.0 unx     4786 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/utils.py
--rw-r--r--  2.0 unx      561 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/config/__init__.py
--rw-r--r--  2.0 unx    20435 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/config/default/agent.conf
--rw-r--r--  2.0 unx     1796 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/config/default/api.conf
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/config/default/logging.conf
--rw-r--r--  2.0 unx     6857 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/config/default/sdk.conf
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/schema/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/schema/action.py
--rw-r--r--  2.0 unx     6824 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/schema/service.py
--rw-r--r--  2.0 unx      282 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/__init__.py
--rw-r--r--  2.0 unx    17434 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/auth.py
--rw-r--r--  2.0 unx     4029 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/debug.py
--rw-r--r--  2.0 unx    89217 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/events.py
--rw-r--r--  2.0 unx    90805 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/models.py
--rw-r--r--  2.0 unx    66636 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/queues.py
--rw-r--r--  2.0 unx   218713 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/tasks.py
--rw-r--r--  2.0 unx    77983 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_4/workers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/__init__.py
--rw-r--r--  2.0 unx    17434 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/auth.py
--rw-r--r--  2.0 unx     4029 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/debug.py
--rw-r--r--  2.0 unx    90043 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/events.py
--rw-r--r--  2.0 unx    90805 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/models.py
--rw-r--r--  2.0 unx    66636 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/queues.py
--rw-r--r--  2.0 unx   234295 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/tasks.py
--rw-r--r--  2.0 unx    77996 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/services/v2_5/workers.py
--rw-r--r--  2.0 unx      338 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/__init__.py
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/apimodel.py
--rw-r--r--  2.0 unx     5233 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/callresult.py
--rw-r--r--  2.0 unx     4598 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/datamodel.py
--rw-r--r--  2.0 unx     1963 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/defs.py
--rw-r--r--  2.0 unx      345 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/errors.py
--rw-r--r--  2.0 unx     2817 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/request.py
--rw-r--r--  2.0 unx     1932 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/response.py
--rw-r--r--  2.0 unx    28237 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/session.py
--rw-r--r--  2.0 unx     4200 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/token_manager.py
--rw-r--r--  2.0 unx       55 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/client/__init__.py
--rw-r--r--  2.0 unx    16055 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/client/client.py
--rw-r--r--  2.0 unx      175 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/__init__.py
--rw-r--r--  2.0 unx     6397 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/builders.py
--rw-r--r--  2.0 unx      552 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/collections.py
--rw-r--r--  2.0 unx      145 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/errors.py
--rw-r--r--  2.0 unx    13503 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/fields.py
--rw-r--r--  2.0 unx     4738 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/models.py
--rw-r--r--  2.0 unx     2993 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/parsers.py
--rw-r--r--  2.0 unx     4006 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/utilities.py
--rw-r--r--  2.0 unx     6294 b- defN 23-Jun-15 07:28 clearml_agent/backend_api/session/jsonmodels/validators.py
--rw-r--r--  2.0 unx      109 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/__init__.py
--rw-r--r--  2.0 unx    12445 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/config.py
--rw-r--r--  2.0 unx     1704 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/converters.py
--rw-r--r--  2.0 unx     1776 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/defs.py
--rw-r--r--  2.0 unx     3531 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/entry.py
--rw-r--r--  2.0 unx     2163 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/environment.py
--rw-r--r--  2.0 unx      186 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/errors.py
--rw-r--r--  2.0 unx      851 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/log.py
--rw-r--r--  2.0 unx     4219 b- defN 23-Jun-15 07:28 clearml_agent/backend_config/utils.py
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-15 07:28 clearml_agent/commands/__init__.py
--rw-r--r--  2.0 unx    15160 b- defN 23-Jun-15 07:28 clearml_agent/commands/base.py
--rw-r--r--  2.0 unx      536 b- defN 23-Jun-15 07:28 clearml_agent/commands/check_config.py
--rw-r--r--  2.0 unx    17027 b- defN 23-Jun-15 07:28 clearml_agent/commands/config.py
--rw-r--r--  2.0 unx     3204 b- defN 23-Jun-15 07:28 clearml_agent/commands/events.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Jun-15 07:28 clearml_agent/commands/resolver.py
--rw-r--r--  2.0 unx   191566 b- defN 23-Jun-15 07:28 clearml_agent/commands/worker.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/external/__init__.py
--rw-r--r--  2.0 unx      256 b- defN 23-Jun-15 07:28 clearml_agent/external/pyhocon/__init__.py
--rw-r--r--  2.0 unx    32918 b- defN 23-Jun-15 07:28 clearml_agent/external/pyhocon/config_parser.py
--rw-r--r--  2.0 unx    22532 b- defN 23-Jun-15 07:28 clearml_agent/external/pyhocon/config_tree.py
--rw-r--r--  2.0 unx    13100 b- defN 23-Jun-15 07:28 clearml_agent/external/pyhocon/converter.py
--rw-r--r--  2.0 unx      352 b- defN 23-Jun-15 07:28 clearml_agent/external/pyhocon/exceptions.py
--rw-r--r--  2.0 unx      353 b- defN 23-Jun-15 07:28 clearml_agent/external/requirements_parser/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 23-Jun-15 07:28 clearml_agent/external/requirements_parser/fragment.py
--rw-r--r--  2.0 unx     2368 b- defN 23-Jun-15 07:28 clearml_agent/external/requirements_parser/parser.py
--rw-r--r--  2.0 unx     9362 b- defN 23-Jun-15 07:28 clearml_agent/external/requirements_parser/requirement.py
--rw-r--r--  2.0 unx      405 b- defN 23-Jun-15 07:28 clearml_agent/external/requirements_parser/vcs.py
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-15 07:28 clearml_agent/glue/__init__.py
--rw-r--r--  2.0 unx      316 b- defN 23-Jun-15 07:28 clearml_agent/glue/definitions.py
--rw-r--r--  2.0 unx    47157 b- defN 23-Jun-15 07:28 clearml_agent/glue/k8s.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/helper/__init__.py
--rw-r--r--  2.0 unx    18556 b- defN 23-Jun-15 07:28 clearml_agent/helper/base.py
--rw-r--r--  2.0 unx     2200 b- defN 23-Jun-15 07:28 clearml_agent/helper/check_update.py
--rw-r--r--  2.0 unx     3650 b- defN 23-Jun-15 07:28 clearml_agent/helper/console.py
--rw-r--r--  2.0 unx      828 b- defN 23-Jun-15 07:28 clearml_agent/helper/dicts.py
--rw-r--r--  2.0 unx     3403 b- defN 23-Jun-15 07:28 clearml_agent/helper/docker_args.py
--rw-r--r--  2.0 unx    15065 b- defN 23-Jun-15 07:28 clearml_agent/helper/process.py
--rw-r--r--  2.0 unx    30196 b- defN 23-Jun-15 07:28 clearml_agent/helper/repo.py
--rw-r--r--  2.0 unx    11656 b- defN 23-Jun-15 07:28 clearml_agent/helper/resource_monitor.py
--rw-r--r--  2.0 unx     5470 b- defN 23-Jun-15 07:28 clearml_agent/helper/runtime_verification.py
--rw-r--r--  2.0 unx     6697 b- defN 23-Jun-15 07:28 clearml_agent/helper/singleton.py
--rw-r--r--  2.0 unx     4759 b- defN 23-Jun-15 07:28 clearml_agent/helper/trace.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/helper/gpu/__init__.py
--rw-r--r--  2.0 unx    14101 b- defN 23-Jun-15 07:28 clearml_agent/helper/gpu/gpustat.py
--rw-r--r--  2.0 unx   122691 b- defN 23-Jun-15 07:28 clearml_agent/helper/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/helper/os/__init__.py
--rw-r--r--  2.0 unx     2949 b- defN 23-Jun-15 07:28 clearml_agent/helper/os/daemonize.py
--rw-r--r--  2.0 unx     9311 b- defN 23-Jun-15 07:28 clearml_agent/helper/os/folder_cache.py
--rw-r--r--  2.0 unx     6180 b- defN 23-Jun-15 07:28 clearml_agent/helper/os/locks.py
--rw-r--r--  2.0 unx     6966 b- defN 23-Jun-15 07:28 clearml_agent/helper/os/portalocker.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/__init__.py
--rw-r--r--  2.0 unx    11518 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/base.py
--rw-r--r--  2.0 unx    32312 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/conda_api.py
--rw-r--r--  2.0 unx     8224 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/external_req.py
--rw-r--r--  2.0 unx     6181 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/poetry_api.py
--rw-r--r--  2.0 unx     1764 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/post_req.py
--rw-r--r--  2.0 unx     4257 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/priority_req.py
--rw-r--r--  2.0 unx    40778 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/pytorch.py
--rw-r--r--  2.0 unx    31340 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/requirements.py
--rw-r--r--  2.0 unx     3452 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/translator.py
--rw-r--r--  2.0 unx     3401 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/venv_update_api.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/pip_api/__init__.py
--rw-r--r--  2.0 unx     3360 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/pip_api/system.py
--rw-r--r--  2.0 unx     2951 b- defN 23-Jun-15 07:28 clearml_agent/helper/package/pip_api/venv.py
--rw-r--r--  2.0 unx     1244 b- defN 23-Jun-15 07:28 clearml_agent/interface/__init__.py
--rw-r--r--  2.0 unx    15036 b- defN 23-Jun-15 07:28 clearml_agent/interface/base.py
--rw-r--r--  2.0 unx     9937 b- defN 23-Jun-15 07:28 clearml_agent/interface/worker.py
--rw-r--r--  2.0 unx    11340 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/LICENSE
--rw-r--r--  2.0 unx    18199 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12619 b- defN 23-Jun-15 07:28 clearml_agent-1.5.3rc4.dist-info/RECORD
-129 files, 2204242 bytes uncompressed, 382523 bytes compressed:  82.7%
+Zip file size: 408354 bytes, number of entries: 133
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-04 11:27 clearml_agent/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Jul-04 11:27 clearml_agent/__main__.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Jul-04 11:27 clearml_agent/complete.py
+-rw-r--r--  2.0 unx      736 b- defN 23-Jul-04 11:27 clearml_agent/config.py
+-rw-r--r--  2.0 unx    11312 b- defN 23-Jul-04 11:27 clearml_agent/definitions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Jul-04 11:27 clearml_agent/errors.py
+-rw-r--r--  2.0 unx    15942 b- defN 23-Jul-04 11:27 clearml_agent/session.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-04 11:27 clearml_agent/version.py
+-rw-r--r--  2.0 unx      123 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/__init__.py
+-rw-r--r--  2.0 unx     4786 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/utils.py
+-rw-r--r--  2.0 unx      561 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/config/__init__.py
+-rw-r--r--  2.0 unx    20435 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/config/default/agent.conf
+-rw-r--r--  2.0 unx     1796 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/config/default/api.conf
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/config/default/logging.conf
+-rw-r--r--  2.0 unx     6857 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/config/default/sdk.conf
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/schema/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/schema/action.py
+-rw-r--r--  2.0 unx     6824 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/schema/service.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/__init__.py
+-rw-r--r--  2.0 unx    17434 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/auth.py
+-rw-r--r--  2.0 unx     4029 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/debug.py
+-rw-r--r--  2.0 unx    89217 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/events.py
+-rw-r--r--  2.0 unx    90805 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/models.py
+-rw-r--r--  2.0 unx    66636 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/queues.py
+-rw-r--r--  2.0 unx   218713 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/tasks.py
+-rw-r--r--  2.0 unx    77983 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_4/workers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/__init__.py
+-rw-r--r--  2.0 unx    17434 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/auth.py
+-rw-r--r--  2.0 unx     4029 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/debug.py
+-rw-r--r--  2.0 unx    90043 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/events.py
+-rw-r--r--  2.0 unx    90805 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/models.py
+-rw-r--r--  2.0 unx    66636 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/queues.py
+-rw-r--r--  2.0 unx   234295 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/tasks.py
+-rw-r--r--  2.0 unx    77996 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/services/v2_5/workers.py
+-rw-r--r--  2.0 unx      338 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/__init__.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/apimodel.py
+-rw-r--r--  2.0 unx     5233 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/callresult.py
+-rw-r--r--  2.0 unx     4598 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/datamodel.py
+-rw-r--r--  2.0 unx     1963 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/defs.py
+-rw-r--r--  2.0 unx      345 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/errors.py
+-rw-r--r--  2.0 unx     2817 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/request.py
+-rw-r--r--  2.0 unx     1932 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/response.py
+-rw-r--r--  2.0 unx    28237 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/session.py
+-rw-r--r--  2.0 unx     4200 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/token_manager.py
+-rw-r--r--  2.0 unx       55 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/client/__init__.py
+-rw-r--r--  2.0 unx    16055 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/client/client.py
+-rw-r--r--  2.0 unx      175 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/__init__.py
+-rw-r--r--  2.0 unx     6397 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/builders.py
+-rw-r--r--  2.0 unx      552 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/collections.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/errors.py
+-rw-r--r--  2.0 unx    13503 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/fields.py
+-rw-r--r--  2.0 unx     4738 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/models.py
+-rw-r--r--  2.0 unx     2993 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/parsers.py
+-rw-r--r--  2.0 unx     4006 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/utilities.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-Jul-04 11:27 clearml_agent/backend_api/session/jsonmodels/validators.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/__init__.py
+-rw-r--r--  2.0 unx    12445 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/config.py
+-rw-r--r--  2.0 unx     1704 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/converters.py
+-rw-r--r--  2.0 unx     1776 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/defs.py
+-rw-r--r--  2.0 unx     3531 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/entry.py
+-rw-r--r--  2.0 unx     2163 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/environment.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/errors.py
+-rw-r--r--  2.0 unx      851 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/log.py
+-rw-r--r--  2.0 unx     4219 b- defN 23-Jul-04 11:27 clearml_agent/backend_config/utils.py
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-04 11:27 clearml_agent/commands/__init__.py
+-rw-r--r--  2.0 unx    15160 b- defN 23-Jul-04 11:27 clearml_agent/commands/base.py
+-rw-r--r--  2.0 unx      536 b- defN 23-Jul-04 11:27 clearml_agent/commands/check_config.py
+-rw-r--r--  2.0 unx    17027 b- defN 23-Jul-04 11:27 clearml_agent/commands/config.py
+-rw-r--r--  2.0 unx     3204 b- defN 23-Jul-04 11:27 clearml_agent/commands/events.py
+-rw-r--r--  2.0 unx     6552 b- defN 23-Jul-04 11:27 clearml_agent/commands/resolver.py
+-rw-r--r--  2.0 unx   194477 b- defN 23-Jul-04 11:27 clearml_agent/commands/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/external/__init__.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Jul-04 11:27 clearml_agent/external/pyhocon/__init__.py
+-rw-r--r--  2.0 unx    32918 b- defN 23-Jul-04 11:27 clearml_agent/external/pyhocon/config_parser.py
+-rw-r--r--  2.0 unx    22532 b- defN 23-Jul-04 11:27 clearml_agent/external/pyhocon/config_tree.py
+-rw-r--r--  2.0 unx    13100 b- defN 23-Jul-04 11:27 clearml_agent/external/pyhocon/converter.py
+-rw-r--r--  2.0 unx      352 b- defN 23-Jul-04 11:27 clearml_agent/external/pyhocon/exceptions.py
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-04 11:27 clearml_agent/external/requirements_parser/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 23-Jul-04 11:27 clearml_agent/external/requirements_parser/fragment.py
+-rw-r--r--  2.0 unx     2368 b- defN 23-Jul-04 11:27 clearml_agent/external/requirements_parser/parser.py
+-rw-r--r--  2.0 unx     9362 b- defN 23-Jul-04 11:27 clearml_agent/external/requirements_parser/requirement.py
+-rw-r--r--  2.0 unx      405 b- defN 23-Jul-04 11:27 clearml_agent/external/requirements_parser/vcs.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-04 11:27 clearml_agent/glue/__init__.py
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-04 11:27 clearml_agent/glue/daemon.py
+-rw-r--r--  2.0 unx      316 b- defN 23-Jul-04 11:27 clearml_agent/glue/definitions.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-04 11:27 clearml_agent/glue/errors.py
+-rw-r--r--  2.0 unx    48544 b- defN 23-Jul-04 11:27 clearml_agent/glue/k8s.py
+-rw-r--r--  2.0 unx     9773 b- defN 23-Jul-04 11:27 clearml_agent/glue/pending_pods_daemon.py
+-rw-r--r--  2.0 unx      452 b- defN 23-Jul-04 11:27 clearml_agent/glue/utilities.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/helper/__init__.py
+-rw-r--r--  2.0 unx    18669 b- defN 23-Jul-04 11:27 clearml_agent/helper/base.py
+-rw-r--r--  2.0 unx     2200 b- defN 23-Jul-04 11:27 clearml_agent/helper/check_update.py
+-rw-r--r--  2.0 unx     3650 b- defN 23-Jul-04 11:27 clearml_agent/helper/console.py
+-rw-r--r--  2.0 unx      828 b- defN 23-Jul-04 11:27 clearml_agent/helper/dicts.py
+-rw-r--r--  2.0 unx     3403 b- defN 23-Jul-04 11:27 clearml_agent/helper/docker_args.py
+-rw-r--r--  2.0 unx    15065 b- defN 23-Jul-04 11:27 clearml_agent/helper/process.py
+-rw-r--r--  2.0 unx    30196 b- defN 23-Jul-04 11:27 clearml_agent/helper/repo.py
+-rw-r--r--  2.0 unx    11656 b- defN 23-Jul-04 11:27 clearml_agent/helper/resource_monitor.py
+-rw-r--r--  2.0 unx     5470 b- defN 23-Jul-04 11:27 clearml_agent/helper/runtime_verification.py
+-rw-r--r--  2.0 unx     6697 b- defN 23-Jul-04 11:27 clearml_agent/helper/singleton.py
+-rw-r--r--  2.0 unx     4759 b- defN 23-Jul-04 11:27 clearml_agent/helper/trace.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/helper/gpu/__init__.py
+-rw-r--r--  2.0 unx    14101 b- defN 23-Jul-04 11:27 clearml_agent/helper/gpu/gpustat.py
+-rw-r--r--  2.0 unx   122691 b- defN 23-Jul-04 11:27 clearml_agent/helper/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/helper/os/__init__.py
+-rw-r--r--  2.0 unx     2949 b- defN 23-Jul-04 11:27 clearml_agent/helper/os/daemonize.py
+-rw-r--r--  2.0 unx     9311 b- defN 23-Jul-04 11:27 clearml_agent/helper/os/folder_cache.py
+-rw-r--r--  2.0 unx     6180 b- defN 23-Jul-04 11:27 clearml_agent/helper/os/locks.py
+-rw-r--r--  2.0 unx     6966 b- defN 23-Jul-04 11:27 clearml_agent/helper/os/portalocker.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/__init__.py
+-rw-r--r--  2.0 unx    11699 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/base.py
+-rw-r--r--  2.0 unx    32312 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/conda_api.py
+-rw-r--r--  2.0 unx     8224 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/external_req.py
+-rw-r--r--  2.0 unx     6212 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/poetry_api.py
+-rw-r--r--  2.0 unx     1764 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/post_req.py
+-rw-r--r--  2.0 unx     4761 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/priority_req.py
+-rw-r--r--  2.0 unx    40778 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/pytorch.py
+-rw-r--r--  2.0 unx    31340 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/requirements.py
+-rw-r--r--  2.0 unx     3452 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/translator.py
+-rw-r--r--  2.0 unx     3401 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/venv_update_api.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/pip_api/__init__.py
+-rw-r--r--  2.0 unx     4063 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/pip_api/system.py
+-rw-r--r--  2.0 unx     2951 b- defN 23-Jul-04 11:27 clearml_agent/helper/package/pip_api/venv.py
+-rw-r--r--  2.0 unx     1244 b- defN 23-Jul-04 11:27 clearml_agent/interface/__init__.py
+-rw-r--r--  2.0 unx    15036 b- defN 23-Jul-04 11:27 clearml_agent/interface/base.py
+-rw-r--r--  2.0 unx     9937 b- defN 23-Jul-04 11:27 clearml_agent/interface/worker.py
+-rw-r--r--  2.0 unx    11340 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18199 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12972 b- defN 23-Jul-04 11:27 clearml_agent-1.6.0rc0.dist-info/RECORD
+133 files, 2221232 bytes uncompressed, 387282 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -246,20 +246,32 @@
 
 Filename: clearml_agent/external/requirements_parser/vcs.py
 Comment: 
 
 Filename: clearml_agent/glue/__init__.py
 Comment: 
 
+Filename: clearml_agent/glue/daemon.py
+Comment: 
+
 Filename: clearml_agent/glue/definitions.py
 Comment: 
 
+Filename: clearml_agent/glue/errors.py
+Comment: 
+
 Filename: clearml_agent/glue/k8s.py
 Comment: 
 
+Filename: clearml_agent/glue/pending_pods_daemon.py
+Comment: 
+
+Filename: clearml_agent/glue/utilities.py
+Comment: 
+
 Filename: clearml_agent/helper/__init__.py
 Comment: 
 
 Filename: clearml_agent/helper/base.py
 Comment: 
 
 Filename: clearml_agent/helper/check_update.py
@@ -363,26 +375,26 @@
 
 Filename: clearml_agent/interface/base.py
 Comment: 
 
 Filename: clearml_agent/interface/worker.py
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/LICENSE
+Filename: clearml_agent-1.6.0rc0.dist-info/LICENSE
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/METADATA
+Filename: clearml_agent-1.6.0rc0.dist-info/METADATA
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/WHEEL
+Filename: clearml_agent-1.6.0rc0.dist-info/WHEEL
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/entry_points.txt
+Filename: clearml_agent-1.6.0rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/top_level.txt
+Filename: clearml_agent-1.6.0rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: clearml_agent-1.5.3rc4.dist-info/RECORD
+Filename: clearml_agent-1.6.0rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clearml_agent/definitions.py

```diff
@@ -148,14 +148,15 @@
 
 DEFAULT_VENV_UPDATE_URL = "https://raw.githubusercontent.com/Yelp/venv-update/v3.2.4/venv_update.py"
 WORKING_REPOSITORY_DIR = "task_repository"
 WORKING_STANDALONE_DIR = "code"
 DEFAULT_VCS_CACHE = normalize_path(CONFIG_DIR, "vcs-cache")
 PIP_EXTRA_INDICES = []
 DEFAULT_PIP_DOWNLOAD_CACHE = normalize_path(CONFIG_DIR, "pip-download-cache")
+ENV_PIP_EXTRA_INSTALL_FLAGS = EnvironmentConfig("CLEARML_EXTRA_PIP_INSTALL_FLAGS", type=list)
 ENV_DOCKER_IMAGE = EnvironmentConfig("CLEARML_DOCKER_IMAGE", "TRAINS_DOCKER_IMAGE")
 ENV_WORKER_ID = EnvironmentConfig("CLEARML_WORKER_ID", "TRAINS_WORKER_ID")
 ENV_WORKER_TAGS = EnvironmentConfig("CLEARML_WORKER_TAGS")
 ENV_AGENT_SKIP_PIP_VENV_INSTALL = EnvironmentConfig("CLEARML_AGENT_SKIP_PIP_VENV_INSTALL")
 ENV_AGENT_SKIP_PYTHON_ENV_INSTALL = EnvironmentConfig("CLEARML_AGENT_SKIP_PYTHON_ENV_INSTALL", type=bool)
 ENV_DOCKER_SKIP_GPUS_FLAG = EnvironmentConfig("CLEARML_DOCKER_SKIP_GPUS_FLAG", "TRAINS_DOCKER_SKIP_GPUS_FLAG")
 ENV_AGENT_GIT_USER = EnvironmentConfig("CLEARML_AGENT_GIT_USER", "TRAINS_AGENT_GIT_USER")
```

## clearml_agent/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.3rc4'
+__version__ = '1.6.0rc0'
```

## clearml_agent/commands/worker.py

```diff
@@ -8,27 +8,28 @@
 import os.path
 import random
 import re
 import shlex
 import shutil
 import signal
 import string
+import socket
 import subprocess
 import sys
 import traceback
 from collections import defaultdict
 from copy import deepcopy, copy
 from datetime import datetime
 from distutils.spawn import find_executable
 from distutils.util import strtobool
 from functools import partial
 from os.path import basename
 from tempfile import mkdtemp, NamedTemporaryFile
 from time import sleep, time
-from typing import Text, Optional, Any, Tuple, List
+from typing import Text, Optional, Any, Tuple, List, Dict, Mapping, Union
 
 import attr
 import six
 from pathlib2 import Path
 from six.moves.urllib.parse import quote
 
 from clearml_agent.external.pyhocon import ConfigTree, ConfigFactory
@@ -364,14 +365,16 @@
             method=Request.def_method,
             async_enable=False,
         )
         try:
             container = result.json()['data']['tasks'][0]['container'] if result.ok else {}
             if container.get('arguments'):
                 container['arguments'] = shlex.split(str(container.get('arguments')).strip())
+            if container.get('image'):
+                container['image'] = container.get('image').strip()
         except (ValueError, TypeError):
             container = {}
     else:
         response = get_task(session, task_id, only_fields=["execution.docker_cmd"])
         container = {}
         if response.execution:
             task_docker_cmd_parts = shlex.split(str(response.execution.docker_cmd or '').strip())
@@ -631,14 +634,16 @@
     # label with parent worker id for worker agent docker in services mode
     _parent_worker_label = "clearml-parent-worker-id={}"
 
     _run_as_user_home = '/clearml_agent_home'
     _docker_fixed_user_cache = '/clearml_agent_cache'
     _temp_cleanup_list = []
 
+    hostname_task_runtime_prop = "_exec_agent_hostname"
+
     @property
     def service(self):
         """ Worker command service endpoint """
         return "workers"
 
     @property
     def _task_status_change_message(self):
@@ -846,14 +851,28 @@
 
         :return: exit code (0 is success)
         """
         # start new process and execute task id
         # "Running task '{}'".format(task_id)
         print(self._task_logging_start_message.format(task_id))
         task_session = task_session or self._session
+
+        # noinspection PyBroadException
+        try:
+            res = task_session.send_request(
+                service='tasks', action='edit', method=Request.def_method,
+                json={
+                    "task": task_id, "force": True, "runtime": {self.hostname_task_runtime_prop: socket.gethostname()}
+                },
+            )
+            if not res.ok:
+                raise Exception("failed setting runtime property")
+        except Exception as ex:
+            print("Warning: failed obtaining/setting hostname for task '{}': {}".format(task_id, ex))
+
         # set task status to in_progress so we know it was popped from the queue
         # noinspection PyBroadException
         try:
             task_session.send_api(tasks_api.StartedRequest(task=task_id, status_message="pulled by agent", force=True))
         except Exception:
             print("Warning: Could not start task id '{}', skipping".format(task_id))
             return
@@ -2348,14 +2367,15 @@
                     ).id
                 )
                 print("Task cloned, new task id={}".format(current_task.id))
             except Exception:
                 raise CommandFailedError("Cloning failed")
         else:
             # make sure this task is not stuck in an execution queue, it shouldn't have been, but just in case.
+            # noinspection PyBroadException
             try:
                 res = self._session.api_client.tasks.dequeue(task=current_task.id)
                 if require_queue and res.meta.result_code != 200:
                     raise ValueError("Execution required enqueued task, "
                                      "but task id={} is not queued.".format(current_task.id))
             except Exception:
                 if require_queue:
@@ -3816,14 +3836,68 @@
                 if "=" not in cmd and args and not args[0].startswith("-"):
                     try:
                         results.append(args.pop(0).strip())
                     except IndexError:
                         pass
         return results
 
+    @staticmethod
+    def _resolve_docker_env_args(docker_args):
+        # type: (List[str]) -> List[str]
+        """
+        Resolve -e / --env docker environment args matching $VAR or ${VAR} from the host environment
+
+        :argument docker_args: List of docker argument strings (flags and values)
+        """
+        non_list_args = (
+            "rm", "read-only", "sig-proxy", "tty", "privileged", "publish-all", "interactive", "init", "help", "detach"
+        )
+        non_list_args_single = (
+            "t", "P", "i", "d",
+        )
+
+        # if no filtering, do nothing
+        if not docker_args:
+            return docker_args
+
+        args = docker_args[:]
+        skip_arg = False
+        for i, cmd in enumerate(docker_args):
+            if skip_arg and not cmd.startswith("-"):
+                continue
+
+            skip_arg = False
+
+            if cmd.startswith("--"):
+                # jump over single command
+                if cmd[2:] in non_list_args:
+                    continue
+            elif cmd.startswith("-"):
+                # jump over single character non args
+                if cmd[1:] in non_list_args_single:
+                    continue
+
+            # if we are here we have a command to bypass and the list after it
+            if cmd in ('-e', '--env'):
+                skip_arg = True
+                for j in range(i+1, len(args)):
+                    if args[j].startswith("-"):
+                        break
+
+                    parts = args[j].split("=", 1)
+                    if len(parts) != 2:
+                        continue
+
+                    args[j] = "{}={}".format(parts[0], os.path.expandvars(parts[1]))
+
+            elif cmd.startswith("-"):
+                skip_arg = True
+
+        return args
+
     def _get_docker_cmd(
             self,
             worker_id, parent_worker_id,
             docker_image, docker_arguments,
             python_version,
             conf_file,
             host_apt_cache,
@@ -3879,17 +3953,22 @@
         elif gpu_devices.strip() == 'none':
             dockers_nvidia_visible_devices = gpu_devices
 
         if docker_arguments:
             docker_arguments = list(docker_arguments) \
                 if isinstance(docker_arguments, (list, tuple)) else [docker_arguments]
             docker_arguments = self._filter_docker_args(docker_arguments)
+            if self._session.config.get("agent.docker_allow_host_environ", None):
+                docker_arguments = self._resolve_docker_env_args(docker_arguments)
             base_cmd += [a for a in docker_arguments if a]
 
         if extra_docker_arguments:
+            # we always resolve environments in the `extra_docker_arguments` becuase the admin set them (not users)
+            extra_docker_arguments = self._resolve_docker_env_args(extra_docker_arguments)
+
             extra_docker_arguments = [extra_docker_arguments] \
                 if isinstance(extra_docker_arguments, six.string_types) else extra_docker_arguments
             base_cmd += [str(a) for a in extra_docker_arguments if a]
 
         # set docker labels
         base_cmd += ['-l', self._worker_label.format(worker_id)]
         base_cmd += ['-l', self._parent_worker_label.format(parent_worker_id)]
@@ -3957,15 +4036,15 @@
                     host_ssh_cache = new_ssh_cache.replace(k8s_pod_mnt, k8s_node_mnt)
                 except Exception:
                     raise ValueError('Error: could not copy .ssh directory into: {}'.format(new_ssh_cache))
                 self.debug("Copied host SSH cache to: {}, host {}".format(new_ssh_cache, host_ssh_cache), context="docker")
 
         base_cmd += ['-e', 'CLEARML_WORKER_ID='+worker_id, ]
         # update the docker image, so the system knows where it runs
-        base_cmd += ['-e', 'CLEARML_DOCKER_IMAGE={} {}'.format(docker_image, ' '.join(docker_arguments or [])).strip()]
+        base_cmd += ['-e', 'CLEARML_DOCKER_IMAGE={}'.format(docker_image)]
 
         if env_task_id:
             base_cmd += ['-e', 'CLEARML_TASK_ID={}'.format(env_task_id), ]
 
         if auth_token:
             # if auth token is passed then put it in the env var
             base_cmd += ['-e', '{}={}'.format(ENV_AGENT_AUTH_TOKEN.vars[0], auth_token)]
```

## clearml_agent/glue/k8s.py

```diff
@@ -9,53 +9,50 @@
 import re
 import subprocess
 import tempfile
 from collections import defaultdict, namedtuple
 from copy import deepcopy
 from pathlib import Path
 from pprint import pformat
-from threading import Thread
 from time import sleep, time
 from typing import Text, List, Callable, Any, Collection, Optional, Union, Iterable, Dict, Tuple, Set
 
 import yaml
 
 from clearml_agent.backend_api.session import Request
 from clearml_agent.commands.events import Events
 from clearml_agent.commands.worker import Worker, get_task_container, set_task_container, get_next_task
 from clearml_agent.definitions import (
     ENV_DOCKER_IMAGE,
     ENV_AGENT_GIT_USER,
     ENV_AGENT_GIT_PASS,
     ENV_FORCE_SYSTEM_SITE_PACKAGES,
 )
-from clearml_agent.errors import APIError
+from clearml_agent.errors import APIError, UsageError
 from clearml_agent.glue.definitions import ENV_START_AGENT_SCRIPT_PATH
+from clearml_agent.glue.errors import GetPodCountError
+from clearml_agent.glue.utilities import get_path, get_bash_output
+from clearml_agent.glue.pending_pods_daemon import PendingPodsDaemon
 from clearml_agent.helper.base import safe_remove_file
 from clearml_agent.helper.dicts import merge_dicts
 from clearml_agent.helper.process import get_bash_output, stringify_bash_output
 from clearml_agent.helper.resource_monitor import ResourceMonitor
 from clearml_agent.interface.base import ObjectID
 
 
 class K8sIntegration(Worker):
+    SUPPORTED_KIND = ("pod", "job")
     K8S_PENDING_QUEUE = "k8s_scheduler"
 
     K8S_DEFAULT_NAMESPACE = "clearml"
     AGENT_LABEL = "CLEARML=agent"
     QUEUE_LABEL = "clearml-agent-queue"
 
     KUBECTL_APPLY_CMD = "kubectl apply --namespace={namespace} -f"
 
-    KUBECTL_CLEANUP_DELETE_CMD = "kubectl delete pods " \
-                                 "-l={agent_label} " \
-                                 "--field-selector=status.phase!=Pending,status.phase!=Running " \
-                                 "--namespace={namespace} " \
-                                 "--output name"
-
     BASH_INSTALL_SSH_CMD = [
         "apt-get update",
         "apt-get install -y openssh-server",
         "mkdir -p /var/run/sshd",
         "echo 'root:training' | chpasswd",
         "echo 'PermitRootLogin yes' >> /etc/ssh/sshd_config",
         "sed -i 's/PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config",
@@ -78,15 +75,15 @@
         "apt-get install -y git libsm6 libxext6 libxrender-dev libglib2.0-0",
         "declare LOCAL_PYTHON",
         "[ ! -z $LOCAL_PYTHON ] || for i in {{15..5}}; do which python3.$i && python3.$i -m pip --version && "
         "export LOCAL_PYTHON=$(which python3.$i) && break ; done",
         "[ ! -z $LOCAL_PYTHON ] || apt-get install -y python3-pip",
         "[ ! -z $LOCAL_PYTHON ] || export LOCAL_PYTHON=python3",
         "{extra_bash_init_cmd}",
-        "$LOCAL_PYTHON -m pip install clearml-agent{agent_install_args}",
+        "[ ! -z $CLEARML_AGENT_NO_UPDATE ] || $LOCAL_PYTHON -m pip install clearml-agent{agent_install_args}",
         "{extra_docker_bash_script}",
         "$LOCAL_PYTHON -m clearml_agent execute {default_execution_agent_args} --id {task_id}"
     ]
 
     DEFAULT_POD_NAME_PREFIX = "clearml-id-"
     DEFAULT_LIMIT_POD_LABEL = "ai.allegro.agent.serial=pod-{pod_number}"
 
@@ -132,14 +129,18 @@
             If provided the pod is scheduled with kubectl apply and overrides are ignored, otherwise with kubectl run.
         :param str clearml_conf_file: clearml.conf file to be use by the pod itself (optional)
         :param str extra_bash_init_script: Additional bash script to run before starting the Task inside the container
         :param str namespace: K8S namespace to be used when creating the new pods (default: clearml)
         :param int max_pods_limit: Maximum number of pods that K8S glue can run at the same time
         """
         super(K8sIntegration, self).__init__()
+        self.kind = os.environ.get("CLEARML_K8S_GLUE_KIND", "pod").strip().lower()
+        if self.kind not in self.SUPPORTED_KIND:
+            raise UsageError(f"Kind '{self.kind}' not supported (expected {','.join(self.SUPPORTED_KIND)})")
+        self.using_jobs = self.kind == "job"
         self.pod_name_prefix = pod_name_prefix or self.DEFAULT_POD_NAME_PREFIX
         self.limit_pod_label = limit_pod_label or self.DEFAULT_LIMIT_POD_LABEL
         self.k8s_pending_queue_name = k8s_pending_queue_name or self.K8S_PENDING_QUEUE
         self.k8s_pending_queue_id = None
         self.container_bash_script = container_bash_script or self.CONTAINER_BASH_SCRIPT
         force_system_packages = ENV_FORCE_SYSTEM_SITE_PACKAGES.get()
         self._force_system_site_packages = force_system_packages if force_system_packages is not None else True
@@ -176,19 +177,26 @@
 
         if clearml_conf_file:
             with open(os.path.expandvars(os.path.expanduser(str(clearml_conf_file))), 'rt') as f:
                 self.conf_file_content = f.read()
 
         self._agent_label = None
 
-        self._monitor_hanging_pods()
+        self._pending_pods_daemon = self._create_pending_pods_daemon(
+            cls_=PendingPodsDaemon,
+            polling_interval=self._polling_interval
+        )
+        self._pending_pods_daemon.start()
 
         self._min_cleanup_interval_per_ns_sec = 1.0
         self._last_pod_cleanup_per_ns = defaultdict(lambda: 0.)
 
+    def _create_pending_pods_daemon(self, cls_, **kwargs):
+        return cls_(agent=self, **kwargs)
+
     def _load_overrides_yaml(self, overrides_yaml):
         if not overrides_yaml:
             return
         overrides = self._load_template_file(overrides_yaml)
         if not overrides:
             return
         containers = overrides.get('spec', {}).get('containers', [])
@@ -206,170 +214,51 @@
         if self.pod_limits or self.pod_requests:
             self.log.warning('Found pod container requests={} limits={}'.format(
                 self.pod_limits, self.pod_requests))
         if containers:
             self.log.warning('Removing containers section: {}'.format(overrides['spec'].pop('containers')))
         self.overrides_json_string = json.dumps(overrides)
 
-    def _monitor_hanging_pods(self):
-        _check_pod_thread = Thread(target=self._monitor_hanging_pods_daemon)
-        _check_pod_thread.daemon = True
-        _check_pod_thread.start()
-
     @staticmethod
     def _load_template_file(path):
         with open(os.path.expandvars(os.path.expanduser(str(path))), 'rt') as f:
             return yaml.load(f, Loader=getattr(yaml, 'FullLoader', None))
 
-    def _get_kubectl_options(self, command, extra_labels=None, filters=None, output="json", labels=None):
-        # type: (str, Iterable[str], Iterable[str], str, Iterable[str]) -> Dict
-        if not labels:
+    @staticmethod
+    def _get_path(d, *path, default=None):
+        try:
+            return functools.reduce(
+                lambda a, b: a[b], path, d
+            )
+        except (IndexError, KeyError):
+            return default
+
+    def _get_kubectl_options(self, command, extra_labels=None, filters=None, output="json", labels=None, ns=None):
+        # type: (str, Iterable[str], Iterable[str], str, Iterable[str], str) -> Dict
+        if labels is False:
+            labels = []
+        elif not labels:
             labels = [self._get_agent_label()]
         labels = list(labels) + (list(extra_labels) if extra_labels else [])
         d = {
-            "-l": ",".join(labels),
-            "-n": str(self.namespace),
+            "-n": ns or str(self.namespace),
             "-o": output,
         }
+        if labels:
+            d["-l"] = ",".join(labels)
         if filters:
             d["--field-selector"] = ",".join(filters)
         return d
 
     def get_kubectl_command(self, command, output="json", **args):
         opts = self._get_kubectl_options(command, output=output, **args)
         return 'kubectl {command} {opts}'.format(
             command=command, opts=" ".join(x for item in opts.items() for x in item)
         )
 
-    def _monitor_hanging_pods_daemon(self):
-        last_tasks_msgs = {}  # last msg updated for every task
-
-        while True:
-            kubectl_cmd = self.get_kubectl_command("get pods", filters=["status.phase=Pending"])
-            self.log.debug("Detecting hanging pods: {}".format(kubectl_cmd))
-            output = stringify_bash_output(get_bash_output(kubectl_cmd))
-            try:
-                output_config = json.loads(output)
-            except Exception as ex:
-                self.log.warning('K8S Glue pods monitor: Failed parsing kubectl output:\n{}\nEx: {}'.format(output, ex))
-                sleep(self._polling_interval)
-                continue
-            pods = output_config.get('items', [])
-            task_id_to_details = dict()
-            for pod in pods:
-                pod_name = pod.get('metadata', {}).get('name', None)
-                if not pod_name:
-                    continue
-
-                task_id = pod_name.rpartition('-')[-1]
-                if not task_id:
-                    continue
-
-                namespace = pod.get('metadata', {}).get('namespace', None)
-                if not namespace:
-                    continue
-
-                task_id_to_details[task_id] = (pod_name, namespace)
-
-                msg = None
-
-                waiting = self._get_path(pod, 'status', 'containerStatuses', 0, 'state', 'waiting')
-                if not waiting:
-                    condition = self._get_path(pod, 'status', 'conditions', 0)
-                    if condition:
-                        reason = condition.get('reason')
-                        if reason == 'Unschedulable':
-                            message = condition.get('message')
-                            msg = reason + (" ({})".format(message) if message else "")
-                else:
-                    reason = waiting.get("reason", None)
-                    message = waiting.get("message", None)
-
-                    msg = reason + (" ({})".format(message) if message else "")
-
-                    if reason == 'ImagePullBackOff':
-                        delete_pod_cmd = 'kubectl delete pods {} -n {}'.format(pod_name, namespace)
-                        self.log.debug(" - deleting pod due to ImagePullBackOff: {}".format(delete_pod_cmd))
-                        get_bash_output(delete_pod_cmd)
-                        try:
-                            self.log.debug(" - Detecting hanging pods: {}".format(kubectl_cmd))
-                            self._session.api_client.tasks.failed(
-                                task=task_id,
-                                status_reason="K8S glue error: {}".format(msg),
-                                status_message="Changed by K8S glue",
-                                force=True
-                            )
-                        except Exception as ex:
-                            self.log.warning(
-                                'K8S Glue pods monitor: Failed deleting task "{}"\nEX: {}'.format(task_id, ex)
-                            )
-
-                        # clean up any msg for this task
-                        last_tasks_msgs.pop(task_id, None)
-                        continue
-                if msg and last_tasks_msgs.get(task_id, None) != msg:
-                    try:
-                        result = self._session.send_request(
-                            service='tasks',
-                            action='update',
-                            json={"task": task_id, "status_message": "K8S glue status: {}".format(msg)},
-                            method=Request.def_method,
-                            async_enable=False,
-                        )
-                        if not result.ok:
-                            result_msg = self._get_path(result.json(), 'meta', 'result_msg')
-                            raise Exception(result_msg or result.text)
-
-                        # update last msg for this task
-                        last_tasks_msgs[task_id] = msg
-                    except Exception as ex:
-                        self.log.warning(
-                            'K8S Glue pods monitor: Failed setting status message for task "{}"\nMSG: {}\nEX: {}'.format(
-                                task_id, msg, ex
-                            )
-                        )
-
-            if task_id_to_details:
-                try:
-                    result = self._session.get(
-                        service='tasks',
-                        action='get_all',
-                        json={"id": list(task_id_to_details), "status": ["stopped"], "only_fields": ["id"]},
-                        method=Request.def_method,
-                        async_enable=False,
-                    )
-                    aborted_task_ids = list(filter(None, (task.get("id") for task in result["tasks"])))
-
-                    for task_id in aborted_task_ids:
-                        pod_name, namespace = task_id_to_details.get(task_id)
-                        if not pod_name:
-                            self.log.error("Failed locating aborted task {} in pending pods list".format(task_id))
-                            continue
-                        self.log.info(
-                            "K8S Glue pods monitor: task {} was aborted by its pod {} is still pending, "
-                            "deleting pod".format(task_id, pod_name)
-                        )
-
-                        kubectl_cmd = "kubectl delete pod {pod_name} --output name {namespace}".format(
-                            namespace=f"--namespace={namespace}" if namespace else "", pod_name=pod_name,
-                        ).strip()
-                        self.log.debug("Deleting aborted task pending pod: {}".format(kubectl_cmd))
-                        output = stringify_bash_output(get_bash_output(kubectl_cmd))
-                        if not output:
-                            self.log.warning("K8S Glue pods monitor: failed deleting pod {}".format(pod_name))
-                except Exception as ex:
-                    self.log.warning(
-                        'K8S Glue pods monitor: failed checking aborted tasks for hanging pods: {}'.format(ex)
-                    )
-
-            # clean up any last message for a task that wasn't seen as a pod
-            last_tasks_msgs = {k: v for k, v in last_tasks_msgs.items() if k in task_id_to_details}
-
-            sleep(self._polling_interval)
-
     def _set_task_user_properties(self, task_id: str, task_session=None, **properties: str):
         session = task_session or self._session
         if self._edit_hyperparams_support is not True:
             # either not supported or never tested
             if self._edit_hyperparams_support == self._session.api_version:
                 # tested against latest api_version, not supported
                 return
@@ -461,25 +350,94 @@
         try:
             tenant = self._session.get_decoded_token(self._session.token, verify=False)["tenant"]
             task_tenant = task_session.get_decoded_token(task_session.token, verify=False)["tenant"]
             return tenant == task_tenant
         except Exception as ex:
             print("ERROR: Failed getting tenant for task session: {}".format(ex))
 
+    def get_jobs_info(self, info_path: str, condition: str = None, namespace=None, debug_msg: str = None)\
+            -> Dict[str, str]:
+        cond = "==".join((x.strip("=") for x in condition.partition("=")[::2]))
+        output = f"jsonpath='{{range .items[?(@.{cond})]}}{{@.{info_path}}}{{\" \"}}{{@.metadata.namespace}}{{\"\\n\"}}{{end}}'"
+        kubectl_cmd = self.get_kubectl_command("get job", output=output, ns=namespace)
+        if debug_msg:
+            self.log.debug(debug_msg.format(cmd=kubectl_cmd))
+        output = stringify_bash_output(get_bash_output(kubectl_cmd))
+        output = output.strip("'")  # for Windows debugging :(
+        try:
+            data_items = dict(l.strip().partition(" ")[::2] for l in output.splitlines())
+            return data_items
+        except Exception as ex:
+            self.log.warning('Failed parsing kubectl output:\n{}\nEx: {}'.format(output, ex))
+
+    def get_pods_for_jobs(self, job_condition: str = None, pod_filters: List[str] = None, debug_msg: str = None):
+        controller_uids = self.get_jobs_info(
+            "spec.selector.matchLabels.controller-uid", condition=job_condition, debug_msg=debug_msg
+        )
+        if not controller_uids:
+            # No pods were found for these jobs
+            return []
+        pods = self.get_pods(filters=pod_filters, debug_msg=debug_msg)
+        return [
+            pod for pod in pods
+            if get_path(pod, "metadata", "labels", "controller-uid") in controller_uids
+        ]
+
+    def get_pods(self, filters: List[str] = None, debug_msg: str = None):
+        kubectl_cmd = self.get_kubectl_command(
+            "get pods",
+            filters=filters,
+            labels=False if self.using_jobs else None,
+        )
+        if debug_msg:
+            self.log.debug(debug_msg.format(cmd=kubectl_cmd))
+        output = stringify_bash_output(get_bash_output(kubectl_cmd))
+        try:
+            output_config = json.loads(output)
+        except Exception as ex:
+            self.log.warning('Failed parsing kubectl output:\n{}\nEx: {}'.format(output, ex))
+            return
+        return output_config.get('items', [])
+
+    def _get_pod_count(self, extra_labels: List[str] = None, msg: str = None):
+            kubectl_cmd_new = self.get_kubectl_command(
+                f"get {self.kind}s",
+                extra_labels= extra_labels
+            )
+            self.log.debug("{}{}".format((msg + ": ") if msg else "", kubectl_cmd_new))
+            process = subprocess.Popen(kubectl_cmd_new.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+            output, error = process.communicate()
+            output = stringify_bash_output(output)
+            error = stringify_bash_output(error)
+
+            try:
+                return len(json.loads(output).get("items", []))
+            except (ValueError, TypeError) as ex:
+                self.log.warning(
+                    "K8S Glue pods monitor: Failed parsing kubectl output:\n{}\nEx: {}".format(output, ex)
+                )
+                raise GetPodCountError()
+
     def run_one_task(self, queue: Text, task_id: Text, worker_args=None, task_session=None, **_):
         print('Pulling task {} launching on kubernetes cluster'.format(task_id))
         session = task_session or self._session
         task_data = session.api_client.tasks.get_all(id=[task_id])[0]
 
         # push task into the k8s queue, so we have visibility on pending tasks in the k8s scheduler
         if self._is_same_tenant(task_session):
             try:
                 print('Pushing task {} into temporary pending queue'.format(task_id))
                 _ = session.api_client.tasks.stop(task_id, force=True)
 
+                # Just make sure to clean up in case the task is stuck in the queue (known issue)
+                self._session.api_client.queues.remove_task(
+                    task=task_id,
+                    queue=self.k8s_pending_queue_id,
+                )
+
                 res = self._session.api_client.tasks.enqueue(
                     task_id,
                     queue=self.k8s_pending_queue_id,
                     status_reason='k8s pending scheduler',
                 )
                 if res.meta.result_code != 200:
                     raise Exception(res.meta.result_msg)
@@ -511,22 +469,22 @@
         # noinspection PyProtectedMember
         config_content = (
             self.conf_file_content or (session._config_file and Path(session._config_file).read_text()) or ""
         ) + '\n{}\n'.format('\n'.join(x for x in extra_config_values if x))
 
         hocon_config_encoded = config_content.encode("ascii")
 
-        create_clearml_conf = ["echo '{}' | base64 --decode >> ~/clearml.conf".format(
+        clearml_conf_create_script = ["echo '{}' | base64 --decode >> ~/clearml.conf".format(
             base64.b64encode(
                 hocon_config_encoded
             ).decode('ascii')
         )]
 
         if task_session:
-            create_clearml_conf.append(
+            clearml_conf_create_script.append(
                 "export CLEARML_AUTH_TOKEN=$(echo '{}' | base64 --decode)".format(
                     base64.b64encode(task_session.token.encode("ascii")).decode('ascii')
                 )
             )
 
         if self.ports_mode:
             print("Kubernetes looking for available pod to use")
@@ -539,31 +497,23 @@
 
         # Search for a free pod number
         pod_count = 0
         pod_number = self.base_pod_num
         while self.ports_mode or self.max_pods_limit:
             pod_number = self.base_pod_num + pod_count
 
-            kubectl_cmd_new = self.get_kubectl_command(
-                "get pods",
-                extra_labels=[self.limit_pod_label.format(pod_number=pod_number)] if self.ports_mode else None
-            )
-            self.log.debug("Looking for a free pod/port: {}".format(kubectl_cmd_new))
-            process = subprocess.Popen(kubectl_cmd_new.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            output, error = process.communicate()
-            output = stringify_bash_output(output)
-            error = stringify_bash_output(error)
-
             try:
-                items_count = len(json.loads(output).get("items", []))
-            except (ValueError, TypeError) as ex:
+                items_count = self._get_pod_count(
+                    extra_labels=[self.limit_pod_label.format(pod_number=pod_number)] if self.ports_mode else None,
+                    msg="Looking for a free pod/port"
+                )
+            except GetPodCountError:
                 self.log.warning(
-                    "K8S Glue pods monitor: Failed parsing kubectl output:\n{}\ntask '{}' "
-                    "will be enqueued back to queue '{}'\nEx: {}".format(
-                        output, task_id, queue, ex
+                    "K8S Glue pods monitor: task '{}' will be enqueued back to queue '{}'".format(
+                        task_id, queue
                     )
                 )
                 session.api_client.tasks.stop(task_id, force=True)
                 # noinspection PyBroadException
                 try:
                     self._session.api_client.tasks.enqueue(task_id, queue=queue, status_reason='kubectl parsing error')
                 except:
@@ -579,16 +529,14 @@
                 max_count = self.max_pods_limit
             else:
                 current_pod_count = pod_count
                 max_count = self.num_of_services - 1
 
             if current_pod_count >= max_count:
                 # All pods are taken, exit
-                self.log.debug(
-                    "kubectl last result: {}\n{}".format(error, output))
                 self.log.warning(
                     "All k8s services are in use, task '{}' "
                     "will be enqueued back to queue '{}'".format(
                         task_id, queue
                     )
                 )
                 session.api_client.tasks.stop(task_id, force=True)
@@ -625,29 +573,29 @@
         except (KeyError, TypeError, AttributeError):
             namespace = self.namespace
 
         if template:
             output, error = self._kubectl_apply(
                 template=template,
                 pod_number=pod_number,
-                create_clearml_conf=create_clearml_conf,
+                clearml_conf_create_script=clearml_conf_create_script,
                 labels=labels,
                 docker_image=container['image'],
                 docker_args=container['arguments'],
                 docker_bash=container.get('setup_shell_script'),
                 task_id=task_id,
                 queue=queue,
                 namespace=namespace,
             )
 
-        print('kubectl output:\n{}\n{}'.format(error, output))
-        if error:
-            send_log = "Running kubectl encountered an error: {}".format(error)
-            self.log.error(send_log)
-            self.send_logs(task_id, send_log.splitlines())
+            print('kubectl output:\n{}\n{}'.format(error, output))
+            if error:
+                send_log = "Running kubectl encountered an error: {}".format(error)
+                self.log.error(send_log)
+                self.send_logs(task_id, send_log.splitlines())
 
         user_props = {"k8s-queue": str(queue_name)}
         if self.ports_mode:
             user_props.update(
                 {
                     "k8s-pod-number": pod_number,
                     "k8s-pod-label": labels[0],
@@ -700,40 +648,18 @@
                 results.append(env)
             else:
                 self.log.warning('skipping docker argument {} (only -e --env supported)'.format(cmd))
         if target:
             return {target: results} if results else {}
         return results
 
-    def _kubectl_apply(
-        self,
-        create_clearml_conf,
-        docker_image,
-        docker_args,
-        docker_bash,
-        labels,
-        queue,
-        task_id,
-        namespace,
-        template=None,
-        pod_number=None
-    ):
-        template.setdefault('apiVersion', 'v1')
-        template['kind'] = 'Pod'
-        template.setdefault('metadata', {})
-        name = self.pod_name_prefix + str(task_id)
-        template['metadata']['name'] = name
-        template.setdefault('spec', {})
-        template['spec'].setdefault('containers', [])
-        template['spec'].setdefault('restartPolicy', 'Never')
-        if labels:
-            labels_dict = dict(pair.split('=', 1) for pair in labels)
-            template['metadata'].setdefault('labels', {})
-            template['metadata']['labels'].update(labels_dict)
-
+    def _create_template_container(
+        self, pod_name: str, task_id: str, docker_image: str, docker_args: List[str],
+        docker_bash: str, clearml_conf_create_script: List[str]
+    ) -> dict:
         container = self._get_docker_args(
             docker_args,
             target="env",
             flags={"-e", "--env"},
             convert=lambda env: {'name': env.partition("=")[0], 'value': env.partition("=")[2]},
         )
 
@@ -749,42 +675,99 @@
             [line.format(extra_bash_init_cmd=self.extra_bash_init_script or '',
                          task_id=task_id,
                          extra_docker_bash_script=extra_docker_bash_script,
                          default_execution_agent_args=self.DEFAULT_EXECUTION_AGENT_ARGS,
                          agent_install_args=self.POD_AGENT_INSTALL_ARGS)
              for line in container_bash_script])
 
-        extra_bash_commands = list(create_clearml_conf or [])
+        extra_bash_commands = list(clearml_conf_create_script or [])
 
         start_agent_script_path = ENV_START_AGENT_SCRIPT_PATH.get() or "~/__start_agent__.sh"
 
         extra_bash_commands.append(
             "echo '{content}' | base64 --decode >> {script_path} ; /bin/bash {script_path}".format(
                 content=base64.b64encode(
                     script_encoded.encode('ascii')
                 ).decode('ascii'),
                 script_path=start_agent_script_path
             )
         )
 
         # Notice: we always leave with exit code 0, so pods are never restarted
-        container = self._merge_containers(
+        return self._merge_containers(
             container,
-            dict(name=name, image=docker_image,
+            dict(name=pod_name, image=docker_image,
                  command=['/bin/bash'],
                  args=['-c', '{} ; exit 0'.format(' ; '.join(extra_bash_commands))])
         )
 
-        if template['spec']['containers']:
-            template['spec']['containers'][0] = self._merge_containers(template['spec']['containers'][0], container)
+    def _kubectl_apply(
+        self,
+        clearml_conf_create_script: List[str],
+        docker_image,
+        docker_args,
+        docker_bash,
+        labels,
+        queue,
+        task_id,
+        namespace,
+        template=None,
+        pod_number=None
+    ):
+        if "apiVersion" not in template:
+            template["apiVersion"] = "batch/v1" if self.using_jobs else "v1"
+        if "kind" in template:
+            if template["kind"].lower() != self.kind:
+                return (
+                    "", f"Template kind {template['kind']} does not maych kind {self.kind.capitalize()} set for agent"
+                )
         else:
-            template['spec']['containers'].append(container)
+            template["kind"] = self.kind.capitalize()
+
+        metadata = template.setdefault('metadata', {})
+        name = self.pod_name_prefix + str(task_id)
+        metadata['name'] = name
+
+        def place_labels(metadata_dict):
+            labels_dict = dict(pair.split('=', 1) for pair in labels)
+            metadata_dict.setdefault('labels', {}).update(labels_dict)
+
+        if labels:
+            # Place labels on base resource (job or single pod)
+            place_labels(metadata)
+
+        spec = template.setdefault('spec', {})
+        if self.using_jobs:
+            spec.setdefault('backoffLimit', 0)
+            spec_template = spec.setdefault('template', {})
+            if labels:
+                # Place same labels fro any pod spawned by the job
+                place_labels(spec_template.setdefault('metadata', {}))
+
+            spec = spec_template.setdefault('spec', {})
+
+        containers = spec.setdefault('containers', [])
+        spec.setdefault('restartPolicy', 'Never')
+
+        container = self._create_template_container(
+            pod_name=name,
+            task_id=task_id,
+            docker_image=docker_image,
+            docker_args=docker_args,
+            docker_bash=docker_bash,
+            clearml_conf_create_script=clearml_conf_create_script
+        )
+
+        if containers:
+            containers[0] = self._merge_containers(containers[0], container)
+        else:
+            containers.append(container)
 
         if self._docker_force_pull:
-            for c in template['spec']['containers']:
+            for c in containers:
                 c.setdefault('imagePullPolicy', 'Always')
 
         fp, yaml_file = tempfile.mkstemp(prefix='clearml_k8stmpl_', suffix='.yml')
         os.close(fp)
         with open(yaml_file, 'wt') as f:
             yaml.dump(template, f)
 
@@ -808,39 +791,105 @@
         except Exception as ex:
             return None, str(ex)
         finally:
             safe_remove_file(yaml_file)
 
         return stringify_bash_output(output), stringify_bash_output(error)
 
+    def _process_bash_lines_response(self, bash_cmd: str, raise_error=True):
+        res = get_bash_output(bash_cmd, raise_error=raise_error)
+        lines = [
+            line for line in
+            (r.strip().rpartition("/")[-1] for r in res.splitlines())
+            if line.startswith(self.pod_name_prefix)
+        ]
+        return lines
+
+    def _delete_pods(self, selectors: List[str], namespace: str, msg: str = None) -> List[str]:
+        kubectl_cmd = \
+            "kubectl delete pod -l={agent_label} " \
+            "--namespace={namespace} --field-selector={selector} --output name".format(
+                selector=",".join(selectors),
+                agent_label=self._get_agent_label(),
+                namespace=namespace,
+            )
+        self.log.debug("Deleting old/failed pods{} for ns {}: {}".format(
+            msg or "", namespace, kubectl_cmd
+        ))
+        lines = self._process_bash_lines_response(kubectl_cmd)
+        self.log.debug(" - deleted pods %s", ", ".join(lines))
+        return lines
+
+    def _delete_jobs_by_names(self, names_to_ns: Dict[str, str], msg: str = None) -> List[str]:
+        if not names_to_ns:
+            return []
+        ns_to_names = defaultdict(list)
+        for name, ns in names_to_ns.items():
+            ns_to_names[ns].append(name)
+
+        results = []
+        for ns, names in ns_to_names.items():
+            kubectl_cmd = "kubectl delete job --namespace={ns} --output=name {names}".format(
+                ns=ns, names=" ".join(names)
+            )
+            self.log.debug("Deleting jobs {}: {}".format(
+                msg or "", kubectl_cmd
+            ))
+            lines = self._process_bash_lines_response(kubectl_cmd)
+            if not lines:
+                continue
+            self.log.debug(" - deleted jobs %s", ", ".join(lines))
+            results.extend(lines)
+        return results
+
+    def _delete_completed_or_failed_pods(self, namespace, msg: str = None):
+        if not self.using_jobs:
+            return self._delete_pods(
+                selectors=["status.phase!=Pending", "status.phase!=Running"], namespace=namespace, msg=msg
+            )
+
+        job_names_to_delete = {}
+
+        # locate failed pods for jobs
+        failed_pods = self.get_pods_for_jobs(
+            job_condition="status.active=1",
+            pod_filters=["status.phase!=Pending", "status.phase!=Running", "status.phase!=Terminating"],
+            debug_msg="Deleting failed pods: {cmd}"
+        )
+        if failed_pods:
+            job_names_to_delete = {
+                get_path(pod, "metadata", "labels", "job-name"): get_path(pod, "metadata", "namespace")
+                for pod in failed_pods
+                if get_path(pod, "metadata", "labels", "job-name")
+            }
+            self.log.debug(f" - found jobs with failed pods: {' '.join(job_names_to_delete)}")
+
+        completed_job_names = self.get_jobs_info(
+            "metadata.name", condition="status.succeeded=1", namespace=namespace, debug_msg=msg
+        )
+        if completed_job_names:
+            self.log.debug(f" - found completed jobs: {' '.join(completed_job_names)}")
+            job_names_to_delete.update(completed_job_names)
+
+        return self._delete_jobs_by_names(names_to_ns=job_names_to_delete, msg=msg)
+
     def _cleanup_old_pods(self, namespaces, extra_msg=None):
         # type: (Iterable[str], Optional[str]) -> Dict[str, List[str]]
         self.log.debug("Cleaning up pods")
         deleted_pods = defaultdict(list)
         for namespace in namespaces:
             if time() - self._last_pod_cleanup_per_ns[namespace] < self._min_cleanup_interval_per_ns_sec:
                 # Do not try to cleanup the same namespace too quickly
                 continue
-            kubectl_cmd = self.KUBECTL_CLEANUP_DELETE_CMD.format(
-                namespace=namespace, agent_label=self._get_agent_label()
-            )
-            self.log.debug("Deleting old/failed pods{} for ns {}: {}".format(
-                extra_msg or "", namespace, kubectl_cmd
-            ))
+
             try:
-                res = get_bash_output(kubectl_cmd, raise_error=True)
-                lines = [
-                    line for line in
-                    (r.strip().rpartition("/")[-1] for r in res.splitlines())
-                    if line.startswith(self.pod_name_prefix)
-                ]
-                self.log.debug(" - deleted pod(s) %s", ", ".join(lines))
-                deleted_pods[namespace].extend(lines)
+                res = self._delete_completed_or_failed_pods(namespace, extra_msg)
+                deleted_pods[namespace].extend(res)
             except Exception as ex:
-                self.log.error("Failed deleting old/failed pods for ns %s: %s", namespace, str(ex))
+                self.log.error("Failed deleting completed/failed pods for ns %s: %s", namespace, str(ex))
             finally:
                 self._last_pod_cleanup_per_ns[namespace] = time()
 
         # Locate tasks belonging to deleted pods that are still marked as pending or running
         tasks_to_abort = []
         try:
             task_ids = list(filter(None, (
@@ -853,36 +902,48 @@
                     service='tasks',
                     action='get_all',
                     json={"id": task_ids, "status": ["in_progress", "queued"], "only_fields": ["id", "status"]},
                     method=Request.def_method,
                 )
                 tasks_to_abort = result["tasks"]
         except Exception as ex:
-            self.log.warning('Failed getting running tasks for deleted pods: {}'.format(ex))
+            self.log.warning('Failed getting running tasks for deleted {}(s): {}'.format(self.kind, ex))
 
         for task in tasks_to_abort:
             task_id = task.get("id")
             status = task.get("status")
             if not task_id or not status:
                 self.log.warning('Failed getting task information: id={}, status={}'.format(task_id, status))
                 continue
             try:
                 if status == "queued":
                     self._session.get(
                         service='tasks',
                         action='dequeue',
-                        json={"task": task_id, "force": True, "status_reason": "Pod deleted (not pending or running)",
-                              "status_message": "Pod deleted by agent {}".format(self.worker_id or "unknown")},
+                        json={
+                            "task": task_id,
+                            "force": True,
+                            "status_reason": "Pod deleted (not pending or running)",
+                            "status_message": "{} deleted by agent {}".format(
+                                self.kind.capitalize(), self.worker_id or "unknown"
+                            )
+                        },
                         method=Request.def_method,
                     )
                 self._session.get(
                     service='tasks',
                     action='failed',
-                    json={"task": task_id, "force": True, "status_reason": "Pod deleted (not pending or running)",
-                          "status_message": "Pod deleted by agent {}".format(self.worker_id or "unknown")},
+                    json={
+                        "task": task_id,
+                        "force": True,
+                        "status_reason": "Pod deleted (not pending or running)",
+                        "status_message": "{} deleted by agent {}".format(
+                            self.kind.capitalize(), self.worker_id or "unknown"
+                        )
+                    },
                     method=Request.def_method,
                 )
             except Exception as ex:
                 self.log.warning('Failed setting task {} to status "failed": {}'.format(task_id, ex))
 
         return deleted_pods
 
@@ -915,26 +976,26 @@
 
             # just in case there are no pods, make sure we look at our base namespace
             namespaces.add(self.namespace)
 
             # check if have pod limit, then check if we hit it.
             if self.max_pods_limit:
                 if current_pods >= self.max_pods_limit:
-                    print("Maximum pod limit reached {}/{}, sleeping for {:.1f} seconds".format(
-                        current_pods, self.max_pods_limit, self._polling_interval))
+                    print("Maximum {} limit reached {}/{}, sleeping for {:.1f} seconds".format(
+                        self.kind, current_pods, self.max_pods_limit, self._polling_interval))
                     # delete old completed / failed pods
-                    self._cleanup_old_pods(namespaces, " due to pod limit")
+                    self._cleanup_old_pods(namespaces, f" due to {self.kind} limit")
                     # go to sleep
                     sleep(self._polling_interval)
                     continue
 
             # iterate over queues (priority style, queues[0] is highest)
             for queue in queues:
                 # delete old completed / failed pods
-                self._cleanup_old_pods(namespaces)
+                self._cleanup_old_pods(namespaces, extra_msg="Cleanup cycle {cmd}")
 
                 # get next task in queue
                 try:
                     response = self._get_next_task(queue=queue, get_task_info=self._impersonate_as_task_owner)
                 except Exception as e:
                     print("Warning: Could not access task queue [{}], error: {}".format(queue, e))
                     continue
```

## clearml_agent/helper/base.py

```diff
@@ -16,28 +16,30 @@
 from collections import OrderedDict
 from distutils.spawn import find_executable
 from functools import total_ordering
 from typing import Text, Dict, Any, Optional, AnyStr, IO, Union
 
 import attr
 import furl
+import six
 import yaml
 from attr import fields_dict
 from pathlib2 import Path
-
-import six
 from six.moves import reduce
-from clearml_agent.external import pyhocon
+
 from clearml_agent.errors import CommandFailedError
+from clearml_agent.external import pyhocon
 from clearml_agent.helper.dicts import filter_keys
 
 pretty_lines = False
 
 log = logging.getLogger(__name__)
 
+use_powershell = os.getenv("CLEARML_AGENT_USE_POWERSHELL", None)
+
 
 def which(cmd, path=None):
     result = find_executable(cmd, path)
     if not result:
         raise ValueError('command "{}" not found'.format(cmd))
     return result
 
@@ -48,15 +50,15 @@
     :param linux: value to return if OS is linux
     :param windows: value to return if OS is Windows
     """
     return windows if is_windows_platform() else linux
 
 
 def bash_c():
-    return 'bash -c' if not is_windows_platform() else 'cmd /c'
+    return 'bash -c' if not is_windows_platform() else ('powershell -Command' if use_powershell else 'cmd /c')
 
 
 def return_list(arg):
     if arg and not isinstance(arg, (tuple, list)):
         return [arg]
 
     return arg
```

## clearml_agent/helper/package/base.py

```diff
@@ -46,15 +46,15 @@
         pass
 
     @abc.abstractmethod
     def install_from_file(self, path):
         pass
 
     @abc.abstractmethod
-    def freeze(self):
+    def freeze(self, freeze_full_environment=False):
         pass
 
     @abc.abstractmethod
     def load_requirements(self, requirements):
         pass
 
     @abc.abstractmethod
@@ -137,27 +137,29 @@
     @cwd.setter
     def cwd(self, value):
         self._cwd = value
 
     @classmethod
     def out_of_scope_install_package(cls, package_name, *args):
         if PackageManager._selected_manager is not None:
+            # noinspection PyBroadException
             try:
-                result = PackageManager._selected_manager._install(package_name, *args)
+                result = PackageManager._selected_manager.install_packages(package_name, *args)
                 if result not in (0, None, True):
                     return False
             except Exception:
                 return False
         return True
 
     @classmethod
-    def out_of_scope_freeze(cls):
+    def out_of_scope_freeze(cls, freeze_full_environment=False):
         if PackageManager._selected_manager is not None:
+            # noinspection PyBroadException
             try:
-                return PackageManager._selected_manager.freeze()
+                return PackageManager._selected_manager.freeze(freeze_full_environment)
             except Exception:
                 pass
         return []
 
     @classmethod
     def set_pip_version(cls, version):
         if not version:
```

## clearml_agent/helper/package/poetry_api.py

```diff
@@ -143,15 +143,15 @@
 
     @property
     def enabled(self):
         return self.config.enabled and (
             any((self.path / indicator).exists() for indicator in self.INDICATOR_FILES)
         )
 
-    def freeze(self):
+    def freeze(self, freeze_full_environment=False):
         lines = self.config.run("show", cwd=str(self.path)).splitlines()
         lines = [[p for p in line.split(' ') if p] for line in lines]
         return {"pip": [parts[0]+'=='+parts[1]+' # '+' '.join(parts[2:]) for parts in lines]}
 
     def get_python_command(self, extra):
         if check_if_command_exists("poetry"):
             return Argv("poetry", "run", "python", *extra)
```

## clearml_agent/helper/package/priority_req.py

```diff
@@ -3,15 +3,15 @@
 
 from .base import PackageManager
 from .requirements import SimpleSubstitution
 
 
 class PriorityPackageRequirement(SimpleSubstitution):
 
-    name = ("cython", "numpy", "setuptools", )
+    name = ("cython", "numpy", "setuptools", "pip", )
     optional_package_names = tuple()
 
     def __init__(self, *args, **kwargs):
         super(PriorityPackageRequirement, self).__init__(*args, **kwargs)
         self._replaced_packages = {}
         # check if we need to replace the packages:
         priority_packages = self.config.get('agent.package_manager.priority_packages', None)
@@ -46,39 +46,47 @@
     def replace_back(self, list_of_requirements):
         """
         :param list_of_requirements: {'pip': ['a==1.0', ]}
         :return: {'pip': ['a==1.0', ]}
         """
         # if we replaced setuptools, it means someone requested it, and since freeze will not contain it,
         # we need to add it manually
-        if not self._replaced_packages or "setuptools" not in self._replaced_packages:
+        if not self._replaced_packages:
             return list_of_requirements
 
-        try:
-            for k, lines in list_of_requirements.items():
-                # k is either pip/conda
-                if k not in ('pip', 'conda'):
-                    continue
-                for i, line in enumerate(lines):
-                    if not line or line.lstrip().startswith('#'):
-                        continue
-                    parts = [p for p in re.split(r'\s|=|\.|<|>|~|!|@|#', line) if p]
-                    if not parts:
+        if "pip" in self._replaced_packages:
+            full_freeze = PackageManager.out_of_scope_freeze(freeze_full_environment=True)
+            # now let's look for pip
+            pips = [line for line in full_freeze.get("pip", []) if line.split("==")[0] == "pip"]
+            if pips and "pip" in list_of_requirements:
+                list_of_requirements["pip"] = [pips[0]] + list_of_requirements["pip"]
+
+        if "setuptools" in self._replaced_packages:
+            try:
+                for k, lines in list_of_requirements.items():
+                    # k is either pip/conda
+                    if k not in ('pip', 'conda'):
                         continue
-                    # if we found setuptools, do nothing
-                    if parts[0] == "setuptools":
-                        return list_of_requirements
-
-            # if we are here it means we have not found setuptools
-            # we should add it:
-            if "pip" in list_of_requirements:
-                list_of_requirements["pip"] = [self._replaced_packages["setuptools"]] + list_of_requirements["pip"]
+                    for i, line in enumerate(lines):
+                        if not line or line.lstrip().startswith('#'):
+                            continue
+                        parts = [p for p in re.split(r'\s|=|\.|<|>|~|!|@|#', line) if p]
+                        if not parts:
+                            continue
+                        # if we found setuptools, do nothing
+                        if parts[0] == "setuptools":
+                            return list_of_requirements
+
+                # if we are here it means we have not found setuptools
+                # we should add it:
+                if "pip" in list_of_requirements:
+                    list_of_requirements["pip"] = [self._replaced_packages["setuptools"]] + list_of_requirements["pip"]
 
-        except Exception as ex:  # noqa
-            return list_of_requirements
+            except Exception as ex:  # noqa
+                return list_of_requirements
 
         return list_of_requirements
 
 
 class PackageCollectorRequirement(SimpleSubstitution):
     """
     This RequirementSubstitution class will allow you to have multiple instances of the same
```

## clearml_agent/helper/package/pip_api/system.py

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 from itertools import chain
 from pathlib import Path
 from typing import Text, Optional
 
-from clearml_agent.definitions import PIP_EXTRA_INDICES, PROGRAM_NAME
+from clearml_agent.definitions import PIP_EXTRA_INDICES, PROGRAM_NAME, ENV_PIP_EXTRA_INSTALL_FLAGS
 from clearml_agent.helper.package.base import PackageManager
 from clearml_agent.helper.process import Argv, DEVNULL
 from clearml_agent.session import Session
 
 
 class SystemPip(PackageManager):
 
@@ -48,34 +48,35 @@
     def download_package(self, package, cache_dir):
         self.run_with_env(
             (
                 'download',
                 package,
                 '--dest', cache_dir,
                 '--no-deps',
-            ) + self.install_flags()
+            ) + self.download_flags()
         )
 
     def load_requirements(self, requirements):
         requirements = requirements.get('pip') if isinstance(requirements, dict) else requirements
         if not requirements:
             return
         with self.temp_file('cached-reqs', requirements) as path:
             self.install_from_file(path)
 
     def uninstall(self, package):
         self.run_with_env(('uninstall', '-y', package))
 
-    def freeze(self):
+    def freeze(self, freeze_full_environment=False):
         """
         pip freeze to all install packages except the running program
         :return: Dict contains pip as key and pip's packages to install
         :rtype: Dict[str: List[str]]
         """
-        packages = self.run_with_env(('freeze',), output=True).splitlines()
+        packages = self.run_with_env(
+            ('freeze',) if not freeze_full_environment else ('freeze', '--all'), output=True).splitlines()
         packages_without_program = [package for package in packages if PROGRAM_NAME not in package]
         return {'pip': packages_without_program}
 
     def run_with_env(self, command, output=False, **kwargs):
         """
         Run a shell command using environment from a virtualenv script
         :param command: command to run
@@ -83,18 +84,36 @@
         :param output: return output
         :param kwargs: kwargs for get_output/check_output command
         """
         command = self._make_command(command)
         # make sure we are not running it with our own PYTHONPATH
         env = dict(**os.environ)
         env.pop('PYTHONPATH', None)
+
+        # Debug print
+        if self.session.debug_mode:
+            print(command)
+
         return (command.get_output if output else command.check_call)(stdin=DEVNULL, env=env, **kwargs)
 
     def _make_command(self, command):
         return Argv(self.bin, '-m', 'pip', '--disable-pip-version-check', *command)
 
     def install_flags(self):
         if self.indices_args is None:
             self.indices_args = tuple(
                 chain.from_iterable(('--extra-index-url', x) for x in PIP_EXTRA_INDICES)
             )
+
+        extra_pip_flags = \
+            ENV_PIP_EXTRA_INSTALL_FLAGS.get() or \
+            self.session.config.get("agent.package_manager.extra_pip_install_flags", None)
+
+        return (self.indices_args + tuple(extra_pip_flags)) if extra_pip_flags else self.indices_args
+
+    def download_flags(self):
+        if self.indices_args is None:
+            self.indices_args = tuple(
+                chain.from_iterable(('--extra-index-url', x) for x in PIP_EXTRA_INDICES)
+            )
+
         return self.indices_args
```

## Comparing `clearml_agent-1.5.3rc4.dist-info/LICENSE` & `clearml_agent-1.6.0rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clearml_agent-1.5.3rc4.dist-info/METADATA` & `clearml_agent-1.6.0rc0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearml-agent
-Version: 1.5.3rc4
+Version: 1.6.0rc0
 Summary: ClearML Agent - Auto-Magical DevOps for Deep Learning
 Home-page: https://github.com/allegroai/clearml-agent
 Author: Allegroai
 Author-email: clearml@allegro.ai
 License: Apache License 2.0
 Keywords: clearml trains devops machine deep learning agent automation hpc cluster
 Platform: UNKNOWN
```

## Comparing `clearml_agent-1.5.3rc4.dist-info/RECORD` & `clearml_agent-1.6.0rc0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 clearml_agent/__init__.py,sha256=x8fsfFnx1WMwOw5RJmsZxSfeUCWc6ZLXGX_78McBsNs,50
 clearml_agent/__main__.py,sha256=UlsXGOOFOyMfJCTpFWpYFmM21rNtdKYQ7lhgAeBYphs,2891
 clearml_agent/complete.py,sha256=g8oDVqTg6Nq-p56bTJyhBwCPgsoerh73VRox8YY4FUM,2410
 clearml_agent/config.py,sha256=-pLaHyLsQJxpEIY3TysH5baN6fc5hkpfhAiBT1P--ps,736
-clearml_agent/definitions.py,sha256=1oRp0cRxYtalR-7_8lbkkIpzgsqkOstGtlXMP2tkLZA,11218
+clearml_agent/definitions.py,sha256=QAabosbFPV3Pfe2wDURRxbTIZh9IkR-8cOKiolKnHdE,11312
 clearml_agent/errors.py,sha256=JI7zT0mLJeL-rwgrFJAUAc__XdGm9HGpnxhEYeSu-44,2826
 clearml_agent/session.py,sha256=k_MFy26zhmeqG2G5BkVwO2HDdjGddYKozfv2C-kofO4,15942
-clearml_agent/version.py,sha256=5N512WpBCPg66uNfl3wE3kwcJkn7DQxBLJz-3FyuixM,25
+clearml_agent/version.py,sha256=K6gqcXekdfXqfW7oY6BDpkQTJh65OT2YzGwvxYDdT8c,25
 clearml_agent/backend_api/__init__.py,sha256=lN-HRyAnJd6044dJ_RKgsA28BarmAG4Pbdxu9IIwWsE,123
 clearml_agent/backend_api/utils.py,sha256=tFHquUe5nJQX9p9dB25nx5HKNfbwOBWj29fG387W1-s,4786
 clearml_agent/backend_api/config/__init__.py,sha256=7prYyl5e9R4evwdOfMevoD-hjpj2P8UTbsy-OwidpDw,561
 clearml_agent/backend_api/config/default/agent.conf,sha256=bCposUHp_LItOSEFVG2SM4GU7R6w8ty2h4BIsa_GPjI,20435
 clearml_agent/backend_api/config/default/api.conf,sha256=aEe45ERpEBh-a5XivxORZQDtoKR8VKOO0_mKxaWM3Uk,1796
 clearml_agent/backend_api/config/default/logging.conf,sha256=ZvFOI9Ww6ro4IgbNcCY-Zx3D25xaSpLKdDgG7PcxMfg,92
 clearml_agent/backend_api/config/default/sdk.conf,sha256=XFiJTCtBCuWQ2r2SgtPRMJsPFb81h175SySt7_aBBU0,6857
@@ -65,31 +65,35 @@
 clearml_agent/backend_config/utils.py,sha256=CguzBvNYf_2SIsEv7v7hcG-hJDLfPgYHQw8Xh4SJ9UU,4219
 clearml_agent/commands/__init__.py,sha256=YV58pttbL_17b-nKhaQ_PvljaUcOiQeVoB-t-dBj_mY,99
 clearml_agent/commands/base.py,sha256=KESXmyIa3gGIMsQoSeBkvC63OLHB-SqrlntXAmrBvs4,15160
 clearml_agent/commands/check_config.py,sha256=EDrc16zKuNvRX-YWEI4y8qutBWk7BmWluyF5lAoF9tk,536
 clearml_agent/commands/config.py,sha256=mo8SR3w-Pd05Ap-iF8YeyqwHhLqRVbvV4ay8jjz3dkg,17027
 clearml_agent/commands/events.py,sha256=8Wz6AkFXvZxf_FKTwaElqaU4pyZ6yWlSAytsCdw1ZdQ,3204
 clearml_agent/commands/resolver.py,sha256=JJKXArIhZVjLwejrCg075eh2i6CDHqbH9iheXBgSnBI,6552
-clearml_agent/commands/worker.py,sha256=LM2uHKcX0NlvpKit-QwyUe2Wf4IE4VW2rBASAJaC0Iw,191566
+clearml_agent/commands/worker.py,sha256=ngNYpUUICdY6RxHAokPab4ehtYmcGmfbHcYp-gKp_Qs,194477
 clearml_agent/external/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 clearml_agent/external/pyhocon/__init__.py,sha256=9Y64dUMI_8P52FEC4HP0IcB90JkrtJEAjqXRn8dLX0Q,256
 clearml_agent/external/pyhocon/config_parser.py,sha256=kKaRs0uKTw_MYi0zzExNksFY9gC_NJw-hB-LlqbSFok,32918
 clearml_agent/external/pyhocon/config_tree.py,sha256=Fbw1_2DoplrJXJTUVNlscmr6x42smNNMAYxilFVT7Dg,22532
 clearml_agent/external/pyhocon/converter.py,sha256=b0Yj2t5GeUJRaH26KBoToOa5KYzuyroz9zJO-Jvea54,13100
 clearml_agent/external/pyhocon/exceptions.py,sha256=k_6C6fB063ifnjiMDiRtL53tF4TO6lcbkwLA2wsYOZc,352
 clearml_agent/external/requirements_parser/__init__.py,sha256=lAOYEvxEeIkllA8iyViWAaiR3GDB7MagIrK_nWGr_L8,353
 clearml_agent/external/requirements_parser/fragment.py,sha256=6wOYDZVGIvx_EGX9CtnsJlgC35Yd4BvxFf6JfyoYhZ0,1298
 clearml_agent/external/requirements_parser/parser.py,sha256=YmuLV_XIHwiQo2XfpeEiA3PHh-YS_drYPc2SKlM6O14,2368
 clearml_agent/external/requirements_parser/requirement.py,sha256=RxAvVLlMTec7uC3IQpBe40D5FqEiB_DyH0-HCoNwNP0,9362
 clearml_agent/external/requirements_parser/vcs.py,sha256=mC72sDWbzzXUuZHZCw25eQ3dJitXII5E4AY3kg8yHEw,405
 clearml_agent/glue/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+clearml_agent/glue/daemon.py,sha256=jgTt_kMcRk815Wq9tfQ9m2qY6uBio5oZ9FuYin9RKhw,358
 clearml_agent/glue/definitions.py,sha256=IIjiKRy7PjAuwi8w2xB_OSSB5YnpREsW5g8xAruL4UU,316
-clearml_agent/glue/k8s.py,sha256=XarWika7pbgeGZag0ypUr5fg907ei-Wf1MQKfVbW-mw,47157
+clearml_agent/glue/errors.py,sha256=pu8chuJdn87kmonenU7aRJwcul8LavLRqizhJeggcgs,130
+clearml_agent/glue/k8s.py,sha256=F_zeNNU7ecl3DvVdQYe6Hkf3eLNviJ647GrIe4Tp8l8,48544
+clearml_agent/glue/pending_pods_daemon.py,sha256=9SvPSIZdoPk7f2PJndjgNOferr2vXRH0WNs3KXa-ZXs,9773
+clearml_agent/glue/utilities.py,sha256=c4CJIf10ADyBwd7fKIMyLqStLWXEGal2v8evmbHrKHo,452
 clearml_agent/helper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-clearml_agent/helper/base.py,sha256=BAHNgCG5HvTTKiI6jKcuO39yTnkeQQmoUFDMxHh0TqY,18556
+clearml_agent/helper/base.py,sha256=Bzui57eVd38bumJ8T8YiW1t6EfuBjNiLnk_9QkzLcIo,18669
 clearml_agent/helper/check_update.py,sha256=jPqXe-3pZ0uRjkhcNuLPxSyXhGuMxJ-IMkbubNMY4WQ,2200
 clearml_agent/helper/console.py,sha256=iaoo3U51xXRwahfWdMMjXw4OkY5BlKGXZdu5SzFIZVA,3650
 clearml_agent/helper/dicts.py,sha256=9NJVHPegGw3Cgn8Lyem2UM6prnzwf8IkR7uKYGPzPlA,828
 clearml_agent/helper/docker_args.py,sha256=e7VDowX2AdYV4_oPe8_ELkJqRiEx0W0CYWR0q7rdUJA,3403
 clearml_agent/helper/process.py,sha256=ik23IsAnzWzADNltfi_DDP5oOyOZc9PXjFXFmLOF4qg,15065
 clearml_agent/helper/repo.py,sha256=qELYKrI_mw-0nnToHx0bdRuK118V-kYN1lXpUovYFE4,30196
 clearml_agent/helper/resource_monitor.py,sha256=4-nCFIgrFjRRbg85bnLWBWvWiMm8on2PKeKx8j1ErJU,11656
@@ -101,29 +105,29 @@
 clearml_agent/helper/gpu/pynvml.py,sha256=Y6mfWiBDp77pR4T_umWzxFGwqaGQO5PVx4FqyLHmUt4,122691
 clearml_agent/helper/os/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 clearml_agent/helper/os/daemonize.py,sha256=rhjg9VQqQR9a-ddBx4KfkFIL2qtrAFuQi34g-co-s4c,2949
 clearml_agent/helper/os/folder_cache.py,sha256=gClbMZke32o59B_hcbmPvtFH9yAxAOeXGP5KpyES-vY,9311
 clearml_agent/helper/os/locks.py,sha256=OiwvAClfN72cnHjiwJObCPwAhBpyUm_dS07Ho3aauaQ,6180
 clearml_agent/helper/os/portalocker.py,sha256=gZ3dCaAsiymueMQittzfF-XHDtrzuSl5mc_V3roNnwo,6966
 clearml_agent/helper/package/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-clearml_agent/helper/package/base.py,sha256=JtNopkeg2hrNSqTSy8igkdvV1GZTwclxBQzCVZ98brE,11518
+clearml_agent/helper/package/base.py,sha256=t5KZ62-FbH5dY0DgYHcy4yDmK1ceIPl0lqvyPnTGEhg,11699
 clearml_agent/helper/package/conda_api.py,sha256=zkLEqXwr18TFxrVM6acIKtVF8mUbCg6RERvyhZtXiY4,32312
 clearml_agent/helper/package/external_req.py,sha256=ddFkbcbsbehUdjM3sC4ZnrZAiXSZtZf87vgpVJc5ol4,8224
-clearml_agent/helper/package/poetry_api.py,sha256=qr7dBDvgOBZUBECnwFTJlD3NltwgfNmGwW9mcnQtfjs,6181
+clearml_agent/helper/package/poetry_api.py,sha256=PDputg1Fnb1gUQJc_McvU1nlG0DJm70Z78AGoVWVr54,6212
 clearml_agent/helper/package/post_req.py,sha256=IZSGNDK8TUTLSAuCAHaN8y5AnFGhhYehm1Du6yJVysM,1764
-clearml_agent/helper/package/priority_req.py,sha256=Vw7Pa8gcwybM_mWVa7xgjeB2VNC7NKUUmGLJMEdBc5M,4257
+clearml_agent/helper/package/priority_req.py,sha256=bM3PBGnjJUOHQrzGVK5IA6QwSKZTY4GCORjZHQd_k68,4761
 clearml_agent/helper/package/pytorch.py,sha256=QhLHUSH1hic1X5q2DpXeSQLMnO5ybRi4xPNtkqQIeXw,40778
 clearml_agent/helper/package/requirements.py,sha256=cyRu7OgfS6_oWhMjbUHzlw78uwOM6oRs6OqpOi3rqVM,31340
 clearml_agent/helper/package/translator.py,sha256=jwdc0wwD7UI1Z80NLwGLEf1cFrzZKI28KPkqA-ZEURI,3452
 clearml_agent/helper/package/venv_update_api.py,sha256=dX_EeraHgU2cd36S2pKEzp_bNKGKeyTz83yOgYyw_vo,3401
 clearml_agent/helper/package/pip_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-clearml_agent/helper/package/pip_api/system.py,sha256=_4XFdVR8NCiuxhvHqTukeuPqbfpkO_Fxj2Mgb3ExMV0,3360
+clearml_agent/helper/package/pip_api/system.py,sha256=V-Nnr5TdTAChi1dtKyJiup0SuijkdBCg2dWEuYHai0A,4063
 clearml_agent/helper/package/pip_api/venv.py,sha256=t-xhl1djtlS_XhATwEeahI6eId_N6mMnN1ai2J0k6OI,2951
 clearml_agent/interface/__init__.py,sha256=8Bxzt8z7hcpx8EBDu7MrSt0aegdcCX1-EI6-yOY6sGs,1244
 clearml_agent/interface/base.py,sha256=gjECQZsolfZY6AADkomj_OzNy0Gy3ap5mnex2O7Wi0A,15036
 clearml_agent/interface/worker.py,sha256=AEKdxr2zWSQvZVl0fYtu-rM_vdO2XvnLy_qpgIbNDQ8,9937
-clearml_agent-1.5.3rc4.dist-info/LICENSE,sha256=y_zZWeeAnf6mRnYn7HBoaFA8qF9Xsx3j01jNTcppKlY,11340
-clearml_agent-1.5.3rc4.dist-info/METADATA,sha256=V79ySuTlhIm_4F-lfdLNTljHKdqa2Z6A-cul2lE-bwA,18199
-clearml_agent-1.5.3rc4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-clearml_agent-1.5.3rc4.dist-info/entry_points.txt,sha256=05FyI7Hjs821dPHdDAe0OOu7ZRYDpJ4i7RpgNdX6NXA,63
-clearml_agent-1.5.3rc4.dist-info/top_level.txt,sha256=_TrkgE1QyUVMVlaIweOwBzQtGx6A2PJ60rBpYMYSlYo,14
-clearml_agent-1.5.3rc4.dist-info/RECORD,,
+clearml_agent-1.6.0rc0.dist-info/LICENSE,sha256=y_zZWeeAnf6mRnYn7HBoaFA8qF9Xsx3j01jNTcppKlY,11340
+clearml_agent-1.6.0rc0.dist-info/METADATA,sha256=ve_QKzxAqI6Jrq-zTCtEmkFL21o9_sLCeN4HibFr-ME,18199
+clearml_agent-1.6.0rc0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+clearml_agent-1.6.0rc0.dist-info/entry_points.txt,sha256=05FyI7Hjs821dPHdDAe0OOu7ZRYDpJ4i7RpgNdX6NXA,63
+clearml_agent-1.6.0rc0.dist-info/top_level.txt,sha256=_TrkgE1QyUVMVlaIweOwBzQtGx6A2PJ60rBpYMYSlYo,14
+clearml_agent-1.6.0rc0.dist-info/RECORD,,
```

