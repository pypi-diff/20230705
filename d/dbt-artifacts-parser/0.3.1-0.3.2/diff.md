# Comparing `tmp/dbt-artifacts-parser-0.3.1.tar.gz` & `tmp/dbt_artifacts_parser-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-artifacts-parser-0.3.1.tar", last modified: Thu May  4 02:37:27 2023, max compression
+gzip compressed data, was "dbt_artifacts_parser-0.3.2.tar", last modified: Wed Jul  5 08:18:28 2023, max compression
```

## Comparing `dbt-artifacts-parser-0.3.1.tar` & `dbt_artifacts_parser-0.3.2.tar`

### file list

```diff
@@ -1,90 +1,50 @@
--rw-r--r--   0        0        0      804 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1824 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2319 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1158 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1896 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.gitignore
--rw-r--r--   0        0        0     1371 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14055 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pylintrc
--rw-r--r--   0        0        0      150 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.pypirc
--rw-r--r--   0        0        0       32 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/.style.yapf
--rw-r--r--   0        0        0    11357 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/LICENSE
--rw-r--r--   0        0        0      159 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0      879 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/Makefile
--rw-r--r--   0        0        0     8681 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/README.md
--rw-r--r--   0        0        0      859 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/__init__.py
--rw-r--r--   0        0        0    11513 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parser.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/__init__.py
--rw-r--r--   0        0        0      977 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/base.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/__init__.py
--rw-r--r--   0        0        0     1887 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/__init__.py
--rw-r--r--   0        0        0    39709 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
--rw-r--r--   0        0        0    40546 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
--rw-r--r--   0        0        0    41294 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
--rw-r--r--   0        0        0    46633 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
--rw-r--r--   0        0        0    47751 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
--rw-r--r--   0        0        0    48519 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
--rw-r--r--   0        0        0    52861 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
--rw-r--r--   0        0        0    35031 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
--rw-r--r--   0        0        0    39455 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/__init__.py
--rw-r--r--   0        0        0     1719 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
--rw-r--r--   0        0        0     1755 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
--rw-r--r--   0        0        0     3346 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
--rw-r--r--   0        0        0     3458 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/__init__.py
--rw-r--r--   0        0        0     2044 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v1.py
--rw-r--r--   0        0        0     2327 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v2.py
--rw-r--r--   0        0        0     2441 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v3.py
--rw-r--r--   0        0        0     2348 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/utils.py
--rw-r--r--   0        0        0     4274 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/version_map.py
--rw-r--r--   0        0        0     5968 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json
--rw-r--r--   0        0        0   129577 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json
--rw-r--r--   0        0        0   135379 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json
--rw-r--r--   0        0        0   138301 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json
--rw-r--r--   0        0        0   157234 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json
--rw-r--r--   0        0        0   159202 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json
--rw-r--r--   0        0        0   163790 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json
--rw-r--r--   0        0        0   174833 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json
--rw-r--r--   0        0        0   115570 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json
--rw-r--r--   0        0        0   129190 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json
--rw-r--r--   0        0        0     4622 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json
--rw-r--r--   0        0        0     4777 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json
--rw-r--r--   0        0        0     9816 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json
--rw-r--r--   0        0        0    10271 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json
--rw-r--r--   0        0        0     5568 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v1.json
--rw-r--r--   0        0        0     6789 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v2.json
--rw-r--r--   0        0        0     7248 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v3.json
--rw-r--r--   0        0        0     1017 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/utils.py
--rwxr-xr-x   0        0        0     1121 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/clean.sh
--rwxr-xr-x   0        0        0     1021 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/format_python.sh
--rw-r--r--   0        0        0     3162 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/generate_parser_classes.sh
--rw-r--r--   0        0        0      978 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1391 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/dev/test_python.sh
--rw-r--r--   0        0        0     1545 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/setup.py
--rw-r--r--   0        0        0      792 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      796 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/parsers/__init__.py
--rw-r--r--   0        0        0     6001 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/parsers/test_utils.py
--rw-r--r--   0        0        0    11587 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/catalog.json
--rw-r--r--   0        0        0   226551 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/manifest.json
--rw-r--r--   0        0        0     4688 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v1/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   265840 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15168 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v2/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   289190 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    15738 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v3/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   269797 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/manifest.json
--rw-r--r--   0        0        0    14576 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v4/jaffle_shop/run_results.json
--rw-r--r--   0        0        0   817922 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v5/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   352436 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v6/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   412717 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v7/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   394308 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop/manifest.json
--rw-r--r--   0        0        0   401315 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v8/jaffle_shop_at_1_4_3/manifest.json
--rw-r--r--   0        0        0  1234064 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/resources/v9/jaffle_shop_at_1.5rc1/manifest.json
--rw-r--r--   0        0        0      938 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_basic.py
--rw-r--r--   0        0        0     6671 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_parser.py
--rw-r--r--   0        0        0     1090 2023-05-04 02:37:27.000000 dbt-artifacts-parser-0.3.1/tests/test_utils.py
--rw-r--r--   0        0        0    10459 1970-01-01 00:00:00.000000 dbt-artifacts-parser-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8998 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/README.md
+-rw-r--r--   0        0        0      859 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/__init__.py
+-rw-r--r--   0        0        0    11513 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parser.py
+-rw-r--r--   0        0        0      796 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/__init__.py
+-rw-r--r--   0        0        0      977 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/base.py
+-rw-r--r--   0        0        0      796 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/catalog/__init__.py
+-rw-r--r--   0        0        0     1887 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/catalog/catalog_v1.py
+-rw-r--r--   0        0        0      796 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/__init__.py
+-rw-r--r--   0        0        0    39709 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v1.py
+-rw-r--r--   0        0        0    40546 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v2.py
+-rw-r--r--   0        0        0    41294 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v3.py
+-rw-r--r--   0        0        0    46633 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v4.py
+-rw-r--r--   0        0        0    47752 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v5.py
+-rw-r--r--   0        0        0    48520 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v6.py
+-rw-r--r--   0        0        0    52862 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v7.py
+-rw-r--r--   0        0        0    35032 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v8.py
+-rw-r--r--   0        0        0    39343 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v9.py
+-rw-r--r--   0        0        0      796 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v1.py
+-rw-r--r--   0        0        0     1755 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v2.py
+-rw-r--r--   0        0        0     3346 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v3.py
+-rw-r--r--   0        0        0     3458 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v4.py
+-rw-r--r--   0        0        0      796 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/__init__.py
+-rw-r--r--   0        0        0     2044 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v1.py
+-rw-r--r--   0        0        0     2327 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v2.py
+-rw-r--r--   0        0        0     2441 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v3.py
+-rw-r--r--   0        0        0     2348 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/utils.py
+-rw-r--r--   0        0        0     4274 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/version_map.py
+-rw-r--r--   0        0        0     5968 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/catalog/catalog_v1.json
+-rw-r--r--   0        0        0   129577 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v1.json
+-rw-r--r--   0        0        0   135379 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v2.json
+-rw-r--r--   0        0        0   138302 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v3.json
+-rw-r--r--   0        0        0   157235 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v4.json
+-rw-r--r--   0        0        0   159203 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v5.json
+-rw-r--r--   0        0        0   163791 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v6.json
+-rw-r--r--   0        0        0   174833 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v7.json
+-rw-r--r--   0        0        0   115570 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v8.json
+-rw-r--r--   0        0        0   129190 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v9.json
+-rw-r--r--   0        0        0     4622 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v1.json
+-rw-r--r--   0        0        0     4777 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v2.json
+-rw-r--r--   0        0        0     9817 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v3.json
+-rw-r--r--   0        0        0    10272 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v4.json
+-rw-r--r--   0        0        0     5568 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v1.json
+-rw-r--r--   0        0        0     6790 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v2.json
+-rw-r--r--   0        0        0     7249 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v3.json
+-rw-r--r--   0        0        0     1017 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/utils.py
+-rw-r--r--   0        0        0     1773 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-07-05 08:18:28.000000 dbt_artifacts_parser-0.3.2/setup.py
+-rw-r--r--   0        0        0    10781 1970-01-01 00:00:00.000000 dbt_artifacts_parser-0.3.2/PKG-INFO
```

### Comparing `dbt-artifacts-parser-0.3.1/.github/CODEOWNERS` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+#
 #  Licensed to the Apache Software Foundation (ASF) under one or more
 #  contributor license agreements.  See the NOTICE file distributed with
 #  this work for additional information regarding copyright ownership.
 #  The ASF licenses this file to You under the Apache License, Version 2.0
 #  (the "License"); you may not use this file except in compliance with
 #  the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
-* @yu-iskw
+#
```

