# Comparing `tmp/coiled-0.8.0.tar.gz` & `tmp/coiled-0.8.1.dev1.tar.gz`

## Comparing `coiled-0.8.0.tar` & `coiled-0.8.1.dev1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/analytics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/exceptions.py
--rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/magic.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/run.py
--rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/types.py
--rw-r--r--   0        0        0    53908 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/authenticate.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/config.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92101 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.0/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.0/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.0/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.0/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 coiled-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0    25059 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/magic.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/run.py
+-rw-r--r--   0        0        0    19772 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/types.py
+-rw-r--r--   0        0        0    53908 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/authenticate.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45735 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.1.dev1/PKG-INFO
```

### Comparing `coiled-0.8.0/coiled/__init__.py` & `coiled-0.8.1.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/analytics.py` & `coiled-0.8.1.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cluster.py` & `coiled-0.8.1.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/coiled.yaml` & `coiled-0.8.1.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/context.py` & `coiled-0.8.1.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/core.py` & `coiled-0.8.1.dev1/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/exceptions.py` & `coiled-0.8.1.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/magic.py` & `coiled-0.8.1.dev1/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/run.py` & `coiled-0.8.1.dev1/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/scan.py` & `coiled-0.8.1.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/software.py` & `coiled-0.8.1.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/types.py` & `coiled-0.8.1.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/utils.py` & `coiled-0.8.1.dev1/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/websockets.py` & `coiled-0.8.1.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/authenticate.py` & `coiled-0.8.1.dev1/coiled/cli/authenticate.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/config.py` & `coiled-0.8.1.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/core.py` & `coiled-0.8.1.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/curl.py` & `coiled-0.8.1.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/env.py` & `coiled-0.8.1.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/login.py` & `coiled-0.8.1.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/package_sync.py` & `coiled-0.8.1.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/prefect.py` & `coiled-0.8.1.dev1/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/run.py` & `coiled-0.8.1.dev1/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/utils.py` & `coiled-0.8.1.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/__init__.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/better_logs.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/logs.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/metrics.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/ssh.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/cluster/utils.py` & `coiled-0.8.1.dev1/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/notebook/__init__.py` & `coiled-0.8.1.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/notebook/notebook.py` & `coiled-0.8.1.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/__init__.py` & `coiled-0.8.1.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/amp.py` & `coiled-0.8.1.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/aws.py` & `coiled-0.8.1.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/entry.py` & `coiled-0.8.1.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/gcp.py` & `coiled-0.8.1.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/cli/setup/prometheus.py` & `coiled-0.8.1.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/extensions/prefect/runners.py` & `coiled-0.8.1.dev1/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/extensions/prefect/workers.py` & `coiled-0.8.1.dev1/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/__init__.py` & `coiled-0.8.1.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/cluster.py` & `coiled-0.8.1.dev1/coiled/v2/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,16 @@
         exists create one.
     account
         Name of Coiled account to use. If not provided, will
         default to the user account for the ``cloud`` object being used.
     shutdown_on_close
         Whether or not to shut down the cluster when it finishes.
         Defaults to True, unless name points to an existing cluster.
+    idle_timeout
+        Shut down the cluster after this duration if no activity has occurred.
     use_scheduler_public_ip
         Boolean value that determines if the Python client connects to the
         Dask scheduler using the scheduler machine's public IP address. The
         default behaviour when set to True is to connect to the scheduler
         using its public IP address, which means traffic will be routed over
         the public internet. When set to False, traffic will be routed over
         the local network the scheduler lives in, so make sure the scheduler
@@ -321,14 +323,15 @@
         scheduler_cpu: Optional[Union[int, List[int]]] = None,
         scheduler_memory: Optional[Union[str, List[str]]] = None,
         scheduler_gpu: Optional[bool] = None,
         asynchronous: bool = False,
         cloud: Optional[CloudV2] = None,
         account: Optional[str] = None,
         shutdown_on_close=None,
+        idle_timeout: Optional[str] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         credentials: Optional[str] = "local",
         credentials_duration_seconds: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
         environ: Optional[Dict[str, str]] = None,
         tags: Optional[Dict[str, str]] = None,
@@ -583,14 +586,17 @@
             self.backend_options["ingress"] = cluster_firewall(**firewall_kwargs)[  # type: ignore
                 "ingress"
             ]  # type: ignore
 
         if jupyter:
             self.scheduler_options["jupyter"] = True
 
+        if idle_timeout:
+            self.scheduler_options["idle_timeout"] = idle_timeout
+
         if not self.asynchronous:
             # If we don't close the cluster, the user's ipython session gets spammed with
             # messages from distributed.
             #
             # Note that this doesn't solve all such spammy dead clusters (which is probably still
             # a problem), just spam created by clusters who failed initial creation.
             error = None
```

### Comparing `coiled-0.8.0/coiled/v2/core.py` & `coiled-0.8.1.dev1/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/cwi_log_link.py` & `coiled-0.8.1.dev1/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/states.py` & `coiled-0.8.1.dev1/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/widgets/__init__.py` & `coiled-0.8.1.dev1/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/widgets/rich.py` & `coiled-0.8.1.dev1/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/coiled/v2/widgets/util.py` & `coiled-0.8.1.dev1/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/LICENSE` & `coiled-0.8.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/README.md` & `coiled-0.8.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/pyproject.toml` & `coiled-0.8.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.0/PKG-INFO` & `coiled-0.8.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.0
+Version: 0.8.1.dev1
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
-Metadata-Version: 2.1 Name: coiled Version: 0.8.0 Project-URL: Homepage, https:
-//coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.8.1.dev1 Project-URL: Homepage,
+https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
 rich>=11.2.0 Requires-Dist: setuptools>=49.3.0 Requires-Dist: typing-extensions
```

