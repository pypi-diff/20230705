# Comparing `tmp/qdldl-0.1.7.tar.gz` & `tmp/qdldl-0.1.7.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/qdldl-0.1.7.tar", last modified: Wed Apr  5 00:30:28 2023, max compression
+gzip compressed data, was "wheelhouse/qdldl-0.1.7.post0.tar", last modified: Wed Jul  5 18:10:46 2023, max compression
```

## Comparing `qdldl-0.1.7.tar` & `qdldl-0.1.7.post0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-05 00:26:06.000000 qdldl-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-05 00:26:06.000000 qdldl-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-05 00:30:28.000000 qdldl-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-05 00:26:06.000000 qdldl-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/amd/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/amd/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/include/SuiteSparse_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/include/amd.h
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/include/amd_internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/include/perm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/amd/src/
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/SuiteSparse_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_1.c
--rw-r--r--   0 runner    (1001) docker     (123)    64841 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_2.c
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_aat.c
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_control.c
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_defaults.c
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_info.c
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_order.c
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_post_tree.c
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_postorder.c
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_preprocess.c
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/amd_valid.c
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/amd/src/perm.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/configure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/configure/qdldl_types.h.in
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/configure/qdldl_version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/examples/example.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/include/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/include/qdldl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/src/qdldl.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/c/qdldl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/minunit.h
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/qdldl_tester.c
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_basic.h
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_identity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_osqp_kkt.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_rank_deficient.h
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_singleton.h
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_sym_structure.h
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_tril_structure.h
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_two_by_two.h
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-05 00:26:06.000000 qdldl-0.1.7/c/qdldl/tests/test_zero_on_diag.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-05 00:26:06.000000 qdldl-0.1.7/cpp/qdldl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-05 00:26:06.000000 qdldl-0.1.7/cpp/qdldl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-05 00:26:06.000000 qdldl-0.1.7/cpp/wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-05 00:26:06.000000 qdldl-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 00:30:28.000000 qdldl-0.1.7/qdldl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 00:30:28.000000 qdldl-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-05 00:26:06.000000 qdldl-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 00:30:28.000000 qdldl-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 00:26:06.000000 qdldl-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-05 00:26:06.000000 qdldl-0.1.7/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-05 00:26:06.000000 qdldl-0.1.7/tests/test_solve_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-05 00:26:06.000000 qdldl-0.1.7/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/amd/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/include/SuiteSparse_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/include/amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/include/amd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/include/perm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/amd/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/SuiteSparse_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_1.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64841 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_aat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_control.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_info.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_order.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/amd_valid.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/amd/src/perm.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/configure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/configure/qdldl_types.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/configure/qdldl_version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/examples/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/include/qdldl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/src/qdldl.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/c/qdldl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/minunit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/qdldl_tester.c
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_osqp_kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_rank_deficient.h
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_singleton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_sym_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_tril_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_two_by_two.h
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/c/qdldl/tests/test_zero_on_diag.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/cpp/qdldl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/cpp/qdldl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/cpp/wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/qdldl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:10:46.000000 qdldl-0.1.7.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/tests/test_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/tests/test_solve_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 18:06:24.000000 qdldl-0.1.7.post0/tests/utils.py
```

### Comparing `qdldl-0.1.7/LICENSE` & `qdldl-0.1.7.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/PKG-INFO` & `qdldl-0.1.7.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdldl
-Version: 0.1.7
+Version: 0.1.7.post0
 Summary: QDLDL, a free LDL factorization routine.
 Home-page: https://github.com/oxfordcontrol/qdldl-python/
 Author: Bartolomeo Stellato, Paul Goulart, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 Description: # qdldl-python
