# Comparing `tmp/credsweeper-1.5.1.tar.gz` & `tmp/credsweeper-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.5.1.tar", last modified: Wed Jun 21 11:06:13 2023, max compression
+gzip compressed data, was "credsweeper-1.5.2.tar", last modified: Wed Jul  5 10:25:15 2023, max compression
```

## Comparing `credsweeper-1.5.1.tar` & `credsweeper-1.5.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 11:05:58.000000 credsweeper-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-21 11:06:13.265659 credsweeper-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-21 11:05:58.000000 credsweeper-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.221659 credsweeper-1.5.1/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.225659 credsweeper-1.5.1/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.229659 credsweeper-1.5.1/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.229659 credsweeper-1.5.1/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.237659 credsweeper-1.5.1/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.241659 credsweeper-1.5.1/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.257659 credsweeper-1.5.1/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/cred_card_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.257659 credsweeper-1.5.1/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/structured_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_entropy_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_pem_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_structured_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.261659 credsweeper-1.5.1/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22458 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 11:05:58.000000 credsweeper-1.5.1/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.225659 credsweeper-1.5.1/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 11:06:13.000000 credsweeper-1.5.1/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 11:06:13.265659 credsweeper-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-21 11:05:58.000000 credsweeper-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:06:13.265659 credsweeper-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-06-21 11:05:59.000000 credsweeper-1.5.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    43633 2023-06-21 11:05:59.000000 credsweeper-1.5.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 10:25:04.000000 credsweeper-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-05 10:25:15.929459 credsweeper-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-05 10:25:04.000000 credsweeper-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.885458 credsweeper-1.5.2/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.893458 credsweeper-1.5.2/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.897459 credsweeper-1.5.2/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.901459 credsweeper-1.5.2/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.917459 credsweeper-1.5.2/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/cred_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.917459 credsweeper-1.5.2/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/structured_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_pem_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_structured_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.921459 credsweeper-1.5.2/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.925459 credsweeper-1.5.2/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21920 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-05 10:25:04.000000 credsweeper-1.5.2/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.889459 credsweeper-1.5.2/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 10:25:15.000000 credsweeper-1.5.2/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 10:25:15.933459 credsweeper-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-05 10:25:04.000000 credsweeper-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 10:25:15.929459 credsweeper-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30506 2023-07-05 10:25:04.000000 credsweeper-1.5.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43642 2023-07-05 10:25:04.000000 credsweeper-1.5.2/tests/test_main.py
```

### Comparing `credsweeper-1.5.1/LICENSE` & `credsweeper-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/PKG-INFO` & `credsweeper-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.1
+Version: 1.5.2
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.1/README.md` & `credsweeper-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/__init__.py` & `credsweeper-1.5.2/credsweeper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
```

### Comparing `credsweeper-1.5.1/credsweeper/__main__.py` & `credsweeper-1.5.2/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/app.py` & `credsweeper-1.5.2/credsweeper/app.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/common/constants.py` & `credsweeper-1.5.2/credsweeper/common/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,18 @@
     BASE64_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/="
     # URL- and filename-safe standard
     BASE64URL_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_"
     # standard base64
     BASE64STD_CHARS = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
 
 
+ENTROPY_LIMIT_BASE64 = 4.5
+ENTROPY_LIMIT_BASE3x = 3
+
+
 class KeyValidationOption(Enum):
     """API validation state"""
     INVALID_KEY = 0
     VALIDATED_KEY = 1
     UNDECIDED = 2
     NOT_AVAILABLE = 3
 
@@ -117,15 +121,15 @@
     ADDED_ACCOMPANY = "added_accompany"
     DELETED_ACCOMPANY = "deleted_accompany"
 
 
 MIN_VARIABLE_LENGTH = 1
 MIN_SEPARATOR_LENGTH = 1
 MIN_VALUE_LENGTH = 4
-MAX_LINE_LENGTH = 1500
+MAX_LINE_LENGTH = 2000
 """ values according https://docs.python.org/3/library/codecs.html """
 UTF_8 = "utf_8"
 UTF_16 = "utf_16"
 LATIN_1 = "latin_1"
 
 DEFAULT_ENCODING = UTF_8
 
@@ -136,7 +140,11 @@
 RECURSIVE_SCAN_LIMITATION = 1 << 30
 
 # default value for config and ValuePatternCheck
 DEFAULT_PATTERN_LEN = 4
 
 # default value for config and ValuePemPatternCheck
 DEFAULT_PEM_PATTERN_LEN = 5
+
+# PEM x509 patterns
+PEM_BEGIN_PATTERN = "-----BEGIN"
+PEM_END_PATTERN = "-----END"
```

### Comparing `credsweeper-1.5.1/credsweeper/common/keyword_checklist.py` & `credsweeper-1.5.2/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.5.2/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.5.2/credsweeper/common/morpheme_checklist.txt`

 * *Files 1% similar despite different names*

```diff
@@ -440,16 +440,15 @@
 dig
 dimen
 ding
 diod
 dir_
 direct
 disab
