# Comparing `tmp/foundry-dev-tools-1.1.tar.gz` & `tmp/foundry-dev-tools-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry-dev-tools-1.1.tar", last modified: Mon Jun 12 09:26:18 2023, max compression
+gzip compressed data, was "foundry-dev-tools-1.2.tar", last modified: Wed Jul  5 10:05:44 2023, max compression
```

## Comparing `foundry-dev-tools-1.1.tar` & `foundry-dev-tools-1.2.tar`

### file list

```diff
@@ -1,112 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.575722 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/blank_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.575722 foundry-dev-tools-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/Configuration_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/FoundryFileSystem_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/FoundryRestClient_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/SSO_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/docs/pictures/
--rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/pictures/tpa_config.png
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/docs/usage_and_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.579722 foundry-dev-tools-1.1/src/foundry_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cached_foundry_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    90644 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/foundry_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/fsspec_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/metadata_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/spark_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/foundry_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/foundry_dev_tools/utils/token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.583722 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 09:26:18.000000 foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.587722 foundry-dev-tools-1.1/src/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.587722 foundry-dev-tools-1.1/src/transforms/api/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/src/transforms/api/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.591722 foundry-dev-tools-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/foundry_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cached_foundry_client_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_cli_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.571722 foundry-dev-tools-1.1/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/tests/test_data/binary_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_data/binary_dataset/bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:26:18.595722 foundry-dev-tools-1.1/tests/test_data/iris/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_data/iris/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29547 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_local_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_spark_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_foundry_sql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33976 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_fsspec_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_multipass_tpa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_spark_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_transforms_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/test_utils_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-12 09:24:47.000000 foundry-dev-tools-1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.021835 foundry-dev-tools-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.021835 foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/blank_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.021835 foundry-dev-tools-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.025836 foundry-dev-tools-1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/Configuration_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/FoundryFileSystem_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/FoundryRestClient_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/SSO_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.025836 foundry-dev-tools-1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.025836 foundry-dev-tools-1.2/docs/pictures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-already-cached-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-already-cached-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-new-transaction-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-new-transaction-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/pictures/tpa_config.png
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/docs/usage_and_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.017835 foundry-dev-tools-1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/cached_foundry_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90358 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/foundry_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/fsspec_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/metadata_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/spark_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/converter/foundry_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/foundry_dev_tools/utils/token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-05 10:05:44.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 10:05:43.000000 foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.029836 foundry-dev-tools-1.2/src/transforms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/api/_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/api/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/api/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/src/transforms/api/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/tests/foundry_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/tests/test_cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-05 10:04:19.000000 foundry-dev-tools-1.2/tests/test_cached_foundry_client_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_cli_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_cli_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.017835 foundry-dev-tools-1.2/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/tests/test_data/binary_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_data/binary_dataset/bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:05:44.033836 foundry-dev-tools-1.2/tests/test_data/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_data/iris/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30233 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_foundry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_foundry_local_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_foundry_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_foundry_spark_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_foundry_sql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33976 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_fsspec_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_multipass_tpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_spark_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_transforms_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/test_utils_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-05 10:04:20.000000 foundry-dev-tools-1.2/tox.ini
```

### Comparing `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/blank_issue.yml` & `foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/blank_issue.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `foundry-dev-tools-1.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.github/pull_request_template.md` & `foundry-dev-tools-1.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.github/workflows/ci.yml` & `foundry-dev-tools-1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.github/workflows/docs.yml` & `foundry-dev-tools-1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.gitignore` & `foundry-dev-tools-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/.pre-commit-config.yaml` & `foundry-dev-tools-1.2/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: mixed-line-ending
     args: ['--fix=lf']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
-- repo: https://github.com/charliermarsh/ruff-pre-commit
+- repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.0.271'
+  rev: 'v0.0.276'
   hooks:
     - id: ruff
       args: ["--fix","--exit-non-zero-on-fix","--show-fixes"]
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
```

### Comparing `foundry-dev-tools-1.1/LICENSE` & `foundry-dev-tools-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/PKG-INFO` & `foundry-dev-tools-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.1
+Version: 1.2
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.1 Summary: Seamlessly
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.2 Summary: Seamlessly
 run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp
 renkamp@merckgroup.com>, Jonas Wunderlich
 wunderlich@merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
 emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
