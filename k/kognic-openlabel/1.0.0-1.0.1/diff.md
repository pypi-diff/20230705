# Comparing `tmp/kognic-openlabel-1.0.0.tar.gz` & `tmp/kognic-openlabel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kognic-openlabel-1.0.0.tar", last modified: Tue Oct 18 13:10:02 2022, max compression
+gzip compressed data, was "kognic-openlabel-1.0.1.tar", last modified: Wed Jul  5 13:05:00 2023, max compression
```

## Comparing `kognic-openlabel-1.0.0.tar` & `kognic-openlabel-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.753451 kognic-openlabel-1.0.0/
--rw-r--r--   0 oskarolin   (501) staff       (20)     2235 2022-10-18 13:10:02.753583 kognic-openlabel-1.0.0/PKG-INFO
--rw-r--r--   0 oskarolin   (501) staff       (20)     1649 2022-10-18 12:15:11.000000 kognic-openlabel-1.0.0/README.md
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.744450 kognic-openlabel-1.0.0/kognic/
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.746446 kognic-openlabel-1.0.0/kognic/openlabel/
--rw-r--r--   0 oskarolin   (501) staff       (20)      125 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/__init__.py
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.747452 kognic-openlabel-1.0.0/kognic/openlabel/models/
--rw-r--r--   0 oskarolin   (501) staff       (20)       95 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/models/__init__.py
--rw-r--r--   0 oskarolin   (501) staff       (20)    51336 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/models/models.py
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.748654 kognic-openlabel-1.0.0/kognic/openlabel/models/utils/
--rw-r--r--   0 oskarolin   (501) staff       (20)        0 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/models/utils/__init__.py
--rw-r--r--   0 oskarolin   (501) staff       (20)      744 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/models/utils/data_type_parsing.py
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.750346 kognic-openlabel-1.0.0/kognic/openlabel/schemas/
--rw-r--r--   0 oskarolin   (501) staff       (20)        1 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/schemas/__init__.py
--rw-r--r--   0 oskarolin   (501) staff       (20)    69192 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/schemas/openlabel-1-0-0-edited.json
--rw-r--r--   0 oskarolin   (501) staff       (20)    67920 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/schemas/openlabel-1-0-0.json
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.751347 kognic-openlabel-1.0.0/kognic/openlabel/tools/
--rw-r--r--   0 oskarolin   (501) staff       (20)        0 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/tools/__init__.py
--rw-r--r--   0 oskarolin   (501) staff       (20)      663 2022-10-17 14:11:21.000000 kognic-openlabel-1.0.0/kognic/openlabel/tools/model_generation.py
-drwxr-xr-x   0 oskarolin   (501) staff       (20)        0 2022-10-18 13:10:02.753138 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/
--rw-r--r--   0 oskarolin   (501) staff       (20)     2235 2022-10-18 13:10:01.000000 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/PKG-INFO
--rw-r--r--   0 oskarolin   (501) staff       (20)      643 2022-10-18 13:10:02.000000 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/SOURCES.txt
--rw-r--r--   0 oskarolin   (501) staff       (20)        1 2022-10-18 13:10:01.000000 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/dependency_links.txt
--rw-r--r--   0 oskarolin   (501) staff       (20)        7 2022-10-18 13:10:02.000000 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/namespace_packages.txt
--rw-r--r--   0 oskarolin   (501) staff       (20)        7 2022-10-18 13:10:02.000000 kognic-openlabel-1.0.0/kognic_openlabel.egg-info/top_level.txt
--rw-r--r--   0 oskarolin   (501) staff       (20)      720 2022-10-18 13:10:02.754207 kognic-openlabel-1.0.0/setup.cfg
--rw-r--r--   0 oskarolin   (501) staff       (20)     1508 2022-10-17 14:15:45.000000 kognic-openlabel-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/flake8.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.872451 kognic-openlabel-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.872451 kognic-openlabel-1.0.1/src/kognic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic/openlabel/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic/openlabel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51336 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic/openlabel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/models/utils/data_type_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69192 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/openlabel-1-0-0-edited.json
+-rw-r--r--   0 runner    (1001) docker     (123)    67920 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/openlabel-1-0-0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic/openlabel/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/src/kognic/openlabel/tools/model_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 13:05:00.000000 kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:05:00.876451 kognic-openlabel-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-05 13:04:50.000000 kognic-openlabel-1.0.1/tests/test_schema.py
```

### Comparing `kognic-openlabel-1.0.0/PKG-INFO` & `kognic-openlabel-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: kognic-openlabel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kognic OpenLABEL Datamodel
-Home-page: https://github.com/annotell/annotell-python
-Download-URL: https://github.com/annotell/annotell-python/tarball/1.0.0
-Author: Kognic
-Author-email: New Annotation <new-annotation@kognic.com>
+Author-email: Kognic <new-annotation@kognic.com>
 License: MIT