-discipl
-discon
+disc
 disk
 dismi
 dispos
 dissoc
 dist
 ditor
 dity
@@ -948,14 +947,15 @@
 numer
 nuous
 nvram
 obj
 oblique
 occur
 ocean
+ocess
 oder
 off
 often
 oken
 oker
 old
 olygon
@@ -1048,15 +1048,15 @@
 prim
 princip
 prior
 priv
 pro_
 probe
 problem
-process
+proc
 prod
 prof
 prog
 proj
 promise
 prompt
 prop
@@ -1200,17 +1200,20 @@
 savi
 scala
 scale
 scali
 scen
 sched
 schem
+scipl
+scont
 scope
 scram
 screen
+scret
 scri
 scro
 seal
 searc
 seccomp
 second
 secre
```

### Comparing `credsweeper-1.5.1/credsweeper/config/config.py` & `credsweeper-1.5.2/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.5.2/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/candidate.py` & `credsweeper-1.5.2/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.5.2/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/candidate_key.py` & `credsweeper-1.5.2/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/credential_manager.py` & `credsweeper-1.5.2/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/credentials/line_data.py` & `credsweeper-1.5.2/credsweeper/credentials/line_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from functools import cached_property
 from typing import Any, Dict, Optional, Tuple
 
 from credsweeper.config import Config
 from credsweeper.utils import Util
+from credsweeper.utils.entropy_validator import EntropyValidator
 
 
 class LineData:
     """Object to treat and store scanned line related data.
 
     Parameters:
         key: Optional[str] = None
@@ -292,15 +293,15 @@
             return False
         if Util.get_extension(self.path) in self.config.source_quote_ext:
             return True
         return False
 
     def __repr__(self) -> str:
         return f"line: '{self.line}' / line_num: {self.line_num} / path: {self.path} " \
-               f"/ value: '{self.value}' / entropy_validation: {Util.is_entropy_validate(self.value)}"
+               f"/ value: '{self.value}' / entropy_validation: {EntropyValidator(self.value)}"
 
     def to_json(self) -> Dict:
         """Convert line data object to dictionary.
 
         Return:
             Dictionary object generated from current line data
 
@@ -314,11 +315,11 @@
             "pattern": self.pattern.pattern,
             "separator": self.separator,
             "separator_span": self.separator_span,
             "value": self.value,
             "variable": self.variable,
             "value_leftquote": self.value_leftquote,
             "value_rightquote": self.value_rightquote,
-            "entropy_validation": Util.is_entropy_validate(self.value)
+            "entropy_validation": EntropyValidator(self.value).to_dict()
         }
         reported_output = {k: v for k, v in full_output.items() if k in self.config.line_data_output}
         return reported_output
