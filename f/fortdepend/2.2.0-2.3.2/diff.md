# Comparing `tmp/fortdepend-2.2.0.tar.gz` & `tmp/fortdepend-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortdepend-2.2.0.tar", last modified: Wed Jul  5 07:46:07 2023, max compression
+gzip compressed data, was "fortdepend-2.3.2.tar", last modified: Wed Jul  5 09:39:05 2023, max compression
```

## Comparing `fortdepend-2.2.0.tar` & `fortdepend-2.3.2.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.151219 fortdepend-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 07:45:53.000000 fortdepend-2.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 07:45:53.000000 fortdepend-2.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 07:45:53.000000 fortdepend-2.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-05 07:46:07.159219 fortdepend-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-05 07:45:53.000000 fortdepend-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/fortdepend.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-05 07:45:53.000000 fortdepend-2.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/fortdepend/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3434 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12865 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/fort_depend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/smartopen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-05 07:45:53.000000 fortdepend-2.2.0/fortdepend/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.155219 fortdepend-2.2.0/fortdepend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 07:46:07.000000 fortdepend-2.2.0/fortdepend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-05 07:45:53.000000 fortdepend-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 07:46:07.159219 fortdepend-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:45:53.000000 fortdepend-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranfile/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleA.f90
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleB.f90
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleC.f90
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleD.f90
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/moduleE.f90
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/multiple_modules.f90
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/preprocessor.f90
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/preprocessor_include_file.F90
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/programTest.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranfile/some_include_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile/some_include_dir/some_include.inc
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:46:07.159219 fortdepend-2.2.0/tests/test_fortranproject/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/different_ext.f08
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleA.f90
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleB.f90
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleC.f90
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleD.f90
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/moduleE.f90
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/multiple_modules.f90
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject/programTest.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_fortranproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/test_smartopen.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/tests.dot
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-05 07:45:53.000000 fortdepend-2.2.0/tests/tests.dot.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.923520 fortdepend-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.911520 fortdepend-2.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.915520 fortdepend-2.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 09:38:52.000000 fortdepend-2.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 09:38:52.000000 fortdepend-2.3.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 09:38:52.000000 fortdepend-2.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-05 09:39:05.923520 fortdepend-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-05 09:38:52.000000 fortdepend-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.915520 fortdepend-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-05 09:38:52.000000 fortdepend-2.3.2/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 09:38:52.000000 fortdepend-2.3.2/docs/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-05 09:38:52.000000 fortdepend-2.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 09:38:52.000000 fortdepend-2.3.2/docs/fortdepend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-05 09:38:52.000000 fortdepend-2.3.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.919520 fortdepend-2.3.2/fortdepend/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3374 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/fort_depend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/smartopen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-05 09:38:52.000000 fortdepend-2.3.2/fortdepend/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.919520 fortdepend-2.3.2/fortdepend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 09:39:05.000000 fortdepend-2.3.2/fortdepend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 09:38:52.000000 fortdepend-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:39:05.923520 fortdepend-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.919520 fortdepend-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.919520 fortdepend-2.3.2/tests/test_fortranfile/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/moduleA.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/moduleB.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/moduleC.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/moduleD.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/moduleE.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/multiple_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/preprocessor.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/preprocessor_include_file.F90
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/programTest.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.919520 fortdepend-2.3.2/tests/test_fortranfile/some_include_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile/some_include_dir/some_include.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:39:05.923520 fortdepend-2.3.2/tests/test_fortranproject/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/different_ext.f08
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/moduleA.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/moduleB.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/moduleC.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/moduleD.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/moduleE.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/multiple_modules.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject/programTest.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_fortranproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/test_smartopen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/tests.dot
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-05 09:38:52.000000 fortdepend-2.3.2/tests/tests.dot.svg
```

### Comparing `fortdepend-2.2.0/.github/workflows/black.yml` & `fortdepend-2.3.2/.github/workflows/black.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,26 +9,26 @@
   run:
     shell: bash
 
 jobs:
   black:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Setup Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
     - name: Install black
       run: |
         python -m pip install --upgrade pip
         pip install black
     - name: Version
       run: |
         python --version
         black --version
     - name: Run black
       run: |
