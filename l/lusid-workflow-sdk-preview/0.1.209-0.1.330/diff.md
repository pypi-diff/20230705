# Comparing `tmp/lusid-workflow-sdk-preview-0.1.209.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.330.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.209.tar", last modified: Fri Apr 14 16:04:20 2023, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.330.tar", last modified: Wed Jul  5 08:27:28 2023, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.209.tar` & `lusid-workflow-sdk-preview-0.1.330.tar`

### file list

```diff
@@ -1,51 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7679 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     3213 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44932 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    32083 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    17241 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     2133 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11241 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7455 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)    11826 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    10500 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_response.py
--rw-r--r--   0 root         (0) root         (0)     8669 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/version.py
--rw-r--r--   0 root         (0) root         (0)     8987 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     4395 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 16:04:20.000000 lusid-workflow-sdk-preview-0.1.209/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-14 16:03:54.000000 lusid-workflow-sdk-preview-0.1.209/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     4531 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56187 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    41163 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    36409 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     3451 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6094 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)    12968 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14045 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     5389 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)    10977 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/version.py
+-rw-r--r--   0 root         (0) root         (0)    11007 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     7614 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:27:28.000000 lusid-workflow-sdk-preview-0.1.330/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-05 08:26:36.000000 lusid-workflow-sdk-preview-0.1.330/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/README.md` & `lusid-workflow-sdk-preview-0.1.330/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.209
-- Package version: 0.1.209
+- API version: 0.1.330
+- Package version: 0.1.330
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -71,71 +71,93 @@
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with lusid_workflow.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = lusid_workflow.TaskDefinitionsApi(api_client)
-    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields.assignee exists AND fields.assignee NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields.resolutionDetail exists AND fields.resolutionDetail NOT eq ''"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields.cancellationDetail exists AND fields.cancellationDetail NOT eq ''"}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
+    create_task_definition_request = {"id":{"scope":"A1","code":"ZZZ"},"displayName":"An example TaskDefinition","description":"Test","states":[{"name":"Submitted"},{"name":"InProgress"},{"name":"SendingSurvey"},{"name":"Done"},{"name":"SurveyNotSent"},{"name":"NotDone"}],"fieldSchema":[{"name":"clientId","type":"String"},{"name":"assignee","type":"String"},{"name":"resolutionDetail","type":"String"}],"initialState":{"name":"Submitted","requiredFields":["clientId"]},"triggers":[{"name":"start","trigger":{"type":"External"}},{"name":"cancel","trigger":{"type":"External"}},{"name":"resolve","trigger":{"type":"External"}},{"name":"timeout","trigger":{"type":"External"}},{"name":"success","trigger":{"type":"External"}},{"name":"failure","trigger":{"type":"External"}}],"transitions":[{"fromState":"Submitted","toState":"InProgress","trigger":"start","guard":"fields['assignee'] exists AND fields['assignee'] NOT eq ''"},{"fromState":"InProgress","toState":"SendingSurvey","trigger":"resolve","guard":"fields['resolutionDetail'] exists AND fields['resolutionDetail'] NOT eq ''","action":"health-check"},{"fromState":"SendingSurvey","toState":"Done","trigger":"success"},{"fromState":"SendingSurvey","toState":"SurveyNotSent","trigger":"failure"},{"fromState":"SendingSurvey","toState":"NotDone","trigger":"timeout"},{"fromState":"InProgress","toState":"NotDone","trigger":"cancel","guard":"fields['cancellationDetail'] exists AND fields['cancellationDetail'] NOT eq ''"}],"actions":[{"name":"health-check","actionDetails":{"type":"RunWorker","workerId":{"scope":"Health","code":"HealthCheckWorker"},"workerAsAt":"2022-01-01T01:02:03.0000000+00:00","workerParameters":{},"workerStatusTriggers":{},"childTaskConfigurations":[{"taskDefinitionId":{"scope":"AAA","code":"BBB"},"initialTrigger":"test-trigger","childTaskFields":{"assignee":{"mapFrom":"foo","setTo":"bar"}}}]}}]} # CreateTaskDefinitionRequest | The data to create a Task Definition
 
     try:
-        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.
+        # [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
         api_response = api_instance.create_task_definition(create_task_definition_request)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling TaskDefinitionsApi->create_task_definition: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://www.lusid.com/workflow*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.
-*TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition.
-*TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition.
-*TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions/{scope} | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
-*TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition.
-*TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task.
-*TasksApi* | [**delete_task**](docs/TasksApi.md#delete_task) | **DELETE** /api/tasks/{id} | [EXPERIMENTAL] DeleteTask: Delete a Task.
-*TasksApi* | [**get_task**](docs/TasksApi.md#get_task) | **GET** /api/tasks/{id} | [EXPERIMENTAL] GetTask: Get a Task.
-*TasksApi* | [**update_task**](docs/TasksApi.md#update_task) | **POST** /api/tasks/{id} | [EXPERIMENTAL] UpdateTask: Update a Task.
-*WorkersApi* | [**create_worker**](docs/WorkersApi.md#create_worker) | **POST** /api/workers | [EXPERIMENTAL] CreateWorker: Endpoint For Creating a Worker
-*WorkersApi* | [**get_worker**](docs/WorkersApi.md#get_worker) | **GET** /api/workers/{scope}/{code} | [EXPERIMENTAL] GetWorker: Endpoint for Retrieving a Worker
+*TaskDefinitionsApi* | [**create_task_definition**](docs/TaskDefinitionsApi.md#create_task_definition) | **POST** /api/taskdefinitions | [EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition
+*TaskDefinitionsApi* | [**delete_task_definition**](docs/TaskDefinitionsApi.md#delete_task_definition) | **DELETE** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition
+*TaskDefinitionsApi* | [**get_task_definition**](docs/TaskDefinitionsApi.md#get_task_definition) | **GET** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] GetTaskDefinition: Get a Task Definition
+*TaskDefinitionsApi* | [**list_task_definitions**](docs/TaskDefinitionsApi.md#list_task_definitions) | **GET** /api/taskdefinitions | [EXPERIMENTAL] ListTaskDefinitions: List Task Definitions
+*TaskDefinitionsApi* | [**list_tasks_for_task_definition**](docs/TaskDefinitionsApi.md#list_tasks_for_task_definition) | **GET** /api/taskdefinitions/{scope}/{code}/tasks | [EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition
+*TaskDefinitionsApi* | [**update_task_definition**](docs/TaskDefinitionsApi.md#update_task_definition) | **PUT** /api/taskdefinitions/{scope}/{code} | [EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition
+*TasksApi* | [**create_task**](docs/TasksApi.md#create_task) | **POST** /api/tasks | [EXPERIMENTAL] CreateTask: Create a new Task
+*TasksApi* | [**delete_task**](docs/TasksApi.md#delete_task) | **DELETE** /api/tasks/{id} | [EXPERIMENTAL] DeleteTask: Delete a Task
+*TasksApi* | [**get_task**](docs/TasksApi.md#get_task) | **GET** /api/tasks/{id} | [EXPERIMENTAL] GetTask: Get a Task
+*TasksApi* | [**list_tasks**](docs/TasksApi.md#list_tasks) | **GET** /api/tasks | [EXPERIMENTAL] ListTasks: List Tasks
+*TasksApi* | [**update_task**](docs/TasksApi.md#update_task) | **POST** /api/tasks/{id} | [EXPERIMENTAL] UpdateTask: Update a Task
+*WorkersApi* | [**create_worker**](docs/WorkersApi.md#create_worker) | **POST** /api/workers | [EXPERIMENTAL] CreateWorker: Create a new Worker
+*WorkersApi* | [**get_worker**](docs/WorkersApi.md#get_worker) | **GET** /api/workers/{scope}/{code} | [EXPERIMENTAL] GetWorker: Get a Worker
+*WorkersApi* | [**list_workers**](docs/WorkersApi.md#list_workers) | **GET** /api/workers | [EXPERIMENTAL] ListWorkers: List Workers
+*WorkersApi* | [**run_worker**](docs/WorkersApi.md#run_worker) | **POST** /api/workers/{scope}/{code}/$run | [EXPERIMENTAL] RunWorker: Run a Worker
 
 
 ## Documentation For Models
 
+ - [ActionDefinition](docs/ActionDefinition.md)
+ - [ActionDetails](docs/ActionDetails.md)
+ - [CreateChildTasksAction](docs/CreateChildTasksAction.md)
  - [CreateTaskDefinitionRequest](docs/CreateTaskDefinitionRequest.md)
  - [CreateTaskRequest](docs/CreateTaskRequest.md)
  - [CreateWorkerRequest](docs/CreateWorkerRequest.md)
  - [DeletedEntityResponse](docs/DeletedEntityResponse.md)
+ - [FieldMapping](docs/FieldMapping.md)
+ - [HealthCheck](docs/HealthCheck.md)
  - [InitialState](docs/InitialState.md)
  - [Link](docs/Link.md)
+ - [LuminesceView](docs/LuminesceView.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
+ - [PagedResourceListOfTask](docs/PagedResourceListOfTask.md)
+ - [PagedResourceListOfTaskDefinition](docs/PagedResourceListOfTaskDefinition.md)
+ - [PagedResourceListOfWorker](docs/PagedResourceListOfWorker.md)
+ - [Parameter](docs/Parameter.md)
+ - [ParameterValue](docs/ParameterValue.md)
  - [ResourceId](docs/ResourceId.md)
- - [ResourceListOfTaskDefinition](docs/ResourceListOfTaskDefinition.md)
+ - [ResourceListOfTask](docs/ResourceListOfTask.md)
+ - [ResultField](docs/ResultField.md)
+ - [ResultMatchingPattern](docs/ResultMatchingPattern.md)
+ - [ResultantChildTaskConfiguration](docs/ResultantChildTaskConfiguration.md)
+ - [RunWorkerAction](docs/RunWorkerAction.md)
+ - [RunWorkerRequest](docs/RunWorkerRequest.md)
+ - [RunWorkerResponse](docs/RunWorkerResponse.md)
  - [Task](docs/Task.md)
  - [TaskDefinition](docs/TaskDefinition.md)
  - [TaskDefinitionVersion](docs/TaskDefinitionVersion.md)
  - [TaskFieldDefinition](docs/TaskFieldDefinition.md)
  - [TaskInstanceField](docs/TaskInstanceField.md)
  - [TaskStateDefinition](docs/TaskStateDefinition.md)
  - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
  - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
+ - [TriggerParentTaskAction](docs/TriggerParentTaskAction.md)
  - [TriggerSchema](docs/TriggerSchema.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
  - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
- - [UpdateTaskResponse](docs/UpdateTaskResponse.md)
  - [Version](docs/Version.md)
  - [Worker](docs/Worker.md)
  - [WorkerConfiguration](docs/WorkerConfiguration.md)
+ - [WorkerStatusTriggers](docs/WorkerStatusTriggers.md)
 
 
 ## Documentation For Authorization
 
 
 ## oauth2
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.209"
+__version__ = "0.1.330"
 
 # import apis into sdk package
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
@@ -27,39 +27,57 @@
 from lusid_workflow.configuration import Configuration
 from lusid_workflow.exceptions import OpenApiException
 from lusid_workflow.exceptions import ApiTypeError
 from lusid_workflow.exceptions import ApiValueError
 from lusid_workflow.exceptions import ApiKeyError
 from lusid_workflow.exceptions import ApiException
 # import models into sdk package
+from lusid_workflow.models.action_definition import ActionDefinition
+from lusid_workflow.models.action_details import ActionDetails
+from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
+from lusid_workflow.models.field_mapping import FieldMapping
+from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
+from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
+from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
+from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
+from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
+from lusid_workflow.models.parameter import Parameter
+from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
-from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
+from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
+from lusid_workflow.models.result_field import ResultField
+from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
+from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
+from lusid_workflow.models.run_worker_action import RunWorkerAction
+from lusid_workflow.models.run_worker_request import RunWorkerRequest
+from lusid_workflow.models.run_worker_response import RunWorkerResponse
 from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
 from lusid_workflow.models.task_field_definition import TaskFieldDefinition
 from lusid_workflow.models.task_instance_field import TaskInstanceField
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
+from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
-from lusid_workflow.models.update_task_response import UpdateTaskResponse
 from lusid_workflow.models.version import Version
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
+from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
 from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
 from fbnsdkutilities.utilities.api_configuration_loader import ApiConfigurationLoader
 from fbnsdkutilities.utilities.refreshing_token import RefreshingToken
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/task_definitions_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -23,15 +23,16 @@
     ApiTypeError,
     ApiValueError
 )
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
+from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
+from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
 from lusid_workflow.models.task_definition import TaskDefinition
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 
 
 class TaskDefinitionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -41,15 +42,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def create_task_definition(self, create_task_definition_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_task_definition(create_task_definition_request, async_req=True)
         >>> result = thread.get()
 
@@ -70,15 +71,15 @@
                  returns the request thread.
         :rtype: TaskDefinition
         """
         kwargs['_return_http_data_only'] = True
         return self.create_task_definition_with_http_info(create_task_definition_request, **kwargs)  # noqa: E501
 
     def create_task_definition_with_http_info(self, create_task_definition_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] CreateTaskDefinition: Create a new Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_task_definition_with_http_info(create_task_definition_request, async_req=True)
         >>> result = thread.get()
 
@@ -158,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -186,15 +187,15 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def delete_task_definition(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_task_definition(scope, code, async_req=True)
         >>> result = thread.get()
 
@@ -217,15 +218,15 @@
                  returns the request thread.
         :rtype: DeletedEntityResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_task_definition_with_http_info(scope, code, **kwargs)  # noqa: E501
 
     def delete_task_definition_with_http_info(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] DeleteTaskDefinition: Delete a Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_task_definition_with_http_info(scope, code, async_req=True)
         >>> result = thread.get()
 
@@ -327,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -356,27 +357,27 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def get_task_definition(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTaskDefinition: Get a Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] GetTaskDefinition: Get a Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_task_definition(scope, code, async_req=True)
         >>> result = thread.get()
 
         :param scope: The scope that identifies a Task Definition (required)
         :type scope: str
         :param code: The code that identifies a Task Definition (required)
         :type code: str
-        :param as_at: AsAt time to retrieve stated Task Definition. Default to current time if not provided.
+        :param as_at: The asAt datetime at which to retrieve the Task Definition. Defaults to returning the latest version of the Task Definition if not specified.
         :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
@@ -389,27 +390,27 @@
                  returns the request thread.
         :rtype: TaskDefinition
         """
         kwargs['_return_http_data_only'] = True
         return self.get_task_definition_with_http_info(scope, code, **kwargs)  # noqa: E501
 
     def get_task_definition_with_http_info(self, scope, code, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTaskDefinition: Get a Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] GetTaskDefinition: Get a Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_task_definition_with_http_info(scope, code, async_req=True)
         >>> result = thread.get()
 
         :param scope: The scope that identifies a Task Definition (required)
         :type scope: str
         :param code: The code that identifies a Task Definition (required)
         :type code: str
-        :param as_at: AsAt time to retrieve stated Task Definition. Default to current time if not provided.
+        :param as_at: The asAt datetime at which to retrieve the Task Definition. Defaults to returning the latest version of the Task Definition if not specified.
         :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -504,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -532,54 +533,62 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def list_task_definitions(self, scope, **kwargs):  # noqa: E501
+    def list_task_definitions(self, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] ListTaskDefinitions: List Task Definitions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_task_definitions(scope, async_req=True)
+        >>> thread = api.list_task_definitions(async_req=True)
         >>> result = thread.get()
 
-        :param scope: (required)
-        :type scope: str
+        :param as_at: The asAt datetime at which to list the Task Definitions. Defaults to return the latest version of each Task Definition if not specified.
+        :type as_at: datetime
+        :param limit: When paginating, limit the number of returned results to this many.
+        :type limit: int
+        :param page: The pagination token to use to continue listing task definitions from a previous call to list task definitions. This value is returned from the previous call. If a pagination token is provided the sortBy, filter, effectiveAt, and asAt fields must not have changed since the original request.
+        :type page: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ResourceListOfTaskDefinition
+        :rtype: PagedResourceListOfTaskDefinition
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_task_definitions_with_http_info(scope, **kwargs)  # noqa: E501
+        return self.list_task_definitions_with_http_info(**kwargs)  # noqa: E501
 
-    def list_task_definitions_with_http_info(self, scope, **kwargs):  # noqa: E501
+    def list_task_definitions_with_http_info(self, **kwargs):  # noqa: E501
         """[EXPERIMENTAL] ListTaskDefinitions: List Task Definitions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_task_definitions_with_http_info(scope, async_req=True)
+        >>> thread = api.list_task_definitions_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param scope: (required)
-        :type scope: str
+        :param as_at: The asAt datetime at which to list the Task Definitions. Defaults to return the latest version of each Task Definition if not specified.
+        :type as_at: datetime
+        :param limit: When paginating, limit the number of returned results to this many.
+        :type limit: int
+        :param page: The pagination token to use to continue listing task definitions from a previous call to list task definitions. This value is returned from the previous call. If a pagination token is provided the sortBy, filter, effectiveAt, and asAt fields must not have changed since the original request.
+        :type page: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -592,21 +601,23 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object, the HTTP status code, and the headers.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (ResourceListOfTaskDefinition, int, HTTPHeaderDict)
+        :rtype: (PagedResourceListOfTaskDefinition, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
         all_params = [
-            'scope'
+            'as_at',
+            'limit',
+            'page'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -619,34 +630,211 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method list_task_definitions" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+
+        if self.api_client.client_side_validation and ('page' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['page']) > 500):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_task_definitions`, length must be less than or equal to `500`")  # noqa: E501
+        if self.api_client.client_side_validation and ('page' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['page']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_task_definitions`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'page' in local_var_params and not re.search(r'^[a-zA-Z0-9\+\/]*={0,3}$', local_var_params['page']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_task_definitions`, must conform to the pattern `/^[a-zA-Z0-9\+\/]*={0,3}$/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
+            query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
+        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
+            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
+        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
+            query_params.append(('page', local_var_params['page']))  # noqa: E501
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        header_params['Accept-Encoding'] = "gzip, deflate, br"
+
+
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
+
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
+
+        response_types_map = {
+            200: "PagedResourceListOfTaskDefinition",
+            400: "LusidValidationProblemDetails",
+            404: "str",
+        }
+
+        return self.api_client.call_api(
+            '/api/taskdefinitions', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
+    def list_tasks_for_task_definition(self, scope, code, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_tasks_for_task_definition(scope, code, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a Task Definition (required)
+        :type scope: str
+        :param code: The code that identifies a Task Definition (required)
+        :type code: str
+        :param as_at: The asAt datetime at which to list the Tasks. Defaults to return the latest version of each Task if not specified.
+        :type as_at: datetime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ResourceListOfTask
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.list_tasks_for_task_definition_with_http_info(scope, code, **kwargs)  # noqa: E501
+
+    def list_tasks_for_task_definition_with_http_info(self, scope, code, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] ListTasksForTaskDefinition: List Tasks for a Task Definition  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_tasks_for_task_definition_with_http_info(scope, code, async_req=True)
+        >>> result = thread.get()
+
+        :param scope: The scope that identifies a Task Definition (required)
+        :type scope: str
+        :param code: The code that identifies a Task Definition (required)
+        :type code: str
+        :param as_at: The asAt datetime at which to list the Tasks. Defaults to return the latest version of each Task if not specified.
+        :type as_at: datetime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :return: Returns the result object, the HTTP status code, and the headers.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: (ResourceListOfTask, int, HTTPHeaderDict)
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'scope',
+            'code',
+            'as_at'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_tasks_for_task_definition" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
         # verify the required parameter 'scope' is set
         if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
                                                         local_var_params['scope'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `scope` when calling `list_task_definitions`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `list_tasks_for_task_definition`")  # noqa: E501
+        # verify the required parameter 'code' is set
+        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
+                                                        local_var_params['code'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `code` when calling `list_tasks_for_task_definition`")  # noqa: E501
 
         if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
                                                         len(local_var_params['scope']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `list_task_definitions`, length must be less than or equal to `64`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `list_tasks_for_task_definition`, length must be less than or equal to `64`")  # noqa: E501
         if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
                                                         len(local_var_params['scope']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `list_task_definitions`, length must be greater than or equal to `1`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `list_tasks_for_task_definition`, length must be greater than or equal to `1`")  # noqa: E501
         if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `scope` when calling `list_task_definitions`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `list_tasks_for_task_definition`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) > 64):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `list_tasks_for_task_definition`, length must be less than or equal to `64`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `list_tasks_for_task_definition`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `list_tasks_for_task_definition`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
         if 'scope' in local_var_params:
             path_params['scope'] = local_var_params['scope']  # noqa: E501
+        if 'code' in local_var_params:
+            path_params['code'] = local_var_params['code']  # noqa: E501
 
         query_params = []
+        if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
+            query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -655,27 +843,27 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
-            200: "ResourceListOfTaskDefinition",
+            200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
             404: "str",
         }
 
         return self.api_client.call_api(
-            '/api/taskdefinitions/{scope}', 'GET',
+            '/api/taskdefinitions/{scope}/{code}/tasks', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -684,15 +872,15 @@
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
     def update_task_definition(self, scope, code, update_task_definition_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_task_definition(scope, code, update_task_definition_request, async_req=True)
         >>> result = thread.get()
 
@@ -717,15 +905,15 @@
                  returns the request thread.
         :rtype: TaskDefinition
         """
         kwargs['_return_http_data_only'] = True
         return self.update_task_definition_with_http_info(scope, code, update_task_definition_request, **kwargs)  # noqa: E501
 
     def update_task_definition_with_http_info(self, scope, code, update_task_definition_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition.  # noqa: E501
+        """[EXPERIMENTAL] UpdateTaskDefinition: Update an existing Task Definition  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_task_definition_with_http_info(scope, code, update_task_definition_request, async_req=True)
         >>> result = thread.get()
 
@@ -839,15 +1027,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api/workers_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -19,79 +19,77 @@
 import six
 
 from lusid_workflow.api_client import ApiClient
 from lusid_workflow.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
-from lusid_workflow.models.create_task_request import CreateTaskRequest
-from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
+from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from lusid_workflow.models.task import Task
-from lusid_workflow.models.update_task_request import UpdateTaskRequest
-from lusid_workflow.models.update_task_response import UpdateTaskResponse
+from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
+from lusid_workflow.models.run_worker_request import RunWorkerRequest
+from lusid_workflow.models.run_worker_response import RunWorkerResponse
+from lusid_workflow.models.worker import Worker
 
 
-class TasksApi(object):
+class WorkersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_task(self, create_task_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTask: Create a new Task.  # noqa: E501
+    def create_worker(self, create_worker_request, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] CreateWorker: Create a new Worker  # noqa: E501
 
+        If the Worker already exists a failure will be returned  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_task(create_task_request, async_req=True)
+        >>> thread = api.create_worker(create_worker_request, async_req=True)
         >>> result = thread.get()
 
-        :param create_task_request: Request to create Task (required)
-        :type create_task_request: CreateTaskRequest
-        :param trigger: The name of the Trigger to invoke
-        :type trigger: str
+        :param create_worker_request: Worker to be created (required)
+        :type create_worker_request: CreateWorkerRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Task
+        :rtype: Worker
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_task_with_http_info(create_task_request, **kwargs)  # noqa: E501
+        return self.create_worker_with_http_info(create_worker_request, **kwargs)  # noqa: E501
 
-    def create_task_with_http_info(self, create_task_request, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] CreateTask: Create a new Task.  # noqa: E501
+    def create_worker_with_http_info(self, create_worker_request, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] CreateWorker: Create a new Worker  # noqa: E501
 
+        If the Worker already exists a failure will be returned  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_task_with_http_info(create_task_request, async_req=True)
+        >>> thread = api.create_worker_with_http_info(create_worker_request, async_req=True)
         >>> result = thread.get()
 
-        :param create_task_request: Request to create Task (required)
-        :type create_task_request: CreateTaskRequest
-        :param trigger: The name of the Trigger to invoke
-        :type trigger: str
+        :param create_worker_request: Worker to be created (required)
+        :type create_worker_request: CreateWorkerRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -104,22 +102,21 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object, the HTTP status code, and the headers.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (Task, int, HTTPHeaderDict)
+        :rtype: (Worker, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
         all_params = [
-            'create_task_request',
-            'trigger'
+            'create_worker_request'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -128,69 +125,61 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_task" % key
+                    " to method create_worker" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'create_task_request' is set
-        if self.api_client.client_side_validation and ('create_task_request' not in local_var_params or  # noqa: E501
-                                                        local_var_params['create_task_request'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `create_task_request` when calling `create_task`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('trigger' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['trigger']) > 150):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `trigger` when calling `create_task`, length must be less than or equal to `150`")  # noqa: E501
-        if self.api_client.client_side_validation and ('trigger' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['trigger']) < 5):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `trigger` when calling `create_task`, length must be greater than or equal to `5`")  # noqa: E501
+        # verify the required parameter 'create_worker_request' is set
+        if self.api_client.client_side_validation and ('create_worker_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['create_worker_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `create_worker_request` when calling `create_worker`")  # noqa: E501
+
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'trigger' in local_var_params and local_var_params['trigger'] is not None:  # noqa: E501
-            query_params.append(('trigger', local_var_params['trigger']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'create_task_request' in local_var_params:
-            body_params = local_var_params['create_task_request']
+        if 'create_worker_request' in local_var_params:
+            body_params = local_var_params['create_worker_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
-            201: "Task",
+            201: "Worker",
             400: "LusidValidationProblemDetails",
         }
 
         return self.api_client.call_api(
-            '/api/tasks', 'POST',
+            '/api/workers', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -198,54 +187,64 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def delete_task(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] DeleteTask: Delete a Task.  # noqa: E501
+    def get_worker(self, scope, code, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] GetWorker: Get a Worker  # noqa: E501
 
+        Will return a NotFound failure if the Worker does not exist  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_task(id, async_req=True)
+        >>> thread = api.get_worker(scope, code, async_req=True)
         >>> result = thread.get()
 
-        :param id: The identifier for the Task to be deleted. (required)
-        :type id: str
+        :param scope: Scope of the worker (required)
+        :type scope: str
+        :param code: Code of the worker (required)
+        :type code: str
+        :param as_at: The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.
+        :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DeletedEntityResponse
+        :rtype: Worker
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_task_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_worker_with_http_info(scope, code, **kwargs)  # noqa: E501
 
-    def delete_task_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] DeleteTask: Delete a Task.  # noqa: E501
+    def get_worker_with_http_info(self, scope, code, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] GetWorker: Get a Worker  # noqa: E501
 
+        Will return a NotFound failure if the Worker does not exist  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_task_with_http_info(id, async_req=True)
+        >>> thread = api.get_worker_with_http_info(scope, code, async_req=True)
         >>> result = thread.get()
 
-        :param id: The identifier for the Task to be deleted. (required)
-        :type id: str
+        :param scope: Scope of the worker (required)
+        :type scope: str
+        :param code: Code of the worker (required)
+        :type code: str
+        :param as_at: The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.
+        :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -258,21 +257,23 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object, the HTTP status code, and the headers.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (DeletedEntityResponse, int, HTTPHeaderDict)
+        :rtype: (Worker, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id'
+            'scope',
+            'code',
+            'as_at'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -281,67 +282,82 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_task" % key
+                    " to method get_worker" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `delete_task`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 40):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_task`, length must be less than or equal to `40`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 30):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_task`, length must be greater than or equal to `30`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_task`, must conform to the pattern `/^[a-zA-Z0-9\-]+$/`")  # noqa: E501
+        # verify the required parameter 'scope' is set
+        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
+                                                        local_var_params['scope'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `get_worker`")  # noqa: E501
+        # verify the required parameter 'code' is set
+        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
+                                                        local_var_params['code'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `code` when calling `get_worker`")  # noqa: E501
+
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) > 64):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `get_worker`, length must be less than or equal to `64`")  # noqa: E501
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `get_worker`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `get_worker`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) > 64):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `get_worker`, length must be less than or equal to `64`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `get_worker`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `get_worker`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'scope' in local_var_params:
+            path_params['scope'] = local_var_params['scope']  # noqa: E501
+        if 'code' in local_var_params:
+            path_params['code'] = local_var_params['code']  # noqa: E501
 
         query_params = []
