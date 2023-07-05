# Comparing `tmp/udps-0.1.19.tar.gz` & `tmp/udps-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udps-0.1.19.tar", max compression
+gzip compressed data, was "udps-0.1.20.tar", max compression
```

## Comparing `udps-0.1.19.tar` & `udps-0.1.20.tar`

### file list

```diff
@@ -1,249 +1,253 @@
--rw-r--r--   0        0        0    11357 2023-06-20 12:08:37.029402 udps-0.1.19/LICENSE
--rw-r--r--   0        0        0     2471 2023-06-20 12:08:37.029402 udps-0.1.19/README.md
--rw-r--r--   0        0        0     3071 2023-06-20 12:08:37.033403 udps-0.1.19/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-20 12:08:37.033403 udps-0.1.19/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.033403 udps-0.1.19/tests/mocks/__init__.py
--rw-r--r--   0        0        0      721 2023-06-20 12:08:37.033403 udps-0.1.19/tests/mocks/mock_writers.py
--rw-r--r--   0        0        0     1028 2023-06-20 12:08:37.033403 udps-0.1.19/tests/test_authz_analyzer.py
--rw-r--r--   0        0        0     5976 2023-06-20 12:08:37.033403 udps-0.1.19/tests/test_cli.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.033403 udps-0.1.19/tests/test_writers/__init__.py
--rw-r--r--   0        0        0     1355 2023-06-20 12:08:37.033403 udps-0.1.19/tests/test_writers/test_csv_writer.py
--rw-r--r--   0        0        0      953 2023-06-20 12:08:37.033403 udps-0.1.19/tests/test_writers/test_multijson_writer.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/__init__.py
--rw-r--r--   0        0        0        1 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/__init__.py
--rw-r--r--   0        0        0    14110 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
--rw-r--r--   0        0        0    11644 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
--rw-r--r--   0        0        0    14917 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
--rw-r--r--   0        0        0     9884 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
--rw-r--r--   0        0        0    20662 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
--rw-r--r--   0        0        0    31812 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
--rw-r--r--   0        0        0    18235 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
--rw-r--r--   0        0        0    17618 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
--rw-r--r--   0        0        0     7529 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
--rw-r--r--   0        0        0     7744 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
--rw-r--r--   0        0        0     4073 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
--rw-r--r--   0        0        0    24204 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
--rw-r--r--   0        0        0    20163 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
--rw-r--r--   0        0        0    13494 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
--rw-r--r--   0        0        0     8446 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
--rw-r--r--   0        0        0    16466 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
--rw-r--r--   0        0        0    16126 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
--rw-r--r--   0        0        0    14831 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
--rw-r--r--   0        0        0     3066 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
--rw-r--r--   0        0        0     5550 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
--rw-r--r--   0        0        0     5906 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
--rw-r--r--   0        0        0     4446 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
--rw-r--r--   0        0        0     8937 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
--rw-r--r--   0        0        0    20162 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
--rw-r--r--   0        0        0    10324 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
--rw-r--r--   0        0        0     6886 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
--rw-r--r--   0        0        0    23422 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
--rw-r--r--   0        0        0     2358 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
--rw-r--r--   0        0        0     7124 2023-06-20 12:08:37.033403 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
--rw-r--r--   0        0        0     4549 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
--rw-r--r--   0        0        0     5215 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
--rw-r--r--   0        0        0     5987 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
--rw-r--r--   0        0        0     5862 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
--rw-r--r--   0        0        0     3396 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
--rw-r--r--   0        0        0     2298 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
--rw-r--r--   0        0        0     5264 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
--rw-r--r--   0        0        0     4596 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
--rw-r--r--   0        0        0     3653 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
--rw-r--r--   0        0        0     4392 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
--rw-r--r--   0        0        0    26158 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
--rw-r--r--   0        0        0    10097 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
--rw-r--r--   0        0        0     8580 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
--rw-r--r--   0        0        0    33775 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
--rw-r--r--   0        0        0    16439 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
--rw-r--r--   0        0        0    13955 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
--rw-r--r--   0        0        0    18162 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
--rw-r--r--   0        0        0     3040 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
--rw-r--r--   0        0        0     5254 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
--rw-r--r--   0        0        0     3569 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
--rw-r--r--   0        0        0     4436 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
--rw-r--r--   0        0        0    14441 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
--rw-r--r--   0        0        0     3582 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
--rw-r--r--   0        0        0     4890 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
--rw-r--r--   0        0        0     4842 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0     2831 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
--rw-r--r--   0        0        0     1595 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
--rw-r--r--   0        0        0     3805 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
--rw-r--r--   0        0        0     2597 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
--rw-r--r--   0        0        0     2321 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
--rw-r--r--   0        0        0     4018 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
--rw-r--r--   0        0        0     5298 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
--rw-r--r--   0        0        0     1579 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/test_exporter.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/utils/__init__.py
--rw-r--r--   0        0        0     1731 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/bigquery/__init__.py
--rw-r--r--   0        0        0     5596 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/bigquery/generate_authz_entry.py
--rw-r--r--   0        0        0     7137 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/bigquery/mocks.py
--rw-r--r--   0        0        0    15539 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/bigquery/test_bigquery.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/databricks/__init__.py
--rw-r--r--   0        0        0    17596 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/databricks/generate_authz_entry.py
--rw-r--r--   0        0        0     9136 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/databricks/mocks.py
--rw-r--r--   0        0        0    13149 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/databricks/test_analyzer.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    14532 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/mongodb/test_atlas_organization_users.py
--rw-r--r--   0        0        0     7391 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/mongodb/test_mongodb.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/postgres/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/postgres/mocks/__init__.py
--rw-r--r--   0        0        0     1195 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
--rw-r--r--   0        0        0    12910 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/postgres/test_postgress_analyzer.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/redshift/__init__.py
--rw-r--r--   0        0        0    12179 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/redshift/test_redshift.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    18443 2023-06-20 12:08:37.037402 udps-0.1.19/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
--rw-r--r--   0        0        0     1086 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/__init__.py
--rw-r--r--   0        0        0    10502 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/cli.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/__init__.py
--rw-r--r--   0        0        0      626 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/__init__.py
--rw-r--r--   0        0        0      113 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
--rw-r--r--   0        0        0     3252 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
--rw-r--r--   0        0        0     7808 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
--rw-r--r--   0        0        0    13042 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
--rw-r--r--   0        0        0       90 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
--rw-r--r--   0        0        0      141 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
--rw-r--r--   0        0        0      111 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
--rw-r--r--   0        0        0       14 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
--rw-r--r--   0        0        0      125 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
--rw-r--r--   0        0        0      893 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
--rw-r--r--   0        0        0      262 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
--rw-r--r--   0        0        0     5539 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
--rw-r--r--   0        0        0     3524 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
--rw-r--r--   0        0        0      660 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
--rw-r--r--   0        0        0      120 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
--rw-r--r--   0        0        0     2045 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
--rw-r--r--   0        0        0     5682 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
--rw-r--r--   0        0        0     3505 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
--rw-r--r--   0        0        0     2481 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
--rw-r--r--   0        0        0     6201 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
--rw-r--r--   0        0        0     3963 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
--rw-r--r--   0        0        0      254 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
--rw-r--r--   0        0        0       87 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
--rw-r--r--   0        0        0      263 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
--rw-r--r--   0        0        0      415 2023-06-20 12:08:37.037402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
--rw-r--r--   0        0        0     6232 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
--rw-r--r--   0        0        0    10500 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
--rw-r--r--   0        0        0      373 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
--rw-r--r--   0        0        0      261 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
--rw-r--r--   0        0        0      263 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
--rw-r--r--   0        0        0      261 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
--rw-r--r--   0        0        0     5655 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
--rw-r--r--   0        0        0     1961 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
--rw-r--r--   0        0        0     1824 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
--rw-r--r--   0        0        0     2502 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
--rw-r--r--   0        0        0     1046 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
--rw-r--r--   0        0        0      263 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
--rw-r--r--   0        0        0    18760 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
--rw-r--r--   0        0        0      172 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
--rw-r--r--   0        0        0    12130 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
--rw-r--r--   0        0        0     1267 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
--rw-r--r--   0        0        0    12938 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
--rw-r--r--   0        0        0     3704 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
--rw-r--r--   0        0        0    10597 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
--rw-r--r--   0        0        0    12040 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
--rw-r--r--   0        0        0     8007 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
--rw-r--r--   0        0        0    15325 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
--rw-r--r--   0        0        0    26419 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
--rw-r--r--   0        0        0     6471 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
--rw-r--r--   0        0        0      513 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
--rw-r--r--   0        0        0     8549 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
--rw-r--r--   0        0        0     5233 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
--rw-r--r--   0        0        0     4475 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
--rw-r--r--   0        0        0     1644 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
--rw-r--r--   0        0        0     2905 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
--rw-r--r--   0        0        0     6158 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
--rw-r--r--   0        0        0     2185 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
--rw-r--r--   0        0        0     2147 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
--rw-r--r--   0        0        0     7453 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
--rw-r--r--   0        0        0     2289 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
--rw-r--r--   0        0        0     2594 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
--rw-r--r--   0        0        0     3377 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
--rw-r--r--   0        0        0     1054 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
--rw-r--r--   0        0        0    17633 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
--rw-r--r--   0        0        0     7562 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
--rw-r--r--   0        0        0     1894 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
--rw-r--r--   0        0        0      398 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
--rw-r--r--   0        0        0     1973 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
--rw-r--r--   0        0        0     3041 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
--rw-r--r--   0        0        0      397 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
--rw-r--r--   0        0        0      561 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
--rw-r--r--   0        0        0     2501 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
--rw-r--r--   0        0        0     9989 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0      482 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
--rw-r--r--   0        0        0      879 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
--rw-r--r--   0        0        0     1000 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
--rw-r--r--   0        0        0     2747 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
--rw-r--r--   0        0        0      173 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
--rw-r--r--   0        0        0      131 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/__init__.py
--rw-r--r--   0        0        0    11747 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
--rw-r--r--   0        0        0    12689 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
--rw-r--r--   0        0        0     7740 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/service.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/__init__.py
--rw-r--r--   0        0        0     5687 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/analyzer.py
--rw-r--r--   0        0        0       53 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/exceptions.py
--rw-r--r--   0        0        0     8187 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/identities.py
--rw-r--r--   0        0        0     1331 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/model.py
--rw-r--r--   0        0        0    10555 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/service/model.py
--rw-r--r--   0        0        0     1425 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/service/scim.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    16135 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
--rw-r--r--   0        0        0    17422 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
--rw-r--r--   0        0        0     6172 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
--rw-r--r--   0        0        0     2527 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
--rw-r--r--   0        0        0     5892 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
--rw-r--r--   0        0        0     2394 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
--rw-r--r--   0        0        0     2197 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/model.py
--rw-r--r--   0        0        0     1553 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
--rw-r--r--   0        0        0     1448 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/service.py
--rw-r--r--   0        0        0     1196 2023-06-20 12:08:37.041402 udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/service_model.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/__init__.py
--rw-r--r--   0        0        0    10604 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/analyzer.py
--rw-r--r--   0        0        0       71 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
--rw-r--r--   0        0        0      369 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
--rw-r--r--   0        0        0      272 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
--rw-r--r--   0        0        0      313 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
--rw-r--r--   0        0        0     2404 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
--rw-r--r--   0        0        0      822 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/deployment.py
--rw-r--r--   0        0        0     2687 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/exporter.py
--rw-r--r--   0        0        0     1891 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/model.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    12641 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
--rw-r--r--   0        0        0      389 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
--rw-r--r--   0        0        0       20 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
--rw-r--r--   0        0        0       11 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
--rw-r--r--   0        0        0      535 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
--rw-r--r--   0        0        0     5827 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/exporter.py
--rw-r--r--   0        0        0     4685 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/model.py
--rw-r--r--   0        0        0     1048 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/service.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/errors/__init__.py
--rw-r--r--   0        0        0       45 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/errors/failed_connection_errors.py
--rw-r--r--   0        0        0     7035 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/main.py
--rw-r--r--   0        0        0      195 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/models/__init__.py
--rw-r--r--   0        0        0     7583 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/models/model.py
--rw-r--r--   0        0        0        0 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/utils/__init__.py
--rw-r--r--   0        0        0      651 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/utils/logger.py
--rw-r--r--   0        0        0      452 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/writers/__init__.py
--rw-r--r--   0        0        0     1020 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/writers/base_writers.py
--rw-r--r--   0        0        0      728 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/writers/csv_writer.py
--rw-r--r--   0        0        0     1138 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/writers/get_writers.py
--rw-r--r--   0        0        0     2090 2023-06-20 12:08:37.045403 udps-0.1.19/universal_data_permissions_scanner/writers/multi_json_exporter.py
--rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 udps-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 09:51:27.775414 udps-0.1.20/LICENSE
+-rw-r--r--   0        0        0     2471 2023-07-05 09:51:27.775414 udps-0.1.20/README.md
+-rw-r--r--   0        0        0     3071 2023-07-05 09:51:27.775414 udps-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-05 09:51:27.775414 udps-0.1.20/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/mocks/__init__.py
+-rw-r--r--   0        0        0      721 2023-07-05 09:51:27.775414 udps-0.1.20/tests/mocks/mock_writers.py
+-rw-r--r--   0        0        0     1028 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_authz_analyzer.py
+-rw-r--r--   0        0        0     6246 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/__init__.py
+-rw-r--r--   0        0        0     1355 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/test_csv_writer.py
+-rw-r--r--   0        0        0      953 2023-07-05 09:51:27.775414 udps-0.1.20/tests/test_writers/test_multijson_writer.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0    14110 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
+-rw-r--r--   0        0        0    11644 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
+-rw-r--r--   0        0        0    14917 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
+-rw-r--r--   0        0        0     9884 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
+-rw-r--r--   0        0        0    20662 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
+-rw-r--r--   0        0        0    31812 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
+-rw-r--r--   0        0        0    18235 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
+-rw-r--r--   0        0        0    17618 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
+-rw-r--r--   0        0        0     7529 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
+-rw-r--r--   0        0        0     7744 2023-07-05 09:51:27.775414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
+-rw-r--r--   0        0        0     4073 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
+-rw-r--r--   0        0        0    24204 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
+-rw-r--r--   0        0        0    20163 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
+-rw-r--r--   0        0        0    13494 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
+-rw-r--r--   0        0        0     8446 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
+-rw-r--r--   0        0        0    16466 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
+-rw-r--r--   0        0        0    16126 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
+-rw-r--r--   0        0        0    14831 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
+-rw-r--r--   0        0        0     3066 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
+-rw-r--r--   0        0        0     5550 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
+-rw-r--r--   0        0        0     5906 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
+-rw-r--r--   0        0        0     4446 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
+-rw-r--r--   0        0        0     8937 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
+-rw-r--r--   0        0        0    20162 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
+-rw-r--r--   0        0        0    10324 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
+-rw-r--r--   0        0        0     6886 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
+-rw-r--r--   0        0        0    23422 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
+-rw-r--r--   0        0        0     2358 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
+-rw-r--r--   0        0        0     7124 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
+-rw-r--r--   0        0        0     4549 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
+-rw-r--r--   0        0        0     5215 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
+-rw-r--r--   0        0        0     5987 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
+-rw-r--r--   0        0        0     5862 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
+-rw-r--r--   0        0        0     3396 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
+-rw-r--r--   0        0        0     2298 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
+-rw-r--r--   0        0        0     5264 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
+-rw-r--r--   0        0        0     4596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
+-rw-r--r--   0        0        0     3653 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
+-rw-r--r--   0        0        0     4392 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
+-rw-r--r--   0        0        0    26158 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
+-rw-r--r--   0        0        0    10097 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
+-rw-r--r--   0        0        0     8580 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
+-rw-r--r--   0        0        0    33775 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
+-rw-r--r--   0        0        0    16439 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
+-rw-r--r--   0        0        0    13955 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
+-rw-r--r--   0        0        0    18162 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
+-rw-r--r--   0        0        0     3040 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
+-rw-r--r--   0        0        0     5254 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
+-rw-r--r--   0        0        0     3569 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
+-rw-r--r--   0        0        0     4436 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
+-rw-r--r--   0        0        0    14441 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
+-rw-r--r--   0        0        0     3582 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
+-rw-r--r--   0        0        0     4890 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
+-rw-r--r--   0        0        0     4842 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
+-rw-r--r--   0        0        0     1595 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
+-rw-r--r--   0        0        0     3805 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
+-rw-r--r--   0        0        0     2597 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
+-rw-r--r--   0        0        0     2321 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
+-rw-r--r--   0        0        0     4018 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
+-rw-r--r--   0        0        0     5298 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
+-rw-r--r--   0        0        0     1579 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/test_exporter.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/utils/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0     5596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/generate_authz_entry.py
+-rw-r--r--   0        0        0     7137 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/mocks.py
+-rw-r--r--   0        0        0    15539 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/bigquery/test_bigquery.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/__init__.py
+-rw-r--r--   0        0        0    17596 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/generate_authz_entry.py
+-rw-r--r--   0        0        0     9136 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/mocks.py
+-rw-r--r--   0        0        0    13149 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/databricks/test_analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    14532 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/test_atlas_organization_users.py
+-rw-r--r--   0        0        0     7391 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/mongodb/test_mongodb.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/mocks/__init__.py
+-rw-r--r--   0        0        0     1195 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
+-rw-r--r--   0        0        0    12910 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/postgres/test_postgress_analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/redshift/__init__.py
+-rw-r--r--   0        0        0    12179 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/redshift/test_redshift.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    19120 2023-07-05 09:51:27.779414 udps-0.1.20/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
+-rw-r--r--   0        0        0     1086 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/__init__.py
+-rw-r--r--   0        0        0    11523 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/cli.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
+-rw-r--r--   0        0        0     3252 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
+-rw-r--r--   0        0        0     7808 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.779414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
+-rw-r--r--   0        0        0    13042 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
+-rw-r--r--   0        0        0       90 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
+-rw-r--r--   0        0        0      141 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
+-rw-r--r--   0        0        0      111 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
+-rw-r--r--   0        0        0       14 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
+-rw-r--r--   0        0        0      125 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
+-rw-r--r--   0        0        0      893 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
+-rw-r--r--   0        0        0      262 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
+-rw-r--r--   0        0        0     5539 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
+-rw-r--r--   0        0        0     3524 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
+-rw-r--r--   0        0        0      660 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
+-rw-r--r--   0        0        0      120 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
+-rw-r--r--   0        0        0     3041 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
+-rw-r--r--   0        0        0     2045 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
+-rw-r--r--   0        0        0     5682 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
+-rw-r--r--   0        0        0     3505 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
+-rw-r--r--   0        0        0     2481 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
+-rw-r--r--   0        0        0     6201 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
+-rw-r--r--   0        0        0     3963 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
+-rw-r--r--   0        0        0      254 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
+-rw-r--r--   0        0        0       87 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
+-rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
+-rw-r--r--   0        0        0      415 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
+-rw-r--r--   0        0        0     6232 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
+-rw-r--r--   0        0        0    10500 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
+-rw-r--r--   0        0        0      373 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
+-rw-r--r--   0        0        0      261 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
+-rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
+-rw-r--r--   0        0        0      261 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
+-rw-r--r--   0        0        0     5655 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
+-rw-r--r--   0        0        0     1961 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
+-rw-r--r--   0        0        0     1824 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
+-rw-r--r--   0        0        0     2502 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
+-rw-r--r--   0        0        0     1046 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
+-rw-r--r--   0        0        0      263 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
+-rw-r--r--   0        0        0    18760 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
+-rw-r--r--   0        0        0      172 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
+-rw-r--r--   0        0        0    12130 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
+-rw-r--r--   0        0        0     1267 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
+-rw-r--r--   0        0        0    12938 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
+-rw-r--r--   0        0        0     3704 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
+-rw-r--r--   0        0        0    10597 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
+-rw-r--r--   0        0        0    12040 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
+-rw-r--r--   0        0        0     8007 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
+-rw-r--r--   0        0        0    15325 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
+-rw-r--r--   0        0        0    26419 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
+-rw-r--r--   0        0        0     6471 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
+-rw-r--r--   0        0        0      513 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
+-rw-r--r--   0        0        0     8549 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
+-rw-r--r--   0        0        0     5233 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
+-rw-r--r--   0        0        0     4475 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
+-rw-r--r--   0        0        0     1644 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
+-rw-r--r--   0        0        0     6158 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
+-rw-r--r--   0        0        0     2185 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
+-rw-r--r--   0        0        0     2147 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
+-rw-r--r--   0        0        0     7453 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
+-rw-r--r--   0        0        0     2289 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
+-rw-r--r--   0        0        0     2594 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
+-rw-r--r--   0        0        0     3377 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
+-rw-r--r--   0        0        0     1054 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
+-rw-r--r--   0        0        0    17633 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
+-rw-r--r--   0        0        0     7562 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
+-rw-r--r--   0        0        0     1894 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
+-rw-r--r--   0        0        0      398 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
+-rw-r--r--   0        0        0     1973 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
+-rw-r--r--   0        0        0     3041 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
+-rw-r--r--   0        0        0      397 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
+-rw-r--r--   0        0        0      561 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
+-rw-r--r--   0        0        0     2501 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
+-rw-r--r--   0        0        0     9989 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0      482 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
+-rw-r--r--   0        0        0      879 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
+-rw-r--r--   0        0        0     1000 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
+-rw-r--r--   0        0        0     2747 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
+-rw-r--r--   0        0        0      173 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
+-rw-r--r--   0        0        0      131 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0    11747 2023-07-05 09:51:27.783414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
+-rw-r--r--   0        0        0    12689 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
+-rw-r--r--   0        0        0     7740 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/service.py
+-rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/__init__.py
+-rw-r--r--   0        0        0     6516 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/analyzer.py
+-rw-r--r--   0        0        0       53 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/exceptions.py
+-rw-r--r--   0        0        0     8187 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/identities.py
+-rw-r--r--   0        0        0     1331 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/model.py
+-rw-r--r--   0        0        0    10555 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
+-rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/__init__.py
+-rw-r--r--   0        0        0      879 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py
+-rw-r--r--   0        0        0      110 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/basic.py
+-rw-r--r--   0        0        0     1894 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py
+-rw-r--r--   0        0        0     2448 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/model.py
+-rw-r--r--   0        0        0     1425 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/scim.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    16135 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
+-rw-r--r--   0        0        0    17422 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
+-rw-r--r--   0        0        0     6172 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
+-rw-r--r--   0        0        0     2527 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
+-rw-r--r--   0        0        0     5892 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
+-rw-r--r--   0        0        0     2394 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
+-rw-r--r--   0        0        0     2197 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/model.py
+-rw-r--r--   0        0        0     1553 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
+-rw-r--r--   0        0        0     1448 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service.py
+-rw-r--r--   0        0        0     1196 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service_model.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/__init__.py
+-rw-r--r--   0        0        0    10604 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/analyzer.py
+-rw-r--r--   0        0        0       71 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
+-rw-r--r--   0        0        0      369 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
+-rw-r--r--   0        0        0      272 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
+-rw-r--r--   0        0        0      313 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
+-rw-r--r--   0        0        0     2404 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
+-rw-r--r--   0        0        0      822 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/deployment.py
+-rw-r--r--   0        0        0     2687 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/exporter.py
+-rw-r--r--   0        0        0     1891 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/model.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    12836 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
+-rw-r--r--   0        0        0      389 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
+-rw-r--r--   0        0        0       20 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
+-rw-r--r--   0        0        0       11 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
+-rw-r--r--   0        0        0      535 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
+-rw-r--r--   0        0        0     5827 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/exporter.py
+-rw-r--r--   0        0        0     4685 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/model.py
+-rw-r--r--   0        0        0     1048 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/service.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/errors/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/errors/failed_connection_errors.py
+-rw-r--r--   0        0        0     7158 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/main.py
+-rw-r--r--   0        0        0      195 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/models/__init__.py
+-rw-r--r--   0        0        0     7583 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/models/model.py
+-rw-r--r--   0        0        0        0 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/utils/__init__.py
+-rw-r--r--   0        0        0      651 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/utils/logger.py
+-rw-r--r--   0        0        0      452 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/base_writers.py
+-rw-r--r--   0        0        0      728 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/csv_writer.py
+-rw-r--r--   0        0        0     1138 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/get_writers.py
+-rw-r--r--   0        0        0     2090 2023-07-05 09:51:27.787414 udps-0.1.20/universal_data_permissions_scanner/writers/multi_json_exporter.py
+-rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 udps-0.1.20/PKG-INFO
```

### Comparing `udps-0.1.19/LICENSE` & `udps-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/README.md` & `udps-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/pyproject.toml` & `udps-0.1.20/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "udps"
-version = "0.1.19"
+version = "0.1.20"
 homepage = "https://github.com/satoricyber/universal-data-permissions-scanner"
 description = "Analyze authorization."
 authors = ["SatoriCyber"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
@@ -19,15 +19,15 @@
     { include = "universal_data_permissions_scanner" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 click = "8.1.3"
-snowflake-connector-python = "=3.0.0"
+snowflake-connector-python = "=3.0.2"
 google-cloud-bigquery = ">=2.1.0,<3.0"
 google-cloud-resource-manager = ">=1.6.3,<2.0"
 google-api-python-client = "~2.66.0"
 boto3 = "^1.26.27"
 pydantic = "^1.10.2"
 networkx = "^2.8.8"
 pyserde = "^0.9.6"
```

### Comparing `udps-0.1.19/tests/mocks/mock_writers.py` & `udps-0.1.20/tests/mocks/mock_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/test_authz_analyzer.py` & `udps-0.1.20/tests/test_authz_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/test_cli.py` & `udps-0.1.20/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,24 +170,32 @@
         'project1',
         '--cluster',
         'cluster1',
     ]
     invoke(cli.atlas, args)
 
 
+@pytest.mark.parametrize(
+    'additional_args',
+    [
+        ['--username', 'user1', '--password', 'abc123'],
+        ['--client_id', "client_id", '--client_secret', 'client_secret', '--tenant_id', 'tenant_id'],
+    ],
+    ids=[
+        'username password',
+        'oauth azure',
+    ],
+)
 @patch('universal_data_permissions_scanner.cli.run_databricks', MagicMock())
-def test_databricks():
+def test_databricks(additional_args: List[str]):
     args = [
-        '--username',
-        'user1',
-        '--password',
-        'password',
         '--host',
         'host',
     ]
+    args.extend(additional_args)
     invoke(cli.databricks, args)
 
 
 def invoke(command: Callable[[List[str]], None], args: List[str]):
     runner = CliRunner()
     result = runner.invoke(command, args, obj=generate_obj())  # type: ignore
     assert result.exit_code == 0, result.output
```

### Comparing `udps-0.1.19/tests/test_writers/test_csv_writer.py` & `udps-0.1.20/tests/test_writers/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/test_writers/test_multijson_writer.py` & `udps-0.1.20/tests/test_writers/test_multijson_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py` & `udps-0.1.20/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json` & `udps-0.1.20/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/test_exporter.py` & `udps-0.1.20/tests/tests_datastores/aws/test_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py` & `udps-0.1.20/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/bigquery/generate_authz_entry.py` & `udps-0.1.20/tests/tests_datastores/bigquery/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/bigquery/mocks.py` & `udps-0.1.20/tests/tests_datastores/bigquery/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/bigquery/test_bigquery.py` & `udps-0.1.20/tests/tests_datastores/bigquery/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/databricks/generate_authz_entry.py` & `udps-0.1.20/tests/tests_datastores/databricks/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/databricks/mocks.py` & `udps-0.1.20/tests/tests_datastores/databricks/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/databricks/test_analyzer.py` & `udps-0.1.20/tests/tests_datastores/databricks/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/mongodb/test_atlas_organization_users.py` & `udps-0.1.20/tests/tests_datastores/mongodb/test_atlas_organization_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/mongodb/test_mongodb.py` & `udps-0.1.20/tests/tests_datastores/mongodb/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py` & `udps-0.1.20/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/postgres/test_postgress_analyzer.py` & `udps-0.1.20/tests/tests_datastores/postgres/test_postgress_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/redshift/test_redshift.py` & `udps-0.1.20/tests/tests_datastores/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/tests/tests_datastores/snowflake/test_snowflake_analyzer.py` & `udps-0.1.20/tests/tests_datastores/snowflake/test_snowflake_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,25 +378,49 @@
                 "ACCOUNTADMIN",
                 "",
                 "",
             ),
             GrantsShare(
                 "2023-01-22 05:03:55.849 -0800",
                 "USAGE",
+                "FUNCTION",
+                "FUNC1",
+                "SHARE",
+                "PDA02239.SHARE1",
+                "false",
+                "ACCOUNTADMIN",
+            ),
+            [],
+            [],
+        ),
+        (  # test 5
+            Share(
+                "2023-01-22T05:03:45.169-08:00",
+                "OUTBOUND",
+                "OUGNBIN.PDA02239.SHARE1",
+                "DB1",
+                "ACCOUNT1",
+                "ACCOUNTADMIN",
+                "",
+                "",
+            ),
+            GrantsShare(
+                "2023-01-22 05:03:55.849 -0800",
+                "USAGE",
                 "DATABASE_ROLE",
                 "DB1.ROLE_SHARE",
                 "SHARE",
                 "PDA02239.SHARE1",
                 "false",
                 "ACCOUNTADMIN",
             ),
             [],
             [],
         ),
