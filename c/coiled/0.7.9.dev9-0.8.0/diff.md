# Comparing `tmp/coiled-0.7.9.dev9.tar.gz` & `tmp/coiled-0.8.0.tar.gz`

## Comparing `coiled-0.7.9.dev9.tar` & `coiled-0.8.0.tar`

### file list

```diff
@@ -1,56 +1,63 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/context.py
--rw-r--r--   0        0        0   102119 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/magic.py
--rw-r--r--   0        0        0    17618 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/software.py
--rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/types.py
--rw-r--r--   0        0        0    52430 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/websockets.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    89825 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    44216 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.7.9.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/analytics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/exceptions.py
+-rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/magic.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/run.py
+-rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/types.py
+-rw-r--r--   0        0        0    53908 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/authenticate.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/config.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92101 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.0/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.0/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 coiled-0.8.0/PKG-INFO
```

### Comparing `coiled-0.7.9.dev9/coiled/__init__.py` & `coiled-0.8.0/coiled/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,25 @@
     revoke_all_api_tokens,
     revoke_api_token,
     set_backend_options,
 )
 from .v2 import (
     AWSOptions,
     BackendOptions,
-    Cloud,
+    CloudV2 as Cloud,
     Cluster,
     FirewallOptions,
     GCPOptions,
     better_cluster_logs,
     cluster_logs,
     create_cluster,
     delete_cluster,
     list_clusters,
 )
+from .run import run
 from importlib_metadata import version
 
 inspect = _inspect.callback
 del _inspect
 
 # Register coiled configuration values with Dask's config system
 from . import config
@@ -47,15 +48,15 @@
 del config
 
 # Top-level coiled.config attribute
 
 
 def __getattr__(name):
     if name == "config":
-        import dask
+        import dask.config
 
         return dask.config.get("coiled")
     raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
 
 
 __version__ = version("coiled")
```

### Comparing `coiled-0.7.9.dev9/coiled/analytics.py` & `coiled-0.8.0/coiled/analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from types import ModuleType
 from typing import Optional
 
-import dask
+import dask.config
 import urllib3
 from dask.distributed import Client, get_client
 from dask.utils import has_keyword
 
 import coiled
```

### Comparing `coiled-0.7.9.dev9/coiled/cluster.py` & `coiled-0.8.0/coiled/cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 import logging
 
-import dask
+import dask.config
 from dask.distributed import Client
 from distributed.deploy.adaptive import Adaptive
 
 from .utils import COILED_LOGGER_NAME
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 
@@ -24,16 +24,26 @@
         target_duration = kwargs.get("target_duration")
         if target_duration:
             with Client(self.cluster) as client:
                 client.run_on_scheduler(
                     lambda: dask.config.set({"distributed.adaptive.target-duration": target_duration})
                 )
 
+    def config_as_string(self):
+        return (
+            f"Config is maximum: {self.maximum}, minimum: {self.minimum}, wait_count: {self.wait_count}, "
+            f"interval: {self.interval}, target_duration: {self.target_duration}."
+        )
+
     async def scale_up(self, n):
         logger.info(f"Adaptive scaling up to {n} workers.")
-        await self.cluster.scale_up(n, reason=f"Adaptive scaling up to {n} workers.")
+        if self.cluster:
+            await self.cluster.scale_up(n, reason=f"Adaptive scaling up to {n} workers. {self.config_as_string()}")
 
     async def scale_down(self, workers):
         if not workers:
             return
         logger.info(f"Adaptive is removing {len(workers)} workers: {workers}.")
-        await self.cluster.scale_down(workers, reason=f"Adaptive removing {len(workers)} workers.")
+        if self.cluster:
+            await self.cluster.scale_down(
+                workers, reason=f"Adaptive removing {len(workers)} workers. {self.config_as_string()}"
+            )
```

### Comparing `coiled-0.7.9.dev9/coiled/coiled.yaml` & `coiled-0.8.0/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/context.py` & `coiled-0.8.0/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/core.py` & `coiled-0.8.0/coiled/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Cloud (and similarly its subclass CloudBeta) is not intended as a user-facing API but rather is a helper
+Cloud (and similarly its subclass CloudV2) is not intended as a user-facing API but rather is a helper
 for implementing top-level user-facing functions.
 
 * Cloud contains methods for our "v1" API (e.g. software environments)
-* CloudBeta contains methods for our "v2" API (clusters, package sync)
+* CloudV2 contains methods for our "v2" API (clusters, package sync)
 
-A few methods in Cloud are reused by CloudBeta, but not much. Ideally we would completely separate these classes
+A few methods in Cloud are reused by CloudV2, but not much. Ideally we would completely separate these classes
 so there's no subclass relationship, or implement a tiny base class CloudBase with subclasses CloudV1 and CloudV2.
 
 Some notes on async:
 
 Because the distributed API can be used as either async and sync, Coiled can too. This is implemented with
 leading-underscore async-only functions like "Cloud._create_software_environment", and then non-underscored
 versions like "Cloud.create_software_environment", where the latter uses a helper method "cloud.sync" to do
@@ -55,18 +55,19 @@
     cast,
     overload,
 )
 
 import aiohttp
 import backoff
 import dask
+import dask.config
 import dask.distributed
 import distributed
 import rich
-from distributed.comm import parse_address
+from distributed.comm.addressing import parse_address
 from distributed.utils import LoopRunner, sync
 from importlib_metadata import PackageNotFoundError, version
 from packaging.version import Version
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from tornado.ioloop import IOLoop
@@ -311,15 +312,15 @@
             f"  <li><b>Server: </b>{self.server}</li>\n"
             f"  <li><b>Account: </b>{self.default_account}</li>\n"
         )
 
         return text
 
     @property
-    def loop(self):
+    def loop(self) -> IOLoop:
         return self._loop_runner.loop
 
     @overload
     @classmethod
     def current(cls, asynchronous: Sync) -> Cloud[Sync]:
         ...
 
@@ -521,15 +522,15 @@
     ) -> Union[_T, Coroutine[None, None, _T]]:
         asynchronous = self.asynchronous
         if asynchronous:
             future = func(*args, **kwargs)
             future = asyncio.wait_for(future, timeout=None)
             return future
         else:
-            return sync(self.loop, func, *args, **kwargs)
+            return cast(_T, sync(self.loop, func, *args, **kwargs))
 
     def _verify_account(self, account: str):
         """Perform sanity checks on account values
 
         In particular, this raises and informative error message if the
         account is not found, and provides a list of possible options.
         """
@@ -2143,15 +2144,16 @@
     gpu_enabled: bool = False,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> Optional[SoftwareEnvironmentAlias]:
     """Create a software environment
 
     .. seealso::
 
-       By default, your local environment is automatically replicated in your cluster (see :doc:`package_sync`).
+       By default, your local environment is automatically replicated in your
+       cluster (see :doc:`software/index`).
 
     .. deprecated:: 0.6.0
 
       The following parameters for ``create_software_environment`` have been deprecated: ``use_entrypoint``
 
     Parameters
     ----------
@@ -2199,15 +2201,15 @@
                 architecture=architecture,
             )
         except Exception as e:
             error = e
             raise
         finally:
             data = {
-                **error_info_for_tracking(error),
+                **(error_info_for_tracking(error) if error else {}),
                 "name": str(name),
                 "conda": bool(conda),
                 "account": account,
                 "pip": bool(pip),
                 "container": container,
                 "use_entrypoint": bool(use_entrypoint),
             }
@@ -2551,14 +2553,15 @@
     zone: Optional[str] = None,
     registry_type: Literal["ecr", "docker_hub", "gar"] = "ecr",
     registry_namespace: Optional[str] = None,
     registry_access_token: Optional[str] = None,
     registry_uri: str = "docker.io",
     registry_username: Optional[str] = None,
     log_output=sys.stdout,
+    use_shim: bool = False,
     **kwargs,
 ):
     """Configure account level settings for cloud provider and container registry.
 
     This method configures account level backend settings for cloud providers, container registries,
     and setting up an account-level VPC for running clusters and other Coiled managed resources.
 
@@ -2672,14 +2675,15 @@
             "credentials": {"aws_access_key_id": "", "aws_secret_access_key": ""},
             "firewall": {},
             "firewall_spec": firewall_spec,
             "network": network or {},
             "zone": zone,
         },
         "registry": {"type": "ecr", "credentials": {}, "public_ecr": False},
+        "use_shim": use_shim,
     }
 
     # override gcp_zone with zone, if set
     if zone and gcp_project_id:
         gcp_zone = zone
 
     output_msg = ""
@@ -2813,15 +2817,15 @@
     gpus: Optional[Union[int, List[int]]] = None,
     arch: Optional[Literal["x86_64", "arm64"]] = None,
 ) -> Dict[str, VmType]:
     """List allowed instance types for the cloud provider configured on your account.
 
     This command allows you to get all instance types available for a backend or a filtered
     list of instance types that match your requirements by using the available keyword
-    arguments. Please refer to :doc:`tutorials/select_instance_types` for more information.
+    arguments. Please refer to :doc:`clusters/size-and-type` for more information.
 
     Parameters
     ----------
     backend:
         Relevant cloud provider (aws or gcp) to get a list of allowed instance types. If
         not provided the list will show the instances for your account cloud provider.
     min_cores
@@ -2857,15 +2861,15 @@
 
 
 def list_gpu_types() -> Dict:
     """List allowed GPU Types.
 
     For AWS the GPU types are tied to the instance type, but for GCP you can
     add different GPU types to GPU enabled instances. Please refer to