+        if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
+            query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
-            200: "DeletedEntityResponse",
+            201: "Worker",
             400: "LusidValidationProblemDetails",
-            404: "str",
         }
 
         return self.api_client.call_api(
-            '/api/tasks/{id}', 'DELETE',
+            '/api/workers/{scope}/{code}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -349,58 +365,62 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def get_task(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTask: Get a Task.  # noqa: E501
+    def list_workers(self, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] ListWorkers: List Workers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_task(id, async_req=True)
+        >>> thread = api.list_workers(async_req=True)
         >>> result = thread.get()
 
-        :param id: Id of the Task to retrieve (required)
-        :type id: str
-        :param as_at:
+        :param as_at: The asAt datetime at which to list the Workers. Defaults to return the latest version of each Worker if not specified.
         :type as_at: datetime
+        :param limit: When paginating, limit the number of returned results to this many.
+        :type limit: int
+        :param page: The pagination token to use to continue listing workers from a previous call to list workers. This value is returned from the previous call. If a pagination token is provided the sortBy, filter, effectiveAt, and asAt fields must not have changed since the original request.
+        :type page: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Task
+        :rtype: PagedResourceListOfWorker
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_task_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_workers_with_http_info(**kwargs)  # noqa: E501
 
-    def get_task_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] GetTask: Get a Task.  # noqa: E501
+    def list_workers_with_http_info(self, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] ListWorkers: List Workers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_task_with_http_info(id, async_req=True)
+        >>> thread = api.list_workers_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: Id of the Task to retrieve (required)
-        :type id: str
-        :param as_at:
+        :param as_at: The asAt datetime at which to list the Workers. Defaults to return the latest version of each Worker if not specified.
         :type as_at: datetime
