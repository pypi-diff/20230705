# Comparing `tmp/prancer-basic-3.0.7.tar.gz` & `tmp/prancer-basic-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prancer-basic-3.0.7.tar", last modified: Mon Jun  5 08:17:15 2023, max compression
+gzip compressed data, was "prancer-basic-3.0.8.tar", last modified: Wed Jul  5 10:12:00 2023, max compression
```

## Comparing `prancer-basic-3.0.7.tar` & `prancer-basic-3.0.8.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/
--rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/LICENSE
--rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/PKG-INFO
--rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/setup.cfg
--rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.887499 prancer-basic-3.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/prancer_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 08:17:15.000000 prancer-basic-3.0.7/src/prancer_basic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/collection_config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/collection_config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/collection_config/config_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/comparison/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparison_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorLexer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorListener.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorParser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/compare_types.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/rule_interpreter.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/test_comparator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/comparison/rules/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.891499 prancer-basic-3.0.7/src/processor/comparison/rules/arm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/arm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7732 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/arm/secret_azure_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/comparison/rules/cloudformation/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/cloudformation/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/comparison/rules/common/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/common/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/common/sensitive_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/comparison/rules/deploymentmanager/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/deploymentmanager/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/comparison/rules/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/terraform/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/comparison/rules/terraform/secret_tf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/arn_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/connector/git_connector/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/git_connector/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/git_connector/git_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/git_connector/git_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10831 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    58392 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_aws.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23681 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_azure.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_azure_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_base.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_custom.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_custom_refactor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_db.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_exception.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_fs.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33187 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_google.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_kubernetes.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/snapshot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/connector/special_compliance/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/special_compliance/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/special_compliance/compliances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/connector/special_crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/special_crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/special_crawler/azure_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/special_crawler/base_crawler.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/validation.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/connector/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/crawler/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/crawler/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    24954 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/crawler/master_snapshot.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    13969 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/crawler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.895499 prancer-basic-3.0.7/src/processor/database/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/database/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     9891 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/database/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/config/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/config/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/config/config_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/config/remote_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/config/rundata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/file/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/file/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/file/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/hcl/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/hcl/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/hcl/hcl_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/hcl/parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/hcl/transformer.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/hcl/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/httpapi/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/httpapi/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/httpapi/http_utils.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/httpapi/restapi.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/httpapi/restapi_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/jinja/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/jinja/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/jinja/jinja_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/json/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/json/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/json/commentjson.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8248 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/json/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/utils/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/cli_generate_azure_vault_key.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/cli_populate_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/cli_terraform_to_json.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/cli_validator.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/compliance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/fs_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/git_connector.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
--rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/utils/jinjatemplates/mastertest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/helper/yaml/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/yaml/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/helper/yaml/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/logging/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/logging/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/logging/dburl_kv.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/logging/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.899499 prancer-basic-3.0.7/src/processor/reporting/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/reporting/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/reporting/json_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/template_processor/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/ack_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/aso_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/aws_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     6180 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/azure_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/template_processor/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/base/base_template_constatns.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/base/base_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/google_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/helm_chart_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/json_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/kcc_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/kubernetes_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/terraform_template_processor.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/template_processor/yaml_template_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/aws/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/aws/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/aws/aws_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/azure/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/azure/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    17363 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/azure/azure_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/base/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/base/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/base/template_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/google/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/google/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/google/google_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/google/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/helm/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/helm/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/helm/helm_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/kubernetes/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/kubernetes/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/kubernetes/kubernetes_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/terraform/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/terraform/helper/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/terraform/helper/expression/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/expression/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/expression/base_expressions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/expression/terraform_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 08:17:15.903499 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/
--rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/__init__.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/collection_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/encoding_function.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/numeric_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/string_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/terraform_functions.py
--rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/helper/module_parser.py
--rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-06-05 08:14:36.000000 prancer-basic-3.0.7/src/processor/templates/terraform/terraform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.814049 prancer-basic-3.0.8/
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16725 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/LICENSE
+-rwxrwxrwx   0 runner    (1001) docker     (123)       57 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-05 10:12:00.814049 prancer-basic-3.0.8/PKG-INFO
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6966 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 10:12:00.814049 prancer-basic-3.0.8/setup.cfg
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1890 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.794049 prancer-basic-3.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.798049 prancer-basic-3.0.8/src/prancer_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 10:12:00.000000 prancer-basic-3.0.8/src/prancer_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.798049 prancer-basic-3.0.8/src/processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)       39 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.798049 prancer-basic-3.0.8/src/processor/collection_config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/collection_config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6485 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/collection_config/config_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2524 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparison_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13229 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorLexer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      655 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorListener.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    28827 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorParser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2224 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/compare_types.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19688 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/rule_interpreter.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1641 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/test_comparator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    39624 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/arm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/arm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7856 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/arm/secret_azure_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/cloudformation/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/cloudformation/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21971 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/cloudformation/secret_aws_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/common/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/common/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      863 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/common/sensitive_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/deploymentmanager/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/deploymentmanager/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21900 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.802049 prancer-basic-3.0.8/src/processor/comparison/rules/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/terraform/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    38629 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/comparison/rules/terraform/secret_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1557 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/arn_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/connector/git_connector/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/git_connector/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7243 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/git_connector/git_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10890 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/git_connector/git_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10831 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    19921 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    58392 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_aws.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23681 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_azure.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    11475 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_azure_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5593 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_base.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    23145 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_custom.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16164 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_custom_refactor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6353 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_db.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      265 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_exception.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6721 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_fs.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33407 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_google.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    26211 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_kubernetes.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2367 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/snapshot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/connector/special_compliance/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/special_compliance/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1717 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/special_compliance/compliances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/connector/special_crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/special_crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4256 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/special_crawler/azure_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      416 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/special_crawler/base_crawler.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    34555 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/validation.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7256 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/connector/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/crawler/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/crawler/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    24954 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/crawler/master_snapshot.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    13969 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/crawler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/database/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/database/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     9891 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/database/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/config/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/config/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5203 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/config/config_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5311 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/config/remote_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5181 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/config/rundata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/file/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/file/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1090 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/file/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/hcl/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/hcl/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      927 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/hcl/hcl_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      893 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/hcl/parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      301 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/hcl/transformer.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    21915 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/hcl/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/httpapi/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/httpapi/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5822 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/httpapi/http_utils.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3094 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/httpapi/restapi.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14551 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/httpapi/restapi_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/jinja/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/jinja/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3383 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/jinja/jinja_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/json/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/json/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     7147 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/json/commentjson.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8248 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/json/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.806049 prancer-basic-3.0.8/src/processor/helper/utils/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      715 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/cli_generate_azure_vault_key.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14311 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/cli_populate_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1620 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/cli_terraform_to_json.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    29976 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/cli_validator.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    10769 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/compliance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      147 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/fs_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      212 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/git_connector.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      461 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/mastersnapshot.json
+-rwxrwxrwx   0 runner    (1001) docker     (123)      236 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/utils/jinjatemplates/mastertest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/helper/yaml/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/yaml/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2516 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/helper/yaml/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/logging/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/logging/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5625 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/logging/dburl_kv.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    16365 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/logging/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/reporting/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/reporting/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4672 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/reporting/json_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/template_processor/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/ack_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/aso_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     4053 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/aws_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     6176 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/azure_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/template_processor/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1675 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/base/base_template_constatns.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    33402 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/base/base_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2181 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/google_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2245 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/helm_chart_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1989 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/json_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1777 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/kcc_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2295 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/kubernetes_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     5778 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/terraform_template_processor.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2026 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/template_processor/yaml_template_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/aws/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/aws/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    14373 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/aws/aws_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/azure/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/azure/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    17452 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/azure/azure_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/base/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/base/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3483 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/base/template_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/google/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/google/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     8857 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/google/google_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2549 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/google/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/helm/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/helm/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      935 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/helm/helm_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/kubernetes/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/kubernetes/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1275 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/kubernetes/kubernetes_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/terraform/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.810049 prancer-basic-3.0.8/src/processor/templates/terraform/helper/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.814049 prancer-basic-3.0.8/src/processor/templates/terraform/helper/expression/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/expression/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      912 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/expression/base_expressions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      195 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/expression/terraform_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:12:00.814049 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/
+-rwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/__init__.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3995 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/collection_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)      755 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/encoding_function.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     1119 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/numeric_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     2257 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/string_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3829 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/terraform_functions.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)     3490 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/helper/module_parser.py
+-rwxrwxrwx   0 runner    (1001) docker     (123)    52928 2023-07-05 10:09:33.000000 prancer-basic-3.0.8/src/processor/templates/terraform/terraform_parser.py
```

### Comparing `prancer-basic-3.0.7/LICENSE` & `prancer-basic-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/PKG-INFO` & `prancer-basic-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.7
+Version: 3.0.8
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.7/README.md` & `prancer-basic-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/setup.py` & `prancer-basic-3.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  Prancer Basic allows to users to run cloud validation.
  The supported cloud frameworks are azure, aws and git.
 """
 
 setup(
     name='prancer-basic',
     # also update the version in processor.__init__.py file
-    version='3.0.7',
+    version='3.0.8',
     description='Prancer Basic, http://prancer.io/',
     long_description=LONG_DESCRIPTION,
     license = "BSD",
     # The project's main homepage.
     url='https://github.com/prancer-io/cloud-validation-framework',
     # Author(s) details
     author='Farshid M/Ajey Khanapuri',
```

### Comparing `prancer-basic-3.0.7/src/prancer_basic.egg-info/PKG-INFO` & `prancer-basic-3.0.8/src/prancer_basic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: prancer-basic
-Version: 3.0.7
+Version: 3.0.8
 Summary: Prancer Basic, http://prancer.io/
 Home-page: https://github.com/prancer-io/cloud-validation-framework
 Author: Farshid M/Ajey Khanapuri
 Author-email: ajey.khanapuri@liquware.com
 License: BSD
 Description: 
          Prancer Basic allows to users to run cloud validation.
```

### Comparing `prancer-basic-3.0.7/src/prancer_basic.egg-info/SOURCES.txt` & `prancer-basic-3.0.8/src/prancer_basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/prancer_basic.egg-info/requires.txt` & `prancer-basic-3.0.8/src/prancer_basic.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/collection_config/config_handler.py` & `prancer-basic-3.0.8/src/processor/collection_config/config_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparison_functions.py` & `prancer-basic-3.0.8/src/processor/comparison/comparison_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorLexer.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorLexer.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorListener.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorListener.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/comparatorParser.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/comparatorParser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/compare_types.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/compare_types.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/rule_interpreter.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/rule_interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/comparisonantlr/test_comparator.py` & `prancer-basic-3.0.8/src/processor/comparison/comparisonantlr/test_comparator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/interpreter.py` & `prancer-basic-3.0.8/src/processor/comparison/interpreter.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/rules/arm/secret_azure_iac.py` & `prancer-basic-3.0.8/src/processor/comparison/rules/arm/secret_azure_iac.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,25 @@
     if math.log(n) > 0:
         normalized_ent = entropy / math.log(n, 2)
     return entropy, normalized_ent
 
 
 def get_paths(source):
     paths = []
-    if isinstance(source, collections.MutableMapping):
-        for k, v in source.items():
-            paths.append([k])
-            paths += [[k] + x for x in get_paths(v)]
-    elif isinstance(source, collections.Sequence) and not isinstance(source, str):
-        for i, v in enumerate(source):
-            paths.append([i])
-            paths += [[i] + x for x in get_paths(v)]
+    try:
+        if isinstance(source, collections.MutableMapping):
+            for k, v in source.items():
+                paths.append([k])
+                paths += [[k] + x for x in get_paths(v)]
+        elif isinstance(source, collections.Sequence) and not isinstance(source, str):
+            for i, v in enumerate(source):
+                paths.append([i])
+                paths += [[i] + x for x in get_paths(v)]
+    except Exception as ex:
+        logger.warning(" get_paths exception:%s" % ex)
     return paths
 
 
 def secret_finder(snapshot, PASSWORD_VALUE_RE, PASSWORD_KEY_RE=None, EXCLUDE_RE=None, shannon_entropy_password=False):
     output = {}
     errors = []
     try:
```

### Comparing `prancer-basic-3.0.7/src/processor/comparison/rules/cloudformation/secret_aws_iac.py` & `prancer-basic-3.0.8/src/processor/comparison/rules/cloudformation/secret_aws_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/rules/common/sensitive_extension.py` & `prancer-basic-3.0.8/src/processor/comparison/rules/common/sensitive_extension.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py` & `prancer-basic-3.0.8/src/processor/comparison/rules/deploymentmanager/secret_gcp_iac.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/comparison/rules/terraform/secret_tf.py` & `prancer-basic-3.0.8/src/processor/comparison/rules/terraform/secret_tf.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/arn_parser.py` & `prancer-basic-3.0.8/src/processor/connector/arn_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/git_connector/git_functions.py` & `prancer-basic-3.0.8/src/processor/connector/git_connector/git_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/git_connector/git_processor.py` & `prancer-basic-3.0.8/src/processor/connector/git_connector/git_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/populate_json.py` & `prancer-basic-3.0.8/src/processor/connector/populate_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_aws.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_aws.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_azure.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_azure.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_azure_refactor.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_azure_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_base.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_base.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_custom.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_custom.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_custom_refactor.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_custom_refactor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_db.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_db.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_fs.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_fs.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_google.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_google.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,17 @@
                     account = response['name']
                     params[item] = account.split('/')[-3]
 
             elif item == r"{key}" or item == r"{service_name}":
                 key_before_split = response['name']
                 params[item] = key_before_split.split('/')[-1]
 
+            elif item == r"{cloud_run_service}":
+                params[item] = response['metadata']['name']
+
         return params
     except Exception as ex:
         return params
 
 def get_request_url_get_method(get_method, item, project_id=None):
     request_url, _ = get_method_api_path(get_method)
     url_list = request_url.split('/')
@@ -529,26 +532,27 @@
 
         else:
             if "selfLink" in item.keys():
                 request_url = item['selfLink']
             elif "id" in item.keys():
                 request_url = request_url+"/"+item["id"].split(":")[-1]
             elif "name" in item.keys():
-                request_url = request_url+"/"+item["name"]
-
-        path_list = request_url.split("https://")
-        
+                request_url = item["name"]
         if  '/{' in request_url or '}/' in request_url:
             return snapshot_data
 
-        if len(path_list) > 1:
-            path_list = path_list[1].split('/')
-            path = "/".join(path_list[1:])
+        if request_url and request_url.startswith("https://"):
+            path_list = request_url.split("https://")
+            if len(path_list) > 1:
+                path_list = path_list[1].split('/')
+                path = "/".join(path_list[1:])
+            else:
+                return snapshot_data
         else:
-            return snapshot_data
+            path = request_url
 
         found_old_record = False
         for snapshot_list in snapshot_data.values():
             old_record = None
             if isinstance(snapshot_list, list):
                 for item in snapshot_list:
                     if item["path"] == path:
```

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_kubernetes.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_kubernetes.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/snapshot_utils.py` & `prancer-basic-3.0.8/src/processor/connector/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/special_compliance/compliances.py` & `prancer-basic-3.0.8/src/processor/connector/special_compliance/compliances.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/special_crawler/azure_crawler.py` & `prancer-basic-3.0.8/src/processor/connector/special_crawler/azure_crawler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/validation.py` & `prancer-basic-3.0.8/src/processor/connector/validation.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/connector/vault.py` & `prancer-basic-3.0.8/src/processor/connector/vault.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/crawler/master_snapshot.py` & `prancer-basic-3.0.8/src/processor/crawler/master_snapshot.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/crawler/utils.py` & `prancer-basic-3.0.8/src/processor/crawler/utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/database/database.py` & `prancer-basic-3.0.8/src/processor/database/database.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/config/config_utils.py` & `prancer-basic-3.0.8/src/processor/helper/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/config/remote_utils.py` & `prancer-basic-3.0.8/src/processor/helper/config/remote_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/config/rundata_utils.py` & `prancer-basic-3.0.8/src/processor/helper/config/rundata_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/file/file_utils.py` & `prancer-basic-3.0.8/src/processor/helper/file/file_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/hcl/hcl_utils.py` & `prancer-basic-3.0.8/src/processor/helper/hcl/hcl_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/hcl/parser.py` & `prancer-basic-3.0.8/src/processor/helper/hcl/parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/hcl/yacc.py` & `prancer-basic-3.0.8/src/processor/helper/hcl/yacc.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/httpapi/http_utils.py` & `prancer-basic-3.0.8/src/processor/helper/httpapi/http_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/httpapi/restapi.py` & `prancer-basic-3.0.8/src/processor/helper/httpapi/restapi.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/httpapi/restapi_azure.py` & `prancer-basic-3.0.8/src/processor/helper/httpapi/restapi_azure.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/jinja/jinja_utils.py` & `prancer-basic-3.0.8/src/processor/helper/jinja/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/json/commentjson.py` & `prancer-basic-3.0.8/src/processor/helper/json/commentjson.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/json/json_utils.py` & `prancer-basic-3.0.8/src/processor/helper/json/json_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/utils/cli_generate_azure_vault_key.py` & `prancer-basic-3.0.8/src/processor/helper/utils/cli_generate_azure_vault_key.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/utils/cli_populate_json.py` & `prancer-basic-3.0.8/src/processor/helper/utils/cli_populate_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/utils/cli_terraform_to_json.py` & `prancer-basic-3.0.8/src/processor/helper/utils/cli_terraform_to_json.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/utils/cli_validator.py` & `prancer-basic-3.0.8/src/processor/helper/utils/cli_validator.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/utils/compliance_utils.py` & `prancer-basic-3.0.8/src/processor/helper/utils/compliance_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/helper/yaml/yaml_utils.py` & `prancer-basic-3.0.8/src/processor/helper/yaml/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/logging/dburl_kv.py` & `prancer-basic-3.0.8/src/processor/logging/dburl_kv.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/logging/log_handler.py` & `prancer-basic-3.0.8/src/processor/logging/log_handler.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/reporting/json_output.py` & `prancer-basic-3.0.8/src/processor/reporting/json_output.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/ack_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/ack_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/aso_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/aso_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/aws_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/aws_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/azure_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/azure_template_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def is_template_file(self, file_path):
         """
         check for valid template file for parse arm template
         """
         if len(file_path.split(".")) > 0 and file_path.split(".")[-1] == "json":
             json_data = json_from_file(file_path)
             if json_data and '$schema' in json_data and json_data['$schema']:
-                match =  re.match(r'.*/deploymentTemplate.json#$', json_data['$schema'], re.I)
+                match =  re.match(r'.*eploymentTemplate.json#$', json_data['$schema'], re.I)
                 return True if match else False
         return False
 
     def process_template(self, paths):
         """
         process the files stored at specified paths and returns the template
         """
@@ -98,17 +98,17 @@
                     logger.error("Invalid template file path %s, or file does not contains the valid json format." % json_file)
                     return template_json
                 elif "$schema" not in json_data:
                     logger.error(
                         "Invalid json : does not contains '$schema' field in json.")
                     return template_json
                 else:
-                    if "deploymentTemplate.json" in json_data['$schema'].split("/")[-1]:
+                    if "eploymentTemplate.json" in json_data['$schema'].split("/")[-1]:
                         template_file_path = json_file_path
-                    elif "deploymentParameters.json" in json_data['$schema'].split("/")[-1]:
+                    elif "eploymentParameters.json" in json_data['$schema'].split("/")[-1]:
                         deployment_file_path = json_file_path
                     else:
                         logger.error("Invalid json : $schema does not contains the correct value")
             
             if template_file_path:
                 if azure_cli_flag and azure_cli_flag == "true":
                     if deployment_file_path:
```

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/base/base_template_constatns.py` & `prancer-basic-3.0.8/src/processor/template_processor/base/base_template_constatns.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/base/base_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/base/base_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/google_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/google_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/helm_chart_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/helm_chart_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/json_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/json_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/kcc_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/kcc_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/kubernetes_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/kubernetes_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/terraform_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/terraform_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/template_processor/yaml_template_processor.py` & `prancer-basic-3.0.8/src/processor/template_processor/yaml_template_processor.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/aws/aws_parser.py` & `prancer-basic-3.0.8/src/processor/templates/aws/aws_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/azure/azure_parser.py` & `prancer-basic-3.0.8/src/processor/templates/azure/azure_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,27 +38,28 @@
         self.replace_spacial_characters(template_json)
         gen_template_json = None
         if template_json:
             gen_template_json = copy.deepcopy(template_json)
             if 'parameters' not in template_json:
                 template_json['parameters'] = {}
             self.gparams = template_json['parameters']
-            for param in self.get_parameter():
-                param_json = json_from_file(param)
-                if 'parameters' in  param_json and param_json['parameters']:
-                    for key, value in param_json['parameters'].items():
-                        # if key in template_json['parameters']:
-                        if "value" in value:
-                            if key not in template_json['parameters']:
-                                template_json['parameters'][key] = {'value': value['value']}
+            if self.get_parameter():
+                for param in self.get_parameter():
+                    param_json = json_from_file(param)
+                    if 'parameters' in  param_json and param_json['parameters']:
+                        for key, value in param_json['parameters'].items():
+                            # if key in template_json['parameters']:
+                            if "value" in value:
+                                if key not in template_json['parameters']:
+                                    template_json['parameters'][key] = {'value': value['value']}
+                                else:
+                                    template_json['parameters'][key]['value'] = value['value']
                             else:
-                                template_json['parameters'][key]['value'] = value['value']
-                        else:
-                            logger.debug("Default value is not specified for %s parameter.", key)
-                gen_template_json['parameters'] = self.gparams
+                                logger.debug("Default value is not specified for %s parameter.", key)
+                    gen_template_json['parameters'] = self.gparams
             # print('%s Updated Parameters %s' % (stars, stars))
             # print(json.dumps(template_json['parameters'], indent=2))
             if 'variables' in template_json:
                 self.gvariables = template_json['variables']
                 new_resource = self.process_resource(template_json['variables'])
                 # print('%s Original Variables %s' % (stars, stars))
                 # print(json.dumps(template_json['variables'], indent=2))
@@ -299,15 +300,15 @@
         return None
             
     def is_template_file(self, filename):
         if filename and filename.endswith('_gen.json'):
             return False
         json_data = json_from_file(filename)
         if json_data and '$schema' in json_data and json_data['$schema']:
-            match =  re.match(r'.*deploymentTemplate.json#$', json_data['$schema'], re.I)
+            match =  re.match(r'.*eploymentTemplate.json#$', json_data['$schema'], re.I)
             return True if match else False
         return None
             
     def eval_expression(self, value):
         match = re.match(r'\[(.*)\]', value, re.I)
         if match:
             return match.groups()[0]
@@ -390,8 +391,8 @@
                         isupdated = True
                         retval = retval[i]
                     
                     if not isupdated:
                         retval = None
                 else:
                     retval = retval[field] if retval and field in retval and isinstance(retval, dict) else None
-        return retval
+        return retval
```

### Comparing `prancer-basic-3.0.7/src/processor/templates/base/template_parser.py` & `prancer-basic-3.0.8/src/processor/templates/base/template_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/google/google_parser.py` & `prancer-basic-3.0.8/src/processor/templates/google/google_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/google/util.py` & `prancer-basic-3.0.8/src/processor/templates/google/util.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/helm/helm_parser.py` & `prancer-basic-3.0.8/src/processor/templates/helm/helm_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/kubernetes/kubernetes_parser.py` & `prancer-basic-3.0.8/src/processor/templates/kubernetes/kubernetes_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/expression/base_expressions.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/expression/base_expressions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/collection_functions.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/collection_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/encoding_function.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/encoding_function.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/numeric_functions.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/string_functions.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/string_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/function/terraform_functions.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/function/terraform_functions.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/helper/module_parser.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/helper/module_parser.py`

 * *Files identical despite different names*

### Comparing `prancer-basic-3.0.7/src/processor/templates/terraform/terraform_parser.py` & `prancer-basic-3.0.8/src/processor/templates/terraform/terraform_parser.py`

 * *Files identical despite different names*

