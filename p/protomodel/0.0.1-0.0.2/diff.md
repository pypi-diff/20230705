# Comparing `tmp/protomodel-0.0.1.tar.gz` & `tmp/protomodel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protomodel-0.0.1.tar", max compression
+gzip compressed data, was "protomodel-0.0.2.tar", max compression
```

## Comparing `protomodel-0.0.1.tar` & `protomodel-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,22 @@
--rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.1/README.md
--rw-r--r--   0        0        0      108 2023-07-05 03:31:17.977392 protomodel-0.0.1/protomodel/__init__.py
--rw-r--r--   0        0        0       22 2023-07-05 03:07:25.797387 protomodel-0.0.1/protomodel/grpc.py
--rw-r--r--   0        0        0      950 2023-07-05 03:31:35.217392 protomodel-0.0.1/protomodel/message.py
--rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.1/protomodel/protomodel/__init__.py
--rw-r--r--   0        0        0       25 2023-07-05 03:07:52.257387 protomodel-0.0.1/protomodel/service.py
--rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.1/protomodel/types/__init__.py
--rw-r--r--   0        0        0      169 2023-07-05 01:01:02.117407 protomodel-0.0.1/protomodel/types/get_types.py
--rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.1/protomodel/utils/__init__.py
--rw-r--r--   0        0        0      387 2023-07-05 03:29:57.057395 protomodel-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       84 2023-07-04 20:52:27.187402 protomodel-0.0.2/README.md
+-rw-r--r--   0        0        0      108 2023-07-05 03:31:17.977392 protomodel-0.0.2/protomodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:40:34.047386 protomodel-0.0.2/protomodel/example/__init__.py
+-rw-r--r--   0        0        0     1567 2023-07-05 04:43:58.577395 protomodel-0.0.2/protomodel/example/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0        0        0      330 2023-07-05 04:46:11.747388 protomodel-0.0.2/protomodel/example/data.proto
+-rw-r--r--   0        0        0      330 2023-07-05 04:42:08.657389 protomodel-0.0.2/protomodel/example/data.py
+-rw-r--r--   0        0        0      521 2023-07-05 04:44:24.847394 protomodel-0.0.2/protomodel/example/run.py
+-rw-r--r--   0        0        0       22 2023-07-05 03:07:25.797387 protomodel-0.0.2/protomodel/grpc.py
+-rw-r--r--   0        0        0     1068 2023-07-05 04:39:57.197387 protomodel-0.0.2/protomodel/message.py
+-rw-r--r--   0        0        0        0 2023-07-05 03:31:11.937394 protomodel-0.0.2/protomodel/protomodel/__init__.py
+-rw-r--r--   0        0        0      329 2023-07-04 21:40:33.857408 protomodel-0.0.2/protomodel/protomodel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      377 2023-07-04 21:40:33.867408 protomodel-0.0.2/protomodel/protomodel/__pycache__/grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-05 03:00:39.517398 protomodel-0.0.2/protomodel/protomodel/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0        0        0      384 2023-07-04 21:40:33.867408 protomodel-0.0.2/protomodel/protomodel/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0        0        0       25 2023-07-05 03:07:52.257387 protomodel-0.0.2/protomodel/service.py
+-rw-r--r--   0        0        0       45 2023-07-05 00:34:36.687412 protomodel-0.0.2/protomodel/types/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-05 00:34:59.067411 protomodel-0.0.2/protomodel/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      409 2023-07-05 01:01:08.637407 protomodel-0.0.2/protomodel/types/__pycache__/get_types.cpython-311.pyc
+-rw-r--r--   0        0        0      169 2023-07-05 01:01:02.117407 protomodel-0.0.2/protomodel/types/get_types.py
+-rw-r--r--   0        0        0        0 2023-07-05 00:59:28.647385 protomodel-0.0.2/protomodel/utils/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-05 04:47:02.627389 protomodel-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 protomodel-0.0.2/PKG-INFO
```

### Comparing `protomodel-0.0.1/protomodel/message.py` & `protomodel-0.0.2/protomodel/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,9 +20,11 @@
             file.write(f"\t{type_field} {field} = {index};\n")
 
         file.write(f"}}\n\n")
 
     def get_type_string(self, type_hint):
         if hasattr(type_hint, "__origin__") and type_hint.__origin__ in [List, list]:
             return f"{get_types(type_hint.__name__)} {type_hint.__args__[0].message.__name__}"
-        else:
-            return get_types(type_hint.__name__)
+        try:
+            return get_types(type_hint.__name__)
+        except:
+            return type_hint.message.__name__ if hasattr(type_hint, "message") else type_hint.__name__
```