-    :doc:`gpu` for more information.
+    :doc:`clusters/gpu` for more information.
 
     Parameters
     ----------
     json
         if set to ``True``, it will return this list in json format instead of a table.
 
     """
```

### Comparing `coiled-0.7.9.dev9/coiled/exceptions.py` & `coiled-0.8.0/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/magic.py` & `coiled-0.8.0/coiled/magic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import logging
 import platform
 import re
+import shutil
 import subprocess
 import sys
 import typing
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from logging import getLogger
@@ -17,20 +18,20 @@
 from urllib.parse import urlparse
 
 from dask import config
 from filelock import BaseFileLock, FileLock
 from packaging.utils import parse_wheel_filename
 from rich.progress import Progress
 
-from coiled._beta.core import CloudBeta
-from coiled._beta.widgets.util import simple_progress
 from coiled.context import track_context
 from coiled.scan import PackageInfo, scan_prefix
 from coiled.types import ArchitectureTypesEnum, PackageLevelEnum, ResolvedPackageInfo
 from coiled.utils import validate_wheel
+from coiled.v2.core import CloudV2
+from coiled.v2.widgets.util import simple_progress
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 ANY_AVAILABLE = "ANY-AVAILABLE"
 
 
@@ -133,25 +134,28 @@
                     "note": None,
                     "sdist": None,
                     "md5": None,
                 }
             wheel_fn = next(file for file in outdir.iterdir() if file.suffix == ".whl")
         logger.info(f"Using wheel @ {wheel_fn}")
         _, build_version, _, _ = parse_wheel_filename(str(wheel_fn.name))
-        has_python, md5 = await validate_wheel(wheel_fn)
+        has_python, md5, missing_py_files = await validate_wheel(wheel_fn, src)
     return {
         "name": pkg_name,
         "source": "pip",
         "channel": None,
         "conda_name": None,
         "client_version": str(build_version),
         "specifier": "",
         "include": True,
         "error": None if has_python else "Built wheel contains no python files!",
-        "note": f"Wheel built from {src}",
+        "note": (
+            f"Wheel built from {src}"
+            + (f" is missing {', '.join(sorted(missing_py_files)[:10])}" if missing_py_files else "")
+        ),
         "sdist": wheel_fn.open("rb"),
         "md5": md5,
     }
 
 
 @track_context
 async def create_wheel_from_egg(pkg_name: str, version: str, src: str) -> ResolvedPackageInfo:
@@ -183,33 +187,136 @@
                 ", will not be included in environment, check stdout for egg conversion log"
             ),
             "note": None,
             "sdist": None,
             "md5": None,
         }
     wheel_fn = next(file for file in outdir.iterdir() if file.suffix == ".whl")
-    has_python, md5 = await validate_wheel(Path(wheel_fn))
+    has_python, md5, missing_py_files = await validate_wheel(Path(wheel_fn), tmpdir.name)
     return {
         "name": pkg_name,
         "source": "pip",
         "channel": None,
         "conda_name": None,
         "client_version": version,
         "specifier": "",
         "include": True,
         "error": None if has_python else "Built wheel has no python files!",
-        "note": "Wheel built from local egg",
+        "note": (
+            "Wheel built from local egg"
+            + (f" is missing {', '.join(sorted(missing_py_files)[:10])}" if missing_py_files else "")
+        ),
+        "sdist": wheel_fn.open("rb"),
+        "md5": md5,
+    }
+
+
+@track_context
+async def create_wheel_from_src_dir(pkg_name: str, version: str, src: str) -> ResolvedPackageInfo:
+    # These locks are set up such that
+    # Threads: Block on each other and check if another thread already built the tarball
+    # Processes: Block on each other, but will not reuse a tarball created by another
+    md5 = None
+    lock_path = Path(config.PATH)
+    lock_path.mkdir(parents=True, exist_ok=True)  # ensure lockfile directory exists
+    package_lock, thread_lock, tmpdir = WHEEL_BUILD_LOCKS.setdefault(
+        pkg_name,
+        (FileLock(lock_path / (f".{pkg_name}{version}.build-lock")), Lock(), TemporaryDirectory()),
+    )
+    async with async_lock(package_lock, thread_lock):
+        outdir = Path(tmpdir.name) / Path(pkg_name)
+        if outdir.exists():
+            logger.debug(f"Checking for existing source archive for {pkg_name} @ {outdir}")
+            wheel_fn = next((file for file in outdir.iterdir() if file.suffix == ".whl"), None)
+        else:
+            wheel_fn = None
+        if not wheel_fn:
+            logger.info(f"No existing source archive, creating an archive for {pkg_name} @ {src}")
+            try:
+                unpacked_dir = outdir / f"{pkg_name}-{version}"
+                # Create fake metadata to make wheel work
+                dist_info_dir = unpacked_dir / f"{unpacked_dir.name}.dist-info"
+                dist_info_dir.mkdir(parents=True)
+                with open(dist_info_dir / "METADATA", "w") as f:
+                    f.write(f"Metadata-Version: 2.1\nName: {pkg_name}\nVersion: {version}\n")
+                with open(dist_info_dir / "WHEEL", "w") as f:
+                    f.write("Wheel-Version: 1.0\nGenerator: coiled\nRoot-Is-Purelib: true\nTag: py3-none-any\n")
+                for file in Path(src).rglob("*.py"):
+                    rel_file = file.relative_to(src)
+                    # Skip top-level __init__.py or __main__.py because they
+                    # should not go in site-packages
+                    if str(rel_file) in ("__init__.py", "__main__.py"):
+                        continue
+                    dest = unpacked_dir / rel_file
+                    dest.parent.mkdir(parents=True, exist_ok=True)
+                    shutil.copy(file, dest)
+                p = await create_subprocess_shell(
+                    cmd=f"{executable} -m wheel pack --dest-dir {outdir} {unpacked_dir}",
+                    stderr=subprocess.STDOUT,
+                    stdout=subprocess.PIPE,
+                )
+                if p.returncode:
+                    print(
+                        f"---wheel packing log for {src}---\n"
+                        + p.stdout.decode(encoding=sys.stdout.encoding or "utf-8")
+                    )
+                    return {
+                        "name": pkg_name,
+                        "source": "pip",
+                        "channel": None,
+                        "conda_name": None,
+                        "client_version": version,
+                        "specifier": "",
+                        "include": False,
+                        "error": (
+                            "Failed to build a package of your local python files. Please check stdout for details"
+                        ),
+                        "note": None,
+                        "sdist": None,
+                        "md5": None,
+                    }
+            except IOError as e:
+                return {
+                    "name": pkg_name,
+                    "source": "pip",
+                    "channel": None,
+                    "conda_name": None,
+                    "client_version": version,
+                    "specifier": "",
+                    "include": False,
+                    "error": f"Failed to build a package of your local python files. Exception: {e}",
+                    "note": None,
+                    "sdist": None,
+                    "md5": None,
+                }
+            wheel_fn = next(file for file in outdir.iterdir() if file.suffix == ".whl")
+        logger.info(f"Using wheel @ {wheel_fn}")
+        _, build_version, _, _ = parse_wheel_filename(str(wheel_fn.name))
+        has_python, md5, missing_py_files = await validate_wheel(wheel_fn, src)
+    return {
+        "name": pkg_name,
+        "source": "pip",
+        "channel": None,
+        "conda_name": None,
+        "client_version": str(build_version),
+        "specifier": "",
+        "include": True,
+        "error": None if has_python else "Built wheel does not contain all python files!",
+        "note": (
+            f"Source wheel built from {src}"
+            + (f" is missing {', '.join(sorted(missing_py_files)[:10])}" if missing_py_files else "")
+        ),
         "sdist": wheel_fn.open("rb"),
         "md5": md5,
     }
 
 
 @track_context
 async def approximate_packages(
-    cloud: CloudBeta,
+    cloud: CloudV2,
     packages: List[PackageInfo],
     priorities: Dict[Tuple[str, Literal["conda", "pip"]], PackageLevelEnum],
     progress: Optional[Progress] = None,
     strict: bool = False,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> typing.List[ResolvedPackageInfo]:
     user_conda_installed_python = next((p for p in packages if p["name"] == "python"), None)
@@ -367,14 +474,23 @@
                     finalized_packages.append(
                         await create_wheel_from_egg(
                             pkg_name=pkg["name"],
                             version=pkg["version"],
                             src=pkg["wheel_target"],
                         )
                     )
+            elif pkg["name"].startswith("coiled_local_"):
+                with simple_progress(f'Creating wheel for {pkg["wheel_target"]}', progress=progress):
+                    finalized_packages.append(
+                        await create_wheel_from_src_dir(
+                            pkg_name=pkg["name"],
+                            version=pkg["version"],
+                            src=pkg["wheel_target"],
+                        )
+                    )
             else:
                 with simple_progress(f'Creating wheel for {pkg["name"]}', progress=progress):
                     finalized_packages.append(
                         await create_wheel(
                             pkg_name=pkg["name"],
                             version=pkg["version"],
                             src=pkg["wheel_target"],
@@ -422,15 +538,15 @@
                 logger.warning(warning)
                 faulty_packages[groups["package"]].append(warning)
         return faulty_packages
 
 
 @track_context
 async def create_environment_approximation(
-    cloud: CloudBeta,
+    cloud: CloudV2,
     priorities: Dict[Tuple[str, Literal["conda", "pip"]], PackageLevelEnum],
     only: Optional[Set[str]] = None,
     strict: bool = False,
     progress: Optional[Progress] = None,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> typing.List[ResolvedPackageInfo]:
     packages = await scan_prefix(progress=progress)
@@ -473,15 +589,15 @@
 
     basicConfig(level=logging.INFO)
 
     from rich.console import Console
     from rich.table import Table
 
     async def run():
-        async with CloudBeta(asynchronous=True) as cloud:
+        async with CloudV2(asynchronous=True) as cloud:
             return await create_environment_approximation(
                 cloud=cloud,
                 priorities={
                     ("dask", "conda"): PackageLevelEnum.CRITICAL,
                     ("twisted", "conda"): PackageLevelEnum.IGNORE,
                     ("graphviz", "conda"): PackageLevelEnum.LOOSE,
                     ("icu", "conda"): PackageLevelEnum.LOOSE,
```

### Comparing `coiled-0.7.9.dev9/coiled/scan.py` & `coiled-0.8.0/coiled/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import sys
 import typing
 from base64 import urlsafe_b64encode
 from collections import defaultdict
 from logging import getLogger
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, cast
 from urllib.parse import urlparse
 
 from importlib_metadata import Distribution, PackagePath
 from packaging.version import InvalidVersion
 from packaging.version import parse as parse_version
 from rich.progress import Progress
 from typing_extensions import Literal
@@ -22,14 +22,44 @@
 from coiled.utils import parse_file_uri
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 
 
+class ResilientDistribution(Distribution):
+    """Subclass of Distribution that adds more resilient methods for retrieving files"""
+
+    def _read_files_egginfo_installed(self):
+        """
+        Read installed-files.txt and return lines in a similar
+        CSV-parsable format as RECORD: each file should be placed
+        relative to the site-packages directory and must be
+        quoted (since file names can contain literal commas).
+
+        This file is written when the package is installed by pip,
+        but it might not be written for other installation methods.
+        Assume the file is accurate if it exists.
+        """
+        text = self.read_text("installed-files.txt")
+        # Prepend the .egg-info/ subdir to the lines in this file.
+        # But this subdir is only available from PathDistribution's
+        # self._path.
+        subdir = getattr(self, "_path", None)
+        if not text or not subdir:
+            return
+
+        site_pkgs_path = cast(Path, self.locate_file("")).resolve()
+        for name in text.splitlines():
+            # relpath will add .. to a path to make it relative to site-packages,
+            # so use that instead of Path.relative_to (which will raise an error)
+            path = Path(os.path.relpath((subdir / name).resolve(), site_pkgs_path))
+            yield f'"{path.as_posix()}"'
+
+
 def normalize_name(name: str):
     # gives the best shot at names being consistent between pypi/conda
     return name.lower().replace("-", "_")
 
 
 def normalize_version(version: str):
     """Attempt to normalize version between conda and pip without tripping over conda not supporting PEP440"""
@@ -84,15 +114,15 @@
     if metadata_location:
         if not metadata_location.exists():
             # a file for this package no longer exists
             # likely pip installed a new version
             # removing the conda installed version
             return None
         else:
-            dist = Distribution.at(pkg.prefix / metadata_location)
+            dist = ResilientDistribution.at(pkg.prefix / metadata_location)
             name = dist.metadata["Name"] or pkg.name
     else:
         name = pkg.name
     return {
         "channel": pkg.channel,
         "path": None,
         "channel_url": pkg.channel_url,
@@ -102,14 +132,17 @@
         "name": name,
         "version": pkg.version,
         "wheel_target": None,
     }
 
 
 async def handle_dist(dist: Distribution, locations: List[Path]) -> Optional[Union[PackageInfo, CondaPlaceHolder]]:
+    # Sometimes the dist name is blank (seemingly only on Windows?)
+    if not dist.name:
+        return
     installer = dist.read_text("INSTALLER") or ""
     installer = installer.rstrip()
     # dist._path can sometimes be a zipp.Path or something else
     dist_path = Path(str(dist._path))  # type: ignore
     if installer == "conda":
         return CondaPlaceHolder(name=dist.name, path=dist_path)
     elif dist_path.parent.suffix == ".egg":
@@ -187,22 +220,17 @@
                     "subdir": None,
                     "conda_name": None,
                     "version": dist.version,
                     "wheel_target": str(path),
                 }
         egg_links = []
         for location in locations:
-            if os.name == "nt":
-                egg_link_pth = location / Path(dist.name).with_suffix(".egg-link")
-                if egg_link_pth.is_file():
-                    egg_links.append(location / Path(dist.name).with_suffix(".egg-link"))
-            else:
-                egg_link_pth = location / Path(dist.name).with_suffix(".egg-link")
-                if egg_link_pth.is_file():
-                    egg_links.append(location / Path(dist.name).with_suffix(".egg-link"))
+            egg_link_pth = location / Path(dist.name).with_suffix(".egg-link")
+            if egg_link_pth.is_file():
+                egg_links.append(location / Path(dist.name).with_suffix(".egg-link"))
         if egg_links:
             return {
                 "name": dist.name,
                 "path": dist_path.parent,
                 "source": "pip",
                 "channel": None,
                 "channel_url": None,
@@ -259,15 +287,15 @@
                     elif line.rstrip() == ".":
                         continue
                     else:
                         p = location / Path(line.rstrip())
                         full_path = str(p.resolve())
                         if p.exists() and full_path not in paths:
                             paths.append(full_path)
-    dists: List[Distribution] = [dist for dist in Distribution.discover(path=list(paths))]
+    dists: List[Distribution] = [dist for dist in ResilientDistribution.discover(path=list(paths))]
     packages = []
     if progress:
         for task in progress.track(
             asyncio.as_completed([handle_dist(dist, locations) for dist in dists]),
             total=len(dists),
             description=f"Scanning {len(dists)} python packages",
         ):
@@ -283,16 +311,16 @@
             # For duplicate .dist-info directories, we need to check which
             # version is actually importable
             existing_pkg = pkgs_by_name.get(pkg_name)
             if existing_pkg is None:
                 pkgs_by_name[pkg_name] = pkg
             else:
                 # Compare hashes to actual files
-                new_dist = Distribution.at(pkg["path"])
-                old_dist = Distribution.at(existing_pkg["path"])
+                new_dist = ResilientDistribution.at(pkg["path"])
+                old_dist = ResilientDistribution.at(existing_pkg["path"])
                 new_dist_path = new_dist._path  # type: ignore
                 old_dist_path = old_dist._path  # type: ignore
                 new_is_egg_info = new_dist_path.name.endswith(".egg-info")  # type: ignore
                 old_is_egg_info = old_dist_path.name.endswith(".egg-info")  # type: ignore
                 new_is_dist_info = new_dist_path.name.endswith(".dist-info")  # type: ignore
                 old_is_dist_info = old_dist_path.name.endswith(".dist-info")  # type: ignore
                 if (new_is_egg_info and not old_is_egg_info) or (new_is_dist_info and not old_is_dist_info):
@@ -345,26 +373,31 @@
                     if not _is_hash_match(old_dist, old_pkg_paths, path):
                         logger.debug("Encountered path that does not match either version: %s", path)
 
     return pkgs_by_name
 
 
 async def scan_prefix(
-    prefix: Optional[Path] = None, progress: Optional[Progress] = None, locations: Optional[List[Path]] = None
+    prefix: Optional[Path] = None,
+    progress: Optional[Progress] = None,
+    locations: Optional[List[Path]] = None,
 ) -> typing.List[PackageInfo]:
     # TODO: private conda channels
     # TODO: detect pre-releases and only set --pre flag for those packages (for conda)
 
     if not prefix:
         prefix = Path(sys.prefix)
+    if not locations:
+        locations = [Path(p) for p in sys.path]
+        cwd = Path.cwd()
+        if cwd not in locations:
+            locations.insert(0, cwd)
     conda_env_future = asyncio.create_task(scan_conda(prefix=prefix, progress=progress))
     # only pass locations to support testing, otherwise we should be using sys.path
-    pip_env_future = asyncio.create_task(
-        scan_pip(locations=locations or [Path(p) for p in sys.path], progress=progress)
-    )
+    pip_env_future = asyncio.create_task(scan_pip(locations=locations, progress=progress))
     conda_env = await conda_env_future
     pip_env = await pip_env_future
     filtered_conda = {}
     # the pip list is the "truth" of what is imported for python deps
     for name, packages in conda_env.items():
         # if a package exists in the pip list but is not a conda place holder
         # then the conda package wont be imported and should be discarded
@@ -401,11 +434,32 @@
                     )
                     break
         if not found:
             # a non python package and safe to include
             filtered_conda[name] = packages[0]
     # remove conda placeholders
     pip_env = {pkg_name: pkg for pkg_name, pkg in pip_env.items() if not isinstance(pkg, CondaPlaceHolder)}
-    return sorted(
+    results = sorted(
         list(pip_env.values()) + list(filtered_conda.values()),
         key=lambda pkg: pkg["name"],
     )
+
+    # Handle modules that are not installed via pip or conda
+    pkg_paths = {pkg["path"].resolve() for pkg in results if pkg["path"]}
+    extra_paths = {p.resolve() for p in locations if prefix not in p.parents} - pkg_paths
+    for extra_path in extra_paths:
+        if not extra_path.is_dir():
+            continue
+        results.append(
+            {
+                "name": f"coiled_local_{extra_path.name.replace('-', '_')}",
+                "path": extra_path,
+                "source": "pip",
+                "version": "0.0.0",
+                "channel_url": None,
+                "channel": None,
+                "subdir": None,
+                "conda_name": None,
+                "wheel_target": str(extra_path),
+            }
+        )
+    return sorted(results, key=lambda pkg: pkg["name"])
```

### Comparing `coiled-0.7.9.dev9/coiled/software.py` & `coiled-0.8.0/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/types.py` & `coiled-0.8.0/coiled/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,17 @@
     """
     All currently supported architecture types
     """
 
     X86_64 = "x86_64"
     ARM64 = "aarch64"
 
+    def __str__(self) -> str:
+        return self.value
+
     @property
     def conda_suffix(self) -> str:
         if self == ArchitectureTypesEnum.X86_64:
             return "64"
         else:
             return self.value
 
@@ -300,15 +303,15 @@
 
     Parameters
     ----------
     keypair_name
         AWS Keypair to assign worker/scheduler instances. This would need to be an existing keypair in your
             account, and needs to be in the same region as your cluster. Note that Coiled can also manage
             adding a unique, ephemeral keypair for SSH access to your cluster;
-            see :doc:`tutorials/ssh` for more information.
+            see :doc:`ssh` for more information.
     use_placement_group
         If possible, this will attempt to put workers in the same cluster placement group (in theory this can
         result in better network between workers, since they'd be physically close to each other in datacenter,
         though we haven't seen this to have much benefit in practice).
     """
 
     keypair_name: Optional[str]