```

### Comparing `foundry-dev-tools-1.1/README.md` & `foundry-dev-tools-1.2/README.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/Configuration_usage.md` & `foundry-dev-tools-1.2/docs/Configuration_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/FoundryFileSystem_usage.md` & `foundry-dev-tools-1.2/docs/FoundryFileSystem_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/FoundryRestClient_usage.md` & `foundry-dev-tools-1.2/docs/FoundryRestClient_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/SSO_usage.md` & `foundry-dev-tools-1.2/docs/SSO_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/architecture.md` & `foundry-dev-tools-1.2/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/changelog.md` & `foundry-dev-tools-1.2/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
+## [1.2] - 2023-07-05
+
+### Added
+- `fdt info` command (#28)
+
+### Fixed
+- foundry dataset view support (#27)
+
 ## [1.1] - 2023-06-12
 
 ### Added
 
 - foundry-dev-tools build CLI (#22) (#23)
 
 ## [1.0.12] - 2023-06-01
@@ -133,14 +141,15 @@
 
 ## [1.0] - 2023-02-28 [YANKED]
 
 - First public Open Source Release of Foundry DevTools.
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/spec/v2.0.0.html
+[1.2]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.1...v1.2
 [1.1]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.12...v1.1
 [1.0.12]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.11...v1.0.12
 [1.0.11]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.10...v1.0.11
 [1.0.10]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.9...v1.0.10
 [1.0.9]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.8...v1.0.9
 [1.0.8]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.7...v1.0.8
 [1.0.7]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.6...v1.0.7
```

### Comparing `foundry-dev-tools-1.1/docs/conf.py` & `foundry-dev-tools-1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/develop.md` & `foundry-dev-tools-1.2/docs/develop.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/index.md` & `foundry-dev-tools-1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/installation.md` & `foundry-dev-tools-1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-dark.svg` & `foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-already-cached-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-already-cached-light.svg` & `foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-already-cached-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-dark.svg` & `foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-new-transaction-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/pictures/mermaid-diagram-new-transaction-light.svg` & `foundry-dev-tools-1.2/docs/pictures/mermaid-diagram-new-transaction-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/pictures/tpa_config.png` & `foundry-dev-tools-1.2/docs/pictures/tpa_config.png`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/docs/usage_and_examples.md` & `foundry-dev-tools-1.2/docs/usage_and_examples.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/pyproject.toml` & `foundry-dev-tools-1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   "pytest-mock",
   "pytest-spark",
   "requests-mock",
   "fsspec",
   "timeflake",
 ]
 transforms = ["pyspark>=3.0.0"]
-cli = ["click", "inquirer", "websockets", "rich"]
+cli = ["click", "inquirer", "websockets", "rich", "packaging"]
 
 [project.urls]
 Homepage = "https://emdgroup.github.io/foundry-dev-tools"
 Documentation = "https://emdgroup.github.io/foundry-dev-tools"
 Source = "https://github.com/emdgroup/foundry-dev-tools"
 Tracker = "https://github.com/emdgroup/foundry-dev-tools/issues"
 Changelog = "https://emdgroup.github.io/foundry-dev-tools/changelog.html"
```

### Comparing `foundry-dev-tools-1.1/setup.py` & `foundry-dev-tools-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/__init__.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/cached_foundry_client.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/cached_foundry_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 
 import foundry_dev_tools.config
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetHasNoSchemaError,
     DatasetNotFoundError,
     FoundryRestClient,
+    SQLReturnType,
 )
 from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
 from foundry_dev_tools.utils.converter.foundry_spark import (
     infer_dataset_format_from_foundry_schema,
 )
+from foundry_dev_tools.utils.misc import is_dataset_a_view
 
 LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     import pandas as pd
     import pyspark.sql
 
@@ -94,33 +96,39 @@
         Returns:
             `Tuple[str, dict]`:
                 local path to the dataset, dataset_identity
 
         """
         dataset_identity = self._get_dataset_identity(dataset_path_or_rid, branch)
 
+        return self._fetch_dataset(dataset_identity, branch=branch), dataset_identity
+
+    def _fetch_dataset(self, dataset_identity: dict, branch: str = "master") -> str:
+        last_transaction = dataset_identity["last_transaction"]
+
         if dataset_identity in list(self.cache.keys()):
-            return (
-                self._return_local_path_of_cached_dataset(dataset_identity, branch),
-                dataset_identity,
-            )
+            return self._return_local_path_of_cached_dataset(dataset_identity, branch)
         try:
             foundry_schema = self.api.get_dataset_schema(
                 dataset_identity["dataset_rid"],
-                dataset_identity["last_transaction_rid"],
+                dataset_identity["last_transaction"]["rid"],
                 branch=branch,
             )
         except DatasetHasNoSchemaError:
             # Binary datasets or no schema
             foundry_schema = None
-        return (
-            self._download_dataset_and_return_local_path(
-                dataset_identity, branch, foundry_schema
-            ),
-            dataset_identity,
+        if is_dataset_a_view(last_transaction["transaction"]):
+            self.cache[dataset_identity] = self.api.query_foundry_sql(
+                f'SELECT * FROM `{dataset_identity["dataset_rid"]}`',  # noqa: S608
+                branch=branch,
+                return_type=SQLReturnType.SPARK,
+            )
+            return self._return_local_path_of_cached_dataset(dataset_identity, branch)
+        return self._download_dataset_and_return_local_path(
+            dataset_identity, branch, foundry_schema
         )
 
     def _get_dataset_identity(self, dataset_path_or_rid, branch):
         if (
             "transforms_freeze_cache" not in self.config
             or self.config["transforms_freeze_cache"] is False
         ):
@@ -162,15 +170,15 @@
         )
 
         path = (
             os.sep.join(
                 [
                     self.cache.get_cache_dir(),
                     dataset_identity["dataset_rid"],
-                    dataset_identity["last_transaction_rid"],
+                    dataset_identity["last_transaction"]["rid"],
                 ]
             )
             + suffix
         )
         params["output_directory"] = path
         self.api.download_dataset_files(**params)
         self.cache.set_item_metadata(path, dataset_identity, foundry_schema)
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/cli/build.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/cli/build.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/config.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,26 +68,29 @@
     for key, value in config.items():
         return_config[key] = (
             TYPES[key](value) if value is not None and key in TYPES else None
         )
     return return_config
 
 
-def initial_config() -> "tuple[dict, pathlib.Path]":
+def initial_config(
+    project_dir: "Path|None" = None,
+) -> "tuple[dict, pathlib.Path, pathlib.Path|None]":
     """Parses the config file and applies defaults.
 
     The order of config values and how they are applied are:
     defaults < global config file < project specific config < env variables
     < overwrites by :py:class:`~foundry_dev_tools.config.Config`
 
     Returns:
-        a tuple (dict, pathlib.Path):
+        a tuple (dict, pathlib.Path, pathlib.Path|None):
             the first dict is the config as parsed
             with defaults applied and environment variables applied
             the second is a Path to the ~/.foundry-dev-tools directory
+            the third one is the Path to the project config file
     """
     foundry_dev_tools_directory = Path.home() / ".foundry-dev-tools"
 
     if not foundry_dev_tools_directory.exists():
         __foundry_local_directory = (
             Path.home() / ".foundry-local"
         )  # for backwards compatibility
@@ -125,16 +128,19 @@
     if foundry_dev_tools_config_file.exists():
         config_parser = ConfigParser()
         with foundry_dev_tools_config_file.open(encoding="UTF-8") as file:
             config_parser.read_file(file)
             if "default" in config_parser:
                 return_config.update(config_parser["default"])
 
-    caller_filename = inspect.stack()[-1].filename
-    project_config_file = find_project_config_file(Path(caller_filename).parent)
+    if not project_dir:
+        caller_filename = inspect.stack()[-1].filename
+        project_config_file = find_project_config_file(Path(caller_filename).parent)
+    else:
+        project_config_file = find_project_config_file(project_dir)
     if project_config_file:
         project_config_parser = ConfigParser()
         with project_config_file.open(encoding="UTF-8") as file:
             project_config_parser.read_file(file)
         if "default" in project_config_parser:
             LOGGER.debug(
                 "Using project based configuration file %s "
@@ -155,15 +161,15 @@
                 "The fallback to the old environment variables will be removed in the future!\n",
                 category=DeprecationWarning,
             )
             return_config[key] = os.getenv(f"FOUNDRY_LOCAL_{key.upper()}")
 
     config.update(return_config)
     return_config = type_convert(config)
-    return return_config, foundry_dev_tools_directory
+    return return_config, foundry_dev_tools_directory, project_config_file
 
 
 class Config(UserDict):
     """Config dict for the global static configs.
 
     Inherits from the static INITIAL_CONFIG.
     It can be used just like any other dict in python.
@@ -318,10 +324,11 @@
 
         return cnf
 
 
 (
     INITIAL_CONFIG,
     FOUNDRY_DEV_TOOLS_DIRECTORY,
+    FOUNDRY_DEV_TOOLS_PROJECT_CONFIG_FILE,
 ) = initial_config()
 Configuration = Config()
 __all__ = ["INITIAL_CONFIG", "FOUNDRY_DEV_TOOLS_DIRECTORY", "Configuration"]
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/foundry_api_client.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/foundry_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 from urllib.parse import quote, quote_plus
 
 import palantir_oauth_client
 import requests
 
 import foundry_dev_tools.config
 
-DEFAULT_REQUESTS_CONNECT_TIMEOUT = 10
-
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     import pandas as pd
     import pyarrow as pa
     import pyspark
 # On Python 3.8 on macOS, the default start method for new processes was
@@ -56,14 +54,22 @@
 # we will have a circular import
 # which may have unintended side effects
 try:
     FDT_VERSION = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
     FDT_VERSION = "unknown"
 
+DEFAULT_REQUESTS_CONNECT_TIMEOUT = 10
+DEFAULT_HEADERS = {
+    "User-Agent": requests.utils.default_user_agent(
+        f"foundry-dev-tools/{FDT_VERSION}/python-requests"
+    ),
+    "Content-Type": "application/json",
+}
+
 
 @contextmanager
 def _poolcontext(*args, **kwargs):
     pool = multiprocessing.Pool(*args, **kwargs)
     yield pool
     pool.terminate()
 
@@ -132,46 +138,50 @@
         self.metadata = f"{self._api_base}/foundry-metadata/api"
         self.data_proxy = f"{self._api_base}/foundry-data-proxy/api"
         self.schema_inference = f"{self._api_base}/foundry-schema-inference/api"
         self.multipass = f"{self._api_base}/multipass/api"
         self.foundry_sql_server_api = f"{self._api_base}/foundry-sql-server/api"
         self.jemma = f"{self._api_base}/jemma/api"
         self.builds2 = f"{self._api_base}/build2/api"
+        self.foundry_stats_api = f"{self._api_base}/foundry-stats/api"
         self._requests_verify_value = _determine_requests_verify_value(self._config)
+        self._requests_session = requests.Session()
+        self._requests_session.verify = self._requests_verify_value
 
     def _headers(self):
         return {
-            "User-Agent": requests.utils.default_user_agent(
-                f"foundry-dev-tools/{FDT_VERSION}/python-requests"
-            ),
-            "Content-Type": "application/json",
+            **DEFAULT_HEADERS,
             "Authorization": f"Bearer {_get_auth_token(self._config)}",
         }
 
-    def _verify(self):
-        return self._requests_verify_value
+    def _request(self, *args, read_timeout: "int|None" = None, **kwargs):
+        kwargs.setdefault("headers", self._headers())
+        kwargs["timeout"] = (
+            (DEFAULT_REQUESTS_CONNECT_TIMEOUT, read_timeout)
+            if read_timeout is None
+            else DEFAULT_REQUESTS_CONNECT_TIMEOUT
+        )
+        return self._requests_session.request(*args, **kwargs)
 
     def create_dataset(self, dataset_path: str) -> dict:
         """Creates an empty dataset in Foundry.
 
         Args:
             dataset_path (str): Path in Foundry, where this empty dataset should be created
                 for example: /Global/Foundry Operations/Foundry Support/iris_new
 
         Returns:
             dict:
                 with keys rid and fileSystemId.
                 The key rid contains the dataset_rid which is the unique identifier of a dataset.
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"path": dataset_path},
         )
         if (
             response.status_code == requests.codes.bad
             and "DuplicateDatasetName" in response.text
         ):
             rid = self.get_dataset_rid(dataset_path=dataset_path)
@@ -188,19 +198,17 @@
         Returns:
             dict:
                 with the keys rid and fileSystemId
 
         Raises:
             DatasetNotFoundError: if dataset does not exist
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.catalog}/catalog/datasets/{dataset_rid}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         if response.status_code == requests.codes.no_content and not response.text:
             raise DatasetNotFoundError(dataset_rid, response=response)
         _raise_for_status_verbose(response)
         return response.json()
 
     def delete_dataset(self, dataset_rid: str):
@@ -209,19 +217,17 @@
         Args:
             dataset_rid (str): Unique identifier of the dataset
 
         Raises:
             DatasetNotFoundError: if dataset does not exist
 
         """
-        response = _request(
+        response = self._request(
             "DELETE",
             f"{self.catalog}/catalog/datasets",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"rid": dataset_rid},
         )
         if (
             response.status_code == requests.codes.bad
             and "DatasetsNotFound" in response.text
         ):
             raise DatasetNotFoundError(dataset_rid, response=response)
@@ -231,19 +237,17 @@
     def move_resource_to_trash(self, resource_id: str):
         """Moves a Compass resource (e.g. dataset or folder) to trash.
 
         Args:
             resource_id (str): rid of the resource
 
         """
-        response_trash = _request(
+        response_trash = self._request(
             "POST",
             f"{self.compass}/batch/trash/add",
-            headers=self._headers(),
-            verify=self._verify(),
             data=f'["{resource_id}"]',
         )
         if response_trash.status_code != requests.codes.no_content:
             raise KeyError(
                 f"Issue while moving resource '{resource_id}' to foundry trash."
             )
         _raise_for_status_verbose(response_trash)
@@ -266,20 +270,18 @@
             parent_branch_id (str): The unique id of the parent branch, if empty creates new root branch
 
         Returns:
             dict:
                 the response as a json object
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"branchesUnrestricted2/{quote_plus(branch)}",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"parentBranchId": parent_branch, "parentRef": parent_branch_id},
         )
         if (
             response.status_code == requests.codes.bad
             and "BranchesAlreadyExist" in response.text
         ):
             raise BranchesAlreadyExistError(dataset_rid, branch, response=response)
@@ -306,20 +308,18 @@
             'rid': 'ri.foundry.main.branch...',
             'ancestorBranchIds': [],
             'creationTime': '',
             'transactionRid': 'ri.foundry.main.transaction....'
          }
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"branchesUpdate2/{quote_plus(branch)}",
-            headers=self._headers(),
-            verify=self._verify(),
             data=f'"{parent_branch}"',
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def get_branch(self, dataset_rid: str, branch: str) -> dict:
         """Returns branch information.
@@ -332,20 +332,18 @@
             dict:
                 with keys id (name) and rid (unique id) of the branch.
 
         Raises:
              BranchNotFoundError: if branch does not exist.
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"branches2/{quote_plus(branch)}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         if response.status_code == requests.codes.no_content and not response.text:
             raise BranchNotFoundError(dataset_rid, branch, response=None)
         _raise_for_status_verbose(response)
         return response.json()
 
     def open_transaction(
@@ -366,19 +364,17 @@
                 the transaction ID
 
         Raises:
             BranchNotFoundError: if branch does not exist
             DatasetNotFoundError: if dataset does not exist
             DatasetHasOpenTransactionError: if dataset has an open transaction
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/" f"transactions",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"branchId": f"{branch}", "record": {}},
         )
         if (
             response.status_code == requests.codes.bad
             and "BranchesNotFound" in response.text
         ):
             raise BranchNotFoundError(dataset_rid, branch, response=response)
@@ -399,20 +395,18 @@
             )
         _raise_for_status_verbose(response)
         # rid holds transaction id
         response_json = response.json()
         transaction_id = response_json["rid"]
         # update type of transaction, default is APPEND
         if mode in ("UPDATE", "SNAPSHOT", "DELETE"):
-            response_update = _request(
+            response_update = self._request(
                 "POST",
                 f"{self.catalog}/catalog/datasets/{dataset_rid}/"
                 f"transactions/{transaction_id}",
-                headers=self._headers(),
-                verify=self._verify(),
                 data=f'"{mode}"',
             )
             _raise_for_status_verbose(response_update)
         return transaction_id
 
     def remove_dataset_file(
         self,
@@ -435,20 +429,18 @@
         Args:
             dataset_rid (str): Unique identifier of the dataset
             transaction_id (str): transaction rid
             logical_path (str): logical path in the backing filesystem
             recursive (bool): recurse into subdirectories
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/files/remove",
-            headers=self._headers(),
-            verify=self._verify(),
             params={"logicalPath": logical_path, "recursive": recursive},
         )
         _raise_for_status_verbose(response)
 
     def add_files_to_delete_transaction(
         self, dataset_rid: str, transaction_id: str, logical_paths: "list[str]"
     ):
@@ -459,40 +451,36 @@
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             transaction_id (str): transaction rid
             logical_paths (List[str]): files in the dataset to delete
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/files/addToDeleteTransaction",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"logicalPaths": logical_paths},
         )
         _raise_for_status_verbose(response)
 
     def commit_transaction(self, dataset_rid: str, transaction_id: str):
         """Commits a transaction, should be called after file upload is complete.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             transaction_id (str): transaction id
 
         Raises:
             KeyError: when there was an issue with committing
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/commit",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"record": {}},
         )
         _raise_for_status_verbose(response)
         if response.status_code != requests.codes.no_content:
             raise KeyError(
                 f"{dataset_rid} issue while committing transaction {transaction_id}"
             )
