# Comparing `tmp/ord-schema-0.3.56.tar.gz` & `tmp/ord-schema-0.3.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.56.tar", last modified: Fri Jun 30 19:04:03 2023, max compression
+gzip compressed data, was "ord-schema-0.3.57.tar", last modified: Wed Jul  5 21:17:03 2023, max compression
```

## Comparing `ord-schema-0.3.56.tar` & `ord-schema-0.3.57.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-30 19:03:38.000000 ord-schema-0.3.56/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:03:38.000000 ord-schema-0.3.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 19:03:38.000000 ord-schema-0.3.56/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 19:04:03.182771 ord-schema-0.3.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-30 19:03:38.000000 ord-schema-0.3.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45197 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-06-30 19:03:38.000000 ord-schema-0.3.56/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.178770 ord-schema-0.3.56/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 19:04:03.000000 ord-schema-0.3.56/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:04:03.182771 ord-schema-0.3.56/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-30 19:03:38.000000 ord-schema-0.3.56/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 19:03:38.000000 ord-schema-0.3.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:04:03.182771 ord-schema-0.3.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-30 19:03:42.000000 ord-schema-0.3.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.965605 ord-schema-0.3.57/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-05 21:16:43.000000 ord-schema-0.3.57/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 21:16:43.000000 ord-schema-0.3.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 21:16:43.000000 ord-schema-0.3.57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-05 21:17:03.965605 ord-schema-0.3.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 21:16:43.000000 ord-schema-0.3.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.957605 ord-schema-0.3.57/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.957605 ord-schema-0.3.57/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.961605 ord-schema-0.3.57/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.961605 ord-schema-0.3.57/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.961605 ord-schema-0.3.57/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45196 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-05 21:16:43.000000 ord-schema-0.3.57/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.957605 ord-schema-0.3.57/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-05 21:17:03.000000 ord-schema-0.3.57/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 21:17:03.000000 ord-schema-0.3.57/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:17:03.000000 ord-schema-0.3.57/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-05 21:17:03.000000 ord-schema-0.3.57/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 21:17:03.000000 ord-schema-0.3.57/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:03.965605 ord-schema-0.3.57/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-05 21:16:43.000000 ord-schema-0.3.57/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-07-05 21:16:43.000000 ord-schema-0.3.57/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-05 21:16:43.000000 ord-schema-0.3.57/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 21:16:43.000000 ord-schema-0.3.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:17:03.965605 ord-schema-0.3.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-05 21:16:46.000000 ord-schema-0.3.57/setup.py
```

### Comparing `ord-schema-0.3.56/LICENSE` & `ord-schema-0.3.57/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/PKG-INFO` & `ord-schema-0.3.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.56
+Version: 0.3.57
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.56/README.md` & `ord-schema-0.3.57/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/__init__.py` & `ord-schema-0.3.57/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/frozen_message.py` & `ord-schema-0.3.57/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/frozen_message_test.py` & `ord-schema-0.3.57/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/logging.py` & `ord-schema-0.3.57/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/macros/__init__.py` & `ord-schema-0.3.57/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/macros/solutions.py` & `ord-schema-0.3.57/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.57/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/macros/workups.py` & `ord-schema-0.3.57/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/message_helpers.py` & `ord-schema-0.3.57/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/message_helpers_test.py` & `ord-schema-0.3.57/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/__init__.py` & `ord-schema-0.3.57/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.57/ord_schema/orm/add_datasets.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.57/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/conftest.py` & `ord-schema-0.3.57/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/database.py` & `ord-schema-0.3.57/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/database_test.py` & `ord-schema-0.3.57/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/mappers.py` & `ord-schema-0.3.57/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.57/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.57/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.57/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/__init__.py` & `ord-schema-0.3.57/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.57/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.57/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.57/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.57/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.57/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/resolvers.py` & `ord-schema-0.3.57/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/resolvers_test.py` & `ord-schema-0.3.57/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/__init__.py` & `ord-schema-0.3.57/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.57/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.57/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.57/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.57/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.57/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -63,14 +63,25 @@
                 type: YIELD
                 percentage {
                     value: $product_yield$
                 }
             }
         }
     }