+        :param limit: When paginating, limit the number of returned results to this many.
+        :type limit: int
+        :param page: The pagination token to use to continue listing workers from a previous call to list workers. This value is returned from the previous call. If a pagination token is provided the sortBy, filter, effectiveAt, and asAt fields must not have changed since the original request.
+        :type page: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -413,22 +433,23 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object, the HTTP status code, and the headers.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (Task, int, HTTPHeaderDict)
+        :rtype: (PagedResourceListOfWorker, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'as_at'
+            'as_at',
+            'limit',
+            'page'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -437,69 +458,66 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_task" % key
+                    " to method list_workers" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_task`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 40):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_task`, length must be less than or equal to `40`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 30):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_task`, length must be greater than or equal to `30`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_task`, must conform to the pattern `/^[a-zA-Z0-9\-]+$/`")  # noqa: E501
+
+        if self.api_client.client_side_validation and ('page' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['page']) > 500):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_workers`, length must be less than or equal to `500`")  # noqa: E501
+        if self.api_client.client_side_validation and ('page' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['page']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_workers`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'page' in local_var_params and not re.search(r'^[a-zA-Z0-9\+\/]*={0,3}$', local_var_params['page']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `page` when calling `list_workers`, must conform to the pattern `/^[a-zA-Z0-9\+\/]*={0,3}$/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
         if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
             query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
+        if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
+            query_params.append(('limit', local_var_params['limit']))  # noqa: E501
+        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
+            query_params.append(('page', local_var_params['page']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
-            200: "Task",
+            201: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
-            404: "str",
         }
 
         return self.api_client.call_api(
-            '/api/tasks/{id}', 'GET',
+            '/api/workers', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -507,62 +525,66 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def update_task(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] UpdateTask: Update a Task.  # noqa: E501
+    def run_worker(self, scope, code, run_worker_request, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] RunWorker: Run a Worker  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_task(id, async_req=True)
+        >>> thread = api.run_worker(scope, code, run_worker_request, async_req=True)
         >>> result = thread.get()
 
-        :param id: Id of the Task to act upon (required)
-        :type id: str
-        :param trigger:
-        :type trigger: str
-        :param update_task_request: The details of the request
-        :type update_task_request: UpdateTaskRequest
+        :param scope: Scope of the worker (required)
+        :type scope: str
+        :param code: Code of the worker (required)
+        :type code: str
+        :param run_worker_request: (required)
+        :type run_worker_request: RunWorkerRequest
+        :param as_at: The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.
+        :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: UpdateTaskResponse
+        :rtype: RunWorkerResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_task_with_http_info(id, **kwargs)  # noqa: E501
+        return self.run_worker_with_http_info(scope, code, run_worker_request, **kwargs)  # noqa: E501
 
-    def update_task_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] UpdateTask: Update a Task.  # noqa: E501
+    def run_worker_with_http_info(self, scope, code, run_worker_request, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] RunWorker: Run a Worker  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_task_with_http_info(id, async_req=True)
+        >>> thread = api.run_worker_with_http_info(scope, code, run_worker_request, async_req=True)
         >>> result = thread.get()
 
-        :param id: Id of the Task to act upon (required)
-        :type id: str
-        :param trigger:
-        :type trigger: str
-        :param update_task_request: The details of the request
-        :type update_task_request: UpdateTaskRequest
+        :param scope: Scope of the worker (required)
+        :type scope: str
+        :param code: Code of the worker (required)
+        :type code: str
+        :param run_worker_request: (required)
+        :type run_worker_request: RunWorkerRequest
+        :param as_at: The asAt datetime at which to retrieve the Worker. Defaults to returning the latest version of the Worker if not specified.
+        :type as_at: datetime
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -575,23 +597,24 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object, the HTTP status code, and the headers.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (UpdateTaskResponse, int, HTTPHeaderDict)
+        :rtype: (RunWorkerResponse, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
         all_params = [
-            'id',
-            'trigger',
-            'update_task_request'
+            'scope',
+            'code',
+            'run_worker_request',
+            'as_at'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -600,80 +623,91 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_task" % key
+                    " to method run_worker" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `update_task`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 40):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `update_task`, length must be less than or equal to `40`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 30):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `update_task`, length must be greater than or equal to `30`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `update_task`, must conform to the pattern `/^[a-zA-Z0-9\-]+$/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('trigger' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['trigger']) > 150):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `trigger` when calling `update_task`, length must be less than or equal to `150`")  # noqa: E501
-        if self.api_client.client_side_validation and ('trigger' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['trigger']) < 5):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `trigger` when calling `update_task`, length must be greater than or equal to `5`")  # noqa: E501
+        # verify the required parameter 'scope' is set
+        if self.api_client.client_side_validation and ('scope' not in local_var_params or  # noqa: E501
+                                                        local_var_params['scope'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `scope` when calling `run_worker`")  # noqa: E501
+        # verify the required parameter 'code' is set
+        if self.api_client.client_side_validation and ('code' not in local_var_params or  # noqa: E501
+                                                        local_var_params['code'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `code` when calling `run_worker`")  # noqa: E501
+        # verify the required parameter 'run_worker_request' is set
+        if self.api_client.client_side_validation and ('run_worker_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['run_worker_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `run_worker_request` when calling `run_worker`")  # noqa: E501
+
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) > 64):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `run_worker`, length must be less than or equal to `64`")  # noqa: E501
+        if self.api_client.client_side_validation and ('scope' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['scope']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `run_worker`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'scope' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['scope']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `scope` when calling `run_worker`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) > 64):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `run_worker`, length must be less than or equal to `64`")  # noqa: E501
+        if self.api_client.client_side_validation and ('code' in local_var_params and  # noqa: E501
+                                                        len(local_var_params['code']) < 1):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `run_worker`, length must be greater than or equal to `1`")  # noqa: E501
+        if self.api_client.client_side_validation and 'code' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['code']):  # noqa: E501
+            raise ApiValueError("Invalid value for parameter `code` when calling `run_worker`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'scope' in local_var_params:
+            path_params['scope'] = local_var_params['scope']  # noqa: E501
+        if 'code' in local_var_params:
+            path_params['code'] = local_var_params['code']  # noqa: E501
 
         query_params = []
-        if 'trigger' in local_var_params and local_var_params['trigger'] is not None:  # noqa: E501
-            query_params.append(('trigger', local_var_params['trigger']))  # noqa: E501
+        if 'as_at' in local_var_params and local_var_params['as_at'] is not None:  # noqa: E501
+            query_params.append(('asAt', local_var_params['as_at']))  # noqa: E501
 
         header_params = dict(local_var_params.get('_headers', {}))
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'update_task_request' in local_var_params:
-            body_params = local_var_params['update_task_request']
+        if 'run_worker_request' in local_var_params:
+            body_params = local_var_params['run_worker_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.209'
+        header_params['X-LUSID-SDK-Version'] = '0.1.330'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
-            200: "UpdateTaskResponse",
+            200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
-            404: "str",
         }
 
         return self.api_client.call_api(
-            '/api/tasks/{id}', 'POST',
+            '/api/workers/{scope}/{code}/$run', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.209/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.330/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.209\n"\
-               "SDK Package Version: 0.1.209".\
+               "Version of the API: 0.1.330\n"\
+               "SDK Package Version: 0.1.330".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,41 +2,59 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
+from lusid_workflow.models.action_definition import ActionDefinition
+from lusid_workflow.models.action_details import ActionDetails
+from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.create_task_definition_request import CreateTaskDefinitionRequest
 from lusid_workflow.models.create_task_request import CreateTaskRequest
 from lusid_workflow.models.create_worker_request import CreateWorkerRequest
 from lusid_workflow.models.deleted_entity_response import DeletedEntityResponse
+from lusid_workflow.models.field_mapping import FieldMapping
+from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.initial_state import InitialState
 from lusid_workflow.models.link import Link
+from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.lusid_problem_details import LusidProblemDetails
 from lusid_workflow.models.lusid_validation_problem_details import LusidValidationProblemDetails
+from lusid_workflow.models.paged_resource_list_of_task import PagedResourceListOfTask
+from lusid_workflow.models.paged_resource_list_of_task_definition import PagedResourceListOfTaskDefinition
+from lusid_workflow.models.paged_resource_list_of_worker import PagedResourceListOfWorker
+from lusid_workflow.models.parameter import Parameter
+from lusid_workflow.models.parameter_value import ParameterValue
 from lusid_workflow.models.resource_id import ResourceId
-from lusid_workflow.models.resource_list_of_task_definition import ResourceListOfTaskDefinition
+from lusid_workflow.models.resource_list_of_task import ResourceListOfTask
+from lusid_workflow.models.result_field import ResultField
+from lusid_workflow.models.result_matching_pattern import ResultMatchingPattern
+from lusid_workflow.models.resultant_child_task_configuration import ResultantChildTaskConfiguration
+from lusid_workflow.models.run_worker_action import RunWorkerAction
+from lusid_workflow.models.run_worker_request import RunWorkerRequest
+from lusid_workflow.models.run_worker_response import RunWorkerResponse
 from lusid_workflow.models.task import Task
 from lusid_workflow.models.task_definition import TaskDefinition
 from lusid_workflow.models.task_definition_version import TaskDefinitionVersion
 from lusid_workflow.models.task_field_definition import TaskFieldDefinition
 from lusid_workflow.models.task_instance_field import TaskInstanceField
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
+from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
-from lusid_workflow.models.update_task_response import UpdateTaskResponse
 from lusid_workflow.models.version import Version
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
+from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_task_definition_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -42,84 +42,89 @@
         'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
         'states': 'list[TaskStateDefinition]',
         'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
         'triggers': 'list[TransitionTriggerDefinition]',
-        'transitions': 'list[TaskTransitionDefinition]'
+        'transitions': 'list[TaskTransitionDefinition]',
+        'actions': 'list[ActionDefinition]'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
         'states': 'states',
         'field_schema': 'fieldSchema',
         'initial_state': 'initialState',
         'triggers': 'triggers',
-        'transitions': 'transitions'
+        'transitions': 'transitions',
+        'actions': 'actions'
     }
 
     required_map = {
-        'id': 'optional',
-        'display_name': 'optional',
+        'id': 'required',
+        'display_name': 'required',
         'description': 'optional',
-        'states': 'optional',
+        'states': 'required',
         'field_schema': 'optional',
-        'initial_state': 'optional',
+        'initial_state': 'required',
         'triggers': 'optional',
-        'transitions': 'optional'
+        'transitions': 'optional',
+        'actions': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, actions=None, local_vars_configuration=None):  # noqa: E501
         """CreateTaskDefinitionRequest - a model defined in OpenAPI"
         
-        :param id: 
+        :param id:  (required)
         :type id: lusid_workflow.ResourceId
-        :param display_name:  Human readable name
+        :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param states:  The states this Task Definition operates over
+        :param states:  The states this Task Definition operates over (required)
         :type states: list[lusid_workflow.TaskStateDefinition]
         :param field_schema:  Defines the fields associated with this Task
         :type field_schema: list[lusid_workflow.TaskFieldDefinition]
-        :param initial_state: 
+        :param initial_state:  (required)
         :type initial_state: lusid_workflow.InitialState
         :param triggers:  Triggers
         :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         :param transitions:  Transitions
         :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        :param actions:  Actions
+        :type actions: list[lusid_workflow.ActionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._display_name = None
         self._description = None
         self._states = None
         self._field_schema = None
         self._initial_state = None
         self._triggers = None
         self._transitions = None
+        self._actions = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
+        self.id = id
         self.display_name = display_name
         self.description = description
         self.states = states
         self.field_schema = field_schema
-        if initial_state is not None:
-            self.initial_state = initial_state
+        self.initial_state = initial_state
         self.triggers = triggers
         self.transitions = transitions
+        self.actions = actions
 
     @property
     def id(self):
         """Gets the id of this CreateTaskDefinitionRequest.  # noqa: E501
 
 
         :return: The id of this CreateTaskDefinitionRequest.  # noqa: E501
@@ -131,14 +136,16 @@
     def id(self, id):
         """Sets the id of this CreateTaskDefinitionRequest.
 
 
         :param id: The id of this CreateTaskDefinitionRequest.  # noqa: E501
         :type id: lusid_workflow.ResourceId
         """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def display_name(self):
         """Gets the display_name of this CreateTaskDefinitionRequest.  # noqa: E501
 
@@ -154,14 +161,19 @@
         """Sets the display_name of this CreateTaskDefinitionRequest.
 
         Human readable name  # noqa: E501
 
         :param display_name: The display_name of this CreateTaskDefinitionRequest.  # noqa: E501
         :type display_name: str
         """
+        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                display_name is not None and len(display_name) < 1):
+            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
         """Gets the description of this CreateTaskDefinitionRequest.  # noqa: E501
 
@@ -200,14 +212,19 @@
         """Sets the states of this CreateTaskDefinitionRequest.
 
         The states this Task Definition operates over  # noqa: E501
 
         :param states: The states of this CreateTaskDefinitionRequest.  # noqa: E501
         :type states: list[lusid_workflow.TaskStateDefinition]
         """
+        if self.local_vars_configuration.client_side_validation and states is None:  # noqa: E501
+            raise ValueError("Invalid value for `states`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                states is not None and len(states) < 1):
+            raise ValueError("Invalid value for `states`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._states = states
 
     @property
     def field_schema(self):
         """Gets the field_schema of this CreateTaskDefinitionRequest.  # noqa: E501
 
@@ -244,14 +261,16 @@
     def initial_state(self, initial_state):
         """Sets the initial_state of this CreateTaskDefinitionRequest.
 
 
         :param initial_state: The initial_state of this CreateTaskDefinitionRequest.  # noqa: E501
         :type initial_state: lusid_workflow.InitialState
         """
+        if self.local_vars_configuration.client_side_validation and initial_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `initial_state`, must not be `None`")  # noqa: E501
 
         self._initial_state = initial_state
 
     @property
     def triggers(self):
         """Gets the triggers of this CreateTaskDefinitionRequest.  # noqa: E501
 
@@ -293,14 +312,37 @@
 
         :param transitions: The transitions of this CreateTaskDefinitionRequest.  # noqa: E501
         :type transitions: list[lusid_workflow.TaskTransitionDefinition]
         """
 
         self._transitions = transitions
 
+    @property
+    def actions(self):
+        """Gets the actions of this CreateTaskDefinitionRequest.  # noqa: E501
+
+        Actions  # noqa: E501
+
+        :return: The actions of this CreateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.ActionDefinition]
+        """
+        return self._actions
+
+    @actions.setter
+    def actions(self, actions):
+        """Sets the actions of this CreateTaskDefinitionRequest.
+
+        Actions  # noqa: E501
+
+        :param actions: The actions of this CreateTaskDefinitionRequest.  # noqa: E501
+        :type actions: list[lusid_workflow.ActionDefinition]
+        """
+
+        self._actions = actions
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_task_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/deleted_entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class ResourceListOfTaskDefinition(object):
+class PagedResourceListOfTaskDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,176 +35,176 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'next_page': 'str',
+        'previous_page': 'str',
         'values': 'list[TaskDefinition]',
         'href': 'str',
-        'links': 'list[Link]',
-        'next_page': 'str',
-        'previous_page': 'str'
+        'links': 'list[Link]'
     }
 
     attribute_map = {
+        'next_page': 'nextPage',
+        'previous_page': 'previousPage',
         'values': 'values',
         'href': 'href',
-        'links': 'links',
-        'next_page': 'nextPage',
-        'previous_page': 'previousPage'
+        'links': 'links'
     }
 
     required_map = {
+        'next_page': 'optional',
+        'previous_page': 'optional',
         'values': 'required',
         'href': 'optional',
-        'links': 'optional',
-        'next_page': 'optional',
-        'previous_page': 'optional'
+        'links': 'optional'
     }
 
-    def __init__(self, values=None, href=None, links=None, next_page=None, previous_page=None, local_vars_configuration=None):  # noqa: E501
-        """ResourceListOfTaskDefinition - a model defined in OpenAPI"
+    def __init__(self, next_page=None, previous_page=None, values=None, href=None, links=None, local_vars_configuration=None):  # noqa: E501
+        """PagedResourceListOfTaskDefinition - a model defined in OpenAPI"
         
+        :param next_page: 
+        :type next_page: str
+        :param previous_page: 
+        :type previous_page: str
         :param values:  (required)
         :type values: list[lusid_workflow.TaskDefinition]
         :param href: 
         :type href: str
         :param links: 
         :type links: list[lusid_workflow.Link]
-        :param next_page: 
-        :type next_page: str
-        :param previous_page: 
-        :type previous_page: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._next_page = None
+        self._previous_page = None
         self._values = None
         self._href = None
         self._links = None
-        self._next_page = None
-        self._previous_page = None
         self.discriminator = None
 
+        self.next_page = next_page
+        self.previous_page = previous_page
         self.values = values
         self.href = href
         self.links = links
-        self.next_page = next_page
-        self.previous_page = previous_page
+
+    @property
+    def next_page(self):
+        """Gets the next_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+
+
+        :return: The next_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+        :rtype: str
+        """
+        return self._next_page
+
+    @next_page.setter
+    def next_page(self, next_page):
+        """Sets the next_page of this PagedResourceListOfTaskDefinition.
+
+
+        :param next_page: The next_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+        :type next_page: str
+        """
+
+        self._next_page = next_page
+
+    @property
+    def previous_page(self):
+        """Gets the previous_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+
+
+        :return: The previous_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+        :rtype: str
+        """
+        return self._previous_page
+
+    @previous_page.setter
+    def previous_page(self, previous_page):
+        """Sets the previous_page of this PagedResourceListOfTaskDefinition.
+
+
+        :param previous_page: The previous_page of this PagedResourceListOfTaskDefinition.  # noqa: E501
+        :type previous_page: str
+        """
+
+        self._previous_page = previous_page
 
     @property
     def values(self):
-        """Gets the values of this ResourceListOfTaskDefinition.  # noqa: E501
+        """Gets the values of this PagedResourceListOfTaskDefinition.  # noqa: E501
 
 
-        :return: The values of this ResourceListOfTaskDefinition.  # noqa: E501
+        :return: The values of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :rtype: list[lusid_workflow.TaskDefinition]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this ResourceListOfTaskDefinition.
+        """Sets the values of this PagedResourceListOfTaskDefinition.
 
 
-        :param values: The values of this ResourceListOfTaskDefinition.  # noqa: E501
+        :param values: The values of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :type values: list[lusid_workflow.TaskDefinition]
         """
         if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
             raise ValueError("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def href(self):
-        """Gets the href of this ResourceListOfTaskDefinition.  # noqa: E501
+        """Gets the href of this PagedResourceListOfTaskDefinition.  # noqa: E501
 
 
-        :return: The href of this ResourceListOfTaskDefinition.  # noqa: E501
+        :return: The href of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
-        """Sets the href of this ResourceListOfTaskDefinition.
+        """Sets the href of this PagedResourceListOfTaskDefinition.
 
 
-        :param href: The href of this ResourceListOfTaskDefinition.  # noqa: E501
+        :param href: The href of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def links(self):
-        """Gets the links of this ResourceListOfTaskDefinition.  # noqa: E501
+        """Gets the links of this PagedResourceListOfTaskDefinition.  # noqa: E501
 
 
-        :return: The links of this ResourceListOfTaskDefinition.  # noqa: E501
+        :return: The links of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :rtype: list[lusid_workflow.Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
-        """Sets the links of this ResourceListOfTaskDefinition.
+        """Sets the links of this PagedResourceListOfTaskDefinition.
 
 
-        :param links: The links of this ResourceListOfTaskDefinition.  # noqa: E501
+        :param links: The links of this PagedResourceListOfTaskDefinition.  # noqa: E501
         :type links: list[lusid_workflow.Link]
         """
 
         self._links = links
 
-    @property
-    def next_page(self):
-        """Gets the next_page of this ResourceListOfTaskDefinition.  # noqa: E501
-
-
-        :return: The next_page of this ResourceListOfTaskDefinition.  # noqa: E501
-        :rtype: str
-        """
-        return self._next_page
-
-    @next_page.setter
-    def next_page(self, next_page):
-        """Sets the next_page of this ResourceListOfTaskDefinition.
-
-
-        :param next_page: The next_page of this ResourceListOfTaskDefinition.  # noqa: E501
-        :type next_page: str
-        """
-
-        self._next_page = next_page
-
-    @property
-    def previous_page(self):
-        """Gets the previous_page of this ResourceListOfTaskDefinition.  # noqa: E501
-
-
-        :return: The previous_page of this ResourceListOfTaskDefinition.  # noqa: E501
-        :rtype: str
-        """
-        return self._previous_page
-
-    @previous_page.setter
-    def previous_page(self, previous_page):
-        """Sets the previous_page of this ResourceListOfTaskDefinition.
-
-
-        :param previous_page: The previous_page of this ResourceListOfTaskDefinition.  # noqa: E501
-        :type previous_page: str
-        """
-
-        self._previous_page = previous_page
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -239,18 +239,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceListOfTaskDefinition):
+        if not isinstance(other, PagedResourceListOfTaskDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ResourceListOfTaskDefinition):
+        if not isinstance(other, PagedResourceListOfTaskDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -59,41 +59,41 @@
         'state': 'state',
         'terminal_state': 'terminalState',
         'as_at_last_transition': 'asAtLastTransition',
         'fields': 'fields'
     }
 
     required_map = {
-        'id': 'optional',
+        'id': 'required',
         'correlation_ids': 'optional',
-        'task_definition_id': 'optional',
-        'task_definition_version': 'optional',
+        'task_definition_id': 'required',
+        'task_definition_version': 'required',
         'version': 'optional',
-        'state': 'optional',
-        'terminal_state': 'optional',
+        'state': 'required',
+        'terminal_state': 'required',
         'as_at_last_transition': 'optional',
         'fields': 'optional'
     }
 
     def __init__(self, id=None, correlation_ids=None, task_definition_id=None, task_definition_version=None, version=None, state=None, terminal_state=None, as_at_last_transition=None, fields=None, local_vars_configuration=None):  # noqa: E501
         """Task - a model defined in OpenAPI"
         
-        :param id:  The unique id for this Task
+        :param id:  The unique id for this Task (required)
         :type id: str
         :param correlation_ids:  User-provided ID used to link entities and tasks
         :type correlation_ids: list[str]
-        :param task_definition_id: 
+        :param task_definition_id:  (required)
         :type task_definition_id: lusid_workflow.ResourceId
-        :param task_definition_version: 
+        :param task_definition_version:  (required)
         :type task_definition_version: lusid_workflow.TaskDefinitionVersion
         :param version: 
         :type version: lusid_workflow.Version
-        :param state:  Current State
+        :param state:  Current State (required)
         :type state: str
-        :param terminal_state:  True if no onward transitions are possible
+        :param terminal_state:  True if no onward transitions are possible (required)
         :type terminal_state: bool
         :param as_at_last_transition:  Last Transition timestamp
         :type as_at_last_transition: datetime
         :param fields:  Fields and their latest values - should correspond with the Task Definition field schema
         :type fields: list[lusid_workflow.TaskInstanceField]
 
         """  # noqa: E501
@@ -108,26 +108,22 @@
         self._version = None
         self._state = None
         self._terminal_state = None
         self._as_at_last_transition = None
         self._fields = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
+        self.id = id
         self.correlation_ids = correlation_ids
-        if task_definition_id is not None:
-            self.task_definition_id = task_definition_id
-        if task_definition_version is not None:
-            self.task_definition_version = task_definition_version
+        self.task_definition_id = task_definition_id
+        self.task_definition_version = task_definition_version
         if version is not None:
             self.version = version
         self.state = state
-        if terminal_state is not None:
-            self.terminal_state = terminal_state
+        self.terminal_state = terminal_state
         self.as_at_last_transition = as_at_last_transition
         self.fields = fields
 
     @property
     def id(self):
         """Gets the id of this Task.  # noqa: E501
 
@@ -143,14 +139,16 @@
         """Sets the id of this Task.
 
         The unique id for this Task  # noqa: E501
 
         :param id: The id of this Task.  # noqa: E501
         :type id: str
         """
+        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def correlation_ids(self):
         """Gets the correlation_ids of this Task.  # noqa: E501
 
@@ -187,14 +185,16 @@
     def task_definition_id(self, task_definition_id):
         """Sets the task_definition_id of this Task.
 
 
         :param task_definition_id: The task_definition_id of this Task.  # noqa: E501
         :type task_definition_id: lusid_workflow.ResourceId
         """
+        if self.local_vars_configuration.client_side_validation and task_definition_id is None:  # noqa: E501
+            raise ValueError("Invalid value for `task_definition_id`, must not be `None`")  # noqa: E501
 
         self._task_definition_id = task_definition_id
 
     @property
     def task_definition_version(self):
         """Gets the task_definition_version of this Task.  # noqa: E501
 
@@ -208,14 +208,16 @@
     def task_definition_version(self, task_definition_version):
         """Sets the task_definition_version of this Task.
 
 
         :param task_definition_version: The task_definition_version of this Task.  # noqa: E501
         :type task_definition_version: lusid_workflow.TaskDefinitionVersion
         """
+        if self.local_vars_configuration.client_side_validation and task_definition_version is None:  # noqa: E501
+            raise ValueError("Invalid value for `task_definition_version`, must not be `None`")  # noqa: E501
 
         self._task_definition_version = task_definition_version
 
     @property
     def version(self):
         """Gets the version of this Task.  # noqa: E501
 
@@ -252,14 +254,19 @@
         """Sets the state of this Task.
 
         Current State  # noqa: E501
 
         :param state: The state of this Task.  # noqa: E501
         :type state: str
         """
+        if self.local_vars_configuration.client_side_validation and state is None:  # noqa: E501
+            raise ValueError("Invalid value for `state`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                state is not None and len(state) < 1):
+            raise ValueError("Invalid value for `state`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._state = state
 
     @property
     def terminal_state(self):
         """Gets the terminal_state of this Task.  # noqa: E501
 
@@ -275,14 +282,16 @@
         """Sets the terminal_state of this Task.
 
         True if no onward transitions are possible  # noqa: E501
 
         :param terminal_state: The terminal_state of this Task.  # noqa: E501
         :type terminal_state: bool
         """
+        if self.local_vars_configuration.client_side_validation and terminal_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `terminal_state`, must not be `None`")  # noqa: E501
 
         self._terminal_state = terminal_state
 
     @property
     def as_at_last_transition(self):
         """Gets the as_at_last_transition of this Task.  # noqa: E501
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/update_task_definition_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskDefinition(object):
+class UpdateTaskDefinitionRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,301 +35,284 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'ResourceId',
-        'version': 'Version',
         'display_name': 'str',
         'description': 'str',
         'states': 'list[TaskStateDefinition]',
         'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
         'triggers': 'list[TransitionTriggerDefinition]',
-        'transitions': 'list[TaskTransitionDefinition]'
+        'transitions': 'list[TaskTransitionDefinition]',
+        'actions': 'list[ActionDefinition]'
     }
 
     attribute_map = {
-        'id': 'id',
-        'version': 'version',
         'display_name': 'displayName',
         'description': 'description',
         'states': 'states',
         'field_schema': 'fieldSchema',
         'initial_state': 'initialState',
         'triggers': 'triggers',
-        'transitions': 'transitions'
+        'transitions': 'transitions',
+        'actions': 'actions'
     }
 
     required_map = {
-        'id': 'optional',
-        'version': 'optional',
-        'display_name': 'optional',
+        'display_name': 'required',
         'description': 'optional',
-        'states': 'optional',
+        'states': 'required',
         'field_schema': 'optional',
-        'initial_state': 'optional',
+        'initial_state': 'required',
         'triggers': 'optional',
-        'transitions': 'optional'
+        'transitions': 'optional',
+        'actions': 'optional'
     }
 
-    def __init__(self, id=None, version=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, local_vars_configuration=None):  # noqa: E501
-        """TaskDefinition - a model defined in OpenAPI"
+    def __init__(self, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, transitions=None, actions=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateTaskDefinitionRequest - a model defined in OpenAPI"
         
-        :param id: 
-        :type id: lusid_workflow.ResourceId
-        :param version: 
-        :type version: lusid_workflow.Version
-        :param display_name:  Human readable name
+        :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
-        :param states:  The states this Task Definition operates over
+        :param states:  The states this Task Definition operates over (required)
         :type states: list[lusid_workflow.TaskStateDefinition]
-        :param field_schema:  The Fields that this Task Definition operates on
+        :param field_schema:  Defines the fields associated with this Task
         :type field_schema: list[lusid_workflow.TaskFieldDefinition]
-        :param initial_state: 
+        :param initial_state:  (required)
         :type initial_state: lusid_workflow.InitialState
-        :param triggers:  The Triggers for State transition
+        :param triggers:  Triggers
         :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
-        :param transitions:  The Transitions between States
+        :param transitions:  Transitions
         :type transitions: list[lusid_workflow.TaskTransitionDefinition]
+        :param actions:  Actions
+        :type actions: list[lusid_workflow.ActionDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
-        self._version = None
         self._display_name = None
         self._description = None
         self._states = None
         self._field_schema = None
         self._initial_state = None
         self._triggers = None
         self._transitions = None
+        self._actions = None
         self.discriminator = None
 
-        if id is not None:
-            self.id = id
-        if version is not None:
-            self.version = version
         self.display_name = display_name
         self.description = description
         self.states = states
         self.field_schema = field_schema
-        if initial_state is not None:
-            self.initial_state = initial_state
+        self.initial_state = initial_state
         self.triggers = triggers
         self.transitions = transitions
-
-    @property
-    def id(self):
-        """Gets the id of this TaskDefinition.  # noqa: E501
-
-
-        :return: The id of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """Sets the id of this TaskDefinition.
-
-
-        :param id: The id of this TaskDefinition.  # noqa: E501
-        :type id: lusid_workflow.ResourceId
-        """
-
-        self._id = id
-
-    @property
-    def version(self):
-        """Gets the version of this TaskDefinition.  # noqa: E501
-
-
-        :return: The version of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.Version
-        """
-        return self._version
-
-    @version.setter
-    def version(self, version):
-        """Sets the version of this TaskDefinition.
-
-
-        :param version: The version of this TaskDefinition.  # noqa: E501
-        :type version: lusid_workflow.Version
-        """
-
-        self._version = version
+        self.actions = actions
 
     @property
     def display_name(self):
-        """Gets the display_name of this TaskDefinition.  # noqa: E501
+        """Gets the display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         Human readable name  # noqa: E501
 
-        :return: The display_name of this TaskDefinition.  # noqa: E501
+        :return: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this TaskDefinition.
+        """Sets the display_name of this UpdateTaskDefinitionRequest.
 
         Human readable name  # noqa: E501
 
-        :param display_name: The display_name of this TaskDefinition.  # noqa: E501
+        :param display_name: The display_name of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type display_name: str
         """
+        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                display_name is not None and len(display_name) < 1):
+            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this TaskDefinition.  # noqa: E501
+        """Gets the description of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         Human readable description  # noqa: E501
 
-        :return: The description of this TaskDefinition.  # noqa: E501
+        :return: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this TaskDefinition.
+        """Sets the description of this UpdateTaskDefinitionRequest.
 
         Human readable description  # noqa: E501
 
-        :param description: The description of this TaskDefinition.  # noqa: E501
+        :param description: The description of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
     def states(self):
-        """Gets the states of this TaskDefinition.  # noqa: E501
+        """Gets the states of this UpdateTaskDefinitionRequest.  # noqa: E501
 
         The states this Task Definition operates over  # noqa: E501
 
-        :return: The states of this TaskDefinition.  # noqa: E501
+        :return: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskStateDefinition]
         """
         return self._states
 
     @states.setter
     def states(self, states):
-        """Sets the states of this TaskDefinition.
+        """Sets the states of this UpdateTaskDefinitionRequest.
 
         The states this Task Definition operates over  # noqa: E501
 
-        :param states: The states of this TaskDefinition.  # noqa: E501
+        :param states: The states of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type states: list[lusid_workflow.TaskStateDefinition]
         """
+        if self.local_vars_configuration.client_side_validation and states is None:  # noqa: E501
+            raise ValueError("Invalid value for `states`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                states is not None and len(states) < 1):
+            raise ValueError("Invalid value for `states`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._states = states
 
     @property
     def field_schema(self):
-        """Gets the field_schema of this TaskDefinition.  # noqa: E501
+        """Gets the field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Fields that this Task Definition operates on  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :return: The field_schema of this TaskDefinition.  # noqa: E501
+        :return: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskFieldDefinition]
         """
         return self._field_schema
 
     @field_schema.setter
     def field_schema(self, field_schema):
-        """Sets the field_schema of this TaskDefinition.
+        """Sets the field_schema of this UpdateTaskDefinitionRequest.
 
-        The Fields that this Task Definition operates on  # noqa: E501
+        Defines the fields associated with this Task  # noqa: E501
 
-        :param field_schema: The field_schema of this TaskDefinition.  # noqa: E501
+        :param field_schema: The field_schema of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type field_schema: list[lusid_workflow.TaskFieldDefinition]
         """
 
         self._field_schema = field_schema
 
     @property
     def initial_state(self):
-        """Gets the initial_state of this TaskDefinition.  # noqa: E501
+        """Gets the initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
 
 
-        :return: The initial_state of this TaskDefinition.  # noqa: E501
+        :return: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: lusid_workflow.InitialState
         """
         return self._initial_state
 
     @initial_state.setter
     def initial_state(self, initial_state):
-        """Sets the initial_state of this TaskDefinition.
+        """Sets the initial_state of this UpdateTaskDefinitionRequest.
 
 
-        :param initial_state: The initial_state of this TaskDefinition.  # noqa: E501
+        :param initial_state: The initial_state of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type initial_state: lusid_workflow.InitialState
         """
+        if self.local_vars_configuration.client_side_validation and initial_state is None:  # noqa: E501
+            raise ValueError("Invalid value for `initial_state`, must not be `None`")  # noqa: E501
 
         self._initial_state = initial_state
 
     @property
     def triggers(self):
-        """Gets the triggers of this TaskDefinition.  # noqa: E501
+        """Gets the triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Triggers for State transition  # noqa: E501
+        Triggers  # noqa: E501
 
-        :return: The triggers of this TaskDefinition.  # noqa: E501
+        :return: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TransitionTriggerDefinition]
         """
         return self._triggers
 
     @triggers.setter
     def triggers(self, triggers):
-        """Sets the triggers of this TaskDefinition.
+        """Sets the triggers of this UpdateTaskDefinitionRequest.
 
-        The Triggers for State transition  # noqa: E501
+        Triggers  # noqa: E501
 
-        :param triggers: The triggers of this TaskDefinition.  # noqa: E501
+        :param triggers: The triggers of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type triggers: list[lusid_workflow.TransitionTriggerDefinition]
         """
 
         self._triggers = triggers
 
     @property
     def transitions(self):
-        """Gets the transitions of this TaskDefinition.  # noqa: E501
+        """Gets the transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
 
-        The Transitions between States  # noqa: E501
+        Transitions  # noqa: E501
 
-        :return: The transitions of this TaskDefinition.  # noqa: E501
+        :return: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskTransitionDefinition]
         """
         return self._transitions
 
     @transitions.setter
     def transitions(self, transitions):
-        """Sets the transitions of this TaskDefinition.
+        """Sets the transitions of this UpdateTaskDefinitionRequest.
 
-        The Transitions between States  # noqa: E501
+        Transitions  # noqa: E501
 
-        :param transitions: The transitions of this TaskDefinition.  # noqa: E501
+        :param transitions: The transitions of this UpdateTaskDefinitionRequest.  # noqa: E501
         :type transitions: list[lusid_workflow.TaskTransitionDefinition]
         """
 
         self._transitions = transitions
 