```

### Comparing `coiled-0.7.9.dev9/coiled/utils.py` & `coiled-0.8.0/coiled/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 import ssl
 import string
 import subprocess
 import sys
 import tempfile
 import threading
 import time
+import traceback
 import warnings
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from hashlib import md5
 from logging.config import dictConfig
 from math import ceil
 from pathlib import Path
-from typing import Dict, Iterable, List, NoReturn, Optional, Tuple, Union
+from typing import Dict, Iterable, List, NoReturn, Optional, Set, Tuple, Union
 from urllib.parse import unquote, urlencode, urlparse
 from zipfile import PyZipFile
 
 import backoff
 from packaging.version import Version
 
 from coiled.context import get_datadog_trace_link, track_context
@@ -37,15 +38,16 @@
     from typing import Literal, Type, TypedDict
 else:
     from typing_extensions import Literal, Type, TypedDict
 
 import aiohttp
 import boto3
 import click
-import dask
+import dask.config
+import dask.utils
 import rich
 import urllib3
 import yaml
 from dask.distributed import Security
 from rich.console import Console
 
 from coiled.exceptions import (
@@ -62,15 +64,15 @@
 from coiled.types import AWSOptions, FirewallOptions, GCPOptions
 
 from .compatibility import COILED_VERSION, PY_VERSION
 from .errors import ServerError
 
 logger = logging.getLogger(__name__)
 
-
+COILED_DIR = str(Path(__file__).parent)
 ACCOUNT_REGEX = re.compile(r"^[a-z0-9]+(?:[-_][a-z0-9]+)*$")
 ALLOWED_PROVIDERS = ["aws", "vm_aws", "gcp", "vm_gcp"]
 
 COILED_LOGGER_NAME = "coiled"
 COILED_SERVER = "https://cloud.coiled.io"
 COILED_RUNTIME_REGEX = re.compile(r"^coiled/coiled-runtime-(?P<version>\d+\-\d+\-\d+)-*")
 
@@ -81,14 +83,17 @@
 AWS_UNBALANCED_INSTANCE_FAMILIES_FILTER = ("c5.", "c6i.", "r6i.", "c7g.", "r7g.")
 
 GCP_SCHEDULER_GPU = {
     "scheduler_accelerator_type": "nvidia-tesla-t4",
     "scheduler_accelerator_count": 1,
 }
 
+# Directories to ignore when building wheels from source
+IGNORE_PYTHON_DIRS = {"build", "dist", "docs", "tests"}
+
 
 class VmType(TypedDict):
     """
     Example:
         {
         'name': 't2d-standard-8',
         'cores': 8,
@@ -140,31 +145,31 @@
 
     The normal ``Security`` class assumes credentials already exist on disk,
     but our credentials exist only in memory. Since Python's SSLContext doesn't
     support directly loading credentials from memory, we write them temporarily
     to disk when creating the context, then delete them immediately."""
 
     def __init__(self, tls_key, tls_cert, extra_conn_args: Optional[dict] = None):
-        self.tls_key = tls_key
-        self.tls_cert = tls_cert
+        self.tls_scheduler_key = tls_key
+        self.tls_scheduler_cert = tls_cert
         self.extra_conn_args = extra_conn_args or {}
 
     def __repr__(self):
         return "GatewaySecurity<...>"
 
     def get_connection_args(self, role):
         ctx = None
-        if self.tls_key and self.tls_cert:
+        if self.tls_scheduler_key and self.tls_scheduler_cert:
             with tempfile.TemporaryDirectory() as tempdir:
                 key_path = os.path.join(tempdir, "dask.pem")
                 cert_path = os.path.join(tempdir, "dask.crt")
                 with open(key_path, "w") as f:
-                    f.write(self.tls_key)
+                    f.write(self.tls_scheduler_key)
                 with open(cert_path, "w") as f:
-                    f.write(self.tls_cert)
+                    f.write(self.tls_scheduler_cert)
                 ctx = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH, cafile=cert_path)
                 ctx.verify_mode = ssl.CERT_REQUIRED
                 ctx.check_hostname = False
                 ctx.load_cert_chain(cert_path, key_path)
         return {
             "ssl_context": ctx,
             "require_encryption": True,
@@ -291,14 +296,15 @@
 async def handle_credentials(
     *,
     server: Optional[str] = None,
     token: Optional[str] = None,
     account: Optional[str] = None,
     save: Optional[bool] = None,
     retry: bool = True,
+    print_invalid_token_messages: bool = True,
 ) -> Tuple[str, str, str]:
     """Validate and optionally save credentials
 
     Parameters
     ----------
     server
         Server to connect to. If not specified, will check the
@@ -360,18 +366,19 @@
         try:
             user_dict = await _fetch_data(
                 session=session,
                 server=server,
                 endpoint="/api/v2/user/me",
             )
         except AuthenticationError:
-            rich.print(
-                "[red]Invalid Coiled token encountered. You can create new tokens and manage "
-                f"your existing ones at {server}/profile?createTokenDialog=1 .\n"
-            )
+            if print_invalid_token_messages:
+                rich.print(
+                    "[red]Invalid Coiled token encountered. You can create new tokens and manage "
+                    f"your existing ones at {server}/profile?createTokenDialog=1 .\n"
+                )
             if retry:
                 return await handle_credentials(server=server, token=None, account=account, save=None, retry=False)
             else:
                 raise
         memberships = await _fetch_data(session=session, server=server, endpoint="/api/v2/user/me/memberships")
         if not isinstance(memberships, list) or not memberships:
             account_membership = None
@@ -1356,29 +1363,44 @@
     if http:
         ports.append(80)
     if https:
         ports.append(443)
     return {"ingress": [{"ports": ports, "cidr": cidr}]}
 
 
-async def validate_wheel(wheel: Path) -> Tuple[bool, str]:
+async def validate_wheel(wheel: Path, src: str) -> Tuple[bool, str, Set[str]]:
     """
-    Validate a wheel contains some python files and return
-    the md5
+    Validate a wheel contains some python files and return the md5
+
+    Also, warn if there are Python files in src directory that are not
+    in the wheel.
     """
     hash = md5()
     has_python = False
+    src_path = Path(src)
+    if (src_path / "src").exists():
+        src_path = src_path / "src"
+    src_python_files = set()
+    for p in src_path.rglob("*.py"):
+        relative_path = p.relative_to(src_path)
+        parent_names = {parent.name for parent in relative_path.parents}
+        if not parent_names.intersection(IGNORE_PYTHON_DIRS):
+            src_python_files.add(str(relative_path))
+
     with PyZipFile(str(wheel), mode="r") as wheelzip:
         info = wheelzip.infolist()
         for file in info:
+            src_python_files.discard(file.filename)
+
             if not has_python and file.filename != "__init__.py" and file.filename.endswith(".py"):
                 has_python = True
             if "dist-info" not in file.filename:
                 hash.update(str(file.CRC).encode())
-    return has_python, hash.hexdigest()
+
+    return has_python, hash.hexdigest(), src_python_files
 
 
 def get_aws_identity():
     import boto3
     import botocore
 
     response = {}
@@ -1493,20 +1515,33 @@
     for tb in reversed(frames):
         tb.tb_next = curr
         curr = tb
 
     return curr
 
 
-def error_info_for_tracking(error) -> dict:
-    loc = {
-        "error_class": error.__class__.__name__,
-        "error_message": str(error),
-        "error_filename": "",
-        "error_line": "",
-    }
-    try:
-        loc["error_filename"] = error.__traceback__.tb_next.tb_next.tb_frame.f_code.co_filename
-        loc["error_line"] = str(error.__traceback__.tb_next.tb_next.tb_frame.f_lineno)
-    except Exception:
-        pass
+def error_info_for_tracking(error: Optional[BaseException] = None) -> dict:
+    loc = {}
+    if error:
+        if error.__traceback__:
+            error_trace = "\n".join(
+                [
+                    line if COILED_DIR in line else "...non coiled code..."
+                    for line in traceback.format_tb(error.__traceback__)
+                ]
+            )
+        else:
+            error_trace = None
+        loc = {
+            "error_class": error.__class__.__name__,
+            "error_message": str(error),
+            "error_filename": "",
+            "error_line": "",
+            "error_trace": error_trace,
+        }
+        try:
+            if error.__traceback__:
+                loc["error_filename"] = error.__traceback__.tb_next.tb_next.tb_frame.f_code.co_filename  # type: ignore
+                loc["error_line"] = str(error.__traceback__.tb_next.tb_next.tb_frame.f_lineno)  # type: ignore
+        except Exception:
+            pass
     return loc
```

### Comparing `coiled-0.7.9.dev9/coiled/websockets.py` & `coiled-0.8.0/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/_beta/__init__.py` & `coiled-0.8.0/coiled/v2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from .cluster import Cluster
 from .core import (
-    CloudBeta,
+    CloudV2,
     cluster_details,
     cluster_logs,
     create_cluster,
     delete_cluster,
     list_clusters,
     log_cluster_debug_info,
     setup_logging,
+    better_cluster_logs,
 )
-from ..types import AWSOptions, GCPOptions, BackendOptions
+from ..types import AWSOptions, GCPOptions, BackendOptions, FirewallOptions
 
 __all__ = [
     "AWSOptions",
     "GCPOptions",
+    "FirewallOptions",
     "BackendOptions",
-    "CloudBeta",
+    "CloudV2",
     "cluster_details",
     "cluster_logs",
     "Cluster",
     "create_cluster",
     "delete_cluster",
     "list_clusters",
     "log_cluster_debug_info",
```

### Comparing `coiled-0.7.9.dev9/coiled/_beta/cluster.py` & `coiled-0.8.0/coiled/v2/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,45 +11,46 @@
 import warnings
 import weakref
 from asyncio import wait_for
 from contextlib import suppress
 from copy import deepcopy
 from itertools import chain, islice
 from typing import (
+    Any,
     Awaitable,
     Callable,
+    Coroutine,
     Dict,
     Generic,
     Iterable,
     List,
     Optional,
     Set,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import botocore
-import dask
+import dask.config
 import dask.distributed
-import distributed
+import dask.utils
 from dateutil import tz
 from distributed.core import Status
 from distributed.deploy.adaptive import Adaptive
+from distributed.deploy.cluster import Cluster as DistributedCluster
 from packaging.version import Version
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, TextColumn, TimeElapsedColumn
 from typing_extensions import Literal, TypeAlias
 from urllib3.util import parse_url
 
 from coiled import magic
-from coiled._beta.widgets.rich import CONSOLE_WIDTH
-from coiled._beta.widgets.util import simple_progress
 from coiled.cluster import CoiledAdaptive, CredentialsPreferred
 from coiled.compatibility import DISTRIBUTED_VERSION
 from coiled.context import track_context
 from coiled.core import IsAsynchronous
 from coiled.errors import ClusterCreationError, DoesNotExist
 from coiled.exceptions import ArgumentCombinationError, InstanceTypeError
 from coiled.types import ArchitectureTypesEnum, AWSOptions, GCPOptions, PackageLevel, PackageLevelEnum
@@ -67,29 +68,31 @@
     parse_wait_for_workers,
     truncate_traceback,
     validate_vm_typing,
 )
 
 from ..core import Async, AWSSessionCredentials, Sync
 from .core import (
-    CloudBeta,
-    CloudBetaSyncAsync,
+    CloudV2,
+    CloudV2SyncAsync,
     log_cluster_debug_info,
     setup_logging,
 )
 from .cwi_log_link import cloudwatch_url
 from .states import (
     ClusterStateEnum,
     InstanceStateEnum,
     ProcessStateEnum,
     flatten_log_states,
     log_states,
     summarize_status,
 )
 from .widgets import EXECUTION_CONTEXT, HAS_RICH
+from .widgets.rich import CONSOLE_WIDTH
+from .widgets.util import simple_progress
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 
 _T = TypeVar("_T")
 
 
 def use_rich_widget():
@@ -105,21 +108,22 @@
 
 _vm_type_cpu_memory_error_msg = (
     "Argument '{kind}_vm_types' can't be used together with '{kind}_cpu' or '{kind}_memory'. "
     "Please use either '{kind}_vm_types' or '{kind}_cpu'/'{kind}_memory' separately."
 )
 
 
-class Cluster(distributed.deploy.Cluster, Generic[IsAsynchronous]):
+class Cluster(DistributedCluster, Generic[IsAsynchronous]):
     """Create a Dask cluster with Coiled
 
     Parameters
     ----------
     n_workers
         Number of workers in this cluster. Defaults to 4.
+        If argument this is not specified, adaptive scaling is enabled.
     name
         Name to use for identifying this cluster. Defaults to ``None``.
     software
         Name of the software environment to use; this allows you to use and re-use existing
         Coiled software environments, and should not be used with package sync or when specifying
         a container to use for this specific cluster.
     container
@@ -142,16 +146,19 @@
     worker_memory
         Amount of memory to request for each worker, Coiled will use a +/- 10% buffer
         from the memory that you specify. You may specify a range of memory by using a
         list of two elements, for example: ``worker_memory=["2GiB", "4GiB"]``.
     worker_disk_size
         Non-default size of persistent disk attached to each worker instance, specified
         in GB.
+    worker_disk_throughput
+        EXPERIMENTAL. For AWS, non-default throughput (in MB/s) for EBS gp3 volumes attached
+        to workers.
     worker_gpu
-        Number of GPUs to attach to each worker. Default is 0, ``True`` is interpretted as 1.
+        Number of GPUs to attach to each worker. Default is 0, ``True`` is interpreted as 1.
         Note that this is ignored if you're explicitly specifying an instance type which
         includes a fixed number of GPUs.
     worker_gpu_type
         For GCP, this lets you specify type of guest GPU for instances.
         Should match the way the cloud provider specifies the GPU, for example:
         ``worker_gpu_type="nvidia-tesla-t4"``.
         By default, Coiled will request NVIDIA T4 if GPU type isn't specified.
@@ -237,16 +244,16 @@
         down, then a TimeoutError is raised.
     package_sync
         Synchronize package versions between your local environment and the cluster.
         Cannot be used with the ``software`` option. Passing ``True`` will sync all packages (recommended).
         If ``software`` is not given, defaults to True.
         Passing specific packages as a list of strings will attempt to synchronize only those packages,
         use with caution.
-        We strongly recommend reading the additional documentation
-        for this feature (see https://docs.coiled.io/user_guide/package_sync.html)!
+        We recommend reading the
+        `additional documentation for this feature <https://docs.coiled.io/user_guide/package_sync.html>`_
     package_sync_ignore
         A list of package names to exclude from the environment. Note their dependencies may still be installed,
         or they may be installed by another package that depends on them!
     package_sync_strict
         Only allow exact packages matches, not recommended unless your client platform/architecture
         matches the cluster platform/architecture
     private_to_creator
@@ -294,31 +301,32 @@
 
     def __init__(
         self: ClusterSyncAsync,
         name: Optional[str] = None,
         *,
         software: Optional[str] = None,
         container: Optional[str] = None,
-        n_workers: int = 4,
+        n_workers: Optional[int] = None,
         worker_class: Optional[str] = None,
         worker_options: Optional[dict] = None,
         worker_vm_types: Optional[list] = None,
         worker_cpu: Optional[Union[int, List[int]]] = None,
         worker_memory: Optional[Union[str, List[str]]] = None,
         worker_disk_size: Optional[int] = None,
+        worker_disk_throughput: Optional[int] = None,
         worker_gpu: Optional[Union[int, bool]] = None,
         worker_gpu_type: Optional[str] = None,
         scheduler_class: Optional[str] = None,
         scheduler_options: Optional[dict] = None,
         scheduler_vm_types: Optional[list] = None,
         scheduler_cpu: Optional[Union[int, List[int]]] = None,
         scheduler_memory: Optional[Union[str, List[str]]] = None,
         scheduler_gpu: Optional[bool] = None,
         asynchronous: bool = False,
-        cloud: Optional[CloudBeta] = None,
+        cloud: Optional[CloudV2] = None,
         account: Optional[str] = None,
         shutdown_on_close=None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         credentials: Optional[str] = "local",
         credentials_duration_seconds: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
@@ -340,14 +348,23 @@
         scheduler_port: Optional[int] = None,
         allow_ingress_from: Optional[str] = None,
         allow_ssh: Optional[bool] = None,
         jupyter: Optional[bool] = None,
         region: Optional[str] = None,
         arm: Optional[bool] = None,
     ):
+        if n_workers is None:
+            # local variable instead of instance attribute would work fine,
+            # except that I want to send this to mix panel, and self._as_json_compatible
+            # wants to look at instance attributes
+            self.start_adaptive = True
+            n_workers = 4
+        else:
+            self.start_adaptive = False
+
         # NOTE:
         # this attribute is only updated while we wait for cluster to come up
         self.errored_worker_count: int = 0
         self.init_time = datetime.datetime.now()
         type(self)._instances.add(self)
 
         senv_kwargs = {"package_sync": package_sync, "software": software, "container": container}
@@ -408,21 +425,21 @@
 
             asynchronous = cloud.asynchronous
 
         self.scheduler_comm: Optional[dask.distributed.rpc] = None
 
         # It's annoying that the user must pass in `asynchronous=True` to get an async Cluster object
         # But I can't think of a good alternative right now.
-        self.cloud: CloudBetaSyncAsync = cloud or CloudBeta.current(asynchronous=asynchronous)
+        self.cloud: CloudV2SyncAsync = cloud or CloudV2.current(asynchronous=asynchronous)
         # if cloud:
         #     self.cleanup_cloud = False
-        #     self.cloud: CloudBeta[IsAsynchronous] = cloud
+        #     self.cloud: CloudV2[IsAsynchronous] = cloud
         # else:
         #     self.cleanup_cloud = True
-        #     self.cloud: CloudBeta[IsAsynchronous] = CloudBeta(asynchronous=asynchronous)
+        #     self.cloud: CloudV2[IsAsynchronous] = CloudV2(asynchronous=asynchronous)
 
         # As of distributed 2021.12.0, deploy.Cluster has a ``loop`` attribute on the
         # base class. We add the attribute manually here for backwards compatibility.
         # TODO: if/when we set the minimum distributed version to be >= 2021.12.0,
         # remove this check.
         if DISTRIBUTED_VERSION >= Version("2021.12.0"):
             kwargs = {"loop": self.cloud.loop}
@@ -461,14 +478,15 @@
             elif worker_cpu < 1:
                 raise ValueError("`worker_cpu` should be at least 1 for arm instance types.")
 
         self.worker_memory = worker_memory or dask.config.get("coiled.worker.memory")
         # FIXME get these from dask config
         self.worker_vm_types = worker_vm_types
         self.worker_disk_size = worker_disk_size
+        self.worker_disk_throughput = worker_disk_throughput
         self.worker_gpu_count = int(worker_gpu) if worker_gpu is not None else None
         self.worker_gpu_type = worker_gpu_type
         self.worker_options = {
             **(cast(dict, dask.config.get("coiled.worker-options", {}))),
             **(worker_options or {}),
         }
 
@@ -613,14 +631,33 @@
                         self.cloud.add_interaction,
                         "cluster-create",
                         success=True,
                         additional_data={
                             **self._as_json_compatible(),
                         },
                     )
+            if self.start_adaptive:
+                adaptive_max = 20
+                logger.warn(
+                    f"""n_workers was not specified so turning on adaptive scaling with a min
+of {n_workers} and max of {adaptive_max}.
+
+To specify a specific cluster size:
+
+    cluster = coiled.Cluster(n_workers=100, ...)
+
+Alternatively, to control adaptive scaling:
+
+    cluster = coiled.Cluster(...)
+    cluster.adapt(minimum=0, maximum=100)
+
+For more information, see: https://docs.coiled.io/user_guide/clusters/size-and-type.html. and https://docs.coiled.io/user_guide/clusters/scale.html#adaptive-scaling.
+"""
+                )
+                self.adapt(minimum=n_workers, maximum=adaptive_max)
 
     @property
     def details_url(self):
         return get_details_url(self.cloud.server, self.account, self.cluster_id)
 
     @property
     def _grafana_url(self) -> Optional[str]:
@@ -900,15 +937,30 @@
                 if package_level["level"] > self.package_sync_fail_on or self.package_sync_strict:
                     halting_failures.append(package)
         if halting_failures:
             # fall back to the note if no error is present
             # this only really happens if a user specified
             # a critical package to ignore
             failure_str = ", ".join([f'{pkg["name"]} - {pkg["error"] or pkg["note"]}' for pkg in halting_failures])
-            raise RuntimeError(f"Issues with critical packages: {failure_str}")
+            raise RuntimeError(
+                f"""Issues with critical packages: {failure_str}
+
+Your software environment has conflicting dependency requirements. In this situation, Coiled recommends creating a
+new environment. By specifying your list of desired packages together, you're much more likely to get a set of
+consistent versions.
+
+If you use conda:
+    conda create -n myenv -c conda-forge coiled package1 package2 package3
+
+If you use pip/venv, create a new environment and then:
+    pip install coiled package1 package2 package3
+or
+    pip install -r requirements.txt
+"""
+            )
 
     @track_context
     async def _attach_to_cluster(self, is_new_cluster: bool):
         # update our view of workers in case someone tries scaling
         # it might be better to continually update this while waiting for the
         # cluster in _security below, but this seems OK for now
         assert self.cluster_id
@@ -1105,14 +1157,15 @@
                     account=self.account,
                     name=self.name,
                     workers=self._start_n_workers,
                     software_environment=self.software_environment,
                     worker_class=self.worker_class,
                     worker_options=self.worker_options,
                     worker_disk_size=self.worker_disk_size,
+                    worker_disk_throughput=self.worker_disk_throughput,
                     gcp_worker_gpu_type=self.worker_gpu_type,
                     gcp_worker_gpu_count=self.worker_gpu_count,
                     scheduler_class=self.scheduler_class,
                     scheduler_options=self.scheduler_options,
                     environ=self.environ,
                     tags=self.tags,
                     dask_config=self.frozen_dask_config,
@@ -1197,14 +1250,15 @@
             "timeout": self.timeout,
             "wait_for_workers": self._wait_for_workers_arg,
             "cluster_id": self.cluster_id,
             "backend_options": self.backend_options,
             "scheduler_gpu": self.scheduler_gpu,
             "use_best_zone": self.use_best_zone,
             "compute_purchase_option": self.compute_purchase_option,
+            "start_adaptive": self.start_adaptive,
             "errored_worker_count": self.errored_worker_count,
             # NOTE: this is not a measure of the CLUSTER life time
             # just a measure of how long this object has been around
             "cluster_object_life": str(datetime.datetime.now() - self.init_time),
         }
 
     def _maybe_log_summary(self, cluster_details):