-        (  # test 4
+        (  # test 6
             Share(
                 "2023-01-22T05:03:45.169-08:00",
                 "OUTBOUND",
                 "OUGNBIN.PDA02239.SHARE1",
                 "DB1",
                 "ACCOUNT1",
                 "ACCOUNTADMIN",
@@ -445,14 +469,15 @@
             ],
         ),
     ],
     ids=(
         "Outbound share no account",
         "No relevant permissions",  # We grant usage permission on database, but no access to data
         "Outbound simple share",
+        "Outbound simple share ignore for function",
         "Share with database user with no access",
         "Share with database user with access",
     ),
 )
 def test_snowflake_analyzer_shares(
     share: Share, grant_share: GrantsShare, roles: List[RoleGrant], expected_writes: List[AuthzEntry]
 ):
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/__init__.py` & `udps-0.1.20/universal_data_permissions_scanner/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for authz-analyzer."""
 
 __author__ = """SatoriCyber"""
 __email__ = 'contact@satoricyber.com'
-__version__ = '0.1.19'
+__version__ = '0.1.20'
 
 from universal_data_permissions_scanner.datastores.aws.analyzer import AwsAssumeRoleInput, AWSAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.aws.analyzer.redshift.analyzer import RedshiftAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.bigquery.analyzer import BigQueryAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.analyzer import MongoDBAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.atlas.analyzer import MongoDBAtlasAuthzAnalyzer  # type: ignore
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/cli.py` & `udps-0.1.20/universal_data_permissions_scanner/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import re
 import sys
 from pathlib import Path
 from typing import List, Optional, TextIO
 
 import click
 
+from universal_data_permissions_scanner.datastores.databricks import (
+    Authentication,
+)
+
 if sys.executable != sys.argv[0]:
     sys.path.insert(0, (os.path.join(os.path.dirname(__file__), "..")))
 
 
 from universal_data_permissions_scanner import AwsAssumeRoleInput  # pylint: disable=wrong-import-position
 from universal_data_permissions_scanner.main import (  # pylint: disable=wrong-import-position
     run_aws_s3,
@@ -67,15 +71,15 @@
 @click.option('--warehouse', '-w', required=False, type=str, help="Warehouse")
 def snowflake(
     ctx: click.Context,
     username: str,
     password: Optional[str],
     account: str,
     host: str,
-    warehouse: str,
+    warehouse: Optional[str],
     rsa_key: Optional[TextIO],
     rsa_pass: Optional[str],
 ):
     """Analyze Snowflake Authorization"""
     if not any([password, rsa_key]):
         click.echo('Error: Required at least one of the options: --password / -p or --rsa / -r')
         return
@@ -258,35 +262,54 @@
 
 
 @main.command()
 @click.pass_context
 @click.option(
     '--username',
     '-u',
-    required=True,
+    required=False,
     type=str,
     help="Databricks account admin username",
 )
 @click.option(
     '--password',
     '-p',
-    required=True,
+    required=False,
     type=str,
     help="Databricks account admin password",
 )
+@click.option('--client_id', '-cid', required=False, type=str, help="Client ID for ouath2")
+@click.option('--client_secret', '-cis', required=False, type=str, help="Client Secret for ouath2")
+@click.option('--tenant_id', '-tid', required=False, type=str, help="Tenant ID for Azure Oauth")
 @click.option(
     '--host', '-h', required=True, type=str, help="workspace host, e.g. https://<workspace>.cloud.databricks.com"
 )
-def databricks(ctx: click.Context, host: str, username: str, password: str):
+def databricks(
+    ctx: click.Context,
+    host: str,
+    username: Optional[str],
+    password: Optional[str],
+    client_id: Optional[str],
+    client_secret: Optional[str],
+    tenant_id: Optional[str],
+):
     """Analyze databricks Authorization"""
+    if (username is not None) and (password is not None):
+        authentication = Authentication.basic(username=username, password=password)
+    elif (client_id is not None) and (client_secret is not None) and (tenant_id is not None):
+        authentication = Authentication.oauth_azure(
+            client_id=client_id, client_secret=client_secret, tenant_id=tenant_id
+        )
+    else:
+        raise ValueError("Either username and password or client_id, client_secret and tenant_id must be provided")
+
     run_databricks(
         logger=ctx.obj['LOGGER'],
         output_format=ctx.obj['FORMAT'],
         output_path=ctx.obj['OUT'],
         host=host,
-        username=username,
-        password=password,
+        authentication=authentication,
     )
 
 
 if __name__ == "__main__":
     main(obj={})  # pylint: disable=no-value-for-parameter
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/__init__.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/bigquery/service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/bigquery/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,53 +15,74 @@
     Table,
 )
 from universal_data_permissions_scanner.datastores.databricks.service.scim import ScimService
 from universal_data_permissions_scanner.utils.logger import get_logger
 from universal_data_permissions_scanner.writers.base_writers import DEFAULT_OUTPUT_FILE, BaseWriter, OutputFormat
 from universal_data_permissions_scanner.writers.get_writers import get_writer
 
+from universal_data_permissions_scanner.datastores.databricks.service.authentication import (
+    Authentication,
+)
+
+
+from universal_data_permissions_scanner.datastores.databricks.service.authentication.basic import BasicAuthentication
+
+from universal_data_permissions_scanner.datastores.databricks.service.authentication.oauth import (
+    OauthProvider,
+    get_authentication_token,
+)
+
 
 @dataclass
 class DatabricksAuthzAnalyzer:
     writer: BaseWriter
     logger: Logger
     unity_catalog_service: UnityCatalogService
     scim_service: ScimService
     metastore_id: Optional[str] = None
 
     @classmethod
     def connect(
         cls,
         host: str,
-        username: str,
-        password: str,
+        authentication: Authentication,
         metastore_id: Optional[str] = None,
         output_format: OutputFormat = OutputFormat.CSV,
         output_path: Union[Path, str] = Path.cwd() / DEFAULT_OUTPUT_FILE,
         logger: Optional[Logger] = None,
         **kwargs: Any,
     ):
         """Analyzer authorization for Databricks
 
         Args:
             host (str): instance url, e.g. https://dbc-a1b2345c-d6e7.cloud.databricks.com