+    @property
+    def actions(self):
+        """Gets the actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+
+        Actions  # noqa: E501
+
+        :return: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.ActionDefinition]
+        """
+        return self._actions
+
+    @actions.setter
+    def actions(self, actions):
+        """Sets the actions of this UpdateTaskDefinitionRequest.
+
+        Actions  # noqa: E501
+
+        :param actions: The actions of this UpdateTaskDefinitionRequest.  # noqa: E501
+        :type actions: list[lusid_workflow.ActionDefinition]
+        """
+
+        self._actions = actions
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -364,18 +347,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskDefinition):
+        if not isinstance(other, UpdateTaskDefinitionRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskDefinition):
+        if not isinstance(other, UpdateTaskDefinitionRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_definition_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_state_definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskFieldDefinition(object):
+class TaskStateDefinition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,94 +35,75 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'name': 'str',
-        'type': 'str'
+        'name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'type': 'type'
+        'name': 'name'
     }
 
     required_map = {
-        'name': 'optional',
-        'type': 'optional'
+        'name': 'required'
     }
 
-    def __init__(self, name=None, type=None, local_vars_configuration=None):  # noqa: E501
-        """TaskFieldDefinition - a model defined in OpenAPI"
+    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
+        """TaskStateDefinition - a model defined in OpenAPI"
         