-        black fortdepend setup.py tests
+        black fortdepend tests
     - uses: stefanzweifel/git-auto-commit-action@v4
       with:
         commit_message: "Apply black changes"
```

### Comparing `fortdepend-2.2.0/.github/workflows/python_publish.yml` & `fortdepend-2.3.2/.github/workflows/python_publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [published]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - name: Set up Python
-        uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - name: Setup Python
+        uses: actions/setup-python@v4
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
```

### Comparing `fortdepend-2.2.0/.gitignore` & `fortdepend-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/LICENCE` & `fortdepend-2.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/Makefile` & `fortdepend-2.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/PKG-INFO` & `fortdepend-2.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fortdepend
-Version: 2.2.0
+Version: 2.3.2
 Summary: Automatically generate Fortran dependencies
-Home-page: https://github.com/ZedThree/fort_depend.py/
-Author: Peter Hill
-Author-email: peter@fusionplasma.co.uk
+Author-email: Peter Hill <peter.hill@york.ac.uk>
 License: MIT
+Project-URL: Source, https://github.com/ZedThree/fort_depend.py
+Project-URL: Tracker, https://github.com/ZedThree/fort_depend.py/issues
 Keywords: build,dependencies,fortran
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Fortran
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENCE
 
 fortdepend
 ==========
```

### Comparing `fortdepend-2.2.0/README.md` & `fortdepend-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/docs/advanced_usage.rst` & `fortdepend-2.3.2/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/docs/basic_usage.rst` & `fortdepend-2.3.2/docs/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/docs/conf.py` & `fortdepend-2.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/docs/fortdepend.rst` & `fortdepend-2.3.2/docs/fortdepend.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/docs/index.rst` & `fortdepend-2.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/fortdepend/__main__.py` & `fortdepend-2.3.2/fortdepend/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import argparse
+
 import colorama
-from fortdepend import FortranProject
-from fortdepend import __version__
+
+from fortdepend import FortranProject, __version__
 
 
 def create_argument_parser():
     """Create the parser for the command line arguments"""
     # Add command line arguments
     parser = argparse.ArgumentParser(description="Generate Fortran dependencies")
     parser.add_argument("-f", "--files", nargs="+", help="Files to process")
@@ -59,17 +60,15 @@
     parser.add_argument(
         "-n",
         "--no-preprocessor",
         action="store_true",
         help="Don't use the preprocessor",
     )
     parser.add_argument(
-        "--version",
-        action="version",
-        version="%(prog)s {version}".format(version=__version__),
+        "--version", action="version", version=f"%(prog)s {__version__}"
     )
 
     return parser
 
 
 def main(args=None):
     """Run the module as a script"""
```

### Comparing `fortdepend-2.2.0/fortdepend/fort_depend.py` & `fortdepend-2.3.2/fortdepend/fort_depend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from __future__ import print_function
-
-import os
 import sys
+from contextlib import suppress
+from pathlib import Path
 
 # Terminal colours
 from colorama import Fore
 
+from .graph import Graph
 from .smartopen import smart_open
 from .units import FortranFile, FortranModule
-from .graph import Graph
-
-# Python 2/3 compatibility
-try:
-    input = raw_input
-except NameError:
-    pass
 
 DEPFILE_HEADER = "# This file is generated automatically. DO NOT EDIT!"
 DEFAULT_IGNORED_MODULES = ["iso_c_binding", "iso_fortran_env"]
 
 
 class FortranProject:
     """Read a set of Fortran source files and produce a set of
@@ -57,15 +50,15 @@
         ignore_modules=None,
         macros=None,
         cpp_includes=None,
         use_preprocessor=True,
         verbose=False,
     ):
         if name is None:
-            self.name = os.path.basename(os.getcwd())
+            self.name = Path.cwd().name
         else:
             self.name = name
 
         if files is None:
             files = self.get_source()
         elif not isinstance(files, list):
             files = [files]
@@ -103,18 +96,17 @@
         """
 
         if extensions is None:
             extensions = [".f90", ".F90"]
         elif not isinstance(extensions, list):
             extensions = [extensions]
 
