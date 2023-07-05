# Comparing `tmp/parse_type-0.6.1.tar.gz` & `tmp/parse_type-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_type-0.6.1.tar", last modified: Sun Jul  2 18:17:41 2023, max compression
+gzip compressed data, was "parse_type-0.6.2.tar", last modified: Wed Jul  5 19:07:28 2023, max compression
```

## Comparing `parse_type-0.6.1.tar` & `parse_type-0.6.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.937255 parse_type-0.6.1/
--rw-r--r--   0 jens       (502) staff       (20)      141 2023-07-02 06:59:36.000000 parse_type-0.6.1/.bumpversion.cfg
--rw-r--r--   0 jens       (502) staff       (20)     1148 2022-03-19 08:12:41.000000 parse_type-0.6.1/.coveragerc
--rw-------   0 jens       (502) staff       (20)      564 2018-10-29 20:24:09.000000 parse_type-0.6.1/.editorconfig
--rw-r--r--   0 jens       (502) staff       (20)     2953 2023-07-02 07:24:28.000000 parse_type-0.6.1/CHANGES.txt
--rw-r--r--   0 jens       (502) staff       (20)     1069 2023-07-02 07:01:28.000000 parse_type-0.6.1/LICENSE
--rw-r--r--   0 jens       (502) staff       (20)      487 2023-07-02 06:59:36.000000 parse_type-0.6.1/MANIFEST.in
--rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-02 18:17:41.937515 parse_type-0.6.1/PKG-INFO
--rw-r--r--   0 jens       (502) staff       (20)     9562 2022-03-11 22:21:42.000000 parse_type-0.6.1/README.rst
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.897128 parse_type-0.6.1/bin/
--rwxr-xr-x   0 jens       (502) staff       (20)      171 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/invoke
--rw-r--r--   0 jens       (502) staff       (20)      207 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/invoke.cmd
--rwx--x--x   0 jens       (502) staff       (20)     7693 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/make_localpi.py
--rwx--x--x   0 jens       (502) staff       (20)      672 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/project_bootstrap.sh
--rwx--x--x   0 jens       (502) staff       (20)     8762 2018-10-29 20:24:10.000000 parse_type-0.6.1/bin/toxcmd.py
--rw-r--r--   0 jens       (502) staff       (20)      694 2023-07-01 20:43:17.000000 parse_type-0.6.1/invoke.yaml
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.904209 parse_type-0.6.1/parse_type/
--rw-r--r--   0 jens       (502) staff       (20)      434 2023-07-02 06:59:36.000000 parse_type-0.6.1/parse_type/__init__.py
--rw-r--r--   0 jens       (502) staff       (20)    12159 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/builder.py
--rw-r--r--   0 jens       (502) staff       (20)     8560 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cardinality.py
--rw-r--r--   0 jens       (502) staff       (20)     6830 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cardinality_field.py
--rw-r--r--   0 jens       (502) staff       (20)     3773 2022-01-18 21:46:14.000000 parse_type-0.6.1/parse_type/cfparse.py
--rw-r--r--   0 jens       (502) staff       (20)    34449 2023-07-01 20:47:57.000000 parse_type-0.6.1/parse_type/parse.py
--rw-r--r--   0 jens       (502) staff       (20)     6176 2018-10-29 20:24:10.000000 parse_type-0.6.1/parse_type/parse_util.py
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.909774 parse_type-0.6.1/parse_type.egg-info/
--rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/PKG-INFO
--rw-r--r--   0 jens       (502) staff       (20)     1236 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (502) staff       (20)      644 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/requires.txt
--rw-r--r--   0 jens       (502) staff       (20)       11 2023-07-02 18:17:41.000000 parse_type-0.6.1/parse_type.egg-info/top_level.txt
--rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-02 06:43:08.000000 parse_type-0.6.1/parse_type.egg-info/zip-safe
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.918114 parse_type-0.6.1/py.requirements/
--rw-r--r--   0 jens       (502) staff       (20)      433 2023-07-01 19:28:19.000000 parse_type-0.6.1/py.requirements/all.txt
--rw-r--r--   0 jens       (502) staff       (20)      526 2023-07-01 19:28:34.000000 parse_type-0.6.1/py.requirements/basic.txt
--rw-r--r--   0 jens       (502) staff       (20)      394 2023-07-01 19:29:19.000000 parse_type-0.6.1/py.requirements/ci.github.testing.txt
--rw-r--r--   0 jens       (502) staff       (20)      907 2023-07-02 06:59:36.000000 parse_type-0.6.1/py.requirements/develop.txt
--rw-r--r--   0 jens       (502) staff       (20)      275 2023-07-02 06:59:36.000000 parse_type-0.6.1/py.requirements/docs.txt
--rw-r--r--   0 jens       (502) staff       (20)      381 2022-01-18 21:46:14.000000 parse_type-0.6.1/py.requirements/optional.txt
--rw-r--r--   0 jens       (502) staff       (20)      325 2023-07-01 19:52:23.000000 parse_type-0.6.1/py.requirements/testing.txt
--rw-r--r--   0 jens       (502) staff       (20)     4119 2023-07-02 18:13:10.000000 parse_type-0.6.1/pyproject.toml
--rw-r--r--   0 jens       (502) staff       (20)     1115 2023-07-02 06:59:36.000000 parse_type-0.6.1/pytest.ini
--rw-r--r--   0 jens       (502) staff       (20)      111 2023-07-02 18:17:41.938852 parse_type-0.6.1/setup.cfg
--rw-r--r--   0 jens       (502) staff       (20)     4343 2023-07-02 18:13:26.000000 parse_type-0.6.1/setup.py
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.925697 parse_type-0.6.1/tasks/
--rw-r--r--   0 jens       (502) staff       (20)     1879 2023-07-01 20:05:14.000000 parse_type-0.6.1/tasks/__init__.py
--rw-r--r--   0 jens       (502) staff       (20)      728 2023-07-01 20:04:08.000000 parse_type-0.6.1/tasks/__main__.py
--rw-r--r--   0 jens       (502) staff       (20)      220 2022-01-18 21:46:14.000000 parse_type-0.6.1/tasks/_compat_shutil.py
--rw-r--r--   0 jens       (502) staff       (20)     7183 2022-01-18 21:46:14.000000 parse_type-0.6.1/tasks/docs.py
--rw-r--r--   0 jens       (502) staff       (20)     1722 2023-07-01 20:09:28.000000 parse_type-0.6.1/tasks/invoke_dry_run.py
--rw-r--r--   0 jens       (502) staff       (20)      840 2023-07-01 20:01:21.000000 parse_type-0.6.1/tasks/py.requirements.txt
--rw-r--r--   0 jens       (502) staff       (20)     7384 2023-07-01 20:09:51.000000 parse_type-0.6.1/tasks/release.py
--rw-r--r--   0 jens       (502) staff       (20)     6937 2023-07-01 20:05:50.000000 parse_type-0.6.1/tasks/test.py
-drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-02 18:17:41.936680 parse_type-0.6.1/tests/
--rw-------   0 jens       (502) staff       (20)        0 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/__init__.py
--rwxr-xr-x   0 jens       (502) staff       (20)     5248 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/parse_type_test.py
--rwxr-xr-x   0 jens       (502) staff       (20)    23498 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_builder.py
--rwxr-xr-x   0 jens       (502) staff       (20)    23905 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_cardinality.py
--rwx--x--x   0 jens       (502) staff       (20)    16286 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_cardinality_field.py
--rwx--x--x   0 jens       (502) staff       (20)     7058 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_cardinality_field0.py
--rw-r--r--   0 jens       (502) staff       (20)     8549 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_cfparse.py
--rw-r--r--   0 jens       (502) staff       (20)    44199 2023-07-01 19:15:46.000000 parse_type-0.6.1/tests/test_parse.py
--rwxr-xr-x   0 jens       (502) staff       (20)     5688 2022-01-18 21:46:14.000000 parse_type-0.6.1/tests/test_parse_decorator.py
--rw-r--r--   0 jens       (502) staff       (20)     1834 2023-07-01 20:54:29.000000 parse_type-0.6.1/tests/test_parse_number.py
--rw-r--r--   0 jens       (502) staff       (20)    18227 2018-10-29 20:24:10.000000 parse_type-0.6.1/tests/test_parse_util.py
--rw-r--r--   0 jens       (502) staff       (20)     3483 2023-07-01 20:28:52.000000 parse_type-0.6.1/tox.ini
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.554926 parse_type-0.6.2/
+-rw-r--r--   0 jens       (502) staff       (20)      141 2023-07-04 04:42:00.000000 parse_type-0.6.2/.bumpversion.cfg
+-rw-r--r--   0 jens       (502) staff       (20)     1148 2022-03-19 08:12:41.000000 parse_type-0.6.2/.coveragerc
+-rw-------   0 jens       (502) staff       (20)      564 2018-10-29 20:24:09.000000 parse_type-0.6.2/.editorconfig
+-rw-r--r--   0 jens       (502) staff       (20)     3294 2023-07-04 04:43:30.000000 parse_type-0.6.2/CHANGES.txt
+-rw-r--r--   0 jens       (502) staff       (20)     1069 2023-07-02 07:01:28.000000 parse_type-0.6.2/LICENSE
+-rw-r--r--   0 jens       (502) staff       (20)      487 2023-07-02 06:59:36.000000 parse_type-0.6.2/MANIFEST.in
+-rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-05 19:07:28.555395 parse_type-0.6.2/PKG-INFO
+-rw-r--r--   0 jens       (502) staff       (20)     9562 2022-03-11 22:21:42.000000 parse_type-0.6.2/README.rst
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.493454 parse_type-0.6.2/bin/
+-rwxr-xr-x   0 jens       (502) staff       (20)      171 2018-10-29 20:24:10.000000 parse_type-0.6.2/bin/invoke
+-rw-r--r--   0 jens       (502) staff       (20)      207 2018-10-29 20:24:10.000000 parse_type-0.6.2/bin/invoke.cmd
+-rwx--x--x   0 jens       (502) staff       (20)     7693 2018-10-29 20:24:10.000000 parse_type-0.6.2/bin/make_localpi.py
+-rwx--x--x   0 jens       (502) staff       (20)      672 2018-10-29 20:24:10.000000 parse_type-0.6.2/bin/project_bootstrap.sh
+-rwx--x--x   0 jens       (502) staff       (20)     8762 2018-10-29 20:24:10.000000 parse_type-0.6.2/bin/toxcmd.py
+-rw-r--r--   0 jens       (502) staff       (20)      694 2023-07-01 20:43:17.000000 parse_type-0.6.2/invoke.yaml
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.500415 parse_type-0.6.2/parse_type/
+-rw-r--r--   0 jens       (502) staff       (20)      434 2023-07-04 04:41:36.000000 parse_type-0.6.2/parse_type/__init__.py
+-rw-r--r--   0 jens       (502) staff       (20)    12159 2022-01-18 21:46:14.000000 parse_type-0.6.2/parse_type/builder.py
+-rw-r--r--   0 jens       (502) staff       (20)     8560 2022-01-18 21:46:14.000000 parse_type-0.6.2/parse_type/cardinality.py
+-rw-r--r--   0 jens       (502) staff       (20)     6830 2022-01-18 21:46:14.000000 parse_type-0.6.2/parse_type/cardinality_field.py
+-rw-r--r--   0 jens       (502) staff       (20)     3773 2022-01-18 21:46:14.000000 parse_type-0.6.2/parse_type/cfparse.py
+-rw-r--r--   0 jens       (502) staff       (20)    34449 2023-07-01 20:47:57.000000 parse_type-0.6.2/parse_type/parse.py
+-rw-r--r--   0 jens       (502) staff       (20)     6176 2018-10-29 20:24:10.000000 parse_type-0.6.2/parse_type/parse_util.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.506589 parse_type-0.6.2/parse_type.egg-info/
+-rw-r--r--   0 jens       (502) staff       (20)    11443 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (502) staff       (20)     1236 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (502) staff       (20)      644 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/requires.txt
+-rw-r--r--   0 jens       (502) staff       (20)       11 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/top_level.txt
+-rw-r--r--   0 jens       (502) staff       (20)        1 2023-07-05 19:07:28.000000 parse_type-0.6.2/parse_type.egg-info/zip-safe
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.516065 parse_type-0.6.2/py.requirements/
+-rw-r--r--   0 jens       (502) staff       (20)      433 2023-07-01 19:28:19.000000 parse_type-0.6.2/py.requirements/all.txt
+-rw-r--r--   0 jens       (502) staff       (20)      526 2023-07-01 19:28:34.000000 parse_type-0.6.2/py.requirements/basic.txt
+-rw-r--r--   0 jens       (502) staff       (20)      394 2023-07-01 19:29:19.000000 parse_type-0.6.2/py.requirements/ci.github.testing.txt
+-rw-r--r--   0 jens       (502) staff       (20)      907 2023-07-02 06:59:36.000000 parse_type-0.6.2/py.requirements/develop.txt
+-rw-r--r--   0 jens       (502) staff       (20)      275 2023-07-02 06:59:36.000000 parse_type-0.6.2/py.requirements/docs.txt
+-rw-r--r--   0 jens       (502) staff       (20)      381 2022-01-18 21:46:14.000000 parse_type-0.6.2/py.requirements/optional.txt
+-rw-r--r--   0 jens       (502) staff       (20)      325 2023-07-01 19:52:23.000000 parse_type-0.6.2/py.requirements/testing.txt
+-rw-r--r--   0 jens       (502) staff       (20)     4119 2023-07-02 18:13:10.000000 parse_type-0.6.2/pyproject.toml
+-rw-r--r--   0 jens       (502) staff       (20)     1115 2023-07-02 06:59:36.000000 parse_type-0.6.2/pytest.ini
+-rw-r--r--   0 jens       (502) staff       (20)      111 2023-07-05 19:07:28.557100 parse_type-0.6.2/setup.cfg
+-rw-r--r--   0 jens       (502) staff       (20)     4343 2023-07-04 04:41:47.000000 parse_type-0.6.2/setup.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.525490 parse_type-0.6.2/tasks/
+-rw-r--r--   0 jens       (502) staff       (20)     1879 2023-07-01 20:05:14.000000 parse_type-0.6.2/tasks/__init__.py
+-rw-r--r--   0 jens       (502) staff       (20)      728 2023-07-01 20:04:08.000000 parse_type-0.6.2/tasks/__main__.py
+-rw-r--r--   0 jens       (502) staff       (20)      220 2022-01-18 21:46:14.000000 parse_type-0.6.2/tasks/_compat_shutil.py
+-rw-r--r--   0 jens       (502) staff       (20)     7183 2022-01-18 21:46:14.000000 parse_type-0.6.2/tasks/docs.py
+-rw-r--r--   0 jens       (502) staff       (20)     1722 2023-07-01 20:09:28.000000 parse_type-0.6.2/tasks/invoke_dry_run.py
+-rw-r--r--   0 jens       (502) staff       (20)      840 2023-07-01 20:01:21.000000 parse_type-0.6.2/tasks/py.requirements.txt
+-rw-r--r--   0 jens       (502) staff       (20)     7384 2023-07-01 20:09:51.000000 parse_type-0.6.2/tasks/release.py
+-rw-r--r--   0 jens       (502) staff       (20)     6937 2023-07-01 20:05:50.000000 parse_type-0.6.2/tasks/test.py
+drwxr-xr-x   0 jens       (502) staff       (20)        0 2023-07-05 19:07:28.553485 parse_type-0.6.2/tests/
+-rw-------   0 jens       (502) staff       (20)        0 2018-10-29 20:24:10.000000 parse_type-0.6.2/tests/__init__.py
+-rwxr-xr-x   0 jens       (502) staff       (20)     5248 2018-10-29 20:24:10.000000 parse_type-0.6.2/tests/parse_type_test.py
+-rwxr-xr-x   0 jens       (502) staff       (20)    23498 2022-01-18 21:46:14.000000 parse_type-0.6.2/tests/test_builder.py
+-rwxr-xr-x   0 jens       (502) staff       (20)    23905 2022-01-18 21:46:14.000000 parse_type-0.6.2/tests/test_cardinality.py
+-rwx--x--x   0 jens       (502) staff       (20)    16286 2018-10-29 20:24:10.000000 parse_type-0.6.2/tests/test_cardinality_field.py
+-rwx--x--x   0 jens       (502) staff       (20)     7058 2018-10-29 20:24:10.000000 parse_type-0.6.2/tests/test_cardinality_field0.py
+-rw-r--r--   0 jens       (502) staff       (20)     8549 2022-01-18 21:46:14.000000 parse_type-0.6.2/tests/test_cfparse.py
+-rw-r--r--   0 jens       (502) staff       (20)    44251 2023-07-04 04:31:28.000000 parse_type-0.6.2/tests/test_parse.py
+-rwxr-xr-x   0 jens       (502) staff       (20)     5688 2022-01-18 21:46:14.000000 parse_type-0.6.2/tests/test_parse_decorator.py
+-rw-r--r--   0 jens       (502) staff       (20)     1834 2023-07-01 20:54:29.000000 parse_type-0.6.2/tests/test_parse_number.py
+-rw-r--r--   0 jens       (502) staff       (20)    18227 2018-10-29 20:24:10.000000 parse_type-0.6.2/tests/test_parse_util.py
+-rw-r--r--   0 jens       (502) staff       (20)     3483 2023-07-01 20:28:52.000000 parse_type-0.6.2/tox.ini
```

### Comparing `parse_type-0.6.1/.coveragerc` & `parse_type-0.6.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/.editorconfig` & `parse_type-0.6.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/CHANGES.txt` & `parse_type-0.6.2/CHANGES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 -------------------------------------------------------------------------------
 
 GOALS:
 
 * Drop support for Python 2.7
 * Support Python >= 3.7 (probably)
 