-        :param name:  The name of this Field
+        :param name:  The Name of this State (required)
         :type name: str
-        :param type:  The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")
-        :type type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
-        self._type = None
         self.discriminator = None
 
         self.name = name
-        self.type = type
 
     @property
     def name(self):
-        """Gets the name of this TaskFieldDefinition.  # noqa: E501
+        """Gets the name of this TaskStateDefinition.  # noqa: E501
 
-        The name of this Field  # noqa: E501
+        The Name of this State  # noqa: E501
 
-        :return: The name of this TaskFieldDefinition.  # noqa: E501
+        :return: The name of this TaskStateDefinition.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this TaskFieldDefinition.
+        """Sets the name of this TaskStateDefinition.
 
-        The name of this Field  # noqa: E501
+        The Name of this State  # noqa: E501
 
-        :param name: The name of this TaskFieldDefinition.  # noqa: E501
+        :param name: The name of this TaskStateDefinition.  # noqa: E501
         :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 1024):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._name = name
 
-    @property
-    def type(self):
-        """Gets the type of this TaskFieldDefinition.  # noqa: E501
-
-        The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")  # noqa: E501
-
-        :return: The type of this TaskFieldDefinition.  # noqa: E501
-        :rtype: str
-        """
-        return self._type
-
-    @type.setter
-    def type(self, type):
-        """Sets the type of this TaskFieldDefinition.
-
-        The value type for the field. Available values are: \"String\", \"Decimal\", \"DateTime\", \"Boolean\")  # noqa: E501
-
-        :param type: The type of this TaskFieldDefinition.  # noqa: E501
-        :type type: str
-        """
-
-        self._type = type
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -157,18 +138,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskFieldDefinition):
+        if not isinstance(other, TaskStateDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskFieldDefinition):
+        if not isinstance(other, TaskStateDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/task_instance_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -46,23 +46,23 @@
     attribute_map = {
         'name': 'name',
         'value': 'value'
     }
 
     required_map = {
         'name': 'required',
-        'value': 'required'
+        'value': 'optional'
     }
 
     def __init__(self, name=None, value=None, local_vars_configuration=None):  # noqa: E501
         """TaskInstanceField - a model defined in OpenAPI"
         
         :param name:  The name of this Field (required)
         :type name: str
