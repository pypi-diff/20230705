# Comparing `tmp/fal_serverless-0.6.36.tar.gz` & `tmp/fal_serverless-0.6.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.36.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.37.tar", max compression
```

## Comparing `fal_serverless-0.6.36.tar` & `fal_serverless-0.6.37.tar`

### file list

```diff
@@ -1,28 +1,65 @@
--rw-r--r--   0        0        0      213 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/README.md
--rw-r--r--   0        0        0     1012 2023-07-03 23:01:04.624228 fal_serverless-0.6.36/pyproject.toml
--rw-r--r--   0        0        0      405 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    23138 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2593 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5426 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15556 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0     5387 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/decorators.py
--rw-r--r--   0        0        0      158 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      578 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    17370 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     4231 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 fal_serverless-0.6.36/setup.py
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 fal_serverless-0.6.36/PKG-INFO
+-rw-r--r--   0        0        0      866 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/README.md
+-rw-r--r--   0        0        0      151 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/__init__.py
+-rw-r--r--   0        0        0     4833 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/check_dir_hash.py
+-rw-r--r--   0        0        0     4182 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/delete.py
+-rw-r--r--   0        0        0     4176 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/download.py
+-rw-r--r--   0        0        0     5184 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/file_exists.py
+-rw-r--r--   0        0        0     4558 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_directory.py
+-rw-r--r--   0        0        0     4247 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/list_root.py
+-rw-r--r--   0        0        0     4736 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_from_url.py
+-rw-r--r--   0        0        0     5735 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/files/upload_local_file.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/__init__.py
+-rw-r--r--   0        0        0     3974 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/create_key.py
+-rw-r--r--   0        0        0     4102 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/delete_key.py
+-rw-r--r--   0        0        0     4278 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/keys/list_keys.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/logs/__init__.py
+-rw-r--r--   0        0        0     4963 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/logs/list_since.py
+-rw-r--r--   0        0        0        0 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/__init__.py
+-rw-r--r--   0        0        0     6864 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage.py
+-rw-r--r--   0        0        0     4851 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/api/usage/per_machine_usage_details.py
+-rw-r--r--   0        0        0     2817 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/client.py
+-rw-r--r--   0        0        0      470 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/errors.py
+-rw-r--r--   0        0        0      784 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/__init__.py
+-rw-r--r--   0        0        0     1980 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/body_upload_local_file.py
+-rw-r--r--   0        0        0     2945 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/file_spec.py
+-rw-r--r--   0        0        0     1352 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/hash_check.py
+-rw-r--r--   0        0        0     2131 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/http_validation_error.py
+-rw-r--r--   0        0        0     1713 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/log_entry.py
+-rw-r--r--   0        0        0     1574 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/new_user_key.py
+-rw-r--r--   0        0        0     1357 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/url_file_upload.py
+-rw-r--r--   0        0        0     3558 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_per_machine_type.py
+-rw-r--r--   0        0        0     1918 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/usage_run_detail.py
+-rw-r--r--   0        0        0     1682 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/user_key_info.py
+-rw-r--r--   0        0        0     2091 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/models/validation_error.py
+-rw-r--r--   0        0        0       25 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/py.typed
+-rw-r--r--   0        0        0      993 2023-07-04 22:59:47.768241 fal_serverless-0.6.37/openapi-fal-rest/openapi_fal_rest/types.py
+-rw-r--r--   0        0        0     1353 2023-07-04 23:01:35.312903 fal_serverless-0.6.37/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    23138 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15747 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0     5342 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/decorators.py
+-rw-r--r--   0        0        0      158 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      684 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0     1209 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/rest_client.py
+-rw-r--r--   0        0        0    17370 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     4287 2023-07-04 22:59:47.772240 fal_serverless-0.6.37/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 fal_serverless-0.6.37/setup.py
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 fal_serverless-0.6.37/PKG-INFO
```

### Comparing `fal_serverless-0.6.36/pyproject.toml` & `fal_serverless-0.6.37/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.36"
+version = "0.6.37"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
+packages = [
+    { include = "fal_serverless", from = "src" },
+    { include = "openapi_fal_rest", from = "openapi-fal-rest" },
+]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
+isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
+isolate-proto = "0.0.33"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
-isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = ">=0.3.6,<0.3.7"
-isolate-proto = "0.0.32"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "2.12.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
 colorama = "^0.4.6"
 portalocker = "^2.7.0"
 rich = "^13.3.2"