```

### Comparing `qdldl-0.1.7/README.md` & `qdldl-0.1.7.post0/README.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/CMakeLists.txt` & `qdldl-0.1.7.post0/c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/LICENSE` & `qdldl-0.1.7.post0/c/amd/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/include/SuiteSparse_config.h` & `qdldl-0.1.7.post0/c/amd/include/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/include/amd.h` & `qdldl-0.1.7.post0/c/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/include/amd_internal.h` & `qdldl-0.1.7.post0/c/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/include/perm.h` & `qdldl-0.1.7.post0/c/amd/include/perm.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/SuiteSparse_config.c` & `qdldl-0.1.7.post0/c/amd/src/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_1.c` & `qdldl-0.1.7.post0/c/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_2.c` & `qdldl-0.1.7.post0/c/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_aat.c` & `qdldl-0.1.7.post0/c/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_control.c` & `qdldl-0.1.7.post0/c/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_defaults.c` & `qdldl-0.1.7.post0/c/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_info.c` & `qdldl-0.1.7.post0/c/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_order.c` & `qdldl-0.1.7.post0/c/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_post_tree.c` & `qdldl-0.1.7.post0/c/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_postorder.c` & `qdldl-0.1.7.post0/c/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_preprocess.c` & `qdldl-0.1.7.post0/c/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/amd_valid.c` & `qdldl-0.1.7.post0/c/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/amd/src/perm.c` & `qdldl-0.1.7.post0/c/amd/src/perm.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/.github/workflows/ci.yml` & `qdldl-0.1.7.post0/c/qdldl/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/CHANGELOG.md` & `qdldl-0.1.7.post0/c/qdldl/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/CMakeLists.txt` & `qdldl-0.1.7.post0/c/qdldl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/LICENSE` & `qdldl-0.1.7.post0/c/qdldl/LICENSE`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/README.md` & `qdldl-0.1.7.post0/c/qdldl/README.md`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/configure/cmake/cmake_uninstall.cmake.in` & `qdldl-0.1.7.post0/c/qdldl/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/configure/qdldl_types.h.in` & `qdldl-0.1.7.post0/c/qdldl/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/examples/example.c` & `qdldl-0.1.7.post0/c/qdldl/examples/example.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/include/qdldl.h` & `qdldl-0.1.7.post0/c/qdldl/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/src/qdldl.c` & `qdldl-0.1.7.post0/c/qdldl/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/tests/CMakeLists.txt` & `qdldl-0.1.7.post0/c/qdldl/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/tests/qdldl_tester.c` & `qdldl-0.1.7.post0/c/qdldl/tests/qdldl_tester.c`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/tests/test_basic.h` & `qdldl-0.1.7.post0/c/qdldl/tests/test_basic.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/tests/test_osqp_kkt.h` & `qdldl-0.1.7.post0/c/qdldl/tests/test_osqp_kkt.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/c/qdldl/tests/test_zero_on_diag.h` & `qdldl-0.1.7.post0/c/qdldl/tests/test_zero_on_diag.h`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/cpp/qdldl.hpp` & `qdldl-0.1.7.post0/cpp/qdldl.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -36,18 +36,26 @@
 		QDLDL_int * Aperm_i;
 		QDLDL_float * Aperm_x;
 		QDLDL_int * A2Aperm;
 
 	public:
 		QDLDL_int nx; // Size
 		QDLDL_int nnz; // Number of nonzero elements in the matrix
+		QDLDL_int sum_Lnz; // Number of nonzero elements in the factor L
 
 		Solver(QDLDL_int n, QDLDL_int * Ap, QDLDL_int *Ai, QDLDL_float * Ax);
 		QDLDL_float * solve(QDLDL_float * b);
 		void update(QDLDL_float * Anew_x);
+
+        QDLDL_float *get_D();
+        QDLDL_int *get_Lp();
+        QDLDL_int *get_Li();
+        QDLDL_float *get_Lx();
+        QDLDL_int *get_P();
+
 		~Solver();
 
 };
 
 } // end namespace
```

### Comparing `qdldl-0.1.7/qdldl.egg-info/PKG-INFO` & `qdldl-0.1.7.post0/qdldl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdldl
-Version: 0.1.7
+Version: 0.1.7.post0
 Summary: QDLDL, a free LDL factorization routine.
 Home-page: https://github.com/oxfordcontrol/qdldl-python/
 Author: Bartolomeo Stellato, Paul Goulart, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 Description: # qdldl-python
```

### Comparing `qdldl-0.1.7/qdldl.egg-info/SOURCES.txt` & `qdldl-0.1.7.post0/qdldl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -55,9 +55,10 @@
 qdldl.egg-info/PKG-INFO
 qdldl.egg-info/SOURCES.txt
 qdldl.egg-info/dependency_links.txt
 qdldl.egg-info/requires.txt
 qdldl.egg-info/top_level.txt
 tests/__init__.py
 tests/test_errors.py
+tests/test_factors.py
 tests/test_solve_ls.py
 tests/utils.py
```

### Comparing `qdldl-0.1.7/setup.py` & `qdldl-0.1.7.post0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='qdldl',
-      version='0.1.7',
+      version='0.1.7.post0',
       author='Bartolomeo Stellato, Paul Goulart, Goran Banjac',
       author_email='bartolomeo.stellato@gmail.com',
       description='QDLDL, a free LDL factorization routine.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       package_dir={'qdldl': 'module'},
       include_package_data=True,  # Include package data from MANIFEST.in
```

### Comparing `qdldl-0.1.7/tests/test_errors.py` & `qdldl-0.1.7.post0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qdldl-0.1.7/tests/test_solve_ls.py` & `qdldl-0.1.7.post0/tests/test_solve_ls.py`

 * *Files identical despite different names*

