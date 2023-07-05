# Comparing `tmp/neosctl-0.8.7.tar.gz` & `tmp/neosctl-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.7.tar", max compression
+gzip compressed data, was "neosctl-0.8.8.tar", max compression
```

## Comparing `neosctl-0.8.7.tar` & `neosctl-0.8.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-07-04 09:13:12.726821 neosctl-0.8.7/README.md
--rw-r--r--   0        0        0       22 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3564 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     5684 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3243 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      122 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8649 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12390 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-07-04 09:13:12.729821 neosctl-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-07-05 11:53:12.771864 neosctl-0.8.8/README.md
+-rw-r--r--   0        0        0       22 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-05 11:53:12.771864 neosctl-0.8.8/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3564 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     5684 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-07-05 11:53:12.772864 neosctl-0.8.8/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3243 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      122 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     7686 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12904 2023-07-05 11:53:12.773864 neosctl-0.8.8/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-07-05 11:53:12.773864 neosctl-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.8/PKG-INFO
```

### Comparing `neosctl-0.8.7/README.md` & `neosctl-0.8.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.7
+# Core CLI v0.8.8
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.7/neosctl/auth.py` & `neosctl-0.8.8/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/cli.py` & `neosctl-0.8.8/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/profile.py` & `neosctl-0.8.8/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/schema.py` & `neosctl-0.8.8/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/__init__.py` & `neosctl-0.8.8/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/data_product.py` & `neosctl-0.8.8/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/data_source.py` & `neosctl-0.8.8/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/data_system.py` & `neosctl-0.8.8/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.8/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/entity.py` & `neosctl-0.8.8/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/link.py` & `neosctl-0.8.8/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/output.py` & `neosctl-0.8.8/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/schema.py` & `neosctl-0.8.8/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/secret.py` & `neosctl-0.8.8/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/spark.py` & `neosctl-0.8.8/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/gateway/tag.py` & `neosctl-0.8.8/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/iam/iam.py` & `neosctl-0.8.8/neosctl/services/iam/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/iam/schema.py` & `neosctl-0.8.8/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/registry/registry.py` & `neosctl-0.8.8/neosctl/services/registry/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.7/neosctl/services/storage/storage.py` & `neosctl-0.8.8/neosctl/services/storage/storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,38 @@
 
 app = typer.Typer()
 
 bucket_app = typer.Typer()
 object_app = typer.Typer()
 tagging_app = typer.Typer()
 
+BUCKET_NAME_PATTERN = "^[a-z0-9][a-z0-9\\.\\-]{2,62}$"
+OBJECT_NAME_PATTERN = "^[a-zA-Z0-9!\\ \\.\\-\\_*\\'\\(\\)]{1,255}$"
+
+BUCKET_NAME_ARGUMENT = typer.Argument(
+    ...,
+    help="Bucket name",
+    callback=util.validate_regex(BUCKET_NAME_PATTERN),
+)
+
+OBJECT_NAME_ARGUMENT = typer.Argument(
+    ...,
+    help="Object name",
+    callback=util.validate_regex(OBJECT_NAME_PATTERN),
+)
+
 app.add_typer(bucket_app, name="bucket", help="Manage object buckets.")
 app.add_typer(object_app, name="object", help="Manage objects.")
 object_app.add_typer(tagging_app, name="tags", help="Manage object tags.")
 
 
 @bucket_app.command(name="create")
 def create_bucket(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
 ) -> None:
     """Create new bucket."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
@@ -49,25 +60,21 @@
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
         secret_key="random-secret",
         secure=secure,
     )
 
-    print(client.list_buckets())  # noqa: T201
+    print([str(x) for x in client.list_buckets()])  # noqa: T201
 
 
 @bucket_app.command(name="delete")
 def delete_bucket(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
 ) -> None:
     """Delete bucket."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
         host,
@@ -77,24 +84,16 @@
     )
     print(client.remove_bucket(bucket_name))  # noqa: T201
 
 
 @object_app.command(name="create")
 def create_object(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
     file: str = typer.Argument(
         ...,
         help="Path to the object file.",
         callback=util.validate_string_not_empty,
     ),
 ) -> None:
     """Create object."""
