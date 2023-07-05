# Comparing `tmp/eido-0.2.0.tar.gz` & `tmp/eido-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eido-0.2.0.tar", last modified: Wed Jun 21 14:51:07 2023, max compression
+gzip compressed data, was "eido-0.2.1.tar", last modified: Wed Jul  5 15:53:59 2023, max compression
```

## Comparing `eido-0.2.0.tar` & `eido-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 14:50:58.000000 eido-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 14:50:58.000000 eido-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 14:51:07.686725 eido-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-21 14:50:58.000000 eido-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.682725 eido-0.2.0/eido/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 14:50:58.000000 eido-0.2.0/eido/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-21 14:50:58.000000 eido-0.2.0/eido/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:50:58.000000 eido-0.2.0/eido/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-21 14:50:58.000000 eido-0.2.0/eido/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-21 14:50:58.000000 eido-0.2.0/eido/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 14:50:58.000000 eido-0.2.0/eido/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:50:58.000000 eido-0.2.0/eido/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 14:50:58.000000 eido-0.2.0/eido/conversion_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-21 14:50:58.000000 eido-0.2.0/eido/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-21 14:50:58.000000 eido-0.2.0/eido/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-21 14:50:58.000000 eido-0.2.0/eido/output_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 14:50:58.000000 eido-0.2.0/eido/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-21 14:50:58.000000 eido-0.2.0/eido/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/eido.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 14:51:07.000000 eido-0.2.0/eido.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:51:07.686725 eido-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 14:50:58.000000 eido-0.2.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:51:07.686725 eido-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-21 14:50:58.000000 eido-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:53:59.500368 eido-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-05 15:53:49.000000 eido-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 15:53:49.000000 eido-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 15:53:59.500368 eido-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-05 15:53:49.000000 eido-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:53:59.500368 eido-0.2.1/eido/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 15:53:49.000000 eido-0.2.1/eido/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 15:53:49.000000 eido-0.2.1/eido/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 15:53:49.000000 eido-0.2.1/eido/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-05 15:53:49.000000 eido-0.2.1/eido/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-05 15:53:49.000000 eido-0.2.1/eido/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-05 15:53:49.000000 eido-0.2.1/eido/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-05 15:53:49.000000 eido-0.2.1/eido/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-05 15:53:49.000000 eido-0.2.1/eido/conversion_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-05 15:53:49.000000 eido-0.2.1/eido/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-05 15:53:49.000000 eido-0.2.1/eido/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-05 15:53:49.000000 eido-0.2.1/eido/output_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-05 15:53:49.000000 eido-0.2.1/eido/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-05 15:53:49.000000 eido-0.2.1/eido/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:53:59.500368 eido-0.2.1/eido.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 15:53:59.000000 eido-0.2.1/eido.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 15:53:59.500368 eido-0.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 15:53:49.000000 eido-0.2.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 15:53:49.000000 eido-0.2.1/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 15:53:49.000000 eido-0.2.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 15:53:59.500368 eido-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-05 15:53:49.000000 eido-0.2.1/setup.py
```

### Comparing `eido-0.2.0/LICENSE.txt` & `eido-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/PKG-INFO` & `eido-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eido
-Version: 0.2.0
+Version: 0.2.1
 Summary: A project metadata validator
 Home-page: https://github.com/pepkit/eido/
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `eido-0.2.0/README.md` & `eido-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/__init__.py` & `eido-0.2.1/eido/__init__.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/argparser.py` & `eido-0.2.1/eido/argparser.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/cli.py` & `eido-0.2.1/eido/cli.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/const.py` & `eido-0.2.1/eido/const.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/conversion.py` & `eido-0.2.1/eido/conversion.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/conversion_plugins.py` & `eido-0.2.1/eido/conversion_plugins.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/exceptions.py` & `eido-0.2.1/eido/exceptions.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/inspection.py` & `eido-0.2.1/eido/inspection.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/output_formatters.py` & `eido-0.2.1/eido/output_formatters.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/schema.py` & `eido-0.2.1/eido/schema.py`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/eido/validation.py` & `eido-0.2.1/eido/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     :param Mapping object: an object to validate
     :param str | dict schema: schema dict to validate against or a path to one
         from the error. Useful when used ith large projects
     :raises EidoValidationError: if validation is unsuccessful
     """
     validator = Draft7Validator(schema)
-    print(object, schema)
+    _LOGGER.debug(f"{object},\n {schema}")
     if not validator.is_valid(object):
         errors = sorted(validator.iter_errors(object), key=lambda e: e.path)
         errors_by_type = {}
 
         # Accumulate and restructure error objects by error type
         for error in errors:
             if not error.message in errors_by_type:
```

### Comparing `eido-0.2.0/eido.egg-info/PKG-INFO` & `eido-0.2.1/eido.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eido
-Version: 0.2.0
+Version: 0.2.1
 Summary: A project metadata validator
 Home-page: https://github.com/pepkit/eido/
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `eido-0.2.0/eido.egg-info/SOURCES.txt` & `eido-0.2.1/eido.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eido-0.2.0/setup.py` & `eido-0.2.1/setup.py`

 * *Files identical despite different names*