@@ -1484,15 +1538,15 @@
 
     @track_context
     async def _close(self, force_shutdown: bool = False) -> None:
         # My small changes to _close probably make sense for legacy Cluster too, but I don't want to carefully
         # test them, so copying this method over.
 
         with suppress(AttributeError):
-            self._adaptive.stop()
+            self._adaptive.stop()  # type: ignore
 
         # Stop here because otherwise we get intermittent `OSError: Timed out` when
         # deleting cluster takes a while and callback tries to poll cluster status.
         for pc in self.periodic_callbacks.values():
             pc.stop()
 
         if hasattr(self, "cluster_id") and self.cluster_id:
@@ -1529,31 +1583,34 @@
     def sync(
         self: Cluster[Async],
         func: Callable[..., Awaitable[_T]],
         *args,
         asynchronous: Union[bool, Literal[None]] = None,
         callback_timeout=None,
         **kwargs,
-    ) -> Awaitable[_T]:
+    ) -> Coroutine[Any, Any, _T]:
         ...
 
     def sync(
         self,
         func: Callable[..., Awaitable[_T]],
         *args,
         asynchronous: Optional[bool] = None,
         callback_timeout=None,
         **kwargs,
-    ) -> Union[_T, Awaitable[_T]]:
-        return super().sync(
-            func,
-            *args,
-            asynchronous=asynchronous,
-            callback_timeout=callback_timeout,
-            **kwargs,
+    ) -> Union[_T, Coroutine[Any, Any, _T]]:
+        return cast(
+            Union[_T, Coroutine[Any, Any, _T]],
+            super().sync(
+                func,
+                *args,
+                asynchronous=asynchronous,
+                callback_timeout=callback_timeout,
+                **kwargs,
+            ),
         )
 
     def _ensure_scheduler_comm(self) -> dask.distributed.rpc:
         """
         Guard to make sure that the scheduler comm exists before trying to use it.
         """
         if not self.scheduler_comm:
@@ -1567,15 +1624,15 @@
         timeout=None,
         err_msg=None,
     ) -> None:
         if timeout is None:
             deadline = None
         else:
             timeout = dask.utils.parse_timedelta(timeout, "s")
-            deadline = time.time() + timeout
+            deadline = time.time() + timeout if timeout else None
         while n_workers and len(self.scheduler_info["workers"]) < n_workers:
             if deadline and time.time() > deadline:
                 err_msg = err_msg or (
                     f"Timed out after {timeout} seconds waiting for {n_workers} workers to arrive, "
                     "check your notifications with coiled.get_notifications() for further details"
                 )
                 raise TimeoutError(err_msg)
@@ -1717,20 +1774,21 @@
                                         f"Locally generated AWS STS token expires in less than 5 minutes ({diff}). "
                                         "Code running on your cluster may be unable to access other AWS services "
                                         "(e.g, S3) when this token expires."
                                     )
 
                                 # don't try to update sooner than in 1 minute
                                 delay = max(60, delay)
-
-                        self.loop.call_later(delay=delay, callback=self._send_credentials)
-                        logger.debug(
-                            "AWS STS token from local credentials shipped to cluster, "
-                            f"planning to refresh in {delay} seconds"
-                        )
+                        if self.loop:
+                            # should never be None but distributed baseclass claims it can be
+                            self.loop.call_later(delay=delay, callback=self._send_credentials)
+                            logger.debug(
+                                "AWS STS token from local credentials shipped to cluster, "
+                                f"planning to refresh in {delay} seconds"
+                            )
                     else:
                         logger.debug("AWS STS token from local credentials shipped to cluster, no scheduled refresh")
 
             except Exception as e:
                 terminating_states = (
                     Status.closing,
                     Status.closed,
@@ -1799,15 +1857,15 @@
         """
         return self.sync(self._scale, n=n)
 
     @track_context
     async def scale_down(self, workers: set, reason: Optional[str] = None) -> None:
         if not self.cluster_id:
             raise ValueError("No cluster available to scale!")
-        cloud = cast(CloudBeta[Async], self.cloud)
+        cloud = cast(CloudV2[Async], self.cloud)
         try:
             scheduler_comm = self._ensure_scheduler_comm()
             await scheduler_comm.retire_workers(
                 names=workers,
                 remove=True,
                 close_workers=True,
             )
@@ -1843,15 +1901,15 @@
             to_close.update(islice(not_yet_arrived, len(plan) - target))
 
         if target < len(plan) - len(to_close):
             L = await self.workers_to_close(target=target)
             to_close.update(L)
         return {"status": "down", "workers": list(to_close)}
 
-    async def workers_to_close(self, target: int):
+    async def workers_to_close(self, target: int) -> List[str]:
         """
         Determine which, if any, workers should potentially be removed from
         the cluster.
 
         Notes
         -----
         ``Cluster.workers_to_close`` dispatches to Scheduler.workers_to_close(),
@@ -1866,30 +1924,28 @@
         Scheduler.workers_to_close
         """
         scheduler_comm = self._ensure_scheduler_comm()
         ret = await scheduler_comm.workers_to_close(
             target=target,
             attribute="name",
         )
-        return ret
+        return ret  # type: ignore
 
     def adapt(self, Adaptive=CoiledAdaptive, **kwargs) -> Adaptive:
         """Dynamically scale the number of workers in the cluster
         based on scaling heuristics.
 
         Parameters
         ----------
         minimum : int
             Minimum number of workers that the cluster should have while
             on low load, defaults to 1.
         maximum : int
             Maximum numbers of workers that the cluster should have while
-            on high load. If maximum is not set, this value will be based
-            on your core count limit. This value is also capped by your
-            core count limit.
+            on high load.
         wait_count : int
             Number of consecutive times that a worker should be suggested
             for removal before the cluster removes it, defaults to 60.
         interval : timedelta or str
             Milliseconds between checks, defaults to 5000 ms.
         target_duration : timedelta or str
             Amount of time we want a computation to take. This affects how
@@ -1931,15 +1987,15 @@
         """
         return self.sync(self._get_logs, scheduler=scheduler, workers=workers)
 
     @track_context
     async def _get_logs(self, scheduler: bool = True, workers: bool = True) -> dict:
         if not self.cluster_id:
             raise ValueError("No cluster available for logs!")
-        cloud = cast(CloudBeta[Async], self.cloud)
+        cloud = cast(CloudV2[Async], self.cloud)
         return await cloud.cluster_logs(
             cluster_id=self.cluster_id,
             account=self.account,
             scheduler=scheduler,
             workers=workers,
         )
```

### Comparing `coiled-0.7.9.dev9/coiled/_beta/core.py` & `coiled-0.8.0/coiled/v2/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     Tuple,
     Union,
     cast,
     overload,
 )
 
 import backoff
-import dask
+import dask.config
+import dask.distributed
 from aiohttp import ClientResponseError, ClientSession, ContentTypeError
 from dask.utils import parse_timedelta
 from distributed.utils import Log, Logs
 from rich.progress import Progress
 from typing_extensions import TypeAlias
 
-from coiled._beta.widgets.util import simple_progress
 from coiled.cli.setup.entry import do_setup_wizard
 from coiled.context import track_context
 from coiled.core import Async, IsAsynchronous, Sync, delete_docstring, list_docstring
 from coiled.core import Cloud as OldCloud
 from coiled.errors import ClusterCreationError, DoesNotExist, ServerError
 from coiled.types import (
     ApproximatePackageRequest,
@@ -60,14 +60,15 @@
 from .states import (
     InstanceStateEnum,
     ProcessStateEnum,
     flatten_log_states,
     get_process_instance_state,
     log_states,
 )
+from .widgets.util import simple_progress
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 
 
 def setup_logging(level=logging.INFO):
     # We want to be able to give info-level messages to users.
     # For users who haven't set up a log handler, this requires creating one (b/c the handler of "last resort,
@@ -96,58 +97,58 @@
     if "message" in error_body:
         raise exception_cls(error_body["message"])
     if "detail" in error_body:
         raise exception_cls(error_body["detail"])
     raise exception_cls(error_body)
 
 
-CloudBetaSyncAsync: TypeAlias = Union["CloudBeta[Async]", "CloudBeta[Sync]"]
+CloudV2SyncAsync: TypeAlias = Union["CloudV2[Async]", "CloudV2[Sync]"]
 
 
-class CloudBeta(OldCloud, Generic[IsAsynchronous]):
-    _recent_sync: List[weakref.ReferenceType[CloudBeta[Sync]]] = list()
-    _recent_async: List[weakref.ReferenceType[CloudBeta[Async]]] = list()
+class CloudV2(OldCloud, Generic[IsAsynchronous]):
+    _recent_sync: List[weakref.ReferenceType[CloudV2[Sync]]] = list()
+    _recent_async: List[weakref.ReferenceType[CloudV2[Async]]] = list()
 
-    # just overriding to get the right signature (CloudBeta, not Cloud)
-    def __enter__(self: CloudBeta[Sync]) -> CloudBeta[Sync]:
+    # just overriding to get the right signature (CloudV2, not Cloud)
+    def __enter__(self: CloudV2[Sync]) -> CloudV2[Sync]:
         return self
 
-    def __exit__(self: CloudBeta[Sync], typ, value, tb) -> None:
+    def __exit__(self: CloudV2[Sync], typ, value, tb) -> None:
         self.close()
 
-    async def __aenter__(self: CloudBeta[Async]) -> CloudBeta[Async]:
+    async def __aenter__(self: CloudV2[Async]) -> CloudV2[Async]:
         return await self._start()
 
-    async def __aexit__(self: CloudBeta[Async], typ, value, tb) -> None:
+    async def __aexit__(self: CloudV2[Async], typ, value, tb) -> None:
         await self._close()
 
-    # these overloads are necessary for the typechecker to know that we really have a CloudBeta, not a Cloud
-    # without them, CloudBeta.current would be typed to return a Cloud
+    # these overloads are necessary for the typechecker to know that we really have a CloudV2, not a Cloud
+    # without them, CloudV2.current would be typed to return a Cloud
     #
     # https://www.python.org/dev/peps/pep-0673/ would remove the need for this.
     # That PEP also mentions a workaround with type vars, which doesn't work for us because type vars aren't
     # subscribtable
     @overload
     @classmethod
-    def current(cls, asynchronous: Sync) -> CloudBeta[Sync]:
+    def current(cls, asynchronous: Sync) -> CloudV2[Sync]:
         ...
 
     @overload
     @classmethod
-    def current(cls, asynchronous: Async) -> CloudBeta[Async]:
+    def current(cls, asynchronous: Async) -> CloudV2[Async]:
         ...
 
     @overload
     @classmethod
-    def current(cls, asynchronous: bool) -> CloudBeta:
+    def current(cls, asynchronous: bool) -> CloudV2:
         ...
 
     @classmethod
-    def current(cls, asynchronous: bool) -> CloudBeta:
-        recent: List[weakref.ReferenceType[CloudBeta]]
+    def current(cls, asynchronous: bool) -> CloudV2:
+        recent: List[weakref.ReferenceType[CloudV2]]
         if asynchronous:
             recent = cls._recent_async
         else:
             recent = cls._recent_sync
         try:
             cloud = recent[-1]()
             while cloud is None or cloud.status != "running":
@@ -614,14 +615,15 @@
         tags: Optional[Dict] = None,
         dask_config: Optional[Dict] = None,
         scheduler_vm_types: Optional[list] = None,
         gcp_worker_gpu_type: Optional[str] = None,
         gcp_worker_gpu_count: Optional[int] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
+        worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[AWSOptions, GCPOptions, dict]] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         private_to_creator: Optional[bool] = None,
     ) -> Tuple[int, bool]:
         # TODO (Declarative): support these args, or decide not to
         # https://gitlab.com/coiled/cloud/-/issues/4305
@@ -642,14 +644,15 @@
             "name": name,
             "workers": workers,
             "worker_instance_types": worker_vm_types,
             "scheduler_instance_types": scheduler_vm_types,
             "worker_options": worker_options,
             "worker_class": worker_class,
             "worker_disk_size": worker_disk_size,
+            "worker_disk_throughput": worker_disk_throughput,
             "scheduler_options": scheduler_options,
             "environ": environ,
             "tags": tags,
             "dask_config": dask_config,
             "private_to_creator": private_to_creator,
             "env_id": senv_v2_id,
             "env_name": software_environment,
@@ -759,14 +762,15 @@
         tags: Optional[Dict] = None,
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
+        worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
     ) -> Tuple[int, bool]:
         ...
 
     @overload
     def create_cluster(
         self: Cloud[Async],
@@ -783,14 +787,15 @@
         tags: Optional[Dict] = None,
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
+        worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
     ) -> Awaitable[Tuple[int, bool]]:
         ...
 
     def create_cluster(
         self,
         name: str,
@@ -806,14 +811,15 @@
         tags: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         dask_config: Optional[Dict] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
+        worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
     ) -> Union[Tuple[int, bool], Awaitable[Tuple[int, bool]]]:
         return self._sync(
             self._create_cluster,
             name=name,
             software_environment=software,
             worker_class=worker_class,
@@ -826,14 +832,15 @@
             tags=tags,
             dask_config=dask_config,
             private_to_creator=private_to_creator,
             scheduler_vm_types=scheduler_vm_types,
             worker_vm_types=worker_vm_types,
             gcp_worker_gpu_type=worker_gpu_type,
             worker_disk_size=worker_disk_size,
+            worker_disk_throughput=worker_disk_throughput,
             backend_options=backend_options,
         )
 
     @track_context
     async def _delete_cluster(self, cluster_id: int, account: Optional[str] = None) -> None:
         account = account or self.default_account
 
@@ -1103,26 +1110,26 @@
             await handle_api_exception(response)
 
         cluster = await response.json()
         return cluster
 
     @overload
     def cluster_logs(
-        self,
+        self: Cloud[Sync],
         cluster_id: int,
         account: Optional[str] = None,
         scheduler: bool = True,
         workers: bool = True,
         errors_only: bool = False,
     ) -> Logs:
         ...
 
     @overload
     def cluster_logs(
-        self,
+        self: Cloud[Async],
         cluster_id: int,
         account: Optional[str] = None,
         scheduler: bool = True,
         workers: bool = True,
         errors_only: bool = False,
     ) -> Awaitable[Logs]:
         ...
@@ -1408,15 +1415,15 @@
     def security(
         self: Cloud[Async], cluster_id: int, account: Optional[str] = None
     ) -> Awaitable[Tuple[dask.distributed.Security, dict]]:
         ...
 
     def security(
         self, cluster_id: int, account: Optional[str] = None
-    ) -> Union[Tuple[dask.distributed.Security, dict], Awaitable[Tuple[dask.distribued.Security, dict]],]:
+    ) -> Union[Tuple[dask.distributed.Security, dict], Awaitable[Tuple[dask.distributed.Security, dict]],]:
         return self._sync(self._security, cluster_id, account)
 
     @track_context
     async def _fetch_package_levels(self) -> List[PackageLevel]:
         pass
         response = await self._do_request(
             "GET",
@@ -1507,15 +1514,15 @@
 
         return self._sync(
             get_result,
             response,
         )
 
 
-Cloud = CloudBeta
+Cloud = CloudV2
 
 
 def cluster_logs(
     cluster_id: int,
     account: Optional[str] = None,
     scheduler: bool = True,
     workers: bool = True,
@@ -1565,26 +1572,26 @@
 def cluster_details(
     cluster_id: int,
     account: Optional[str] = None,
 ) -> dict:
     """
     Get details of a cluster as a dictionary.
     """
-    with CloudBeta() as cloud:
+    with CloudV2() as cloud:
         return cloud.cluster_details(
             cluster_id=cluster_id,
             account=account,
         )
 
 
 def log_cluster_debug_info(
     cluster_id: int,
     account: Optional[str] = None,
 ):
-    with CloudBeta() as cloud:
+    with CloudV2() as cloud:
         details = cloud.cluster_details(cluster_id, account)
         logger.debug("Cluster details:")
         logger.debug(json.dumps(details, indent=2))
 
         states_by_type = cloud.get_cluster_states(cluster_id, account)
 
         logger.debug("cluster state history:")
@@ -1602,14 +1609,15 @@
     environ: Optional[Dict] = None,
     tags: Optional[Dict] = None,
     dask_config: Optional[Dict] = None,
     private_to_creator: Optional[bool] = None,
     scheduler_vm_types: Optional[list] = None,
     worker_vm_types: Optional[list] = None,
     worker_disk_size: Optional[int] = None,
+    worker_disk_throughput: Optional[int] = None,
     backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
 ) -> int:
     """Create a cluster
 
     Parameters
     ---------
     name
@@ -1639,39 +1647,40 @@
     dask_config
         Dictionary of dask config to put on cluster
 
     See Also
     --------
     coiled.Cluster
     """
-    with CloudBeta(account=account) as cloud:
+    with CloudV2(account=account) as cloud:
         cluster, existing = cloud.create_cluster(
             name=name,
             software=software,
             worker_options=worker_options,
             scheduler_options=scheduler_options,
             account=account,
             workers=workers,
             environ=environ,
             tags=tags,
             dask_config=dask_config,
             private_to_creator=private_to_creator,
             backend_options=backend_options,
             worker_vm_types=worker_vm_types,
             worker_disk_size=worker_disk_size,
+            worker_disk_throughput=worker_disk_throughput,
             scheduler_vm_types=scheduler_vm_types,
         )
         return cluster
 
 
 @list_docstring
 def list_clusters(account=None, max_pages: Optional[int] = None):
-    with CloudBeta() as cloud:
+    with CloudV2() as cloud:
         return cloud.list_clusters(account=account, max_pages=max_pages)
 
 
 @delete_docstring
 def delete_cluster(name: str, account: Optional[str] = None):
-    with CloudBeta() as cloud:
+    with CloudV2() as cloud:
         cluster_id = cloud.get_cluster_by_name(name=name, account=account)
         if cluster_id is not None:
             return cloud.delete_cluster(cluster_id=cluster_id, account=account)
```

### Comparing `coiled-0.7.9.dev9/coiled/_beta/cwi_log_link.py` & `coiled-0.8.0/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/_beta/states.py` & `coiled-0.8.0/coiled/v2/states.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 class BaseStateEnum(str, Enum):
     """
     Abstract class intended to be used for all state Enums
     inherits from str for easy comparisons
     """
 
+    # important for 3.11 compatibility
+    def __str__(self) -> str:
+        return self.value
+
 
 class ClusterStateEnum(BaseStateEnum):
     """
     Valid states for Clusters
     """
 
     pending = "pending"
@@ -80,14 +84,18 @@
     cluster = "cluster"
     scheduler = "scheduler"
     scheduler_instance = "scheduler_instance"
     cluster_infra = "cluster_infra"
     worker = "worker"
     worker_instance = "worker_instance"
 
+    # important for 3.11 compatibility
+    def __str__(self) -> str:
+        return self.value
+
 
 class State(NamedTuple):
     type: StatefulObjectType
     updated: datetime
     name: str
     state: str
     reason: str
```

### Comparing `coiled-0.7.9.dev9/coiled/_beta/widgets/__init__.py` & `coiled-0.8.0/coiled/v2/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Status display widgets for Coiled cluster instances.
 
 Each widget implementation must have an ``update()`` instance method that takes two
 arguments. The first argument is the JSON response from the declarative
 ``/api/v2/clusters/account/{account}/id/{cluster_id}`` endpoint, parsed into a
-dictionary. The second argument is a list of `coiled._beta.states.State` instances
+dictionary. The second argument is a list of `coiled.v2.states.State` instances
 that contain the state changes of the cluster, scheduler, and workers.
 
 The widget implementation is then responsible for drawing itself to the environment.
 Current implementations support Jupyter Notebook-like contexts and IPython console
 contexts via the ``_ipython_display_`` and ``_repr_mimebundle_`` methods.
 
 Please avoid adding unconditional dependencies on rendering or widget libraries, so
```

### Comparing `coiled-0.7.9.dev9/coiled/_beta/widgets/rich.py` & `coiled-0.8.0/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/_beta/widgets/util.py` & `coiled-0.8.0/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/config.py` & `coiled-0.8.0/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/core.py` & `coiled-0.8.0/coiled/cli/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import click
 
 from ..compatibility import COILED_VERSION
+from .authenticate import authenticate
 from .cluster import cluster
 from .config import config
 from .curl import curl
 from .diagnostics import diagnostics
 from .env import env
 from .login import login
 from .notebook import notebook
 from .package_sync import package_sync
+from .prefect import prefect
 from .run import run
 from .setup import setup
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
@@ -25,10 +27,12 @@
 cli.add_command(login)
 cli.add_command(env)
 cli.add_command(diagnostics)
 cli.add_command(setup)
 cli.add_command(cluster)
 cli.add_command(notebook)
 cli.add_command(package_sync)
+cli.add_command(prefect)
 cli.add_command(curl)
 cli.add_command(config)
 cli.add_command(run)
+cli.add_command(authenticate)
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/curl.py` & `coiled-0.8.0/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/env.py` & `coiled-0.8.0/coiled/cli/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from dask import config
 from rich.console import Console
 from rich.table import Table
 
-from coiled._beta.core import setup_logging
 from coiled.exceptions import BuildError
 from coiled.types import ArchitectureTypesEnum
+from coiled.v2.core import setup_logging
 
 from ..core import Cloud, create_software_environment, delete_software_environment
 from ..utils import COILED_SERVER
 from .utils import CONTEXT_SETTINGS
 
 console = Console()
 
@@ -107,20 +107,22 @@
         table.add_column("Status", style="green")
         server = config.get("coiled.server", COILED_SERVER).replace("8000", "5173")
         account = account or config.get("coiled.account")
         for env_name, env_details in environments.items():
             latest_build = env_details["latest_spec"].get("latest_build")
             if latest_build:
                 build_status = latest_build["state"] if latest_build["state"] != "error" else "[red]error[/red]"
+                env_url = f"{server}/software/alias/{env_details['id']}/build/{latest_build['id']}?account={account}"
             else:
                 build_status = "n/a"
+                env_url = f"{server}/software/alias/{env_details['id']}?account={account}"
             table.add_row(
                 env_name,
                 env_details["updated"],
-                f"{server}/software/{env_details['id']}/latest?account={account}",
+                env_url,
                 build_status,
             )
         console.print(table)
 
 
 @env.command(
     context_settings=CONTEXT_SETTINGS,
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/login.py` & `coiled-0.8.0/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/package_sync.py` & `coiled-0.8.0/coiled/cli/package_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,83 @@
 import asyncio
 import logging
-import pkgutil
 import sys
 from csv import writer as csv_writer
 from logging import basicConfig
 from pathlib import Path
 
 import click
 from rich.console import Console
-from rich.panel import Panel
 from rich.table import Table
 
 from coiled.scan import scan_prefix
+from coiled.utils import IGNORE_PYTHON_DIRS
 
 
 @click.group()
 def package_sync():
     basicConfig(level=logging.INFO)
 
 
 @package_sync.command()
 @click.option("--csv", is_flag=True, default=False, help="Output as CSV")
-def scan(csv: bool):
+@click.option("--verbose", "-v", is_flag=True, default=False, help="Output files that will end up in wheels")
+def scan(csv: bool, verbose: bool):
     result = asyncio.run(scan_prefix(Path(sys.prefix)))
     table = Table(title="Packages")
     table.add_column("Package Name", style="cyan", no_wrap=True)
     table.add_column("Conda Name", style="cyan", no_wrap=True)
     table.add_column("Version", style="magenta")
     table.add_column("Source", style="magenta")
     table.add_column("Channel", style="magenta", overflow="fold")
     table.add_column("Channel URL", style="magenta", overflow="fold")
     table.add_column("Wheel target", style="green", overflow="fold")
     table.add_column("Path", overflow="fold")
-    table.add_column("Can build wheel", style="green")
+    if verbose:
+        table.add_column("Python modules", overflow="fold")
     rows = []
     for pkg in result:
-        rows.append(
-            [
-                pkg["name"],
-                pkg["conda_name"],
-                pkg["version"],
-                pkg["source"],
-                pkg["channel"] or "",
-                pkg["channel_url"] or "",
-                pkg["wheel_target"] or "",
-                str(pkg["path"]) if pkg["path"] else "",
-                True,
-            ]
-        )
-
-    for _, name, ispkg in pkgutil.iter_modules(path=["."]):
-        will_sync = False
-        if ispkg:
-            for pkg in result:
-                if pkg["path"]:
-                    if (pkg["path"] / name).resolve() == (Path(".") / name).resolve():  # type: ignore
-                        will_sync = True
-        if not will_sync:
-            rows.append(
-                [
-                    name,
-                    "",
-                    "",
-                    "cwd",
-                    "",
-                    "",
-                    str(Path(".") / name) if ispkg else str((Path(".") / name).with_suffix(".py")),
-                    False,
-                ]
-            )
+        row = [
+            pkg["name"],
+            pkg["conda_name"],
+            pkg["version"],
+            pkg["source"],
+            pkg["channel"] or "",
+            pkg["channel_url"] or "",
+            pkg["wheel_target"] or "",
+            str(pkg["path"]) if pkg["path"] else "",
+        ]
+        if verbose:
+            if pkg["name"].startswith("coiled_local_") and pkg["path"]:
+                modules = []
+                for path in pkg["path"].rglob("*.py"):
+                    relative_path = path.relative_to(pkg["path"])
+                    parent_names = {parent.name for parent in relative_path.parents}
+                    if not parent_names.intersection(IGNORE_PYTHON_DIRS) and str(relative_path) not in (
+                        "__init__.py",
+                        "__main__.py",
+                    ):
+                        modules.append(str(relative_path))
+                row.append("\n".join(modules))
+            else:
+                row.append("")
+
+        rows.append(row)
+
     rows = sorted(rows, key=lambda x: (x[3], x[0].lower()))
 
     if csv:
         writer = csv_writer(sys.stdout, lineterminator="\n")
         writer.writerow([c.header for c in table.columns])
         writer.writerows(rows)
     else:
         for row in rows:
-            row[-1] = "true" if row[-1] else "[red]false[/red]"
             table.add_row(*row)
         console = Console()
         console.print(table)
-        console.print(
-            Panel(
-                "[yellow]Warning: You have importable code in your path"
-                " which won't be available on your cluster because we're"
-                " unable to build wheel.[/yellow]"
-            )
-        )
 
 
 @package_sync.command()
 @click.option("--csv", is_flag=True, default=False, help="Output as CSV")
 def debug(csv: bool):
     table = Table(title="Debug")
     table.add_column("Path", no_wrap=True, overflow="fold")
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/run.py` & `coiled-0.8.0/coiled/cli/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,28 +55,34 @@
 @click.option(
     "--gpu",
     default=False,
     is_flag=True,
     help="Have a GPU available.",
 )
 @click.option(
+    "--region",
+    default=None,
+    help="The cloud provider region in which to run the notebook.",
+)
+@click.option(
     "--file",
     "-f",
     default=[],
     multiple=True,
     help="Local files required to run command.",
 )
 @click.argument("command", nargs=-1)
 def run(
     name: str,
     account: Optional[str],
     software: Optional[str],
     container: Optional[str],
     vm_type: Sequence[str],
     gpu: bool,
+    region: Optional[str],
     file,
     command,
 ):
     """
     Run a command on the cloud.
 
     .. warning::
@@ -112,15 +118,16 @@
         software=software,
         container=container,
         scheduler_options={"idle_timeout": "24 hours"},
         scheduler_vm_types=list(vm_type) if vm_type else None,
         allow_ssh=True,
         environ=env,
         scheduler_gpu=gpu,
-        tags={"coiled-cluster-type": "run"},
+        region=region,
+        tags={"coiled-cluster-type": "run/cli"},
     ) as cluster:
         with Client(cluster) as client:
             # Extract and upload files from `command`
             command = shlex.split(" ".join(command))
             for idx, i in enumerate(command):
                 if os.path.exists(i) and os.path.isfile(i):
                     client.upload_file(i, load=False)
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/utils.py` & `coiled-0.8.0/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.8.0/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.8.0/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/logs.py` & `coiled-0.8.0/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/metrics.py` & `coiled-0.8.0/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.8.0/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/cluster/utils.py` & `coiled-0.8.0/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.8.0/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.8.0/coiled/cli/notebook/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,14 +229,15 @@
             cloud=cloud,
             n_workers=0,
             software=software,
             container=container,
             jupyter=True,
             scheduler_options={"idle_timeout": "24 hours"},
             scheduler_vm_types=list(vm_type) if vm_type else None,
