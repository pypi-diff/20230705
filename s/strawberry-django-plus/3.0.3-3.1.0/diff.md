# Comparing `tmp/strawberry_django_plus-3.0.3.tar.gz` & `tmp/strawberry_django_plus-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-3.0.3.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.1.0.tar", max compression
```

## Comparing `strawberry_django_plus-3.0.3.tar` & `strawberry_django_plus-3.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-06-25 13:00:34.004619 strawberry_django_plus-3.0.3/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-25 13:00:34.004619 strawberry_django_plus-3.0.3/README.md
--rw-r--r--   0        0        0     4208 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3088 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5649 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5800 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    30229 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3033 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1556 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     2060 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0      896 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    24115 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14791 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26973 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1340 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    28094 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0     2532 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1027 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2423 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    17118 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/type.py
--rw-r--r--   0        0        0     9889 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13343 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     6604 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    16377 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0     1027 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-05 14:49:08.966455 strawberry_django_plus-3.1.0/LICENSE
+-rw-r--r--   0        0        0     3928 2023-07-05 14:49:08.966455 strawberry_django_plus-3.1.0/README.md
+-rw-r--r--   0        0        0     4208 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3088 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5800 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    30445 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     2060 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1920 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    24115 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-07-05 14:49:08.970455 strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26973 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28094 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2423 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    17118 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13343 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     6604 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16377 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      951 2023-07-05 14:49:08.974455 strawberry_django_plus-3.1.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 strawberry_django_plus-3.1.0/PKG-INFO
```

### Comparing `strawberry_django_plus-3.0.3/LICENSE` & `strawberry_django_plus-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/README.md` & `strawberry_django_plus-3.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 [![build status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fblb-ventures%2Fstrawberry-django-plus%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/blb-ventures/strawberry-django-plus/goto?ref=main)
 [![coverage](https://img.shields.io/codecov/c/github/blb-ventures/strawberry-django-plus.svg)](https://codecov.io/gh/blb-ventures/strawberry-django-plus)
 [![downloads](https://pepy.tech/badge/strawberry-django-plus)](https://pepy.tech/project/strawberry-django-plus)
 [![PyPI version](https://img.shields.io/pypi/v/strawberry-django-plus.svg)](https://pypi.org/project/strawberry-django-plus/)
 ![python version](https://img.shields.io/pypi/pyversions/strawberry-django-plus.svg)
 ![django version](https://img.shields.io/pypi/djversions/strawberry-django-plus.svg)
 
+> **Warning**
+>
+> All the extra features provided by this lib were contributed and merged directly
+> into the official
+> [strawberry-graphql-django](https://github.com/strawberry-graphql/strawberry-graphql-django)
+> lib. Since then this lib is deprecated and the official integration should be used instead
+> and development will continue there!
+>
+> If you were using this lib before, check out the
+> [migration guide](https://blb-ventures.github.io/strawberry-django-plus/migration-guide#migrating-to-strawberry-django)
+> for more information on how to migrate your code.
+
 Enhanced Strawberry integration with Django.
 
 Built on top of [strawberry-django](https://github.com/strawberry-graphql/strawberry-graphql-django)
 integration, enhancing its overall functionality.
 
 Check the [docs](https://blb-ventures.github.io/strawberry-django-plus/)
 for information on how to use this lib.
```

### Comparing `strawberry_django_plus-3.0.3/pyproject.toml` & `strawberry_django_plus-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "3.0.3"
+version = "3.1.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "3.0.3"  # x-release-please-version
+__version__ = "3.1.0"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/field.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,14 +615,15 @@
 
     return f
 
 
 def node(
     *,
     name: Optional[str] = None,
+    field_name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
@@ -658,14 +659,15 @@
         }
         ```
 
     """
     extensions = [*list(extensions), relay.NodeExtension()]
     return StrawberryDjangoField(
         python_name=None,
+        django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
@@ -681,14 +683,15 @@
 
 
 @overload
 def connection(
     graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
     name: Optional[str] = None,
+    field_name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
@@ -706,14 +709,15 @@
 
 @overload
 def connection(
     graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
     resolver: Optional[_RESOLVER_TYPE[NodeIterableType[Any]]] = None,
     name: Optional[str] = None,
+    field_name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     init: Literal[True] = True,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
@@ -731,14 +735,15 @@
 
 
 def connection(
     graphql_type: Optional[Type[relay.Connection[relay.NodeType]]] = None,
     *,
     resolver: Optional[_RESOLVER_TYPE[NodeIterableType[Any]]] = None,
     name: Optional[str] = None,
+    field_name: Optional[str] = None,
     is_subscription: bool = False,
     description: Optional[str] = None,
     permission_classes: Optional[List[Type[BasePermission]]] = None,
     deprecation_reason: Optional[str] = None,
     default: Any = dataclasses.MISSING,
     default_factory: Union[Callable[..., object], object] = dataclasses.MISSING,
     metadata: Optional[Mapping[Any, Any]] = None,
@@ -804,14 +809,15 @@
     .. _Relay connections:
         https://relay.dev/graphql/connections.htm
 
     """
     extensions = [*list(extensions), StrawberryDjangoConnectionExtension()]
     f = StrawberryDjangoField(
         python_name=None,
+        django_name=field_name,
         graphql_name=name,
         type_annotation=StrawberryAnnotation.from_annotation(graphql_type),
         description=description,
         is_subscription=is_subscription,
         permission_classes=permission_classes or [],
         deprecation_reason=deprecation_reason,
         default=default,
```

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/relay.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/type.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/types.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.1.0/strawberry_django_plus/utils/typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,12 +16,11 @@
 TypeOrSequence: TypeAlias = Union[_T, Sequence[_T]]
 TypeOrIterable: TypeAlias = Union[_T, Iterable[_T]]
 UserType: TypeAlias = Union[AbstractBaseUser, "AnonymousUser"]
 ResolverInfo: TypeAlias = Union[Info[StrawberryDjangoContext, Any], GraphQLResolveInfo]
 
 
 def is_auto(type_: Any) -> bool:
-    try:
-        return isinstance(type_, StrawberryAuto)
-    except NameError:
-        # This is to support "from __future__ import annotations" cases
-        return type_ == "strawberry.auto" or type_ == "gql.auto"
+    if isinstance(type_, str):
+        return type_ in ["strawberry.auto", "gql.auto", "auto"]
+
+    return isinstance(type_, StrawberryAuto)
```

### Comparing `strawberry_django_plus-3.0.3/PKG-INFO` & `strawberry_django_plus-3.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 3.0.3
+Version: 3.1.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -39,14 +39,26 @@
 [![build status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fblb-ventures%2Fstrawberry-django-plus%2Fbadge%3Fref%3Dmain&style=flat)](https://actions-badge.atrox.dev/blb-ventures/strawberry-django-plus/goto?ref=main)
 [![coverage](https://img.shields.io/codecov/c/github/blb-ventures/strawberry-django-plus.svg)](https://codecov.io/gh/blb-ventures/strawberry-django-plus)
 [![downloads](https://pepy.tech/badge/strawberry-django-plus)](https://pepy.tech/project/strawberry-django-plus)
 [![PyPI version](https://img.shields.io/pypi/v/strawberry-django-plus.svg)](https://pypi.org/project/strawberry-django-plus/)
 ![python version](https://img.shields.io/pypi/pyversions/strawberry-django-plus.svg)
 ![django version](https://img.shields.io/pypi/djversions/strawberry-django-plus.svg)
 
+> **Warning**
+>
+> All the extra features provided by this lib were contributed and merged directly
+> into the official
+> [strawberry-graphql-django](https://github.com/strawberry-graphql/strawberry-graphql-django)
+> lib. Since then this lib is deprecated and the official integration should be used instead
+> and development will continue there!
+>
+> If you were using this lib before, check out the
+> [migration guide](https://blb-ventures.github.io/strawberry-django-plus/migration-guide#migrating-to-strawberry-django)
+> for more information on how to migrate your code.
+
 Enhanced Strawberry integration with Django.
 
 Built on top of [strawberry-django](https://github.com/strawberry-graphql/strawberry-graphql-django)
 integration, enhancing its overall functionality.
 
 Check the [docs](https://blb-ventures.github.io/strawberry-django-plus/)
 for information on how to use this lib.
```

