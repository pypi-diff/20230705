# Comparing `tmp/iam_actions-1.2.20230704.tar.gz` & `tmp/iam_actions-1.2.20230705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230704.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230705.tar", max compression
```

## Comparing `iam_actions-1.2.20230704.tar` & `iam_actions-1.2.20230705.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/README.md
--rw-r--r--   0        0        0      228 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/__init__.py
--rw-r--r--   0        0        0  4362696 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-04 02:54:02.569849 iam_actions-1.2.20230704/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560956 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544073 2023-07-04 02:56:01.959111 iam_actions-1.2.20230704/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-04 02:56:02.963124 iam_actions-1.2.20230704/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230704/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230704/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/README.md
+-rw-r--r--   0        0        0      228 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4362696 2023-07-05 02:54:40.484892 iam_actions-1.2.20230705/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-05 02:52:58.992711 iam_actions-1.2.20230705/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560956 2023-07-05 02:54:40.484892 iam_actions-1.2.20230705/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-05 02:54:40.484892 iam_actions-1.2.20230705/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544073 2023-07-05 02:54:40.484892 iam_actions-1.2.20230705/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-05 02:54:41.268894 iam_actions-1.2.20230705/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230705/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230705/PKG-INFO
```

### Comparing `iam_actions-1.2.20230704/LICENSE` & `iam_actions-1.2.20230705/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/README.md` & `iam_actions-1.2.20230705/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/actions.json` & `iam_actions-1.2.20230705/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4135,217 +4135,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "ListIngestionDestinations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIngestionDestination": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -17622,305 +17622,305 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "GetProtectedQuery": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
             "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -25323,129 +25323,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "CreateScan": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -33037,25 +33037,25 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -33473,25 +33473,25 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "GetCustomerVerificationEligibility": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
@@ -35151,91 +35151,91 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "GetProject": {
+        "ListUserProjects": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "ListUserProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectCredentials": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetProjectCredentials",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetProjectConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetProjectConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserProjects": {
+        "GetProjectCredentials": {
             "access_level": "Undocumented",
-            "action": "ListUserProjects",
+            "action": "GetProjectCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProjectConfiguration": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "GetProjectConfiguration",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "datazonecontrol": {
-        "GetEnvironment": {
+        "GetMetadataCollector": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "GetMetadataCollector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DissociateAccount": {
+        "ListAssociatedEnvironments": {
             "access_level": "Undocumented",
-            "action": "DissociateAccount",
+            "action": "ListAssociatedEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListEnvironment": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteEnvironment": {
             "access_level": "Undocumented",
@@ -35249,185 +35249,185 @@
             "access_level": "Undocumented",
             "action": "ListMetadataCollectorRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataCollector": {
+        "GetUserPortalLoginAuthCode": {
             "access_level": "Undocumented",
-            "action": "GetMetadataCollector",
+            "action": "GetUserPortalLoginAuthCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListMetadataCollectors": {
             "access_level": "Undocumented",
             "action": "ListMetadataCollectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceByEnvironment": {
+        "UpdateAccountAssociationDescription": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceByEnvironment",
+            "action": "UpdateAccountAssociationDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "CreateAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "CreateAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAllAssociatedAccountsForEnvironment": {
             "access_level": "Undocumented",
             "action": "ListAllAssociatedAccountsForEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAssociationInvitations": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAccountAssociationInvitations",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "ReviewAccountAssociationInvitation": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "ReviewAccountAssociationInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPortalLoginAuthCode": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "GetUserPortalLoginAuthCode",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListDataSourcesByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListDataSourcesByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReviewAccountAssociationInvitation": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ReviewAccountAssociationInvitation",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedEnvironments": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedEnvironments",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountAssociationDescription": {
+        "GetAssociatedDomain": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountAssociationDescription",
+            "action": "GetAssociatedDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "GetDataSourceByEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "GetDataSourceByEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAssociationInvitation": {
+        "DissociateAccount": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAssociationInvitation",
+            "action": "DissociateAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourcesByEnvironment": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListDataSourcesByEnvironment",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironment": {
+        "ListAccountAssociationInvitations": {
             "access_level": "Undocumented",
-            "action": "ListEnvironment",
+            "action": "ListAccountAssociationInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssociatedDomain": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "GetAssociatedDomain",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -57160,225 +57160,225 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "CreateTargetGroup": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -63928,33 +63928,33 @@
             "condition_keys": [],
             "description": "Grants permission to verify the email for FreeRTOS extended maintenance plan (EMP)",
             "orphan": false,
             "resources": []
         }
     },
     "freetier": {
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetFreeTierAlertPreference": {
             "access_level": "Undocumented",
             "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -72425,1377 +72425,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "UntagServerCertificate": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateAccessKey": {
             "access_level": "Undocumented",
             "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -75620,41 +75620,41 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "ListInvoiceSummaries": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -81561,889 +81561,889 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "UpdateResourcePosition": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
             "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -85198,315 +85198,315 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "CreateRescoreExecutionPlan": {
+        "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRescoreExecutionPlans": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "ListRescoreExecutionPlans",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "ListStreams": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -88092,169 +88092,169 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "GetWorkloadAssets": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAdditionalNodes": {
             "access_level": "Undocumented",
             "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -96918,225 +96918,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "DeleteChannelPolicy": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateChannelGroup": {
             "access_level": "Undocumented",
             "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetHeadObject": {
             "access_level": "Undocumented",
             "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -104216,177 +104216,177 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "GetNotificationEvent": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
             "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
@@ -104394,73 +104394,73 @@
             "access_level": "Undocumented",
             "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SendActivationCode": {
             "access_level": "Undocumented",
             "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListEmailContacts": {
             "access_level": "Undocumented",
             "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -106833,129 +106833,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "CreatePipeline": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -107570,315 +107570,315 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "payment-cryptography": {
-        "VerifyPinData": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "VerifyMac": {
             "access_level": "Undocumented",
             "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "MakePayment": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPaymentPreferences": {
             "access_level": "Undocumented",
             "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentStatus": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentStatus",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "GetPaymentStatus": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -113315,281 +113315,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "AssociateResourceSharePermission": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131166,113 +131166,113 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "ListInstances": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
             "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -146270,273 +146270,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "ListSolFunctionInstances": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "GetSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -148371,49 +148371,41 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "UpdatePolicyStore": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeletePolicy": {
             "access_level": "Undocumented",
             "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
-            "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "CreatePolicyTemplate": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "IsAuthorized": {
             "access_level": "Undocumented",
@@ -148427,149 +148419,157 @@
             "access_level": "Undocumented",
             "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSchema": {
             "access_level": "Undocumented",
             "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateIdentitySource": {
             "access_level": "Undocumented",
             "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListPolicyStores": {
             "access_level": "Undocumented",
             "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "ListPolicyTemplates": {
+            "access_level": "Undocumented",
+            "action": "ListPolicyTemplates",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "voiceid": {
         "AssociateFraudster": {
             "access_level": "Write",
             "action": "AssociateFraudster",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230705/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230705/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/generate.py` & `iam_actions-1.2.20230705/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230705/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230705/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/generate/services.py` & `iam_actions-1.2.20230705/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/policies.json` & `iam_actions-1.2.20230705/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230705/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/iam_actions/services.json` & `iam_actions-1.2.20230705/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230704/pyproject.toml` & `iam_actions-1.2.20230705/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230704"
+version = "1.2.20230705"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230704/setup.py` & `iam_actions-1.2.20230705/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230704',
+    'version': '1.2.20230705',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230704/PKG-INFO` & `iam_actions-1.2.20230705/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230704
+Version: 1.2.20230705
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

