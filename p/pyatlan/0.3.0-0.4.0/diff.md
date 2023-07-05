# Comparing `tmp/pyatlan-0.3.0.tar.gz` & `tmp/pyatlan-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.3.0.tar", last modified: Mon Jul  3 11:36:01 2023, max compression
+gzip compressed data, was "pyatlan-0.4.0.tar", last modified: Wed Jul  5 03:43:15 2023, max compression
```

## Comparing `pyatlan-0.3.0.tar` & `pyatlan-0.4.0.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.562886 pyatlan-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-03 11:35:48.000000 pyatlan-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 11:35:48.000000 pyatlan-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:35:48.000000 pyatlan-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-03 11:36:01.562886 pyatlan-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-03 11:35:48.000000 pyatlan-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.542884 pyatlan-0.3.0/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47536 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/events/atlan_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.546885 pyatlan-0.3.0/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.550885 pyatlan-0.3.0/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60973 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 11:35:48.000000 pyatlan-0.3.0/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.542884 pyatlan-0.3.0/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 11:36:01.000000 pyatlan-0.3.0/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:36:01.562886 pyatlan-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-03 11:35:48.000000 pyatlan-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.550885 pyatlan-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.554885 pyatlan-0.3.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.558885 pyatlan-0.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:36:01.562886 pyatlan-0.3.0/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 11:35:48.000000 pyatlan-0.3.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.251740 pyatlan-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-05 03:43:03.000000 pyatlan-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 03:43:03.000000 pyatlan-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 03:43:03.000000 pyatlan-0.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 03:43:15.251740 pyatlan-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 03:43:03.000000 pyatlan-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.235740 pyatlan-0.4.0/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50168 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.243740 pyatlan-0.4.0/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60934 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 03:43:03.000000 pyatlan-0.4.0/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.239740 pyatlan-0.4.0/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 03:43:15.000000 pyatlan-0.4.0/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 03:43:03.000000 pyatlan-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-05 03:43:03.000000 pyatlan-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 03:43:15.251740 pyatlan-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-05 03:43:03.000000 pyatlan-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.243740 pyatlan-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.247740 pyatlan-0.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.247740 pyatlan-0.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:15.251740 pyatlan-0.4.0/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-05 03:43:03.000000 pyatlan-0.4.0/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.3.0/LICENSE` & `pyatlan-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/PKG-INFO` & `pyatlan-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.3.0
+Version: 0.4.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.3.0/README.md` & `pyatlan-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-0.4.0/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.4.0/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/enum_cache.py` & `pyatlan-0.4.0/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/group_cache.py` & `pyatlan-0.4.0/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/role_cache.py` & `pyatlan-0.4.0/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/cache/user_cache.py` & `pyatlan-0.4.0/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/client/atlan.py` & `pyatlan-0.4.0/pyatlan/client/atlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
+import abc
 import contextlib
 import copy
 import json
 import logging
 import os