```

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/deep_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.5.2/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/__init__.py` & `credsweeper-1.5.2/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.5.2/credsweeper/file_handler/analysis_target.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.5.2/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/files_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/patch_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/file_handler/text_provider.py` & `credsweeper-1.5.2/credsweeper/file_handler/text_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/__init__.py` & `credsweeper-1.5.2/credsweeper/filters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from credsweeper.filters.value_camel_case_check import ValueCamelCaseCheck
 from credsweeper.filters.value_couple_keyword_check import ValueCoupleKeywordCheck
 from credsweeper.filters.value_dictionary_keyword_check import ValueDictionaryKeywordCheck
 from credsweeper.filters.value_dictionary_value_length_check import ValueDictionaryValueLengthCheck
 from credsweeper.filters.value_entropy_base32_check import ValueEntropyBase32Check
 from credsweeper.filters.value_entropy_base36_check import ValueEntropyBase36Check
 from credsweeper.filters.value_entropy_base64_check import ValueEntropyBase64Check
-from credsweeper.filters.value_entropy_check import ValueEntropyCheck
 from credsweeper.filters.value_file_path_check import ValueFilePathCheck
 from credsweeper.filters.value_first_word_check import ValueFirstWordCheck
 from credsweeper.filters.value_grafana_check import ValueGrafanaCheck
 from credsweeper.filters.value_json_web_token_check import ValueJsonWebTokenCheck
 from credsweeper.filters.value_last_word_check import ValueLastWordCheck
 from credsweeper.filters.value_length_check import ValueLengthCheck
 from credsweeper.filters.value_method_check import ValueMethodCheck
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/cred_card_number_check.py` & `credsweeper-1.5.2/credsweeper/filters/cred_card_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/filter.py` & `credsweeper-1.5.2/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/__init__.py` & `credsweeper-1.5.2/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/group.py` & `credsweeper-1.5.2/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.5.2/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.5.2/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.5.2/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.5.2/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.5.2/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.5.2/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_entropy_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_length_check.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
-from credsweeper.utils import Util
 
 
-class ValueEntropyCheck(Filter):
-    """Check that candidate have Shanon Entropy > 3 (for HEX_CHARS or BASE36_CHARS) or > 4.5 (for BASE64_CHARS)."""
+class ValueLengthCheck(Filter):
+    """Check if potential candidate value is not too short (longer or equal to `min_len`)."""
 
-    def __init__(self, config: Config = None) -> None:
-        pass
+    def __init__(self, config: Config) -> None:
+        self.min_len = config.min_keyword_value_length
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
             target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        return not Util.is_entropy_validate(line_data.value)
+        if len(line_data.value) < self.min_len:
+            return True
+        return False
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_length_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_method_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+import re
+
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueLengthCheck(Filter):
-    """Check if potential candidate value is not too short (longer or equal to `min_len`)."""
+class ValueMethodCheck(Filter):
+    """Check if potential candidate value is a function.
+
+    Check if potential candidate value is a function by looking for '(', ')' or 'function' sub-strings in it
+    """
+
+    PATTERN = re.compile(".*\\(.*\\).*")
 
-    def __init__(self, config: Config) -> None:
-        self.min_len = config.min_keyword_value_length
+    def __init__(self, config: Config = None) -> None:
+        pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
         Args:
             line_data: credential candidate data
             target: multiline target from which line data was obtained
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        if len(line_data.value) < self.min_len:
+        if "function" in line_data.value or self.PATTERN.search(line_data.value):
             return True
         return False
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_method_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_token_base32_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-import re
+from password_strength import PasswordStats
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueMethodCheck(Filter):
-    """Check if potential candidate value is a function.
-
-    Check if potential candidate value is a function by looking for '(', ')' or 'function' sub-strings in it
-    """
-
-    PATTERN = re.compile(".*\\(.*\\).*")
+class ValueTokenBase32Check(Filter):
+    """Check that candidate have good randomization"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
@@ -26,10 +21,22 @@
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        if "function" in line_data.value or self.PATTERN.search(line_data.value):
-            return True
-        return False
+
+        strength = float(PasswordStats(line_data.value).strength())
+        min_strength = ValueTokenBase32Check.get_min_strength(len(line_data.value))
+        return min_strength > strength
+
+    @staticmethod
+    def get_min_strength(x: int) -> float:
+        """Returns minimal strength. Precalculated data is applied for speedup"""
+        if 16 == x:
+            y = 0.7047
+        elif 8 <= x <= 32:
+            y = ((0.000046 * x - 0.0044) * x + 0.146) * x - 0.7
+        else:
+            y = 1
+        return y
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_number_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_pem_pattern_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_pem_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_structured_token_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_structured_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_token_base36_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueTokenBase32Check(Filter):
+class ValueTokenBase36Check(Filter):
     """Check that candidate have good randomization"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
@@ -23,20 +23,25 @@
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
 
         strength = float(PasswordStats(line_data.value).strength())
-        min_strength = ValueTokenBase32Check.get_min_strength(len(line_data.value))
+        min_strength = ValueTokenBase36Check.get_min_strength(len(line_data.value))
         return min_strength > strength
 
     @staticmethod
     def get_min_strength(x: int) -> float:
         """Returns minimal strength. Precalculated data is applied for speedup"""
-        if 16 == x:
-            y = 0.7047
+        if 15 == x:
+            y = 0.66
+        elif 24 == x:
+            y = 0.9
+        elif 25 == x:
+            y = 0.9
         elif 8 <= x <= 32:
-            y = ((0.000046 * x - 0.0044) * x + 0.146) * x - 0.7
+            # approximation not exceed standard deviation
+            y = ((0.000067 * x - 0.00571) * x + 0.1718) * x - 0.86
         else:
             y = 1
         return y
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_token_base64_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueTokenBase36Check(Filter):
+class ValueTokenBase64Check(Filter):
     """Check that candidate have good randomization"""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
@@ -23,25 +23,26 @@
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
 
         strength = float(PasswordStats(line_data.value).strength())
-        min_strength = ValueTokenBase36Check.get_min_strength(len(line_data.value))
+        min_strength = ValueTokenBase64Check.get_min_strength(len(line_data.value))
         return min_strength > strength
 
     @staticmethod
     def get_min_strength(x: int) -> float:
-        """Returns minimal strength. Precalculated data is applied for speedup"""
-        if 15 == x:
-            y = 0.66
+        """Returns minimal strength. Precalculated rounded data is applied for speedup"""
+        if 18 == x:
+            y = 0.7
+        elif 20 == x:
+            y = 0.8
         elif 24 == x:
             y = 0.9
-        elif 25 == x:
+        elif 32 == x:
             y = 0.9
-        elif 8 <= x <= 32:
-            # approximation not exceed standard deviation
-            y = ((0.000067 * x - 0.00571) * x + 0.1718) * x - 0.86
+        elif x < 40:
+            y = ((0.0000405 * x - 0.004117) * x + 0.141) * x - 0.65
         else:
             y = 1
         return y
```

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_token_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.5.2/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.5.2/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/logger/logger.py` & `credsweeper-1.5.2/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/ml_model/features.py` & `credsweeper-1.5.2/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.5.2/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.5.2/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/ml_model/model_config.json` & `credsweeper-1.5.2/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/rules/config.yaml` & `credsweeper-1.5.2/credsweeper/rules/config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -22,29 +22,29 @@
   usage_list:
     - src
 
 - name: AWS Client ID
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - A
   min_line_len: 20
   usage_list:
     - src
     - doc
 
 - name: AWS Multi
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
     - (?P<value>[0-9a-zA-Z/+]{40})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - AKIA
     - ASIA
   min_line_len: 20