-            username (str): An account admin user name which has permission on the metastore as well.
-            password (str): Password for the user.
+            authentication: Authentication method, either basic or oauth
             output_format (OutputFormat, optional): Output format. Defaults to OutputFormat.CSV.
             output_path (Union[Path, str], optional): Output path. Defaults to Path.cwd()/DEFAULT_OUTPUT_FILE.
             logger (Optional[Logger], optional): Logger. Defaults to None.
 
         Returns:
             cls: instance
         """
         writer = get_writer(filename=output_path, output_format=output_format)
         if logger is None:
             logger = get_logger(False)
         logger.debug("Connecting to Databricks instance at %s", host)
-        api_client = ApiClient(host=host, user=username, password=password, **kwargs)
+        if isinstance(authentication.authentication, BasicAuthentication):
+            api_client = ApiClient(
+                host=host,
+                user=authentication.authentication.username,
+                password=authentication.authentication.password,
+                **kwargs,
+            )
+        elif isinstance(authentication.authentication, OauthProvider):  # type: ignore
+            token = get_authentication_token(authentication.authentication)
+            api_client = ApiClient(host=host, token=token, **kwargs)
+        else:
+            raise ValueError("Unknown authentication method")
         unity_catalog_service = UnityCatalogService(api_client)
         scim_service = ScimService(api_client)
         return cls(
             writer=writer,
             logger=logger,
             unity_catalog_service=unity_catalog_service,
             scim_service=scim_service,
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/identities.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/identities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/policy_tree.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/service/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/databricks/service/scim.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/databricks/service/scim.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/resolvers.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/mongodb/service_model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/mongodb/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/database_query_results.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/database_query_results.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/deployment.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/deployment.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/exporter.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/postgres/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/postgres/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/analyzer.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     @classmethod
     def connect(  # pylint: disable=too-many-locals
         cls,
         host: str,
         account: str,
         username: str,
-        warehouse: str,
+        warehouse: Optional[str],
         logger: Optional[Logger] = None,
         output_format: OutputFormat = OutputFormat.CSV,
         output_path: Union[Path, str] = Path.cwd() / DEFAULT_OUTPUT_FILE,
         rsa_key: Optional[str] = None,
         rsa_pass: Optional[str] = None,
         **snowflake_connection_kwargs: Any,
     ):
@@ -91,15 +91,16 @@
         """
         if logger is None:
             logger = get_logger(False)
 
         writer = get_writer(filename=output_path, output_format=output_format)
 
         # Handle case sensitive warehouse name, wrap with quotes