+Project-URL: homepage, https://github.com/annotell/kognic-openlabel-python
 Keywords: Kognic,OpenLABEL
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Kognic OpenLABEL
@@ -51,14 +49,17 @@
 ```
     
 ## Further reading
 https://www.asam.net/project-detail/asam-openlabel-v100/
 
 # Changelog
 
+## [1.0.1] - 2023-07-05
+- Pin pydantic version to <2
+
 ## [1.0.0] - 2022-10-18
 - Annotell becomes Kognic
 
 ## [0.1.4] - 2022-01-24
 - Improved serializability for enum classes
 
 ## [0.1.3] - 2022-01-04
```

### Comparing `kognic-openlabel-1.0.0/README.md` & `kognic-openlabel-1.0.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 ```
     
 ## Further reading
 https://www.asam.net/project-detail/asam-openlabel-v100/
 
 # Changelog
 
+## [1.0.1] - 2023-07-05
+- Pin pydantic version to <2
+
 ## [1.0.0] - 2022-10-18
 - Annotell becomes Kognic
 
 ## [0.1.4] - 2022-01-24
 - Improved serializability for enum classes
 
 ## [0.1.3] - 2022-01-04
```

### Comparing `kognic-openlabel-1.0.0/kognic/openlabel/models/models.py` & `kognic-openlabel-1.0.1/src/kognic/openlabel/models/models.py`

 * *Files identical despite different names*

### Comparing `kognic-openlabel-1.0.0/kognic/openlabel/models/utils/data_type_parsing.py` & `kognic-openlabel-1.0.1/src/kognic/openlabel/models/utils/data_type_parsing.py`

 * *Files identical despite different names*

### Comparing `kognic-openlabel-1.0.0/kognic/openlabel/schemas/openlabel-1-0-0-edited.json` & `kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/openlabel-1-0-0-edited.json`

 * *Files identical despite different names*

### Comparing `kognic-openlabel-1.0.0/kognic/openlabel/schemas/openlabel-1-0-0.json` & `kognic-openlabel-1.0.1/src/kognic/openlabel/schemas/openlabel-1-0-0.json`

 * *Files identical despite different names*

### Comparing `kognic-openlabel-1.0.0/kognic/openlabel/tools/model_generation.py` & `kognic-openlabel-1.0.1/src/kognic/openlabel/tools/model_generation.py`

 * *Files identical despite different names*

### Comparing `kognic-openlabel-1.0.0/kognic_openlabel.egg-info/PKG-INFO` & `kognic-openlabel-1.0.1/src/kognic_openlabel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: kognic-openlabel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kognic OpenLABEL Datamodel
-Home-page: https://github.com/annotell/annotell-python
-Download-URL: https://github.com/annotell/annotell-python/tarball/1.0.0
-Author: Kognic
-Author-email: New Annotation <new-annotation@kognic.com>
+Author-email: Kognic <new-annotation@kognic.com>
 License: MIT
+Project-URL: homepage, https://github.com/annotell/kognic-openlabel-python
 Keywords: Kognic,OpenLABEL
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Kognic OpenLABEL
@@ -51,14 +49,17 @@
 ```
     
 ## Further reading
 https://www.asam.net/project-detail/asam-openlabel-v100/
 
 # Changelog
 
+## [1.0.1] - 2023-07-05
+- Pin pydantic version to <2
+
 ## [1.0.0] - 2022-10-18
 - Annotell becomes Kognic
 
 ## [0.1.4] - 2022-01-24
 - Improved serializability for enum classes
 
 ## [0.1.3] - 2022-01-04
```

### Comparing `kognic-openlabel-1.0.0/setup.cfg` & `kognic-openlabel-1.0.1/setup.cfg`

 * *Files identical despite different names*