@@ -52,15 +52,15 @@
     - src
     - doc
 
 - name: AWS MWS Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>amzn\.mws\.[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>amzn\.mws\.[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - amzn
   min_line_len: 30
   usage_list:
     - src
@@ -79,29 +79,29 @@
   usage_list:
     - src
 
 - name: Dynatrace API Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>dt0[a-zA-Z]{1}[0-9]{2}\.[A-Z0-9]{24}\.[A-Z0-9]{64})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>dt0[a-zA-Z]{1}[0-9]{2}\.[A-Z0-9]{24}\.[A-Z0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - dt0
   min_line_len: 90
   usage_list:
     - src
     - doc
 
 - name: Facebook Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>EAAC[0-9A-Za-z]{27,})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>EAAC[0-9A-Za-z]{27,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - EAAC
   min_line_len: 31
   usage_list:
     - src
@@ -123,15 +123,15 @@
     - src
     - doc
 
 - name: Google API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>AIza[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>AIza[0-9A-Za-z_-]{35})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - GoogleApiKeyValidation
   required_substrings:
     - AIza
   min_line_len: 39
@@ -156,15 +156,15 @@
     - src
     - doc
 
 - name: Google OAuth Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ya29\.[0-9A-Za-z_-]{22,})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>ya29\.[0-9A-Za-z_-]{22,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - ya29.
   min_line_len: 27
   usage_list:
     - src
@@ -184,43 +184,43 @@
     - src
     - doc
 
 - name: Instagram Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>IGQVJ[\w]{100,})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>IGQVJ[\w]{100,})
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - IGQVJ
   min_line_len: 105
   usage_list:
     - src
     - doc
 
 - name: JSON Web Token
   severity: medium
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>eyJ[A-Za-z0-9=_-]{13,}(\.[A-Za-z0-9-_.+\/=]+)?)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>eyJ[A-Za-z0-9=_-]{13,}(\.[A-Za-z0-9-_.+\/=]+)?)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - eyJ
   min_line_len: 16
   usage_list:
     - src
     - doc
 
 - name: MailChimp API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>[0-9a-zA-Z]{32}-us[0-9]{1,2})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[0-9a-zA-Z]{32}-us[0-9]{1,2})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: false
   validations:
     - MailChimpKeyValidation
   required_substrings:
     - -us
   min_line_len: 35
@@ -228,15 +228,15 @@
     - src
     - doc
 
 - name: MailGun API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>key-[0-9a-zA-Z]{32})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>key-[0-9a-zA-Z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - key-
   min_line_len: 36
   usage_list:
     - src
@@ -266,24 +266,25 @@
   required_substrings:
     - access_token$production$
   min_line_len: 72
   usage_list:
     - src
     - doc
 
-- name: PEM Certificate
+- name: PEM Private Key
   severity: high
   type: pem_key
   values:
-    - (?P<value>-----BEGIN\s(?!ENCRYPTED|EC).*PRIVATE)
+    - (?P<value>-----BEGIN\s(?!ENCRYPTED|EC)[^-]*PRIVATE[^-]*KEY[^-]*-----(.+-----END[^-]+-----)?)
   filter_type:
     - LineSpecificKeyCheck
-  min_line_len: 20
+  min_line_len: 27
   usage_list:
     - src
+    - doc
 
 - name: Picatic API Key
   severity: high
   type: pattern
   values:
     - (?P<value>sk_live_[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
@@ -335,15 +336,15 @@
     - src
     - doc
 
 - name: Slack Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>xox[a|b|p|r|o|s]\-[-a-zA-Z0-9]{10,250})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>xox[a|b|p|r|o|s]\-[-a-zA-Z0-9]{10,250})
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SlackTokenValidation
   required_substrings:
     - xox
   min_line_len: 15
@@ -395,15 +396,15 @@
     - src
     - doc
 
 - name: Square Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>EAAA[0-9A-Za-z_-]{60})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>EAAA[0-9A-Za-z_-]{60})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareAccessTokenValidation
   required_substrings:
     - EAAA
   min_line_len: 64
