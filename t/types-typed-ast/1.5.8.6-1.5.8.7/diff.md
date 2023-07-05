# Comparing `tmp/types-typed-ast-1.5.8.6.tar.gz` & `tmp/types-typed-ast-1.5.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-typed-ast-1.5.8.6.tar", last modified: Tue Mar 28 12:33:13 2023, max compression
+gzip compressed data, was "types-typed-ast-1.5.8.7.tar", last modified: Wed Jul  5 18:21:31 2023, max compression
```

## Comparing `types-typed-ast-1.5.8.6.tar` & `types-typed-ast-1.5.8.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:13.861138 types-typed-ast-1.5.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-28 12:33:13.861138 types-typed-ast-1.5.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:13.861138 types-typed-ast-1.5.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:13.861138 types-typed-ast-1.5.8.6/typed_ast-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/typed_ast-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:25.000000 types-typed-ast-1.5.8.6/typed_ast-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-03-28 12:32:25.000000 types-typed-ast-1.5.8.6/typed_ast-stubs/ast27.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-28 12:32:25.000000 types-typed-ast-1.5.8.6/typed_ast-stubs/ast3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-28 12:32:25.000000 types-typed-ast-1.5.8.6/typed_ast-stubs/conversions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:13.861138 types-typed-ast-1.5.8.6/types_typed_ast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/types_typed_ast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/types_typed_ast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/types_typed_ast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 12:33:13.000000 types-typed-ast-1.5.8.6/types_typed_ast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:31.136128 types-typed-ast-1.5.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-05 18:21:28.000000 types-typed-ast-1.5.8.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 18:21:28.000000 types-typed-ast-1.5.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 18:21:31.136128 types-typed-ast-1.5.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:21:31.136128 types-typed-ast-1.5.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-05 18:21:28.000000 types-typed-ast-1.5.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:31.136128 types-typed-ast-1.5.8.7/typed_ast-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 18:21:28.000000 types-typed-ast-1.5.8.7/typed_ast-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:17.000000 types-typed-ast-1.5.8.7/typed_ast-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-05 18:21:17.000000 types-typed-ast-1.5.8.7/typed_ast-stubs/ast27.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-05 18:21:17.000000 types-typed-ast-1.5.8.7/typed_ast-stubs/ast3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 18:21:17.000000 types-typed-ast-1.5.8.7/typed_ast-stubs/conversions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:21:31.136128 types-typed-ast-1.5.8.7/types_typed_ast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 18:21:31.000000 types-typed-ast-1.5.8.7/types_typed_ast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-05 18:21:31.000000 types-typed-ast-1.5.8.7/types_typed_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:21:31.000000 types-typed-ast-1.5.8.7/types_typed_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 18:21:31.000000 types-typed-ast-1.5.8.7/types_typed_ast.egg-info/top_level.txt
```

### Comparing `types-typed-ast-1.5.8.6/CHANGELOG.md` & `types-typed-ast-1.5.8.7/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.5.8.7 (2023-07-05)
+
+Mark `types-typed-ast` as no longer updated (#10410)
+
 ## 1.5.8.6 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 1.5.8.5 (2023-03-11)
 
 typed_ast: Add missing field to `typed_ast.ast3.TypeIgnore` (#9868)
```

### Comparing `types-typed-ast-1.5.8.6/PKG-INFO` & `types-typed-ast-1.5.8.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-typed-ast
-Version: 1.5.8.6
+Version: 1.5.8.7
 Summary: Typing stubs for typed-ast
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/typed-ast.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `typed-ast`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/typed-ast. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-typed-ast` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `597810e46e823732a87dd7c0c6632e2c63a40016` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-typed-ast-1.5.8.6/setup.py` & `types-typed-ast-1.5.8.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `typed-ast`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/typed-ast. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-typed-ast` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `597810e46e823732a87dd7c0c6632e2c63a40016` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.5.8.6",
+      version="1.5.8.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/typed-ast.md",
```

### Comparing `types-typed-ast-1.5.8.6/typed_ast-stubs/ast27.pyi` & `types-typed-ast-1.5.8.7/typed_ast-stubs/ast27.pyi`

 * *Files identical despite different names*

### Comparing `types-typed-ast-1.5.8.6/typed_ast-stubs/ast3.pyi` & `types-typed-ast-1.5.8.7/typed_ast-stubs/ast3.pyi`

 * *Files identical despite different names*

### Comparing `types-typed-ast-1.5.8.6/types_typed_ast.egg-info/PKG-INFO` & `types-typed-ast-1.5.8.7/types_typed_ast.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-typed-ast
-Version: 1.5.8.6
+Version: 1.5.8.7
 Summary: Typing stubs for typed-ast
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/typed-ast.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `typed-ast`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/typed-ast. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-typed-ast` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `597810e46e823732a87dd7c0c6632e2c63a40016` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