+    provenance {
+        record_created {
+            time {
+                value: "2023-07-01"
+            }
+            person {
+                name: "test"
+                email: "test@example.com"
+            }
+        }
+    }
     """
     template_filename = os.path.join(dirname, "template.pbtxt")
     with open(template_filename, "w") as f:
         f.write(template_string)
     data = pd.DataFrame(
         {
             "input_smiles": ["C", "CC", "CCC"],
@@ -86,30 +97,39 @@
     reaction1_compound1 = reaction1.inputs["test"].components.add()
     reaction1_compound1.identifiers.add(value="C", type="SMILES")
     reaction1_compound1.amount.mass.CopyFrom(reaction_pb2.Mass(value=1.2, units="GRAM"))
     reaction1_product1 = reaction1.outcomes.add().products.add()
     reaction1_product1.identifiers.add(value="CO", type="SMILES")
     reaction1_product1.measurements.add(analysis_key="my_analysis", type="YIELD", percentage=dict(value=7.8))
     reaction1.outcomes[0].analyses["my_analysis"].type = reaction_pb2.Analysis.WEIGHT
+    reaction1.provenance.record_created.time.value = "2023-07-01"
+    reaction1.provenance.record_created.person.name = "test"
+    reaction1.provenance.record_created.person.email = "test@example.com"
     reaction2 = expected.reactions.add()
     reaction2_compound1 = reaction2.inputs["test"].components.add()
     reaction2_compound1.identifiers.add(value="CC", type="SMILES")
     reaction2_compound1.amount.mass.CopyFrom(reaction_pb2.Mass(value=3.4, units="GRAM"))
     reaction2_product1 = reaction2.outcomes.add().products.add()
     reaction2_product1.identifiers.add(value="CCO", type="SMILES")
     reaction2_product1.measurements.add(analysis_key="my_analysis", type="YIELD", percentage=dict(value=9.0))
     reaction2.outcomes[0].analyses["my_analysis"].type = reaction_pb2.Analysis.WEIGHT
+    reaction2.provenance.record_created.time.value = "2023-07-01"
+    reaction2.provenance.record_created.person.name = "test"
+    reaction2.provenance.record_created.person.email = "test@example.com"
     reaction3 = expected.reactions.add()
     reaction3_compound1 = reaction3.inputs["test"].components.add()
     reaction3_compound1.identifiers.add(value="CCC", type="SMILES")
     reaction3_compound1.amount.mass.CopyFrom(reaction_pb2.Mass(value=5.6, units="GRAM"))
     reaction3_product1 = reaction3.outcomes.add().products.add()
     reaction3_product1.identifiers.add(value="CCCO", type="SMILES")
     reaction3_product1.measurements.add(analysis_key="my_analysis", type="YIELD", percentage=dict(value=8.7))
     reaction3.outcomes[0].analyses["my_analysis"].type = reaction_pb2.Analysis.WEIGHT
+    reaction3.provenance.record_created.time.value = "2023-07-01"
+    reaction3.provenance.record_created.person.name = "test"
+    reaction3.provenance.record_created.person.email = "test@example.com"
     yield template_filename, spreadsheet_filename, expected
 
 
 def test_main(setup, tmp_path):
     template_filename, spreadsheet_filename, expected = setup
     output_filename = (tmp_path / "dataset.pbtxt").as_posix()
     argv = [
```

### Comparing `ord-schema-0.3.56/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.57/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.57/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.57/ord_schema/scripts/process_dataset_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         with pytest.raises(validations.ValidationError, match="validation encountered errors"):
             process_dataset.main(docopt.docopt(process_dataset.__doc__, argv))
         error_filename = f"{dataset2_filename}.error"
         assert os.path.exists(error_filename)
         expected_output = [
             "Reaction: Reactions should have at least 1 reaction input\n",
             "Reaction: Reactions should have at least 1 reaction outcome\n",
+            "Reaction: Reaction requires provenance\n",
         ]
         with open(error_filename) as f:
             assert f.readlines() == expected_output
 
     def test_main_with_updates(self, setup):
         dataset1_filename, _ = setup
         dirname = os.path.dirname(dataset1_filename)
@@ -402,14 +403,17 @@
         component.is_limiting = True
         component.amount.moles.value = 2
         component.amount.moles.units = reaction_pb2.Moles.MILLIMOLE
         reaction.outcomes.add().conversion.value = 25
         image = reaction.observations.add().image
         image.bytes_value = b"test data value"
         image.format = "png"
+        reaction.provenance.record_created.time.value = "2023-07-01"
+        reaction.provenance.record_created.person.name = "test"
+        reaction.provenance.record_created.person.email = "test@example.com"
         dataset = dataset_pb2.Dataset(reactions=[reaction])
         dataset_filename = os.path.join(test_subdirectory, "test.pbtxt")
         message_helpers.write_message(dataset, dataset_filename)
         with pytest.raises(ValueError, match="larger than --max_size"):
             self._run(test_subdirectory, ["--max_size", "0.0"])
 
     def test_delete_dataset(self, setup):
```

### Comparing `ord-schema-0.3.56/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.57/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.57/ord_schema/scripts/validate_dataset_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     dummy_component.identifiers.add(type="CUSTOM")
     dummy_component.identifiers[0].details = "custom_identifier"
     dummy_component.identifiers[0].value = "custom_value"
     dummy_component.is_limiting = True
     dummy_component.amount.mass.value = 1
     dummy_component.amount.mass.units = reaction_pb2.Mass.GRAM
     reaction1.outcomes.add().conversion.value = 75
+    reaction1.provenance.record_created.time.value = "2023-07-01"
+    reaction1.provenance.record_created.person.name = "test"
+    reaction1.provenance.record_created.person.email = "test@example.com"
     dataset1 = dataset_pb2.Dataset(reactions=[reaction1])
     dataset1_filename = os.path.join(test_subdirectory, "dataset1.pbtxt")
     message_helpers.write_message(dataset1, dataset1_filename)
     # reaction2 is empty.
     reaction2 = reaction_pb2.Reaction()
     dataset2 = dataset_pb2.Dataset(reactions=[reaction1, reaction2])
     dataset2_filename = os.path.join(test_subdirectory, "dataset2.pbtxt")
```

### Comparing `ord-schema-0.3.56/ord_schema/templating.py` & `ord-schema-0.3.57/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/templating_test.py` & `ord-schema-0.3.57/ord_schema/templating_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     component = dummy_input.components.add()
     component.identifiers.add(type="SMILES", value="CCO")
     component.is_limiting = True
     component.amount.mass.value = 1
     component.amount.mass.units = reaction_pb2.Mass.GRAM
     outcome.conversion.value = 75
     outcome.conversion.precision = 99
+    message.provenance.record_created.time.value = "2023-07-01"
+    message.provenance.record_created.person.name = "test"
+    message.provenance.record_created.person.email = "test@example.com"
     yield message
 
 
 def test_valid_templating(valid_reaction):
     template_string = text_format.MessageToString(valid_reaction)
     template_string = template_string.replace('value: "CCO"', 'value: "$smiles$"')
     template_string = template_string.replace("value: 75", "value: $conversion$")
@@ -117,14 +120,17 @@
         templating.generate_dataset(template_string, df)
 
 
 def test_missing_values(tmp_path):
     # pylint: disable=too-many-locals
     # Build a template reaction.
     reaction = reaction_pb2.Reaction()
+    reaction.provenance.record_created.time.value = "2023-07-01"
+    reaction.provenance.record_created.person.name = "test"
+    reaction.provenance.record_created.person.email = "test@example.com"
     input1 = reaction.inputs["one"]
     input1_component1 = input1.components.add()
     input1_component1.identifiers.add(value="CCO", type="SMILES")
     input1_component1.amount.mass.value = 1.2
     input1_component1.amount.mass.units = reaction_pb2.Mass.GRAM
     input1_component2 = input1.components.add()
     input1_component2.is_limiting = True
```

### Comparing `ord-schema-0.3.56/ord_schema/units.py` & `ord-schema-0.3.57/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/units_test.py` & `ord-schema-0.3.57/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/updates.py` & `ord-schema-0.3.57/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/updates_test.py` & `ord-schema-0.3.57/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema/validations.py` & `ord-schema-0.3.57/ord_schema/validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 @dataclasses.dataclass
 class ValidationOptions:
     """Options for message validation."""
 
     # Check that Dataset and Reaction IDs are well-formed.
     validate_ids: bool = False
     # Require ReactionProvenance for Reactions.
-    require_provenance: bool = False
+    require_provenance: bool = True
     # Allow reactions with valid reaction SMILES and nothing else.
     allow_reaction_smiles_only: bool = True
 
 
 @dataclasses.dataclass
 class ValidationOutput:
     """Validation output: errors and warnings."""
```

### Comparing `ord-schema-0.3.56/ord_schema/validations_test.py` & `ord-schema-0.3.57/ord_schema/validations_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     # Restore the original showwarning.
     warnings.showwarning = original_showwarning
 
 
 def _run_validation(message, **kwargs):
     original = type(message)()
     original.CopyFrom(message)
+    if "options" not in kwargs:
+        kwargs["options"] = validations.ValidationOptions(require_provenance=False)
     output = validations.validate_message(message, **kwargs)
     # Verify that `message` is unchanged by the validation process.
     assert original == message
     return output
 
 
 @pytest.mark.parametrize(
@@ -358,15 +360,15 @@
 
 
 def test_reaction_id():
     message = reaction_pb2.Reaction()
     _ = message.inputs["test"]
     message.outcomes.add()
     message.reaction_id = "ord-c0bbd41f095a44a78b6221135961d809"
-    options = validations.ValidationOptions(validate_ids=True)
+    options = validations.ValidationOptions(validate_ids=True, require_provenance=False)
     output = _run_validation(message, recurse=False, options=options)
     assert len(output.errors) == 0
     assert len(output.warnings) == 0
 
 
 @pytest.mark.parametrize(
     "reaction_id",
```

### Comparing `ord-schema-0.3.56/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.57/ord_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.56
+Version: 0.3.57
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.56/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.57/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.57/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/proto/dataset.proto` & `ord-schema-0.3.57/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/proto/reaction.proto` & `ord-schema-0.3.57/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/proto/test.proto` & `ord-schema-0.3.57/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.56/setup.py` & `ord-schema-0.3.57/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.56",
+    version="0.3.57",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