@@ -504,20 +492,18 @@
             dataset_rid (str): Unique identifier of the dataset
             transaction_id (str): transaction id
 
         Raises:
             KeyError: When abort transaction fails
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.catalog}/catalog/datasets/{dataset_rid}/"
             f"transactions/{transaction_id}/abortWithMetadata",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"record": {}},
         )
         _raise_for_status_verbose(response)
         if response.status_code != requests.codes.no_content:
             raise KeyError(
                 f"{dataset_rid} issue while aborting transaction {transaction_id}"
             )
@@ -544,52 +530,69 @@
                 of transaction information.
 
         Raises:
             BranchNotFoundError: if branch not found
             DatasetHasNoTransactionsError: If the dataset has not transactions
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.catalog}/catalog/datasets/"
             f"{dataset_rid}/reverse-transactions2/{quote_plus(branch)}",
-            headers=self._headers(),
-            verify=self._verify(),
             params={
                 "pageSize": last,
                 "includeOpenExclusiveTransaction": include_open_exclusive_transaction,
             },
         )
         if response.status_code in (404, 400):
             raise BranchNotFoundError(dataset_rid, branch, response=response)
         _raise_for_status_verbose(response)
         as_json = response.json()
         if "values" in as_json and len(response.json()["values"]) > 0:
             return response.json()["values"]
         raise DatasetHasNoTransactionsError(dataset_rid, response=response)
 
-    def get_dataset_last_transaction_rid(
+    def get_dataset_last_transaction(
         self, dataset_rid: str, branch: str = "master"
-    ) -> "str | None":
+    ) -> "dict | None":
         """Returns the last transaction of a dataset / branch combination.
 
         Args:
             dataset_rid (str): Unique identifier of the dataset
             branch (str): Branch
 
         Returns:
-            str | None:
-                last_transaction_rid as string or None if dataset has no transaction.
+            dict | None:
+                response from transaction API or None if dataset has no transaction.
 
         """
         try:
-            return self.get_dataset_transactions(dataset_rid, branch)[0]["rid"]
+            return self.get_dataset_transactions(dataset_rid, branch)[0]
         except DatasetHasNoTransactionsError:
             return None
 
+    def get_dataset_last_transaction_rid(
+        self, dataset_rid: str, branch: str = "master"
+    ) -> "str | None":
+        """Returns the last transaction rid of a dataset / branch combination.
+
+        Args:
+            dataset_rid (str): Unique identifier of the dataset
+            branch (str): Branch
+
+        Returns:
+            str | None:
+                transaction rid or None if dataset has no transaction.
+
+        """
+        last_transaction = self.get_dataset_last_transaction(dataset_rid, branch)
+        if last_transaction:
+            return last_transaction["rid"]
+        return None
+
     def upload_dataset_file(
         self,
         dataset_rid: str,
         transaction_rid: str,
         path_or_buf: "str | Path | IO[AnyStr]",
         path_in_foundry_dataset: str,
     ):
@@ -607,15 +610,15 @@
         original_open = open
         builtins.open = (
             lambda f, *args, **kwargs: f
             if hasattr(f, "read")
             else original_open(f, *args, **kwargs)
         )
         with open(path_or_buf, "rb") as file:  # noqa: PTH123