+            worker_vm_types=list(vm_type) if vm_type else None,
             allow_ssh=True,
             environ=env,
             scheduler_gpu=gpu,
             region=region,
             tags={"coiled-cluster-type": "notebook"},
         )
 
@@ -324,30 +325,40 @@
         webbrowser.open(url, new=2)
 
     if block:
         print("[green]Use Control-C to stop this notebook server [/]")
         with Progress(SpinnerColumn()) as progress:
             # Wait for shutdown signal from user
 
-            def signal_handler(signal, frame):
+            def signal_handler_noop(_, frame):
+                # Ignore the input signal
+                return
+
+            def signal_handler(_, frame):
                 progress.stop()
-                if interrupt_nested.is_set():
-                    return
+                # Restore original handler so KeyboardInterrupt show up as exceptions
+                signal.signal(signal.SIGINT, original_handler)
+                try:
+                    exit = Confirm.ask("Are you sure you want to stop this notebook server?", default=True)
+                except KeyboardInterrupt:
+                    # Register noop handler since we're shutting down and
+                    # want to make sure the notebook is shutdown even when
+                    # hammering ctrl-C
+                    signal.signal(signal.SIGINT, signal_handler_noop)
+                    exit = True
+                if exit:
+                    interrupt.set()
                 else:
-                    interrupt_nested.set()
-                    if Confirm.ask("Are you sure you want to stop this notebook server?", default=True):
-                        interrupt.set()
-                    else:
-                        print("[green]Continuing with this notebook server... [/]")
-                        progress.start()
-                        interrupt_nested.clear()
+                    signal.signal(signal.SIGINT, signal_handler)
+                    print("[green]Continuing with this notebook server... [/]")
+                    progress.start()
 
