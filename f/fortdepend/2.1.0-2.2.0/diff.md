# Comparing `tmp/fortdepend-2.1.0.tar.gz` & `tmp/fortdepend-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortdepend-2.1.0.tar", last modified: Wed Feb 16 11:36:37 2022, max compression
+gzip compressed data, was "fortdepend-2.2.0.tar", last modified: Wed Jul  5 07:46:07 2023, max compression
```

## Comparing `fortdepend-2.1.0.tar` & `fortdepend-2.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.068230 fortdepend-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.068230 fortdepend-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-16 11:36:24.000000 fortdepend-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-16 11:36:24.000000 fortdepend-2.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-02-16 11:36:24.000000 fortdepend-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-02-16 11:36:37.072229 fortdepend-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-02-16 11:36:24.000000 fortdepend-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.068230 fortdepend-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-02-16 11:36:24.000000 fortdepend-2.1.0/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-02-16 11:36:24.000000 fortdepend-2.1.0/docs/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-02-16 11:36:24.000000 fortdepend-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-16 11:36:24.000000 fortdepend-2.1.0/docs/fortdepend.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-02-16 11:36:24.000000 fortdepend-2.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.068230 fortdepend-2.1.0/fortdepend/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3434 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12866 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/fort_depend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/smartopen.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-02-16 11:36:24.000000 fortdepend-2.1.0/fortdepend/units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/fortdepend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-02-16 11:36:36.000000 fortdepend-2.1.0/fortdepend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-02-16 11:36:37.000000 fortdepend-2.1.0/fortdepend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 11:36:36.000000 fortdepend-2.1.0/fortdepend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-16 11:36:36.000000 fortdepend-2.1.0/fortdepend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-16 11:36:36.000000 fortdepend-2.1.0/fortdepend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-16 11:36:37.000000 fortdepend-2.1.0/fortdepend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-02-16 11:36:24.000000 fortdepend-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-02-16 11:36:37.076229 fortdepend-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 11:36:24.000000 fortdepend-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/tests/test_fortranfile/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/moduleA.f90
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/moduleB.f90
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/moduleC.f90
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/moduleD.f90
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/moduleE.f90
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/multiple_modules.f90
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/preprocessor.f90
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/preprocessor_include_file.F90
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/programTest.f90
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/tests/test_fortranfile/some_include_dir/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile/some_include_dir/some_include.inc
--rw-r--r--   0 runner    (1001) docker     (121)     7579 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:37.072229 fortdepend-2.1.0/tests/test_fortranproject/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/different_ext.f08
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/moduleA.f90
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/moduleB.f90
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/moduleC.f90
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/moduleD.f90
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/moduleE.f90
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/multiple_modules.f90
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject/programTest.f90
--rw-r--r--   0 runner    (1001) docker     (121)    12855 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_fortranproject.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/test_smartopen.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/tests.dot
--rw-r--r--   0 runner    (1001) docker     (121)     3811 2022-02-16 11:36:24.000000 fortdepend-2.1.0/tests/tests.dot.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.151219 fortdepend-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 07:45:53.000000 fortdepend-2.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 07:45:53.000000 fortdepend-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-05 07:46:07.159219 fortdepend-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-05 07:45:53.000000 fortdepend-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/fortdepend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/fortdepend/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3434 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12865 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/fort_depend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/smartopen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/fortdepend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 07:45:53.000000 fortdepend-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 07:46:07.159219 fortdepend-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:45:53.000000 fortdepend-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranfile/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleA.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleB.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleC.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleD.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleE.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/multiple_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/preprocessor.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/preprocessor_include_file.F90
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/programTest.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranfile/some_include_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/some_include_dir/some_include.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranproject/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/different_ext.f08
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleA.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleB.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleC.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleD.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleE.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/multiple_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/programTest.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_smartopen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/tests.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/tests.dot.svg
```

### Comparing `fortdepend-2.1.0/.github/workflows/black.yml` & `fortdepend-2.2.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/.github/workflows/python_publish.yml` & `fortdepend-2.2.0/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/.github/workflows/test.yml` & `fortdepend-2.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/.gitignore` & `fortdepend-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/LICENCE` & `fortdepend-2.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/Makefile` & `fortdepend-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/PKG-INFO` & `fortdepend-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fortdepend
-Version: 2.1.0
+Version: 2.2.0
 Summary: Automatically generate Fortran dependencies
 Home-page: https://github.com/ZedThree/fort_depend.py/
 Author: Peter Hill
 Author-email: peter@fusionplasma.co.uk
 License: MIT
 Keywords: build,dependencies,fortran
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -178,9 +177,7 @@
 This will automatically rebuild the dependency file if any of the
 source files change. You might not like to do this if you have a lot
 of files and need to preprocess them!
 
 [pcpp]: https://github.com/ned14/pcpp
 [graphviz]: https://github.com/xflr6/graphviz
 [docs]: https://fortdepend.readthedocs.io/en/latest/