-            response = _request(
+            response = self._request(
                 "POST",
                 f"{self.data_proxy}/dataproxy/datasets/{dataset_rid}/"
                 f"transactions/{transaction_rid}/putFile",
                 params={"logicalPath": path_in_foundry_dataset},
                 data=file,
                 headers={
                     "Content-Type": "application/octet-stream",
@@ -693,27 +696,23 @@
                 the json response of the api
 
         Raises:
             DatasetNotFoundError: if dataset not found
 
         """
         if "ri.foundry.main.dataset" in dataset_path_or_rid:
-            response = _request(
+            response = self._request(
                 "GET",
                 f"{self.compass}/resources/{dataset_path_or_rid}",
-                headers=self._headers(),
-                verify=self._verify(),
                 params={"decoration": "path"},
             )
         else:
-            response = _request(
+            response = self._request(
                 "GET",
                 f"{self.compass}/resources",
-                headers=self._headers(),
-                verify=self._verify(),
                 params={"path": dataset_path_or_rid, "decoration": "path"},
             )
         _raise_for_status_verbose(response)
         if response.status_code != requests.codes.ok:
             raise DatasetNotFoundError(dataset_path_or_rid, response=response)
         as_json = response.json()
         if as_json["directlyTrashed"]:
@@ -735,20 +734,18 @@
                 information about child objects
 
         Raises:
             FolderNotFoundError: if folder not found
         """
         query_params = {"pageToken": None, "limit": page_size}
         while True:
-            response = _request(
+            response = self._request(
                 "GET",
                 f"{self.compass}/folders/{folder_rid}/children",
-                headers=self._headers(),
                 params=query_params,
-                verify=self._verify(),
             )
             if response.status_code == requests.codes.not_found:
                 raise FolderNotFoundError(folder_rid, response=response)
             _raise_for_status_verbose(response)
             response_as_json = response.json()
             yield from response_as_json["values"]
             if response_as_json["nextPageToken"] is None:
@@ -765,19 +762,17 @@
                 e.g. ri.compass.main.folder.aca0cce9-2419-4978-bb18-d4bc6e50bd7e
 
         Returns:
             dict:
                 with keys rid and name and other properties.
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.compass}/folders",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"name": name, "parentId": parent_id},
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def get_dataset_rid(self, dataset_path: str) -> str:
         """Returns the rid of a dataset, uses dataset_path as input.
@@ -825,19 +820,17 @@
         batch_size = 100
         batches = [
             dataset_rids[i : i + batch_size]
             for i in range(0, len(dataset_rids), batch_size)
         ]
         result = {}
         for batch in batches:
-            response = _request(
+            response = self._request(
                 "POST",
                 f"{self.compass}/batch/paths",
-                headers=self._headers(),
-                verify=self._verify(),
                 json=batch,
             )
             _raise_for_status_verbose(response)
             result = {**result, **response.json()}
         return result
 
     def is_dataset_in_trash(self, dataset_path: str) -> bool:
@@ -873,21 +866,19 @@
         Raises:
             DatasetNotFoundError: if dataset was not found
             DatasetHasNoSchemaError: if dataset has no scheme
             BranchNotFoundError: if branch was not found
             KeyError: if the combination of dataset_rid, transaction_rid and branch was not found
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.metadata}/schemas/datasets/"
             f"{dataset_rid}/branches/{quote_plus(branch)}",
             params={"endTransactionRid": transaction_rid},
-            headers=self._headers(),
-            verify=self._verify(),
         )
         if response.status_code == requests.codes.forbidden:
             raise DatasetNotFoundError(dataset_rid, response=response)
         if response.status_code == requests.codes.no_content:
             # here we don't know if schema does not exist or branch does not exist
             # we ask api for branch information, if branch does not exist, exception is thrown
             self.get_branch(dataset_rid, branch)
@@ -915,22 +906,20 @@
         Args:
             dataset_rid (str): The rid of the dataset
             transaction_rid (str): The rid of the transaction
             schema (dict): The foundry schema
             branch (str): The branch
 
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.metadata}/schemas/datasets/"
             f"{dataset_rid}/branches/{quote_plus(branch)}",
             params={"endTransactionRid": transaction_rid},
             json=schema,
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
 
     def infer_dataset_schema(self, dataset_rid: str, branch: str = "master") -> dict:
         """Calls the foundry-schema-inference service to infer the dataset schema.
 
         Returns dict with foundry schema, if status == SUCCESS
@@ -942,21 +931,19 @@
         Returns:
             dict:
                 with dataset schema, that can be used to call upload_dataset_schema
 
         Raises:
             ValueError: if foundry schema inference failed
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.schema_inference}/datasets/"
             f"{dataset_rid}/branches/{quote_plus(branch)}/schema",
             json={},
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         parsed_response = response.json()
         if parsed_response["status"] == "SUCCESS":
             return parsed_response["data"]["foundrySchema"]
         if parsed_response["status"] == "WARN":
             warnings.warn(
@@ -971,45 +958,47 @@
             f"'{parsed_response['status']}' "
             f"and message '{parsed_response['message']}'."
         )
 
     def get_dataset_identity(
         self, dataset_path_or_rid: str, branch="master", check_read_access=True
     ) -> dict:
-        """Returns the current identity of this dataset (dataset_path, dataset_rid, last_transaction_rid).
+        """Returns the identity of this dataset (dataset_path, dataset_rid, last_transaction_rid, last_transaction).
 
         Args:
             dataset_path_or_rid (str): Path to dataset (e.g. /Global/...)
                 or rid of dataset (e.g. ri.foundry.main.dataset...)
             branch (str): branch of the dataset
             check_read_access (bool): default is True, checks if the user has read access ('gatekeeper:view-resource')
                 to the dataset otherwise exception is thrown
 
         Returns:
             dict:
-                with the keys 'dataset_path', 'dataset_rid' and 'last_transaction_rid'
+                with the keys 'dataset_path', 'dataset_rid', 'last_transaction_rid', 'last_transaction'
 
         Raises:
             DatasetNoReadAccessError: if you have no read access for that dataset
 
         """
         dataset_details = self.get_dataset_details(dataset_path_or_rid)
         dataset_rid = dataset_details["rid"]
         dataset_path = dataset_details["path"]
         if (
             check_read_access
             and "gatekeeper:view-resource" not in dataset_details["operations"]
         ):
             raise DatasetNoReadAccessError(dataset_rid)
+        last_transaction = self.get_dataset_last_transaction(dataset_rid, branch)
         return {
             "dataset_path": dataset_path,
             "dataset_rid": dataset_rid,
-            "last_transaction_rid": self.get_dataset_last_transaction_rid(
-                dataset_rid, branch
-            ),
+            "last_transaction_rid": last_transaction["rid"]
+            if last_transaction
+            else None,
+            "last_transaction": last_transaction,
         }
 
     def list_dataset_files(
         self,
         dataset_rid: str,
         exclude_hidden_files: bool = True,
         view: str = "master",
@@ -1038,20 +1027,18 @@
                 filenames
 
         Raises:
             DatasetNotFound: if dataset was not found
         """
 
         def _inner_get(next_page_token=None):
-            response = _request(
+            response = self._request(
                 "GET",
                 f"{self.catalog}/catalog/datasets/"
                 f"{dataset_rid}/views2/{quote_plus(view)}/files",
-                headers=self._headers(),
-                verify=self._verify(),
                 params={
                     "pageSize": 10000000,
                     "includeOpenExclusiveTransaction": include_open_exclusive_transaction,
                     "logicalPath": logical_path,
                     "excludeHiddenFiles": exclude_hidden_files,
                     "pageStartLogicalPath": next_page_token,
                 },
@@ -1079,21 +1066,64 @@
             view (str): branch or transaction rid of the dataset
 
         Returns:
             dict:
                 sizeInBytes, numFiles, hiddenFilesSizeInBytes, numHiddenFiles, numTransactions
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.catalog}/catalog/datasets/"
             f"{dataset_rid}/views/{quote_plus(view)}"
             f"/stats",
-            headers=self._headers(),
-            verify=self._verify(),
+        )
+        _raise_for_status_verbose(response)
+        return response.json()
+
+    def foundry_stats(
+        self, dataset_rid: str, end_transaction_rid: str, branch: str = "master"
+    ) -> dict:
+        """Returns row counts and size of the dataset/view.
+
+        Args:
+            dataset_rid (str): The dataset RID.
+            end_transaction_rid (str): The specific transaction RID,
+                which will be used to return the statistics.
+            branch (str): The branch to query
+
+        Returns:
+            dict:
+                With the following structure:
+                {
+                datasetRid:str,
+                branch:str,
+                endTransactionRid:str,
+                schemaId:str,
+                computedDatasetStats:{
+                    rowCount:str|None,
+                    sizeInBytes:str,
+                    columnStats:{
+                        "...":{
+                            nullCount:str|None,
+                            uniqueCount:str|None,
+                            avgLength:str|None,
+                            maxLength:str|None
+                            }
+                        }
+                    }
+                }
+        """
+        response = self._request(
+            "POST",
+            f"{self.foundry_stats_api}/computed-stats-v2/get-v2",
+            json={
+                "datasetRid": dataset_rid,
+                "branch": branch,
+                "endTransactionRid": end_transaction_rid,
+            },
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def download_dataset_file(
         self,
         dataset_rid: str,
@@ -1141,19 +1171,18 @@
             resp.raw.decode_content = True
             shutil.copyfileobj(resp.raw, out_file)
 
         resp.close()
         return os.fspath(local_path)
 
     def _download_dataset_file(self, dataset_rid, view, foundry_file_path, stream=True):
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.data_proxy}/dataproxy/datasets/"
             f"{dataset_rid}/views/{quote_plus(view)}/{quote(foundry_file_path)}",
-            headers=self._headers(),
             stream=stream,
         )
         _raise_for_status_verbose(response)
         return response
 
     def download_dataset_files(
         self,
@@ -1205,15 +1234,15 @@
                             repeat(dataset_rid),
                             repeat(output_directory),
                             files,
                             repeat(view),
                         ),
                     )
                 )
-        return list(filter(lambda p: p != "", local_paths))  # noqa: PLC1901
+        return list(filter(lambda p: p != "", local_paths))
 
     @contextmanager
     def download_dataset_files_temporary(
         self,
         dataset_rid: str,
         files: "list | None" = None,
         view: str = "master",
@@ -1272,20 +1301,18 @@
         Returns:
             :external+requests:py:class:`~requests.Response`:
                 with the csv stream.
                 Can be converted to a pandas DataFrame
                 >>> pd.read_csv(io.BytesIO(response.content))
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.data_proxy}/dataproxy/datasets/"
             f"{dataset_rid}/branches/{quote_plus(branch)}/csv",
-            headers=self._headers(),
-            verify=self._verify(),
             params={"includeColumnNames": True, "includeBom": True},
             stream=True,
         )
 
         _raise_for_status_verbose(response)
         return response
 
@@ -1327,19 +1354,17 @@
         """
         # if return_type is a str this will also work, this will get fixed in python 3.12
         # where we would be able to use `return_type not in SQLReturnType`
         if return_type not in SQLReturnType:
             raise ValueError(
                 f"return_type ({return_type}) should be a member of foundry_dev_tools.foundry_api_client.SQLReturnType"
             )
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.data_proxy}/dataproxy/queryWithFallbacks",
-            headers=self._headers(),
-            verify=self._verify(),
             params={"fallbackBranchIds": [branch]},
             json={"query": query},
             read_timeout=timeout,
         )
 
         if (
             response.status_code == requests.codes.not_found
@@ -1474,19 +1499,17 @@
                 'multipass:family-name': ['<family-name>'],
                 'multipass:upn': ['<upn>'],
                 'multipass:realm': ['<your-company>'],
                 'multipass:realm-name': ['<your-org>']}
            }
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.multipass}/me",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def get_group(self, group_id: str) -> dict:
         """Returns the multipass group information.
 
@@ -1503,34 +1526,30 @@
                 'multipass:realm': ['palantir-internal-realm'],
                 'multipass:organization': ['<your-org>'],
                 'multipass:organization-rid': ['ri.multipass..organization.<...>'],
                 'multipass:realm-name': ['Palantir Internal']
             }
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.multipass}/groups/{group_id}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def delete_group(self, group_id: str):
         """Deletes multipass group.
 
         Args:
             group_id (str): the group id to delete
         """