@@ -411,15 +412,15 @@
     - src
     - doc
 
 - name: Square Client ID
   severity: medium
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>sq0[a-z]{3}-[0-9A-Za-z_-]{22})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>sq0[a-z]{3}-[0-9A-Za-z_-]{22})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - SquareClientIdValidation
   required_substrings:
     - sq0
   min_line_len: 29
@@ -454,15 +455,15 @@
   usage_list:
     - src
 
 - name: Twilio API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>SK[0-9a-fA-F]{32})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>SK[0-9a-fA-F]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - SK
   min_line_len: 34
   usage_list:
     - src
@@ -534,43 +535,43 @@
     - src
     - doc
 
 - name: Github Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>(ghr|gho|ghu|ghs)_[\w]{36,255})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>(ghr|gho|ghu|ghs)_[\w]{36,255})
   filter_type: GeneralPattern
   required_substrings:
     - gh
   min_line_len: 40
   usage_list:
     - src
     - doc
 
 - name: Github Personal Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ghp_[\w]{36,255})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>ghp_[\w]{36,255})
   filter_type: GeneralPattern
   validations:
     - GithubTokenValidation
   required_substrings:
     - ghp_
   min_line_len: 40
   usage_list:
     - src
     - doc
 
 - name: Github Fine-granted Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>github_pat_[0-9A-Za-z_]{80,255})
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>github_pat_[0-9A-Za-z_]{80,255})
   filter_type: GeneralPattern
   validations:
     - GithubTokenValidation
   required_substrings:
     - github_pat_
   min_line_len: 90
   usage_list:
@@ -657,306 +658,306 @@
     - src
     - doc
 
 - name: Azure Secret Value
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_~.-]{3}8Q~[a-zA-Z0-9_~.-]{34})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_~.-]{3}8Q~[a-zA-Z0-9_~.-]{34})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 40
   required_substrings:
     - 8Q~
   usage_list:
     - src
     - doc
 
 - name: Bitbucket App Password
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATBB[A-Za-z0-9]{24}[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>ATBB[A-Za-z0-9]{24}[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 28
   required_substrings:
     - ATBB
   usage_list:
     - src
     - doc
 
 - name: Bitbucket Repository Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATCTT3xFfGN0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>ATCTT3xFfGN0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 183
   required_substrings:
     - ATCTT3xFfGN0
   usage_list:
     - src
     - doc
 
 - name: Bitbucket HTTP Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>BBDC-[NMO][ADgjQTwz][A-Za-z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>BBDC-[NMO][ADgjQTwz][A-Za-z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 49
   required_substrings:
     - BBDC-
   usage_list:
     - src
     - doc
 
 - name: Bitbucket Client ID
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z.$_/+-])(?P<value>[a-zA-Z0-9]{18}([a-zA-Z0-9]{14})?)([^0-9A-Za-z.$_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{18}([a-zA-Z0-9]{14})?)([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 18
   usage_list:
     - src
     - doc
 
 - name: Bitbucket Client Secret
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z.$_/+-])(?P<value>([a-zA-Z0-9_-]{32}){1,2})([^0-9A-Za-z.$_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>([a-zA-Z0-9_-]{32}){1,2})([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 32
   usage_list:
     - src
     - doc
 
 - name: Jira / Confluence PAT token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z+/-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 44
   required_substrings:
     - M
     - N
     - O
   usage_list:
     - src
     - doc
 
 - name: Atlassian Old PAT token
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z.$_/+-])(?P<value>[a-zA-Z0-9]{24})([^=0-9A-Za-z.$_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{24})([^=0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 24
   usage_list:
     - src
     - doc
 
 - name: Atlassian PAT token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 191
   required_substrings:
     - ATATT3xFfGF0
   usage_list:
     - src
     - doc
 
 - name: Digital Ocean PAT
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>dop_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>dop_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - dop_v1_
   usage_list:
     - src
     - doc
 
 - name: Digital Ocean OAuth Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>doo_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>doo_v1_[a-f0-9]{64})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 71
   required_substrings:
     - doo_v1_
   usage_list:
     - src
     - doc
 
 - name: Dropbox OAuth2 API Access Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?P<value>sl.[A-Za-z0-9_-]{135})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>sl.[A-Za-z0-9_-]{135})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 138
   required_substrings:
     - sl.
   usage_list:
     - src
     - doc
 
 - name: NuGet API key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>oy2[a-z0-9]{43})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>oy2[a-z0-9]{43})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - oy2
   usage_list:
     - src
     - doc
 
 - name: Gitlab PAT
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glpat-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>glpat-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 26
   required_substrings:
     - glpat-
   usage_list:
     - src
     - doc
 
 - name: Gitlab Pipeline Trigger Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glptt-[a-f0-9]{40})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>glptt-[a-f0-9]{40})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 46
   required_substrings:
     - glptt-
   usage_list:
     - src
     - doc
 
 - name: Gitlab Registration Runner Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>GR1348941[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>GR1348941[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 29
   required_substrings:
     - GR1348941
   usage_list:
     - src
     - doc
 
 - name: Gitlab Registration Runner Token 2023
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glrt-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>glrt-[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
   min_line_len: 25
   required_substrings:
     - glrt-
   usage_list:
     - src
     - doc
 
 - name: Grafana Provisioned API Key
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>eyJ[a-zA-Z0-9=/-]{64,360})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>eyJ[a-zA-Z0-9=/-]{64,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 67
   required_substrings:
     - eyJ
   usage_list:
     - src
     - doc
 
 - name: Grafana Access Policy Token
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>glc_eyJ[a-zA-Z0-9=/-]{80,360})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>glc_eyJ[a-zA-Z0-9=/-]{80,360})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueGrafanaCheck
   min_line_len: 87
   required_substrings:
     - glc_eyJ
   usage_list:
     - src
     - doc
 
 - name: Dropbox API secret (long term)
   severity: high
   type: pattern
   values:
-    - (^|[^0-9A-Za-z])(?=[A-Za-z0-9]{64})(?P<value>[A-Za-z0-9]{10,12}[B-Za-z0-9]A{10,12}[B-Za-z0-9][A-Za-z0-9]{40,44})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?=[A-Za-z0-9]{64})(?P<value>[A-Za-z0-9]{10,12}[B-Za-z0-9]A{10,12}[B-Za-z0-9][A-Za-z0-9]{40,44})([^=0-9A-Za-z_/+-]|$)
   filter_type: []
   min_line_len: 43
   required_substrings:
     - AAAAAAAAAA
   usage_list:
     - src
     - doc
 
 - name: Dropbox App secret
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 15
   usage_list:
     - src
     - doc
 
 - name: Gitlab Incoming Email Token
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z._/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 24
   usage_list:
     - src
     - doc
 
 - name: Gitlab Feed Token
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z._/+-])(?P<value>[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 20
   usage_list:
     - src
     - doc
 
 - name: Jira 2FA
   severity: info
   type: pattern
   values:
-    - (^|[^0-9A-Za-z_/+-])(?P<value>[A-Z2-7]{16})([^=0-9A-Za-z_/+-]|$)
+    - (^|[^.0-9A-Za-z_/+-])(?P<value>[A-Z2-7]{16})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueCoupleKeywordCheck
     - ValuePatternCheck
     - ValueEntropyBase32Check
     - ValueBase32DataCheck
     - ValueTokenBase32Check
   min_line_len: 16
```

### Comparing `credsweeper-1.5.1/credsweeper/rules/rule.py` & `credsweeper-1.5.2/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.5.2/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.5.2/credsweeper/scanner/scan_type/scan_type.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.5.2/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/scanner/scanner.py` & `credsweeper-1.5.2/credsweeper/scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from pathlib import Path
 from typing import List, Optional, Type, Tuple, Dict, Union
 
 from credsweeper.app import APP_PATH
 from credsweeper.common.constants import RuleType, MIN_VARIABLE_LENGTH, MIN_SEPARATOR_LENGTH, MIN_VALUE_LENGTH, \
-    MAX_LINE_LENGTH, Separator
+    MAX_LINE_LENGTH, Separator, PEM_BEGIN_PATTERN
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.rules import Rule
 from credsweeper.scanner.scan_type import MultiPattern, PemKeyPattern, ScanType, SinglePattern
 from credsweeper.utils import Util
 
@@ -98,15 +98,15 @@
                     if x in target_line_trimmed:
                         keyword_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
                         break
             # Check if have length not smaller than smallest `min_line_len` in all pattern rules
             if target_line_trimmed_len >= self.min_pattern_len:
                 pattern_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
             # Check if have "BEGIN" substring. Cannot otherwise ba matched as a PEM key
-            if target_line_trimmed_len >= self.min_pem_key_len and "BEGIN" in target_line_trimmed:
+            if target_line_trimmed_len >= self.min_pem_key_len and PEM_BEGIN_PATTERN in target_line_trimmed:
                 pem_targets.append((target, target_line_trimmed_lower, target_line_trimmed_len))
 
         return keyword_targets, pattern_targets, pem_targets
 
     def _is_available(self, usage_list: List[str], rule: Rule) -> bool:
         """separate the method to reduce complexity"""
         if rule.severity < self.config.severity:
```

### Comparing `credsweeper-1.5.1/credsweeper/secret/config.json` & `credsweeper-1.5.2/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/secret/log.yaml` & `credsweeper-1.5.2/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/utils/util.py` & `credsweeper-1.5.2/credsweeper/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Any, Dict, List, Tuple, Optional, Union
 
 import whatthepatch
 import yaml
 from lxml import etree
 from typing_extensions import TypedDict
 
-from credsweeper.common.constants import Chars, DiffRowType, KeywordPattern, Separator, AVAILABLE_ENCODINGS, \
+from credsweeper.common.constants import DiffRowType, KeywordPattern, Separator, AVAILABLE_ENCODINGS, \
     DEFAULT_ENCODING, LATIN_1
 
 logger = logging.getLogger(__name__)
 
 DiffDict = TypedDict(
     "DiffDict",
     {
@@ -65,36 +65,23 @@
         if result[-1] == "|":
             result = result[:-1]
         result += ")"
 
         return result
 
     @staticmethod
-    def is_entropy_validate(data: str) -> bool:
-        """Verifies data entropy with base64, base36 and base16(hex)"""
-        # Replaced to the steps due: 1 - coverage 2 - YAPF
-        if Util.get_shannon_entropy(data, Chars.BASE64_CHARS.value) > 4.5:
-            return True
-        elif Util.get_shannon_entropy(data, Chars.BASE36_CHARS.value) > 3:
-            return True
-        elif Util.get_shannon_entropy(data, Chars.HEX_CHARS.value) > 3:
-            return True
-        else:
-            return False
-
-    @staticmethod
     def get_shannon_entropy(data: str, iterator: str) -> float:
         """Borrowed from http://blog.dkbza.org/2007/05/scanning-data-for-entropy-anomalies.html."""
         if not data:
             return 0
 
         entropy = 0.
-        data_len = len(data)
+        data_len = float(len(data))
         for x in iterator:
-            p_x = float(data.count(x)) / data_len
+            p_x = data.count(x) / data_len
             if p_x > 0:
                 entropy += -p_x * math.log(p_x, 2)
 
         return entropy
 
     """Precalculated data for speedup"""
     MIN_DATA_ENTROPY: Dict[int, float] = {
```

### Comparing `credsweeper-1.5.1/credsweeper/validations/__init__.py` & `credsweeper-1.5.2/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/apply_validation.py` & `credsweeper-1.5.2/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/github_token_validation.py` & `credsweeper-1.5.2/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.5.2/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.5.2/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.5.2/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.5.2/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.5.2/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.5.2/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.5.2/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper/validations/validation.py` & `credsweeper-1.5.2/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.5.2/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.1
+Version: 1.5.2
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.1/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.5.2/credsweeper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 credsweeper/filters/value_camel_case_check.py
 credsweeper/filters/value_couple_keyword_check.py
 credsweeper/filters/value_dictionary_keyword_check.py
 credsweeper/filters/value_dictionary_value_length_check.py
 credsweeper/filters/value_entropy_base32_check.py
 credsweeper/filters/value_entropy_base36_check.py
 credsweeper/filters/value_entropy_base64_check.py
-credsweeper/filters/value_entropy_check.py
 credsweeper/filters/value_file_path_check.py
 credsweeper/filters/value_first_word_check.py
 credsweeper/filters/value_grafana_check.py
 credsweeper/filters/value_json_web_token_check.py
 credsweeper/filters/value_last_word_check.py
 credsweeper/filters/value_length_check.py
 credsweeper/filters/value_method_check.py
@@ -119,14 +118,15 @@
 credsweeper/scanner/scan_type/multi_pattern.py
 credsweeper/scanner/scan_type/pem_key_pattern.py
 credsweeper/scanner/scan_type/scan_type.py
 credsweeper/scanner/scan_type/single_pattern.py
 credsweeper/secret/config.json
 credsweeper/secret/log.yaml
 credsweeper/utils/__init__.py
+credsweeper/utils/entropy_validator.py
 credsweeper/utils/util.py
 credsweeper/validations/__init__.py
 credsweeper/validations/apply_validation.py
 credsweeper/validations/github_token_validation.py
 credsweeper/validations/google_api_key_validation.py
 credsweeper/validations/google_multi_validation.py
 credsweeper/validations/mailchimp_key_validation.py
```

### Comparing `credsweeper-1.5.1/setup.py` & `credsweeper-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.1/tests/test_app.py` & `credsweeper-1.5.2/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     rule: Password
                     / severity: medium
                     / line_data_list:
                         [line: 'password = \"cackle!\"'
                         / line_num: 1
                         / path: {target_path}
                         / value: 'cackle!'
-                        / entropy_validation: False]
+                        / entropy_validation: BASE64_CHARS 2.120590 False]
                     / api_validation: NOT_AVAILABLE
                     / ml_validation: VALIDATED_KEY\n
                     Detected Credentials: 1\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
         self.assertEqual(expected, output)
@@ -98,15 +98,15 @@
                     rule: Password
                     / severity: medium
                     / line_data_list:
                     [line: '  "password": "dkajco1"'
                         / line_num: 3
                         / path: .changes/1.16.98.json
                         / value: 'dkajco1'
-                        / entropy_validation: False]
+                        / entropy_validation: BASE64_CHARS 2.807355 False]
                     / api_validation: NOT_AVAILABLE
                     / ml_validation: VALIDATED_KEY\n
                     Added File Credentials: 1\n
                     Deleted File Credentials: 0\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
@@ -123,39 +123,40 @@
                     rule: AWS Client ID
                         / severity: high
                         / line_data_list:
                             [line: ' clid = "AKIAQWADE5R42RDZ4JEM"'
                             / line_num: 4
                             / path: creds.py
                             / value: 'AKIAQWADE5R42RDZ4JEM'
-                            / entropy_validation: False]
+                            / entropy_validation: BASE64_CHARS 3.684184 False]
                         / api_validation: NOT_AVAILABLE
                         / ml_validation: VALIDATED_KEY
                     rule: AWS Multi
                         / severity: high
                         / line_data_list:
                             [line: ' clid = "AKIAQWADE5R42RDZ4JEM"'
                             / line_num: 4
                             / path: creds.py
                             / value: 'AKIAQWADE5R42RDZ4JEM'
-                            / entropy_validation: False, line: ' token = "V84C7sDU001tFFodKU95USNy97TkqXymnvsFmYhQ"'
+                            / entropy_validation: BASE64_CHARS 3.684184 False,
+                            line: ' token = "V84C7sDU001tFFodKU95USNy97TkqXymnvsFmYhQ"'
                             / line_num: 5
                             / path: creds.py
                             / value: 'V84C7sDU001tFFodKU95USNy97TkqXymnvsFmYhQ'
-                            / entropy_validation: True]
+                            / entropy_validation: BASE64_CHARS 4.784184 True]
                         / api_validation: NOT_AVAILABLE
                         / ml_validation: VALIDATED_KEY
                     rule: Token
                         / severity: medium
                         / line_data_list:
                             [line: ' token = "V84C7sDU001tFFodKU95USNy97TkqXymnvsFmYhQ"'
                             / line_num: 5
                             / path: creds.py
                             / value: 'V84C7sDU001tFFodKU95USNy97TkqXymnvsFmYhQ'
-                            / entropy_validation: True]
+                            / entropy_validation: BASE64_CHARS 4.784184 True]
                         / api_validation: NOT_AVAILABLE
                         / ml_validation: VALIDATED_KEY\n
                     Added File Credentials: 3\n
                     Deleted File Credentials: 0\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