-        tmp = os.listdir(".")
         files = []
         for ext in extensions:
-            files.extend([x for x in tmp if x.endswith(ext)])
+            files.extend([x.name for x in Path.cwd().iterdir() if x.suffix == ext])
 
         return files
 
     def get_modules(self):
         """Return a dict of all the modules found in the project
 
         Works by iterating over the list of `FortranFile` and merging
@@ -293,33 +285,31 @@
         Args:
             filename (str): Name of the output file
             overwrite (bool): Overwrite existing dependency file [False]
             build (str): Directory to prepend to filenames
             skip_programs (bool): Don't write dependencies for programs
         """
 
+        build = Path(build)
+
         def _format_dependencies(target, target_extension, dep_list):
-            _, filename = os.path.split(target)
-            target_name = os.path.splitext(filename)[0] + target_extension
-            listing = "\n{} : ".format(os.path.join(build, target_name))
+            target_name = Path(target).with_suffix(target_extension).name
+            listing = f"\n{build / target_name} : "
             for dep in dep_list:
-                _, depfilename = os.path.split(dep)
-                depobjectname = os.path.splitext(depfilename)[0] + ".o"
-                listing += " \\\n\t{}".format(os.path.join(build, depobjectname))
+                depobjectname = Path(dep).with_suffix(".o").name
+                listing += f" \\\n\t{build / depobjectname}"
             listing += "\n"
             return listing
 
+        filename = Path(filename)
+
         # Test file doesn't exist
-        if os.path.exists(filename):
-            if not (overwrite):
-                print(
-                    Fore.RED
-                    + "Warning: file '{}' exists.".format(filename)
-                    + Fore.RESET
-                )
+        if filename.exists():
+            if not overwrite:
+                print(f"{Fore.RED}Warning: file '{filename}' exists.{Fore.RESET}")
                 opt = input("Overwrite? Y... for yes.")
                 if opt.lower().startswith("y"):
                     pass
                 else:
                     return
 
         with smart_open(filename, "w") as f:
@@ -366,21 +356,18 @@
             ignore_modules = []
         elif not isinstance(ignore_modules, list):
             ignore_modules = [ignore_modules]
 
         ignored_modules = ignore_modules + DEFAULT_IGNORED_MODULES
 
         # Remove from module dict
-        for ignore_mod in ignored_modules:
+        for ignore_mod in map(str.lower, ignored_modules):
             self.modules.pop(ignore_mod, None)
             # Remove from 'used' modules
             for module in self.modules.values():
-                try:
+                with suppress(ValueError):
                     module.uses.remove(ignore_mod)
-                except ValueError:
-                    pass
+
             # Remove from 'used' files
             for source_file in self.files.values():
-                try:
+                with suppress(ValueError):
                     source_file.uses.remove(ignore_mod)
-                except ValueError:
-                    pass
```

### Comparing `fortdepend-2.2.0/fortdepend/units.py` & `fortdepend-2.3.2/fortdepend/units.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .preprocessor import FortranPreprocessor
 import re
 
