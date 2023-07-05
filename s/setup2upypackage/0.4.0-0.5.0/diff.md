# Comparing `tmp/setup2upypackage-0.4.0.tar.gz` & `tmp/setup2upypackage-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup2upypackage-0.4.0.tar", last modified: Sat Jun 10 09:26:00 2023, max compression
+gzip compressed data, was "setup2upypackage-0.5.0.tar", last modified: Wed Jul  5 21:02:39 2023, max compression
```

## Comparing `setup2upypackage-0.4.0.tar` & `setup2upypackage-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/setup2upypackage/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/src/setup2upypackage/setup2upypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 09:25:53.000000 setup2upypackage-0.4.0/src/setup2upypackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-10 09:26:00.000000 setup2upypackage-0.4.0/src/setup2upypackage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:26:00.931922 setup2upypackage-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/tests/test_absolute_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-06-10 09:25:40.000000 setup2upypackage-0.4.0/tests/test_setup2upypackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:02:39.338695 setup2upypackage-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/src/setup2upypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/src/setup2upypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/src/setup2upypackage/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/src/setup2upypackage/setup2upypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 21:02:31.000000 setup2upypackage-0.5.0/src/setup2upypackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 21:02:39.000000 setup2upypackage-0.5.0/src/setup2upypackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:02:39.342695 setup2upypackage-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/tests/test_absolute_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-05 21:02:17.000000 setup2upypackage-0.5.0/tests/test_setup2upypackage.py
```

### Comparing `setup2upypackage-0.4.0/LICENSE.txt` & `setup2upypackage-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/PKG-INFO` & `setup2upypackage-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.4.0
+Version: 0.5.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -56,14 +56,15 @@
         - [Options](#options)
     - [Create](#create)
         - [Create package JSON file](#create-package-json-file)
             - [Create specific package JSON file](#create-specific-package-json-file)
         - [Create package JSON file from changelog](#create-package-json-file-from-changelog)
 - [Contributing](#contributing)
     - [Unittests](#unittests)
+    - [Precommit hooks](#precommit-hooks)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
 
 ## Installation
 
 ### Install required tools
@@ -197,14 +198,32 @@
 ```bash
 python create_report_dirs.py
 coverage html
 ```
 
 The coverage report is placed at `reports/coverage/html/index.html`
 
+### Precommit hooks
+
+This repo is equipped with a `.pre-commit-hooks.yaml` file to be usable in
+other repos.
+
+In order to run this repo's pre commit hooks, perform the following steps
+
+```bash
+pip install pre-commit
+# for older systems without colored output support, last supported version is
+# 1.18.3 (7c3404ef1f7593094c854f99bcd3b3eec75fbb2f, 1.19.0 broke it)
+# test it with:
+# from os import openpty
+# r,w = openpty()
+
+pre-commit run --all-files
+```
+
 ## Credits
 
 Based on the [PyPa sample project][ref-pypa-sample].
 
 <!-- Links -->
 [ref-rtd-micropython-package-validation]: https://micropython-package-validation.readthedocs.io/en/latest/
 [ref-pypa-sample]: https://github.com/pypa/sampleproject
```

### Comparing `setup2upypackage-0.4.0/README.md` & `setup2upypackage-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         - [Options](#options)
     - [Create](#create)
         - [Create package JSON file](#create-package-json-file)
             - [Create specific package JSON file](#create-specific-package-json-file)
         - [Create package JSON file from changelog](#create-package-json-file-from-changelog)
 - [Contributing](#contributing)
     - [Unittests](#unittests)
+    - [Precommit hooks](#precommit-hooks)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
 
 ## Installation
 
 ### Install required tools
@@ -171,14 +172,32 @@
 ```bash
 python create_report_dirs.py
 coverage html
 ```
 
 The coverage report is placed at `reports/coverage/html/index.html`
 
+### Precommit hooks
+
+This repo is equipped with a `.pre-commit-hooks.yaml` file to be usable in
+other repos.
+
+In order to run this repo's pre commit hooks, perform the following steps
+
+```bash
+pip install pre-commit
+# for older systems without colored output support, last supported version is
+# 1.18.3 (7c3404ef1f7593094c854f99bcd3b3eec75fbb2f, 1.19.0 broke it)
+# test it with:
+# from os import openpty
+# r,w = openpty()
+
+pre-commit run --all-files
+```
+
 ## Credits
 
 Based on the [PyPa sample project][ref-pypa-sample].
 
 <!-- Links -->
 [ref-rtd-micropython-package-validation]: https://micropython-package-validation.readthedocs.io/en/latest/
 [ref-pypa-sample]: https://github.com/pypa/sampleproject
```

### Comparing `setup2upypackage-0.4.0/setup.py` & `setup2upypackage-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/src/setup2upypackage/main.py` & `setup2upypackage-0.5.0/src/setup2upypackage/main.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/src/setup2upypackage/setup2upypackage.py` & `setup2upypackage-0.5.0/src/setup2upypackage/setup2upypackage.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/src/setup2upypackage.egg-info/PKG-INFO` & `setup2upypackage-0.5.0/src/setup2upypackage.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.4.0
+Version: 0.5.0
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
@@ -56,14 +56,15 @@
         - [Options](#options)
     - [Create](#create)
         - [Create package JSON file](#create-package-json-file)
             - [Create specific package JSON file](#create-specific-package-json-file)
         - [Create package JSON file from changelog](#create-package-json-file-from-changelog)
 - [Contributing](#contributing)
     - [Unittests](#unittests)
+    - [Precommit hooks](#precommit-hooks)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
 
 ## Installation
 
 ### Install required tools
@@ -197,14 +198,32 @@
 ```bash
 python create_report_dirs.py
 coverage html
 ```
 
 The coverage report is placed at `reports/coverage/html/index.html`
 
+### Precommit hooks
+
+This repo is equipped with a `.pre-commit-hooks.yaml` file to be usable in
+other repos.
+
+In order to run this repo's pre commit hooks, perform the following steps
+
+```bash
+pip install pre-commit
+# for older systems without colored output support, last supported version is
+# 1.18.3 (7c3404ef1f7593094c854f99bcd3b3eec75fbb2f, 1.19.0 broke it)
+# test it with:
+# from os import openpty
+# r,w = openpty()
+
+pre-commit run --all-files
+```
+
 ## Credits
 
 Based on the [PyPa sample project][ref-pypa-sample].
 
 <!-- Links -->
 [ref-rtd-micropython-package-validation]: https://micropython-package-validation.readthedocs.io/en/latest/
 [ref-pypa-sample]: https://github.com/pypa/sampleproject
```

### Comparing `setup2upypackage-0.4.0/src/setup2upypackage.egg-info/SOURCES.txt` & `setup2upypackage-0.5.0/src/setup2upypackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/tests/test_absolute_truth.py` & `setup2upypackage-0.5.0/tests/test_absolute_truth.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.4.0/tests/test_setup2upypackage.py` & `setup2upypackage-0.5.0/tests/test_setup2upypackage.py`

 * *Files identical despite different names*