### Comparing `dbt-artifacts-parser-0.3.1/LICENSE` & `dbt_artifacts_parser-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/README.md` & `dbt_artifacts_parser-0.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 - [ManifestV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for manifest.json v2
 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for manifest.json v3
 - [ManifestV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for manifest.json v4
 - [ManifestV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5
 - [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6
 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for manifest.json v7
 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/manifest_v8.py) for manifest.json v8
+- [ManifestV9](dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9
 
 ### Run Results
 - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for run_results.json v2
 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
 - [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
 
@@ -128,14 +129,21 @@
 
 # parse manifest.json v8
 from dbt_artifacts_parser.parser import parse_manifest_v8
 
 with open("path/to/manifest.json", "r") as fp:
     manifest_dict = json.load(fp)
     manifest_obj = parse_manifest_v8(manifest=manifest_dict)
+
+# parse manifest.json v9
+from dbt_artifacts_parser.parser import parse_manifest_v9
+
+with open("path/to/manifest.json", "r") as fp:
+    manifest_dict = json.load(fp)
+    manifest_obj = parse_manifest_v9(manifest=manifest_dict)
 ```
 
 ### Parse run-results.json
 
 ```python
 import json
```

#### html2text {}

```diff
@@ -12,27 +12,28 @@
 manifest.json v2 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/
 manifest_v3.py) for manifest.json v3 - [ManifestV4](dbt_artifacts_parser/
 parsers/manifest/manifest_v4.py) for manifest.json v4 - [ManifestV5]
 (dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5 -
 [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for
 manifest.json v6 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/
 manifest_v7.py) for manifest.json v7 - [ManifestV8](dbt_artifacts_parser/
-parsers/manifest/manifest_v8.py) for manifest.json v8 ### Run Results -
-[RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for
-run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/
-manifest_v2.py) for run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/
-parsers/manifest/manifest_v3.py) for run_results.json v3 - [RunResultsV4]
-(dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
-### Sources - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py)
-for sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
-sources_v2.py) for sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/
-sources/sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json
-```python import json # parse any version of catalog.json from
-dbt_artifacts_parser.parser import parse_catalog with open("path/to/
-catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
+parsers/manifest/manifest_v8.py) for manifest.json v8 - [ManifestV9]
+(dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9 ###
+Run Results - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/
+manifest_v1.py) for run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/
+parsers/manifest/manifest_v2.py) for run_results.json v2 - [RunResultsV3]
+(dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
+- [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for
+run_results.json v4 ### Sources - [SourcesV1](dbt_artifacts_parser/parsers/
+sources/sources_v1.py) for sources.json v1 - [SourcesV2](dbt_artifacts_parser/
+parsers/sources/sources_v2.py) for sources.json v2 - [SourcesV3]
+(dbt_artifacts_parser/parsers/sources/sources_v3.py) for sources.json v3 ##
+Examples ### Parse catalog.json ```python import json # parse any version of
+catalog.json from dbt_artifacts_parser.parser import parse_catalog with open
+("path/to/catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog(catalog=catalog_dict) # parse catalog.json v1 from
 dbt_artifacts_parser.parser import parse_catalog_v1 with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog_v1(catalog=catalog_dict) ``` ### Parse manifest.json ```python
 import json # parse any version of manifest.json from
 dbt_artifacts_parser.parser import parse_manifest with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
@@ -56,15 +57,18 @@
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v6(manifest=manifest_dict) # parse manifest.json v7 from
 dbt_artifacts_parser.parser import parse_manifest_v7 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v7(manifest=manifest_dict) # parse manifest.json v8 from
 dbt_artifacts_parser.parser import parse_manifest_v8 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
-parse_manifest_v8(manifest=manifest_dict) ``` ### Parse run-results.json
+parse_manifest_v8(manifest=manifest_dict) # parse manifest.json v9 from
+dbt_artifacts_parser.parser import parse_manifest_v9 with open("path/to/
+manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
+parse_manifest_v9(manifest=manifest_dict) ``` ### Parse run-results.json
 ```python import json # parse any version of run-results.json from
 dbt_artifacts_parser.parser import parse_run_results with open("path/to/run-
 resultsjson", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
 parse_run_results(run_results=run_results_dict) # parse run-results.json v1
 from dbt_artifacts_parser.parser import parse_run_results_v1 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v1(run_results=run_results_dict) # parse
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/__init__.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 """
 A dbt artifacts parser in python
 """
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parser.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parser.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/__init__.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/base.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/__init__.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/catalog/catalog_v1.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/catalog/catalog_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/__init__.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v1.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v2.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v3.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v4.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v5.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v5.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 # pylint: disable=no-name-in-module
 from pydantic import Extra, Field, constr
+
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
     class Config:
         extra = Extra.forbid
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v6.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v6.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 # pylint: disable=no-name-in-module
 from pydantic import Extra, Field, constr
+
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
 
     class Config:
         extra = Extra.forbid
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v7.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v7.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import Extra, Field, constr
+
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
     class Config:
         extra = Extra.forbid
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v8.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v8.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from dbt_artifacts_parser.parsers.base import BaseParserModel
 from pydantic import Extra, Field, constr
 
+from dbt_artifacts_parser.parsers.base import BaseParserModel
+
 
 class ManifestMetadata(BaseParserModel):
     class Config:
         extra = Extra.forbid
 
     dbt_schema_version: Optional[
         str
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/manifest/manifest_v9.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/manifest/manifest_v9.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 # generated by datamodel-codegen:
 #   filename:  manifest_v9.json
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Union
+from typing import Any, Dict, List, Optional, Union
 
-from pydantic import constr
-from pydantic import Extra
-from pydantic import Field
+from pydantic import Extra, Field, constr
 
 from dbt_artifacts_parser.parsers.base import BaseParserModel
 
 
 class ManifestMetadata(BaseParserModel):
     class Config:
         extra = Extra.forbid
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/__init__.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v1.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v2.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v3.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/run_results/run_results_v4.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/run_results/run_results_v4.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/__init__.py` & `dbt_artifacts_parser-0.3.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-#
 #  Licensed to the Apache Software Foundation (ASF) under one or more
 #  contributor license agreements.  See the NOTICE file distributed with
 #  this work for additional information regarding copyright ownership.
 #  The ASF licenses this file to You under the Apache License, Version 2.0
 #  (the "License"); you may not use this file except in compliance with
 #  the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#
+from setuptools import setup
+
+setup()
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v1.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v1.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v2.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v2.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/sources/sources_v3.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/sources/sources_v3.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/utils.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/parsers/version_map.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/parsers/version_map.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/catalog/catalog_v1.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/catalog/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v1.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v2.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v3.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v3.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -8637,8 +8637,8 @@
 00021bc0: 2020 7d0a 2020 7d2c 0a20 2022 2473 6368    }.  },.  "$sch
 00021bd0: 656d 6122 3a20 2268 7474 703a 2f2f 6a73  ema": "http://js
 00021be0: 6f6e 2d73 6368 656d 612e 6f72 672f 6472  on-schema.org/dr
 00021bf0: 6166 742d 3037 2f73 6368 656d 6123 222c  aft-07/schema#",
 00021c00: 0a20 2022 2469 6422 3a20 2268 7474 7073  .  "$id": "https
 00021c10: 3a2f 2f73 6368 656d 6173 2e67 6574 6462  ://schemas.getdb
 00021c20: 742e 636f 6d2f 6462 742f 6d61 6e69 6665  t.com/dbt/manife
-00021c30: 7374 2f76 332e 6a73 6f6e 220a 7d         st/v3.json".}
+00021c30: 7374 2f76 332e 6a73 6f6e 220a 7d0a       st/v3.json".}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v4.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v4.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -9821,8 +9821,8 @@
 000265c0: 2224 7363 6865 6d61 223a 2022 6874 7470  "$schema": "http
 000265d0: 3a2f 2f6a 736f 6e2d 7363 6865 6d61 2e6f  ://json-schema.o
 000265e0: 7267 2f64 7261 6674 2d30 372f 7363 6865  rg/draft-07/sche
 000265f0: 6d61 2322 2c0a 2020 2224 6964 223a 2022  ma#",.  "$id": "
 00026600: 6874 7470 733a 2f2f 7363 6865 6d61 732e  https://schemas.
 00026610: 6765 7464 6274 2e63 6f6d 2f64 6274 2f6d  getdbt.com/dbt/m
 00026620: 616e 6966 6573 742f 7634 2e6a 736f 6e22  anifest/v4.json"
-00026630: 0a7d                                     .}
+00026630: 0a7d 0a                                  .}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v5.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v5.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -9944,8 +9944,8 @@
 00026d70: 2224 7363 6865 6d61 223a 2022 6874 7470  "$schema": "http
 00026d80: 3a2f 2f6a 736f 6e2d 7363 6865 6d61 2e6f  ://json-schema.o
 00026d90: 7267 2f64 7261 6674 2d30 372f 7363 6865  rg/draft-07/sche
 00026da0: 6d61 2322 2c0a 2020 2224 6964 223a 2022  ma#",.  "$id": "
 00026db0: 6874 7470 733a 2f2f 7363 6865 6d61 732e  https://schemas.
 00026dc0: 6765 7464 6274 2e63 6f6d 2f64 6274 2f6d  getdbt.com/dbt/m
 00026dd0: 616e 6966 6573 742f 7635 2e6a 736f 6e22  anifest/v5.json"
-00026de0: 0a7d                                     .}
+00026de0: 0a7d 0a                                  .}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v6.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v6.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -10230,8 +10230,8 @@
 00027f50: 2020 207d 0a20 207d 2c0a 2020 2224 7363     }.  },.  "$sc
 00027f60: 6865 6d61 223a 2022 6874 7470 3a2f 2f6a  hema": "http://j
 00027f70: 736f 6e2d 7363 6865 6d61 2e6f 7267 2f64  son-schema.org/d
 00027f80: 7261 6674 2d30 372f 7363 6865 6d61 2322  raft-07/schema#"
 00027f90: 2c0a 2020 2224 6964 223a 2022 6874 7470  ,.  "$id": "http
 00027fa0: 733a 2f2f 7363 6865 6d61 732e 6765 7464  s://schemas.getd
 00027fb0: 6274 2e63 6f6d 2f64 6274 2f6d 616e 6966  bt.com/dbt/manif
-00027fc0: 6573 742f 7636 2e6a 736f 6e22 0a7d       est/v6.json".}
+00027fc0: 6573 742f 7636 2e6a 736f 6e22 0a7d 0a    est/v6.json".}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v7.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v7.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v8.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v8.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/manifest/manifest_v9.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/manifest/manifest_v9.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v1.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v2.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v2.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v3.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v3.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -607,8 +607,8 @@
 000025e0: 0a20 2022 2473 6368 656d 6122 3a20 2268  .  "$schema": "h
 000025f0: 7474 703a 2f2f 6a73 6f6e 2d73 6368 656d  ttp://json-schem
 00002600: 612e 6f72 672f 6472 6166 742d 3037 2f73  a.org/draft-07/s
 00002610: 6368 656d 6123 222c 0a20 2022 2469 6422  chema#",.  "$id"
 00002620: 3a20 2268 7474 7073 3a2f 2f73 6368 656d  : "https://schem
 00002630: 6173 2e67 6574 6462 742e 636f 6d2f 6462  as.getdbt.com/db
 00002640: 742f 7275 6e2d 7265 7375 6c74 732f 7633  t/run-results/v3
-00002650: 2e6a 736f 6e22 0a7d                      .json".}
+00002650: 2e6a 736f 6e22 0a7d 0a                   .json".}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/run-results/run-results_v4.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/run-results/run-results_v4.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -635,8 +635,8 @@
 000027a0: 207d 0a20 207d 2c0a 2020 2224 7363 6865   }.  },.  "$sche
 000027b0: 6d61 223a 2022 6874 7470 3a2f 2f6a 736f  ma": "http://jso
 000027c0: 6e2d 7363 6865 6d61 2e6f 7267 2f64 7261  n-schema.org/dra
 000027d0: 6674 2d30 372f 7363 6865 6d61 2322 2c0a  ft-07/schema#",.
 000027e0: 2020 2224 6964 223a 2022 6874 7470 733a    "$id": "https:
 000027f0: 2f2f 7363 6865 6d61 732e 6765 7464 6274  //schemas.getdbt
 00002800: 2e63 6f6d 2f64 6274 2f72 756e 2d72 6573  .com/dbt/run-res
-00002810: 756c 7473 2f76 342e 6a73 6f6e 220a 7d    ults/v4.json".}
+00002810: 756c 7473 2f76 342e 6a73 6f6e 220a 7d0a  ults/v4.json".}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v1.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v1.json`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v2.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v2.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -418,8 +418,8 @@
 00001a10: 2c0a 2020 2224 7363 6865 6d61 223a 2022  ,.  "$schema": "
 00001a20: 6874 7470 3a2f 2f6a 736f 6e2d 7363 6865  http://json-sche
 00001a30: 6d61 2e6f 7267 2f64 7261 6674 2d30 372f  ma.org/draft-07/
 00001a40: 7363 6865 6d61 2322 2c0a 2020 2224 6964  schema#",.  "$id
 00001a50: 223a 2022 6874 7470 733a 2f2f 7363 6865  ": "https://sche
 00001a60: 6d61 732e 6765 7464 6274 2e63 6f6d 2f64  mas.getdbt.com/d
 00001a70: 6274 2f73 6f75 7263 6573 2f76 322e 6a73  bt/sources/v2.js
-00001a80: 6f6e 220a 7d                             on".}
+00001a80: 6f6e 220a 7d0a                           on".}.
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/resources/sources/sources_v3.json` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/resources/sources/sources_v3.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -447,7 +447,8 @@
 00001be0: 2473 6368 656d 6122 3a20 2268 7474 703a  $schema": "http:
 00001bf0: 2f2f 6a73 6f6e 2d73 6368 656d 612e 6f72  //json-schema.or
 00001c00: 672f 6472 6166 742d 3037 2f73 6368 656d  g/draft-07/schem
 00001c10: 6123 222c 0a20 2022 2469 6422 3a20 2268  a#",.  "$id": "h
 00001c20: 7474 7073 3a2f 2f73 6368 656d 6173 2e67  ttps://schemas.g
 00001c30: 6574 6462 742e 636f 6d2f 6462 742f 736f  etdbt.com/dbt/so
 00001c40: 7572 6365 732f 7633 2e6a 736f 6e22 0a7d  urces/v3.json".}
+00001c50: 0a                                       .
```

### Comparing `dbt-artifacts-parser-0.3.1/dbt_artifacts_parser/utils.py` & `dbt_artifacts_parser-0.3.2/dbt_artifacts_parser/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-artifacts-parser-0.3.1/pyproject.toml` & `dbt_artifacts_parser-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.module]
 name = "dbt_artifacts_parser"
 
+[tool.flit.sdist]
+exclude = [
+    ".github/",
+    ".gitignore",
+    ".pre-commit-config.yaml",
+    ".style.yapf",
+    ".pylintrc",
+    ".pypirc",
+    "Makefile",
+    "dev/",
+    "tests/",
+]
+
 [project]
 name = "dbt-artifacts-parser"
 authors = [{name = "yu-iskw"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7.0"
 classifiers = [
@@ -26,15 +39,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Typing :: Typed",
 ]
 dynamic = ["version", "description"]
 dependencies = [
-    "pydantic >=1.6",
+    "pydantic >=1.6,<2.0",
     "datamodel-code-generator >=0.12.0",
 ]
 
 [project.urls]
 Home = "https://github.com/yu-iskw/dbt-artifacts-parser"
 
 [project.optional-dependencies]
@@ -51,7 +64,10 @@
     "flit ==3.7.1",
     "build ==0.7.0",
     "yapf >=0.29.0",
     "pyyaml >=5.3",
     "pdoc3 >=0.9.2",
     "pre-commit >=2.15.0",
 ]
+
+[tool.isort]
+profile = "black"
```

### Comparing `dbt-artifacts-parser-0.3.1/PKG-INFO` & `dbt_artifacts_parser-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-artifacts-parser
-Version: 0.3.1
+Version: 0.3.2
 Summary: A dbt artifacts parser in python
 Author: yu-iskw
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Requires-Dist: pydantic >=1.6
+Requires-Dist: pydantic >=1.6,<2.0
 Requires-Dist: datamodel-code-generator >=0.12.0
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
 Requires-Dist: pre-commit >=2.15.0 ; extra == "dev"
@@ -69,14 +69,15 @@
 - [ManifestV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for manifest.json v2
 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for manifest.json v3
 - [ManifestV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for manifest.json v4
 - [ManifestV5](dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5
 - [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for manifest.json v6
 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/manifest_v7.py) for manifest.json v7
 - [ManifestV8](dbt_artifacts_parser/parsers/manifest/manifest_v8.py) for manifest.json v8
+- [ManifestV9](dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9
 
 ### Run Results
 - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for run_results.json v1
 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/manifest_v2.py) for run_results.json v2
 - [RunResultsV3](dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
 - [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
 
@@ -169,14 +170,21 @@
 
 # parse manifest.json v8
 from dbt_artifacts_parser.parser import parse_manifest_v8
 
 with open("path/to/manifest.json", "r") as fp:
     manifest_dict = json.load(fp)
     manifest_obj = parse_manifest_v8(manifest=manifest_dict)
+
+# parse manifest.json v9
+from dbt_artifacts_parser.parser import parse_manifest_v9
+
+with open("path/to/manifest.json", "r") as fp:
+    manifest_dict = json.load(fp)
+    manifest_obj = parse_manifest_v9(manifest=manifest_dict)
 ```
 
 ### Parse run-results.json
 
 ```python
 import json
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.3.1 Summary: A dbt
+Metadata-Version: 2.1 Name: dbt-artifacts-parser Version: 0.3.2 Summary: A dbt
 artifacts parser in python Author: yu-iskw Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Typing :: Typed Requires-Dist: pydantic >=1.6
+Python :: 3.10 Classifier: Typing :: Typed Requires-Dist: pydantic >=1.6,<2.0
 Requires-Dist: datamodel-code-generator >=0.12.0 Requires-Dist: flit ==3.7.1 ;
 extra == "dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist:
 yapf >=0.29.0 ; extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pre-commit
 >=2.15.0 ; extra == "dev" Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra ==
 "test" Requires-Dist: pylint >=2.12.0 ; extra == "test" Requires-Dist: mypy
 ==0.910 ; extra == "test" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra ==
@@ -35,27 +35,28 @@
 manifest.json v2 - [ManifestV3](dbt_artifacts_parser/parsers/manifest/
 manifest_v3.py) for manifest.json v3 - [ManifestV4](dbt_artifacts_parser/
 parsers/manifest/manifest_v4.py) for manifest.json v4 - [ManifestV5]
 (dbt_artifacts_parser/parsers/manifest/manifest_v5.py) for manifest.json v5 -
 [ManifestV6](dbt_artifacts_parser/parsers/manifest/manifest_v6.py) for
 manifest.json v6 - [ManifestV7](dbt_artifacts_parser/parsers/manifest/
 manifest_v7.py) for manifest.json v7 - [ManifestV8](dbt_artifacts_parser/
-parsers/manifest/manifest_v8.py) for manifest.json v8 ### Run Results -
-[RunResultsV1](dbt_artifacts_parser/parsers/manifest/manifest_v1.py) for
-run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/parsers/manifest/
-manifest_v2.py) for run_results.json v2 - [RunResultsV3](dbt_artifacts_parser/
-parsers/manifest/manifest_v3.py) for run_results.json v3 - [RunResultsV4]
-(dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for run_results.json v4
-### Sources - [SourcesV1](dbt_artifacts_parser/parsers/sources/sources_v1.py)
-for sources.json v1 - [SourcesV2](dbt_artifacts_parser/parsers/sources/
-sources_v2.py) for sources.json v2 - [SourcesV3](dbt_artifacts_parser/parsers/
-sources/sources_v3.py) for sources.json v3 ## Examples ### Parse catalog.json
-```python import json # parse any version of catalog.json from
-dbt_artifacts_parser.parser import parse_catalog with open("path/to/
-catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
+parsers/manifest/manifest_v8.py) for manifest.json v8 - [ManifestV9]
+(dbt_artifacts_parser/parsers/manifest/manifest_v9.py) for manifest.json v9 ###
+Run Results - [RunResultsV1](dbt_artifacts_parser/parsers/manifest/
+manifest_v1.py) for run_results.json v1 - [RunResultsV2](dbt_artifacts_parser/
+parsers/manifest/manifest_v2.py) for run_results.json v2 - [RunResultsV3]
+(dbt_artifacts_parser/parsers/manifest/manifest_v3.py) for run_results.json v3
+- [RunResultsV4](dbt_artifacts_parser/parsers/manifest/manifest_v4.py) for
+run_results.json v4 ### Sources - [SourcesV1](dbt_artifacts_parser/parsers/
+sources/sources_v1.py) for sources.json v1 - [SourcesV2](dbt_artifacts_parser/
+parsers/sources/sources_v2.py) for sources.json v2 - [SourcesV3]
+(dbt_artifacts_parser/parsers/sources/sources_v3.py) for sources.json v3 ##
+Examples ### Parse catalog.json ```python import json # parse any version of
+catalog.json from dbt_artifacts_parser.parser import parse_catalog with open
+("path/to/catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog(catalog=catalog_dict) # parse catalog.json v1 from
 dbt_artifacts_parser.parser import parse_catalog_v1 with open("path/to/
 catalog.json", "r") as fp: catalog_dict = json.load(fp) catalog_obj =
 parse_catalog_v1(catalog=catalog_dict) ``` ### Parse manifest.json ```python
 import json # parse any version of manifest.json from
 dbt_artifacts_parser.parser import parse_manifest with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
@@ -79,15 +80,18 @@
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v6(manifest=manifest_dict) # parse manifest.json v7 from
 dbt_artifacts_parser.parser import parse_manifest_v7 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
 parse_manifest_v7(manifest=manifest_dict) # parse manifest.json v8 from
 dbt_artifacts_parser.parser import parse_manifest_v8 with open("path/to/
 manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
-parse_manifest_v8(manifest=manifest_dict) ``` ### Parse run-results.json
+parse_manifest_v8(manifest=manifest_dict) # parse manifest.json v9 from
+dbt_artifacts_parser.parser import parse_manifest_v9 with open("path/to/
+manifest.json", "r") as fp: manifest_dict = json.load(fp) manifest_obj =
+parse_manifest_v9(manifest=manifest_dict) ``` ### Parse run-results.json
 ```python import json # parse any version of run-results.json from
 dbt_artifacts_parser.parser import parse_run_results with open("path/to/run-
 resultsjson", "r") as fp: run_results_dict = json.load(fp) run_results_obj =
 parse_run_results(run_results=run_results_dict) # parse run-results.json v1
 from dbt_artifacts_parser.parser import parse_run_results_v1 with open("path/
 to/run-results.json", "r") as fp: run_results_dict = json.load(fp)
 run_results_obj = parse_run_results_v1(run_results=run_results_dict) # parse
```