-
-# For 3.10 and later, importlib-metadata's newer versions are included in the standard library.
-importlib-metadata = { version = ">=4.4", python = "<3.10" }
 packaging = ">=21.3"
 pathspec = "^0.11.1"
 
+# rest-api-client dependencies
+httpx = ">=0.15.4,<0.25.0"
+attrs = ">=21.3.0"
+python-dateutil = "^2.8.0"
+types-python-dateutil = "^2.8.0"
+
+# For 3.9 and earlier, importlib-metadata's newer versions are included in the standard library.
+importlib-metadata = { version = ">=4.4", python = "<3.10" }
+
+[tool.poetry.group.dev.dependencies]
+openapi-python-client = "^0.14.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fal-serverless = "fal_serverless.cli:cli"
```

### Comparing `fal_serverless-0.6.36/src/fal_serverless/api.py` & `fal_serverless-0.6.37/src/fal_serverless/api.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.37/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.37/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.37/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/cli.py` & `fal_serverless-0.6.37/src/fal_serverless/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,20 +337,25 @@
 @click.pass_obj
 def get_logs(
     host: api.FalServerlessHost, lines: int | None = 100, url: str | None = None
 ):
     if url:
         url = remove_http_and_port_from_url(url)
     logs = host._connection.get_logs(lines=lines, url=url)
-    if not logs:
-        console.print("No logs found")
-        return
     log_printer = IsolateLogPrinter(debug=True)
-    for log in logs:
-        log_printer.print(log)
+    first_log = next(logs, None)
+    if not first_log:
+        if url:
+            console.print("No logs found, make sure you have the correct URL")
+        else:
+            console.print("No logs found")
+    else:
+        log_printer.print(first_log)
+        for log in logs:
+            log_printer.print(log)
 
 
 ##### Alias group #####
 @click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
 @click.option("--port", default=DEFAULT_PORT, envvar=PORT_ENVVAR, hidden=True)
 @click.pass_context
```

### Comparing `fal_serverless-0.6.36/src/fal_serverless/decorators.py` & `fal_serverless-0.6.37/src/fal_serverless/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import sys
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, TypeVar
 
-import requests
-from fal_serverless.auth import USER
+import openapi_fal_rest.api.files.file_exists as file_exists_api
+import openapi_fal_rest.models.file_spec as file_spec_model
+from fal_serverless.rest_client import REST_CLIENT
 
 if sys.version_info >= (3, 11):
     from typing import Concatenate
 else:
     from typing_extensions import Concatenate
 
 if sys.version_info >= (3, 10):
@@ -22,54 +23,53 @@
 import fal_serverless.flags as flags
 from fal_serverless.api import FalServerlessError, InternalFalServerlessError, isolated
 
 ArgsT = ParamSpec("ArgsT")
 ReturnT = TypeVar("ReturnT")
 
 
-# TODO: this should be a client method from the client generated from the OpenAPI server
-def file_exists(file_path: Path | str, calculate_checksum: bool) -> FileSpec | None:
+def file_exists(
+    file_path: Path | str, calculate_checksum: bool
+) -> file_spec_model.FileSpec | None:
     file_str = str(file_path)
-    url = f"https://{flags.REST_HOST}/files/file/exists/{file_str}?calculate_checksum={calculate_checksum}"
-    response = requests.post(url, headers={"Authorization": USER.bearer_token})
+    response = file_exists_api.sync_detailed(
+        file_str,
+        client=REST_CLIENT,
+        calculate_checksum=calculate_checksum,
+    )
 
     if response.status_code == 200:
-        return FileSpec(**response.json())
+        return response.parsed  # type: ignore
     elif response.status_code == 404:
         return None
     else:
         raise InternalFalServerlessError(
-            f"Failed to check if file exists: {response.status_code} {response.text}"
+            f"Failed to check if file exists: {response.status_code} {response.parsed}"
         )
 
 
-# TODO: We will be able to do init=True when we get the client generated from the OpenAPI server
-@dataclass(init=False)
+@dataclass
 class FileSpec:
     path: Path
     size: int
     is_file: bool
     checksum_sha256: str | None = None
     checksum_md5: str | None = None
 
-    def __init__(
-        self,
-        path: str,
-        size: int,
-        is_file: bool,
-        checksum_sha256: str | None,
-        checksum_md5: str | None,
-        # ignore any other fields passed
-        **_others: Any,
-    ):
-        self.path = Path(path)
-        self.size = size
-        self.is_file = is_file
-        self.checksum_sha256 = checksum_sha256
-        self.checksum_md5 = checksum_md5
+    @classmethod
+    def from_model(cls, file_spec: file_spec_model.FileSpec) -> FileSpec:
+        return cls(
+            path=Path(file_spec.path),
+            size=file_spec.size,
+            is_file=file_spec.is_file,
+            checksum_sha256=file_spec.checksum_sha256
+            if file_spec.checksum_sha256
+            else None,
+            checksum_md5=file_spec.checksum_md5 if file_spec.checksum_md5 else None,
+        )
 
 
 def setup(
     file_path: Path | str,
     checksum_sha256: str | None = None,
     checksum_md5: str | None = None,
     force: bool = False,
@@ -115,15 +115,15 @@
 
                 if checksum_md5 and file.checksum_md5 != checksum_md5:
                     raise FalServerlessError(
                         f"Setup function {func.__name__} created file with unexpected MD5 checksum.\n"
                         f"Expected {checksum_md5} but got {file.checksum_md5}"
                     )
 
-            return file
+            return FileSpec.from_model(file)
 
         return internal_wrapper
 
     return wrapper
 
 
 def download_file(
```

### Comparing `fal_serverless-0.6.36/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.37/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.37/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/flags.py` & `fal_serverless-0.6.37/src/fal_serverless/flags.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 TEST_MODE = bool_envvar("ISOLATE_TEST_MODE")
 AUTH_DISABLED = bool_envvar("ISOLATE_AUTH_DISABLED")
 
 GRPC_HOST = os.getenv("FAL_HOST", "api.alpha.fal.ai:443")
 assert GRPC_HOST.startswith("api"), "FAL_HOST must start with 'api'"
 
 REST_HOST = GRPC_HOST.replace("api", "rest", 1)
+REST_SCHEME = "http" if TEST_MODE or AUTH_DISABLED else "https"
+REST_URL = f"{REST_SCHEME}://{REST_HOST}"
 
 FORCE_SETUP = bool_envvar("FAL_FORCE_SETUP")
```

### Comparing `fal_serverless-0.6.36/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.37/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.37/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.37/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.37/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.37/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/sdk.py` & `fal_serverless-0.6.37/src/fal_serverless/sdk.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.36/src/fal_serverless/sync.py` & `fal_serverless-0.6.37/src/fal_serverless/sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 from __future__ import annotations
 
 import hashlib
 import os
 import zipfile
+from pathlib import Path
 
-import requests
-from fal_serverless.api import FAL_SERVERLESS_DEFAULT_URL
-from fal_serverless.sdk import Credentials, get_default_credentials
+import openapi_fal_rest.api.files.check_dir_hash as check_dir_hash_api
+import openapi_fal_rest.api.files.upload_local_file as upload_local_file_api
+import openapi_fal_rest.models.body_upload_local_file as upload_file_model
+import openapi_fal_rest.models.hash_check as hash_check_model
+import openapi_fal_rest.types as rest_types
+from fal_serverless.rest_client import REST_CLIENT
 from pathspec import PathSpec
 
 
-def _check_hash(target_path: str, hash_string: str, creds: Credentials) -> bool:
-    url = f"{REST_URL}/files/dir/check_hash/{target_path}"
-    headers = creds.to_headers()
-    headers["Content-Type"] = "application/json"
-    result = requests.post(url=url, headers=headers, json={"hash": hash_string})
-    return result.status_code == 200 and result.json() is True
+def _check_hash(target_path: str, hash_string: str) -> bool:
+    response = check_dir_hash_api.sync_detailed(
+        target_path,
+        client=REST_CLIENT,
+        json_body=hash_check_model.HashCheck(hash_string),
+    )
 
+    res: bool = response.parsed  # type: ignore
+    return response.status_code == 200 and res
 
-def _upload_file(
-    source_path: str, target_path: str, creds: Credentials, unzip: bool = False
-) -> None:
 
-    url = f"{REST_URL}/files/file/local/{target_path}"
-    headers = creds.to_headers()
+def _upload_file(source_path: str, target_path: str, unzip: bool = False):
     with open(source_path, "rb") as file_to_upload:
-        files = {"file_upload": file_to_upload}
-        params = {"unzip": unzip}
-        response = requests.post(url, headers=headers, files=files, params=params)
+        body = upload_file_model.BodyUploadLocalFile(
+            rest_types.File(
+                payload=file_to_upload,
+                # We need to set a file_name, otherwise the server errors processing the file
+                file_name=os.path.basename(source_path),
+            )
+        )
 
-    if response.status_code == 200:
-        return response.json()
-    else:
+        response = upload_local_file_api.sync_detailed(
+            target_path,
+            client=REST_CLIENT,
+            unzip=unzip,
+            multipart_data=body,
+        )
+
+    if response.status_code != 200:
         raise Exception(
-            f"Failed to upload file. Server returned status code {response.status_code} and message {response.text}"
+            f"Failed to upload file. Server returned status code {response.status_code} and message {response.parsed}"
         )
 
 
 def _compute_directory_hash(dir_path: str) -> str:
     hash = hashlib.sha256()
     for root, _, files in os.walk(dir_path):
         for file in files:
@@ -74,52 +85,42 @@
                 relative_path = os.path.relpath(file_path, dir_path)
 
                 if not _is_ignored(relative_path, gitignore_patterns):
                     arcname = relative_path
                     zipf.write(file_path, arcname)
 
 
-def sync_dir(local_dir: str, remote_dir: str, force_upload=False) -> str:
+def sync_dir(local_dir: str | Path, remote_dir: str, force_upload=False) -> str:
     local_dir_abs = os.path.expanduser(local_dir)
     if not os.path.isabs(remote_dir) or not remote_dir.startswith("/data"):
         raise ValueError(
             "'remote_dir' must be an absolute path starting with `/data`, e.g. '/data/sync/my_dir'"
         )
 
     remote_dir = remote_dir.replace("/data/", "", 1)
 
     # Compute the local directory hash
     local_hash = _compute_directory_hash(local_dir_abs)
 
-    creds = get_default_credentials()
-
     print(f"Syncing {local_dir} with {remote_dir}...")
 
-    if _check_hash(remote_dir, local_hash, creds) and not force_upload:
+    if _check_hash(remote_dir, local_hash) and not force_upload:
         print(f"{remote_dir} already uploaded and matches {local_dir}")
         return remote_dir
 
     with open(os.path.join(local_dir_abs, ".fal_hash"), "w") as f:
         f.write(local_hash)
 
     # Zip the local directory
     zip_path = f"{local_dir_abs}.zip"
 
     _zip_directory(local_dir_abs, zip_path)
 
     # Upload the zipped directory to the serverless environment
-    _upload_file(zip_path, remote_dir, creds, unzip=True)
+    _upload_file(zip_path, remote_dir, unzip=True)
 
     os.remove(zip_path)
 
     print("Done")
 
     # Return the full path to the remote directory
     return remote_dir
-
-
-def _get_rest_host_url(url: str) -> str:
-    assert url.startswith("api."), "Expected FAL_HOST format to be `api.<env>.fal.ai`"
-    return "https://" + url.replace("api", "rest", 1)  # to replace just once
-
-
-REST_URL = _get_rest_host_url(FAL_SERVERLESS_DEFAULT_URL)
```