+from abc import ABC
 from typing import ClassVar, Generator, Optional, Type, TypeVar, Union
 
 import requests
 from pydantic import (
     BaseSettings,
     HttpUrl,
     PrivateAttr,
@@ -79,14 +81,15 @@
     AssetRequest,
     AssetResponse,
     AtlanObject,
     AtlanTag,
     AtlanTagName,
     AtlanTags,
     BulkRequest,
+    SearchRequest,
 )
 from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataRequest
 from pyatlan.model.enums import (
     AtlanConnectorType,
     AtlanDeleteType,
     AtlanTypeCategory,
     CertificateStatus,
@@ -95,20 +98,15 @@
 from pyatlan.model.group import (
     AtlanGroup,
     CreateGroupRequest,
     CreateGroupResponse,
     GroupResponse,
     RemoveFromGroupRequest,
 )
-from pyatlan.model.lineage import (
-    LineageListRequest,
-    LineageListResponse,
-    LineageRequest,
-    LineageResponse,
-)
+from pyatlan.model.lineage import LineageListRequest, LineageRequest, LineageResponse
 from pyatlan.model.query import ParsedQuery, QueryParserRequest
 from pyatlan.model.response import AssetMutationResponse
 from pyatlan.model.role import RoleResponse
 from pyatlan.model.search import (
     DSL,
     IndexSearchRequest,
     Query,
@@ -129,15 +127,20 @@
     AtlanUser,
     ChangeRoleRequest,
     CreateUserRequest,
     UserMinimalResponse,
     UserResponse,
 )
 from pyatlan.multipart_data_generator import MultipartDataGenerator
-from pyatlan.utils import HTTPStatus, get_logger
+from pyatlan.utils import (
+    API,
+    HTTPStatus,
+    get_logger,
+    unflatten_custom_metadata_for_entity,
+)
 
 LOGGER = get_logger()
 T = TypeVar("T", bound=Referenceable)
 A = TypeVar("A", bound=Asset)
 Assets = Union[
     AtlasGlossary,
     AtlasGlossaryCategory,
@@ -237,60 +240,116 @@
     api_key: str
     _session: requests.Session = PrivateAttr(default_factory=get_session)
     _request_params: dict = PrivateAttr()
 
     class Config:
         env_prefix = "atlan_"
 
-    class SearchResults:
+    class SearchResults(ABC):
         def __init__(
             self,
             client: "AtlanClient",
-            criteria: IndexSearchRequest,
+            endpoint: API,
+            criteria: SearchRequest,
             start: int,
             size: int,
-            count: int,
             assets: list[Asset],
         ):
             self._client = client
+            self._endpoint = endpoint
             self._criteria = criteria
             self._start = start
             self._size = size
-            self.count = count
             self._assets = assets
 
         def current_page(self) -> list[Asset]:
             return self._assets
 
         def next_page(self, start=None, size=None) -> bool:
             self._start = start or self._start + self._size
             if size:
                 self._size = size
             return self._get_next_page() if self._assets else False
 
-        # TODO Rename this here and in `next_page`
+        @abc.abstractmethod
         def _get_next_page(self):
-            self._criteria.dsl.from_ = self._start
-            self._criteria.dsl.size = self._size
+            pass
+
+        # TODO Rename this here and in `next_page`
+        def _get_next_page_json(self):
             raw_json = self._client._call_api(
-                INDEX_SEARCH,
+                self._endpoint,
                 request_obj=self._criteria,
             )
             if "entities" not in raw_json:
                 self._assets = []
-                return False
+                return None
             self._assets = parse_obj_as(list[Asset], raw_json["entities"])
-            return True
+            return raw_json
 
         def __iter__(self) -> Generator[Asset, None, None]:
             while True:
                 yield from self.current_page()
                 if not self.next_page():
                     break
 
+    class IndexSearchResults(SearchResults):
+        def __init__(
+            self,
+            client: "AtlanClient",
+            criteria: IndexSearchRequest,
+            start: int,
+            size: int,
+            count: int,
+            assets: list[Asset],
+        ):
+            super().__init__(client, INDEX_SEARCH, criteria, start, size, assets)
+            self._count = count
+
+        def _get_next_page(self):
+            self._criteria.dsl.from_ = self._start
+            self._criteria.dsl.size = self._size
+            if raw_json := super()._get_next_page_json():
+                self._count = (
+                    raw_json["approximateCount"]
+                    if "approximateCount" in raw_json
+                    else 0
+                )
+                return True
+            return False
+
+        @property
+        def count(self) -> int:
+            return self._count
+
+    class LineageListResults(SearchResults):
+        def __init__(
+            self,
+            client: "AtlanClient",
+            criteria: LineageListRequest,
+            start: int,
+            size: int,
+            has_more: bool,
+            assets: list[Asset],
+        ):
+            super().__init__(client, GET_LINEAGE_LIST, criteria, start, size, assets)
+            self._has_more = has_more
+
+        def _get_next_page(self):
+            self._criteria.offset = self._start
+            self._criteria.size = self._size
+            if raw_json := super()._get_next_page_json():
+                self._has_more = parse_obj_as(bool, raw_json["hasMore"])
+                return True
+            return False
+
+        @property
+        def has_more(self) -> bool:
+            return self._has_more
+
     @classmethod
     def register_client(cls, client: "AtlanClient"):
         if not isinstance(client, AtlanClient):
             raise ValueError("client must be an instance of AtlanClient")
         cls._default_client = client
 
     @classmethod
@@ -850,29 +909,33 @@
     def delete_entity_by_guid(self, guid) -> AssetMutationResponse:
         raw_json = self._call_api(
             DELETE_ENTITY_BY_GUID.format_path_with_params(guid),
             {"deleteType": AtlanDeleteType.SOFT.value},
         )
         return AssetMutationResponse(**raw_json)
 
-    def search(self, criteria: IndexSearchRequest) -> SearchResults:
+    def search(self, criteria: IndexSearchRequest) -> IndexSearchResults:
         raw_json = self._call_api(
             INDEX_SEARCH,
             request_obj=criteria,
         )
         if "entities" in raw_json:
             try:
+                for entity in raw_json["entities"]:
+                    unflatten_custom_metadata_for_entity(
+                        entity=entity, attributes=criteria.attributes
+                    )
                 assets = parse_obj_as(list[Asset], raw_json["entities"])
             except ValidationError as err:
                 LOGGER.error("Problem parsing JSON: %s", raw_json["entities"])
                 raise err
         else:
             assets = []
         count = raw_json["approximateCount"] if "approximateCount" in raw_json else 0
-        return AtlanClient.SearchResults(
+        return AtlanClient.IndexSearchResults(
             client=self,
             criteria=criteria,
             start=criteria.dsl.from_,
             size=criteria.dsl.size,
             count=count,
             assets=assets,
         )
@@ -1233,23 +1296,40 @@
         raw_json = self._call_api(
             GET_LINEAGE, None, lineage_request, exclude_unset=False
         )
         return LineageResponse(**raw_json)
 
     def get_lineage_list(
         self, lineage_request: LineageListRequest
-    ) -> LineageListResponse:
+    ) -> LineageListResults:
         if lineage_request.direction == LineageDirection.BOTH:
             raise InvalidRequestException(
                 message="Unable to request both directions of lineage at the same time through the lineage list API.",
             )
         raw_json = self._call_api(
-            GET_LINEAGE_LIST, None, lineage_request, exclude_unset=True
+            GET_LINEAGE_LIST, None, request_obj=lineage_request, exclude_unset=True
+        )
+        if "entities" in raw_json:
+            try:
+                assets = parse_obj_as(list[Asset], raw_json["entities"])
+                has_more = parse_obj_as(bool, raw_json["hasMore"])
+            except ValidationError as err:
+                LOGGER.error("Problem parsing JSON: %s", raw_json["entities"])
+                raise err
+        else:
+            assets = []
+            has_more = False
+        return AtlanClient.LineageListResults(
+            client=self,
+            criteria=lineage_request,
+            start=lineage_request.offset or 0,
+            size=lineage_request.size or 10,
+            has_more=has_more,
+            assets=assets,
         )
-        return LineageListResponse(**raw_json)
 
     @validate_arguments()
     def find_personas_by_name(
         self,
         name: str,
         attributes: Optional[list[str]] = None,
     ) -> list[Persona]:
```

### Comparing `pyatlan-0.3.0/pyatlan/client/constants.py` & `pyatlan-0.4.0/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/error.py` & `pyatlan-0.4.0/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/events/atlan_event_handler.py` & `pyatlan-0.4.0/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-0.4.0/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/exceptions.py` & `pyatlan-0.4.0/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.4.0/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/assets.py` & `pyatlan-0.4.0/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/atlan_image.py` & `pyatlan-0.4.0/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/core.py` & `pyatlan-0.4.0/pyatlan/model/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
-from typing import TYPE_CHECKING
+from abc import ABC
+from typing import TYPE_CHECKING, List
 
 from pydantic import BaseModel, Extra, Field, validator
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from pydantic.dataclasses import dataclass
@@ -111,14 +112,27 @@
         json_encoders = {
             datetime: lambda v: int(v.timestamp() * 1000),
             "AtlanTagName": AtlanTagName.json_encode_atlan_tag,
         }
         validate_assignment = True
 
 
+class SearchRequest(AtlanObject, ABC):
+    attributes: Optional[List[str]] = Field(
+        description="List of attributes to be returned for each result.",
+        default_factory=list,
+    )
+    offset: Optional[int] = Field(
+        description="Starting point for pagination.", alias="from"
+    )
+    size: Optional[int] = Field(
+        description="How many results to include in each page of results."
+    )
+
+
 @dataclass
 class Announcement:
     announcement_title: str
     announcement_message: Optional[str]
     announcement_type: AnnouncementType
```

### Comparing `pyatlan-0.3.0/pyatlan/model/custom_metadata.py` & `pyatlan-0.4.0/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/enums.py` & `pyatlan-0.4.0/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/events.py` & `pyatlan-0.4.0/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/group.py` & `pyatlan-0.4.0/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/lineage.py` & `pyatlan-0.4.0/pyatlan/model/lineage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from pydantic.dataclasses import dataclass
 
 from pyatlan.error import InvalidRequestError
 from pyatlan.model.assets import Asset
-from pyatlan.model.core import AtlanObject
+from pyatlan.model.core import AtlanObject, SearchRequest
 from pyatlan.model.enums import AtlanComparisonOperator, LineageDirection
 
 
 class LineageRelation(AtlanObject):
     from_entity_id: Optional[str]
     to_entity_id: Optional[str]
     process_id: Optional[str]
@@ -243,15 +243,15 @@
     )
     criteria: List[EntityFilter] = Field(
         description="Basis on which to compare a result for inclusion.",
         alias="criterion",
     )
 
 
-class LineageListRequest(AtlanObject):
+class LineageListRequest(SearchRequest):
     guid: str = Field(
         description="Unique identifier of the asset for which to retrieve lineage."
     )
     depth: int = Field(
         description="Number of degrees of separation (hops) across which lineage should be fetched."
         "A depth of 1 will fetch the immediate upstream or downstream assets, while 2"
         "will also fetch the immediate upstream or downstream assets of those assets,"
@@ -272,17 +272,14 @@
         "in the lineage result."
     )
     relationship_traversal_filters: Optional[FilterList] = Field(
         description="Filters to apply for skipping traversal based on relationships."
         "Any sub-graphs beyond the relationships filtered out by these filters will not be included"
         "in the lineage result."
     )
-    attributes: Optional[List[str]] = Field(
-        description="List of attributes to be returned for each asset."
-    )
     offset: Optional[int] = Field(
         description="Starting point for pagination.", alias="from"
     )
     size: Optional[int] = Field(
         description="How many results to include in each page of results."
     )
     exclude_meanings: Optional[bool] = Field(
@@ -307,20 +304,7 @@
             depth=1000000,
             direction=LineageDirection.DOWNSTREAM,
             offset=0,
             size=10,
             exclude_meanings=True,
             exclude_classifications=True,
         )
-
-
-class LineageListResponse(AtlanObject):
-    entities: List[Asset] = Field(description="Entities in the lineage requested.")
-    has_more: bool = Field(
-        description="Whether there are more entities present in lineage that can be traversed (true) or not (false)."
-    )
-    entity_count: int = Field(
-        description="Total count of entities returned, equal to the size of the entities list."
-    )
-    search_parameters: LineageListRequest = Field(
-        description="Request used to produce this lineage."
-    )
```

### Comparing `pyatlan-0.3.0/pyatlan/model/query.py` & `pyatlan-0.4.0/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/response.py` & `pyatlan-0.4.0/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/role.py` & `pyatlan-0.4.0/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/search.py` & `pyatlan-0.4.0/pyatlan/model/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     StrictInt,
     StrictStr,
     constr,
     validate_arguments,
     validator,
 )
 