-
-
```

### Comparing `fortdepend-2.1.0/README.md` & `fortdepend-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/docs/advanced_usage.rst` & `fortdepend-2.2.0/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/docs/basic_usage.rst` & `fortdepend-2.2.0/docs/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/docs/conf.py` & `fortdepend-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/docs/fortdepend.rst` & `fortdepend-2.2.0/docs/fortdepend.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/docs/index.rst` & `fortdepend-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/fortdepend/__main__.py` & `fortdepend-2.2.0/fortdepend/__main__.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/fortdepend/fort_depend.py` & `fortdepend-2.2.0/fortdepend/fort_depend.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         files=None,
         ignore_modules=None,
         macros=None,
         cpp_includes=None,
         use_preprocessor=True,
         verbose=False,
     ):
-
         if name is None:
             self.name = os.path.basename(os.getcwd())
         else:
             self.name = name
 
         if files is None:
             files = self.get_source()
```

### Comparing `fortdepend-2.1.0/fortdepend/graph.py` & `fortdepend-2.2.0/fortdepend/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         filename (str): Name of the output file
         format (str): Image format
         view (bool): Immediately display the graph [True]
 
     """
 
     def __init__(self, tree, filename=None, format="svg", view=True):
-
         if not has_graphviz:
             warnings.warn("graphviz not installed: can't make graph", RuntimeWarning)
             return
 
         if filename is None:
             filename = "graph.dot"
```

### Comparing `fortdepend-2.1.0/fortdepend/smartopen.py` & `fortdepend-2.2.0/fortdepend/smartopen.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/fortdepend/units.py` & `fortdepend-2.2.0/fortdepend/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     ):
         self.filename = filename
         self.uses = None
         self.modules = None
         self.depends_on = None
 
         if readfile:
-            with smart_open(self.filename, "r") as f:
-                contents = f.read()
+            with smart_open(self.filename, "r", encoding="utf-8") as f:
+                contents = f.read().lower()
 
             preprocessor = FortranPreprocessor()
 
             if macros:
                 if isinstance(macros, dict):
                     for k, v in macros.items():
                         preprocessor.define("{} {}".format(k, v))
```

### Comparing `fortdepend-2.1.0/fortdepend.egg-info/PKG-INFO` & `fortdepend-2.2.0/fortdepend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fortdepend
-Version: 2.1.0
+Version: 2.2.0
 Summary: Automatically generate Fortran dependencies
 Home-page: https://github.com/ZedThree/fort_depend.py/
 Author: Peter Hill
 Author-email: peter@fusionplasma.co.uk
 License: MIT
 Keywords: build,dependencies,fortran
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -178,9 +177,7 @@
 This will automatically rebuild the dependency file if any of the
 source files change. You might not like to do this if you have a lot
 of files and need to preprocess them!
 
 [pcpp]: https://github.com/ned14/pcpp
 [graphviz]: https://github.com/xflr6/graphviz
 [docs]: https://fortdepend.readthedocs.io/en/latest/
-
-
```

### Comparing `fortdepend-2.1.0/fortdepend.egg-info/SOURCES.txt` & `fortdepend-2.2.0/fortdepend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/setup.cfg` & `fortdepend-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/conftest.py` & `fortdepend-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/test_fortranfile.py` & `fortdepend-2.2.0/tests/test_fortranfile.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/test_fortranmodule.py` & `fortdepend-2.2.0/tests/test_fortranmodule.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/test_fortranproject.py` & `fortdepend-2.2.0/tests/test_fortranproject.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/test_smartopen.py` & `fortdepend-2.2.0/tests/test_smartopen.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.1.0/tests/tests.dot.svg` & `fortdepend-2.2.0/tests/tests.dot.svg`

 * *Files identical despite different names*

