# Comparing `tmp/foursight_smaht-0.0.0.1b2.tar.gz` & `tmp/foursight_smaht-0.0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.0.0.1b2.tar", max compression
+gzip compressed data, was "foursight_smaht-0.0.0.1b3.tar", max compression
```

## Comparing `foursight_smaht-0.0.0.1b2.tar` & `foursight_smaht-0.0.0.1b3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2023-06-29 16:16:46.829708 foursight_smaht-0.0.0.1b2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-29 16:16:46.830680 foursight_smaht-0.0.0.1b2/chalicelib_smaht/__init__.py
--rw-r--r--   0        0        0     1030 2023-06-30 14:13:49.029298 foursight_smaht-0.0.0.1b2/chalicelib_smaht/app_utils.py
--rw-r--r--   0        0        0      873 2023-06-30 14:21:01.676349 foursight_smaht-0.0.0.1b2/chalicelib_smaht/buckets.py
--rw-r--r--   0        0        0     4805 2023-06-29 16:16:46.831422 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_schedules.py
--rw-r--r--   0        0        0    13354 2023-06-30 14:22:35.139013 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-29 16:16:46.832258 foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-29 16:16:46.832595 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/__init__.py
--rw-r--r--   0        0        0     9652 2023-06-30 14:35:43.119450 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/audit_checks.py
--rw-r--r--   0        0        0     2883 2023-06-30 14:12:30.984804 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-29 16:16:46.833562 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/es_checks.py
--rw-r--r--   0        0        0      262 2023-06-29 16:16:46.833957 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-29 16:16:46.834082 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-29 16:16:46.834353 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-29 16:16:46.834575 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4019 2023-06-30 14:28:16.941473 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/utils.py
--rw-r--r--   0        0        0    39037 2023-06-30 14:29:26.276042 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2572 2023-06-30 14:12:31.026319 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-06-29 16:16:46.836068 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    22581 2023-06-30 14:40:29.435109 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/system_checks.py
--rw-r--r--   0        0        0    59196 2023-06-30 14:41:50.645088 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wfr_checks.py
--rw-r--r--   0        0        0    57441 2023-06-30 14:42:15.050104 foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wrangler_checks.py
--rw-r--r--   0        0        0      773 2023-06-30 14:12:30.981074 foursight_smaht-0.0.0.1b2/chalicelib_smaht/deploy.py
--rw-r--r--   0        0        0      601 2023-06-30 14:23:10.247383 foursight_smaht-0.0.0.1b2/chalicelib_smaht/package.py
--rw-r--r--   0        0        0      253 2023-06-30 16:58:20.012820 foursight_smaht-0.0.0.1b2/chalicelib_smaht/vars.py
--rw-r--r--   0        0        0     1122 2023-06-30 18:28:49.358366 foursight_smaht-0.0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b2/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 16:16:46.829708 foursight_smaht-0.0.0.1b3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-29 16:16:46.830680 foursight_smaht-0.0.0.1b3/chalicelib_smaht/__init__.py
+-rw-r--r--   0        0        0     1030 2023-06-30 14:13:49.029298 foursight_smaht-0.0.0.1b3/chalicelib_smaht/app_utils.py
+-rw-r--r--   0        0        0      873 2023-06-30 14:21:01.676349 foursight_smaht-0.0.0.1b3/chalicelib_smaht/buckets.py
+-rw-r--r--   0        0        0     4805 2023-06-29 16:16:46.831422 foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_schedules.py
+-rw-r--r--   0        0        0    13474 2023-07-05 16:00:20.159155 foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-29 16:16:46.832258 foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-29 16:16:46.832595 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/__init__.py
+-rw-r--r--   0        0        0     9652 2023-06-30 14:35:43.119450 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/audit_checks.py
+-rw-r--r--   0        0        0     2883 2023-06-30 14:12:30.984804 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-29 16:16:46.833562 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/es_checks.py
+-rw-r--r--   0        0        0      262 2023-06-29 16:16:46.833957 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-29 16:16:46.834082 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-29 16:16:46.834353 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-29 16:16:46.834575 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4019 2023-06-30 14:28:16.941473 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39037 2023-06-30 14:29:26.276042 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2572 2023-06-30 14:12:31.026319 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-06-29 16:16:46.836068 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    22581 2023-06-30 14:40:29.435109 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/system_checks.py
+-rw-r--r--   0        0        0    59196 2023-06-30 14:41:50.645088 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/wfr_checks.py
+-rw-r--r--   0        0        0    57441 2023-06-30 14:42:15.050104 foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      773 2023-06-30 14:12:30.981074 foursight_smaht-0.0.0.1b3/chalicelib_smaht/deploy.py
+-rw-r--r--   0        0        0      601 2023-06-30 14:23:10.247383 foursight_smaht-0.0.0.1b3/chalicelib_smaht/package.py
+-rw-r--r--   0        0        0      253 2023-06-30 16:58:20.012820 foursight_smaht-0.0.0.1b3/chalicelib_smaht/vars.py
+-rw-r--r--   0        0        0     1122 2023-07-05 16:00:25.762076 foursight_smaht-0.0.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b3/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 foursight_smaht-0.0.0.1b3/PKG-INFO
```

### Comparing `foursight_smaht-0.0.0.1b2/LICENSE.txt` & `foursight_smaht-0.0.0.1b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/app_utils.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/buckets.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_schedules.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_setup.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8933467741935485%*

 * *Differences: {"'access_key_status'": "{'schedule': {'morning_checks': {replace: OrderedDict([('data', "*

 * *                        "OrderedDict([('kwargs', OrderedDict([('primary', True), ('queue_action', "*

 * *                        "'prod')]))]))])}}, 'display': ['staging']}",*

 * * "'check_deleted_files_lifecycle_status'": "{'schedule': {'hourly_checks': {replace: "*

 * *                                           "OrderedDict([('data', OrderedDict([('kwargs', "*

 * *                                           "OrderedDict([('files_per_run […]*

```diff
@@ -1,453 +1,474 @@
 {
     "access_key_status": {
+        "display": [
+            "staging"
+        ],
         "group": "Maintenance Checks",
         "schedule": {
             "morning_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "Admin Access Key Status"
     },
     "check_deleted_files_lifecycle_status": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Lifecycle Checks",
         "schedule": {
             "hourly_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "check_after": 14,
                         "files_per_run": 50,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "Check for deleted files that require lifecycle updates"
     },
     "check_file_lifecycle_status": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Lifecycle Checks",
         "schedule": {
             "hourly_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "files_per_run": 100,
                         "first_check_after": 14,
                         "max_checking_frequency": 14,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "Check for files that require lifecycle updates"
     },
     "check_validation_errors": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Audit Checks",
         "schedule": {
             "monthly_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Search for Validation Errors"
     },
     "clean_s3_es_checks": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "System Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Wipe Checks Older Than One Month"
     },
     "datastore_status": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Maintenance Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Datastore Status"
     },
     "ecs_status": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "ECS Status"
     },
     "ecs_task_listing": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "ECS Task Listing"
     },
     "elastic_search_space": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Elasticsearch Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "ES Disk Space Check"
     },
     "elasticsearch_s3_count_diff": {
+        "display": [
+            "staging"
+        ],
         "group": "Elasticsearch Checks",
         "schedule": {
             "monthly_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "S3/ES Check Count Differential"
     },
     "failed_metawfrs": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Pipeline Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Failed MetaWorkflowRuns"
     },
     "find_meta_workflow_runs_requiring_output_linktos": {
+        "display": [
+            "staging"
+        ],
         "group": "Pipeline Checks",
         "schedule": {
             "hourly_checks_2": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns to PATCH output files"
     },
     "find_meta_workflow_runs_to_kill": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Pipeline Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns to stop"
     },
     "find_meta_workflow_runs_with_linkto_errors": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Pipeline Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns with output file PATCH errors"
     },
     "find_meta_workflow_runs_with_quality_metric_failure": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Pipeline Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns with QC failure(s)"
     },
     "find_sample_for_meta_workflow": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Pipeline Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Create MetaWorkflowRun from Sample"
     },
     "indexing_progress": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Elasticsearch Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Indexing progress"
     },
     "indexing_records": {
         "conditions": [
             "put_env"
         ],
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Elasticsearch Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Indexing records"
     },
     "invoke_ecs_task": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Invoke an ECS Task"
     },
     "metawfrs_to_checkstatus": {
+        "display": [
+            "staging"
+        ],
         "group": "Pipeline Checks",
         "schedule": {
             "fifteen_min_checks_3": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns to check status"
     },
     "metawfrs_to_run": {
+        "display": [
+            "staging"
+        ],
         "group": "Pipeline Checks",
         "schedule": {
             "fifteen_min_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "MetaWorkflowRuns to run"
     },
     "page_children_routes": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Audit Checks",
         "schedule": {
             "monthly_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Pages with bad routes"
     },
     "rollback_application_version": {
+        "display": [
+            "staging"
+        ],
         "group": "Maintenance Checks",
         "schedule": {
             "fifteen_min_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Application Rollback Check"
     },
     "scale_ecs_service": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Scale ECS Service"
     },
     "scale_elasticsearch": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Maintenance Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Scale OpenSearch"
     },
     "scale_rds": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Maintenance Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Scale RDS"
     },
     "snapshot_rds": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "System Checks",
         "schedule": {
             "monthly_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Snapshot RDS"
     },
     "spot_failed_metawfrs": {
+        "display": [
+            "staging"
+        ],
         "group": "Pipeline Checks",
         "schedule": {
             "fifteen_min_checks_2": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
@@ -455,53 +476,53 @@
         "title": "Spot-failed MetaWorkflowRuns"
     },
     "status_of_elasticsearch_indices": {
         "conditions": [
             "put_env"
         ],
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "Elasticsearch Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Status of elasticsearch indices"
     },
     "trigger_codebuild_run": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
         "title": "Trigger CodeBuild Run"
     },
     "update_ecs_application_versions": {
         "display": [
-            "<env-name>"
+            "staging"
         ],
         "group": "ECS Checks",
         "schedule": {
             "manual_checks": {
-                "<env-name>": {
+                "data": {
                     "dependencies": [],
                     "kwargs": {
                         "primary": true
                     }
                 }
             }
         },
```

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/check_setup.json-local` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/audit_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/ecs_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/es_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/lifecycle_utils.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/linecount_dicts.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/utils.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfr_utils.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/helpers/wfrset_utils.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/lifecycle_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/system_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wfr_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/checks/wrangler_checks.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/deploy.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/chalicelib_smaht/package.py` & `foursight_smaht-0.0.0.1b3/chalicelib_smaht/package.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.0.0.1b2/pyproject.toml` & `foursight_smaht-0.0.0.1b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-smaht"
-version = "0.0.0.1b2"
+version = "0.0.0.1b3"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_smaht" }
 ]
```

### Comparing `foursight_smaht-0.0.0.1b2/setup.py` & `foursight_smaht-0.0.0.1b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-smaht',
-    'version': '0.0.0.1b2',
+    'version': '0.0.0.1b3',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_smaht-0.0.0.1b2/PKG-INFO` & `foursight_smaht-0.0.0.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-smaht
-Version: 0.0.0.1b2
+Version: 0.0.0.1b3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