-from pyatlan.model.core import AtlanObject
+from pyatlan.model.core import AtlanObject, SearchRequest
 from pyatlan.model.enums import AtlanConnectorType, SortOrder
 
 if TYPE_CHECKING:
     from dataclasses import dataclass
 else:
     from pydantic.dataclasses import dataclass
 
@@ -1774,17 +1774,16 @@
     def validate_query(cls, v, values):
         if v or "post_filter" in values and values["post_filter"]:
             return v
         else:
             raise ValueError("Either query or post_filter is required")
 
 
-class IndexSearchRequest(AtlanObject):
+class IndexSearchRequest(SearchRequest):
     dsl: DSL
-    attributes: list[str] = Field(default_factory=list)
     relation_attributes: list[str] = Field(
         default_factory=list, alias="relationAttributes"
     )
 
     class Config:
         json_encoders = {Query: lambda v: v.to_dict(), SortItem: lambda v: v.to_dict()}
```

### Comparing `pyatlan-0.3.0/pyatlan/model/structs.py` & `pyatlan-0.4.0/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/typedef.py` & `pyatlan-0.4.0/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/model/user.py` & `pyatlan-0.4.0/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/multipart_data_generator.py` & `pyatlan-0.4.0/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/pyatlan/utils.py` & `pyatlan-0.4.0/pyatlan/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
 import enum
 import logging