@@ -175,15 +176,15 @@
                     rule: Google API Key
                     / severity: high
                     / line_data_list:
                     [line: 'AIzaGiReoG-CrackleCrackle12315618_12315'
                         / line_num: 1
                         / path: {target_path}
                         / value: 'AIzaGiReoG-CrackleCrackle12315618_12315'
-                        / entropy_validation: True]
+                        / entropy_validation: BASE36_CHARS 3.165196 True]
                     / api_validation: INVALID_KEY
                     / ml_validation: NOT_AVAILABLE\n
                     Detected Credentials: 1\n
                     Time Elapsed:
                     """
         expected = " ".join(expected.split())
         self.assertEqual(expected, output)
```

### Comparing `credsweeper-1.5.1/tests/test_main.py` & `credsweeper-1.5.2/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,16 +552,16 @@
     def test_yaml_p(self) -> None:
         # test for finding credentials in YAML
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "binary.yaml"])
         cred_sweeper = CredSweeper(depth=5)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         self.assertEqual(2, len(found_credentials))
-        self.assertSetEqual({"Secret", "PEM Certificate"}, set(i.rule_name for i in found_credentials))
-        self.assertSetEqual({"we5345d0f3da48544z1t1e275y05i161x995q485\n", "-----BEGIN RSA PRIVATE"},
+        self.assertSetEqual({"Secret", "PEM Private Key"}, set(i.rule_name for i in found_credentials))
+        self.assertSetEqual({"we5345d0f3da48544z1t1e275y05i161x995q485\n", "-----BEGIN RSA PRIVATE KEY-----"},
                             set(i.line_data_list[0].value for i in found_credentials))
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_yaml_n(self) -> None:
         # test to prove that no credentials are found without depth
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "binary.yaml"])
```