+            original_handler = signal.getsignal(signal.SIGINT)
             signal.signal(signal.SIGINT, signal_handler)
             interrupt = threading.Event()
-            interrupt_nested = threading.Event()
             progress.add_task("spinning...", total=None)  # starts an infinite spinner
             interrupt.wait()
 
         # `.callback` gets the underlying function from the click command.
         # It can sometimes be `None`. Not sure why, but we handle that case here
         # to make type checking happy.
         stop_func = stop_notebook.callback
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/__init__.py` & `coiled-0.8.0/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/amp.py` & `coiled-0.8.0/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/aws.py` & `coiled-0.8.0/coiled/cli/setup/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import traceback
 from typing import Optional, Tuple, Union
 
 import boto3
 import botocore
 import click
-import dask
+import dask.config
 import jsondiff
 from rich import print
 from rich.panel import Panel
 from rich.prompt import Confirm, IntPrompt
 
 import coiled
 
@@ -74,39 +74,58 @@
 @click.option(
     "-y",
     "--yes",
     default=False,
     is_flag=True,
     help="Don't prompt for confirmation, just do it!",
 )
+@click.option(
+    "--accept-delete",
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="use with --yes if you also want to accept deletes",
+)
+@click.option(
+    "--use-new",
+    default=False,
+    is_flag=True,
+    hidden=True,
+    help="Use new setup backend",
+)
 def aws_setup(
     iam_user: str,
     setup_policy: Optional[str],
     ongoing_policy: Optional[str],
     profile: Optional[str],
     update_policies: bool,
     update_instance_policy: bool,
     cloudshell_link: Optional[bool],
     region: Optional[str],
     manual_final_setup: bool,
     quotas: bool,
     yes: bool,
+    accept_delete: bool,
+    use_shim: bool,
 ):
+    accept_delete = yes and accept_delete  # (only accept_delete if --yes is also specified)
     if not do_setup(
         aws_profile=profile,
         slug=iam_user,
         setup_name=setup_policy,
         ongoing_name=ongoing_policy,
         just_update_policies=update_policies,
         just_update_instance_policy=update_instance_policy,
         cloudshell_link=cloudshell_link,
         region=region,
         manual_final_setup=manual_final_setup,
         quotas=quotas,
         yes=yes,
+        accept_delete=accept_delete,
+        use_shim=use_shim,
     ):
         pass
         # print("[red]The setup process didn't finish.[/red]")
 
 
 DEFAULT_REGION = "us-east-1"
 