+import re
 import time
 from functools import reduce
 from typing import Any, Optional
 
 ADMIN_URI = "api/service/"
 BASE_URI = "api/meta/"
 SQL_URI = "api/sql/"
@@ -180,7 +181,33 @@
 
 
 class HTTPStatus:
     OK = 200
     NO_CONTENT = 204
     NOT_FOUND = 404
     SERVICE_UNAVAILABLE = 503
+
+
+def unflatten_custom_metadata(
+    attributes: Optional[list[str]], asset_attributes: Optional[dict[str, Any]]
+) -> Optional[dict[str, Any]]:
+    if not attributes or not asset_attributes:
+        return None
+    retval: dict[str, Any] = {}
+    metadata_attribute = re.compile(r"(\w+)[.](\w+)")
+    for attribute_of_interest in attributes:
+        if matched := metadata_attribute.match(attribute_of_interest):
+            if attribute_of_interest in asset_attributes:
+                key = matched[1]
+                if key not in retval:
+                    retval[key] = {}
+                retval[key][matched[2]] = asset_attributes[attribute_of_interest]
+    return retval
+
+
+def unflatten_custom_metadata_for_entity(
+    entity: dict[str, Any], attributes: Optional[list[str]]
+):
+    if custom_metadata := unflatten_custom_metadata(
+        attributes=attributes, asset_attributes=entity.get("attributes", None)
+    ):
+        entity["businessAttributes"] = custom_metadata
```

### Comparing `pyatlan-0.3.0/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.4.0/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.3.0
+Version: 0.4.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.3.0/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.4.0/pyatlan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.md
+requirements-dev.txt
+requirements.txt
 setup.py
 pyatlan/__init__.py
 pyatlan/error.py
 pyatlan/exceptions.py
 pyatlan/multipart_data_generator.py
 pyatlan/utils.py
 pyatlan/version.txt
