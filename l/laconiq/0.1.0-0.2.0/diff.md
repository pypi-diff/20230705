# Comparing `tmp/laconiq-0.1.0.tar.gz` & `tmp/laconiq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laconiq-0.1.0.tar", max compression
+gzip compressed data, was "laconiq-0.2.0.tar", max compression
```

## Comparing `laconiq-0.1.0.tar` & `laconiq-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10226 2023-06-25 04:16:15.972388 laconiq-0.1.0/LICENSE
--rw-r--r--   0        0        0       54 2023-06-25 04:16:15.972388 laconiq-0.1.0/README.md
--rw-r--r--   0        0        0       44 2023-06-25 04:16:15.972388 laconiq-0.1.0/laconiq/__init__.py
--rw-r--r--   0        0        0     1240 2023-06-25 04:16:15.972388 laconiq-0.1.0/laconiq/generators.py
--rw-r--r--   0        0        0     2370 2023-06-25 04:16:15.972388 laconiq-0.1.0/laconiq/maker.py
--rw-r--r--   0        0        0      436 2023-06-25 04:16:15.972388 laconiq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 laconiq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-07-05 04:38:43.476547 laconiq-0.2.0/LICENSE
+-rw-r--r--   0        0        0       54 2023-07-05 04:38:43.476547 laconiq-0.2.0/README.md
+-rw-r--r--   0        0        0       44 2023-07-05 04:38:43.476547 laconiq-0.2.0/laconiq/__init__.py
+-rw-r--r--   0        0        0     1240 2023-07-05 04:38:43.476547 laconiq-0.2.0/laconiq/generators.py
+-rw-r--r--   0        0        0     2907 2023-07-05 04:38:43.476547 laconiq-0.2.0/laconiq/maker.py
+-rw-r--r--   0        0        0      436 2023-07-05 04:38:43.476547 laconiq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 laconiq-0.2.0/PKG-INFO
```

### Comparing `laconiq-0.1.0/LICENSE` & `laconiq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laconiq-0.1.0/laconiq/generators.py` & `laconiq-0.2.0/laconiq/generators.py`

 * *Files identical despite different names*

### Comparing `laconiq-0.1.0/laconiq/maker.py` & `laconiq-0.2.0/laconiq/maker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import types
+import typing
 from enum import Enum
 from random import choice
 
 from .generators import generate_for_type
 
 
 def make_one_enum(enum_klass):
@@ -29,22 +30,33 @@
 
     attrs = {}
 
     for prop, value in model_klass.schema()['properties'].items():
         if prop in desired_instance_attrs.keys():
             attrs[prop] = desired_instance_attrs.get(prop)
         else:
+            if 'type' in value and value['type'] == 'array':
+                # is it an array?
+                klass_or_instance = model_klass.__annotations__[prop]
+                origs = typing.get_args(klass_or_instance)
+                if len(origs) > 1:
+                    raise ValueError("Multiple subscriptions not yet supported")
+                attrs[prop] = make(origs[0], _quantity=3)
+                continue
+
             if 'type' in value:
+                # is it a simple type? like str, uuid, int, email
                 attrs[prop] = generate_for_type(
                     value.get('type'),
                     value.get('format', None)
                 )
                 continue
 
             if '$ref' in value.keys():
+                # is it a union?
                 klass_or_instance = model_klass.__annotations__[prop]
                 if isinstance(klass_or_instance, types.UnionType):
                     continue
 
                 # klass_or_instance is class here
                 if issubclass(klass_or_instance, Enum):
                     attrs[prop] = make(klass_or_instance)  # type: ignore
```