-        warehouse = f'"{warehouse}"'
+        if warehouse is not None:
+            warehouse = f'"{warehouse}"'
 
         if rsa_key is not None:
             snowflake_connection_kwargs["private_key"] = SnowflakeAuthzAnalyzer._read_private_key(rsa_key, rsa_pass)
 
         try:
             connector = snowflake.connector.connect(  # type: ignore
                 user=username,
@@ -287,15 +288,20 @@
         for row in rows:
             try:
                 database_permission = PermissionType(row[1])
             except ValueError:
                 self.logger.debug("Privilege doesn't grant permission to data, skipping privilege %s", row[1])
                 continue
 
-            granted_on = GrantedOn(row[2])
+            try:
+                granted_on = GrantedOn(row[2])
+            except ValueError:
+                self.logger.warning("Unknown granted on %s", row[2])
+                continue
+
             resource_name: List[str] = row[3].split(".")
             if granted_on is GrantedOn.DATABASE_ROLE and database_permission is PermissionType.USAGE:
                 on_role(DBRole(resource_name[-1], set()))
             else:
                 try:
                     permission_level = PERMISSION_LEVEL_MAP[database_permission]
                 except KeyError:
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql` & `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/exporter.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/model.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/datastores/snowflake/service.py` & `udps-0.1.20/universal_data_permissions_scanner/datastores/snowflake/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/main.py` & `udps-0.1.20/universal_data_permissions_scanner/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,24 @@
     PostgresAuthzAnalyzer,
     RedshiftAuthzAnalyzer,
     SnowflakeAuthzAnalyzer,
 )
 from universal_data_permissions_scanner.writers import OutputFormat, get_writer
 
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer
+from universal_data_permissions_scanner.datastores.databricks import Authentication
 
 
 def run_snowflake(
     logger: Logger,
     username: str,
     password: Optional[str],
     account: str,
     host: str,
-    warehouse: str,
+    warehouse: Optional[str],
     output_format: OutputFormat,
     output_path: Path,
     rsa_key: Optional[str],
     rsa_pass: Optional[str],
 ):
     """Run snowflake analyzer.
 
@@ -232,30 +233,29 @@
     )
     analyzer.run()
 
 
 def run_databricks(
     logger: Logger,
     host: str,
-    username: str,
-    password: str,
+    authentication: Authentication,
     output_format: OutputFormat,
     output_path: Path,
 ):
     """Run Databricks analyzer.
 
     Args:
         logger (Logger): Logger
         host (str): workspace host, e.g. https://<workspace>.cloud.databricks.com
         key (str): Databricks API key
         output_format (OutputFormat): Output format, CSV or JSON
         output_path (str): Where to write the output