```

### Comparing `pyatlan-0.3.0/setup.py` & `pyatlan-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 
 import io
 import os
 
 from setuptools import find_packages, setup
 
 # External dependencies
-requirements = ["requests>=2.24", "pydantic>=1.10.8", "jinja2>=3.1.2"]
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
+
+# Development dependencies
+with open("requirements-dev.txt") as f:
+    extra = f.read().splitlines()
 
 
 def read(file_name):
     """Read a text file and return the content as a string."""
     with io.open(
         os.path.join(os.path.dirname(__file__), file_name), encoding="utf-8"
     ) as f:
@@ -53,29 +58,14 @@
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
     ],
     packages=find_packages(),
     install_requires=requirements,
-    extra_requires={
-        "dev": [
-            "pytest>=7.3.1",
-            "flake8>=5.0.4",
-            "mypy>=0.991",
-            "black>=22.10.0",
-            "types-requests>=2.28.11.17",
-            "pre-commit>=2.20.0",
-            "deepdiff>=6.2.1",
-            "pytest-cov>=4.0.0",
-            "pytest-order==1.1.0",
-            "retry==0.9.2",
-            "types-retry==0.9.9.3",
-            "twine>=4.0.2",
-        ]
-    },
+    extra_requires={"dev": extra},
     include_package_data=True,
     zip_safe=False,
     keywords="atlan client",
     python_requires=">=3.9",
     repository="https://github.com/atlanhq/atlan-python",
 )