@@ -360,15 +379,15 @@
 
 def attach_policy(iam, user, policy_arn):
     # idempotent
     iam.attach_user_policy(UserName=user, PolicyArn=policy_arn)
     coiled.add_interaction(action="AttachUserPolicy", success=True, arn=policy_arn)
 
 
-def make_access_key(iam, user, retry=0) -> Tuple[Optional[str], Optional[str]]:
+def make_access_key(iam, user, *, retry=0, accept_delete: bool = False) -> Tuple[Optional[str], Optional[str]]:
     try:
         r = iam.create_access_key(UserName=user)
         coiled.add_interaction(action="CreateAccessKey", success=True, user=user)
 
         key_id = r["AccessKey"]["AccessKeyId"]
         key_secret = r["AccessKey"]["SecretAccessKey"]
 
@@ -383,16 +402,16 @@
         )
         if retry:
             print("[red]already retried, giving up[/red]")
             return None, None
 
         # FIXME let user select which key to delete
         # if Confirm.ask(PROMPTS["replace_access_key"].format(user_name=user, key_id=key_id), default=True):
-        if delete_access_key(iam, user):
-            return make_access_key(iam, user, retry + 1)
+        if delete_access_key(iam, user, accept_delete=accept_delete):
+            return make_access_key(iam, user, retry=retry + 1, accept_delete=accept_delete)
 
     return None, None
 
 
 def get_user_access_keys(iam, user):
     try:
         r = iam.list_access_keys(UserName=user)
@@ -409,20 +428,20 @@
                 error_message=str(e),
             )
             return False, []
         else:
             raise
 
 
-def delete_access_key(iam, user):
+def delete_access_key(iam, user, accept_delete: bool = False):
     r = iam.list_access_keys(UserName=user)
     key_id = r["AccessKeyMetadata"][0]["AccessKeyId"]
 
     # NOTE: --yes doesn't apply to this since currently
-    if Confirm.ask(
+    if accept_delete or Confirm.ask(
         PROMPTS["replace_access_key"].format(user_name=user, key_id=key_id),
         default=True,
     ):
         coiled.add_interaction(action="prompt:DeleteAccessKey", success=True, user=user)
         iam.delete_access_key(UserName=user, AccessKeyId=key_id)
         coiled.add_interaction(action="DeleteAccessKey", success=True, user=user, key_id=key_id)
         print(f"    Deleted access key [green]{key_id}[/green]")
@@ -568,15 +587,15 @@
         f"  [green]{cli_command}[/green]\n"
     )
 
     # box might be nice but would make copying the command much worse
     print(instruction_text)
 
 
-def do_coiled_setup(iam, key, secret, region, yes) -> bool:
+def do_coiled_setup(iam, key, secret, region, yes, use_shim) -> bool:
     success = False
 
     if key and secret:
         print("[bold]You can setup Coiled to use the AWS credentials you just created.")
         print(
             "This AWS access key will go to Coiled, where it will be stored securely and "
             "used to create clusters in your AWS account on your behalf."
@@ -595,14 +614,15 @@
             if wait_till_key_works(iam, key, secret):
                 print("Setting up Coiled to use your AWS account...")
                 coiled.set_backend_options(
                     backend="aws",
                     aws_access_key_id=key,
                     aws_secret_access_key=secret,
                     aws_region=region,
+                    use_shim=use_shim,
                 )
                 success = True
                 coiled.add_interaction(action="CoiledSetup", success=True)
             else:
                 coiled.add_interaction(action="CoiledSetup", success=False)
                 print("[red]Access key is still not ready. You need to complete Coiled setup manually.")
                 print()
@@ -612,23 +632,15 @@
         if not success:
             show_manual_setup(key, secret)
 
     return success
 
 
 def do_full_setup(
-    session,
-    iam,
-    user_name,
-    account,
-    region,
-    setup_name,
-    ongoing_name,
-    manual_final_setup,
-    yes,
+    session, iam, user_name, account, region, setup_name, ongoing_name, manual_final_setup, yes, accept_delete, use_shim
 ) -> bool:
     # Check for existing user
     user_exists, user_keys = get_user_access_keys(iam, user_name)
 
     # Check for existing policies
     setup_arn, setup_diff = get_policy_diff(iam, account, setup_name, setup_doc)
     ongoing_arn, ongoing_diff = get_policy_diff(iam, account, ongoing_name, ongoing_doc)
@@ -727,20 +739,20 @@
         for arn in create_arns:
             print(f"  {arn}")
     print(f"IAM User [green]{user_name}[/green] is now setup with IAM Policies attached.")
     print()
 
     check_quotas(session, region=region)
 
-    key, secret = make_access_key(iam, user_name)
+    key, secret = make_access_key(iam, user_name, accept_delete=accept_delete)
 
     if manual_final_setup:
         return show_manual_setup(key, secret)
     else:
-        return do_coiled_setup(iam, key, secret, region, yes)
+        return do_coiled_setup(iam, key, secret, region, yes, use_shim)
 
 
 def show_manual_setup(key, secret):
     with coiled.Cloud() as cloud:
         coiled_account = cloud.default_account
 
     setup_url = (
@@ -858,14 +870,16 @@
     just_update_policies=False,
     just_update_instance_policy=False,
     region=None,
     cloudshell_link=None,
     manual_final_setup=None,
     quotas=None,
     yes=False,
+    accept_delete=False,
+    use_shim=False,
 ) -> bool:
     try:
         import getpass
         import socket
 
         local_user = f"{getpass.getuser()}@{socket.gethostname()}"
     except Exception:
@@ -884,14 +898,15 @@
         ongoing_policy=ongoing_name,
         update_policies=just_update_policies,
         update_instance_policy=just_update_instance_policy,
         region=region,
         cloudshell_link=cloudshell_link,
         manual_final_setup=manual_final_setup,
         yes=yes,
+        accept_delete=accept_delete,
     )
 
     if cloudshell_link:
         show_cloudshell_instructions(region)
         return False
 
     try:
@@ -939,14 +954,16 @@
                     user_name,
                     account,
                     region,
                     setup_name,
                     ongoing_name,
                     manual_final_setup=manual_final_setup,
                     yes=yes,
+                    accept_delete=accept_delete,
+                    use_shim=use_shim,
                 )
 
         except iam.exceptions.ClientError as e:
             error_code = e.response["Error"].get("Code")
             error_msg = e.response["Error"].get("Message")
             error_op = e.operation_name
 
@@ -974,15 +991,15 @@
                 print("To run this setup script you'll need the following IAM permissions:")
                 for permission in SCRIPT_REQUIRED_IAM:
                     print(f"- {permission}")
                 print(
                     "If you don't have access to an AWS profile with these permissions, you may need to ask "
                     "someone with administrative access to your AWS account to help you create the IAM User "
                     "and IAM Policies described in our documentation: "
-                    "[link]https://docs.coiled.io/user_guide/aws_configure.html[/link]"
+                    "[link]https://docs.coiled.io/user_guide/aws/manual.html[/link]"
                 )
                 setup_failure(
                     f"Permission error during for {error_op}. {error_msg}",
                     backend="aws",
                 )
                 return False
             else:
@@ -1096,14 +1113,26 @@
         },
         {
             "class": "G4dn (NVIDIA T4 GPU) Spot",
             "name": "All G and VT Spot Instance Requests",
             "code": "L-3819A6DF",
             "low": -1,
         },
+        {
+            "class": "P (NVIDIA V100/A100 GPU) On-Demand",
+            "name": "Running On-Demand P instances",
+            "code": "L-417A185B",
+            "low": -1,
+        },
+        {
+            "class": "P (NVIDIA V100/A100 GPU) Spot",
+            "name": "All P Spot Instance Requests",
+            "code": "L-7212CCBC",
+            "low": -1,
+        },
     ]
 
     quota_lines = []
 
     for quota in quotas:
         quota["link"] = get_quota_link(region, quota["code"])
 
@@ -1127,15 +1156,15 @@
             "An unexpected error occurred while trying to read your AWS service quotas:\n\n"
             f"[red]{e}[/red]\n\n"
             "You can check the quotas in the AWS Console using the links below."
         )
 
     for quota in quotas:
         quota_label = quota["class"]
-        if quota.get("value"):
+        if quota.get("value") is not None:
             quota_value_text = f"{quota.get('value'):>6} vCPU"
             if quota.get("is_low"):
                 quota_value_text = f"{quota_value_text} (this quota is low, you may wish to request increase)"
         else:
             quota_value_text = f"[link]{quota['link']}[/link]"
 
         quota_lines.append(f"{quota_label:<36}{quota_value_text}")
@@ -1163,21 +1192,24 @@
     if error_message:
         quota_text = f"{error_message}\n\n{quota_text}"
 
     print(Panel(quota_text))
 
     if got_quotas:
         if request_quotas:
+            # when running explicit quota check (`--quotas`), prompt about each quota
             do_quota_increases(quota_client, region, quotas)
         elif low_quotas:
             print(
                 "Some of your quotas are low. If you'd like to request any increases for these quotas, "
                 "we can prompt you for the desired quota value and attempt to submit this request to AWS.\n"
             )
             if Confirm.ask(PROMPTS["request_quotas"], default=True):
+                # when running normal setup flow, just prompt about low quotas
+                # note that we never consider GPU quotas low ("low" threshold is set to -1)
                 do_quota_increases(quota_client, region, low_quotas)
 
 
 def get_quota_value(quota_client, quota_code: str) -> int:
     quota = quota_client.get_service_quota(
         ServiceCode="ec2",
         QuotaCode=quota_code,
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/entry.py` & `coiled-0.8.0/coiled/cli/setup/entry.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             setup_failure(f"Exception raised {traceback.format_exc()}", backend="gcp")
             raise
     elif choice == "3":  # Other
         print(
             "\nCoiled currently supports Amazon Web Service and Google Cloud."
             "It's easy to make an account with either and get "
             "started using Coiled. Please see our documentation about choosing a cloud provider:\n"
-            "[link]https://docs.coiled.io/user_guide/backends.html#need-a-cloud-provider-account[/link]\n\n"
+            "[link]https://docs.coiled.io/user_guide/setup/no-cloud-provider.html[/link]\n\n"
             "If you're not ready to create your own cloud provider account, "
             "but would still like to try Coiled, we can set you up with a trial on our account. "
             "Reach out to us at "
             "[link=mailto:hello@coiled.io?subject=Trial%20Account]hello@coiled.io[/link] "
             "with a brief note about how you're using Dask."
         )
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/gcp.py` & `coiled-0.8.0/coiled/cli/setup/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 import tempfile
 import time
 from typing import Optional
 
 import click
-import dask
+import dask.config
 from rich import print
 from rich.panel import Panel
 from rich.prompt import Confirm
 from rich.table import Table
 
 import coiled
 
@@ -413,15 +413,15 @@
             print(f"Exported Coiled 'data access' role definition to {export_path}")
 
         return
 
     if not has_gcloud():
         print(
             "[red]The required `gcloud` CLI was not found. "
-            "See [link]https://docs.coiled.io/user_guide/gcp-cli.html[/link] for instructions."
+            "See [link]https://docs.coiled.io/user_guide/setup/gcp/cli.html[/link] for instructions."
         )
         setup_failure("Gcloud cli missing", backend="gcp")
         return False
 
     project = get_gcloud_config("project")
 
     if not project:
```

### Comparing `coiled-0.7.9.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.8.0/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/LICENSE` & `coiled-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/README.md` & `coiled-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/pyproject.toml` & `coiled-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.9.dev9/PKG-INFO` & `coiled-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.7.9.dev9
+Version: 0.8.0
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.7.9.dev9 Project-URL: Homepage,
-https://coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.8.0 Project-URL: Homepage, https:
+//coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
 rich>=11.2.0 Requires-Dist: setuptools>=49.3.0 Requires-Dist: typing-extensions
```