-        :param value:  The value of this Field (required)
+        :param value:  The value of this Field
         :type value: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
@@ -91,14 +91,17 @@
         The name of this Field  # noqa: E501
 
         :param name: The name of this TaskInstanceField.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def value(self):
         """Gets the value of this TaskInstanceField.  # noqa: E501
 
@@ -114,16 +117,14 @@
         """Sets the value of this TaskInstanceField.
 
         The value of this Field  # noqa: E501
 
         :param value: The value of this TaskInstanceField.  # noqa: E501
         :type value: str
         """
-        if self.local_vars_configuration.client_side_validation and value is None:  # noqa: E501
-            raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
 
         self._value = value
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/run_worker_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskStateDefinition(object):
+class RunWorkerRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,63 +35,65 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'name': 'str'
+        'parameters': 'list[ParameterValue]'
     }
 
     attribute_map = {
-        'name': 'name'
+        'parameters': 'parameters'
     }
 
     required_map = {
-        'name': 'optional'
+        'parameters': 'required'
     }
 
-    def __init__(self, name=None, local_vars_configuration=None):  # noqa: E501
-        """TaskStateDefinition - a model defined in OpenAPI"
+    def __init__(self, parameters=None, local_vars_configuration=None):  # noqa: E501
+        """RunWorkerRequest - a model defined in OpenAPI"
         
-        :param name:  The Name of this State
-        :type name: str
+        :param parameters:  The Parameter and their values. (required)
+        :type parameters: list[lusid_workflow.ParameterValue]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
+        self._parameters = None
         self.discriminator = None
 
-        self.name = name
+        self.parameters = parameters
 
     @property
-    def name(self):
-        """Gets the name of this TaskStateDefinition.  # noqa: E501
+    def parameters(self):
+        """Gets the parameters of this RunWorkerRequest.  # noqa: E501
 
-        The Name of this State  # noqa: E501
+        The Parameter and their values.  # noqa: E501
 
-        :return: The name of this TaskStateDefinition.  # noqa: E501
-        :rtype: str
+        :return: The parameters of this RunWorkerRequest.  # noqa: E501
+        :rtype: list[lusid_workflow.ParameterValue]
         """
-        return self._name
+        return self._parameters
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this TaskStateDefinition.
+    @parameters.setter
+    def parameters(self, parameters):
+        """Sets the parameters of this RunWorkerRequest.
 
-        The Name of this State  # noqa: E501
+        The Parameter and their values.  # noqa: E501
 
-        :param name: The name of this TaskStateDefinition.  # noqa: E501
-        :type name: str
+        :param parameters: The parameters of this RunWorkerRequest.  # noqa: E501
+        :type parameters: list[lusid_workflow.ParameterValue]
         """