```

### Comparing `pyatlan-0.3.0/tests/integration/admin_test.py` & `pyatlan-0.4.0/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/atlan_tag_test.py` & `pyatlan-0.4.0/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/client.py` & `pyatlan-0.4.0/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/connection_test.py` & `pyatlan-0.4.0/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/custom_metadata_test.py` & `pyatlan-0.4.0/tests/integration/custom_metadata_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,16 +507,22 @@
     be_active = Term.with_state("ACTIVE")
     be_a_term = Term.with_type_name("AtlasGlossaryTerm")
     have_attr = Exists.with_custom_metadata(
         set_name=CM_RACI, attr_name=CM_ATTR_RACI_ACCOUNTABLE
     )
     query = Bool(must=[be_active, be_a_term, have_attr])
     dsl = DSL(query=query)
+    attributes = ["name", "anchor"]
+    cm_attributes = CustomMetadataCache.get_attributes_for_search_results(
+        set_name=CM_RACI
+    )
+    assert cm_attributes
+    attributes.extend(cm_attributes)
     request = IndexSearchRequest(
-        dsl=dsl, attributes=["name", "anchor"], relation_attributes=["name"]
+        dsl=dsl, attributes=attributes, relation_attributes=["name"]
     )
     response = client.search(criteria=request)
     assert response
     count = 0
     # TODO: replace with exponential back-off and jitter
     while response.count == 0 and count < 10:
         time.sleep(2)
@@ -526,14 +532,17 @@
     for t in response:
         assert isinstance(t, AtlasGlossaryTerm)
         assert t.guid == term.guid
         assert t.qualified_name == term.qualified_name
         anchor = t.attributes.anchor
         assert anchor
         assert anchor.name == glossary.name
+        _validate_raci_attributes_replacement(
+            client, t.get_custom_metadata(name=CM_RACI)
+        )
 
 
 @pytest.mark.order(after="test_replace_term_cm_ipr")
 def test_search_by_specific_accountable(
     client: AtlanClient,
     cm_raci: CustomMetadataDef,
     glossary: AtlasGlossary,
```

### Comparing `pyatlan-0.3.0/tests/integration/file_test.py` & `pyatlan-0.4.0/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/glossary_test.py` & `pyatlan-0.4.0/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/lineage_test.py` & `pyatlan-0.4.0/tests/integration/lineage_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -395,30 +395,31 @@
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
 ):
     lineage = LineageListRequest.create(guid=table.guid)
     lineage.attributes = ["name"]
+    lineage.size = 1
     response = client.get_lineage_list(lineage)
     assert response
