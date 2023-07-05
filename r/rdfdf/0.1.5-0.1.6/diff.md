# Comparing `tmp/rdfdf-0.1.5.tar.gz` & `tmp/rdfdf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfdf-0.1.5.tar", max compression
+gzip compressed data, was "rdfdf-0.1.6.tar", max compression
```

## Comparing `rdfdf-0.1.5.tar` & `rdfdf-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.5/LICENSE
--rw-r--r--   0        0        0     8674 2023-06-29 06:45:26.524130 rdfdf-0.1.5/README.md
--rw-r--r--   0        0        0      459 2023-07-04 12:55:48.452775 rdfdf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.5/rdfdf/__init__.py
--rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_1.py
--rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_2.py
--rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_3.py
--rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.5/rdfdf/examples/example_4.py
--rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.5/rdfdf/helpers/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.5/rdfdf/helpers/importers.py
--rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.5/rdfdf/helpers/rdfdf_utils.py
--rw-r--r--   0        0        0     4234 2023-07-04 12:55:12.926009 rdfdf-0.1.5/rdfdf/rdfdf.py
--rw-r--r--   0        0        0     9231 1970-01-01 00:00:00.000000 rdfdf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 07:12:58.000000 rdfdf-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8674 2023-06-29 06:45:26.524130 rdfdf-0.1.6/README.md
+-rw-r--r--   0        0        0      459 2023-07-05 06:32:54.665184 rdfdf-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 10:17:54.081795 rdfdf-0.1.6/rdfdf/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_1.py
+-rw-r--r--   0        0        0     1154 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_2.py
+-rw-r--r--   0        0        0     1517 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_3.py
+-rw-r--r--   0        0        0     1373 2023-05-15 09:40:40.000000 rdfdf-0.1.6/rdfdf/examples/example_4.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:11:06.000000 rdfdf-0.1.6/rdfdf/helpers/__init__.py
+-rw-r--r--   0        0        0     1323 2023-06-20 14:36:07.751495 rdfdf-0.1.6/rdfdf/helpers/importers.py
+-rw-r--r--   0        0        0      969 2023-05-22 07:07:02.000000 rdfdf-0.1.6/rdfdf/helpers/rdfdf_utils.py
+-rw-r--r--   0        0        0     4201 2023-07-05 06:32:04.361342 rdfdf-0.1.6/rdfdf/rdfdf.py
+-rw-r--r--   0        0        0     9231 1970-01-01 00:00:00.000000 rdfdf-0.1.6/PKG-INFO
```

### Comparing `rdfdf-0.1.5/LICENSE` & `rdfdf-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/README.md` & `rdfdf-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/examples/example_1.py` & `rdfdf-0.1.6/rdfdf/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/examples/example_2.py` & `rdfdf-0.1.6/rdfdf/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/examples/example_3.py` & `rdfdf-0.1.6/rdfdf/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/examples/example_4.py` & `rdfdf-0.1.6/rdfdf/examples/example_4.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/helpers/importers.py` & `rdfdf-0.1.6/rdfdf/helpers/importers.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/helpers/rdfdf_utils.py` & `rdfdf-0.1.6/rdfdf/helpers/rdfdf_utils.py`

 * *Files identical despite different names*

### Comparing `rdfdf-0.1.5/rdfdf/rdfdf.py` & `rdfdf-0.1.6/rdfdf/rdfdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,17 @@
                 #     __subject__=_subject,
                 #     __object__=_object,
                 #     __store__=self.store
                 # )(rule)
 
                 ## new
                 field_rule_result = rule(
-                    __subject__=_subject,
-                    __object__=_object,
-                    __store__=self.store
+                    _subject,
+                    _object,
+                    self.store
                 )
 
                 # yield only rdflib.Graph instances
                 if isinstance(field_rule_result, Graph):
                     yield field_rule_result
                 continue
```

### Comparing `rdfdf-0.1.5/PKG-INFO` & `rdfdf-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfdf
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: GPL3
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