+        if self.local_vars_configuration.client_side_validation and parameters is None:  # noqa: E501
+            raise ValueError("Invalid value for `parameters`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._parameters = parameters
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -127,18 +129,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskStateDefinition):
+        if not isinstance(other, RunWorkerRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskStateDefinition):
+        if not isinstance(other, RunWorkerRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/resource_list_of_task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class TaskTransitionDefinition(object):
+class ResourceListOfTask(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,153 +35,175 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'from_state': 'str',
-        'to_state': 'str',
-        'trigger': 'str',
-        'guard': 'str'
+        'values': 'list[Task]',
+        'href': 'str',
+        'links': 'list[Link]',
+        'next_page': 'str',
+        'previous_page': 'str'
     }
 
     attribute_map = {
-        'from_state': 'fromState',
-        'to_state': 'toState',
-        'trigger': 'trigger',
-        'guard': 'guard'
+        'values': 'values',
+        'href': 'href',
+        'links': 'links',
+        'next_page': 'nextPage',
+        'previous_page': 'previousPage'
     }
 
     required_map = {
-        'from_state': 'optional',
-        'to_state': 'optional',
-        'trigger': 'optional',
-        'guard': 'optional'
+        'values': 'required',
+        'href': 'optional',
+        'links': 'optional',
+        'next_page': 'optional',
+        'previous_page': 'optional'
     }
 
-    def __init__(self, from_state=None, to_state=None, trigger=None, guard=None, local_vars_configuration=None):  # noqa: E501
-        """TaskTransitionDefinition - a model defined in OpenAPI"
+    def __init__(self, values=None, href=None, links=None, next_page=None, previous_page=None, local_vars_configuration=None):  # noqa: E501
+        """ResourceListOfTask - a model defined in OpenAPI"
         
-        :param from_state:  The State this Transition if coming From
-        :type from_state: str
-        :param to_state:  The State this Transition is going To
-        :type to_state: str
-        :param trigger:  The Trigger for this Transition
-        :type trigger: str
-        :param guard:  The Guard for this Transition, if any
-        :type guard: str
+        :param values:  (required)
+        :type values: list[lusid_workflow.Task]
+        :param href: 
+        :type href: str
+        :param links: 
+        :type links: list[lusid_workflow.Link]
+        :param next_page: 
+        :type next_page: str
+        :param previous_page: 
+        :type previous_page: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._from_state = None
-        self._to_state = None
-        self._trigger = None
-        self._guard = None
+        self._values = None
+        self._href = None
+        self._links = None
+        self._next_page = None
+        self._previous_page = None
         self.discriminator = None
 
-        self.from_state = from_state
-        self.to_state = to_state
-        self.trigger = trigger
-        self.guard = guard
+        self.values = values
+        self.href = href
+        self.links = links
+        self.next_page = next_page
+        self.previous_page = previous_page
 
     @property
-    def from_state(self):
-        """Gets the from_state of this TaskTransitionDefinition.  # noqa: E501
+    def values(self):
+        """Gets the values of this ResourceListOfTask.  # noqa: E501
 
-        The State this Transition if coming From  # noqa: E501
 
-        :return: The from_state of this TaskTransitionDefinition.  # noqa: E501
-        :rtype: str
+        :return: The values of this ResourceListOfTask.  # noqa: E501
+        :rtype: list[lusid_workflow.Task]
         """
-        return self._from_state
+        return self._values
 
-    @from_state.setter
-    def from_state(self, from_state):
-        """Sets the from_state of this TaskTransitionDefinition.
+    @values.setter
+    def values(self, values):
+        """Sets the values of this ResourceListOfTask.
 
-        The State this Transition if coming From  # noqa: E501
 
-        :param from_state: The from_state of this TaskTransitionDefinition.  # noqa: E501
-        :type from_state: str
+        :param values: The values of this ResourceListOfTask.  # noqa: E501
+        :type values: list[lusid_workflow.Task]
         """
+        if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
+            raise ValueError("Invalid value for `values`, must not be `None`")  # noqa: E501
 
-        self._from_state = from_state
+        self._values = values
 
     @property
-    def to_state(self):
-        """Gets the to_state of this TaskTransitionDefinition.  # noqa: E501
+    def href(self):
+        """Gets the href of this ResourceListOfTask.  # noqa: E501
 
-        The State this Transition is going To  # noqa: E501
 
-        :return: The to_state of this TaskTransitionDefinition.  # noqa: E501
+        :return: The href of this ResourceListOfTask.  # noqa: E501
         :rtype: str
         """
-        return self._to_state
+        return self._href
+
+    @href.setter
+    def href(self, href):
+        """Sets the href of this ResourceListOfTask.
+
+
+        :param href: The href of this ResourceListOfTask.  # noqa: E501
+        :type href: str
+        """
+
+        self._href = href
+
+    @property
+    def links(self):
+        """Gets the links of this ResourceListOfTask.  # noqa: E501
+
+
+        :return: The links of this ResourceListOfTask.  # noqa: E501
+        :rtype: list[lusid_workflow.Link]
+        """
+        return self._links
 
-    @to_state.setter
-    def to_state(self, to_state):
-        """Sets the to_state of this TaskTransitionDefinition.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this ResourceListOfTask.
 
-        The State this Transition is going To  # noqa: E501
 
-        :param to_state: The to_state of this TaskTransitionDefinition.  # noqa: E501
-        :type to_state: str
+        :param links: The links of this ResourceListOfTask.  # noqa: E501
+        :type links: list[lusid_workflow.Link]
         """
 
-        self._to_state = to_state
+        self._links = links
 
     @property
-    def trigger(self):
-        """Gets the trigger of this TaskTransitionDefinition.  # noqa: E501
+    def next_page(self):
+        """Gets the next_page of this ResourceListOfTask.  # noqa: E501
 
-        The Trigger for this Transition  # noqa: E501
 
-        :return: The trigger of this TaskTransitionDefinition.  # noqa: E501
+        :return: The next_page of this ResourceListOfTask.  # noqa: E501
         :rtype: str
         """
-        return self._trigger
+        return self._next_page
 
-    @trigger.setter
-    def trigger(self, trigger):
-        """Sets the trigger of this TaskTransitionDefinition.
+    @next_page.setter
+    def next_page(self, next_page):
+        """Sets the next_page of this ResourceListOfTask.
 
-        The Trigger for this Transition  # noqa: E501
 
-        :param trigger: The trigger of this TaskTransitionDefinition.  # noqa: E501
-        :type trigger: str
+        :param next_page: The next_page of this ResourceListOfTask.  # noqa: E501
+        :type next_page: str
         """
 
-        self._trigger = trigger
+        self._next_page = next_page
 
     @property
-    def guard(self):
-        """Gets the guard of this TaskTransitionDefinition.  # noqa: E501
+    def previous_page(self):
+        """Gets the previous_page of this ResourceListOfTask.  # noqa: E501
 
-        The Guard for this Transition, if any  # noqa: E501
 
-        :return: The guard of this TaskTransitionDefinition.  # noqa: E501
+        :return: The previous_page of this ResourceListOfTask.  # noqa: E501
         :rtype: str
         """
-        return self._guard
+        return self._previous_page
 
-    @guard.setter
-    def guard(self, guard):
-        """Sets the guard of this TaskTransitionDefinition.
+    @previous_page.setter
+    def previous_page(self, previous_page):
+        """Sets the previous_page of this ResourceListOfTask.
 
-        The Guard for this Transition, if any  # noqa: E501
 
-        :param guard: The guard of this TaskTransitionDefinition.  # noqa: E501
-        :type guard: str
+        :param previous_page: The previous_page of this ResourceListOfTask.  # noqa: E501
+        :type previous_page: str
         """
 
-        self._guard = guard
+        self._previous_page = previous_page
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -217,18 +239,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TaskTransitionDefinition):
+        if not isinstance(other, ResourceListOfTask):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TaskTransitionDefinition):
+        if not isinstance(other, ResourceListOfTask):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -45,38 +45,37 @@
 
     attribute_map = {
         'name': 'name',
         'trigger': 'trigger'
     }
 
     required_map = {
-        'name': 'optional',
-        'trigger': 'optional'
+        'name': 'required',
+        'trigger': 'required'
     }
 
     def __init__(self, name=None, trigger=None, local_vars_configuration=None):  # noqa: E501
         """TransitionTriggerDefinition - a model defined in OpenAPI"
         
-        :param name:  The key/Name of this Trigger
+        :param name:  The key/Name of this Trigger (required)
         :type name: str
-        :param trigger: 
+        :param trigger:  (required)
         :type trigger: lusid_workflow.TriggerSchema
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._trigger = None
         self.discriminator = None
 
         self.name = name
-        if trigger is not None:
-            self.trigger = trigger
+        self.trigger = trigger
 
     @property
     def name(self):
         """Gets the name of this TransitionTriggerDefinition.  # noqa: E501
 
         The key/Name of this Trigger  # noqa: E501
 
@@ -90,14 +89,25 @@
         """Sets the name of this TransitionTriggerDefinition.
 
         The key/Name of this Trigger  # noqa: E501
 
         :param name: The name of this TransitionTriggerDefinition.  # noqa: E501
         :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) > 1024):
+            raise ValueError("Invalid value for `name`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def trigger(self):
         """Gets the trigger of this TransitionTriggerDefinition.  # noqa: E501
 
@@ -111,14 +121,16 @@
     def trigger(self, trigger):
         """Sets the trigger of this TransitionTriggerDefinition.
 
 
         :param trigger: The trigger of this TransitionTriggerDefinition.  # noqa: E501
         :type trigger: lusid_workflow.TriggerSchema
         """
+        if self.local_vars_configuration.client_side_validation and trigger is None:  # noqa: E501
+            raise ValueError("Invalid value for `trigger`, must not be `None`")  # noqa: E501
 
         self._trigger = trigger
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/trigger_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -43,21 +43,21 @@
     }
 
     attribute_map = {
         'type': 'type'
     }
 
     required_map = {
-        'type': 'optional'
+        'type': 'required'
     }
 
     def __init__(self, type=None, local_vars_configuration=None):  # noqa: E501
         """TriggerSchema - a model defined in OpenAPI"
         
-        :param type:  The type of Trigger
+        :param type:  The type of Trigger; available value(s): External (required)
         :type type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
@@ -66,30 +66,35 @@
 
         self.type = type
 
     @property
     def type(self):
         """Gets the type of this TriggerSchema.  # noqa: E501
 
-        The type of Trigger  # noqa: E501
+        The type of Trigger; available value(s): External  # noqa: E501
 
         :return: The type of this TriggerSchema.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this TriggerSchema.
 
-        The type of Trigger  # noqa: E501
+        The type of Trigger; available value(s): External  # noqa: E501
 
         :param type: The type of this TriggerSchema.  # noqa: E501
         :type type: str
         """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._type = type
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/update_task_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,42 +35,72 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'correlation_ids': 'list[str]',
         'fields': 'list[TaskInstanceField]'
     }
 
     attribute_map = {
+        'correlation_ids': 'correlationIds',
         'fields': 'fields'
     }
 
     required_map = {
+        'correlation_ids': 'optional',
         'fields': 'optional'
     }
 
-    def __init__(self, fields=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, correlation_ids=None, fields=None, local_vars_configuration=None):  # noqa: E501
         """UpdateTaskRequest - a model defined in OpenAPI"
         
+        :param correlation_ids:  A set of guid identifiers that allow correlation across the application tier
+        :type correlation_ids: list[str]
         :param fields:  Defines the fields associated with the update
         :type fields: list[lusid_workflow.TaskInstanceField]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._correlation_ids = None
         self._fields = None
         self.discriminator = None
 
+        self.correlation_ids = correlation_ids
         self.fields = fields
 
     @property
+    def correlation_ids(self):
+        """Gets the correlation_ids of this UpdateTaskRequest.  # noqa: E501
+
+        A set of guid identifiers that allow correlation across the application tier  # noqa: E501
+
+        :return: The correlation_ids of this UpdateTaskRequest.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._correlation_ids
+
+    @correlation_ids.setter
+    def correlation_ids(self, correlation_ids):
+        """Sets the correlation_ids of this UpdateTaskRequest.
+
+        A set of guid identifiers that allow correlation across the application tier  # noqa: E501
+
+        :param correlation_ids: The correlation_ids of this UpdateTaskRequest.  # noqa: E501
+        :type correlation_ids: list[str]
+        """
+
+        self._correlation_ids = correlation_ids
+
+    @property
     def fields(self):
         """Gets the fields of this UpdateTaskRequest.  # noqa: E501
 
         Defines the fields associated with the update  # noqa: E501
 
         :return: The fields of this UpdateTaskRequest.  # noqa: E501
         :rtype: list[lusid_workflow.TaskInstanceField]
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/update_task_response.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class UpdateTaskResponse(object):
+class TriggerParentTaskAction(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,124 +35,112 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'was_successful': 'bool',
-        'as_at': 'datetime',
-        'message': 'str'
+        'type': 'str',
+        'trigger': 'str'
     }
 
     attribute_map = {
-        'was_successful': 'wasSuccessful',
-        'as_at': 'asAt',
-        'message': 'message'
+        'type': 'type',
+        'trigger': 'trigger'
     }
 
     required_map = {
-        'was_successful': 'optional',
-        'as_at': 'optional',
-        'message': 'optional'
+        'type': 'required',
+        'trigger': 'required'
     }
 
-    def __init__(self, was_successful=None, as_at=None, message=None, local_vars_configuration=None):  # noqa: E501
-        """UpdateTaskResponse - a model defined in OpenAPI"
+    def __init__(self, type=None, trigger=None, local_vars_configuration=None):  # noqa: E501
+        """TriggerParentTaskAction - a model defined in OpenAPI"
         
-        :param was_successful:  A flag indicating success
-        :type was_successful: bool
-        :param as_at:  If successful, the AsAt time
-        :type as_at: datetime
-        :param message:  Any messaging
-        :type message: str
+        :param type:  Type name for this Action (required)
+        :type type: str
+        :param trigger:  Trigger on parent task to be invoked (required)
+        :type trigger: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._was_successful = None
-        self._as_at = None
-        self._message = None
+        self._type = None
+        self._trigger = None
         self.discriminator = None
 
-        if was_successful is not None:
-            self.was_successful = was_successful
-        self.as_at = as_at
-        self.message = message
+        self.type = type
+        self.trigger = trigger
 
     @property
-    def was_successful(self):
-        """Gets the was_successful of this UpdateTaskResponse.  # noqa: E501
+    def type(self):
+        """Gets the type of this TriggerParentTaskAction.  # noqa: E501
 
-        A flag indicating success  # noqa: E501
+        Type name for this Action  # noqa: E501
 
-        :return: The was_successful of this UpdateTaskResponse.  # noqa: E501
-        :rtype: bool
-        """
-        return self._was_successful
-
-    @was_successful.setter
-    def was_successful(self, was_successful):
-        """Sets the was_successful of this UpdateTaskResponse.
-
-        A flag indicating success  # noqa: E501
-
-        :param was_successful: The was_successful of this UpdateTaskResponse.  # noqa: E501
-        :type was_successful: bool
-        """
-
-        self._was_successful = was_successful
-
-    @property
-    def as_at(self):
-        """Gets the as_at of this UpdateTaskResponse.  # noqa: E501
-
-        If successful, the AsAt time  # noqa: E501
-
-        :return: The as_at of this UpdateTaskResponse.  # noqa: E501
-        :rtype: datetime
+        :return: The type of this TriggerParentTaskAction.  # noqa: E501
+        :rtype: str
         """
-        return self._as_at
-
-    @as_at.setter
-    def as_at(self, as_at):
-        """Sets the as_at of this UpdateTaskResponse.
-
-        If successful, the AsAt time  # noqa: E501
+        return self._type
 
-        :param as_at: The as_at of this UpdateTaskResponse.  # noqa: E501
-        :type as_at: datetime
-        """
+    @type.setter
+    def type(self, type):
+        """Sets the type of this TriggerParentTaskAction.
+
+        Type name for this Action  # noqa: E501
+
+        :param type: The type of this TriggerParentTaskAction.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["TriggerParentTask"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
-        self._as_at = as_at
+        self._type = type
 
     @property
-    def message(self):
-        """Gets the message of this UpdateTaskResponse.  # noqa: E501
+    def trigger(self):
+        """Gets the trigger of this TriggerParentTaskAction.  # noqa: E501
 
-        Any messaging  # noqa: E501
+        Trigger on parent task to be invoked  # noqa: E501
 
-        :return: The message of this UpdateTaskResponse.  # noqa: E501
+        :return: The trigger of this TriggerParentTaskAction.  # noqa: E501
         :rtype: str
         """