-    assert response.entities
-    assert len(response.entities) == 4
-    assert response.entity_count == 4
-    assert isinstance(response.entities[0], Process)
-    assert isinstance(response.entities[1], MaterialisedView)
-    assert isinstance(response.entities[2], Process)
-    assert isinstance(response.entities[3], View)
-    one = response.entities[3]
+    results = []
+    for a in response:
+        results.append(a)
+    assert len(results) == 4
+    assert isinstance(results[0], Process)
+    assert isinstance(results[1], MaterialisedView)
+    assert isinstance(results[2], Process)
+    assert isinstance(results[3], View)
+    one = results[3]
     assert one.guid == view.guid
     lineage = LineageListRequest.create(guid=table.guid)
     lineage.direction = LineageDirection.UPSTREAM
     response = client.get_lineage_list(lineage)
     assert response
-    assert not response.entities
     assert not response.has_more
 
 
 def test_fetch_lineage_middle(
     client: AtlanClient,
     connection: Connection,
     database: Database,
@@ -486,32 +487,36 @@
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
 ):
     lineage = LineageListRequest.create(guid=mview.guid)
     lineage.attributes = ["name"]
+    lineage.size = 5
     response = client.get_lineage_list(lineage)
     assert response
-    assert response.entities
-    assert len(response.entities) == 2
-    assert response.entity_count == 2
-    assert isinstance(response.entities[0], Process)
-    assert isinstance(response.entities[1], View)
-    assert response.entities[1].guid == view.guid
+    results = []
+    for a in response:
+        results.append(a)
+    assert len(results) == 2
+    assert isinstance(results[0], Process)
+    assert isinstance(results[1], View)
+    assert results[1].guid == view.guid
     lineage = LineageListRequest.create(guid=mview.guid)
     lineage.direction = LineageDirection.UPSTREAM
+    lineage.size = 5
     response = client.get_lineage_list(lineage)
     assert response
-    assert response.entities
-    assert len(response.entities) == 2
-    assert response.entity_count == 2
-    assert isinstance(response.entities[0], Process)
-    assert isinstance(response.entities[1], Table)
-    assert response.entities[1].guid == table.guid
+    results = []
+    for a in response:
+        results.append(a)
+    assert len(results) == 2
+    assert isinstance(results[0], Process)
+    assert isinstance(results[1], Table)
+    assert results[1].guid == table.guid
 
 
 def test_fetch_lineage_end(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
@@ -562,30 +567,31 @@
     mview: MaterialisedView,
     view: View,
     lineage_start: Process,
     lineage_end: Process,
 ):
     lineage = LineageListRequest.create(guid=view.guid)
     lineage.attributes = ["name"]
+    lineage.size = 10
     response = client.get_lineage_list(lineage)
     assert response
-    assert not response.entities
     assert not response.has_more
     lineage = LineageListRequest.create(guid=view.guid)
     lineage.direction = LineageDirection.UPSTREAM
     response = client.get_lineage_list(lineage)
     assert response