-        response = _request(
+        response = self._request(
             "DELETE",
             f"{self.multipass}/administration/groups/{group_id}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
 
     def create_third_party_application(
         self,
         client_type: str,
         display_name: str,
@@ -1591,19 +1610,17 @@
             ]:
                 raise AssertionError(
                     f"grant ({grant}) needs to be one of "
                     "AUTHORIZATION_CODE, REFRESH_TOKEN or CLIENT_CREDENTIALS"
                 )
         if allowed_organization_rids is None:
             allowed_organization_rids = []
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.multipass}/clients",
-            headers=self._headers(),
-            verify=self._verify(),
             json={
                 "allowedOrganizationRids": allowed_organization_rids,
                 "clientType": client_type,
                 "displayName": display_name,
                 "description": description,
                 "grantTypes": grant_types,
                 "redirectUris": redirect_uris,
@@ -1616,19 +1633,17 @@
 
     def delete_third_party_application(self, client_id: str):
         """Deletes a Third Party Application.
 
         Args:
             client_id (str): The unique identifier of the TPA.
         """
-        response = _request(
+        response = self._request(
             "DELETE",
             f"{self.multipass}/clients/{client_id}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
 
     def update_third_party_application(
         self,
         client_id: str,
         client_type: str,
@@ -1690,19 +1705,17 @@
             ]:
                 raise AssertionError(
                     f"grant ({grant}) needs to be one of "
                     "AUTHORIZATION_CODE, REFRESH_TOKEN or CLIENT_CREDENTIALS"
                 )
         if allowed_organization_rids is None:
             allowed_organization_rids = []
-        response = _request(
+        response = self._request(
             "PUT",
             f"{self.multipass}/clients/{client_id}",
-            headers=self._headers(),
-            verify=self._verify(),
             json={
                 "allowedOrganizationRids": allowed_organization_rids,
                 "clientType": client_type,
                 "displayName": display_name,
                 "description": description,
                 "grantTypes": grant_types,
                 "redirectUris": redirect_uris,
@@ -1738,19 +1751,17 @@
                 "logoUri":null,
                 "grantTypes":[<"AUTHORIZATION_CODE","REFRESH_TOKEN","CLIENT_CREDENTIALS">],
                 "redirectUris":[],
                 "allowedOrganizationRids":[]
             }
 
         """
-        response = _request(
+        response = self._request(
             "PUT",
             f"{self.multipass}/clients/{client_id}/rotateSecret",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def enable_third_party_application(
         self, client_id: str, operations: "list | None", resources: "list | None"
     ) -> dict:
@@ -1781,19 +1792,17 @@
             }
 
         """
         if operations is None:
             operations = []
         if resources is None:
             resources = []
-        response = _request(
+        response = self._request(
             "PUT",
             f"{self.multipass}/client-installations/{client_id}",
-            headers=self._headers(),
-            verify=self._verify(),
             json={"operations": operations, "resources": resources},
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def start_checks_and_build(
         self,
@@ -1809,19 +1818,17 @@
             ref_name (str): the git ref_name for the branch
             commit_hash (str): the git commit hash
             file_paths (List[str]): a list of python transform files
 
         Returns:
             dict: the JSON API response
         """
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.jemma}/builds",
-            headers=self._headers(),
-            verify=self._verify(),
             json={
                 "jobs": [
                     {
                         "name": "Checks",
                         "type": "exec",
                         "parameters": {
                             "repositoryTarget": {
@@ -1855,48 +1862,42 @@
 
         Args:
             build_rid (str): the build RID
 
         Returns:
             dict: the JSON API response
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.builds2}/info/builds2/{build_rid}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def get_job_report(self, job_rid: str) -> dict:
         """Get the report for a job.
 
         Args:
             job_rid (str): the job RID
 
         Returns:
             dict: the job report response
 
         """
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.builds2}/info/jobs3/{job_rid}",
-            headers=self._headers(),
-            verify=self._verify(),
         )
         _raise_for_status_verbose(response)
         return response.json()
 
     def _execute_fsql_query(self, query: str, branch="master", timeout=600) -> dict:
-        response = _request(
+        response = self._request(
             "POST",
             f"{self.foundry_sql_server_api}/queries/execute",
-            headers=self._headers(),
-            verify=self._requests_verify_value,
             json={
                 "dialect": "SPARK",
                 "fallbackBranchIds": [branch],
                 "parameters": {
                     "type": "unnamedParameterValues",
                     "unnamedParameterValues": [],
                 },
@@ -1910,19 +1911,17 @@
         return response.json()
 
     def _poll_fsql_query_status(self, initial_response_json: dict, timeout=600):
         start_time = time.time()
         query_id = initial_response_json["queryId"]
         response_json = initial_response_json
         while response_json["status"]["type"] == "running":
-            response = _request(
+            response = self._request(
                 "GET",
                 f"{self.foundry_sql_server_api}/queries/{query_id}/status",
-                headers=self._headers(),
-                verify=self._requests_verify_value,
                 json={},
             )
             _raise_for_status_verbose(response)
             response_json = response.json()
             if response_json["status"]["type"] == "failed":
                 raise FoundrySqlQueryFailedError(response=response)
             if time.time() > start_time + timeout:
@@ -1944,15 +1943,15 @@
         # Download time seems to be a lot faster (2x) with gzip encoding turned on, while
         # memory consumption increases by the amount of raw bytes returned from the sql server.
         # I will optimize for faster downloads, for now. This decision can be revisited later.
         #
         # 01/2022: Moving to 'requests' instead of 'urllib3', did some experiments again
         # and noticed that preloading content is significantly faster than stream=True
 
-        response = _request(
+        response = self._request(
             "GET",
             f"{self.foundry_sql_server_api}/queries/{query_id}/results",
             headers=headers,
         )
         bytes_io = io.BytesIO(response.content)
         arrow_format = bytes_io.read(1).decode("UTF-8")
         if arrow_format != "A":
@@ -2177,20 +2176,21 @@
         "Authorization": "Basic "
         + base64.b64encode(bytes(client_id + ":" + client_secret, "ISO-8859-1")).decode(
             "ascii"
         ),
         "Content-Type": "application/x-www-form-urlencoded",
     }
 
-    response = _request(
+    response = requests.request(
         "POST",
         f"{foundry_url}/multipass/api/oauth2/token",
         data={"grant_type": "client_credentials", "scope": scopes},
         headers=headers,
         verify=requests_verify_value,
+        timeout=DEFAULT_REQUESTS_CONNECT_TIMEOUT,
     )
     _raise_for_status_verbose(response)
     return response.json()
 
 
 @lru_with_ttl(ttl_seconds=3600)
 def _get_palantir_oauth_token(
@@ -2210,26 +2210,14 @@
         client_secret=client_secret,
         use_local_webserver=False,
     )
 
     return credentials.token
 
 
-def _request(*args, **kwargs):
-    if "read_timeout" in kwargs:
-        read_timeout = kwargs["read_timeout"]
-        del kwargs["read_timeout"]
-        return requests.request(
-            *args,
-            **kwargs,
-            timeout=(DEFAULT_REQUESTS_CONNECT_TIMEOUT, read_timeout),
-        )
-    return requests.request(*args, **kwargs, timeout=DEFAULT_REQUESTS_CONNECT_TIMEOUT)
-
-
 class FoundryDevToolsError(Exception):
     """Metaclass for :class:`FoundryAPIError` and :class:`foundry_dev_tools.fsspec_impl.FoundryFileSystemError`.
 
     Catch all foundry_dev_tools errors:
 
     >>> try:
     >>>     fun() # raise DatasetNotFoundError or any other
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/fsspec_impl.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/metadata_store.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/metadata_store.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/caches/spark_caches.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/caches/spark_caches.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 
 pyspark = import_optional_dependency("pyspark")
 
 
 class DiskPersistenceBackedSparkCache(MutableMapping):
     """A cache that stores spark dataframes inside a directory."""
 
-    FORMATS = ["parquet", "csv", "unknown"]
-    DEFAULT_FORMAT = "parquet"
-    STORE_LAST_N_TRANSACTIONS = 2
+    _DEFAULT_FORMAT = "parquet"
+    _STORE_LAST_N_TRANSACTIONS = 2
 
     def __init__(self, cache_dir: str, clear_cache: bool = False, **kwargs):
         self._cache_dir = cache_dir
         if clear_cache:
             shutil.rmtree(self._cache_dir, ignore_errors=True)
         Path(self._cache_dir).mkdir(parents=True, exist_ok=True)
         self.metadata_store = DatasetMetadataStore(self._cache_dir)
 
     def __setitem__(self, key: dict, value: "pyspark.sql.dataframe.DataFrame") -> None:
         _validate_cache_key(key)
-        path = self._get_storage_location(key, self.DEFAULT_FORMAT)
-        value.write.format(self.DEFAULT_FORMAT).save(path=path, mode="overwrite")
+        path = self._get_storage_location(key, self._DEFAULT_FORMAT)
+        value.write.format(self._DEFAULT_FORMAT).save(path=path, mode="overwrite")
         self.set_item_metadata(path, key, value.schema.jsonValue())
 
     def set_item_metadata(self, path: str, dataset_identity: dict, schema: dict):
         """Writes schema and metadata.json entry.
 
         Use when files are added to cache without calling cache[entry] = df
 
@@ -208,15 +207,15 @@
             raise RuntimeError(
                 "Cache dir not in sync with db.\n"
                 f"Please delete the cache dir ({self.get_cache_dir()})"
                 "and restart the transform."
             )
 
         transaction_to_delete = all_transactions_sorted[
-            self.STORE_LAST_N_TRANSACTIONS :
+            self._STORE_LAST_N_TRANSACTIONS :
         ]
         for transaction in transaction_to_delete:
             directory_path = os.fspath(
                 Path(self.get_cache_dir())
                 / dataset_identity["dataset_rid"]
                 / transaction
             )
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/converter/foundry_spark.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/converter/foundry_spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/importer.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/importer.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/misc.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,7 +51,23 @@
 
     It uses the amount of terminal columns to print a line of good length
     Args:
         c (str): the char to print
         print_handler (Callable[[str],Any]): the function to use for printing
     """
     print_handler(c * os.get_terminal_size().columns)
+
+
+def is_dataset_a_view(dataset_transaction: dict):
+    """Determines based on a transaction, if a dataset is a view.
+
+    Args:
+        dataset_transaction (dict): a transaction on the dataset in question
+
+    Returns:
+        bool: if dataset is a view
+    """
+    return (
+        "record" in dataset_transaction
+        and "view" in dataset_transaction["record"]
+        and dataset_transaction["record"]["view"] is True
+    )
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/repo.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/repo.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/spark.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools/utils/token_provider.py` & `foundry-dev-tools-1.2/src/foundry_dev_tools/utils/token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/PKG-INFO` & `foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.1
+Version: 1.2
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp <nicolas.renkamp@merckgroup.com>, Jonas Wunderlich <jonas.wunderlich@merckgroup.com>
 License: Apache-2.0
 Project-URL: Homepage, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
 Project-URL: Tracker, https://github.com/emdgroup/foundry-dev-tools/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.1 Summary: Seamlessly
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.2 Summary: Seamlessly
 run your Palantir Foundry Repository transforms code on your local machine.
 Author-email: Nicolas Renkamp
 renkamp@merckgroup.com>, Jonas Wunderlich
 wunderlich@merckgroup.com> License: Apache-2.0 Project-URL: Homepage, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Documentation, https://
 emdgroup.github.io/foundry-dev-tools Project-URL: Source, https://github.com/
 emdgroup/foundry-dev-tools Project-URL: Tracker, https://github.com/emdgroup/
```

### Comparing `foundry-dev-tools-1.1/src/foundry_dev_tools.egg-info/SOURCES.txt` & `foundry-dev-tools-1.2/src/foundry_dev_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 src/foundry_dev_tools.egg-info/dependency_links.txt
 src/foundry_dev_tools.egg-info/entry_points.txt
 src/foundry_dev_tools.egg-info/not-zip-safe
 src/foundry_dev_tools.egg-info/requires.txt
 src/foundry_dev_tools.egg-info/top_level.txt
 src/foundry_dev_tools/cli/__init__.py
 src/foundry_dev_tools/cli/build.py
+src/foundry_dev_tools/cli/info.py
 src/foundry_dev_tools/cli/main.py
 src/foundry_dev_tools/utils/__init__.py
 src/foundry_dev_tools/utils/importer.py
 src/foundry_dev_tools/utils/misc.py
 src/foundry_dev_tools/utils/repo.py
 src/foundry_dev_tools/utils/spark.py
 src/foundry_dev_tools/utils/token_provider.py
@@ -67,24 +68,26 @@
 src/transforms/api/_transform.py
 tests/__init__.py
 tests/conftest.py
 tests/foundry_mock_client.py
 tests/test_cached_foundry_client.py
 tests/test_cached_foundry_client_integration.py
 tests/test_cli_build.py
+tests/test_cli_info.py
 tests/test_config.py
 tests/test_foundry_api.py
 tests/test_foundry_local_deprecation.py
 tests/test_foundry_mock.py
 tests/test_foundry_spark_converters.py
 tests/test_foundry_sql_client.py
 tests/test_fsspec_impl.py
 tests/test_importer.py
 tests/test_multipass_tpa.py
 tests/test_spark_caches.py
 tests/test_token_provider.py
 tests/test_transforms.py
 tests/test_transforms_integration.py
+tests/test_utils_misc.py
 tests/test_utils_repo.py
 tests/utils.py
 tests/test_data/binary_dataset/bin
 tests/test_data/iris/iris.csv
```

### Comparing `foundry-dev-tools-1.1/src/transforms/api/__init__.py` & `foundry-dev-tools-1.2/src/transforms/api/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/transforms/api/_configure.py` & `foundry-dev-tools-1.2/src/transforms/api/_configure.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/transforms/api/_dataset.py` & `foundry-dev-tools-1.2/src/transforms/api/_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 import foundry_dev_tools.config
 from foundry_dev_tools.cached_foundry_client import CachedFoundryClient
 from foundry_dev_tools.foundry_api_client import (
     BranchNotFoundError,
     DatasetHasNoSchemaError,
     DatasetHasNoTransactionsError,
+    SQLReturnType,
 )
 from foundry_dev_tools.utils.caches.spark_caches import DiskPersistenceBackedSparkCache
+from foundry_dev_tools.utils.misc import is_dataset_a_view
 from foundry_dev_tools.utils.repo import git_toplevel_dir
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _as_list(list_or_single_item: "list[Any] | Any | None") -> "list[Any]":
     """Helper function turning single values or None into lists.
@@ -128,15 +130,15 @@
             "Dataset rid: %s, path: %s on branch %s has no schema, "
             "falling back to file download. "
             "Only filesystem() is supported with this dataset.",
             dataset_identity["dataset_rid"],
             dataset_identity["dataset_path"],
             branch,
         )
-        self._cached_client.fetch_dataset(dataset_identity["dataset_rid"], branch)
+        self._cached_client._fetch_dataset(dataset_identity, branch)
         return None, dataset_identity, branch
 
     def _offline(
         self, alias: str, branch: str
     ) -> "tuple[pyspark.sql.DataFrame | None, dict, str]":
         dataset_identity = self._cache.get_dataset_identity_not_branch_aware(alias)
         if self._cache.dataset_has_schema(dataset_identity):
@@ -179,25 +181,31 @@
             and self.config["transforms_sql_sample_row_limit"] is not None
         ):
             query = query + f" LIMIT {self.config['transforms_sql_sample_row_limit']}"
         LOGGER.debug(
             "Executing Foundry/SparkSQL Query: %s \n on branch %s", query, branch
         )
         return self._cached_client.api.query_foundry_sql(
-            query, branch=branch, return_type="spark"
+            query, branch=branch, return_type=SQLReturnType.SPARK
         )
 
     def _retrieve_from_foundry_and_cache(
         self, dataset_identity: dict, branch: str
     ) -> pyspark.sql.DataFrame:
         LOGGER.debug("Caching data for %s on branch %s", dataset_identity, branch)
-        stats = self._cached_client.api.get_dataset_stats(
-            dataset_identity["dataset_rid"], dataset_identity["last_transaction_rid"]
-        )
-        size_in_mega_bytes = stats["sizeInBytes"] / 1024 / 1024
+        transaction = dataset_identity["last_transaction"]["transaction"]
+        if is_dataset_a_view(transaction):
+            foundry_stats = self._cached_client.api.foundry_stats(
+                dataset_identity["dataset_rid"],
+                dataset_identity["last_transaction"]["rid"],
+            )
+            size_in_bytes = int(foundry_stats["computedDatasetStats"]["sizeInBytes"])
+        else:
+            size_in_bytes = transaction["metadata"]["totalFileSize"]
+        size_in_mega_bytes = size_in_bytes / 1024 / 1024
         size_in_mega_bytes_rounded = round(size_in_mega_bytes, ndigits=2)
         LOGGER.debug("Dataset has size of %s MegaBytes.", size_in_mega_bytes_rounded)
         if (
             "transforms_force_full_dataset_download" in self.config
             and self.config["transforms_force_full_dataset_download"] is True
         ) or (
             size_in_mega_bytes < self.config["transforms_sql_dataset_size_threshold"]
```

### Comparing `foundry-dev-tools-1.1/src/transforms/api/_decorators.py` & `foundry-dev-tools-1.2/src/transforms/api/_decorators.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/src/transforms/api/_transform.py` & `foundry-dev-tools-1.2/src/transforms/api/_transform.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/conftest.py` & `foundry-dev-tools-1.2/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,31 +72,34 @@
         )
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.conf_save:
             (
                 foundry_dev_tools.config.INITIAL_CONFIG,
                 foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY,
+                foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_PROJECT_CONFIG_FILE,
             ) = self.conf_save[0]
             foundry_dev_tools.config.Configuration = self.conf_save[1]
 
 
 def override_config(
     initial_config_overwrite: "dict | None" = None,
     config_overwrite: "dict | None" = None,
     read_initial=False,
-) -> "tuple[tuple[dict, pathlib.Path], foundry_dev_tools.config.Config]":
+) -> "tuple[tuple[dict, pathlib.Path,pathlib.Path|None], foundry_dev_tools.config.Config]":
     save = (
         copy.deepcopy(foundry_dev_tools.config.INITIAL_CONFIG),
         copy.deepcopy(foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY),
+        copy.deepcopy(foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_PROJECT_CONFIG_FILE),
     )
     if read_initial:
         (
             foundry_dev_tools.config.INITIAL_CONFIG,
             foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_DIRECTORY,
+            foundry_dev_tools.config.FOUNDRY_DEV_TOOLS_PROJECT_CONFIG_FILE,
         ) = foundry_dev_tools.config.initial_config()
 
     if initial_config_overwrite:
         foundry_dev_tools.config.INITIAL_CONFIG.update(
             foundry_dev_tools.config.type_convert(initial_config_overwrite)
         )
```

### Comparing `foundry-dev-tools-1.1/tests/foundry_mock_client.py` & `foundry-dev-tools-1.2/tests/foundry_mock_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,21 +95,21 @@
                 for file in files_with_hidden
                 if file["logicalPath"] not in [file2["logicalPath"] for file2 in files]
             ),
             "numHiddenFiles": len(files_with_hidden) - len(files),
             "numTransactions": num_transactions,
         }
 
-    def get_dataset_last_transaction_rid(
+    def get_dataset_last_transaction(
         self, dataset_rid: str, branch="master"
-    ) -> "str | None":
+    ) -> "dict | None":
         transactions = self._load_transactions(dataset_rid=dataset_rid)
         if len(transactions) == 0:
             return None
-        return transactions[0]["rid"]
+        return transactions[0]
 
     def get_dataset_identity(
         self, dataset_path_or_rid: str, branch="master", check_read_access=True
     ):
         if "ri.foundry.main.dataset" in dataset_path_or_rid:
             dataset_path = self._rid_to_fs_path(dataset_path_or_rid)
             dataset_rid = dataset_path_or_rid
@@ -129,23 +129,44 @@
             dataset_rid = fs.path.basename(maybe_dataset_rid_file[0])[1:]
         transactions = self._load_transactions(dataset_rid=dataset_rid)
         if (
             len(transactions) == 0
             or len(transactions) == 1
             and transactions[0]["status"] == "OPEN"
         ):
-            last_transaction_rid = None
-        elif len(transactions) > 1 and transactions[0]["status"] == "OPEN":
+            return {
+                "dataset_path": dataset_path,
+                "dataset_rid": dataset_rid,
+                "last_transaction_rid": None,
+                "last_transaction": None,
+            }
+        if len(transactions) > 1 and transactions[0]["status"] == "OPEN":
             last_transaction_rid = transactions[1]["rid"]
         else:
             last_transaction_rid = transactions[0]["rid"]
+
+        stats = self.get_dataset_stats(
+            dataset_rid=dataset_rid, view=last_transaction_rid
+        )
         return {
             "dataset_path": dataset_path,
             "dataset_rid": dataset_rid,
             "last_transaction_rid": last_transaction_rid,
+            "last_transaction": {
+                "rid": last_transaction_rid,
+                "transaction": {
+                    "record": {},
+                    "metadata": {
+                        "fileCount": stats["numFiles"],
+                        "hiddenFileCount": stats["numHiddenFiles"],
+                        "totalFileSize": stats["sizeInBytes"],
+                        "totalHiddenFileSize": stats["hiddenFilesSizeInBytes"],
+                    },
+                },
+            },
         }
 
     def _get_transaction(self, dataset_rid: str, transaction_rid: str) -> dict:
         transactions = self._load_transactions(dataset_rid=dataset_rid)
         maybe_transaction = [
             transaction
             for transaction in transactions
```

### Comparing `foundry-dev-tools-1.1/tests/test_cached_foundry_client.py` & `foundry-dev-tools-1.2/tests/test_cached_foundry_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,25 +261,26 @@
 @patch(
     API + ".get_dataset_identity",
     MagicMock(
         return_value={
             "dataset_rid": DATASET_RID,
             "dataset_path": DATASET_PATH,
             "last_transaction_rid": TRANSACTION_RID,
+            "last_transaction": {"rid": TRANSACTION_RID, "transaction": {}},
         }
     ),
 )
 @patch(API + ".get_dataset_schema")
 @patch(API + ".list_dataset_files")
 @patch(API + ".is_dataset_in_trash")
-@patch(API + ".get_dataset_last_transaction_rid")
+@patch(API + ".get_dataset_last_transaction")
 @patch(API + ".get_dataset_rid")
 def test_fetch_dataset(
     get_dataset_rid,
-    get_dataset_last_transaction_rid,
+    get_dataset_last_transaction,
     is_dataset_in_trash,
     list_dataset_files,
     get_dataset_schema,
     mocker,
 ):
     from_foundry_and_cache = mocker.spy(
         CachedFoundryClient,
@@ -295,15 +296,15 @@
     )
     offline = mocker.spy(
         CachedFoundryClient,
         "_get_dataset_identity_offline",
     )
 
     get_dataset_rid.return_value = DATASET_RID
-    get_dataset_last_transaction_rid.return_value = TRANSACTION_RID
+    get_dataset_last_transaction.return_value = {"rid": TRANSACTION_RID}
     is_dataset_in_trash.return_value = False
     df = get_spark_session().createDataFrame([[1]], "col1:int")
     get_dataset_schema.return_value = {
         "fieldSchemaList": [
             {"type": "INTEGER", "name": "col1", "nullable": True, "customMetadata": {}}
         ],
         "dataFrameReaderClass": "com.palantir.foundry.spark.input.ParquetDataFrameReader",
@@ -331,14 +332,15 @@
 
     fdt = CachedFoundryClient()
     path, dataset_identity = fdt.fetch_dataset(DATASET_PATH, "master")
     assert path.split(os.sep, maxsplit=-1)[-1] == TRANSACTION_RID + ".parquet"
     assert dataset_identity == {
         "dataset_rid": DATASET_RID,
         "last_transaction_rid": TRANSACTION_RID,
+        "last_transaction": {"rid": TRANSACTION_RID, "transaction": {}},
         "dataset_path": DATASET_PATH,
     }
 
     online.assert_called()
     online.reset_mock()
     offline.assert_not_called()
     offline.reset_mock()
@@ -377,25 +379,35 @@
 @patch(
     API + ".get_dataset_identity",
     MagicMock(
         return_value={
             "dataset_rid": DATASET_RID,
             "dataset_path": DATASET_PATH,
             "last_transaction_rid": TRANSACTION_RID,
+            "last_transaction": {
+                "rid": TRANSACTION_RID,
+                "transaction": {
+                    "record": {},
+                    "metadata": {
+                        "fileCount": 1,
+                        "hiddenFileCount": 0,
+                        "totalFileSize": 1000,
+                        "totalHiddenFileSize": 0,
+                    },
+                },
+            },
         }
     ),
 )
 @patch(API + ".get_dataset_schema")
 @patch(API + ".list_dataset_files")
 @patch(API + ".is_dataset_in_trash")
-@patch(API + ".get_dataset_last_transaction_rid")
 @patch(API + ".get_dataset_rid")
 def test_load_dataset(
     get_dataset_rid,
-    get_dataset_last_transaction_rid,
     is_dataset_in_trash,
     list_dataset_files,
     get_dataset_schema,
     mocker,
 ):
     from_foundry_and_cache = mocker.spy(
         CachedFoundryClient,
@@ -404,15 +416,14 @@
     from_cache = mocker.spy(
         CachedFoundryClient,
         "_return_local_path_of_cached_dataset",
     )
     fdt = CachedFoundryClient()
 
     get_dataset_rid.return_value = DATASET_RID
-    get_dataset_last_transaction_rid.return_value = TRANSACTION_RID
     is_dataset_in_trash.return_value = False
     df = get_spark_session().createDataFrame([[1]], "col1:int")
     list_dataset_files.return_value = ["pandas/dataset.parquet"]
     get_dataset_schema.return_value = {
         "fieldSchemaList": [
             {"type": "INTEGER", "name": "col1", "nullable": True, "customMetadata": {}}
         ],
@@ -501,7 +512,70 @@
         from_foundry = cfc.fetch_dataset("/Namespace1/project1/save_model_test")
         import pickle
 
         with Path(from_foundry[0]).joinpath("model.pickle").open(mode="rb") as f:
             model_returned = pickle.load(f)  # noqa: S301, trusted, we are mocking
 
         assert model == model_returned
+
+
+@patch(
+    API + ".get_dataset_identity",
+    MagicMock(
+        return_value={
+            "dataset_rid": DATASET_RID,
+            "dataset_path": DATASET_PATH,
+            "last_transaction_rid": TRANSACTION_RID,
+            "last_transaction": {
+                "rid": TRANSACTION_RID,
+                "transaction": {
+                    "record": {"view": True},
+                    "metadata": {
+                        "fileCount": 1,
+                        "hiddenFileCount": 0,
+                        "totalFileSize": 0,
+                        "totalHiddenFileSize": 0,
+                    },
+                },
+            },
+        }
+    ),
+)
+@patch(API + ".get_dataset_schema")
+@patch(API + ".query_foundry_sql")
+@patch(API + ".is_dataset_in_trash")
+@patch(API + ".get_dataset_rid")
+def test_load_dataset_is_view(
+    get_dataset_rid,
+    is_dataset_in_trash,
+    query_foundry_sql,
+    get_dataset_schema,
+    mocker,
+):
+    from_cache = mocker.spy(
+        CachedFoundryClient,
+        "_return_local_path_of_cached_dataset",
+    )
+    fdt = CachedFoundryClient()
+
+    get_dataset_rid.return_value = DATASET_RID
+    is_dataset_in_trash.return_value = False
+    df = get_spark_session().createDataFrame([[1]], "col1:int")
+    query_foundry_sql.return_value = df
+    get_dataset_schema.return_value = {
+        "fieldSchemaList": [
+            {"type": "INTEGER", "name": "col1", "nullable": True, "customMetadata": {}}
+        ],
+        "dataFrameReaderClass": "com.palantir.foundry.spark.input.ParquetDataFrameReader",
+        "customMetadata": {"format": "parquet", "options": {}},
+    }
+
+    spark_df = fdt.load_dataset(DATASET_PATH, "master")
+
+    from_cache.assert_called()
+    assert query_foundry_sql.call_count == 1
+    from_cache.reset_mock()
+    assert_frame_equal(spark_df.toPandas(), df.toPandas())
+
+    fdt.load_dataset(DATASET_PATH, "master")
+    assert query_foundry_sql.call_count == 1
+    from_cache.assert_called()
```

### Comparing `foundry-dev-tools-1.1/tests/test_cached_foundry_client_integration.py` & `foundry-dev-tools-1.2/tests/test_cached_foundry_client_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_cli_build.py` & `foundry-dev-tools-1.2/tests/test_cli_build.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_config.py` & `foundry-dev-tools-1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_data/binary_dataset/bin` & `foundry-dev-tools-1.2/tests/test_data/binary_dataset/bin`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_data/iris/iris.csv` & `foundry-dev-tools-1.2/tests/test_data/iris/iris.csv`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_foundry_api.py` & `foundry-dev-tools-1.2/tests/test_foundry_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 def test_get_config(is_integration_test, client):
     if is_integration_test:
         assert client._headers()["Authorization"] is not None
     else:
         assert client._headers()["Authorization"] == "Bearer 123"
-        assert client._verify() is not None
+    assert client._requests_verify_value is not None
     assert "transforms_sql_sample_row_limit" in client._config
     assert "transforms_sql_dataset_size_threshold" in client._config
     assert "foundry_url" in client._config
 
 
 @pytest.mark.no_patch_conf()
 def test_sso_config(mocker, tmpdir):
@@ -104,14 +104,25 @@
         client.get_branch(ds["rid"], BRANCH)
 
     branch = client.create_branch(ds["rid"], BRANCH)
     with pytest.raises(BranchesAlreadyExistError):
         _ = client.create_branch(ds["rid"], BRANCH)
     branch_returned = client.get_branch(ds["rid"], BRANCH)
     assert branch == branch_returned
+
+    assert client.get_dataset_identity(ds["rid"], BRANCH) == {
+        "dataset_path": dataset_path,
+        "dataset_rid": ds["rid"],
+        "last_transaction_rid": None,
+        "last_transaction": None,
+    }
+
+    assert client.get_dataset_last_transaction_rid(ds["rid"], BRANCH) is None
+    assert client.get_dataset_last_transaction(ds["rid"], BRANCH) is None
+
     transaction_rid = client.open_transaction(ds["rid"], "SNAPSHOT", BRANCH)
 
     with pytest.raises(DatasetHasOpenTransactionError) as exc_info:
         client.open_transaction(ds["rid"], "SNAPSHOT", BRANCH)
     assert exc_info.value.dataset_rid == ds["rid"]
     assert exc_info.value.open_transaction_rid == transaction_rid
 
@@ -171,14 +182,17 @@
 
     last_good_transaction_rid = client.open_transaction(ds["rid"], "APPEND", BRANCH)
     client.commit_transaction(ds["rid"], last_good_transaction_rid)
 
     failed_transaction = client.open_transaction(ds["rid"], "UPDATE", BRANCH)
     client.abort_transaction(ds["rid"], failed_transaction)
 
+    last_transaction_rid = client.get_dataset_last_transaction(ds["rid"], BRANCH)["rid"]
+    assert last_transaction_rid == last_good_transaction_rid
+
     last_transaction_rid = client.get_dataset_last_transaction_rid(ds["rid"], BRANCH)
     assert last_transaction_rid == last_good_transaction_rid
 
     client.create_branch(ds["rid"], "from-master", branch["id"], branch["rid"])
 
     client.delete_dataset(ds["rid"])
     assert client.is_dataset_in_trash(dataset_path) is True
@@ -188,15 +202,15 @@
 
     with pytest.raises(DatasetNotFoundError):
         client.delete_dataset(ds["rid"])
 
 
 def test_get_dataset_rid(mocker, is_integration_test, client, iris_dataset):
     if not is_integration_test:
-        mock_get = mocker.patch("requests.request")
+        mock_get = mocker.patch("requests.Session.request")
         mock_get.return_value.status_code = 200
         mock_get.return_value.json.return_value = {
             "rid": iris_dataset[0],
             "name": "iris",
             "created": {
                 "time": "2020-01-30T11:18:00.130419Z",
                 "userId": "3c8fbda5-686e-4fcb-ad52-d95e4281d99f",
@@ -316,19 +330,23 @@
         == "Foundry Schema inference completed with status 'WARN' "
         'and message \'No column delimiters found. The delimiter (Comma ",") '
         "was our best guess.'."
     )
     client.delete_dataset(ds["rid"])
 
 
-def test_get_dataset_last_transaction_rid(client, iris_dataset):
-    transaction_rid = client.get_dataset_last_transaction_rid(
+def test_get_dataset_last_transaction(client, iris_dataset):
+    transaction_rid = client.get_dataset_last_transaction(
         iris_dataset[0], branch=iris_dataset[3]
-    )
+    )["rid"]
     assert transaction_rid == iris_dataset[2]
+    assert (
+        client.get_dataset_last_transaction_rid(iris_dataset[0], branch=iris_dataset[3])
+        == iris_dataset[2]
+    )
 
 
 def test_get_dataset_stats(mocker, is_integration_test, client, iris_dataset):
     stats_by_branch = client.get_dataset_stats(iris_dataset[0], view=iris_dataset[3])
     iris_path = f"{TEST_FOLDER.as_posix()}/test_data/iris/iris.csv"
     expected_iris_size = os.path.getsize(iris_path)
     assert stats_by_branch == {
@@ -563,15 +581,15 @@
 
     the_response = mocker.Mock(spec=Response)
     the_response.text = "issue_text"
     the_response.status_code = 400
     the_response.raise_for_status.side_effect = HTTPError(
         "message", response=the_response
     )
-    mocker.patch("requests.request").return_value = the_response
+    mocker.patch("requests.Session.request").return_value = the_response
     with pytest.raises(HTTPError):
         client.get_dataset("test")
     captured = capsys.readouterr()
     assert captured.err == "message\nissue_text\n"
     assert not captured.out
 
 
@@ -609,15 +627,15 @@
         next(
             client.get_child_objects_of_folder(folder_rid="ri.compass.main.folder.1337")
         )
 
     # Test pagination
     import requests
 
-    spy = mocker.spy(requests, "request")
+    spy = mocker.spy(requests.Session, "request")
     children = client.get_child_objects_of_folder(
         folder_rid=INTEGRATION_TEST_COMPASS_ROOT_RID,
         page_size=1,
     )
     spy.assert_not_called()
     next(children)
     spy.assert_called()
```

### Comparing `foundry-dev-tools-1.1/tests/test_foundry_local_deprecation.py` & `foundry-dev-tools-1.2/tests/test_foundry_local_deprecation.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_foundry_mock.py` & `foundry-dev-tools-1.2/tests/test_foundry_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         with pytest.raises(DatasetNotFoundError):
             client.get_dataset_identity(dataset_path_or_rid="doesnotExists")
         with pytest.raises(DatasetNotFoundError):
             client.get_dataset_identity(
                 dataset_path_or_rid="ri.foundry.main.dataset.12342ede-1530-0cf3-8f56-9a4b2231404c"
             )
 
-        assert client.get_dataset_last_transaction_rid(ds["rid"]) is None
+        assert client.get_dataset_last_transaction(ds["rid"]) is None
 
         transaction_rid = client.open_transaction(ds["rid"], "SNAPSHOT", BRANCH)
         branch = client.get_branch(dataset_rid=ds["rid"], branch=BRANCH)
         assert branch["transactionRid"] is None
         assert branch["openTransactionRid"] == transaction_rid
 
         assert (
@@ -198,15 +198,15 @@
         client.commit_transaction(ds["rid"], transaction_rid)
 
         identity_with_transaction_rid = client.get_dataset_identity(
             dataset_path_or_rid=ds["rid"]
         )
         assert identity_with_transaction_rid["last_transaction_rid"] == transaction_rid
 
-        assert client.get_dataset_last_transaction_rid(ds["rid"]) == transaction_rid
+        assert client.get_dataset_last_transaction(ds["rid"])["rid"] == transaction_rid
 
         branch = client.get_branch(dataset_rid=ds["rid"], branch=BRANCH)
         assert branch["transactionRid"] == transaction_rid
         assert branch["openTransactionRid"] is None
 
         files_by_branch = client.list_dataset_files(
             dataset_rid=ds["rid"], view=BRANCH, detail=True
```

### Comparing `foundry-dev-tools-1.1/tests/test_foundry_spark_converters.py` & `foundry-dev-tools-1.2/tests/test_foundry_spark_converters.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_foundry_sql_client.py` & `foundry-dev-tools-1.2/tests/test_foundry_sql_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_fsspec_impl.py` & `foundry-dev-tools-1.2/tests/test_fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_multipass_tpa.py` & `foundry-dev-tools-1.2/tests/test_multipass_tpa.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_spark_caches.py` & `foundry-dev-tools-1.2/tests/test_spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_token_provider.py` & `foundry-dev-tools-1.2/tests/test_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_transforms.py` & `foundry-dev-tools-1.2/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,33 @@
     transform_df,
     transform_pandas,
 )
 from transforms.api._transform import TransformInput, TransformOutput
 
 
 def get_dataset_identity_mock(self, dataset_path: str, branch="master"):
+    dataset_rid = dataset_path.replace("/", "") + "rid1"
+    transaction_rid = dataset_path.replace("/", "") + "rid1" + "t1"
+    stats = get_dataset_stats_mock(self, dataset_rid, branch)
     return {
         "dataset_path": dataset_path,
-        "dataset_rid": dataset_path.replace("/", "") + "rid1",
-        "last_transaction_rid": dataset_path.replace("/", "") + "rid1" + "t1",
+        "dataset_rid": dataset_rid,
+        "last_transaction_rid": transaction_rid,
+        "last_transaction": {
+            "rid": transaction_rid,
+            "transaction": {
+                "record": {},
+                "metadata": {
+                    "fileCount": stats["numFiles"],
+                    "hiddenFileCount": stats["numHiddenFiles"],
+                    "totalFileSize": stats["sizeInBytes"],
+                    "totalHiddenFileSize": stats["hiddenFilesSizeInBytes"],
+                },
+            },
+        },
     }
 
 
 def get_dataset_stats_mock(self, dataset_rid, branch_or_transaction_rid):
     # we return a dataset that is of size 1 mb bigger than the limit to force sql execution and not file download
     return {
         "sizeInBytes": (
```

### Comparing `foundry-dev-tools-1.1/tests/test_transforms_integration.py` & `foundry-dev-tools-1.2/tests/test_transforms_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/test_utils_repo.py` & `foundry-dev-tools-1.2/tests/test_utils_repo.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tests/utils.py` & `foundry-dev-tools-1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.1/tox.ini` & `foundry-dev-tools-1.2/tox.ini`

 * *Files identical despite different names*