+        authentication: Authentication method
     """
     analyzer = DatabricksAuthzAnalyzer.connect(
         host=host,
-        username=username,
-        password=password,
+        authentication=authentication,
         output_path=output_path,
         output_format=output_format,
         logger=logger,
     )
     analyzer.run()
```

### Comparing `udps-0.1.19/universal_data_permissions_scanner/models/model.py` & `udps-0.1.20/universal_data_permissions_scanner/models/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/utils/logger.py` & `udps-0.1.20/universal_data_permissions_scanner/utils/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/writers/base_writers.py` & `udps-0.1.20/universal_data_permissions_scanner/writers/base_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/writers/csv_writer.py` & `udps-0.1.20/universal_data_permissions_scanner/writers/csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/writers/get_writers.py` & `udps-0.1.20/universal_data_permissions_scanner/writers/get_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/universal_data_permissions_scanner/writers/multi_json_exporter.py` & `udps-0.1.20/universal_data_permissions_scanner/writers/multi_json_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.19/PKG-INFO` & `udps-0.1.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udps
-Version: 0.1.19
+Version: 0.1.20
 Summary: Analyze authorization.
 Home-page: https://github.com/satoricyber/universal-data-permissions-scanner
 Author: SatoriCyber
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -40,15 +40,15 @@
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: pyright (>=1.1.293,<2.0.0) ; extra == "test"
 Requires-Dist: pyserde (>=0.9.6,<0.10.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "test"
 Requires-Dist: redshift-connector (>=2.0.909,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: snowflake-connector-python (==3.0.0)
+Requires-Dist: snowflake-connector-python (==3.0.2)
 Requires-Dist: tox (>=4.0.14,<5.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0) ; extra == "test" or extra == "release"
 Requires-Dist: types-psycopg2 (>=2.9.21.2,<3.0.0.0) ; extra == "test"
 Requires-Dist: types-requests (>=2.28.11.7,<3.0.0.0) ; extra == "test"
 Requires-Dist: virtualenv (>=20.17.1,<21.0.0)
 Description-Content-Type: text/markdown
```