+from .preprocessor import FortranPreprocessor
 from .smartopen import smart_open
 
 UNIT_REGEX = re.compile(
     r"^\s*(?P<unit_type>module(?!\s+procedure)|program)\s+(?P<modname>\w*)",
     re.IGNORECASE,
 )
 END_REGEX = re.compile(
@@ -43,31 +43,31 @@
         self.filename = filename
         self.uses = None
         self.modules = None
         self.depends_on = None
 
         if readfile:
             with smart_open(self.filename, "r", encoding="utf-8") as f:
-                contents = f.read().lower()
+                contents = f.read()
 
             preprocessor = FortranPreprocessor()
+            macros = macros or {}
 
-            if macros:
-                if isinstance(macros, dict):
-                    for k, v in macros.items():
-                        preprocessor.define("{} {}".format(k, v))
-                else:
-                    if not isinstance(macros, list):
-                        macros = [macros]
-                    for macro in macros:
-                        if "=" in macro:
-                            temp = macro.split("=")
-                            preprocessor.define("{} {}".format(*temp))
-                        else:
-                            preprocessor.define(macro)
+            if isinstance(macros, dict):
+                for k, v in macros.items():
+                    preprocessor.define(f"{k} {v}")
+            else:
+                if not isinstance(macros, list):
+                    macros = [macros]
+                for macro in macros:
+                    if "=" in macro:
+                        key, value = macro.split("=")
+                        preprocessor.define(f"{key} {value}")
+                    else:
+                        preprocessor.define(macro)
 
             if cpp_includes:
                 if not isinstance(cpp_includes, list):
                     cpp_includes = [cpp_includes]
                 for include_dir in cpp_includes:
                     preprocessor.add_path(include_dir)
 
@@ -77,54 +77,50 @@
             self.modules = self.get_modules(contents.splitlines())
             self.uses = self.get_uses()
 
     def __str__(self):
         return self.filename
 
     def __repr__(self):
-        return "FortranFile('{}')".format(self.filename)
+        return f"FortranFile('{self.filename}')"
 
     def get_modules(self, contents, macros=None):
         """Return all the modules or programs that are in the file
 
         Args:
             contents (str): Contents of the source file
         """
 
         contains = {}
         found_units = []
         starts = []
         ends = []
 
         for num, line in enumerate(contents):
-            unit = re.match(UNIT_REGEX, line)
-            end = re.match(END_REGEX, line)
-            if unit:
+            if unit := UNIT_REGEX.match(line):
                 found_units.append(unit)
                 starts.append(num)
-            if end:
+            if end := END_REGEX.match(line):
                 ends.append(num)
 
         if found_units:
             if (len(found_units) != len(starts)) or (len(starts) != len(ends)):
-                error_string = (
-                    "Unmatched start/end of modules in {} ({} begins/{} ends)".format(
-                        self.filename, len(starts), len(ends)
-                    )
+                raise ValueError(
+                    f"Unmatched start/end of modules in {self.filename} ({len(starts)} begins/{len(ends)} ends)"
                 )
-                raise ValueError(error_string)
             for unit, start, end in zip(found_units, starts, ends):
                 name = unit.group("modname")
-                contains[name] = FortranModule(
+                mod = FortranModule(
                     unit_type=unit.group("unit_type"),
                     name=name,
                     source_file=self,
                     text=(contents, start, end),
                     macros=macros,
                 )
+                contains[mod.name] = mod
 
         # Remove duplicates before returning
         return contains
 
     def get_uses(self):
         """Return a sorted list of the modules this file USEs"""
 
@@ -147,48 +143,45 @@
         text (tuple): Tuple containing source_file contents, and start and end lines of the module
         macros (dict): Any defined macros
 
     """
 
     def __init__(self, unit_type, name, source_file=None, text=None, macros=None):
         self.unit_type = unit_type.strip().lower()
-        self.name = name.strip().lower()
+        self.name = name.strip().lower() if self.unit_type == "module" else name.strip()
 
         if source_file is not None:
             self.source_file = source_file
             self.defined_at = text[1]
             self.end = text[2]
 
             self.uses = self.get_uses(text[0], macros)
         else:
             self.source_file = FortranFile(filename="empty", readfile=False)
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
-        return "FortranModule({}, '{}', '{}')".format(
-            self.unit_type, self.name, self.source_file.filename
-        )
+        return f"FortranModule({self.unit_type}, '{self.name}', '{self.source_file.filename}')"
 
     def get_uses(self, contents, macros=None):
         """Return which modules are used in the file after expanding macros
 
         Args:
             contents (str): Contents of the source file
             macros (dict): Dict of preprocessor macros to be expanded
 
         """
 
         uses = []
 
         for line in contents[self.defined_at : self.end]:
-            found = re.match(USE_REGEX, line)
-            if found:
-                uses.append(found.group("moduse").strip())
+            if found := USE_REGEX.match(line):
+                uses.append(found.group("moduse").strip().lower())
 
         # Remove duplicates
         uniq_mods = list(set(uses))
 
         if macros is not None:
             for i, mod in enumerate(uniq_mods):
                 for k, v in macros.items():
```

### Comparing `fortdepend-2.2.0/fortdepend.egg-info/PKG-INFO` & `fortdepend-2.3.2/fortdepend.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fortdepend
-Version: 2.2.0
+Version: 2.3.2
 Summary: Automatically generate Fortran dependencies
-Home-page: https://github.com/ZedThree/fort_depend.py/
-Author: Peter Hill
-Author-email: peter@fusionplasma.co.uk
+Author-email: Peter Hill <peter.hill@york.ac.uk>
 License: MIT
+Project-URL: Source, https://github.com/ZedThree/fort_depend.py
+Project-URL: Tracker, https://github.com/ZedThree/fort_depend.py/issues
 Keywords: build,dependencies,fortran
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Fortran
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENCE
 
 fortdepend
 ==========
```

### Comparing `fortdepend-2.2.0/fortdepend.egg-info/SOURCES.txt` & `fortdepend-2.3.2/fortdepend.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 .coveragerc
 .gitignore
 .readthedocs.yml
 LICENCE
 Makefile
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 .github/workflows/black.yml
 .github/workflows/python_publish.yml
 .github/workflows/test.yml
 docs/advanced_usage.rst
 docs/basic_usage.rst
 docs/conf.py
 docs/fortdepend.rst
```

### Comparing `fortdepend-2.2.0/tests/conftest.py` & `fortdepend-2.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/tests/test_fortranfile.py` & `fortdepend-2.3.2/tests/test_fortranfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,51 +29,51 @@
 
     def test_get_empty_uses(self):
         assert self.testfile.uses is None
         assert self.testfile.get_uses() == []
 
     def test_get_single_module(self):
         contents = ["module modA", "end module modA"]
-        expected = {"modA": "FortranModule(module, 'moda', 'file.f90')"}
+        expected = {"moda": "FortranModule(module, 'moda', 'file.f90')"}
 
         assert self.testfile.modules is None
         module_list = self.testfile.get_modules(contents)
 
         for key, value in expected.items():
             assert key in module_list
             assert repr(module_list[key]) == value
 
     def test_get_multiple_modules(self):
         contents = ["module modA", "end module modA", "module modB", "end module modB"]
         expected = {
-            "modA": "FortranModule(module, 'moda', 'file.f90')",
-            "modB": "FortranModule(module, 'modb', 'file.f90')",
+            "moda": "FortranModule(module, 'moda', 'file.f90')",
+            "modb": "FortranModule(module, 'modb', 'file.f90')",
         }
 
         assert self.testfile.modules is None
         module_list = self.testfile.get_modules(contents)
 
         for key, value in expected.items():
             assert key in module_list
             assert repr(module_list[key]) == value
 
     def test_module_with_module_procedure(self):
         contents = ["module modA", "module procedure foo", "end module modA"]
-        expected = {"modA": "FortranModule(module, 'moda', 'file.f90')"}
+        expected = {"moda": "FortranModule(module, 'moda', 'file.f90')"}
 
         assert self.testfile.modules is None
         module_list = self.testfile.get_modules(contents)
 
         for key, value in expected.items():
             assert key in module_list
             assert repr(module_list[key]) == value
 
     def test_get_program(self):
         contents = ["program progA", "end program progA"]
-        expected = {"progA": "FortranModule(program, 'proga', 'file.f90')"}
+        expected = {"progA": "FortranModule(program, 'progA', 'file.f90')"}
 
         assert self.testfile.modules is None
         module_list = self.testfile.get_modules(contents)
 
         for key, value in expected.items():
             assert key in module_list
             assert repr(module_list[key]) == value
@@ -84,17 +84,17 @@
             "end program progA",
             "module modA",
             "end module modA",
             "module modB",
             "end module modB",
         ]
         expected = {
-            "modA": "FortranModule(module, 'moda', 'file.f90')",
-            "modB": "FortranModule(module, 'modb', 'file.f90')",
-            "progA": "FortranModule(program, 'proga', 'file.f90')",
+            "moda": "FortranModule(module, 'moda', 'file.f90')",
+            "modb": "FortranModule(module, 'modb', 'file.f90')",
+            "progA": "FortranModule(program, 'progA', 'file.f90')",
         }
 
         assert self.testfile.modules is None
         module_list = self.testfile.get_modules(contents)
 
         for key, value in expected.items():
             assert key in module_list
@@ -115,69 +115,69 @@
 class TestReadFortranFile:
     def test_empty_uses(self):
         testfile = FortranFile(filename="moduleA.f90", readfile=True)
         assert testfile.uses == []
 
     def test_get_single_module(self):
         testfile = FortranFile(filename="moduleA.f90", readfile=True)
-        expected = {"modA": "FortranModule(module, 'moda', 'moduleA.f90')"}
+        expected = {"moda": "FortranModule(module, 'moda', 'moduleA.f90')"}
 
         for key, value in expected.items():
             assert key in testfile.modules
             assert repr(testfile.modules[key]) == value
 
     def test_get_program_and_multiple_modules(self):
         testfile = FortranFile(filename="multiple_modules.f90", readfile=True)
         expected = {
-            "modA": "FortranModule(module, 'moda', 'multiple_modules.f90')",
-            "modB": "FortranModule(module, 'modb', 'multiple_modules.f90')",
-            "modC": "FortranModule(module, 'modc', 'multiple_modules.f90')",
-            "modD": "FortranModule(module, 'modd', 'multiple_modules.f90')",
-            "progA": "FortranModule(program, 'proga', 'multiple_modules.f90')",
+            "moda": "FortranModule(module, 'moda', 'multiple_modules.f90')",
+            "modb": "FortranModule(module, 'modb', 'multiple_modules.f90')",
+            "modc": "FortranModule(module, 'modc', 'multiple_modules.f90')",
+            "modd": "FortranModule(module, 'modd', 'multiple_modules.f90')",
+            "progA": "FortranModule(program, 'progA', 'multiple_modules.f90')",
         }
 
         for key, value in expected.items():
             assert key in testfile.modules
             assert repr(testfile.modules[key]) == value
 
     def test_single_uses(self):
         testfile = FortranFile(filename="moduleB.f90", readfile=True)
-        assert testfile.uses == ["modA"]
+        assert testfile.uses == ["moda"]
 
     def test_multiple_uses(self):
         testfile = FortranFile(filename="moduleC.f90", readfile=True)
-        assert set(testfile.uses) == set(["modA", "modB"])
+        assert set(testfile.uses) == set(["moda", "modb"])
 
     def test_multiple_uses_in_multiple_units(self):
         testfile = FortranFile(filename="multiple_modules.f90", readfile=True)
         assert set(testfile.uses) == set(
-            ["modA", "modB", "modC", "modD", "iso_c_binding"]
+            ["moda", "modb", "modc", "modd", "iso_c_binding"]
         )
 
     def test_macro_replacement_dict(self):
         testfile = FortranFile(
             filename="moduleC.f90",
             readfile=True,
             macros={"modA": "module_A", "modB": "module_B"},
         )
-        assert sorted(testfile.uses) == sorted(["module_A", "module_B"])
+        assert sorted(testfile.uses) == sorted(["module_a", "module_b"])
 
     def test_macro_replacement_list(self):
         testfile = FortranFile(
             filename="moduleC.f90",
             readfile=True,
             macros=["modA=module_A", "modB=module_B"],
         )
-        assert sorted(testfile.uses) == sorted(["module_A", "module_B"])
+        assert sorted(testfile.uses) == sorted(["module_a", "module_b"])
 
     def test_macro_replacement_single_value(self):
         testfile = FortranFile(
             filename="moduleC.f90", readfile=True, macros="modA=module_A"
         )
-        assert sorted(testfile.uses) == sorted(["module_A", "modB"])
+        assert sorted(testfile.uses) == sorted(["module_a", "modb"])
 
     def test_conditional_include(self):
         testfile = FortranFile(
             filename="preprocessor.f90", readfile=True, macros=["FOO"]
         )
         assert testfile.uses == ["foo"]
```

### Comparing `fortdepend-2.2.0/tests/test_fortranmodule.py` & `fortdepend-2.3.2/tests/test_fortranmodule.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/tests/test_fortranproject.py` & `fortdepend-2.3.2/tests/test_fortranproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,22 @@
         ]
 
         assert sorted(testproject.files) == sorted(expected_files)
 
     def test_get_all_modules(self):
         testproject = FortranProject()
         expected_modules = [
-            "modA",
-            "modB",
-            "modC",
-            "modD",
-            "modE",
-            "modF",
-            "modG",
-            "modH",
+            "moda",
+            "modb",
+            "modc",
+            "modd",
+            "mode",
+            "modf",
+            "modg",
+            "modh",
             "progA",
             "test",
         ]
 
         assert sorted(testproject.modules) == sorted(expected_modules)
 
     def test_get_all_programs(self):
@@ -82,19 +82,19 @@
             "programTest.f90",
         ]
 
         assert sorted(testproject.files) == sorted(expected_files)
 
     def test_ignore_modules(self):
         testproject = FortranProject(
-            files="multiple_modules.f90", ignore_modules="modF"
+            files="multiple_modules.f90", ignore_modules=["modF", "modg"]
         )
-        assert sorted(["modG", "modH", "progA"]) == sorted(testproject.modules.keys())
-        assert [] == testproject.modules["modG"].uses
-        assert sorted(["modG", "modH"]) == sorted(
+        assert sorted(["modh", "progA"]) == sorted(testproject.modules.keys())
+        assert [] == testproject.modules["modh"].uses
+        assert sorted(["modh"]) == sorted(
             testproject.files["multiple_modules.f90"].uses
         )
 
     def test_depends_by_module(self):
         """This one is a little complicated...
 
         The dictionary depends_by_module uses FortranModule objects as
@@ -330,16 +330,16 @@
             if line != ""
         ]
 
         assert sorted(expected_contents) == sorted(contents)
 
     def test_get_all_used_modules(self):
         expected_used = {
-            "progA": sorted(["modF", "modG", "modH"]),
-            "test": sorted(["modA", "modB", "modC", "modD"]),
+            "progA": sorted(["modf", "modg", "modh"]),
+            "test": sorted(["moda", "modb", "modc", "modd"]),
         }
 
         testproject = FortranProject()
         used_by_program = {}
         for program in testproject.programs.keys():
             used_by_program[program] = testproject.get_all_used_modules(program)
```

### Comparing `fortdepend-2.2.0/tests/test_smartopen.py` & `fortdepend-2.3.2/tests/test_smartopen.py`

 * *Files identical despite different names*

### Comparing `fortdepend-2.2.0/tests/tests.dot.svg` & `fortdepend-2.3.2/tests/tests.dot.svg`

 * *Files identical despite different names*