@@ -114,19 +113,15 @@
     )
     print(f"Object {object_name} is added to the bucket {bucket_name}")  # noqa: T201
 
 
 @object_app.command(name="list")
 def list_objects(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
     prefix: typing.Union[str, None] = typer.Option(None, help="Path prefix"),
 ) -> None:
     """List objects."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
@@ -138,24 +133,16 @@
 
     print([obj._object_name for obj in client.list_objects(bucket_name, prefix=prefix)])  # noqa: SLF001, T201
 
 
 @object_app.command(name="get")
 def get_object(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
     file: str = typer.Argument(
         ...,
         help="Path to file where to store the object.",
         callback=util.validate_string_not_empty,
     ),
 ) -> None:
     """Get object."""
@@ -174,24 +161,16 @@
     with pathlib.Path(file).open("wb") as fh:
         fh.write(response.data)
 
 
 @object_app.command(name="delete")
 def delete_object(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
 ) -> None:
     """Delete object."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
         host,
@@ -203,24 +182,16 @@
     client.remove_object(bucket_name, object_name)
     print(f"Object {object_name} is deleted from the bucket {bucket_name}.")  # type: ignore[reportGeneralTypeIssues] # noqa: E501, T201
 
 
 @tagging_app.command(name="set")
 def set_object_tags(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
     tags: typing.List[str] = typer.Argument(
         ...,
         help="Tags as pairs of key=value",
         callback=util.validate_strings_are_not_empty,
     ),
 ) -> None:
     """Set object tags. Be aware that this command overwrites any tags that are already set to the object."""
@@ -240,24 +211,16 @@
         minio_tags[key] = value
     client.set_object_tags(bucket_name, object_name, minio_tags)
 
 
 @tagging_app.command(name="get")
 def get_object_tags(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
 ) -> None:
     """Get object tags."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
         host,
@@ -268,24 +231,16 @@
 
     print(client.get_object_tags(bucket_name, object_name))  # noqa: T201
 
 
 @tagging_app.command(name="delete")
 def delete_object_tags(
     ctx: typer.Context,
-    bucket_name: str = typer.Argument(
-        ...,
-        help="Bucket name",
-        callback=util.validate_string_not_empty,
-    ),
-    object_name: str = typer.Argument(
-        ...,
-        help="Object name",
-        callback=util.validate_string_not_empty,
-    ),
+    bucket_name: str = BUCKET_NAME_ARGUMENT,
+    object_name: str = OBJECT_NAME_ARGUMENT,
 ) -> None:
     """Delete object tags."""
     secure = ctx.obj.storage_api_url.startswith("https://")
     host = ctx.obj.storage_api_url.rstrip("/").replace("https://", "").replace("http://", "")
 
     client = minio.Minio(  # nosec: B106
         host,
```

### Comparing `neosctl-0.8.7/neosctl/util.py` & `neosctl-0.8.8/neosctl/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import configparser
 import json
 import pathlib
+import re
 import sys
 import typing
 
 import click
 import httpx
 import pydantic
 import typer
@@ -404,13 +405,34 @@
     param: click.Parameter,
     values: typing.List[str],
 ) -> typing.List[str]:
     """List of strings validation callback."""
     return [validate_string_not_empty(ctx, param, value) for value in values]
 
 
+def validate_regex(
+    pattern: str,
+) -> typing.Callable[[click.Context, click.Parameter, str], str]:
+    """Regex validation callback."""
+
+    def factory(
+        ctx: click.Context,
+        param: click.Parameter,
+        value: str,
+    ) -> str:
+        value = value.strip()
+
+        if not re.match(pattern, value):
+            message = f"Value does not satisfy the rule {pattern}"
+            raise typer.BadParameter(message, ctx=ctx, param=param)
+
+        return value
+
+    return factory
+
+
 def user_profile_callback(
     ctx: typer.Context,
 ) -> None:
     """Inject required user_profile into context."""
     user_profile = get_user_profile(ctx.obj.config, ctx.obj.profile_name)
     ctx.obj.profile = user_profile
```

### Comparing `neosctl-0.8.7/pyproject.toml` & `neosctl-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.7"
+version = "0.8.8"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.7/PKG-INFO` & `neosctl-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.7
+Version: 0.8.8
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.7
+# Core CLI v0.8.8
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

