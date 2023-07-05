# Comparing `tmp/virtool_workflow-5.3.0.tar.gz` & `tmp/virtool_workflow-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_workflow-5.3.0.tar", max compression
+gzip compressed data, was "virtool_workflow-5.3.1.tar", max compression
```

## Comparing `virtool_workflow-5.3.0.tar` & `virtool_workflow-5.3.1.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0     1097 2023-02-09 05:13:13.342688 virtool_workflow-5.3.0/LICENSE
--rw-r--r--   0        0        0     3874 2023-02-09 05:13:13.342688 virtool_workflow-5.3.0/README.md
--rw-r--r--   0        0        0     1135 2023-02-09 05:13:33.582965 virtool_workflow-5.3.0/pyproject.toml
--rw-r--r--   0        0        0      370 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/__init__.py
--rw-r--r--   0        0        0      126 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/__init__.py
--rw-r--r--   0        0        0      795 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/analysis.py
--rw-r--r--   0        0        0     7127 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/fastqc.py
--rw-r--r--   0        0        0      405 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/fixtures.py
--rw-r--r--   0        0        0     2148 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/hmms.py
--rw-r--r--   0        0        0     1079 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/indexes.py
--rw-r--r--   0        0        0     1355 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/reads.py
--rw-r--r--   0        0        0      717 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/sample.py
--rw-r--r--   0        0        0     4082 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/skewer.py
--rw-r--r--   0        0        0      549 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/subtractions.py
--rw-r--r--   0        0        0     1978 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/trimming.py
--rw-r--r--   0        0        0      992 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/analysis/utils.py
--rw-r--r--   0        0        0        0 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/__init__.py
--rw-r--r--   0        0        0     4789 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/analysis.py
--rw-r--r--   0        0        0     1528 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/client.py
--rw-r--r--   0        0        0     2476 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/errors.py
--rw-r--r--   0        0        0     2106 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/hmm.py
--rw-r--r--   0        0        0     3616 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/indexes.py
--rw-r--r--   0        0        0     4167 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/jobs.py
--rw-r--r--   0        0        0     3168 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/samples.py
--rw-r--r--   0        0        0     4016 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/subtractions.py
--rw-r--r--   0        0        0     1861 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/uploads.py
--rw-r--r--   0        0        0     3769 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/api/utils.py
--rw-r--r--   0        0        0     1510 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/builtin_fixtures.py
--rw-r--r--   0        0        0     1392 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/cli.py
--rw-r--r--   0        0        0        0 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/__init__.py
--rw-r--r--   0        0        0     1117 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/analysis.py
--rw-r--r--   0        0        0      376 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/files.py
--rw-r--r--   0        0        0     6565 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/indexes.py
--rw-r--r--   0        0        0      240 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/jobs.py
--rw-r--r--   0        0        0      864 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/samples.py
--rw-r--r--   0        0        0     1500 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/data_model/subtractions.py
--rw-r--r--   0        0        0     1697 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/decorators.py
--rw-r--r--   0        0        0      230 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/errors.py
--rw-r--r--   0        0        0     2647 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/hooks.py
--rw-r--r--   0        0        0        0 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/__init__.py
--rw-r--r--   0        0        0     2937 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/discovery.py
--rw-r--r--   0        0        0      138 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/events.py
--rw-r--r--   0        0        0     3561 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/executor.py
--rw-r--r--   0        0        0     4389 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/hook.py
--rw-r--r--   0        0        0     2504 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/providers.py
--rw-r--r--   0        0        0     1566 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/redis.py
--rw-r--r--   0        0        0     5618 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/run.py
--rw-r--r--   0        0        0     4636 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/run_subprocess.py
--rw-r--r--   0        0        0      714 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/sentry.py
--rw-r--r--   0        0        0      203 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/states.py
--rw-r--r--   0        0        0     2437 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/step.py
--rw-r--r--   0        0        0      432 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/runtime/utils.py
--rw-r--r--   0        0        0        0 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/testing/__init__.py
--rw-r--r--   0        0        0     1609 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/testing/fixtures.py
--rw-r--r--   0        0        0      752 2023-02-09 05:13:14.106694 virtool_workflow-5.3.0/virtool_workflow/workflow.py
--rw-r--r--   0        0        0     5115 1970-01-01 00:00:00.000000 virtool_workflow-5.3.0/setup.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 virtool_workflow-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-05 20:22:12.764709 virtool_workflow-5.3.1/LICENSE
+-rw-r--r--   0        0        0     3874 2023-07-05 20:22:12.764709 virtool_workflow-5.3.1/README.md
+-rw-r--r--   0        0        0     1094 2023-07-05 20:22:39.040563 virtool_workflow-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0      370 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/__init__.py
+-rw-r--r--   0        0        0      795 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/analysis.py
+-rw-r--r--   0        0        0     7127 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/fastqc.py
+-rw-r--r--   0        0        0      405 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/fixtures.py
+-rw-r--r--   0        0        0     2148 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/hmms.py
+-rw-r--r--   0        0        0     1079 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/indexes.py
+-rw-r--r--   0        0        0     1355 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/reads.py
+-rw-r--r--   0        0        0      717 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/sample.py
+-rw-r--r--   0        0        0     4082 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/skewer.py
+-rw-r--r--   0        0        0      549 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/subtractions.py
+-rw-r--r--   0        0        0     1978 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/trimming.py
+-rw-r--r--   0        0        0      992 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/analysis/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/__init__.py
+-rw-r--r--   0        0        0     4789 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/analysis.py
+-rw-r--r--   0        0        0     1528 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/client.py
+-rw-r--r--   0        0        0     2476 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/errors.py
+-rw-r--r--   0        0        0     2106 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/hmm.py
+-rw-r--r--   0        0        0     3616 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/indexes.py
+-rw-r--r--   0        0        0     4248 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/jobs.py
+-rw-r--r--   0        0        0     3168 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/samples.py
+-rw-r--r--   0        0        0     4016 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/subtractions.py
+-rw-r--r--   0        0        0     1861 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/uploads.py
+-rw-r--r--   0        0        0     3769 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/api/utils.py
+-rw-r--r--   0        0        0     1510 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/builtin_fixtures.py
+-rw-r--r--   0        0        0     1392 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/cli.py
+-rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/analysis.py
+-rw-r--r--   0        0        0      376 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/files.py
+-rw-r--r--   0        0        0     6565 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/indexes.py
+-rw-r--r--   0        0        0      240 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/jobs.py
+-rw-r--r--   0        0        0      864 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/samples.py
+-rw-r--r--   0        0        0     1500 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/data_model/subtractions.py
+-rw-r--r--   0        0        0     1697 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/decorators.py
+-rw-r--r--   0        0        0      230 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/errors.py
+-rw-r--r--   0        0        0     2647 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/discovery.py
+-rw-r--r--   0        0        0      138 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/events.py
+-rw-r--r--   0        0        0     3561 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/executor.py
+-rw-r--r--   0        0        0     4389 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/hook.py
+-rw-r--r--   0        0        0     2504 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/providers.py
+-rw-r--r--   0        0        0     1566 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/redis.py
+-rw-r--r--   0        0        0     5618 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/run.py
+-rw-r--r--   0        0        0     4636 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/run_subprocess.py
+-rw-r--r--   0        0        0      684 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/sentry.py
+-rw-r--r--   0        0        0      203 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/states.py
+-rw-r--r--   0        0        0     2437 2023-07-05 20:22:13.652705 virtool_workflow-5.3.1/virtool_workflow/runtime/step.py
+-rw-r--r--   0        0        0      432 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/runtime/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/testing/__init__.py
+-rw-r--r--   0        0        0     1609 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/testing/fixtures.py
+-rw-r--r--   0        0        0      752 2023-07-05 20:22:13.656705 virtool_workflow-5.3.1/virtool_workflow/workflow.py
+-rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 virtool_workflow-5.3.1/PKG-INFO
```

### Comparing `virtool_workflow-5.3.0/LICENSE` & `virtool_workflow-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/README.md` & `virtool_workflow-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/pyproject.toml` & `virtool_workflow-5.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtool-workflow"
-version = "5.3.0"
+version = "5.3.1"
 description = "A framework for developing bioinformatics workflows for Virtool."
 authors = ["Ian Boyes", "Blake Smith", "Ryan Fang"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/virtool/virtool-workflow"
 classifiers = [
     "Topic :: Software Development :: Libraries",
@@ -20,17 +20,14 @@
 aiohttp = "^3.8.1"
 aiofiles = "^0.7.0"
 virtool-core = "^3.0.0"
 aioredis = "1.3.1"
 sentry-sdk = "^1.5.7"
 pyfixtures = "^1.0.0"
 
-[tool.poetry.extras]
-test = ["virtool"]
-
 [tool.poetry.scripts]
 run-workflow = "virtool_workflow.cli:cli_main"
 
 [tool.poetry.group.dev.dependencies]
 syrupy = "^3.0.5"
 sphinx = "^4.0.2"
 pytest-regressions = "^2.4.1"
```

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/analysis.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/fastqc.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/fastqc.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/hmms.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/hmms.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/indexes.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/reads.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/reads.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/sample.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/sample.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/skewer.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/skewer.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/subtractions.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/trimming.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/trimming.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/analysis/utils.py` & `virtool_workflow-5.3.1/virtool_workflow/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/analysis.py` & `virtool_workflow-5.3.1/virtool_workflow/api/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/client.py` & `virtool_workflow-5.3.1/virtool_workflow/api/client.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/errors.py` & `virtool_workflow-5.3.1/virtool_workflow/api/errors.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/hmm.py` & `virtool_workflow-5.3.1/virtool_workflow/api/hmm.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/indexes.py` & `virtool_workflow-5.3.1/virtool_workflow/api/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/jobs.py` & `virtool_workflow-5.3.1/virtool_workflow/api/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,18 @@
     jobs_api_connection_string: str,
     step_name: str,
     step_description: str,
     stage: str,
     state: str,
     progress: float,
     error: Optional[Exception] = None,
-    max_tb: int = 50,
+    max_tb: int = 500,
 ):
+    if error:
+        logger.critical("Reporting error to API", exc_info=error)
 
     payload = {
         "state": state,
         "stage": stage,
         "step_name": step_name,
         "step_description": step_description,
         "error": {
```

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/samples.py` & `virtool_workflow-5.3.1/virtool_workflow/api/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/subtractions.py` & `virtool_workflow-5.3.1/virtool_workflow/api/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/uploads.py` & `virtool_workflow-5.3.1/virtool_workflow/api/uploads.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/api/utils.py` & `virtool_workflow-5.3.1/virtool_workflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/builtin_fixtures.py` & `virtool_workflow-5.3.1/virtool_workflow/builtin_fixtures.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/cli.py` & `virtool_workflow-5.3.1/virtool_workflow/cli.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/data_model/analysis.py` & `virtool_workflow-5.3.1/virtool_workflow/data_model/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/data_model/indexes.py` & `virtool_workflow-5.3.1/virtool_workflow/data_model/indexes.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/data_model/samples.py` & `virtool_workflow-5.3.1/virtool_workflow/data_model/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/data_model/subtractions.py` & `virtool_workflow-5.3.1/virtool_workflow/data_model/subtractions.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/decorators.py` & `virtool_workflow-5.3.1/virtool_workflow/decorators.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/hooks.py` & `virtool_workflow-5.3.1/virtool_workflow/hooks.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/discovery.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/discovery.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/executor.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/executor.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/hook.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/hook.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/providers.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/providers.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/redis.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/redis.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/run.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/run.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/run_subprocess.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/sentry.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/sentry.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import pkg_resources
 import sentry_sdk
 from sentry_sdk.integrations.logging import LoggingIntegration
 
 logger = getLogger("runtime")
 
 
-def configure_sentry(dsn: Optional[str], event_level: int = logging.ERROR):
+def configure_sentry(dsn: Optional[str]):
     """
     Initialize Sentry for log aggregation.
     """
     if dsn is None:
         return
 
     logger.info(f"Initializing Sentry dsn='{dsn[:15]}...'")
 
     sentry_sdk.init(
         dsn=dsn,
         integrations=[
             LoggingIntegration(
-                event_level=event_level,
+                event_level=logging.WARNING,
             )
         ],
         release=pkg_resources.get_distribution("virtool-workflow").version,
         traces_sample_rate=0.2,
     )
```

### Comparing `virtool_workflow-5.3.0/virtool_workflow/runtime/step.py` & `virtool_workflow-5.3.1/virtool_workflow/runtime/step.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/testing/fixtures.py` & `virtool_workflow-5.3.1/virtool_workflow/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/virtool_workflow/workflow.py` & `virtool_workflow-5.3.1/virtool_workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `virtool_workflow-5.3.0/setup.py` & `virtool_workflow-5.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,142 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: virtool-workflow
+Version: 5.3.1
+Summary: A framework for developing bioinformatics workflows for Virtool.
+Home-page: https://github.com/virtool/virtool-workflow
+License: MIT
+Author: Ian Boyes
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: aioredis (==1.3.1)
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: pyfixtures (>=1.0.0,<2.0.0)
+Requires-Dist: sentry-sdk (>=1.5.7,<2.0.0)
+Requires-Dist: virtool-core (>=3.0.0,<4.0.0)
+Project-URL: Repository, https://github.com/virtool/virtool-workflow
+Description-Content-Type: text/markdown
 
-packages = \
-['virtool_workflow',
- 'virtool_workflow.analysis',
- 'virtool_workflow.api',
- 'virtool_workflow.data_model',
- 'virtool_workflow.runtime',
- 'virtool_workflow.testing']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiofiles>=0.7.0,<0.8.0',
- 'aiohttp>=3.8.1,<4.0.0',
- 'aioredis==1.3.1',
- 'click>=8.0.0,<9.0.0',
- 'pyfixtures>=1.0.0,<2.0.0',
- 'sentry-sdk>=1.5.7,<2.0.0',
- 'virtool-core>=3.0.0,<4.0.0']
-
-entry_points = \
-{'console_scripts': ['run-workflow = virtool_workflow.cli:cli_main']}
-
-setup_kwargs = {
-    'name': 'virtool-workflow',
-    'version': '5.3.0',
-    'description': 'A framework for developing bioinformatics workflows for Virtool.',
-    'long_description': '# Virtool Workflow\n\n![Tests](https://github.com/virtool/virtool-workflow/workflows/Tests/badge.svg?branch=master)\n[![PyPI version](https://badge.fury.io/py/virtool-workflow.svg)](https://badge.fury.io/py/virtool-workflow)\n\nA framework for developing bioinformatic workflows in Python.\n\n```python\nfrom virtool_workflow import step\n\n\n@step\ndef step_function():\n    ...\n\n\n@step\ndef step_function_2():\n    ...\n```\n\n- [Documentation](https://workflow.virtool.ca)\n- [Website](https://www.virtool.ca/)\n\n## Contributing\n\n### Commits\n\nAll commits must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0) specification.\n\nThese standardized commit messages are used to automatically publish releases using [`semantic-release`](https://semantic-release.gitbook.io/semantic-release)\nafter commits are merged to `main` from successful PRs.\n\n**Example**\n\n```text\nfeat: add API support for assigning labels to existing samples\n```\n\nDescriptive bodies and footers are required where necessary to describe the impact of the commit. Use bullets where appropriate.\n\nAdditional Requirements\n\n1. **Write in the imperative**. For example, _"fix bug"_, not _"fixed bug"_ or _"fixes bug"_.\n2. **Don\'t refer to issues or code reviews**. For example, don\'t write something like this: _"make style changes requested in review"_.\n   Instead, _"update styles to improve accessibility"_.\n3. **Commits are not your personal journal**. For example, don\'t write something like this: _"got server running again"_\n   or _"oops. fixed my code smell"_.\n\nFrom Tim Pope: [A Note About Git Commit Messages](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)\n\n### Poetry\n\nDependencies & virtual environments are managed with [Poetry](https://python-poetry.org/ "Poetry")\n\nTo install `poetry`:\n\n```sh\nsudo pip install poetry\n```\n\nTo install dependencies, and the `virtool-workflow` package, into a virtual environment:\n\n```sh\ngit clone https://github.com/virtool/virtool-workflow\ncd virtool-workflow\n\npoetry install\n```\n\nTo run commands in the virtual environment:\n\n```sh\npoetry run <<command>>\n```\n\n### Tests\n\n[Pytest](https://docs.pytest.org/en/7.1.x/ "Pytest") is used to implement unit\nand integration tests.\n\nA pytest plugin,\n[pytest-docker-compose](https://github.com/pytest-docker-compose/pytest-docker-compose)\nhandles starting and stopping any required external services for integration\ntests. [docker-compose](https://docs.docker.com/compose/) will need to be\ninstalled on your system for this to work. It might also be necessary to setup a\n`docker` user group on your system, so you can [use docker without\nsudo](https://linoxide.com/use-docker-without-sudo-ubuntu/).\n\n`virtool-workflow` depends on some external bioinformatics tools such as [Bowtie\n2](http://bowtie-bio.sourceforge.net/bowtie2/index.shtml),\n[FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/), and\n[Skewer](https://github.com/relipmoc/skewer). Installation of these tools can be\nsomewhat involved, so it\'s best to run the test suite using `docker`. The\n[virtool/workflow-tools](https://github.com/virtool/workflow-tools) image\nprovides a base with all of the external dependencies pre-installed.\n\n[./tests/docker-compose.yml](./tests/docker-compose.yml) will run the test suite\ninside a container based on\n[virtool/workflow-tools](https://github.com/virtool/workflow-tools) and mount\nthe local docker socket so that `pytest`, running inside the container, can\nmanage the other services required by the integration tests.\n\nTo run the entire test suite:\n\n```sh\ncd tests\ndocker-compose up --exit-code-from pytest\n```\n\nTo run a subset of the tests, `tests/integration` only for example:\n\n```sh\ncd tests\nTEST_PATH=tests/integration docker-compose up --exit-code-from pytest\n```\n\n:warning: The `TEST_PATH` is a relative path from the repository root, not the `tests` directory.\n',
-    'author': 'Ian Boyes',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/virtool/virtool-workflow',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+# Virtool Workflow
 
+![Tests](https://github.com/virtool/virtool-workflow/workflows/Tests/badge.svg?branch=master)
+[![PyPI version](https://badge.fury.io/py/virtool-workflow.svg)](https://badge.fury.io/py/virtool-workflow)
+
+A framework for developing bioinformatic workflows in Python.
+
+```python
+from virtool_workflow import step
+
+
+@step
+def step_function():
+    ...
+
+
+@step
+def step_function_2():
+    ...
+```
+
+- [Documentation](https://workflow.virtool.ca)
+- [Website](https://www.virtool.ca/)
+
+## Contributing
+
+### Commits
+
+All commits must follow the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0) specification.
+
+These standardized commit messages are used to automatically publish releases using [`semantic-release`](https://semantic-release.gitbook.io/semantic-release)
+after commits are merged to `main` from successful PRs.
+
+**Example**
+
+```text
+feat: add API support for assigning labels to existing samples
+```
+
+Descriptive bodies and footers are required where necessary to describe the impact of the commit. Use bullets where appropriate.
+
+Additional Requirements
+
+1. **Write in the imperative**. For example, _"fix bug"_, not _"fixed bug"_ or _"fixes bug"_.
+2. **Don't refer to issues or code reviews**. For example, don't write something like this: _"make style changes requested in review"_.
+   Instead, _"update styles to improve accessibility"_.
+3. **Commits are not your personal journal**. For example, don't write something like this: _"got server running again"_
+   or _"oops. fixed my code smell"_.
+
+From Tim Pope: [A Note About Git Commit Messages](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
+
+### Poetry
+
+Dependencies & virtual environments are managed with [Poetry](https://python-poetry.org/ "Poetry")
+
+To install `poetry`:
+
+```sh
+sudo pip install poetry
+```
+
+To install dependencies, and the `virtool-workflow` package, into a virtual environment:
+
+```sh
+git clone https://github.com/virtool/virtool-workflow
+cd virtool-workflow
+
+poetry install
+```
+
+To run commands in the virtual environment:
+
+```sh
+poetry run <<command>>
+```
+
+### Tests
+
+[Pytest](https://docs.pytest.org/en/7.1.x/ "Pytest") is used to implement unit
+and integration tests.
+
+A pytest plugin,
+[pytest-docker-compose](https://github.com/pytest-docker-compose/pytest-docker-compose)
+handles starting and stopping any required external services for integration
+tests. [docker-compose](https://docs.docker.com/compose/) will need to be
+installed on your system for this to work. It might also be necessary to setup a
+`docker` user group on your system, so you can [use docker without
+sudo](https://linoxide.com/use-docker-without-sudo-ubuntu/).
+
+`virtool-workflow` depends on some external bioinformatics tools such as [Bowtie
+2](http://bowtie-bio.sourceforge.net/bowtie2/index.shtml),
+[FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/), and
+[Skewer](https://github.com/relipmoc/skewer). Installation of these tools can be
+somewhat involved, so it's best to run the test suite using `docker`. The
+[virtool/workflow-tools](https://github.com/virtool/workflow-tools) image
+provides a base with all of the external dependencies pre-installed.
+
+[./tests/docker-compose.yml](./tests/docker-compose.yml) will run the test suite
+inside a container based on
+[virtool/workflow-tools](https://github.com/virtool/workflow-tools) and mount
+the local docker socket so that `pytest`, running inside the container, can
+manage the other services required by the integration tests.
+
+To run the entire test suite:
+
+```sh
+cd tests
+docker-compose up --exit-code-from pytest
+```
+
+To run a subset of the tests, `tests/integration` only for example:
+
+```sh
+cd tests
+TEST_PATH=tests/integration docker-compose up --exit-code-from pytest
+```
+
+:warning: The `TEST_PATH` is a relative path from the repository root, not the `tests` directory.
 
-setup(**setup_kwargs)
```