-        return self._message
-
-    @message.setter
-    def message(self, message):
-        """Sets the message of this UpdateTaskResponse.
+        return self._trigger
 
-        Any messaging  # noqa: E501
-
-        :param message: The message of this UpdateTaskResponse.  # noqa: E501
-        :type message: str
-        """
+    @trigger.setter
+    def trigger(self, trigger):
+        """Sets the trigger of this TriggerParentTaskAction.
+
+        Trigger on parent task to be invoked  # noqa: E501
+
+        :param trigger: The trigger of this TriggerParentTaskAction.  # noqa: E501
+        :type trigger: str
+        """
+        if self.local_vars_configuration.client_side_validation and trigger is None:  # noqa: E501
+            raise ValueError("Invalid value for `trigger`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                trigger is not None and len(trigger) > 1024):
+            raise ValueError("Invalid value for `trigger`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                trigger is not None and len(trigger) < 1):
+            raise ValueError("Invalid value for `trigger`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                trigger is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', trigger)):  # noqa: E501
+            raise ValueError(r"Invalid value for `trigger`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
-        self._message = message
+        self._trigger = trigger
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -188,18 +176,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateTaskResponse):
+        if not isinstance(other, TriggerParentTaskAction):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UpdateTaskResponse):
+        if not isinstance(other, TriggerParentTaskAction):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/result_field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class Worker(object):
+class ResultField(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,216 +35,164 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'ResourceId',
+        'name': 'str',
+        'type': 'str',
         'display_name': 'str',
-        'description': 'str',
-        'worker_configuration': 'WorkerConfiguration',
-        'version': 'Version',
-        'links': 'list[Link]'
+        'description': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
+        'name': 'name',
+        'type': 'type',
         'display_name': 'displayName',
-        'description': 'description',
-        'worker_configuration': 'workerConfiguration',
-        'version': 'version',
-        'links': 'links'
+        'description': 'description'
     }
 
     required_map = {
-        'id': 'required',
-        'display_name': 'required',
-        'description': 'optional',
-        'worker_configuration': 'required',
-        'version': 'optional',
-        'links': 'optional'
+        'name': 'required',
+        'type': 'required',
+        'display_name': 'optional',
+        'description': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, worker_configuration=None, version=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """Worker - a model defined in OpenAPI"
+    def __init__(self, name=None, type=None, display_name=None, description=None, local_vars_configuration=None):  # noqa: E501
+        """ResultField - a model defined in OpenAPI"
         
-        :param id:  (required)
-        :type id: lusid_workflow.ResourceId
-        :param display_name:  Human readable name (required)
+        :param name:  Name (required)
+        :type name: str
+        :param type:  The type of this Parameter (required)
+        :type type: str
+        :param display_name:  DisplayName
         :type display_name: str
-        :param description:  Human readable description
+        :param description:  Description
         :type description: str
-        :param worker_configuration:  (required)
-        :type worker_configuration: lusid_workflow.WorkerConfiguration
-        :param version: 
-        :type version: lusid_workflow.Version
-        :param links: 
-        :type links: list[lusid_workflow.Link]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._id = None
+        self._name = None
+        self._type = None
         self._display_name = None
         self._description = None
-        self._worker_configuration = None
-        self._version = None
-        self._links = None
         self.discriminator = None
 
-        self.id = id
+        self.name = name
+        self.type = type
         self.display_name = display_name
         self.description = description
-        self.worker_configuration = worker_configuration
-        if version is not None:
-            self.version = version
-        self.links = links
 
     @property
-    def id(self):
-        """Gets the id of this Worker.  # noqa: E501
+    def name(self):
+        """Gets the name of this ResultField.  # noqa: E501
 
+        Name  # noqa: E501
 
-        :return: The id of this Worker.  # noqa: E501
-        :rtype: lusid_workflow.ResourceId
+        :return: The name of this ResultField.  # noqa: E501
+        :rtype: str
         """
-        return self._id
+        return self._name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this Worker.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ResultField.
 
+        Name  # noqa: E501
 
-        :param id: The id of this Worker.  # noqa: E501
-        :type id: lusid_workflow.ResourceId
+        :param name: The name of this ResultField.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._id = id
+        self._name = name
+
+    @property
+    def type(self):
+        """Gets the type of this ResultField.  # noqa: E501
+
+        The type of this Parameter  # noqa: E501
+
+        :return: The type of this ResultField.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ResultField.
+
+        The type of this Parameter  # noqa: E501
+
+        :param type: The type of this ResultField.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
 
     @property
     def display_name(self):
-        """Gets the display_name of this Worker.  # noqa: E501
+        """Gets the display_name of this ResultField.  # noqa: E501
 
-        Human readable name  # noqa: E501
+        DisplayName  # noqa: E501
 
-        :return: The display_name of this Worker.  # noqa: E501
+        :return: The display_name of this ResultField.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this Worker.
+        """Sets the display_name of this ResultField.
 
-        Human readable name  # noqa: E501
+        DisplayName  # noqa: E501
 
-        :param display_name: The display_name of this Worker.  # noqa: E501
+        :param display_name: The display_name of this ResultField.  # noqa: E501
         :type display_name: str
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def description(self):
-        """Gets the description of this Worker.  # noqa: E501
+        """Gets the description of this ResultField.  # noqa: E501
 
-        Human readable description  # noqa: E501
+        Description  # noqa: E501
 
-        :return: The description of this Worker.  # noqa: E501
+        :return: The description of this ResultField.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this Worker.
+        """Sets the description of this ResultField.
 
-        Human readable description  # noqa: E501
+        Description  # noqa: E501
 
-        :param description: The description of this Worker.  # noqa: E501
+        :param description: The description of this ResultField.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
-    @property
-    def worker_configuration(self):
-        """Gets the worker_configuration of this Worker.  # noqa: E501
-
-
-        :return: The worker_configuration of this Worker.  # noqa: E501
-        :rtype: lusid_workflow.WorkerConfiguration
-        """
-        return self._worker_configuration
-
-    @worker_configuration.setter
-    def worker_configuration(self, worker_configuration):
-        """Sets the worker_configuration of this Worker.
-
-
-        :param worker_configuration: The worker_configuration of this Worker.  # noqa: E501
-        :type worker_configuration: lusid_workflow.WorkerConfiguration
-        """
-        if self.local_vars_configuration.client_side_validation and worker_configuration is None:  # noqa: E501
-            raise ValueError("Invalid value for `worker_configuration`, must not be `None`")  # noqa: E501
-
-        self._worker_configuration = worker_configuration
-
-    @property
-    def version(self):
-        """Gets the version of this Worker.  # noqa: E501
-
-
-        :return: The version of this Worker.  # noqa: E501
-        :rtype: lusid_workflow.Version
-        """
-        return self._version
-
-    @version.setter
-    def version(self, version):
-        """Sets the version of this Worker.
-
-
-        :param version: The version of this Worker.  # noqa: E501
-        :type version: lusid_workflow.Version
-        """
-
-        self._version = version
-
-    @property
-    def links(self):
-        """Gets the links of this Worker.  # noqa: E501
-
-
-        :return: The links of this Worker.  # noqa: E501
-        :rtype: list[lusid_workflow.Link]
-        """
-        return self._links
-
-    @links.setter
-    def links(self, links):
-        """Sets the links of this Worker.
-
-
-        :param links: The links of this Worker.  # noqa: E501
-        :type links: list[lusid_workflow.Link]
-        """
-
-        self._links = links
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -279,18 +227,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Worker):
+        if not isinstance(other, ResultField):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Worker):
+        if not isinstance(other, ResultField):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/models/result_matching_pattern.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class WorkerConfiguration(object):
+class ResultMatchingPattern(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,68 +35,74 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str'
+        'filter': 'str'
     }
 
     attribute_map = {
-        'type': 'type'
+        'filter': 'filter'
     }
 
     required_map = {
-        'type': 'required'
+        'filter': 'required'
     }
 
-    def __init__(self, type=None, local_vars_configuration=None):  # noqa: E501
-        """WorkerConfiguration - a model defined in OpenAPI"
+    def __init__(self, filter=None, local_vars_configuration=None):  # noqa: E501
+        """ResultMatchingPattern - a model defined in OpenAPI"
         
-        :param type:  The type of worker (required)
-        :type type: str
+        :param filter:  Filter string (required)
+        :type filter: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
+        self._filter = None
         self.discriminator = None
 
-        self.type = type
+        self.filter = filter
 
     @property
-    def type(self):
-        """Gets the type of this WorkerConfiguration.  # noqa: E501
+    def filter(self):
+        """Gets the filter of this ResultMatchingPattern.  # noqa: E501
 
-        The type of worker  # noqa: E501
+        Filter string  # noqa: E501
 
-        :return: The type of this WorkerConfiguration.  # noqa: E501
+        :return: The filter of this ResultMatchingPattern.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._filter
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this WorkerConfiguration.
+    @filter.setter
+    def filter(self, filter):
+        """Sets the filter of this ResultMatchingPattern.
 
-        The type of worker  # noqa: E501
+        Filter string  # noqa: E501
 
-        :param type: The type of this WorkerConfiguration.  # noqa: E501
-        :type type: str
+        :param filter: The filter of this ResultMatchingPattern.  # noqa: E501
+        :type filter: str
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and filter is None:  # noqa: E501
+            raise ValueError("Invalid value for `filter`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+                filter is not None and len(filter) > 1024):
+            raise ValueError("Invalid value for `filter`, length must be less than or equal to `1024`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                filter is not None and len(filter) < 1):
+            raise ValueError("Invalid value for `filter`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                filter is not None and not re.search(r'^[\s\S]*$', filter)):  # noqa: E501
+            raise ValueError(r"Invalid value for `filter`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._type = type
+        self._filter = filter
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -132,18 +138,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkerConfiguration):
+        if not isinstance(other, ResultMatchingPattern):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, WorkerConfiguration):
+        if not isinstance(other, ResultMatchingPattern):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.209
+    The version of the OpenAPI document: 0.1.330
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.330/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,37 +8,55 @@
 lusid_workflow/exceptions.py
 lusid_workflow/rest.py
 lusid_workflow/api/__init__.py
 lusid_workflow/api/task_definitions_api.py
 lusid_workflow/api/tasks_api.py
 lusid_workflow/api/workers_api.py
 lusid_workflow/models/__init__.py
+lusid_workflow/models/action_definition.py
+lusid_workflow/models/action_details.py
+lusid_workflow/models/create_child_tasks_action.py
 lusid_workflow/models/create_task_definition_request.py
 lusid_workflow/models/create_task_request.py
 lusid_workflow/models/create_worker_request.py
 lusid_workflow/models/deleted_entity_response.py
+lusid_workflow/models/field_mapping.py
+lusid_workflow/models/health_check.py
 lusid_workflow/models/initial_state.py
 lusid_workflow/models/link.py
+lusid_workflow/models/luminesce_view.py
 lusid_workflow/models/lusid_problem_details.py
 lusid_workflow/models/lusid_validation_problem_details.py
+lusid_workflow/models/paged_resource_list_of_task.py
+lusid_workflow/models/paged_resource_list_of_task_definition.py
+lusid_workflow/models/paged_resource_list_of_worker.py
+lusid_workflow/models/parameter.py
+lusid_workflow/models/parameter_value.py
 lusid_workflow/models/resource_id.py
-lusid_workflow/models/resource_list_of_task_definition.py
+lusid_workflow/models/resource_list_of_task.py
+lusid_workflow/models/result_field.py
+lusid_workflow/models/result_matching_pattern.py
+lusid_workflow/models/resultant_child_task_configuration.py
+lusid_workflow/models/run_worker_action.py
+lusid_workflow/models/run_worker_request.py
+lusid_workflow/models/run_worker_response.py
 lusid_workflow/models/task.py
 lusid_workflow/models/task_definition.py
 lusid_workflow/models/task_definition_version.py
 lusid_workflow/models/task_field_definition.py
 lusid_workflow/models/task_instance_field.py
 lusid_workflow/models/task_state_definition.py
 lusid_workflow/models/task_transition_definition.py
 lusid_workflow/models/transition_trigger_definition.py
+lusid_workflow/models/trigger_parent_task_action.py
 lusid_workflow/models/trigger_schema.py
 lusid_workflow/models/update_task_definition_request.py
 lusid_workflow/models/update_task_request.py
-lusid_workflow/models/update_task_response.py
 lusid_workflow/models/version.py
 lusid_workflow/models/worker.py
 lusid_workflow/models/worker_configuration.py
+lusid_workflow/models/worker_status_triggers.py
 lusid_workflow_sdk_preview.egg-info/PKG-INFO
 lusid_workflow_sdk_preview.egg-info/SOURCES.txt
 lusid_workflow_sdk_preview.egg-info/dependency_links.txt
 lusid_workflow_sdk_preview.egg-info/requires.txt
 lusid_workflow_sdk_preview.egg-info/top_level.txt
```

### Comparing `lusid-workflow-sdk-preview-0.1.209/setup.py` & `lusid-workflow-sdk-preview-0.1.330/setup.py`

 * *Files identical despite different names*