-    assert response.entities
-    assert len(response.entities) == 4
-    assert response.entity_count == 4
-    assert isinstance(response.entities[0], Process)
-    assert isinstance(response.entities[1], MaterialisedView)
-    assert isinstance(response.entities[2], Process)
-    assert isinstance(response.entities[3], Table)
-    one = response.entities[3]
+    results = []
+    for a in response:
+        results.append(a)
+    assert len(results) == 4
+    assert isinstance(results[0], Process)
+    assert isinstance(results[1], MaterialisedView)
+    assert isinstance(results[2], Process)
+    assert isinstance(results[3], Table)
+    one = results[3]
     assert one.guid == table.guid
 
 
 def test_search_by_lineage(
     client: AtlanClient,
     connection: Connection,
     database: Database,
```

### Comparing `pyatlan-0.3.0/tests/integration/persona_test.py` & `pyatlan-0.4.0/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/purpose_test.py` & `pyatlan-0.4.0/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/query_parser_test.py` & `pyatlan-0.4.0/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/s3_asset_test.py` & `pyatlan-0.4.0/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/test_client.py` & `pyatlan-0.4.0/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/integration/test_index_search.py` & `pyatlan-0.4.0/tests/integration/test_index_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,16 @@
 
 
 @pytest.mark.parametrize(
     "with_name",
     [
         (method)
         for method in dir(Exists)
-        if method.startswith("with_") and method != "with_custom_metadata"
+        # if method.startswith("with_") and method != "with_custom_metadata"
+        if method == "with_create_time_as_timestamp"
     ],
 )
 def test_exists_query_factory(client: AtlanClient, with_name):
     assert hasattr(Exists, with_name)
     query = getattr(Exists, with_name)()
     filter = ~Term(field="__typeName.keyword", value="__AtlasAuditEntry")
     dsl = DSL(query=query, post_filter=filter, size=1)
```

### Comparing `pyatlan-0.3.0/tests/integration/test_sql_assets.py` & `pyatlan-0.4.0/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/conftest.py` & `pyatlan-0.4.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/badge_condition_test.py` & `pyatlan-0.4.0/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/badge_test.py` & `pyatlan-0.4.0/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/column_test.py` & `pyatlan-0.4.0/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/connection_test.py` & `pyatlan-0.4.0/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/constants.py` & `pyatlan-0.4.0/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/database_test.py` & `pyatlan-0.4.0/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/file_test.py` & `pyatlan-0.4.0/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/glossary_category_test.py` & `pyatlan-0.4.0/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/glossary_term_test.py` & `pyatlan-0.4.0/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/glossary_test.py` & `pyatlan-0.4.0/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/materialised_view_test.py` & `pyatlan-0.4.0/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/process_test.py` & `pyatlan-0.4.0/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/readme_test.py` & `pyatlan-0.4.0/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.4.0/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/s3object_test.py` & `pyatlan-0.4.0/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/schema_test.py` & `pyatlan-0.4.0/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/table_test.py` & `pyatlan-0.4.0/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/model/view_test.py` & `pyatlan-0.4.0/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_atlan_tag_name.py` & `pyatlan-0.4.0/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_client.py` & `pyatlan-0.4.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_custom_metadata.py` & `pyatlan-0.4.0/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_events.py` & `pyatlan-0.4.0/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_glossary_term.py` & `pyatlan-0.4.0/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_lineage.py` & `pyatlan-0.4.0/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_model.py` & `pyatlan-0.4.0/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.3.0/tests/unit/test_search_model.py` & `pyatlan-0.4.0/tests/unit/test_search_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,18 +266,19 @@
     dsl = DSL(
         query=Term(field="__typeName.keyword", value="Schema"),
         post_filter=Term(field="databaseName.keyword", value="ATLAN_SAMPLE_DATA"),
     )
     request = IndexSearchRequest(dsl=dsl, attributes=["schemaName", "databaseName"])
     assert (
         request.json(by_alias=True, exclude_none=True)
-        == '{"dsl": {"from": 0, "size": 100, "track_total_hits": true, '
+        == '{"attributes": ["schemaName", "databaseName"],'
+        ' "dsl": {"from": 0, "size": 100, "track_total_hits": true, '
         '"post_filter": {"term": {"databaseName.keyword": '
         '{"value": "ATLAN_SAMPLE_DATA"}}}, "query": {"term": {"__typeName.keyword": {"value": "Schema"}}}}, '
-        '"attributes": ["schemaName", "databaseName"], "relationAttributes": []}'
+        '"relationAttributes": []}'
     )
 
 
 def test_adding_terms_results_in_must_bool():
     term_1 = Term(field="name", value="Bob")
     term_2 = Term(field="name", value="Dave")
     result = term_1 + term_2
```

### Comparing `pyatlan-0.3.0/tests/unit/test_typedef_model.py` & `pyatlan-0.4.0/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