+Version: 0.6.2 (2023-07-04)
+-------------------------------------------------------------------------------
+
+FIXES:
+
+* #21: tests/test_parse.py tests ``parse_type.parse`` (per default).
+  REASON: Using for older installed ``parse`` module may cause weird problems.
+  RELATED TO: ``parse v1.19.1`` (behavior changed compared to ``v1.19.0``)
+
 
 Version: 0.6.1 (2023-07-02)
 -------------------------------------------------------------------------------
 
 * Switch to MIT license (same as: `parse`_ module)
 * Use SPDX-License-Identifier in source code (to simplify understanding)
 * UPDATE/SYNC to `parse`_ v1.19.1
```

### Comparing `parse_type-0.6.1/LICENSE` & `parse_type-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/PKG-INFO` & `parse_type-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_type
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simplifies to build parse types based on the parse module
 Home-page: https://github.com/jenisys/parse_type
 Download-URL: http://pypi.python.org/pypi/parse_type
 Author: Jens Engel
 Author-email: Jens Engel <jenisys@noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jenisys/parse_type
```

### Comparing `parse_type-0.6.1/README.rst` & `parse_type-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/bin/make_localpi.py` & `parse_type-0.6.2/bin/make_localpi.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/bin/project_bootstrap.sh` & `parse_type-0.6.2/bin/project_bootstrap.sh`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/bin/toxcmd.py` & `parse_type-0.6.2/bin/toxcmd.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/invoke.yaml` & `parse_type-0.6.2/invoke.yaml`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/builder.py` & `parse_type-0.6.2/parse_type/builder.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/cardinality.py` & `parse_type-0.6.2/parse_type/cardinality.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/cardinality_field.py` & `parse_type-0.6.2/parse_type/cardinality_field.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/cfparse.py` & `parse_type-0.6.2/parse_type/cfparse.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/parse.py` & `parse_type-0.6.2/parse_type/parse.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type/parse_util.py` & `parse_type-0.6.2/parse_type/parse_util.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type.egg-info/PKG-INFO` & `parse_type-0.6.2/parse_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-type
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simplifies to build parse types based on the parse module
 Home-page: https://github.com/jenisys/parse_type
 Download-URL: http://pypi.python.org/pypi/parse_type
 Author: Jens Engel
 Author-email: Jens Engel <jenisys@noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jenisys/parse_type
