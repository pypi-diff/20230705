# Comparing `tmp/grai_source_dbt_cloud-0.1.0a2.tar.gz` & `tmp/grai_source_dbt_cloud-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt_cloud-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_dbt_cloud-0.1.0a6.tar", max compression
```

## Comparing `grai_source_dbt_cloud-0.1.0a2.tar` & `grai_source_dbt_cloud-0.1.0a6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a2/README.md
--rw-r--r--   0        0        0     1125 2023-07-03 14:03:37.813368 grai_source_dbt_cloud-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-30 11:56:24.311647 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/__init__.py
--rw-r--r--   0        0        0     1090 2023-07-03 13:56:25.099263 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/base.py
--rw-r--r--   0        0        0     4549 2023-06-06 17:35:16.800994 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/loader.py
--rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/py.typed
--rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      142 2023-05-03 16:29:40.848719 grai_source_dbt_cloud-0.1.0a6/README.md
+-rw-r--r--   0        0        0     1125 2023-07-05 08:39:28.215748 grai_source_dbt_cloud-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-07-05 08:33:17.555438 grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-05 08:07:14.459967 grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/base.py
+-rw-r--r--   0        0        0     5058 2023-07-05 08:32:48.916974 grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/loader.py
+-rw-r--r--   0        0        0        0 2023-05-03 16:29:40.852043 grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/py.typed
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 grai_source_dbt_cloud-0.1.0a6/PKG-INFO
```

### Comparing `grai_source_dbt_cloud-0.1.0a2/pyproject.toml` & `grai_source_dbt_cloud-0.1.0a6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt_cloud"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha6"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt_cloud", from = "src" },
 ]
 readme = "README.md"
@@ -14,15 +14,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = {version = "^0.3.0a11", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
-grai-source-dbt = {version = "^0.3.0a1", allow-prereleases = true}
+grai-source-dbt = {version = "^0.3.0a7", allow-prereleases = true}
 dbtc = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.0"
 mypy = "^0.991"
 black = "^22.12.0"
```

### Comparing `grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/base.py` & `grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         namespace: Optional[str] = "default",
     ):
         super().__init__(source, version)
 
         self.connector = DbtCloudConnector(
             namespace=namespace,
             api_key=api_key,
+            source=source,
         )
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         nodes, edges = self.connector.get_nodes_and_edges()
         return nodes, edges
 
     def events(self, last_event_date: Optional[str]):
```

### Comparing `grai_source_dbt_cloud-0.1.0a2/src/grai_source_dbt_cloud/loader.py` & `grai_source_dbt_cloud-0.1.0a6/src/grai_source_dbt_cloud/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,47 +2,56 @@
 from functools import lru_cache
 from typing import List, Optional
 
 from dbtc import dbtCloudClient
 
 from grai_source_dbt.adapters import adapt_to_client
 from grai_source_dbt.processor import ManifestProcessor
+from grai_schemas.v1.source import SourceV1
 
 
 class Event:
     """ """
 
-    def __init__(self, reference: str, date: str, status: str, metadata: dict, nodes: List[str]):
+    def __init__(
+        self, reference: str, date: str, status: str, metadata: dict, nodes: List[str]
+    ):
         self.reference = reference
         self.date = date
         self.status = status
         self.metadata = metadata
         self.nodes = nodes
 
 
 class DbtCloudConnector:
     """ """
 
     def __init__(
         self,
         api_key: str,
+        source: SourceV1,
         namespace: Optional[str] = "default",
     ):
+        self.source = source
         self.api_key = api_key
         self.namespace = namespace
 
     def get_nodes_and_edges(self):
         """ """
         self.load_client()
 
         account = self.get_default_acount()
 
-        manifest_obj = self.client.cloud.get_most_recent_run_artifact(account_id=account["id"], path="manifest.json")
-
-        manifest = ManifestProcessor.load(manifest_obj, self.namespace)
+        manifest_obj = self.client.cloud.get_most_recent_run_artifact(
+            account_id=account["id"], path="manifest.json"
+        )
+
+        manifest = ManifestProcessor.load(
+            manifest_obj, self.namespace, self.source.spec
+        )
 
         return manifest.adapted_nodes, manifest.adapted_edges
 
     def get_events(self, last_event_date) -> List[Event]:
         """
 
         Args:
@@ -58,22 +67,33 @@
         account = self.get_default_acount()
 
         runs = self.get_runs(account_id=account["id"], last_event_date=last_event_date)
 
         events = []
 
         for run in runs:
-            if last_event_date and datetime.fromisoformat(run["created_at"]) < last_event_date:
+            if (
+                last_event_date
+                and datetime.fromisoformat(run["created_at"]) < last_event_date
+            ):
                 break
 
             nodes = self.get_run_nodes(account_id=account["id"], run_id=run["id"])
 
             status = "success" if run["status"] == 10 else "error"
 
-            events.append(Event(reference=run["id"], date=run["created_at"], status=status, metadata=run, nodes=nodes))
+            events.append(
+                Event(
+                    reference=run["id"],
+                    date=run["created_at"],
+                    status=status,
+                    metadata=run,
+                    nodes=nodes,
+                )
+            )
 
         return events
 
     def get_run_nodes(self, account_id: str, run_id: str) -> List[str]:
         """
 
         Args:
@@ -132,15 +152,17 @@
             )
         except:
             print(f"Something has gone wrong, no manifest.json for run {run_id}")
 
             return []
 
         unique_ids = [
-            result["unique_id"] for result in run_results["results"] if not result["unique_id"].startswith("test.")
+            result["unique_id"]
+            for result in run_results["results"]
+            if not result["unique_id"].startswith("test.")
         ]
 
         manifest = ManifestProcessor.load(manifest_obj, self.namespace)
 
         name_mapper = get_adapted_node_map(manifest=manifest)
 
         return [name_mapper(unique_id) for unique_id in unique_ids]
@@ -170,21 +192,28 @@
         runs = []
 
         offset = 0
         limit = 100
 
         while True:
             result = self.client.cloud.list_runs(
-                account_id=account_id, order_by="-created_at", limit=limit, offset=offset
+                account_id=account_id,
+                order_by="-created_at",
+                limit=limit,
+                offset=offset,
             )
 
             runs.extend(result["data"])
 
             if result["extra"]["pagination"]["total_count"] <= len(runs):
                 break
 
-            if last_event_date and datetime.fromisoformat(result["data"][-1]["created_at"]) < last_event_date:
+            if (
+                last_event_date
+                and datetime.fromisoformat(result["data"][-1]["created_at"])
+                < last_event_date
+            ):
                 break
 
             offset += limit
 
         return runs
```

### Comparing `grai_source_dbt_cloud-0.1.0a2/PKG-INFO` & `grai_source_dbt_cloud-0.1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt-cloud
-Version: 0.1.0a2
+Version: 0.1.0a6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbtc (>=0.4.2,<0.5.0)
 Requires-Dist: grai-client (>=0.3.0a11,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
-Requires-Dist: grai-source-dbt (>=0.3.0a1,<0.4.0)
+Requires-Dist: grai-source-dbt (>=0.3.0a7,<0.4.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt-cloud
 Description-Content-Type: text/markdown
 
 # Grai dbt Cloud Integration
```