```

### Comparing `parse_type-0.6.1/parse_type.egg-info/SOURCES.txt` & `parse_type-0.6.2/parse_type.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/parse_type.egg-info/requires.txt` & `parse_type-0.6.2/parse_type.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/py.requirements/basic.txt` & `parse_type-0.6.2/py.requirements/basic.txt`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/py.requirements/develop.txt` & `parse_type-0.6.2/py.requirements/develop.txt`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/pyproject.toml` & `parse_type-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/pytest.ini` & `parse_type-0.6.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/setup.py` & `parse_type-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 # -----------------------------------------------------------------------------
 # SETUP:
 # -----------------------------------------------------------------------------
 setup(
     name = "parse_type",
-    version = "0.6.1",
+    version = "0.6.2",
     author = "Jens Engel",
     author_email = "jenisys@noreply.github.com",
     url = "https://github.com/jenisys/parse_type",
     download_url= "http://pypi.python.org/pypi/parse_type",
     description = "Simplifies to build parse types based on the parse module",
     long_description = long_description,
     keywords= "parse, parsing",
```

### Comparing `parse_type-0.6.1/tasks/__init__.py` & `parse_type-0.6.2/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/__main__.py` & `parse_type-0.6.2/tasks/__main__.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/docs.py` & `parse_type-0.6.2/tasks/docs.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/invoke_dry_run.py` & `parse_type-0.6.2/tasks/invoke_dry_run.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/py.requirements.txt` & `parse_type-0.6.2/tasks/py.requirements.txt`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/release.py` & `parse_type-0.6.2/tasks/release.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tasks/test.py` & `parse_type-0.6.2/tasks/test.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/parse_type_test.py` & `parse_type-0.6.2/tests/parse_type_test.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_builder.py` & `parse_type-0.6.2/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_cardinality.py` & `parse_type-0.6.2/tests/test_cardinality.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_cardinality_field.py` & `parse_type-0.6.2/tests/test_cardinality_field.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_cardinality_field0.py` & `parse_type-0.6.2/tests/test_cardinality_field0.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_cfparse.py` & `parse_type-0.6.2/tests/test_cfparse.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_parse.py` & `parse_type-0.6.2/tests/test_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 from datetime import datetime, time
 from decimal import Decimal
 import pickle
 import re
 
 # -- EXTENSION:
 import os
-PARSE_MODULE = os.environ.get("PARSE_TYPE_PARSE_MODULE", "parse")
+PARSE_MODULE = os.environ.get("PARSE_TYPE_PARSE_MODULE", "parse_type")
 if PARSE_MODULE.startswith("parse_type"):
-    # -- USE VENDOR MODULE: parse_type.parse (probably older that original)
+    # -- USE EMBEDDED PARSE MODULE: parse_type.parse
+    # HINT: Has either same version or is older than original module.
     from parse_type import parse
 else:
     # -- USE ORIGINAL MODULE: parse
     import parse
 # -- EXTENSION-END
```

### Comparing `parse_type-0.6.1/tests/test_parse_decorator.py` & `parse_type-0.6.2/tests/test_parse_decorator.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_parse_number.py` & `parse_type-0.6.2/tests/test_parse_number.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tests/test_parse_util.py` & `parse_type-0.6.2/tests/test_parse_util.py`

 * *Files identical despite different names*

### Comparing `parse_type-0.6.1/tox.ini` & `parse_type-0.6.2/tox.ini`

 * *Files identical despite different names*

