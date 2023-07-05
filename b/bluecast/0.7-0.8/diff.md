# Comparing `tmp/bluecast-0.7.tar.gz` & `tmp/bluecast-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.7.tar", max compression
+gzip compressed data, was "bluecast-0.8.tar", max compression
```

## Comparing `bluecast-0.7.tar` & `bluecast-0.8.tar`

### file list

```diff
@@ -1,111 +1,116 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.7/LICENSE
--rw-r--r--   0        0        0    20021 2023-06-30 06:13:52.474377 bluecast-0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.7/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.7/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.7/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    12782 2023-06-27 06:12:53.582996 bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0    12769 2023-06-27 07:43:47.489769 bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0    18653 2023-06-27 06:12:51.958971 bluecast-0.7/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.7/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.7/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3962 2023-06-29 10:56:40.664250 bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     3612 2023-06-29 17:56:28.976335 bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0     2873 2023-06-29 15:32:18.638107 bluecast-0.7/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-29 09:57:47.802211 bluecast-0.7/bluecast/eda/__init__.py
--rw-r--r--   0        0        0      152 2023-06-29 10:24:21.113333 bluecast-0.7/bluecast/eda/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3051 2023-06-29 10:56:40.208243 bluecast-0.7/bluecast/eda/__pycache__/analyse.cpython-310.pyc
--rw-r--r--   0        0        0     3708 2023-06-29 10:32:55.497841 bluecast-0.7/bluecast/eda/analyse.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.7/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.7/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.7/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1955 2023-06-29 10:24:22.109350 bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1957 2023-06-29 13:35:03.129236 bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1321 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     2212 2023-06-28 11:13:13.084298 bluecast-0.7/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.7/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.7/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.7/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.7/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.7/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.7/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.7/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     9292 2023-06-29 10:56:40.924254 bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0     8899 2023-06-29 15:25:20.467211 bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    14148 2023-06-30 05:58:04.387112 bluecast-0.7/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.7/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.7/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
--rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     2239 2023-06-27 04:06:05.910063 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     2228 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
--rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4561 2023-06-27 07:43:47.501769 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     1982 2023-06-27 07:43:47.505769 bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     2332 2023-06-27 07:43:47.505769 bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.7/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     1890 2023-06-27 03:46:28.907353 bluecast-0.7/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.7/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.7/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.7/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.7/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1797 2023-06-29 10:57:31.301060 bluecast-0.7/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     8753 2023-06-29 10:24:22.017348 bluecast-0.7/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.7/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.7/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.7/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.7/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.7/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.7/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.7/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.7/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.7/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4064 2023-06-27 04:06:05.962063 bluecast-0.7/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.7/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.7/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.7/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     1176 2023-06-29 10:57:29.465031 bluecast-0.7/bluecast/tests/test_analyse.py
--rw-r--r--   0        0        0     6677 2023-06-28 11:19:35.634947 bluecast-0.7/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.7/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.7/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.7/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.7/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.7/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.7/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.7/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.7/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.7/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2296 2023-06-27 03:46:28.907353 bluecast-0.7/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.7/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.7/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.7/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1478 2023-06-30 06:15:04.035657 bluecast-0.7/pyproject.toml
--rw-r--r--   0        0        0    21171 1970-01-01 00:00:00.000000 bluecast-0.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.8/LICENSE
+-rw-r--r--   0        0        0    21843 2023-07-04 12:34:21.155729 bluecast-0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.8/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.8/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.8/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    12784 2023-07-04 05:47:32.922473 bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0    12771 2023-07-04 05:55:24.921932 bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0     3288 2023-07-04 05:48:22.227257 bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-310.pyc
+-rw-r--r--   0        0        0     3889 2023-07-04 08:06:47.096758 bluecast-0.8/bluecast/blueprints/__pycache__/cast_cv.cpython-38.pyc
+-rw-r--r--   0        0        0    18655 2023-07-04 04:45:52.998854 bluecast-0.8/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0     6015 2023-07-04 09:07:51.456141 bluecast-0.8/bluecast/blueprints/cast_cv.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.8/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.8/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3792 2023-07-04 05:47:32.926473 bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3684 2023-07-04 04:33:16.382858 bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     4815 2023-07-05 03:56:09.501654 bluecast-0.8/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/eda/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-04 05:47:32.270463 bluecast-0.8/bluecast/eda/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3051 2023-07-04 05:47:32.270463 bluecast-0.8/bluecast/eda/__pycache__/analyse.cpython-310.pyc
+-rw-r--r--   0        0        0     3708 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/eda/analyse.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.8/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.8/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.8/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1955 2023-06-29 10:24:22.109350 bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1957 2023-06-29 13:35:03.129236 bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1321 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2212 2023-06-28 11:13:13.084298 bluecast-0.8/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.8/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.8/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.8/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.8/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.8/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.8/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.8/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     9075 2023-07-04 05:47:33.326480 bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     9009 2023-07-03 13:08:03.868811 bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    14435 2023-07-03 13:07:54.936762 bluecast-0.8/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.8/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.8/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.8/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     2239 2023-06-27 04:06:05.910063 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     2228 2023-06-27 07:43:47.497769 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-27 07:43:47.501769 bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1982 2023-06-27 07:43:47.505769 bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     2332 2023-06-27 07:43:47.505769 bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.8/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1890 2023-06-27 03:46:28.907353 bluecast-0.8/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.8/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.8/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.8/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.8/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.8/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1797 2023-07-04 05:47:32.018459 bluecast-0.8/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     8753 2023-07-04 05:47:32.846472 bluecast-0.8/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2412 2023-07-04 05:47:33.582484 bluecast-0.8/bluecast/tests/__pycache__/test_cast_cv.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.8/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.8/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.8/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.8/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.8/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.8/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.8/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.8/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.8/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4064 2023-06-27 04:06:05.962063 bluecast-0.8/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.8/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.8/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.8/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.8/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     1176 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/tests/test_analyse.py
+-rw-r--r--   0        0        0     6677 2023-06-30 06:22:16.681826 bluecast-0.8/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1357 2023-07-04 05:47:13.522164 bluecast-0.8/bluecast/tests/test_cast_cv.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.8/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.8/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.8/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.8/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.8/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.8/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.8/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.8/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.8/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2296 2023-06-27 03:46:28.907353 bluecast-0.8/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.8/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.8/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.8/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1478 2023-07-02 15:26:48.016156 bluecast-0.8/pyproject.toml
+-rw-r--r--   0        0        0    22993 1970-01-01 00:00:00.000000 bluecast-0.8/PKG-INFO
```

### Comparing `bluecast-0.7/LICENSE` & `bluecast-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/README.md` & `bluecast-0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,17 @@
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Explanatory analysis](#explanatory-analysis)
     * [Enable cross-validation](#enable-cross-validation)
+    * [Use multi-model blended pipeline](#use-multi-model-blended-pipeline)
     * [Categorical encoding](#categorical-encoding)
+    * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
     * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
@@ -88,20 +90,15 @@
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 ### Advanced usage
 
 #### Explanatory analysis
 
-BlueCast offers a simple way to get a first overview of the data. This is
-
-#### Enable cross-validation
-
-While the default behaviour of BlueCast is to use a simple
-train-test-split, cross-validation can be enabled easily:
+BlueCast offers a simple way to get a first overview of the data:
 
 ```sh
 from bluecast.eda.analyse import (
     bi_variate_plots,
     correlation_heatmap,
     correlation_to_target,
     univariate_plots,
@@ -134,25 +131,77 @@
 # show correlation to target
 correlation_to_target(train_data.loc[
             :, feat_type_detector.num_columns
         ],
         "EC1",)
 ```
 
+#### Enable cross-validation
+
+While the default behaviour of BlueCast is to use a simple
+train-test-split, cross-validation can be enabled easily:
+
+```sh
+from bluecast.blueprints.cast import BlueCast
+from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
+
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.hypertuning_cv_folds = 5 # default is 1
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCast(
+        class_problem="binary",
+        target_column="target"
+        conf_training=train_config,
+    )
+
+automl.fit(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
+#### Use multi-model blended pipeline
+
+By default, BlueCast trains a single model. However, it is possible to
+train multiple models with one call for extra robustness. `BlueCastCV`
+has a `fit` and a `fit_eval` method. The `fit_eval` method trains the
+models, but also provides out-of-fold validation. Also `BlueCastCV`
+allows to pass custom configurations.
+
+```sh
+from bluecast.blueprints.cast import BlueCastCV
+from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCastCV(
+        class_problem="binary",
+        #conf_training=train_config,
+        #conf_xgboost=xgboost_param_config,
+        #custom_preprocessor=custom_preprocessor, # this takes place right after test_train_split
+        #custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
+        #custom_feature_selector=custom_feature_selector,
+    )
+
+# this class has a train method:
+# automl.fit(df_train, target_col="target")
+
+automl.fit_eval(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
 #### Categorical encoding
 
 By default, BlueCast uses target encoding.
 This behaviour can be changed in the TrainingConfig by setting `cat_encoding_via_ml_algorithm`
 to True. This will change the expectations of `custom_last_mile_computation` though.
 If `cat_encoding_via_ml_algorithm` is set to False, `custom_last_mile_computation`
 will receive numerical features only as target encoding will apply before. If `cat_encoding_via_ml_algorithm`
 is True (default setting) `custom_last_mile_computation` will receive categorical
-features as well, because Xgboost#s inbuilt categorical encoding will be used.
-
-```sh
+features as well, because Xgboost's inbuilt categorical encoding will be used.
 
 #### Custom  training configuration
 
 Despite e2eml, BlueCast allows easy customization. Users can adjust the
 configuration and just pass it to the `BlueCast` class. Here is an example:
 
 ```sh
```

### Comparing `bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 27 06:12:51 2023 UTC, .py size: 18653 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e37d 9a64 dd48 0000  o........}.d.H..
+00000000: 6f0d 0d0a 0000 0000 00a4 a364 df48 0000  o..........d.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6402 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6401 6402 6c0d 5a0e 6401 6405 6c0f  Z.d.d.l.Z.d.d.l.
@@ -97,15 +97,15 @@
 00000600: 1884 045a 1664 1265 136a 1464 1965 136a  ...Z.d.e.j.d.e.j
 00000610: 1464 1a65 136a 1764 1665 0664 1365 1865  .d.e.j.d.e.d.e.e
 00000620: 0665 0c66 0219 0066 0a64 1b64 1c84 045a  .e.f...f.d.d...Z
 00000630: 1964 1265 136a 1464 1365 136a 1466 0464  .d.e.j.d.e.j.f.d
 00000640: 1d64 1e84 045a 1a64 1265 136a 1464 1365  .d...Z.d.e.j.d.e
 00000650: 1b65 1c6a 1d65 1c6a 1d66 0219 0066 0464  .e.j.e.j.f...f.d
 00000660: 1f64 2084 045a 1e64 0253 0029 22da 0842  .d ..Z.d.S.)"..B
-00000670: 6c75 6543 6173 7461 2206 0000 5275 6e20  lueCasta"...Run 
+00000670: 6c75 6543 6173 7461 2406 0000 5275 6e20  lueCasta$...Run 
 00000680: 6675 6c6c 7920 636f 6e66 6967 7572 6564  fully configured
 00000690: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
 000006a0: 626c 7565 7072 696e 742e 0a0a 2020 2020  blueprint...    
 000006b0: 4375 7374 6f6d 697a 6174 696f 6e20 7669  Customization vi
 000006c0: 6120 636c 6173 7320 6174 7472 6962 7574  a class attribut
 000006d0: 6573 2069 7320 706f 7373 6962 6c65 2e20  es is possible. 
 000006e0: 436f 6e66 6967 7320 6361 6e20 6265 2069  Configs can be i
@@ -135,665 +135,665 @@
 00000860: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
 00000870: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
 00000880: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
 00000890: 7468 6520 6361 7465 676f 7269 6361 6c20  the categorical 
 000008a0: 636f 6c75 6d6e 732e 2049 6620 6e6f 7420  columns. If not 
 000008b0: 7072 6f76 6964 6564 2c0a 2020 2020 426c  provided,.    Bl
 000008c0: 7565 4361 7374 2077 696c 6c20 696e 6665  ueCast will infe
-000008d0: 7220 7468 6573 6520 6175 746f 6d61 6963  r these automaic
-000008e0: 616c 6c79 2e0a 2020 2020 3a70 6172 616d  ally..    :param
-000008f0: 203a 6461 7465 5f63 6f6c 756d 6e73 3a20   :date_columns: 
-00000900: 5461 6b65 7320 6120 6c69 7374 206f 6620  Takes a list of 
-00000910: 7374 7269 6e67 7320 636f 6e74 6169 6e69  strings containi
-00000920: 6e67 2074 6865 206e 616d 6573 206f 6620  ng the names of 
-00000930: 7468 6520 6461 7465 2063 6f6c 756d 6e73  the date columns
-00000940: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
-00000950: 642c 0a20 2020 2042 6c75 6543 6173 7420  d,.    BlueCast 
-00000960: 7769 6c6c 2069 6e66 6572 2074 6865 7365  will infer these
-00000970: 2061 7574 6f6d 6169 6361 6c6c 792e 0a20   automaically.. 
-00000980: 2020 203a 7061 7261 6d20 3a74 696d 655f     :param :time_
-00000990: 7370 6c69 745f 636f 6c75 6d6e 3a20 5461  split_column: Ta
-000009a0: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-000009b0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
-000009c0: 206f 6620 7468 6520 7469 6d65 2073 706c   of the time spl
-000009d0: 6974 2063 6f6c 756d 6e2e 2049 6620 6e6f  it column. If no
-000009e0: 7420 7072 6f76 6964 6564 2c0a 2020 2020  t provided,.    
-000009f0: 426c 7565 4361 7374 2077 696c 6c20 6e6f  BlueCast will no
-00000a00: 7420 7370 6c69 7420 7468 6520 6461 7461  t split the data
-00000a10: 2062 7920 7469 6d65 206f 7220 6f72 6465   by time or orde
-00000a20: 722c 2062 7574 2064 6f20 6120 7261 6e64  r, but do a rand
-00000a30: 6f6d 2073 706c 6974 2069 6e73 7465 6164  om split instead
-00000a40: 2e0a 2020 2020 3a70 6172 616d 203a 6d6c  ..    :param :ml
-00000a50: 5f6d 6f64 656c 3a20 5461 6b65 7320 616e  _model: Takes an
-00000a60: 2069 6e73 7461 6e63 6520 6f66 2061 2058   instance of a X
-00000a70: 6762 6f6f 7374 4d6f 6465 6c20 636c 6173  gboostModel clas
-00000a80: 732e 2049 6620 6e6f 7420 7072 6f76 6964  s. If not provid
-00000a90: 6564 2c20 426c 7565 4361 7374 2077 696c  ed, BlueCast wil
-00000aa0: 6c20 696e 7374 616e 7469 6174 6520 6f6e  l instantiate on
-00000ab0: 652e 0a20 2020 2054 6869 7320 6973 2061  e..    This is a
-00000ac0: 6e20 4150 4920 746f 2070 6173 7320 616e  n API to pass an
-00000ad0: 7920 6d6f 6465 6c20 636c 6173 732e 2049  y model class. I
-00000ae0: 6e68 6572 6974 2074 6865 2062 6173 6563  nherit the basec
-00000af0: 6c61 7373 2066 726f 6d20 6d6c 5f6d 6f64  lass from ml_mod
-00000b00: 656c 6c69 6e67 2e62 6173 655f 6d6f 6465  elling.base_mode
-00000b10: 6c2e 4261 7365 4d6f 6465 6c2e 0a20 2020  l.BaseModel..   
-00000b20: 203a 7061 7261 6d20 6375 7374 6f6d 5f70   :param custom_p
-00000b30: 7265 7072 6f63 6573 736f 723a 2054 616b  reprocessor: Tak
-00000b40: 6573 2061 6e20 696e 7374 616e 6365 206f  es an instance o
-00000b50: 6620 6120 4375 7374 6f6d 5072 6570 726f  f a CustomPrepro
-00000b60: 6365 7373 696e 6720 636c 6173 732e 2041  cessing class. A
-00000b70: 6c6c 6f77 7320 7573 6572 7320 746f 2069  llows users to i
-00000b80: 6e6a 6563 7420 6375 7374 6f6d 0a20 2020  nject custom.   
-00000b90: 2070 7265 7072 6f63 6573 7369 6e67 2073   preprocessing s
-00000ba0: 7465 7073 2077 6869 6368 2074 616b 6520  teps which take 
-00000bb0: 706c 6163 6520 7269 6768 7420 6166 7465  place right afte
-00000bc0: 7220 7468 6520 7472 6169 6e20 7465 7374  r the train test
-00000bd0: 2073 7069 742e 0a20 2020 203a 7061 7261   spit..    :para
-00000be0: 6d20 6375 7374 6f6d 5f6c 6173 745f 6d69  m custom_last_mi
-00000bf0: 6c65 5f63 6f6d 7075 7461 7469 6f6e 3a20  le_computation: 
-00000c00: 5461 6b65 7320 616e 2069 6e73 7461 6e63  Takes an instanc
-00000c10: 6520 6f66 2061 2043 7573 746f 6d50 7265  e of a CustomPre
-00000c20: 7072 6f63 6573 7369 6e67 2063 6c61 7373  processing class
-00000c30: 2e20 416c 6c6f 7773 2075 7365 7273 2074  . Allows users t
-00000c40: 6f20 696e 6a65 6374 2063 7573 746f 6d0a  o inject custom.
-00000c50: 2020 2020 7072 6570 726f 6365 7373 696e      preprocessin
-00000c60: 6720 7374 6570 7320 7768 6963 6820 7461  g steps which ta
-00000c70: 6b65 2070 6c61 6365 2072 6967 6874 2062  ke place right b
-00000c80: 6566 6f72 6520 7468 6520 6d6f 6465 6c20  efore the model 
-00000c90: 7472 6169 6e69 6e67 2e0a 2020 2020 4eda  training..    N.
-00000ca0: 0d63 6c61 7373 5f70 726f 626c 656d 2902  .class_problem).
-00000cb0: da06 6269 6e61 7279 da0a 6d75 6c74 6963  ..binary..multic
-00000cc0: 6c61 7373 da0d 7461 7267 6574 5f63 6f6c  lass..target_col
-00000cd0: 756d 6eda 0b63 6174 5f63 6f6c 756d 6e73  umn..cat_columns
-00000ce0: da0c 6461 7465 5f63 6f6c 756d 6e73 da11  ..date_columns..
-00000cf0: 7469 6d65 5f73 706c 6974 5f63 6f6c 756d  time_split_colum
-00000d00: 6eda 086d 6c5f 6d6f 6465 6cda 1c63 7573  n..ml_model..cus
-00000d10: 746f 6d5f 6c61 7374 5f6d 696c 655f 636f  tom_last_mile_co
-00000d20: 6d70 7574 6174 696f 6eda 1363 7573 746f  mputation..custo
-00000d30: 6d5f 7072 6570 726f 6365 7373 6f72 da17  m_preprocessor..
-00000d40: 6375 7374 6f6d 5f66 6561 7475 7265 5f73  custom_feature_s
-00000d50: 656c 6563 746f 72da 0d63 6f6e 665f 7472  elector..conf_tr
-00000d60: 6169 6e69 6e67 da0c 636f 6e66 5f78 6762  aining..conf_xgb
-00000d70: 6f6f 7374 da13 636f 6e66 5f70 6172 616d  oost..conf_param
-00000d80: 735f 7867 626f 6f73 7463 0d00 0000 0000  s_xgboostc......
-00000d90: 0000 0000 0000 0d00 0000 0200 0000 4300  ..............C.
-00000da0: 0000 7370 0000 007c 017c 005f 0064 017c  ..sp...|.|._.d.|
-00000db0: 005f 017c 037c 005f 027c 047c 005f 037c  ._.|.|._.|.|._.|
-00000dc0: 057c 005f 047c 027c 005f 057c 0a7c 005f  .|._.|.|._.|.|._
-00000dd0: 067c 0b7c 005f 077c 0c7c 005f 0864 007c  .|.|._.|.|._.d.|
-00000de0: 005f 0964 007c 005f 0a64 007c 005f 0b64  ._.d.|._.d.|._.d
-00000df0: 007c 005f 0c7c 067c 005f 0d7c 077c 005f  .|._.|.|._.|.|._
-00000e00: 0e7c 087c 005f 0f7c 097c 005f 1064 007c  .|.|._.|.|._.d.|
-00000e10: 005f 1164 0053 0029 024e 4629 1272 1d00  ._.d.S.).NF).r..
-00000e20: 0000 da0f 7072 6564 6963 7469 6f6e 5f6d  ....prediction_m
-00000e30: 6f64 6572 2100 0000 7222 0000 0072 2300  oder!...r"...r#.
-00000e40: 0000 7220 0000 0072 2800 0000 7229 0000  ..r ...r(...r)..
-00000e50: 0072 2a00 0000 da12 6665 6174 5f74 7970  .r*.....feat_typ
-00000e60: 655f 6465 7465 6374 6f72 da0b 6361 745f  e_detector..cat_
-00000e70: 656e 636f 6465 72da 1474 6172 6765 745f  encoder..target_
-00000e80: 6c61 6265 6c5f 656e 636f 6465 72da 0f73  label_encoder..s
-00000e90: 6368 656d 615f 6465 7465 6374 6f72 7224  chema_detectorr$
-00000ea0: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
-00000eb0: 0000 da0b 7368 6170 5f76 616c 7565 7329  ....shap_values)
-00000ec0: 0dda 0473 656c 6672 1d00 0000 7220 0000  ...selfr....r ..
-00000ed0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000ee0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
-00000ef0: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
-00000f00: 0000 00a9 0072 3200 0000 fa3e 2f68 6f6d  .....r2....>/hom
-00000f10: 652f 7468 6f6d 6173 2f49 6465 6150 726f  e/thomas/IdeaPro
-00000f20: 6a65 6374 732f 426c 7565 4361 7374 2f62  jects/BlueCast/b
-00000f30: 6c75 6563 6173 742f 626c 7565 7072 696e  luecast/blueprin
-00000f40: 7473 2f63 6173 742e 7079 da08 5f5f 696e  ts/cast.py..__in
-00000f50: 6974 5f5f 3c00 0000 7326 0000 0006 1106  it__<...s&......
-00000f60: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00000f70: 0102 0304 fe06 0306 0106 0106 0106 0106  ................
-00000f80: 010a 017a 1142 6c75 6543 6173 742e 5f5f  ...z.BlueCast.__
-00000f90: 696e 6974 5f5f da02 6466 da06 7265 7475  init__..df..retu
-00000fa0: 726e 6302 0000 0000 0000 0000 0000 0003  rnc.............
-00000fb0: 0000 0005 0000 0043 0000 0073 3001 0000  .......C...s0...
-00000fc0: 7c00 6a00 7307 7401 8300 7c00 5f00 7c00  |.j.s.t...|._.|.
-00000fd0: 6a00 6a02 7315 6401 7d02 7403 6a04 7c02  j.j.s.d.}.t.j.|.
-00000fe0: 7405 6402 6403 8d03 0100 7c00 6a00 6a06  t.d.d.....|.j.j.
-00000ff0: 6404 6b02 7225 6405 7d02 7403 6a04 7c02  d.k.r%d.}.t.j.|.
-00001000: 7405 6402 6403 8d03 0100 7c00 6a00 6a02  t.d.d.....|.j.j.
-00001010: 7236 7c00 6a07 7336 6406 7d02 7403 6a04  r6|.j.s6d.}.t.j.
-00001020: 7c02 7405 6402 6403 8d03 0100 7c00 6a08  |.t.d.d.....|.j.
-00001030: 7343 6407 7d02 7403 6a04 7c02 7405 6402  sCd.}.t.j.|.t.d.
-00001040: 6403 8d03 0100 7c00 6a00 6a09 740a 7c01  d.....|.j.j.t.|.
-00001050: 6a0b 8301 6b05 725a 7c00 6a00 6a02 725a  j...k.rZ|.j.j.rZ
-00001060: 6408 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-00001070: 8d03 0100 7c00 6a00 6a0c 7270 7c00 6a00  ....|.j.j.rp|.j.
-00001080: 6a0d 7270 6409 7c00 6a00 5f0d 640a 7d02  j.rpd.|.j._.d.}.
-00001090: 7403 6a04 7c02 7405 6402 6403 8d03 0100  t.j.|.t.d.d.....
-000010a0: 7c00 6a00 6a0c 7281 7c00 6a0e 7281 640b  |.j.j.r.|.j.r.d.
-000010b0: 7d02 7403 6a04 7c02 7405 6402 6403 8d03  }.t.j.|.t.d.d...
-000010c0: 0100 7c00 6a00 6a0c 7294 7c00 6a0f 7296  ..|.j.j.r.|.j.r.
-000010d0: 640c 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-000010e0: 8d03 0100 6400 5300 6400 5300 6400 5300  ....d.S.d.S.d.S.
-000010f0: 290d 4e61 9301 0000 4665 6174 7572 6520  ).Na....Feature 
-00001100: 7365 6c65 6374 696f 6e20 6973 2064 6973  selection is dis
-00001110: 6162 6c65 642e 2055 7064 6174 6520 7468  abled. Update th
-00001120: 6520 5472 6169 6e69 6e67 436f 6e66 6967  e TrainingConfig
-00001130: 2070 6172 616d 2027 656e 6162 6c65 5f66   param 'enable_f
-00001140: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
-00001150: 270a 2020 2020 2020 2020 2020 2020 746f  '.            to
-00001160: 2065 6e61 626c 6520 6974 206f 7220 6d61   enable it or ma
-00001170: 6b65 2075 7365 206f 6620 6120 6375 7374  ke use of a cust
-00001180: 6f6d 2070 7265 7072 6f63 6573 736f 7220  om preprocessor 
-00001190: 746f 2064 6f20 6974 206d 616e 7561 6c6c  to do it manuall
-000011a0: 7920 6475 7269 6e67 2074 6865 206c 6173  y during the las
-000011b0: 7420 6d69 6c65 2063 6f6d 7075 7461 7469  t mile computati
-000011c0: 6f6e 7320 7374 6570 2e0a 2020 2020 2020  ons step..      
-000011d0: 2020 2020 2020 4665 6174 7572 6520 7365        Feature se
-000011e0: 6c65 6374 696f 6e20 6973 2072 6563 6f6d  lection is recom
-000011f0: 6d65 6e64 6564 2066 6f72 2064 6174 6173  mended for datas
-00001200: 6574 7320 7769 7468 206d 616e 7920 6665  ets with many fe
-00001210: 6174 7572 6573 2028 3e31 3030 3029 2e20  atures (>1000). 
-00001220: 466f 7220 6461 7461 7365 7473 2077 6974  For datasets wit
-00001230: 6820 6120 736d 616c 6c20 616d 6f75 6e74  h a small amount
-00001240: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
-00001250: 6665 6174 7572 6573 2066 6561 7475 7265  features feature
-00001260: 2073 656c 6563 7469 6f6e 2069 7320 6e6f   selection is no
-00001270: 7420 7265 636f 6d6d 656e 6465 642e 0a20  t recommended.. 
-00001280: 2020 2020 2020 2020 2020 20e9 0200 0000             .....
-00001290: 2901 da0a 7374 6163 6b6c 6576 656c e901  )...stacklevel..
-000012a0: 0000 0061 0501 0000 4372 6f73 7320 7661  ...a....Cross va
-000012b0: 6c69 6461 7469 6f6e 2069 7320 6469 7361  lidation is disa
-000012c0: 626c 6564 2e20 5570 6461 7465 2074 6865  bled. Update the
-000012d0: 2054 7261 696e 696e 6743 6f6e 6669 6720   TrainingConfig 
-000012e0: 7061 7261 6d20 2768 7970 6572 7475 6e69  param 'hypertuni
-000012f0: 6e67 5f63 765f 666f 6c64 7327 0a20 2020  ng_cv_folds'.   
-00001300: 2020 2020 2020 2020 2074 6f20 656e 6162           to enab
-00001310: 6c65 2069 742e 2043 726f 7373 2076 616c  le it. Cross val
-00001320: 6964 6174 696f 6e20 6973 2064 6973 6162  idation is disab
-00001330: 6c65 6420 6f6e 2064 6566 6175 6c74 2074  led on default t
-00001340: 6f20 616c 6c6f 7720 6661 7374 2070 726f  o allow fast pro
-00001350: 746f 7479 7069 6e67 2e20 466f 7220 726f  totyping. For ro
-00001360: 6275 7374 2068 7970 6572 7061 7261 6d65  bust hyperparame
-00001370: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
-00001380: 7475 6e69 6e67 2075 7369 6e67 2061 7420  tuning using at 
-00001390: 6c65 6173 7420 3520 666f 6c64 7320 6973  least 5 folds is
-000013a0: 2072 6563 6f6d 6d65 6e64 6564 2e61 5f01   recommended.a_.
-000013b0: 0000 4665 6174 7572 6520 7365 6c65 6374  ..Feature select
-000013c0: 696f 6e20 6973 2065 6e61 626c 6564 2062  ion is enabled b
-000013d0: 7574 206e 6f20 6665 6174 7572 6520 7365  ut no feature se
-000013e0: 6c65 6374 6f72 2068 6173 2062 6565 6e20  lector has been 
-000013f0: 7072 6f76 6964 6564 2e20 4661 6c6c 696e  provided. Fallin
-00001400: 6720 6261 636b 2074 6f0a 2020 2020 2020  g back to.      
-00001410: 2020 2020 2020 6372 6f73 732d 7661 6c69        cross-vali
-00001420: 6461 7465 6420 6665 6174 7572 6520 656c  dated feature el
-00001430: 696d 696e 6174 696f 6e2e 2053 7065 6369  imination. Speci
-00001440: 6669 6361 6c6c 7920 666f 7220 736d 616c  fically for smal
-00001450: 6c20 6461 7461 7365 7473 2063 6865 636b  l datasets check
-00001460: 2074 6865 206c 6f67 7320 746f 2076 6572   the logs to ver
-00001470: 6966 7920 7468 6174 206e 6f74 2074 6f6f  ify that not too
-00001480: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
-00001490: 7920 6665 6174 7572 6573 2068 6176 6520  y features have 
-000014a0: 6265 656e 2072 656d 6f76 6564 2e20 4f74  been removed. Ot
-000014b0: 6865 7277 6973 652c 2063 6f6e 7369 6465  herwise, conside
-000014c0: 7220 6469 7361 626c 696e 6720 6665 6174  r disabling feat
-000014d0: 7572 6520 7365 6c65 6374 696f 6e20 6f72  ure selection or
-000014e0: 2070 726f 7669 6469 6e67 2061 2063 7573   providing a cus
-000014f0: 746f 6d0a 2020 2020 2020 2020 2020 2020  tom.            
-00001500: 6665 6174 7572 6520 7365 6c65 6374 6f72  feature selector
-00001510: 2e61 6501 0000 4e6f 2058 6762 6f6f 7374  .ae...No Xgboost
-00001520: 5475 6e65 5061 7261 6d73 436f 6e66 6967  TuneParamsConfig
-00001530: 2068 6173 2062 6565 6e20 7072 6f76 6964   has been provid
-00001540: 6564 2e20 4661 6c6c 696e 6720 6261 636b  ed. Falling back
-00001550: 2074 6f20 6465 6661 756c 7420 7661 6c75   to default valu
-00001560: 6573 2e20 4465 6661 756c 7420 7661 6c75  es. Default valu
-00001570: 6573 0a20 2020 2020 2020 2020 2020 2068  es.            h
-00001580: 6176 6520 6265 656e 2063 686f 7365 6e20  ave been chosen 
-00001590: 746f 2073 7065 6564 2075 7020 7468 6520  to speed up the 
-000015a0: 7072 6f74 6f74 7970 696e 672e 2046 6f72  prototyping. For
-000015b0: 2072 6f62 7573 7420 6879 7065 7270 6172   robust hyperpar
-000015c0: 616d 6574 6572 2074 756e 696e 6720 636f  ameter tuning co
-000015d0: 6e73 6964 6572 2070 726f 7669 6469 6e67  nsider providing
-000015e0: 2061 2063 7573 746f 6d0a 2020 2020 2020   a custom.      
-000015f0: 2020 2020 2020 5867 626f 6f73 7454 756e        XgboostTun
-00001600: 6550 6172 616d 7343 6f6e 6669 6720 7769  eParamsConfig wi
-00001610: 7468 2061 2064 6565 7065 7220 6879 7065  th a deeper hype
-00001620: 7270 6172 616d 6574 6572 2073 6561 7263  rparameter searc
-00001630: 6820 7370 6163 6520 616e 6420 6120 6375  h space and a cu
-00001640: 7374 6f6d 2054 7261 696e 696e 6743 6f6e  stom TrainingCon
-00001650: 6669 6720 746f 2065 6e61 626c 650a 2020  fig to enable.  
-00001660: 2020 2020 2020 2020 2020 6372 6f73 732d            cross-
-00001670: 7661 6c69 6461 7469 6f6e 2e61 0f01 0000  validation.a....
-00001680: 5468 6520 6d69 6e69 6d75 6d20 6e75 6d62  The minimum numb
-00001690: 6572 206f 6620 6665 6174 7572 6573 2074  er of features t
-000016a0: 6f20 7365 6c65 6374 2069 7320 6772 6561  o select is grea
-000016b0: 7465 7220 6f72 2065 7175 616c 2074 6f20  ter or equal to 
-000016c0: 7468 6520 6e75 6d62 6572 206f 6620 6665  the number of fe
-000016d0: 6174 7572 6573 2069 6e0a 2020 2020 2020  atures in.      
-000016e0: 2020 2020 2020 7468 6520 6461 7461 7365        the datase
-000016f0: 7420 7768 696c 6520 6665 6174 7572 6520  t while feature 
-00001700: 7365 6c65 6374 696f 6e20 6973 2065 6e61  selection is ena
-00001710: 626c 6564 2e20 436f 6e73 6964 6572 2072  bled. Consider r
-00001720: 6564 7563 696e 6720 7468 6520 6d69 6e69  educing the mini
-00001730: 6d75 6d20 6e75 6d62 6572 206f 6620 6665  mum number of fe
-00001740: 6174 7572 6573 2074 6f0a 2020 2020 2020  atures to.      
-00001750: 2020 2020 2020 7365 6c65 6374 206f 7220        select or 
-00001760: 6469 7361 626c 696e 6720 6665 6174 7572  disabling featur
-00001770: 6520 7365 6c65 6374 696f 6e20 7669 6120  e selection via 
-00001780: 5472 6169 6e69 6e67 436f 6e66 6967 2e46  TrainingConfig.F
-00001790: 612b 0200 0053 4841 5020 7661 6c75 6573  a+...SHAP values
-000017a0: 2063 616e 6e6f 7420 6265 2063 616c 6375   cannot be calcu
-000017b0: 6c61 7465 6420 7768 656e 2063 6174 6567  lated when categ
-000017c0: 6f72 6963 616c 2065 6e63 6f64 696e 6720  orical encoding 
-000017d0: 7669 6120 4d4c 2061 6c67 6f72 6974 686d  via ML algorithm
-000017e0: 2069 7320 656e 6162 6c65 6420 6475 6520   is enabled due 
-000017f0: 746f 0a20 2020 2020 2020 2020 2020 2069  to.            i
-00001800: 6e63 6f6d 7061 7469 6269 6c69 7479 2077  ncompatibility w
-00001810: 6974 6820 7468 6520 7368 6170 206c 6962  ith the shap lib
-00001820: 7261 7279 2e20 5365 6520 7468 6973 2047  rary. See this G
-00001830: 6974 4875 6220 6973 7375 6520 666f 7220  itHub issue for 
-00001840: 6d6f 7265 2063 6f6e 7465 7874 3a0a 2020  more context:.  
-00001850: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-00001860: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6c75  //github.com/slu
-00001870: 6e64 6265 7267 2f73 6861 702f 6973 7375  ndberg/shap/issu
-00001880: 6573 2f32 3636 0a0a 2020 2020 2020 2020  es/266..        
-00001890: 2020 2020 4361 6c63 756c 6174 696f 6e20      Calculation 
-000018a0: 6f66 2053 6861 7020 7661 6c75 6573 2068  of Shap values h
-000018b0: 6173 2062 6565 6e20 6368 616e 6765 6420  as been changed 
-000018c0: 746f 2066 616c 7365 2e0a 2020 2020 2020  to false..      
-000018d0: 2020 2020 2020 436f 6e73 6964 6572 2064        Consider d
-000018e0: 6973 6162 6c69 6e67 2063 6174 6567 6f72  isabling categor
-000018f0: 6963 616c 2065 6e63 6f64 696e 6720 7669  ical encoding vi
-00001900: 6120 4d4c 2061 6c67 6f72 6974 686d 2069  a ML algorithm i
-00001910: 6e20 7468 6520 5472 6169 6e69 6e67 436f  n the TrainingCo
-00001920: 6e66 6967 2069 6620 7368 6170 2076 616c  nfig if shap val
-00001930: 7565 7320 6172 650a 2020 2020 2020 2020  ues are.        
-00001940: 2020 2020 7265 7175 6972 6564 2e20 416c      required. Al
-00001950: 7465 726e 6174 6976 656c 7920 7573 6520  ternatively use 
-00001960: 5867 626f 6f73 7420 6173 2061 2063 7573  Xgboost as a cus
-00001970: 746f 6d20 6d6f 6465 6c20 616e 6420 6361  tom model and ca
-00001980: 6c63 756c 6174 6520 7368 6170 2076 616c  lculate shap val
-00001990: 7565 7320 6d61 6e75 616c 6c79 2076 6961  ues manually via
-000019a0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-000019b0: 645f 636f 6e74 7269 6273 3d54 7275 652e  d_contribs=True.
-000019c0: 7af0 4361 7465 676f 7269 6361 6c20 656e  z.Categorical en
-000019d0: 636f 6469 6e67 2076 6961 204d 4c20 616c  coding via ML al
-000019e0: 676f 7269 7468 6d20 6973 2065 6e61 626c  gorithm is enabl
-000019f0: 6564 2e20 4d61 6b65 2073 7572 6520 746f  ed. Make sure to
-00001a00: 2068 616e 646c 6520 6361 7465 676f 7269   handle categori
-00001a10: 6361 6c20 6665 6174 7572 6573 0a20 2020  cal features.   
-00001a20: 2020 2020 2020 2020 2077 6974 6869 6e20           within 
-00001a30: 7468 6520 7072 6f76 6964 6564 206d 6c20  the provided ml 
-00001a40: 6d6f 6465 6c20 6f72 2063 6f6e 7369 6465  model or conside
-00001a50: 7220 6469 7361 626c 696e 6720 6361 7465  r disabling cate
-00001a60: 676f 7269 6361 6c20 656e 636f 6469 6e67  gorical encoding
-00001a70: 2076 6961 204d 4c20 616c 676f 7269 7468   via ML algorith
-00001a80: 6d20 696e 2074 6865 0a20 2020 2020 2020  m in the.       
-00001a90: 2020 2020 2054 7261 696e 696e 6743 6f6e       TrainingCon
-00001aa0: 6669 6720 616c 7465 726e 6174 6976 656c  fig alternativel
-00001ab0: 792e 7afd 4361 7465 676f 7269 6361 6c20  y.z.Categorical 
-00001ac0: 656e 636f 6469 6e67 2076 6961 204d 4c20  encoding via ML 
-00001ad0: 616c 676f 7269 7468 6d20 6973 2065 6e61  algorithm is ena
-00001ae0: 626c 6564 2e20 4d61 6b65 2073 7572 6520  bled. Make sure 
-00001af0: 746f 2068 616e 646c 6520 6361 7465 676f  to handle catego
-00001b00: 7269 6361 6c20 6665 6174 7572 6573 0a20  rical features. 
-00001b10: 2020 2020 2020 2020 2020 2077 6974 6869             withi
-00001b20: 6e20 7468 6520 7072 6f76 6964 6564 206c  n the provided l
-00001b30: 6173 7420 6d69 6c65 2063 6f6d 7075 7461  ast mile computa
-00001b40: 7469 6f6e 206f 7220 636f 6e73 6964 6572  tion or consider
-00001b50: 2064 6973 6162 6c69 6e67 2063 6174 6567   disabling categ
-00001b60: 6f72 6963 616c 2065 6e63 6f64 696e 6720  orical encoding 
-00001b70: 7669 6120 4d4c 2061 6c67 6f72 6974 686d  via ML algorithm
-00001b80: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
-00001b90: 2020 2020 5472 6169 6e69 6e67 436f 6e66      TrainingConf
-00001ba0: 6967 2061 6c74 6572 6e61 7469 7665 6c79  ig alternatively
-00001bb0: 2e29 1072 2800 0000 720a 0000 00da 1865  .).r(...r......e
-00001bc0: 6e61 626c 655f 6665 6174 7572 655f 7365  nable_feature_se
-00001bd0: 6c65 6374 696f 6eda 0877 6172 6e69 6e67  lection..warning
-00001be0: 73da 0477 6172 6eda 0b55 7365 7257 6172  s..warn..UserWar
-00001bf0: 6e69 6e67 da14 6879 7065 7274 756e 696e  ning..hypertunin
-00001c00: 675f 6376 5f66 6f6c 6473 7227 0000 0072  g_cv_foldsr'...r
-00001c10: 2900 0000 da16 6d69 6e5f 6665 6174 7572  ).....min_featur
-00001c20: 6573 5f74 6f5f 7365 6c65 6374 da03 6c65  es_to_select..le
-00001c30: 6eda 0763 6f6c 756d 6e73 da1d 6361 745f  n..columns..cat_
-00001c40: 656e 636f 6469 6e67 5f76 6961 5f6d 6c5f  encoding_via_ml_
-00001c50: 616c 676f 7269 7468 6dda 1563 616c 6375  algorithm..calcu
-00001c60: 6c61 7465 5f73 6861 705f 7661 6c75 6573  late_shap_values
-00001c70: 7224 0000 0072 2500 0000 2903 7231 0000  r$...r%...).r1..
-00001c80: 0072 3500 0000 da07 6d65 7373 6167 6572  .r5.....messager
-00001c90: 3200 0000 7232 0000 0072 3300 0000 da0e  2...r2...r3.....
-00001ca0: 696e 6974 6961 6c5f 6368 6563 6b73 6200  initial_checksb.
-00001cb0: 0000 734e 0000 0006 0108 0108 0104 0110  ..sN............
-00001cc0: 050c 0204 0110 0306 0302 ff04 0202 fe04  ................
-00001cd0: 0410 0406 0104 0110 0412 0206 0102 ff04  ................
-00001ce0: 0310 0306 0202 ff06 0202 fe08 0404 0110  ................
-00001cf0: 080e 0104 0110 0306 0202 ff04 0202 fe04  ................
-00001d00: 0414 0308 f97a 1742 6c75 6543 6173 742e  .....z.BlueCast.
-00001d10: 696e 6974 6961 6c5f 6368 6563 6b73 da0a  initial_checks..
-00001d20: 7461 7267 6574 5f63 6f6c 6303 0000 0000  target_colc.....
-00001d30: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
-00001d40: 0000 0073 1e03 0000 7400 8300 0100 7401  ...s....t.....t.
-00001d50: 8300 7d03 7c03 a002 7c01 a101 7d01 7c03  ..}.|...|...}.|.
-00001d60: 7c00 5f03 7c00 6a03 6a04 7229 7c00 6a05  |._.|.j.j.r)|.j.
-00001d70: 7c00 6a03 6a04 7600 7229 7406 8300 7c00  |.j.j.v.r)t...|.
-00001d80: 5f07 7c00 6a07 a008 7c01 7c00 6a05 1900  _.|.j...|.|.j...
-00001d90: a101 7c01 7c00 6a05 3c00 7c00 6a03 6a04  ..|.|.j.<.|.j.j.
-00001da0: 7c00 5f04 7c00 6a03 6a09 7c00 5f09 7c00  |._.|.j.j.|._.|.
-00001db0: 6a0a 733a 740b 8300 7c00 5f0a 7c00 a00c  j.s:t...|._.|...
-00001dc0: 7c01 a101 0100 740d 7c01 7c02 7c00 6a0e  |.....t.|.|.|.j.
-00001dd0: 7c00 6a0a 6a0f 7c00 6a0a 6a10 7c00 6a0a  |.j.j.|.j.j.|.j.
-00001de0: 6a11 8306 5c04 7d04 7d05 7d06 7d07 7c00  j...\.}.}.}.}.|.
-00001df0: 6a12 7297 7c00 6a12 a013 7c04 7c06 a102  j.r.|.j...|.|...
-00001e00: 5c02 7d04 7d06 7c00 6a12 6a14 7c05 7c07  \.}.}.|.j.j.|.|.
-00001e10: 6401 6402 8d03 5c02 7d05 7d07 7401 8300  d.d...\.}.}.t...
-00001e20: 7d03 7c03 a002 7c04 a101 7d08 7c04 6a15  }.|...|...}.|.j.
-00001e30: 6403 6404 8d01 7c06 6a15 6403 6404 8d01  d.d...|.j.d.d...
-00001e40: 0202 7d04 7d06 7c05 6a15 6403 6404 8d01  ..}.}.|.j.d.d...
-00001e50: 7c07 6a15 6403 6404 8d01 0202 7d05 7d07  |.j.d.d.....}.}.
-00001e60: 7c02 7c03 6a04 7600 7297 7c03 6a04 a016  |.|.j.v.r.|.j...
-00001e70: 7c02 a101 0100 7417 7c04 8301 7417 7c05  |.....t.|...t.|.
-00001e80: 8301 0202 7d04 7d05 7418 7c04 7c00 6a09  ....}.}.t.|.|.j.
-00001e90: 8302 7418 7c05 7c00 6a09 8302 0202 7d04  ..t.|.|.j.....}.
-00001ea0: 7d05 7419 8300 7c00 5f1a 7c00 6a1a a01b  }.t...|._.|.j...
-00001eb0: 7c04 a101 0100 7c00 6a1a a014 7c05 a101  |.....|.j...|...
-00001ec0: 7d05 7c00 6a04 6405 7501 72df 7c00 6a1c  }.|.j.d.u.r.|.j.
-00001ed0: 6406 6b02 72df 7c00 6a0a 6a1d 73df 741e  d.k.r.|.j.j.s.t.
-00001ee0: 7c03 6a04 8301 7c00 5f1f 7c00 6a1f a020  |.j...|._.|.j.. 
-00001ef0: 7c04 7c06 a102 7d04 7c00 6a1f a021 7c05  |.|...}.|.j..!|.
-00001f00: a101 7d05 6e40 7c00 6a04 6405 7501 9001  ..}.n@|.j.d.u...
-00001f10: 7204 7c00 6a1c 6407 6b02 9001 7204 7c00  r.|.j.d.k...r.|.
-00001f20: 6a0a 6a1d 9001 7304 7422 7c03 6a04 8301  j.j...s.t"|.j...
-00001f30: 7c00 5f1f 7c00 6a1f a023 7c04 7c06 a102  |._.|.j..#|.|...
-00001f40: 7d04 7c00 6a1f a024 7c05 a101 7d05 6e1b  }.|.j..$|...}.n.
-00001f50: 7c00 6a0a 6a1d 9001 721f 7c04 7c00 6a04  |.j.j...r.|.|.j.
-00001f60: 1900 a025 6408 a101 7c04 7c00 6a04 3c00  ...%d...|.|.j.<.
-00001f70: 7c05 7c00 6a04 1900 a025 6408 a101 7c05  |.|.j....%d...|.
-00001f80: 7c00 6a04 3c00 7c00 6a26 9001 7237 7c00  |.j.<.|.j&..r7|.
-00001f90: 6a26 a013 7c04 7c06 a102 5c02 7d04 7d06  j&..|.|...\.}.}.
-00001fa0: 7c00 6a26 6a14 7c05 7c07 6401 6402 8d03  |.j&j.|.|.d.d...
-00001fb0: 5c02 7d05 7d07 7c00 6a27 9001 7346 7428  \.}.}.|.j'..sFt(
-00001fc0: 7c00 6a0a 6a10 7c00 6a0a 6a29 6409 8d02  |.j.j.|.j.j)d...
-00001fd0: 7c00 5f27 7c00 6a0a 6a2a 9001 725e 7c00  |._'|.j.j*..r^|.
-00001fe0: 6a27 a013 7c04 7c06 a102 5c02 7d04 7d06  j'..|.|...\.}.}.
-00001ff0: 7c00 6a27 6a14 7c05 6401 6402 8d02 5c02  |.j'j.|.d.d...\.
-00002000: 7d05 7d08 7c00 6a2b 9001 736f 742c 7c00  }.}.|.j+..sot,|.
-00002010: 6a1c 7c00 6a0a 7c00 6a2d 7c00 6a2e 640a  j.|.j.|.j-|.j.d.
-00002020: 8d04 7c00 5f2b 7c00 6a2b a01b 7c04 7c05  ..|._+|.j+..|.|.
-00002030: 7c06 7c07 a104 0100 7c00 6a0a 9001 728a  |.|.....|.j...r.
-00002040: 7c00 6a0a 6a2f 9001 728a 7430 7c00 6a2b  |.j.j/..r.t0|.j+
-00002050: 6a31 7c05 640b 8303 7c00 5f32 6403 7c00  j1|.d...|._2d.|.
-00002060: 5f33 6405 5300 290c 7a19 5472 6169 6e20  _3d.S.).z.Train 
-00002070: 6120 6675 6c6c 204d 4c20 7069 7065 6c69  a full ML pipeli
-00002080: 6e65 2e46 a901 da0e 7072 6564 6963 746f  ne.F....predicto
-00002090: 6e5f 6d6f 6465 54a9 01da 0464 726f 704e  n_modeT....dropN
-000020a0: 721e 0000 0072 1f00 0000 da08 6361 7465  r....r......cate
-000020b0: 676f 7279 2902 da0c 7261 6e64 6f6d 5f73  gory)...random_s
-000020c0: 7461 7465 723f 0000 0029 0372 2800 0000  tater?...).r(...
-000020d0: 7229 0000 0072 2a00 0000 da04 7472 6565  r)...r*.....tree
-000020e0: 2934 720f 0000 0072 1600 0000 5a1b 6669  )4r....r....Z.fi
-000020f0: 745f 7472 616e 7366 6f72 6d5f 6665 6174  t_transform_feat
-00002100: 7572 655f 7479 7065 7372 2c00 0000 7221  ure_typesr,...r!
-00002110: 0000 0072 2000 0000 7214 0000 0072 2e00  ...r ...r....r..
-00002120: 0000 5a1b 6669 745f 7472 616e 7366 6f72  ..Z.fit_transfor
-00002130: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
-00002140: 2200 0000 7228 0000 0072 0a00 0000 7245  "...r(...r....rE
-00002150: 0000 0072 1b00 0000 7223 0000 00da 0a74  ...r....r#.....t
-00002160: 7261 696e 5f73 697a 655a 1367 6c6f 6261  rain_sizeZ.globa
-00002170: 6c5f 7261 6e64 6f6d 5f73 7461 7465 5a14  l_random_stateZ.
-00002180: 7472 6169 6e5f 7370 6c69 745f 7374 7261  train_split_stra
-00002190: 7469 6679 7226 0000 00da 0d66 6974 5f74  tifyr&.....fit_t
-000021a0: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
-000021b0: 6f72 6dda 0b72 6573 6574 5f69 6e64 6578  orm..reset_index
-000021c0: da06 7265 6d6f 7665 7217 0000 0072 1300  ..remover....r..
-000021d0: 0000 7218 0000 0072 2f00 0000 da03 6669  ..r....r/.....fi
-000021e0: 7472 1d00 0000 7242 0000 0072 1900 0000  tr....rB...r....
-000021f0: 722d 0000 005a 1e66 6974 5f74 6172 6765  r-...Z.fit_targe
-00002200: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
-00002210: 636c 6173 73da 2474 7261 6e73 666f 726d  class.$transform
-00002220: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
-00002230: 696e 6172 795f 636c 6173 7372 1a00 0000  inary_classr....
-00002240: 5a1c 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
-00002250: 6f64 655f 6d75 6c74 6963 6c61 7373 da22  ode_multiclass."
-00002260: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
-00002270: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
-00002280: 7373 da06 6173 7479 7065 7225 0000 0072  ss..astyper%...r
-00002290: 2700 0000 7215 0000 0072 3f00 0000 723a  '...r....r?...r:
-000022a0: 0000 0072 2400 0000 7211 0000 0072 2900  ...r$...r....r).
-000022b0: 0000 722a 0000 0072 4300 0000 720e 0000  ..r*...rC...r...
-000022c0: 00da 056d 6f64 656c 7230 0000 0072 2b00  ...modelr0...r+.
-000022d0: 0000 2909 7231 0000 0072 3500 0000 7246  ..).r1...r5...rF
-000022e0: 0000 0072 2c00 0000 da07 785f 7472 6169  ...r,.....x_trai
-000022f0: 6eda 0678 5f74 6573 74da 0779 5f74 7261  n..x_test..y_tra
-00002300: 696e da06 795f 7465 7374 da01 5f72 3200  in..y_test.._r2.
-00002310: 0000 7232 0000 0072 3300 0000 7253 0000  ..r2...r3...rS..
-00002320: 00a6 0000 0073 be00 0000 0602 0601 0a01  .....s..........
-00002330: 0601 0802 0e01 0801 0603 0801 02ff 02fe  ................
-00002340: 0401 02ff 0a06 0a01 0602 0801 0a02 0202  ................
-00002350: 0201 0201 0401 0601 0601 0601 0cfa 0609  ................
-00002360: 1201 0601 0601 0aff 0603 0a01 0e01 0201  ................
-00002370: 0aff 0e03 0201 0aff 0a03 0c01 1202 0c01  ................
-00002380: 0601 08ff 0804 0c01 0c01 0a03 0a01 0601  ................
-00002390: 02ff 0c03 0e01 0e01 0c02 0c01 0601 04ff  ................
-000023a0: 0c03 0e01 0e01 0a01 1601 1601 0802 0601  ................
-000023b0: 0401 08ff 0603 0601 0aff 0804 0201 0601  ................
-000023c0: 0601 08fe 0a05 0601 0401 08ff 0603 0401  ................
-000023d0: 0aff 0804 0201 0401 0401 0401 0401 08fc  ................
-000023e0: 1206 1201 1201 0a01 7a0c 426c 7565 4361  ........z.BlueCa
-000023f0: 7374 2e66 6974 da07 6466 5f65 7661 6cda  st.fit..df_eval.
-00002400: 0b74 6172 6765 745f 6576 616c 6305 0000  .target_evalc...
-00002410: 0000 0000 0000 0000 0008 0000 0004 0000  ................
-00002420: 0043 0000 0073 2c00 0000 7c00 a000 7c01  .C...s,...|...|.
-00002430: 7c04 a102 0100 7c00 a001 7c02 a101 5c02  |.....|...|...\.
-00002440: 7d05 7d06 7402 7c03 6a03 7c05 7c06 8303  }.}.t.|.j.|.|...
-00002450: 7d07 7c07 5300 2901 618e 0200 0054 7261  }.|.S.).a....Tra
-00002460: 696e 2061 2066 756c 6c20 4d4c 2070 6970  in a full ML pip
-00002470: 656c 696e 6520 616e 6420 6576 616c 7561  eline and evalua
-00002480: 7465 206f 6e20 6120 686f 6c64 6f75 7420  te on a holdout 
-00002490: 7365 742e 0a0a 2020 2020 2020 2020 5468  set...        Th
-000024a0: 6973 2069 7320 6120 636f 6e76 656e 6965  is is a convenie
-000024b0: 6e63 6520 6675 6e63 7469 6f6e 2074 6f20  nce function to 
-000024c0: 7472 6169 6e20 616e 6420 6576 616c 7561  train and evalua
-000024d0: 7465 206f 6e20 6120 686f 6c64 6f75 7420  te on a holdout 
-000024e0: 7365 742e 2049 7420 6973 2072 6563 6f6d  set. It is recom
-000024f0: 6d65 6e64 6564 2074 6f20 7573 6520 7468  mended to use th
-00002500: 6973 2066 6f72 206d 6f64 656c 0a20 2020  is for model.   
-00002510: 2020 2020 2065 7870 6c6f 7261 7469 6f6e       exploration
-00002520: 2e20 4f6e 2070 726f 6475 6374 696f 6e20  . On production 
-00002530: 7468 6520 7369 6d70 6c65 2066 6974 2829  the simple fit()
-00002540: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
-00002550: 2062 6520 7573 6564 2e0a 2020 2020 2020   be used..      
-00002560: 2020 3a70 6172 616d 203a 6466 3a20 5461    :param :df: Ta
-00002570: 6b65 7320 6120 7061 6e64 6173 2044 6174  kes a pandas Dat
-00002580: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
-00002590: 6720 7468 6520 7472 6169 6e69 6e67 2064  g the training d
-000025a0: 6174 6120 616e 6420 7468 6520 7461 7267  ata and the targ
-000025b0: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
-000025c0: 7261 6d20 3a64 665f 6576 616c 3a20 5461  ram :df_eval: Ta
-000025d0: 6b65 7320 6120 7061 6e64 6173 2044 6174  kes a pandas Dat
-000025e0: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
-000025f0: 6720 7468 6520 6576 616c 7561 7469 6f6e  g the evaluation
-00002600: 2064 6174 612c 2062 7574 206e 6f74 2074   data, but not t
-00002610: 6865 2074 6172 6765 7473 2e0a 2020 2020  he targets..    
-00002620: 2020 2020 3a70 6172 616d 203a 7461 7267      :param :targ
-00002630: 6574 5f65 7661 6c3a 2054 616b 6573 2061  et_eval: Takes a
-00002640: 2070 616e 6461 7320 5365 7269 6573 2063   pandas Series c
-00002650: 6f6e 7461 696e 696e 6720 7468 6520 6576  ontaining the ev
-00002660: 616c 7561 7469 6f6e 2074 6172 6765 7473  aluation targets
-00002670: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002680: 203a 7461 7267 6574 5f63 6f6c 3a20 5461   :target_col: Ta
-00002690: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
-000026a0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
-000026b0: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
-000026c0: 6f6c 756d 6e20 696e 7369 6465 2074 6865  olumn inside the
-000026d0: 2074 7261 696e 696e 6720 6461 7461 2064   training data d
-000026e0: 662e 0a20 2020 2020 2020 2029 0472 5300  f..        ).rS.
-000026f0: 0000 da07 7072 6564 6963 7472 0d00 0000  ....predictr....
-00002700: da06 7661 6c75 6573 2908 7231 0000 0072  ..values).r1...r
-00002710: 3500 0000 725d 0000 0072 5e00 0000 7246  5...r]...r^...rF
-00002720: 0000 00da 0779 5f70 726f 6273 da09 795f  .....y_probs..y_
-00002730: 636c 6173 7365 735a 0965 7661 6c5f 6469  classesZ.eval_di
-00002740: 6374 7232 0000 0072 3200 0000 7233 0000  ctr2...r2...r3..
-00002750: 00da 0866 6974 5f65 7661 6c16 0100 0073  ...fit_eval....s
-00002760: 0800 0000 0c10 0e01 0e01 0401 7a11 426c  ............z.Bl
-00002770: 7565 4361 7374 2e66 6974 5f65 7661 6c63  ueCast.fit_evalc
-00002780: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00002790: 0400 0000 4300 0000 7350 0100 0074 0083  ....C...sP...t..
-000027a0: 0001 007c 006a 0173 0a74 0264 0183 0182  ...|.j.s.t.d....
-000027b0: 017c 006a 0373 1174 0264 0283 0182 017c  .|.j.s.t.d.....|
-000027c0: 006a 016a 047c 017c 006a 0567 0164 038d  .j.j.|.|.j.g.d..
-000027d0: 027d 017c 006a 0672 2e7c 006a 066a 077c  .}.|.j.r.|.j.j.|
-000027e0: 0164 0464 058d 025c 027d 017d 027c 016a  .d.d...\.}.}.|.j
-000027f0: 0864 0464 068d 017d 0174 097c 0183 017d  .d.d...}.t.|...}
-00002800: 0174 0a7c 017c 006a 0b83 027d 017c 006a  .t.|.|.j...}.|.j
-00002810: 0c72 417c 006a 0ca0 077c 01a1 017d 017c  .rA|.j...|...}.|
-00002820: 006a 0d72 5d7c 006a 0e72 5d7c 006a 0f64  .j.r]|.j.r]|.j.d
-00002830: 076b 0272 5d74 107c 006a 0e74 1183 0272  .k.r]t.|.j.t...r
-00002840: 5d7c 006a 036a 1273 5d7c 006a 0ea0 137c  ]|.j.j.s]|.j...|
-00002850: 01a1 017d 016e 2b7c 006a 0d72 797c 006a  ...}.n+|.j.ry|.j
-00002860: 0e72 797c 006a 0f64 086b 0272 7974 107c  .ry|.j.d.k.ryt.|
-00002870: 006a 0e74 1483 0272 797c 006a 036a 1273  .j.t...ry|.j.j.s
-00002880: 797c 006a 0ea0 157c 01a1 017d 016e 0f7c  y|.j...|...}.n.|
-00002890: 006a 036a 1272 887c 017c 006a 0d19 00a0  .j.j.r.|.|.j....
-000028a0: 1664 09a1 017c 017c 006a 0d3c 007c 006a  .d...|.|.j.<.|.j
-000028b0: 1772 957c 006a 176a 077c 0164 0464 058d  .r.|.j.j.|.d.d..
-000028c0: 025c 027d 017d 027c 006a 1872 a67c 006a  .\.}.}.|.j.r.|.j
-000028d0: 036a 1972 a67c 006a 186a 077c 0164 0464  .j.r.|.j.j.|.d.d
-000028e0: 058d 025c 027d 017d 027c 0153 0029 0a7a  ...\.}.}.|.S.).z
-000028f0: 3754 7261 6e73 666f 726d 206e 6577 2064  7Transform new d
-00002900: 6174 6120 6163 636f 7264 696e 6720 746f  ata according to
-00002910: 2070 7265 7072 6f63 6573 7369 6e67 2070   preprocessing p
-00002920: 6970 656c 696e 652e fa2a 4665 6174 7572  ipeline..*Featur
-00002930: 6520 7479 7065 2063 6f6e 7665 7274 6572  e type converter
-00002940: 2063 6f75 6c64 206e 6f74 2062 6520 666f   could not be fo
-00002950: 756e 642e 7a2a 5472 6169 6e69 6e67 2063  und.z*Training c
-00002960: 6f6e 6669 6775 7261 7469 6f6e 2063 6f75  onfiguration cou
-00002970: 6c64 206e 6f74 2062 6520 666f 756e 642e  ld not be found.
-00002980: 2901 5a0b 6967 6e6f 7265 5f63 6f6c 7354  ).Z.ignore_colsT
-00002990: 7247 0000 0072 4900 0000 721e 0000 0072  rG...rI...r....r
-000029a0: 1f00 0000 724b 0000 0029 1a72 0f00 0000  ....rK...).r....
-000029b0: 722c 0000 00da 0945 7863 6570 7469 6f6e  r,.....Exception
-000029c0: 7228 0000 005a 1774 7261 6e73 666f 726d  r(...Z.transform
-000029d0: 5f66 6561 7475 7265 5f74 7970 6573 7220  _feature_typesr 
-000029e0: 0000 0072 2600 0000 7250 0000 0072 5100  ...r&...rP...rQ.
-000029f0: 0000 7217 0000 0072 1300 0000 7222 0000  ..r....r....r"..
-00002a00: 0072 2f00 0000 7221 0000 0072 2d00 0000  .r/...r!...r-...
-00002a10: 721d 0000 00da 0a69 7369 6e73 7461 6e63  r......isinstanc
-00002a20: 6572 1900 0000 7242 0000 0072 5400 0000  er....rB...rT...
-00002a30: 721a 0000 0072 5500 0000 7256 0000 0072  r....rU...rV...r
-00002a40: 2500 0000 7227 0000 0072 3a00 0000 2903  %...r'...r:...).
-00002a50: 7231 0000 0072 3500 0000 725c 0000 0072  r1...r5...r\...r
-00002a60: 3200 0000 7232 0000 0072 3300 0000 da12  2...r2...r3.....
-00002a70: 7472 616e 7366 6f72 6d5f 6e65 775f 6461  transform_new_da
-00002a80: 7461 2b01 0000 7354 0000 0006 0206 0108  ta+...sT........
-00002a90: 0106 0208 0106 0208 0106 ff06 0414 010c  ................
-00002aa0: 0108 020c 0106 020c 0104 0302 ff04 0202  ................
-00002ab0: fe0a 030a 0102 ff06 0202 fe0e 0404 0202  ................
-00002ac0: ff04 0202 fe0a 030a 0102 ff06 0202 fe0e  ................
-00002ad0: 0408 0116 0106 0214 010e 0214 0104 027a  ...............z
-00002ae0: 1b42 6c75 6543 6173 742e 7472 616e 7366  .BlueCast.transf
-00002af0: 6f72 6d5f 6e65 775f 6461 7461 6302 0000  orm_new_datac...
-00002b00: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-00002b10: 0043 0000 0073 9800 0000 7c00 6a00 7307  .C...s....|.j.s.
-00002b20: 7401 6401 8301 8201 7c00 6a02 730e 7401  t.d.....|.j.s.t.
-00002b30: 6402 8301 8201 7c00 6a03 7315 7404 6403  d.....|.j.s.t.d.
-00002b40: 8301 8201 7405 8300 0100 7c00 a006 7c01  ....t.....|...|.
-00002b50: a101 7d01 7407 7408 a009 a100 9b00 6404  ..}.t.t.......d.
-00002b60: 9d02 8301 0100 7c00 6a00 a00a 7c01 a101  ......|.j...|...
-00002b70: 5c02 7d02 7d03 7c00 6a02 6a0b 7248 7c00  \.}.}.|.j.j.rH|.
-00002b80: 6a0c 7c00 6a02 6a0b 7600 7248 7c00 6a0d  j.|.j.j.v.rH|.j.
-00002b90: 7248 7c00 6a02 7248 7c00 6a0d a00e 740f  rH|.j.rH|.j...t.
-00002ba0: a010 7c03 a101 a101 7d03 7c02 7c03 6602  ..|.....}.|.|.f.
-00002bb0: 5300 2905 7a90 5072 6564 6963 7420 6f6e  S.).z.Predict on
-00002bc0: 2075 6e73 6565 6e20 6461 7461 2e0a 0a20   unseen data... 
-00002bd0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-00002be0: 6520 7072 6564 6963 7465 6420 7072 6f62  e predicted prob
-00002bf0: 6162 696c 6974 6965 7320 616e 6420 7468  abilities and th
-00002c00: 6520 7072 6564 6963 7465 6420 636c 6173  e predicted clas
-00002c10: 7365 733a 0a20 2020 2020 2020 2079 5f70  ses:.        y_p
-00002c20: 726f 6273 2c20 795f 636c 6173 7365 7320  robs, y_classes 
-00002c30: 3d20 7072 6564 6963 7428 6466 290a 2020  = predict(df).  
-00002c40: 2020 2020 2020 7a1b 4d6c 206d 6f64 656c        z.Ml model
-00002c50: 2063 6f75 6c64 206e 6f74 2062 6520 666f   could not be fo
-00002c60: 756e 6472 6400 0000 7a15 636f 6e66 5f74  undrd...z.conf_t
-00002c70: 7261 696e 696e 6720 6973 204e 6f6e 657a  raining is Nonez
-00002c80: 0f3a 2050 7265 6469 6374 696e 672e 2e2e  .: Predicting...
-00002c90: 2911 7224 0000 0072 6500 0000 722c 0000  ).r$...re...r,..
-00002ca0: 0072 2800 0000 da0a 5661 6c75 6545 7272  .r(.....ValueErr
-00002cb0: 6f72 720f 0000 0072 6700 0000 7210 0000  orr....rg...r...
-00002cc0: 0072 0200 0000 da06 7574 636e 6f77 725f  .r......utcnowr_
-00002cd0: 0000 0072 2100 0000 7220 0000 0072 2e00  ...r!...r ...r..
-00002ce0: 0000 5a1f 6c61 6265 6c5f 656e 636f 6465  ..Z.label_encode
-00002cf0: 725f 7265 7665 7273 655f 7472 616e 7366  r_reverse_transf
-00002d00: 6f72 6dda 0270 64da 0653 6572 6965 7329  orm..pd..Series)
-00002d10: 0472 3100 0000 7235 0000 0072 6100 0000  .r1...r5...ra...
-00002d20: 7262 0000 0072 3200 0000 7232 0000 0072  rb...r2...r2...r
-00002d30: 3300 0000 725f 0000 005d 0100 0073 2800  3...r_...]...s(.
-00002d40: 0000 0606 0801 0602 0801 0602 0801 0602  ................
-00002d50: 0a01 1202 1001 0802 0e02 0401 02ff 0402  ................
-00002d60: 02fe 0604 0801 04ff 0804 7a10 426c 7565  ..........z.Blue
-00002d70: 4361 7374 2e70 7265 6469 6374 290a 4e4e  Cast.predict).NN
-00002d80: 4e4e 4e4e 4e4e 4e4e 291f da08 5f5f 6e61  NNNNNNNN)...__na
-00002d90: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00002da0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00002db0: 5f5f 646f 635f 5f72 0600 0000 7209 0000  __doc__r....r...
-00002dc0: 00da 0373 7472 da05 666c 6f61 74da 0369  ...str..float..i
-00002dd0: 6e74 7207 0000 0072 0500 0000 7211 0000  ntr....r....r...
-00002de0: 0072 0300 0000 7212 0000 0072 1500 0000  .r....r....r....
-00002df0: 720a 0000 0072 0c00 0000 720b 0000 0072  r....r....r....r
-00002e00: 3400 0000 726a 0000 00da 0944 6174 6146  4...rj.....DataF
-00002e10: 7261 6d65 7245 0000 0072 5300 0000 726b  ramerE...rS...rk
-00002e20: 0000 0072 0400 0000 7263 0000 0072 6700  ...r....rc...rg.
-00002e30: 0000 7208 0000 00da 026e 70da 076e 6461  ..r......np..nda
-00002e40: 7272 6179 725f 0000 0072 3200 0000 7232  rrayr_...r2...r2
-00002e50: 0000 0072 3200 0000 7233 0000 0072 1c00  ...r2...r3...r..
-00002e60: 0000 2700 0000 736c 0000 0008 0004 0102  ..'...sl........
-00002e70: 1802 0102 0102 0102 0102 0102 0302 0102  ................
-00002e80: 0102 0104 f106 0202 fe0c 0302 fd14 0402  ................
-00002e90: fc14 0502 fb06 0602 fa0e 0702 f906 0802  ................
-00002ea0: f806 0902 f702 0a0a 0102 ff02 f606 0d02  ................
-00002eb0: f306 0e02 f206 0f0a f114 2618 4402 7004  ..........&.D.p.
-00002ec0: 0202 fe04 0302 fd04 0402 fc02 0502 fb0a  ................
-00002ed0: 060a fa16 1524 3272 1c00 0000 2930 726f  .....$2r....)0ro
-00002ee0: 0000 0072 3b00 0000 7202 0000 00da 0674  ...r;...r......t
-00002ef0: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
-00002f00: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
-00002f10: 0000 0072 0900 0000 da05 6e75 6d70 7972  ...r......numpyr
-00002f20: 7400 0000 da06 7061 6e64 6173 726a 0000  t.....pandasrj..
-00002f30: 00da 1f62 6c75 6563 6173 742e 636f 6e66  ...bluecast.conf
-00002f40: 6967 2e74 7261 696e 696e 675f 636f 6e66  ig.training_conf
-00002f50: 6967 720a 0000 0072 0b00 0000 720c 0000  igr....r....r...
-00002f60: 005a 2062 6c75 6563 6173 742e 6576 616c  .Z bluecast.eval
-00002f70: 7561 7469 6f6e 2e65 7661 6c5f 6d65 7472  uation.eval_metr
-00002f80: 6963 7372 0d00 0000 5a1f 626c 7565 6361  icsr....Z.blueca
-00002f90: 7374 2e65 7661 6c75 6174 696f 6e2e 7368  st.evaluation.sh
-00002fa0: 6170 5f76 616c 7565 7372 0e00 0000 5a24  ap_valuesr....Z$
-00002fb0: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
-00002fc0: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
-00002fd0: 7469 6c73 720f 0000 0072 1000 0000 5a1d  tilsr....r....Z.
-00002fe0: 626c 7565 6361 7374 2e6d 6c5f 6d6f 6465  bluecast.ml_mode
-00002ff0: 6c6c 696e 672e 7867 626f 6f73 7472 1100  lling.xgboostr..
-00003000: 0000 da1d 626c 7565 6361 7374 2e70 7265  ....bluecast.pre
-00003010: 7072 6f63 6573 7369 6e67 2e63 7573 746f  processing.custo
-00003020: 6d72 1200 0000 5a28 626c 7565 6361 7374  mr....Z(bluecast
-00003030: 2e70 7265 7072 6f63 6573 7369 6e67 2e64  .preprocessing.d
-00003040: 6174 6574 696d 655f 6665 6174 7572 6573  atetime_features
-00003050: 7213 0000 005a 2b62 6c75 6563 6173 742e  r....Z+bluecast.
-00003060: 7072 6570 726f 6365 7373 696e 672e 656e  preprocessing.en
-00003070: 636f 6465 5f74 6172 6765 745f 6c61 6265  code_target_labe
-00003080: 6c73 7214 0000 005a 2862 6c75 6563 6173  lsr....Z(bluecas
-00003090: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
-000030a0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
-000030b0: 6e72 1500 0000 5a24 626c 7565 6361 7374  nr....Z$bluecast
-000030c0: 2e70 7265 7072 6f63 6573 7369 6e67 2e66  .preprocessing.f
-000030d0: 6561 7475 7265 5f74 7970 6573 7216 0000  eature_typesr...
-000030e0: 005a 2562 6c75 6563 6173 742e 7072 6570  .Z%bluecast.prep
-000030f0: 726f 6365 7373 696e 672e 6e75 6c6c 735f  rocessing.nulls_
-00003100: 616e 645f 696e 6673 7217 0000 005a 2462  and_infsr....Z$b
-00003110: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00003120: 7373 696e 672e 7363 6865 6d61 5f63 6865  ssing.schema_che
-00003130: 636b 7372 1800 0000 5a26 626c 7565 6361  cksr....Z&blueca
-00003140: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00003150: 2e74 6172 6765 745f 656e 636f 6469 6e67  .target_encoding
-00003160: 7219 0000 0072 1a00 0000 5a27 626c 7565  r....r....Z'blue
-00003170: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
-00003180: 6e67 2e74 7261 696e 5f74 6573 745f 7370  ng.train_test_sp
-00003190: 6c69 7472 1b00 0000 721c 0000 0072 3200  litr....r....r2.
-000031a0: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
-000031b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000031c0: 2a00 0000 0400 0808 0c01 2401 0802 0801  *.........$.....
-000031d0: 1402 0c05 0c01 1001 0c01 0c01 0c01 0c01  ................
-000031e0: 0c01 0c01 0c01 0c01 1001 0c04 1203       ..............
+000008d0: 7220 7468 6573 6520 6175 746f 6d61 7469  r these automati
+000008e0: 6361 6c6c 792e 0a20 2020 203a 7061 7261  cally..    :para
+000008f0: 6d20 3a64 6174 655f 636f 6c75 6d6e 733a  m :date_columns:
+00000900: 2054 616b 6573 2061 206c 6973 7420 6f66   Takes a list of
+00000910: 2073 7472 696e 6773 2063 6f6e 7461 696e   strings contain
+00000920: 696e 6720 7468 6520 6e61 6d65 7320 6f66  ing the names of
+00000930: 2074 6865 2064 6174 6520 636f 6c75 6d6e   the date column
+00000940: 732e 2049 6620 6e6f 7420 7072 6f76 6964  s. If not provid
+00000950: 6564 2c0a 2020 2020 426c 7565 4361 7374  ed,.    BlueCast
+00000960: 2077 696c 6c20 696e 6665 7220 7468 6573   will infer thes
+00000970: 6520 6175 746f 6d61 7469 6361 6c6c 792e  e automatically.
+00000980: 0a20 2020 203a 7061 7261 6d20 3a74 696d  .    :param :tim
+00000990: 655f 7370 6c69 745f 636f 6c75 6d6e 3a20  e_split_column: 
+000009a0: 5461 6b65 7320 6120 7374 7269 6e67 2063  Takes a string c
+000009b0: 6f6e 7461 696e 696e 6720 7468 6520 6e61  ontaining the na
+000009c0: 6d65 206f 6620 7468 6520 7469 6d65 2073  me of the time s
+000009d0: 706c 6974 2063 6f6c 756d 6e2e 2049 6620  plit column. If 
+000009e0: 6e6f 7420 7072 6f76 6964 6564 2c0a 2020  not provided,.  
+000009f0: 2020 426c 7565 4361 7374 2077 696c 6c20    BlueCast will 
+00000a00: 6e6f 7420 7370 6c69 7420 7468 6520 6461  not split the da
+00000a10: 7461 2062 7920 7469 6d65 206f 7220 6f72  ta by time or or
+00000a20: 6465 722c 2062 7574 2064 6f20 6120 7261  der, but do a ra
+00000a30: 6e64 6f6d 2073 706c 6974 2069 6e73 7465  ndom split inste
+00000a40: 6164 2e0a 2020 2020 3a70 6172 616d 203a  ad..    :param :
+00000a50: 6d6c 5f6d 6f64 656c 3a20 5461 6b65 7320  ml_model: Takes 
+00000a60: 616e 2069 6e73 7461 6e63 6520 6f66 2061  an instance of a
+00000a70: 2058 6762 6f6f 7374 4d6f 6465 6c20 636c   XgboostModel cl
+00000a80: 6173 732e 2049 6620 6e6f 7420 7072 6f76  ass. If not prov
+00000a90: 6964 6564 2c20 426c 7565 4361 7374 2077  ided, BlueCast w
+00000aa0: 696c 6c20 696e 7374 616e 7469 6174 6520  ill instantiate 
+00000ab0: 6f6e 652e 0a20 2020 2054 6869 7320 6973  one..    This is
+00000ac0: 2061 6e20 4150 4920 746f 2070 6173 7320   an API to pass 
+00000ad0: 616e 7920 6d6f 6465 6c20 636c 6173 732e  any model class.
+00000ae0: 2049 6e68 6572 6974 2074 6865 2062 6173   Inherit the bas
+00000af0: 6563 6c61 7373 2066 726f 6d20 6d6c 5f6d  eclass from ml_m
+00000b00: 6f64 656c 6c69 6e67 2e62 6173 655f 6d6f  odelling.base_mo
+00000b10: 6465 6c2e 4261 7365 4d6f 6465 6c2e 0a20  del.BaseModel.. 
+00000b20: 2020 203a 7061 7261 6d20 6375 7374 6f6d     :param custom
+00000b30: 5f70 7265 7072 6f63 6573 736f 723a 2054  _preprocessor: T
+00000b40: 616b 6573 2061 6e20 696e 7374 616e 6365  akes an instance
+00000b50: 206f 6620 6120 4375 7374 6f6d 5072 6570   of a CustomPrep
+00000b60: 726f 6365 7373 696e 6720 636c 6173 732e  rocessing class.
+00000b70: 2041 6c6c 6f77 7320 7573 6572 7320 746f   Allows users to
+00000b80: 2069 6e6a 6563 7420 6375 7374 6f6d 0a20   inject custom. 
+00000b90: 2020 2070 7265 7072 6f63 6573 7369 6e67     preprocessing
+00000ba0: 2073 7465 7073 2077 6869 6368 2074 616b   steps which tak
+00000bb0: 6520 706c 6163 6520 7269 6768 7420 6166  e place right af
+00000bc0: 7465 7220 7468 6520 7472 6169 6e20 7465  ter the train te
+00000bd0: 7374 2073 7069 742e 0a20 2020 203a 7061  st spit..    :pa
+00000be0: 7261 6d20 6375 7374 6f6d 5f6c 6173 745f  ram custom_last_
+00000bf0: 6d69 6c65 5f63 6f6d 7075 7461 7469 6f6e  mile_computation
+00000c00: 3a20 5461 6b65 7320 616e 2069 6e73 7461  : Takes an insta
+00000c10: 6e63 6520 6f66 2061 2043 7573 746f 6d50  nce of a CustomP
+00000c20: 7265 7072 6f63 6573 7369 6e67 2063 6c61  reprocessing cla
+00000c30: 7373 2e20 416c 6c6f 7773 2075 7365 7273  ss. Allows users
+00000c40: 2074 6f20 696e 6a65 6374 2063 7573 746f   to inject custo
+00000c50: 6d0a 2020 2020 7072 6570 726f 6365 7373  m.    preprocess
+00000c60: 696e 6720 7374 6570 7320 7768 6963 6820  ing steps which 
+00000c70: 7461 6b65 2070 6c61 6365 2072 6967 6874  take place right
+00000c80: 2062 6566 6f72 6520 7468 6520 6d6f 6465   before the mode
+00000c90: 6c20 7472 6169 6e69 6e67 2e0a 2020 2020  l training..    
+00000ca0: 4eda 0d63 6c61 7373 5f70 726f 626c 656d  N..class_problem
+00000cb0: 2902 da06 6269 6e61 7279 da0a 6d75 6c74  )...binary..mult
+00000cc0: 6963 6c61 7373 da0d 7461 7267 6574 5f63  iclass..target_c
+00000cd0: 6f6c 756d 6eda 0b63 6174 5f63 6f6c 756d  olumn..cat_colum
+00000ce0: 6e73 da0c 6461 7465 5f63 6f6c 756d 6e73  ns..date_columns
+00000cf0: da11 7469 6d65 5f73 706c 6974 5f63 6f6c  ..time_split_col
+00000d00: 756d 6eda 086d 6c5f 6d6f 6465 6cda 1c63  umn..ml_model..c
+00000d10: 7573 746f 6d5f 6c61 7374 5f6d 696c 655f  ustom_last_mile_
+00000d20: 636f 6d70 7574 6174 696f 6eda 1363 7573  computation..cus
+00000d30: 746f 6d5f 7072 6570 726f 6365 7373 6f72  tom_preprocessor
+00000d40: da17 6375 7374 6f6d 5f66 6561 7475 7265  ..custom_feature
+00000d50: 5f73 656c 6563 746f 72da 0d63 6f6e 665f  _selector..conf_
+00000d60: 7472 6169 6e69 6e67 da0c 636f 6e66 5f78  training..conf_x
+00000d70: 6762 6f6f 7374 da13 636f 6e66 5f70 6172  gboost..conf_par
+00000d80: 616d 735f 7867 626f 6f73 7463 0d00 0000  ams_xgboostc....
+00000d90: 0000 0000 0000 0000 0d00 0000 0200 0000  ................
+00000da0: 4300 0000 7370 0000 007c 017c 005f 0064  C...sp...|.|._.d
+00000db0: 017c 005f 017c 037c 005f 027c 047c 005f  .|._.|.|._.|.|._
+00000dc0: 037c 057c 005f 047c 027c 005f 057c 0a7c  .|.|._.|.|._.|.|
+00000dd0: 005f 067c 0b7c 005f 077c 0c7c 005f 0864  ._.|.|._.|.|._.d
+00000de0: 007c 005f 0964 007c 005f 0a64 007c 005f  .|._.d.|._.d.|._
+00000df0: 0b64 007c 005f 0c7c 067c 005f 0d7c 077c  .d.|._.|.|._.|.|
+00000e00: 005f 0e7c 087c 005f 0f7c 097c 005f 1064  ._.|.|._.|.|._.d
+00000e10: 007c 005f 1164 0053 0029 024e 4629 1272  .|._.d.S.).NF).r
+00000e20: 1d00 0000 da0f 7072 6564 6963 7469 6f6e  ......prediction
+00000e30: 5f6d 6f64 6572 2100 0000 7222 0000 0072  _moder!...r"...r
+00000e40: 2300 0000 7220 0000 0072 2800 0000 7229  #...r ...r(...r)
+00000e50: 0000 0072 2a00 0000 da12 6665 6174 5f74  ...r*.....feat_t
+00000e60: 7970 655f 6465 7465 6374 6f72 da0b 6361  ype_detector..ca
+00000e70: 745f 656e 636f 6465 72da 1474 6172 6765  t_encoder..targe
+00000e80: 745f 6c61 6265 6c5f 656e 636f 6465 72da  t_label_encoder.
+00000e90: 0f73 6368 656d 615f 6465 7465 6374 6f72  .schema_detector
+00000ea0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00000eb0: 2700 0000 da0b 7368 6170 5f76 616c 7565  '.....shap_value
+00000ec0: 7329 0dda 0473 656c 6672 1d00 0000 7220  s)...selfr....r 
+00000ed0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+00000ee0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00000ef0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00000f00: 722a 0000 00a9 0072 3200 0000 fa3e 2f68  r*.....r2....>/h
+00000f10: 6f6d 652f 7468 6f6d 6173 2f49 6465 6150  ome/thomas/IdeaP
+00000f20: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
+00000f30: 2f62 6c75 6563 6173 742f 626c 7565 7072  /bluecast/bluepr
+00000f40: 696e 7473 2f63 6173 742e 7079 da08 5f5f  ints/cast.py..__
+00000f50: 696e 6974 5f5f 3c00 0000 7326 0000 0006  init__<...s&....
+00000f60: 1106 0106 0106 0106 0106 0106 0106 0106  ................
+00000f70: 0106 0102 0304 fe06 0306 0106 0106 0106  ................
+00000f80: 0106 010a 017a 1142 6c75 6543 6173 742e  .....z.BlueCast.
+00000f90: 5f5f 696e 6974 5f5f da02 6466 da06 7265  __init__..df..re
+00000fa0: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
+00000fb0: 0003 0000 0005 0000 0043 0000 0073 3001  .........C...s0.
+00000fc0: 0000 7c00 6a00 7307 7401 8300 7c00 5f00  ..|.j.s.t...|._.
+00000fd0: 7c00 6a00 6a02 7315 6401 7d02 7403 6a04  |.j.j.s.d.}.t.j.
+00000fe0: 7c02 7405 6402 6403 8d03 0100 7c00 6a00  |.t.d.d.....|.j.
+00000ff0: 6a06 6404 6b02 7225 6405 7d02 7403 6a04  j.d.k.r%d.}.t.j.
+00001000: 7c02 7405 6402 6403 8d03 0100 7c00 6a00  |.t.d.d.....|.j.
+00001010: 6a02 7236 7c00 6a07 7336 6406 7d02 7403  j.r6|.j.s6d.}.t.
+00001020: 6a04 7c02 7405 6402 6403 8d03 0100 7c00  j.|.t.d.d.....|.
+00001030: 6a08 7343 6407 7d02 7403 6a04 7c02 7405  j.sCd.}.t.j.|.t.
+00001040: 6402 6403 8d03 0100 7c00 6a00 6a09 740a  d.d.....|.j.j.t.
+00001050: 7c01 6a0b 8301 6b05 725a 7c00 6a00 6a02  |.j...k.rZ|.j.j.
+00001060: 725a 6408 7d02 7403 6a04 7c02 7405 6402  rZd.}.t.j.|.t.d.
+00001070: 6403 8d03 0100 7c00 6a00 6a0c 7270 7c00  d.....|.j.j.rp|.
+00001080: 6a00 6a0d 7270 6409 7c00 6a00 5f0d 640a  j.j.rpd.|.j._.d.
+00001090: 7d02 7403 6a04 7c02 7405 6402 6403 8d03  }.t.j.|.t.d.d...
+000010a0: 0100 7c00 6a00 6a0c 7281 7c00 6a0e 7281  ..|.j.j.r.|.j.r.
+000010b0: 640b 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+000010c0: 8d03 0100 7c00 6a00 6a0c 7294 7c00 6a0f  ....|.j.j.r.|.j.
+000010d0: 7296 640c 7d02 7403 6a04 7c02 7405 6402  r.d.}.t.j.|.t.d.
+000010e0: 6403 8d03 0100 6400 5300 6400 5300 6400  d.....d.S.d.S.d.
+000010f0: 5300 290d 4e61 9301 0000 4665 6174 7572  S.).Na....Featur
+00001100: 6520 7365 6c65 6374 696f 6e20 6973 2064  e selection is d
+00001110: 6973 6162 6c65 642e 2055 7064 6174 6520  isabled. Update 
+00001120: 7468 6520 5472 6169 6e69 6e67 436f 6e66  the TrainingConf
+00001130: 6967 2070 6172 616d 2027 656e 6162 6c65  ig param 'enable
+00001140: 5f66 6561 7475 7265 5f73 656c 6563 7469  _feature_selecti
+00001150: 6f6e 270a 2020 2020 2020 2020 2020 2020  on'.            
+00001160: 746f 2065 6e61 626c 6520 6974 206f 7220  to enable it or 
+00001170: 6d61 6b65 2075 7365 206f 6620 6120 6375  make use of a cu
+00001180: 7374 6f6d 2070 7265 7072 6f63 6573 736f  stom preprocesso
+00001190: 7220 746f 2064 6f20 6974 206d 616e 7561  r to do it manua
+000011a0: 6c6c 7920 6475 7269 6e67 2074 6865 206c  lly during the l
+000011b0: 6173 7420 6d69 6c65 2063 6f6d 7075 7461  ast mile computa
+000011c0: 7469 6f6e 7320 7374 6570 2e0a 2020 2020  tions step..    
+000011d0: 2020 2020 2020 2020 4665 6174 7572 6520          Feature 
+000011e0: 7365 6c65 6374 696f 6e20 6973 2072 6563  selection is rec
+000011f0: 6f6d 6d65 6e64 6564 2066 6f72 2064 6174  ommended for dat
+00001200: 6173 6574 7320 7769 7468 206d 616e 7920  asets with many 
+00001210: 6665 6174 7572 6573 2028 3e31 3030 3029  features (>1000)
+00001220: 2e20 466f 7220 6461 7461 7365 7473 2077  . For datasets w
+00001230: 6974 6820 6120 736d 616c 6c20 616d 6f75  ith a small amou
+00001240: 6e74 0a20 2020 2020 2020 2020 2020 206f  nt.            o
+00001250: 6620 6665 6174 7572 6573 2066 6561 7475  f features featu
+00001260: 7265 2073 656c 6563 7469 6f6e 2069 7320  re selection is 
+00001270: 6e6f 7420 7265 636f 6d6d 656e 6465 642e  not recommended.
+00001280: 0a20 2020 2020 2020 2020 2020 20e9 0200  .            ...
+00001290: 0000 2901 da0a 7374 6163 6b6c 6576 656c  ..)...stacklevel
+000012a0: e901 0000 0061 0501 0000 4372 6f73 7320  .....a....Cross 
+000012b0: 7661 6c69 6461 7469 6f6e 2069 7320 6469  validation is di
+000012c0: 7361 626c 6564 2e20 5570 6461 7465 2074  sabled. Update t
+000012d0: 6865 2054 7261 696e 696e 6743 6f6e 6669  he TrainingConfi
+000012e0: 6720 7061 7261 6d20 2768 7970 6572 7475  g param 'hypertu
+000012f0: 6e69 6e67 5f63 765f 666f 6c64 7327 0a20  ning_cv_folds'. 
+00001300: 2020 2020 2020 2020 2020 2074 6f20 656e             to en
+00001310: 6162 6c65 2069 742e 2043 726f 7373 2076  able it. Cross v
+00001320: 616c 6964 6174 696f 6e20 6973 2064 6973  alidation is dis
+00001330: 6162 6c65 6420 6f6e 2064 6566 6175 6c74  abled on default
+00001340: 2074 6f20 616c 6c6f 7720 6661 7374 2070   to allow fast p
+00001350: 726f 746f 7479 7069 6e67 2e20 466f 7220  rototyping. For 
+00001360: 726f 6275 7374 2068 7970 6572 7061 7261  robust hyperpara
+00001370: 6d65 7465 720a 2020 2020 2020 2020 2020  meter.          
+00001380: 2020 7475 6e69 6e67 2075 7369 6e67 2061    tuning using a
+00001390: 7420 6c65 6173 7420 3520 666f 6c64 7320  t least 5 folds 
+000013a0: 6973 2072 6563 6f6d 6d65 6e64 6564 2e61  is recommended.a
+000013b0: 5f01 0000 4665 6174 7572 6520 7365 6c65  _...Feature sele
+000013c0: 6374 696f 6e20 6973 2065 6e61 626c 6564  ction is enabled
+000013d0: 2062 7574 206e 6f20 6665 6174 7572 6520   but no feature 
+000013e0: 7365 6c65 6374 6f72 2068 6173 2062 6565  selector has bee
+000013f0: 6e20 7072 6f76 6964 6564 2e20 4661 6c6c  n provided. Fall
+00001400: 696e 6720 6261 636b 2074 6f0a 2020 2020  ing back to.    
+00001410: 2020 2020 2020 2020 6372 6f73 732d 7661          cross-va
+00001420: 6c69 6461 7465 6420 6665 6174 7572 6520  lidated feature 
+00001430: 656c 696d 696e 6174 696f 6e2e 2053 7065  elimination. Spe
+00001440: 6369 6669 6361 6c6c 7920 666f 7220 736d  cifically for sm
+00001450: 616c 6c20 6461 7461 7365 7473 2063 6865  all datasets che
+00001460: 636b 2074 6865 206c 6f67 7320 746f 2076  ck the logs to v
+00001470: 6572 6966 7920 7468 6174 206e 6f74 2074  erify that not t
+00001480: 6f6f 0a20 2020 2020 2020 2020 2020 206d  oo.            m
+00001490: 616e 7920 6665 6174 7572 6573 2068 6176  any features hav
+000014a0: 6520 6265 656e 2072 656d 6f76 6564 2e20  e been removed. 
+000014b0: 4f74 6865 7277 6973 652c 2063 6f6e 7369  Otherwise, consi
+000014c0: 6465 7220 6469 7361 626c 696e 6720 6665  der disabling fe
+000014d0: 6174 7572 6520 7365 6c65 6374 696f 6e20  ature selection 
+000014e0: 6f72 2070 726f 7669 6469 6e67 2061 2063  or providing a c
+000014f0: 7573 746f 6d0a 2020 2020 2020 2020 2020  ustom.          
+00001500: 2020 6665 6174 7572 6520 7365 6c65 6374    feature select
+00001510: 6f72 2e61 6501 0000 4e6f 2058 6762 6f6f  or.ae...No Xgboo
+00001520: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
+00001530: 6967 2068 6173 2062 6565 6e20 7072 6f76  ig has been prov
+00001540: 6964 6564 2e20 4661 6c6c 696e 6720 6261  ided. Falling ba
+00001550: 636b 2074 6f20 6465 6661 756c 7420 7661  ck to default va
+00001560: 6c75 6573 2e20 4465 6661 756c 7420 7661  lues. Default va
+00001570: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+00001580: 2068 6176 6520 6265 656e 2063 686f 7365   have been chose
+00001590: 6e20 746f 2073 7065 6564 2075 7020 7468  n to speed up th
+000015a0: 6520 7072 6f74 6f74 7970 696e 672e 2046  e prototyping. F
+000015b0: 6f72 2072 6f62 7573 7420 6879 7065 7270  or robust hyperp
+000015c0: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
+000015d0: 636f 6e73 6964 6572 2070 726f 7669 6469  consider providi
+000015e0: 6e67 2061 2063 7573 746f 6d0a 2020 2020  ng a custom.    
+000015f0: 2020 2020 2020 2020 5867 626f 6f73 7454          XgboostT
+00001600: 756e 6550 6172 616d 7343 6f6e 6669 6720  uneParamsConfig 
+00001610: 7769 7468 2061 2064 6565 7065 7220 6879  with a deeper hy
+00001620: 7065 7270 6172 616d 6574 6572 2073 6561  perparameter sea
+00001630: 7263 6820 7370 6163 6520 616e 6420 6120  rch space and a 
+00001640: 6375 7374 6f6d 2054 7261 696e 696e 6743  custom TrainingC
+00001650: 6f6e 6669 6720 746f 2065 6e61 626c 650a  onfig to enable.
+00001660: 2020 2020 2020 2020 2020 2020 6372 6f73              cros
+00001670: 732d 7661 6c69 6461 7469 6f6e 2e61 0f01  s-validation.a..
+00001680: 0000 5468 6520 6d69 6e69 6d75 6d20 6e75  ..The minimum nu
+00001690: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+000016a0: 2074 6f20 7365 6c65 6374 2069 7320 6772   to select is gr
+000016b0: 6561 7465 7220 6f72 2065 7175 616c 2074  eater or equal t
+000016c0: 6f20 7468 6520 6e75 6d62 6572 206f 6620  o the number of 
+000016d0: 6665 6174 7572 6573 2069 6e0a 2020 2020  features in.    
+000016e0: 2020 2020 2020 2020 7468 6520 6461 7461          the data
+000016f0: 7365 7420 7768 696c 6520 6665 6174 7572  set while featur
+00001700: 6520 7365 6c65 6374 696f 6e20 6973 2065  e selection is e
+00001710: 6e61 626c 6564 2e20 436f 6e73 6964 6572  nabled. Consider
+00001720: 2072 6564 7563 696e 6720 7468 6520 6d69   reducing the mi
+00001730: 6e69 6d75 6d20 6e75 6d62 6572 206f 6620  nimum number of 
+00001740: 6665 6174 7572 6573 2074 6f0a 2020 2020  features to.    
+00001750: 2020 2020 2020 2020 7365 6c65 6374 206f          select o
+00001760: 7220 6469 7361 626c 696e 6720 6665 6174  r disabling feat
+00001770: 7572 6520 7365 6c65 6374 696f 6e20 7669  ure selection vi
+00001780: 6120 5472 6169 6e69 6e67 436f 6e66 6967  a TrainingConfig
+00001790: 2e46 612b 0200 0053 4841 5020 7661 6c75  .Fa+...SHAP valu
+000017a0: 6573 2063 616e 6e6f 7420 6265 2063 616c  es cannot be cal
+000017b0: 6375 6c61 7465 6420 7768 656e 2063 6174  culated when cat
+000017c0: 6567 6f72 6963 616c 2065 6e63 6f64 696e  egorical encodin
+000017d0: 6720 7669 6120 4d4c 2061 6c67 6f72 6974  g via ML algorit
+000017e0: 686d 2069 7320 656e 6162 6c65 6420 6475  hm is enabled du
+000017f0: 6520 746f 0a20 2020 2020 2020 2020 2020  e to.           
+00001800: 2069 6e63 6f6d 7061 7469 6269 6c69 7479   incompatibility
+00001810: 2077 6974 6820 7468 6520 7368 6170 206c   with the shap l
+00001820: 6962 7261 7279 2e20 5365 6520 7468 6973  ibrary. See this
+00001830: 2047 6974 4875 6220 6973 7375 6520 666f   GitHub issue fo
+00001840: 7220 6d6f 7265 2063 6f6e 7465 7874 3a0a  r more context:.
+00001850: 2020 2020 2020 2020 2020 2020 6874 7470              http
+00001860: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00001870: 6c75 6e64 6265 7267 2f73 6861 702f 6973  lundberg/shap/is
+00001880: 7375 6573 2f32 3636 0a0a 2020 2020 2020  sues/266..      
+00001890: 2020 2020 2020 4361 6c63 756c 6174 696f        Calculatio
+000018a0: 6e20 6f66 2053 6861 7020 7661 6c75 6573  n of Shap values
+000018b0: 2068 6173 2062 6565 6e20 6368 616e 6765   has been change
+000018c0: 6420 746f 2066 616c 7365 2e0a 2020 2020  d to false..    
+000018d0: 2020 2020 2020 2020 436f 6e73 6964 6572          Consider
+000018e0: 2064 6973 6162 6c69 6e67 2063 6174 6567   disabling categ
+000018f0: 6f72 6963 616c 2065 6e63 6f64 696e 6720  orical encoding 
+00001900: 7669 6120 4d4c 2061 6c67 6f72 6974 686d  via ML algorithm
+00001910: 2069 6e20 7468 6520 5472 6169 6e69 6e67   in the Training
+00001920: 436f 6e66 6967 2069 6620 7368 6170 2076  Config if shap v
+00001930: 616c 7565 7320 6172 650a 2020 2020 2020  alues are.      
+00001940: 2020 2020 2020 7265 7175 6972 6564 2e20        required. 
+00001950: 416c 7465 726e 6174 6976 656c 7920 7573  Alternatively us
+00001960: 6520 5867 626f 6f73 7420 6173 2061 2063  e Xgboost as a c
+00001970: 7573 746f 6d20 6d6f 6465 6c20 616e 6420  ustom model and 
+00001980: 6361 6c63 756c 6174 6520 7368 6170 2076  calculate shap v
+00001990: 616c 7565 7320 6d61 6e75 616c 6c79 2076  alues manually v
+000019a0: 6961 0a20 2020 2020 2020 2020 2020 2070  ia.            p
+000019b0: 7265 645f 636f 6e74 7269 6273 3d54 7275  red_contribs=Tru
+000019c0: 652e 7af0 4361 7465 676f 7269 6361 6c20  e.z.Categorical 
+000019d0: 656e 636f 6469 6e67 2076 6961 204d 4c20  encoding via ML 
+000019e0: 616c 676f 7269 7468 6d20 6973 2065 6e61  algorithm is ena
+000019f0: 626c 6564 2e20 4d61 6b65 2073 7572 6520  bled. Make sure 
+00001a00: 746f 2068 616e 646c 6520 6361 7465 676f  to handle catego
+00001a10: 7269 6361 6c20 6665 6174 7572 6573 0a20  rical features. 
+00001a20: 2020 2020 2020 2020 2020 2077 6974 6869             withi
+00001a30: 6e20 7468 6520 7072 6f76 6964 6564 206d  n the provided m
+00001a40: 6c20 6d6f 6465 6c20 6f72 2063 6f6e 7369  l model or consi
+00001a50: 6465 7220 6469 7361 626c 696e 6720 6361  der disabling ca
+00001a60: 7465 676f 7269 6361 6c20 656e 636f 6469  tegorical encodi
+00001a70: 6e67 2076 6961 204d 4c20 616c 676f 7269  ng via ML algori
+00001a80: 7468 6d20 696e 2074 6865 0a20 2020 2020  thm in the.     
+00001a90: 2020 2020 2020 2054 7261 696e 696e 6743         TrainingC
+00001aa0: 6f6e 6669 6720 616c 7465 726e 6174 6976  onfig alternativ
+00001ab0: 656c 792e 7afd 4361 7465 676f 7269 6361  ely.z.Categorica
+00001ac0: 6c20 656e 636f 6469 6e67 2076 6961 204d  l encoding via M
+00001ad0: 4c20 616c 676f 7269 7468 6d20 6973 2065  L algorithm is e
+00001ae0: 6e61 626c 6564 2e20 4d61 6b65 2073 7572  nabled. Make sur
+00001af0: 6520 746f 2068 616e 646c 6520 6361 7465  e to handle cate
+00001b00: 676f 7269 6361 6c20 6665 6174 7572 6573  gorical features
+00001b10: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00001b20: 6869 6e20 7468 6520 7072 6f76 6964 6564  hin the provided
+00001b30: 206c 6173 7420 6d69 6c65 2063 6f6d 7075   last mile compu
+00001b40: 7461 7469 6f6e 206f 7220 636f 6e73 6964  tation or consid
+00001b50: 6572 2064 6973 6162 6c69 6e67 2063 6174  er disabling cat
+00001b60: 6567 6f72 6963 616c 2065 6e63 6f64 696e  egorical encodin
+00001b70: 6720 7669 6120 4d4c 2061 6c67 6f72 6974  g via ML algorit
+00001b80: 686d 2069 6e20 7468 650a 2020 2020 2020  hm in the.      
+00001b90: 2020 2020 2020 5472 6169 6e69 6e67 436f        TrainingCo
+00001ba0: 6e66 6967 2061 6c74 6572 6e61 7469 7665  nfig alternative
+00001bb0: 6c79 2e29 1072 2800 0000 720a 0000 00da  ly.).r(...r.....
+00001bc0: 1865 6e61 626c 655f 6665 6174 7572 655f  .enable_feature_
+00001bd0: 7365 6c65 6374 696f 6eda 0877 6172 6e69  selection..warni
+00001be0: 6e67 73da 0477 6172 6eda 0b55 7365 7257  ngs..warn..UserW
+00001bf0: 6172 6e69 6e67 da14 6879 7065 7274 756e  arning..hypertun
+00001c00: 696e 675f 6376 5f66 6f6c 6473 7227 0000  ing_cv_foldsr'..
+00001c10: 0072 2900 0000 da16 6d69 6e5f 6665 6174  .r).....min_feat
+00001c20: 7572 6573 5f74 6f5f 7365 6c65 6374 da03  ures_to_select..
+00001c30: 6c65 6eda 0763 6f6c 756d 6e73 da1d 6361  len..columns..ca
+00001c40: 745f 656e 636f 6469 6e67 5f76 6961 5f6d  t_encoding_via_m
+00001c50: 6c5f 616c 676f 7269 7468 6dda 1563 616c  l_algorithm..cal
+00001c60: 6375 6c61 7465 5f73 6861 705f 7661 6c75  culate_shap_valu
+00001c70: 6573 7224 0000 0072 2500 0000 2903 7231  esr$...r%...).r1
+00001c80: 0000 0072 3500 0000 da07 6d65 7373 6167  ...r5.....messag
+00001c90: 6572 3200 0000 7232 0000 0072 3300 0000  er2...r2...r3...
+00001ca0: da0e 696e 6974 6961 6c5f 6368 6563 6b73  ..initial_checks
+00001cb0: 6200 0000 734e 0000 0006 0108 0108 0104  b...sN..........
+00001cc0: 0110 050c 0204 0110 0306 0302 ff04 0202  ................
+00001cd0: fe04 0410 0406 0104 0110 0412 0206 0102  ................
+00001ce0: ff04 0310 0306 0202 ff06 0202 fe08 0404  ................
+00001cf0: 0110 080e 0104 0110 0306 0202 ff04 0202  ................
+00001d00: fe04 0414 0308 f97a 1742 6c75 6543 6173  .......z.BlueCas
+00001d10: 742e 696e 6974 6961 6c5f 6368 6563 6b73  t.initial_checks
+00001d20: da0a 7461 7267 6574 5f63 6f6c 6303 0000  ..target_colc...
+00001d30: 0000 0000 0000 0000 0009 0000 0007 0000  ................
+00001d40: 0043 0000 0073 1e03 0000 7400 8300 0100  .C...s....t.....
+00001d50: 7401 8300 7d03 7c03 a002 7c01 a101 7d01  t...}.|...|...}.
+00001d60: 7c03 7c00 5f03 7c00 6a03 6a04 7229 7c00  |.|._.|.j.j.r)|.
+00001d70: 6a05 7c00 6a03 6a04 7600 7229 7406 8300  j.|.j.j.v.r)t...
+00001d80: 7c00 5f07 7c00 6a07 a008 7c01 7c00 6a05  |._.|.j...|.|.j.
+00001d90: 1900 a101 7c01 7c00 6a05 3c00 7c00 6a03  ....|.|.j.<.|.j.
+00001da0: 6a04 7c00 5f04 7c00 6a03 6a09 7c00 5f09  j.|._.|.j.j.|._.
+00001db0: 7c00 6a0a 733a 740b 8300 7c00 5f0a 7c00  |.j.s:t...|._.|.
+00001dc0: a00c 7c01 a101 0100 740d 7c01 7c02 7c00  ..|.....t.|.|.|.
+00001dd0: 6a0e 7c00 6a0a 6a0f 7c00 6a0a 6a10 7c00  j.|.j.j.|.j.j.|.
+00001de0: 6a0a 6a11 8306 5c04 7d04 7d05 7d06 7d07  j.j...\.}.}.}.}.
+00001df0: 7c00 6a12 7297 7c00 6a12 a013 7c04 7c06  |.j.r.|.j...|.|.
+00001e00: a102 5c02 7d04 7d06 7c00 6a12 6a14 7c05  ..\.}.}.|.j.j.|.
+00001e10: 7c07 6401 6402 8d03 5c02 7d05 7d07 7401  |.d.d...\.}.}.t.
+00001e20: 8300 7d03 7c03 a002 7c04 a101 7d08 7c04  ..}.|...|...}.|.
+00001e30: 6a15 6403 6404 8d01 7c06 6a15 6403 6404  j.d.d...|.j.d.d.
+00001e40: 8d01 0202 7d04 7d06 7c05 6a15 6403 6404  ....}.}.|.j.d.d.
+00001e50: 8d01 7c07 6a15 6403 6404 8d01 0202 7d05  ..|.j.d.d.....}.
+00001e60: 7d07 7c02 7c03 6a04 7600 7297 7c03 6a04  }.|.|.j.v.r.|.j.
+00001e70: a016 7c02 a101 0100 7417 7c04 8301 7417  ..|.....t.|...t.
+00001e80: 7c05 8301 0202 7d04 7d05 7418 7c04 7c00  |.....}.}.t.|.|.
+00001e90: 6a09 8302 7418 7c05 7c00 6a09 8302 0202  j...t.|.|.j.....
+00001ea0: 7d04 7d05 7419 8300 7c00 5f1a 7c00 6a1a  }.}.t...|._.|.j.
+00001eb0: a01b 7c04 a101 0100 7c00 6a1a a014 7c05  ..|.....|.j...|.
+00001ec0: a101 7d05 7c00 6a04 6405 7501 72df 7c00  ..}.|.j.d.u.r.|.
+00001ed0: 6a1c 6406 6b02 72df 7c00 6a0a 6a1d 73df  j.d.k.r.|.j.j.s.
+00001ee0: 741e 7c03 6a04 8301 7c00 5f1f 7c00 6a1f  t.|.j...|._.|.j.
+00001ef0: a020 7c04 7c06 a102 7d04 7c00 6a1f a021  . |.|...}.|.j..!
+00001f00: 7c05 a101 7d05 6e40 7c00 6a04 6405 7501  |...}.n@|.j.d.u.
+00001f10: 9001 7204 7c00 6a1c 6407 6b02 9001 7204  ..r.|.j.d.k...r.
+00001f20: 7c00 6a0a 6a1d 9001 7304 7422 7c03 6a04  |.j.j...s.t"|.j.
+00001f30: 8301 7c00 5f1f 7c00 6a1f a023 7c04 7c06  ..|._.|.j..#|.|.
+00001f40: a102 7d04 7c00 6a1f a024 7c05 a101 7d05  ..}.|.j..$|...}.
+00001f50: 6e1b 7c00 6a0a 6a1d 9001 721f 7c04 7c00  n.|.j.j...r.|.|.
+00001f60: 6a04 1900 a025 6408 a101 7c04 7c00 6a04  j....%d...|.|.j.
+00001f70: 3c00 7c05 7c00 6a04 1900 a025 6408 a101  <.|.|.j....%d...
+00001f80: 7c05 7c00 6a04 3c00 7c00 6a26 9001 7237  |.|.j.<.|.j&..r7
+00001f90: 7c00 6a26 a013 7c04 7c06 a102 5c02 7d04  |.j&..|.|...\.}.
+00001fa0: 7d06 7c00 6a26 6a14 7c05 7c07 6401 6402  }.|.j&j.|.|.d.d.
+00001fb0: 8d03 5c02 7d05 7d07 7c00 6a27 9001 7346  ..\.}.}.|.j'..sF
+00001fc0: 7428 7c00 6a0a 6a10 7c00 6a0a 6a29 6409  t(|.j.j.|.j.j)d.
+00001fd0: 8d02 7c00 5f27 7c00 6a0a 6a2a 9001 725e  ..|._'|.j.j*..r^
+00001fe0: 7c00 6a27 a013 7c04 7c06 a102 5c02 7d04  |.j'..|.|...\.}.
+00001ff0: 7d06 7c00 6a27 6a14 7c05 6401 6402 8d02  }.|.j'j.|.d.d...
+00002000: 5c02 7d05 7d08 7c00 6a2b 9001 736f 742c  \.}.}.|.j+..sot,
+00002010: 7c00 6a1c 7c00 6a0a 7c00 6a2d 7c00 6a2e  |.j.|.j.|.j-|.j.
+00002020: 640a 8d04 7c00 5f2b 7c00 6a2b a01b 7c04  d...|._+|.j+..|.
+00002030: 7c05 7c06 7c07 a104 0100 7c00 6a0a 9001  |.|.|.....|.j...
+00002040: 728a 7c00 6a0a 6a2f 9001 728a 7430 7c00  r.|.j.j/..r.t0|.
+00002050: 6a2b 6a31 7c05 640b 8303 7c00 5f32 6403  j+j1|.d...|._2d.
+00002060: 7c00 5f33 6405 5300 290c 7a19 5472 6169  |._3d.S.).z.Trai
+00002070: 6e20 6120 6675 6c6c 204d 4c20 7069 7065  n a full ML pipe
+00002080: 6c69 6e65 2e46 a901 da0e 7072 6564 6963  line.F....predic
+00002090: 746f 6e5f 6d6f 6465 54a9 01da 0464 726f  ton_modeT....dro
+000020a0: 704e 721e 0000 0072 1f00 0000 da08 6361  pNr....r......ca
+000020b0: 7465 676f 7279 2902 da0c 7261 6e64 6f6d  tegory)...random
+000020c0: 5f73 7461 7465 723f 0000 0029 0372 2800  _stater?...).r(.
+000020d0: 0000 7229 0000 0072 2a00 0000 da04 7472  ..r)...r*.....tr
+000020e0: 6565 2934 720f 0000 0072 1600 0000 5a1b  ee)4r....r....Z.
+000020f0: 6669 745f 7472 616e 7366 6f72 6d5f 6665  fit_transform_fe
+00002100: 6174 7572 655f 7479 7065 7372 2c00 0000  ature_typesr,...
+00002110: 7221 0000 0072 2000 0000 7214 0000 0072  r!...r ...r....r
+00002120: 2e00 0000 5a1b 6669 745f 7472 616e 7366  ....Z.fit_transf
+00002130: 6f72 6d5f 7461 7267 6574 5f6c 6162 656c  orm_target_label
+00002140: 7372 2200 0000 7228 0000 0072 0a00 0000  sr"...r(...r....
+00002150: 7245 0000 0072 1b00 0000 7223 0000 00da  rE...r....r#....
+00002160: 0a74 7261 696e 5f73 697a 655a 1367 6c6f  .train_sizeZ.glo
+00002170: 6261 6c5f 7261 6e64 6f6d 5f73 7461 7465  bal_random_state
+00002180: 5a14 7472 6169 6e5f 7370 6c69 745f 7374  Z.train_split_st
+00002190: 7261 7469 6679 7226 0000 00da 0d66 6974  ratifyr&.....fit
+000021a0: 5f74 7261 6e73 666f 726d da09 7472 616e  _transform..tran
+000021b0: 7366 6f72 6dda 0b72 6573 6574 5f69 6e64  sform..reset_ind
+000021c0: 6578 da06 7265 6d6f 7665 7217 0000 0072  ex..remover....r
+000021d0: 1300 0000 7218 0000 0072 2f00 0000 da03  ....r....r/.....
+000021e0: 6669 7472 1d00 0000 7242 0000 0072 1900  fitr....rB...r..
+000021f0: 0000 722d 0000 005a 1e66 6974 5f74 6172  ..r-...Z.fit_tar
+00002200: 6765 745f 656e 636f 6465 5f62 696e 6172  get_encode_binar
+00002210: 795f 636c 6173 73da 2474 7261 6e73 666f  y_class.$transfo
+00002220: 726d 5f74 6172 6765 745f 656e 636f 6465  rm_target_encode
+00002230: 5f62 696e 6172 795f 636c 6173 7372 1a00  _binary_classr..
+00002240: 0000 5a1c 6669 745f 7461 7267 6574 5f65  ..Z.fit_target_e
+00002250: 6e63 6f64 655f 6d75 6c74 6963 6c61 7373  ncode_multiclass
+00002260: da22 7472 616e 7366 6f72 6d5f 7461 7267  ."transform_targ
+00002270: 6574 5f65 6e63 6f64 655f 6d75 6c74 6963  et_encode_multic
+00002280: 6c61 7373 da06 6173 7479 7065 7225 0000  lass..astyper%..
+00002290: 0072 2700 0000 7215 0000 0072 3f00 0000  .r'...r....r?...
+000022a0: 723a 0000 0072 2400 0000 7211 0000 0072  r:...r$...r....r
+000022b0: 2900 0000 722a 0000 0072 4300 0000 720e  )...r*...rC...r.
+000022c0: 0000 00da 056d 6f64 656c 7230 0000 0072  .....modelr0...r
+000022d0: 2b00 0000 2909 7231 0000 0072 3500 0000  +...).r1...r5...
+000022e0: 7246 0000 0072 2c00 0000 da07 785f 7472  rF...r,.....x_tr
+000022f0: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
+00002300: 7261 696e da06 795f 7465 7374 da01 5f72  rain..y_test.._r
+00002310: 3200 0000 7232 0000 0072 3300 0000 7253  2...r2...r3...rS
+00002320: 0000 00a6 0000 0073 be00 0000 0602 0601  .......s........
+00002330: 0a01 0601 0802 0e01 0801 0603 0801 02ff  ................
+00002340: 02fe 0401 02ff 0a06 0a01 0602 0801 0a02  ................
+00002350: 0202 0201 0201 0401 0601 0601 0601 0cfa  ................
+00002360: 0609 1201 0601 0601 0aff 0603 0a01 0e01  ................
+00002370: 0201 0aff 0e03 0201 0aff 0a03 0c01 1202  ................
+00002380: 0c01 0601 08ff 0804 0c01 0c01 0a03 0a01  ................
+00002390: 0601 02ff 0c03 0e01 0e01 0c02 0c01 0601  ................
+000023a0: 04ff 0c03 0e01 0e01 0a01 1601 1601 0802  ................
+000023b0: 0601 0401 08ff 0603 0601 0aff 0804 0201  ................
+000023c0: 0601 0601 08fe 0a05 0601 0401 08ff 0603  ................
+000023d0: 0401 0aff 0804 0201 0401 0401 0401 0401  ................
+000023e0: 08fc 1206 1201 1201 0a01 7a0c 426c 7565  ..........z.Blue
+000023f0: 4361 7374 2e66 6974 da07 6466 5f65 7661  Cast.fit..df_eva
+00002400: 6cda 0b74 6172 6765 745f 6576 616c 6305  l..target_evalc.
+00002410: 0000 0000 0000 0000 0000 0008 0000 0004  ................
+00002420: 0000 0043 0000 0073 2c00 0000 7c00 a000  ...C...s,...|...
+00002430: 7c01 7c04 a102 0100 7c00 a001 7c02 a101  |.|.....|...|...
+00002440: 5c02 7d05 7d06 7402 7c03 6a03 7c05 7c06  \.}.}.t.|.j.|.|.
+00002450: 8303 7d07 7c07 5300 2901 618e 0200 0054  ..}.|.S.).a....T
+00002460: 7261 696e 2061 2066 756c 6c20 4d4c 2070  rain a full ML p
+00002470: 6970 656c 696e 6520 616e 6420 6576 616c  ipeline and eval
+00002480: 7561 7465 206f 6e20 6120 686f 6c64 6f75  uate on a holdou
+00002490: 7420 7365 742e 0a0a 2020 2020 2020 2020  t set...        
+000024a0: 5468 6973 2069 7320 6120 636f 6e76 656e  This is a conven
+000024b0: 6965 6e63 6520 6675 6e63 7469 6f6e 2074  ience function t
+000024c0: 6f20 7472 6169 6e20 616e 6420 6576 616c  o train and eval
+000024d0: 7561 7465 206f 6e20 6120 686f 6c64 6f75  uate on a holdou
+000024e0: 7420 7365 742e 2049 7420 6973 2072 6563  t set. It is rec
+000024f0: 6f6d 6d65 6e64 6564 2074 6f20 7573 6520  ommended to use 
+00002500: 7468 6973 2066 6f72 206d 6f64 656c 0a20  this for model. 
+00002510: 2020 2020 2020 2065 7870 6c6f 7261 7469         explorati
+00002520: 6f6e 2e20 4f6e 2070 726f 6475 6374 696f  on. On productio
+00002530: 6e20 7468 6520 7369 6d70 6c65 2066 6974  n the simple fit
+00002540: 2829 2066 756e 6374 696f 6e20 7368 6f75  () function shou
+00002550: 6c64 2062 6520 7573 6564 2e0a 2020 2020  ld be used..    
+00002560: 2020 2020 3a70 6172 616d 203a 6466 3a20      :param :df: 
+00002570: 5461 6b65 7320 6120 7061 6e64 6173 2044  Takes a pandas D
+00002580: 6174 6146 7261 6d65 2063 6f6e 7461 696e  ataFrame contain
+00002590: 696e 6720 7468 6520 7472 6169 6e69 6e67  ing the training
+000025a0: 2064 6174 6120 616e 6420 7468 6520 7461   data and the ta
+000025b0: 7267 6574 732e 0a20 2020 2020 2020 203a  rgets..        :
+000025c0: 7061 7261 6d20 3a64 665f 6576 616c 3a20  param :df_eval: 
+000025d0: 5461 6b65 7320 6120 7061 6e64 6173 2044  Takes a pandas D
+000025e0: 6174 6146 7261 6d65 2063 6f6e 7461 696e  ataFrame contain
+000025f0: 696e 6720 7468 6520 6576 616c 7561 7469  ing the evaluati
+00002600: 6f6e 2064 6174 612c 2062 7574 206e 6f74  on data, but not
+00002610: 2074 6865 2074 6172 6765 7473 2e0a 2020   the targets..  
+00002620: 2020 2020 2020 3a70 6172 616d 203a 7461        :param :ta
+00002630: 7267 6574 5f65 7661 6c3a 2054 616b 6573  rget_eval: Takes
+00002640: 2061 2070 616e 6461 7320 5365 7269 6573   a pandas Series
+00002650: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00002660: 6576 616c 7561 7469 6f6e 2074 6172 6765  evaluation targe
+00002670: 7473 2e0a 2020 2020 2020 2020 3a70 6172  ts..        :par
+00002680: 616d 203a 7461 7267 6574 5f63 6f6c 3a20  am :target_col: 
+00002690: 5461 6b65 7320 6120 7374 7269 6e67 2063  Takes a string c
+000026a0: 6f6e 7461 696e 696e 6720 7468 6520 6e61  ontaining the na
+000026b0: 6d65 206f 6620 7468 6520 7461 7267 6574  me of the target
+000026c0: 2063 6f6c 756d 6e20 696e 7369 6465 2074   column inside t
+000026d0: 6865 2074 7261 696e 696e 6720 6461 7461  he training data
+000026e0: 2064 662e 0a20 2020 2020 2020 2029 0472   df..        ).r
+000026f0: 5300 0000 da07 7072 6564 6963 7472 0d00  S.....predictr..
+00002700: 0000 da06 7661 6c75 6573 2908 7231 0000  ....values).r1..
+00002710: 0072 3500 0000 725d 0000 0072 5e00 0000  .r5...r]...r^...
+00002720: 7246 0000 00da 0779 5f70 726f 6273 da09  rF.....y_probs..
+00002730: 795f 636c 6173 7365 735a 0965 7661 6c5f  y_classesZ.eval_
+00002740: 6469 6374 7232 0000 0072 3200 0000 7233  dictr2...r2...r3
+00002750: 0000 00da 0866 6974 5f65 7661 6c16 0100  .....fit_eval...
+00002760: 0073 0800 0000 0c10 0e01 0e01 0401 7a11  .s............z.
+00002770: 426c 7565 4361 7374 2e66 6974 5f65 7661  BlueCast.fit_eva
+00002780: 6c63 0200 0000 0000 0000 0000 0000 0300  lc..............
+00002790: 0000 0400 0000 4300 0000 7350 0100 0074  ......C...sP...t
+000027a0: 0083 0001 007c 006a 0173 0a74 0264 0183  .....|.j.s.t.d..
+000027b0: 0182 017c 006a 0373 1174 0264 0283 0182  ...|.j.s.t.d....
+000027c0: 017c 006a 016a 047c 017c 006a 0567 0164  .|.j.j.|.|.j.g.d
+000027d0: 038d 027d 017c 006a 0672 2e7c 006a 066a  ...}.|.j.r.|.j.j
+000027e0: 077c 0164 0464 058d 025c 027d 017d 027c  .|.d.d...\.}.}.|
+000027f0: 016a 0864 0464 068d 017d 0174 097c 0183  .j.d.d...}.t.|..
+00002800: 017d 0174 0a7c 017c 006a 0b83 027d 017c  .}.t.|.|.j...}.|
+00002810: 006a 0c72 417c 006a 0ca0 077c 01a1 017d  .j.rA|.j...|...}
+00002820: 017c 006a 0d72 5d7c 006a 0e72 5d7c 006a  .|.j.r]|.j.r]|.j
+00002830: 0f64 076b 0272 5d74 107c 006a 0e74 1183  .d.k.r]t.|.j.t..
+00002840: 0272 5d7c 006a 036a 1273 5d7c 006a 0ea0  .r]|.j.j.s]|.j..
+00002850: 137c 01a1 017d 016e 2b7c 006a 0d72 797c  .|...}.n+|.j.ry|
+00002860: 006a 0e72 797c 006a 0f64 086b 0272 7974  .j.ry|.j.d.k.ryt
+00002870: 107c 006a 0e74 1483 0272 797c 006a 036a  .|.j.t...ry|.j.j
+00002880: 1273 797c 006a 0ea0 157c 01a1 017d 016e  .sy|.j...|...}.n
+00002890: 0f7c 006a 036a 1272 887c 017c 006a 0d19  .|.j.j.r.|.|.j..
+000028a0: 00a0 1664 09a1 017c 017c 006a 0d3c 007c  ...d...|.|.j.<.|
+000028b0: 006a 1772 957c 006a 176a 077c 0164 0464  .j.r.|.j.j.|.d.d
+000028c0: 058d 025c 027d 017d 027c 006a 1872 a67c  ...\.}.}.|.j.r.|
+000028d0: 006a 036a 1972 a67c 006a 186a 077c 0164  .j.j.r.|.j.j.|.d
+000028e0: 0464 058d 025c 027d 017d 027c 0153 0029  .d...\.}.}.|.S.)
+000028f0: 0a7a 3754 7261 6e73 666f 726d 206e 6577  .z7Transform new
+00002900: 2064 6174 6120 6163 636f 7264 696e 6720   data according 
+00002910: 746f 2070 7265 7072 6f63 6573 7369 6e67  to preprocessing
+00002920: 2070 6970 656c 696e 652e fa2a 4665 6174   pipeline..*Feat
+00002930: 7572 6520 7479 7065 2063 6f6e 7665 7274  ure type convert
+00002940: 6572 2063 6f75 6c64 206e 6f74 2062 6520  er could not be 
+00002950: 666f 756e 642e 7a2a 5472 6169 6e69 6e67  found.z*Training
+00002960: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
+00002970: 6f75 6c64 206e 6f74 2062 6520 666f 756e  ould not be foun
+00002980: 642e 2901 5a0b 6967 6e6f 7265 5f63 6f6c  d.).Z.ignore_col
+00002990: 7354 7247 0000 0072 4900 0000 721e 0000  sTrG...rI...r...
+000029a0: 0072 1f00 0000 724b 0000 0029 1a72 0f00  .r....rK...).r..
+000029b0: 0000 722c 0000 00da 0945 7863 6570 7469  ..r,.....Excepti
+000029c0: 6f6e 7228 0000 005a 1774 7261 6e73 666f  onr(...Z.transfo
+000029d0: 726d 5f66 6561 7475 7265 5f74 7970 6573  rm_feature_types
+000029e0: 7220 0000 0072 2600 0000 7250 0000 0072  r ...r&...rP...r
+000029f0: 5100 0000 7217 0000 0072 1300 0000 7222  Q...r....r....r"
+00002a00: 0000 0072 2f00 0000 7221 0000 0072 2d00  ...r/...r!...r-.
+00002a10: 0000 721d 0000 00da 0a69 7369 6e73 7461  ..r......isinsta
+00002a20: 6e63 6572 1900 0000 7242 0000 0072 5400  ncer....rB...rT.
+00002a30: 0000 721a 0000 0072 5500 0000 7256 0000  ..r....rU...rV..
+00002a40: 0072 2500 0000 7227 0000 0072 3a00 0000  .r%...r'...r:...
+00002a50: 2903 7231 0000 0072 3500 0000 725c 0000  ).r1...r5...r\..
+00002a60: 0072 3200 0000 7232 0000 0072 3300 0000  .r2...r2...r3...
+00002a70: da12 7472 616e 7366 6f72 6d5f 6e65 775f  ..transform_new_
+00002a80: 6461 7461 2b01 0000 7354 0000 0006 0206  data+...sT......
+00002a90: 0108 0106 0208 0106 0208 0106 ff06 0414  ................
+00002aa0: 010c 0108 020c 0106 020c 0104 0302 ff04  ................
+00002ab0: 0202 fe0a 030a 0102 ff06 0202 fe0e 0404  ................
+00002ac0: 0202 ff04 0202 fe0a 030a 0102 ff06 0202  ................
+00002ad0: fe0e 0408 0116 0106 0214 010e 0214 0104  ................
+00002ae0: 027a 1b42 6c75 6543 6173 742e 7472 616e  .z.BlueCast.tran
+00002af0: 7366 6f72 6d5f 6e65 775f 6461 7461 6302  sform_new_datac.
+00002b00: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00002b10: 0000 0043 0000 0073 9800 0000 7c00 6a00  ...C...s....|.j.
+00002b20: 7307 7401 6401 8301 8201 7c00 6a02 730e  s.t.d.....|.j.s.
+00002b30: 7401 6402 8301 8201 7c00 6a03 7315 7404  t.d.....|.j.s.t.
+00002b40: 6403 8301 8201 7405 8300 0100 7c00 a006  d.....t.....|...
+00002b50: 7c01 a101 7d01 7407 7408 a009 a100 9b00  |...}.t.t.......
+00002b60: 6404 9d02 8301 0100 7c00 6a00 a00a 7c01  d.......|.j...|.
+00002b70: a101 5c02 7d02 7d03 7c00 6a02 6a0b 7248  ..\.}.}.|.j.j.rH
+00002b80: 7c00 6a0c 7c00 6a02 6a0b 7600 7248 7c00  |.j.|.j.j.v.rH|.
+00002b90: 6a0d 7248 7c00 6a02 7248 7c00 6a0d a00e  j.rH|.j.rH|.j...
+00002ba0: 740f a010 7c03 a101 a101 7d03 7c02 7c03  t...|.....}.|.|.
+00002bb0: 6602 5300 2905 7a90 5072 6564 6963 7420  f.S.).z.Predict 
+00002bc0: 6f6e 2075 6e73 6565 6e20 6461 7461 2e0a  on unseen data..
+00002bd0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+00002be0: 7468 6520 7072 6564 6963 7465 6420 7072  the predicted pr
+00002bf0: 6f62 6162 696c 6974 6965 7320 616e 6420  obabilities and 
+00002c00: 7468 6520 7072 6564 6963 7465 6420 636c  the predicted cl
+00002c10: 6173 7365 733a 0a20 2020 2020 2020 2079  asses:.        y
+00002c20: 5f70 726f 6273 2c20 795f 636c 6173 7365  _probs, y_classe
+00002c30: 7320 3d20 7072 6564 6963 7428 6466 290a  s = predict(df).
+00002c40: 2020 2020 2020 2020 7a1b 4d6c 206d 6f64          z.Ml mod
+00002c50: 656c 2063 6f75 6c64 206e 6f74 2062 6520  el could not be 
+00002c60: 666f 756e 6472 6400 0000 7a15 636f 6e66  foundrd...z.conf
+00002c70: 5f74 7261 696e 696e 6720 6973 204e 6f6e  _training is Non
+00002c80: 657a 0f3a 2050 7265 6469 6374 696e 672e  ez.: Predicting.
+00002c90: 2e2e 2911 7224 0000 0072 6500 0000 722c  ..).r$...re...r,
+00002ca0: 0000 0072 2800 0000 da0a 5661 6c75 6545  ...r(.....ValueE
+00002cb0: 7272 6f72 720f 0000 0072 6700 0000 7210  rrorr....rg...r.
+00002cc0: 0000 0072 0200 0000 da06 7574 636e 6f77  ...r......utcnow
+00002cd0: 725f 0000 0072 2100 0000 7220 0000 0072  r_...r!...r ...r
+00002ce0: 2e00 0000 5a1f 6c61 6265 6c5f 656e 636f  ....Z.label_enco
+00002cf0: 6465 725f 7265 7665 7273 655f 7472 616e  der_reverse_tran
+00002d00: 7366 6f72 6dda 0270 64da 0653 6572 6965  sform..pd..Serie
+00002d10: 7329 0472 3100 0000 7235 0000 0072 6100  s).r1...r5...ra.
+00002d20: 0000 7262 0000 0072 3200 0000 7232 0000  ..rb...r2...r2..
+00002d30: 0072 3300 0000 725f 0000 005d 0100 0073  .r3...r_...]...s
+00002d40: 2800 0000 0606 0801 0602 0801 0602 0801  (...............
+00002d50: 0602 0a01 1202 1001 0802 0e02 0401 02ff  ................
+00002d60: 0402 02fe 0604 0801 04ff 0804 7a10 426c  ............z.Bl
+00002d70: 7565 4361 7374 2e70 7265 6469 6374 290a  ueCast.predict).
+00002d80: 4e4e 4e4e 4e4e 4e4e 4e4e 291f da08 5f5f  NNNNNNNNNN)...__
+00002d90: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00002da0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00002db0: da07 5f5f 646f 635f 5f72 0600 0000 7209  ..__doc__r....r.
+00002dc0: 0000 00da 0373 7472 da05 666c 6f61 74da  .....str..float.
+00002dd0: 0369 6e74 7207 0000 0072 0500 0000 7211  .intr....r....r.
+00002de0: 0000 0072 0300 0000 7212 0000 0072 1500  ...r....r....r..
+00002df0: 0000 720a 0000 0072 0c00 0000 720b 0000  ..r....r....r...
+00002e00: 0072 3400 0000 726a 0000 00da 0944 6174  .r4...rj.....Dat
+00002e10: 6146 7261 6d65 7245 0000 0072 5300 0000  aFramerE...rS...
+00002e20: 726b 0000 0072 0400 0000 7263 0000 0072  rk...r....rc...r
+00002e30: 6700 0000 7208 0000 00da 026e 70da 076e  g...r......np..n
+00002e40: 6461 7272 6179 725f 0000 0072 3200 0000  darrayr_...r2...
+00002e50: 7232 0000 0072 3200 0000 7233 0000 0072  r2...r2...r3...r
+00002e60: 1c00 0000 2700 0000 736c 0000 0008 0004  ....'...sl......
+00002e70: 0102 1802 0102 0102 0102 0102 0102 0302  ................
+00002e80: 0102 0102 0104 f106 0202 fe0c 0302 fd14  ................
+00002e90: 0402 fc14 0502 fb06 0602 fa0e 0702 f906  ................
+00002ea0: 0802 f806 0902 f702 0a0a 0102 ff02 f606  ................
+00002eb0: 0d02 f306 0e02 f206 0f0a f114 2618 4402  ............&.D.
+00002ec0: 7004 0202 fe04 0302 fd04 0402 fc02 0502  p...............
+00002ed0: fb0a 060a fa16 1524 3272 1c00 0000 2930  .......$2r....)0
+00002ee0: 726f 0000 0072 3b00 0000 7202 0000 00da  ro...r;...r.....
+00002ef0: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
+00002f00: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00002f10: 7208 0000 0072 0900 0000 da05 6e75 6d70  r....r......nump
+00002f20: 7972 7400 0000 da06 7061 6e64 6173 726a  yrt.....pandasrj
+00002f30: 0000 00da 1f62 6c75 6563 6173 742e 636f  .....bluecast.co
+00002f40: 6e66 6967 2e74 7261 696e 696e 675f 636f  nfig.training_co
+00002f50: 6e66 6967 720a 0000 0072 0b00 0000 720c  nfigr....r....r.
+00002f60: 0000 005a 2062 6c75 6563 6173 742e 6576  ...Z bluecast.ev
+00002f70: 616c 7561 7469 6f6e 2e65 7661 6c5f 6d65  aluation.eval_me
+00002f80: 7472 6963 7372 0d00 0000 5a1f 626c 7565  tricsr....Z.blue
+00002f90: 6361 7374 2e65 7661 6c75 6174 696f 6e2e  cast.evaluation.
+00002fa0: 7368 6170 5f76 616c 7565 7372 0e00 0000  shap_valuesr....
+00002fb0: 5a24 626c 7565 6361 7374 2e67 656e 6572  Z$bluecast.gener
+00002fc0: 616c 5f75 7469 6c73 2e67 656e 6572 616c  al_utils.general
+00002fd0: 5f75 7469 6c73 720f 0000 0072 1000 0000  _utilsr....r....
+00002fe0: 5a1d 626c 7565 6361 7374 2e6d 6c5f 6d6f  Z.bluecast.ml_mo
+00002ff0: 6465 6c6c 696e 672e 7867 626f 6f73 7472  delling.xgboostr
+00003000: 1100 0000 da1d 626c 7565 6361 7374 2e70  ......bluecast.p
+00003010: 7265 7072 6f63 6573 7369 6e67 2e63 7573  reprocessing.cus
+00003020: 746f 6d72 1200 0000 5a28 626c 7565 6361  tomr....Z(blueca
+00003030: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00003040: 2e64 6174 6574 696d 655f 6665 6174 7572  .datetime_featur
+00003050: 6573 7213 0000 005a 2b62 6c75 6563 6173  esr....Z+bluecas
+00003060: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+00003070: 656e 636f 6465 5f74 6172 6765 745f 6c61  encode_target_la
+00003080: 6265 6c73 7214 0000 005a 2862 6c75 6563  belsr....Z(bluec
+00003090: 6173 742e 7072 6570 726f 6365 7373 696e  ast.preprocessin
+000030a0: 672e 6665 6174 7572 655f 7365 6c65 6374  g.feature_select
+000030b0: 696f 6e72 1500 0000 5a24 626c 7565 6361  ionr....Z$blueca
+000030c0: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+000030d0: 2e66 6561 7475 7265 5f74 7970 6573 7216  .feature_typesr.
+000030e0: 0000 005a 2562 6c75 6563 6173 742e 7072  ...Z%bluecast.pr
+000030f0: 6570 726f 6365 7373 696e 672e 6e75 6c6c  eprocessing.null
+00003100: 735f 616e 645f 696e 6673 7217 0000 005a  s_and_infsr....Z
+00003110: 2462 6c75 6563 6173 742e 7072 6570 726f  $bluecast.prepro
+00003120: 6365 7373 696e 672e 7363 6865 6d61 5f63  cessing.schema_c
+00003130: 6865 636b 7372 1800 0000 5a26 626c 7565  hecksr....Z&blue
+00003140: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
+00003150: 6e67 2e74 6172 6765 745f 656e 636f 6469  ng.target_encodi
+00003160: 6e67 7219 0000 0072 1a00 0000 5a27 626c  ngr....r....Z'bl
+00003170: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
+00003180: 7369 6e67 2e74 7261 696e 5f74 6573 745f  sing.train_test_
+00003190: 7370 6c69 7472 1b00 0000 721c 0000 0072  splitr....r....r
+000031a0: 3200 0000 7232 0000 0072 3200 0000 7233  2...r2...r2...r3
+000031b0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000031c0: 0073 2a00 0000 0400 0808 0c01 2401 0802  .s*.........$...
+000031d0: 0801 1402 0c05 0c01 1001 0c01 0c01 0c01  ................
+000031e0: 0c01 0c01 0c01 0c01 0c01 1001 0c04 1203  ................
```

### Comparing `bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-38.pyc` & `bluecast-0.8/bluecast/blueprints/__pycache__/cast.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 06:12:51 2023 UTC, .py size: 18653 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e37d 9a64 dd48 0000  U........}.d.H..
+00000000: 550d 0d0a 0000 0000 00a4 a364 df48 0000  U..........d.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6402 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6401 6402 6c0d 5a0e 6401 6405 6c0f  Z.d.d.l.Z.d.d.l.
@@ -93,15 +93,15 @@
 000005c0: 1565 136a 1465 0664 0264 0a9c 0364 0b64  .e.j.e.d.d...d.d
 000005d0: 0c84 045a 1665 136a 1465 136a 1465 136a  ...Z.e.j.e.j.e.j
 000005e0: 1765 0665 1865 0665 0c66 0219 0064 0d9c  .e.e.e.e.f...d..
 000005f0: 0564 0e64 0f84 045a 1965 136a 1465 136a  .d.d...Z.e.j.e.j
 00000600: 1464 079c 0264 1064 1184 045a 1a65 136a  .d...d.d...Z.e.j
 00000610: 1465 1b65 1c6a 1d65 1c6a 1d66 0219 0064  .e.e.j.e.j.f...d
 00000620: 079c 0264 1264 1384 045a 1e64 0253 0029  ...d.d...Z.d.S.)
-00000630: 15da 0842 6c75 6543 6173 7461 2206 0000  ...BlueCasta"...
+00000630: 15da 0842 6c75 6543 6173 7461 2406 0000  ...BlueCasta$...
 00000640: 5275 6e20 6675 6c6c 7920 636f 6e66 6967  Run fully config
 00000650: 7572 6564 2063 6c61 7373 6966 6963 6174  ured classificat
 00000660: 696f 6e20 626c 7565 7072 696e 742e 0a0a  ion blueprint...
 00000670: 2020 2020 4375 7374 6f6d 697a 6174 696f      Customizatio
 00000680: 6e20 7669 6120 636c 6173 7320 6174 7472  n via class attr
 00000690: 6962 7574 6573 2069 7320 706f 7373 6962  ibutes is possib
 000006a0: 6c65 2e20 436f 6e66 6967 7320 6361 6e20  le. Configs can 
@@ -132,668 +132,668 @@
 00000830: 206f 6620 7374 7269 6e67 7320 636f 6e74   of strings cont
 00000840: 6169 6e69 6e67 2074 6865 206e 616d 6573  aining the names
 00000850: 206f 6620 7468 6520 6361 7465 676f 7269   of the categori
 00000860: 6361 6c20 636f 6c75 6d6e 732e 2049 6620  cal columns. If 
 00000870: 6e6f 7420 7072 6f76 6964 6564 2c0a 2020  not provided,.  
 00000880: 2020 426c 7565 4361 7374 2077 696c 6c20    BlueCast will 
 00000890: 696e 6665 7220 7468 6573 6520 6175 746f  infer these auto
-000008a0: 6d61 6963 616c 6c79 2e0a 2020 2020 3a70  maically..    :p
-000008b0: 6172 616d 203a 6461 7465 5f63 6f6c 756d  aram :date_colum
-000008c0: 6e73 3a20 5461 6b65 7320 6120 6c69 7374  ns: Takes a list
-000008d0: 206f 6620 7374 7269 6e67 7320 636f 6e74   of strings cont
-000008e0: 6169 6e69 6e67 2074 6865 206e 616d 6573  aining the names
-000008f0: 206f 6620 7468 6520 6461 7465 2063 6f6c   of the date col
-00000900: 756d 6e73 2e20 4966 206e 6f74 2070 726f  umns. If not pro
-00000910: 7669 6465 642c 0a20 2020 2042 6c75 6543  vided,.    BlueC
-00000920: 6173 7420 7769 6c6c 2069 6e66 6572 2074  ast will infer t
-00000930: 6865 7365 2061 7574 6f6d 6169 6361 6c6c  hese automaicall
-00000940: 792e 0a20 2020 203a 7061 7261 6d20 3a74  y..    :param :t
-00000950: 696d 655f 7370 6c69 745f 636f 6c75 6d6e  ime_split_column
-00000960: 3a20 5461 6b65 7320 6120 7374 7269 6e67  : Takes a string
-00000970: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-00000980: 6e61 6d65 206f 6620 7468 6520 7469 6d65  name of the time
-00000990: 2073 706c 6974 2063 6f6c 756d 6e2e 2049   split column. I
-000009a0: 6620 6e6f 7420 7072 6f76 6964 6564 2c0a  f not provided,.
-000009b0: 2020 2020 426c 7565 4361 7374 2077 696c      BlueCast wil
-000009c0: 6c20 6e6f 7420 7370 6c69 7420 7468 6520  l not split the 
-000009d0: 6461 7461 2062 7920 7469 6d65 206f 7220  data by time or 
-000009e0: 6f72 6465 722c 2062 7574 2064 6f20 6120  order, but do a 
-000009f0: 7261 6e64 6f6d 2073 706c 6974 2069 6e73  random split ins
-00000a00: 7465 6164 2e0a 2020 2020 3a70 6172 616d  tead..    :param
-00000a10: 203a 6d6c 5f6d 6f64 656c 3a20 5461 6b65   :ml_model: Take
-00000a20: 7320 616e 2069 6e73 7461 6e63 6520 6f66  s an instance of
-00000a30: 2061 2058 6762 6f6f 7374 4d6f 6465 6c20   a XgboostModel 
-00000a40: 636c 6173 732e 2049 6620 6e6f 7420 7072  class. If not pr
-00000a50: 6f76 6964 6564 2c20 426c 7565 4361 7374  ovided, BlueCast
-00000a60: 2077 696c 6c20 696e 7374 616e 7469 6174   will instantiat
-00000a70: 6520 6f6e 652e 0a20 2020 2054 6869 7320  e one..    This 
-00000a80: 6973 2061 6e20 4150 4920 746f 2070 6173  is an API to pas
-00000a90: 7320 616e 7920 6d6f 6465 6c20 636c 6173  s any model clas
-00000aa0: 732e 2049 6e68 6572 6974 2074 6865 2062  s. Inherit the b
-00000ab0: 6173 6563 6c61 7373 2066 726f 6d20 6d6c  aseclass from ml
-00000ac0: 5f6d 6f64 656c 6c69 6e67 2e62 6173 655f  _modelling.base_
-00000ad0: 6d6f 6465 6c2e 4261 7365 4d6f 6465 6c2e  model.BaseModel.
-00000ae0: 0a20 2020 203a 7061 7261 6d20 6375 7374  .    :param cust
-00000af0: 6f6d 5f70 7265 7072 6f63 6573 736f 723a  om_preprocessor:
-00000b00: 2054 616b 6573 2061 6e20 696e 7374 616e   Takes an instan
-00000b10: 6365 206f 6620 6120 4375 7374 6f6d 5072  ce of a CustomPr
-00000b20: 6570 726f 6365 7373 696e 6720 636c 6173  eprocessing clas
-00000b30: 732e 2041 6c6c 6f77 7320 7573 6572 7320  s. Allows users 
-00000b40: 746f 2069 6e6a 6563 7420 6375 7374 6f6d  to inject custom
-00000b50: 0a20 2020 2070 7265 7072 6f63 6573 7369  .    preprocessi
-00000b60: 6e67 2073 7465 7073 2077 6869 6368 2074  ng steps which t
-00000b70: 616b 6520 706c 6163 6520 7269 6768 7420  ake place right 
-00000b80: 6166 7465 7220 7468 6520 7472 6169 6e20  after the train 
-00000b90: 7465 7374 2073 7069 742e 0a20 2020 203a  test spit..    :
-00000ba0: 7061 7261 6d20 6375 7374 6f6d 5f6c 6173  param custom_las
-00000bb0: 745f 6d69 6c65 5f63 6f6d 7075 7461 7469  t_mile_computati
-00000bc0: 6f6e 3a20 5461 6b65 7320 616e 2069 6e73  on: Takes an ins
-00000bd0: 7461 6e63 6520 6f66 2061 2043 7573 746f  tance of a Custo
-00000be0: 6d50 7265 7072 6f63 6573 7369 6e67 2063  mPreprocessing c
-00000bf0: 6c61 7373 2e20 416c 6c6f 7773 2075 7365  lass. Allows use
-00000c00: 7273 2074 6f20 696e 6a65 6374 2063 7573  rs to inject cus
-00000c10: 746f 6d0a 2020 2020 7072 6570 726f 6365  tom.    preproce
-00000c20: 7373 696e 6720 7374 6570 7320 7768 6963  ssing steps whic
-00000c30: 6820 7461 6b65 2070 6c61 6365 2072 6967  h take place rig
-00000c40: 6874 2062 6566 6f72 6520 7468 6520 6d6f  ht before the mo
-00000c50: 6465 6c20 7472 6169 6e69 6e67 2e0a 2020  del training..  
-00000c60: 2020 4e29 02da 0662 696e 6172 79da 0a6d    N)...binary..m
-00000c70: 756c 7469 636c 6173 7329 0cda 0d63 6c61  ulticlass)...cla
-00000c80: 7373 5f70 726f 626c 656d da0d 7461 7267  ss_problem..targ
-00000c90: 6574 5f63 6f6c 756d 6eda 0b63 6174 5f63  et_column..cat_c
-00000ca0: 6f6c 756d 6e73 da0c 6461 7465 5f63 6f6c  olumns..date_col
-00000cb0: 756d 6e73 da11 7469 6d65 5f73 706c 6974  umns..time_split
-00000cc0: 5f63 6f6c 756d 6eda 086d 6c5f 6d6f 6465  _column..ml_mode
-00000cd0: 6cda 1c63 7573 746f 6d5f 6c61 7374 5f6d  l..custom_last_m
-00000ce0: 696c 655f 636f 6d70 7574 6174 696f 6eda  ile_computation.
-00000cf0: 1363 7573 746f 6d5f 7072 6570 726f 6365  .custom_preproce
-00000d00: 7373 6f72 da17 6375 7374 6f6d 5f66 6561  ssor..custom_fea
-00000d10: 7475 7265 5f73 656c 6563 746f 72da 0d63  ture_selector..c
-00000d20: 6f6e 665f 7472 6169 6e69 6e67 da0c 636f  onf_training..co
-00000d30: 6e66 5f78 6762 6f6f 7374 da13 636f 6e66  nf_xgboost..conf
-00000d40: 5f70 6172 616d 735f 7867 626f 6f73 7463  _params_xgboostc
-00000d50: 0d00 0000 0000 0000 0000 0000 0d00 0000  ................
-00000d60: 0200 0000 4300 0000 7370 0000 007c 017c  ....C...sp...|.|
-00000d70: 005f 0064 017c 005f 017c 037c 005f 027c  ._.d.|._.|.|._.|
-00000d80: 047c 005f 037c 057c 005f 047c 027c 005f  .|._.|.|._.|.|._
-00000d90: 057c 0a7c 005f 067c 0b7c 005f 077c 0c7c  .|.|._.|.|._.|.|
-00000da0: 005f 0864 007c 005f 0964 007c 005f 0a64  ._.d.|._.d.|._.d
-00000db0: 007c 005f 0b64 007c 005f 0c7c 067c 005f  .|._.d.|._.|.|._
-00000dc0: 0d7c 077c 005f 0e7c 087c 005f 0f7c 097c  .|.|._.|.|._.|.|
-00000dd0: 005f 1064 007c 005f 1164 0053 0029 024e  ._.d.|._.d.S.).N
-00000de0: 4629 1272 1f00 0000 da0f 7072 6564 6963  F).r......predic
-00000df0: 7469 6f6e 5f6d 6f64 6572 2100 0000 7222  tion_moder!...r"
-00000e00: 0000 0072 2300 0000 7220 0000 0072 2800  ...r#...r ...r(.
-00000e10: 0000 7229 0000 0072 2a00 0000 da12 6665  ..r)...r*.....fe
-00000e20: 6174 5f74 7970 655f 6465 7465 6374 6f72  at_type_detector
-00000e30: da0b 6361 745f 656e 636f 6465 72da 1474  ..cat_encoder..t
-00000e40: 6172 6765 745f 6c61 6265 6c5f 656e 636f  arget_label_enco
-00000e50: 6465 72da 0f73 6368 656d 615f 6465 7465  der..schema_dete
-00000e60: 6374 6f72 7224 0000 0072 2500 0000 7226  ctorr$...r%...r&
-00000e70: 0000 0072 2700 0000 da0b 7368 6170 5f76  ...r'.....shap_v
-00000e80: 616c 7565 7329 0dda 0473 656c 6672 1f00  alues)...selfr..
-00000e90: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00000ea0: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00000eb0: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
-00000ec0: 2900 0000 722a 0000 00a9 0072 3200 0000  )...r*.....r2...
-00000ed0: fa3e 2f68 6f6d 652f 7468 6f6d 6173 2f49  .>/home/thomas/I
-00000ee0: 6465 6150 726f 6a65 6374 732f 426c 7565  deaProjects/Blue
-00000ef0: 4361 7374 2f62 6c75 6563 6173 742f 626c  Cast/bluecast/bl
-00000f00: 7565 7072 696e 7473 2f63 6173 742e 7079  ueprints/cast.py
-00000f10: da08 5f5f 696e 6974 5f5f 3c00 0000 7326  ..__init__<...s&
-00000f20: 0000 0000 1106 0106 0106 0106 0106 0106  ................
-00000f30: 0106 0106 0106 0106 0302 fe04 0306 0106  ................
-00000f40: 0106 0106 0106 0106 017a 1142 6c75 6543  .........z.BlueC
-00000f50: 6173 742e 5f5f 696e 6974 5f5f 2902 da02  ast.__init__)...
-00000f60: 6466 da06 7265 7475 726e 6302 0000 0000  df..returnc.....
-00000f70: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-00000f80: 0000 0073 3001 0000 7c00 6a00 730e 7401  ...s0...|.j.s.t.
-00000f90: 8300 7c00 5f00 7c00 6a00 6a02 732a 6401  ..|._.|.j.j.s*d.
-00000fa0: 7d02 7403 6a04 7c02 7405 6402 6403 8d03  }.t.j.|.t.d.d...
-00000fb0: 0100 7c00 6a00 6a06 6404 6b02 724a 6405  ..|.j.j.d.k.rJd.
-00000fc0: 7d02 7403 6a04 7c02 7405 6402 6403 8d03  }.t.j.|.t.d.d...
-00000fd0: 0100 7c00 6a00 6a02 726c 7c00 6a07 736c  ..|.j.j.rl|.j.sl
-00000fe0: 6406 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-00000ff0: 8d03 0100 7c00 6a08 7386 6407 7d02 7403  ....|.j.s.d.}.t.
-00001000: 6a04 7c02 7405 6402 6403 8d03 0100 7c00  j.|.t.d.d.....|.
-00001010: 6a00 6a09 740a 7c01 6a0b 8301 6b05 72b4  j.j.t.|.j...k.r.
-00001020: 7c00 6a00 6a02 72b4 6408 7d02 7403 6a04  |.j.j.r.d.}.t.j.
-00001030: 7c02 7405 6402 6403 8d03 0100 7c00 6a00  |.t.d.d.....|.j.
-00001040: 6a0c 72e0 7c00 6a00 6a0d 72e0 6409 7c00  j.r.|.j.j.r.d.|.
-00001050: 6a00 5f0d 640a 7d02 7403 6a04 7c02 7405  j._.d.}.t.j.|.t.
-00001060: 6402 6403 8d03 0100 7c00 6a00 6a0c 9001  d.d.....|.j.j...
-00001070: 7206 7c00 6a0e 9001 7206 640b 7d02 7403  r.|.j...r.d.}.t.
-00001080: 6a04 7c02 7405 6402 6403 8d03 0100 7c00  j.|.t.d.d.....|.
-00001090: 6a00 6a0c 9001 722c 7c00 6a0f 9001 722c  j.j...r,|.j...r,
-000010a0: 640c 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-000010b0: 8d03 0100 6400 5300 290d 4e61 9301 0000  ....d.S.).Na....
-000010c0: 4665 6174 7572 6520 7365 6c65 6374 696f  Feature selectio
-000010d0: 6e20 6973 2064 6973 6162 6c65 642e 2055  n is disabled. U
-000010e0: 7064 6174 6520 7468 6520 5472 6169 6e69  pdate the Traini
-000010f0: 6e67 436f 6e66 6967 2070 6172 616d 2027  ngConfig param '
-00001100: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
-00001110: 656c 6563 7469 6f6e 270a 2020 2020 2020  election'.      
-00001120: 2020 2020 2020 746f 2065 6e61 626c 6520        to enable 
-00001130: 6974 206f 7220 6d61 6b65 2075 7365 206f  it or make use o
-00001140: 6620 6120 6375 7374 6f6d 2070 7265 7072  f a custom prepr
-00001150: 6f63 6573 736f 7220 746f 2064 6f20 6974  ocessor to do it
-00001160: 206d 616e 7561 6c6c 7920 6475 7269 6e67   manually during
-00001170: 2074 6865 206c 6173 7420 6d69 6c65 2063   the last mile c
-00001180: 6f6d 7075 7461 7469 6f6e 7320 7374 6570  omputations step
-00001190: 2e0a 2020 2020 2020 2020 2020 2020 4665  ..            Fe
-000011a0: 6174 7572 6520 7365 6c65 6374 696f 6e20  ature selection 
-000011b0: 6973 2072 6563 6f6d 6d65 6e64 6564 2066  is recommended f
-000011c0: 6f72 2064 6174 6173 6574 7320 7769 7468  or datasets with
-000011d0: 206d 616e 7920 6665 6174 7572 6573 2028   many features (
-000011e0: 3e31 3030 3029 2e20 466f 7220 6461 7461  >1000). For data
-000011f0: 7365 7473 2077 6974 6820 6120 736d 616c  sets with a smal
-00001200: 6c20 616d 6f75 6e74 0a20 2020 2020 2020  l amount.       
-00001210: 2020 2020 206f 6620 6665 6174 7572 6573       of features
-00001220: 2066 6561 7475 7265 2073 656c 6563 7469   feature selecti
-00001230: 6f6e 2069 7320 6e6f 7420 7265 636f 6d6d  on is not recomm
-00001240: 656e 6465 642e 0a20 2020 2020 2020 2020  ended..         
-00001250: 2020 20e9 0200 0000 2901 da0a 7374 6163     .....)...stac
-00001260: 6b6c 6576 656c e901 0000 0061 0501 0000  klevel.....a....
-00001270: 4372 6f73 7320 7661 6c69 6461 7469 6f6e  Cross validation
-00001280: 2069 7320 6469 7361 626c 6564 2e20 5570   is disabled. Up
-00001290: 6461 7465 2074 6865 2054 7261 696e 696e  date the Trainin
-000012a0: 6743 6f6e 6669 6720 7061 7261 6d20 2768  gConfig param 'h
-000012b0: 7970 6572 7475 6e69 6e67 5f63 765f 666f  ypertuning_cv_fo
-000012c0: 6c64 7327 0a20 2020 2020 2020 2020 2020  lds'.           
-000012d0: 2074 6f20 656e 6162 6c65 2069 742e 2043   to enable it. C
-000012e0: 726f 7373 2076 616c 6964 6174 696f 6e20  ross validation 
-000012f0: 6973 2064 6973 6162 6c65 6420 6f6e 2064  is disabled on d
-00001300: 6566 6175 6c74 2074 6f20 616c 6c6f 7720  efault to allow 
-00001310: 6661 7374 2070 726f 746f 7479 7069 6e67  fast prototyping
-00001320: 2e20 466f 7220 726f 6275 7374 2068 7970  . For robust hyp
-00001330: 6572 7061 7261 6d65 7465 720a 2020 2020  erparameter.    
-00001340: 2020 2020 2020 2020 7475 6e69 6e67 2075          tuning u
-00001350: 7369 6e67 2061 7420 6c65 6173 7420 3520  sing at least 5 
-00001360: 666f 6c64 7320 6973 2072 6563 6f6d 6d65  folds is recomme
-00001370: 6e64 6564 2e61 5f01 0000 4665 6174 7572  nded.a_...Featur
-00001380: 6520 7365 6c65 6374 696f 6e20 6973 2065  e selection is e
-00001390: 6e61 626c 6564 2062 7574 206e 6f20 6665  nabled but no fe
-000013a0: 6174 7572 6520 7365 6c65 6374 6f72 2068  ature selector h
-000013b0: 6173 2062 6565 6e20 7072 6f76 6964 6564  as been provided
-000013c0: 2e20 4661 6c6c 696e 6720 6261 636b 2074  . Falling back t
-000013d0: 6f0a 2020 2020 2020 2020 2020 2020 6372  o.            cr
-000013e0: 6f73 732d 7661 6c69 6461 7465 6420 6665  oss-validated fe
-000013f0: 6174 7572 6520 656c 696d 696e 6174 696f  ature eliminatio
-00001400: 6e2e 2053 7065 6369 6669 6361 6c6c 7920  n. Specifically 
-00001410: 666f 7220 736d 616c 6c20 6461 7461 7365  for small datase
-00001420: 7473 2063 6865 636b 2074 6865 206c 6f67  ts check the log
-00001430: 7320 746f 2076 6572 6966 7920 7468 6174  s to verify that
-00001440: 206e 6f74 2074 6f6f 0a20 2020 2020 2020   not too.       
-00001450: 2020 2020 206d 616e 7920 6665 6174 7572       many featur
-00001460: 6573 2068 6176 6520 6265 656e 2072 656d  es have been rem
-00001470: 6f76 6564 2e20 4f74 6865 7277 6973 652c  oved. Otherwise,
-00001480: 2063 6f6e 7369 6465 7220 6469 7361 626c   consider disabl
-00001490: 696e 6720 6665 6174 7572 6520 7365 6c65  ing feature sele
-000014a0: 6374 696f 6e20 6f72 2070 726f 7669 6469  ction or providi
-000014b0: 6e67 2061 2063 7573 746f 6d0a 2020 2020  ng a custom.    
-000014c0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
-000014d0: 7365 6c65 6374 6f72 2e61 6501 0000 4e6f  selector.ae...No
-000014e0: 2058 6762 6f6f 7374 5475 6e65 5061 7261   XgboostTunePara
-000014f0: 6d73 436f 6e66 6967 2068 6173 2062 6565  msConfig has bee
-00001500: 6e20 7072 6f76 6964 6564 2e20 4661 6c6c  n provided. Fall
-00001510: 696e 6720 6261 636b 2074 6f20 6465 6661  ing back to defa
-00001520: 756c 7420 7661 6c75 6573 2e20 4465 6661  ult values. Defa
-00001530: 756c 7420 7661 6c75 6573 0a20 2020 2020  ult values.     
-00001540: 2020 2020 2020 2068 6176 6520 6265 656e         have been
-00001550: 2063 686f 7365 6e20 746f 2073 7065 6564   chosen to speed
-00001560: 2075 7020 7468 6520 7072 6f74 6f74 7970   up the prototyp
-00001570: 696e 672e 2046 6f72 2072 6f62 7573 7420  ing. For robust 
-00001580: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
-00001590: 756e 696e 6720 636f 6e73 6964 6572 2070  uning consider p
-000015a0: 726f 7669 6469 6e67 2061 2063 7573 746f  roviding a custo
-000015b0: 6d0a 2020 2020 2020 2020 2020 2020 5867  m.            Xg
-000015c0: 626f 6f73 7454 756e 6550 6172 616d 7343  boostTuneParamsC
-000015d0: 6f6e 6669 6720 7769 7468 2061 2064 6565  onfig with a dee
-000015e0: 7065 7220 6879 7065 7270 6172 616d 6574  per hyperparamet
-000015f0: 6572 2073 6561 7263 6820 7370 6163 6520  er search space 
-00001600: 616e 6420 6120 6375 7374 6f6d 2054 7261  and a custom Tra
-00001610: 696e 696e 6743 6f6e 6669 6720 746f 2065  iningConfig to e
-00001620: 6e61 626c 650a 2020 2020 2020 2020 2020  nable.          
-00001630: 2020 6372 6f73 732d 7661 6c69 6461 7469    cross-validati
-00001640: 6f6e 2e61 0f01 0000 5468 6520 6d69 6e69  on.a....The mini
-00001650: 6d75 6d20 6e75 6d62 6572 206f 6620 6665  mum number of fe
-00001660: 6174 7572 6573 2074 6f20 7365 6c65 6374  atures to select
-00001670: 2069 7320 6772 6561 7465 7220 6f72 2065   is greater or e
-00001680: 7175 616c 2074 6f20 7468 6520 6e75 6d62  qual to the numb
-00001690: 6572 206f 6620 6665 6174 7572 6573 2069  er of features i
-000016a0: 6e0a 2020 2020 2020 2020 2020 2020 7468  n.            th
-000016b0: 6520 6461 7461 7365 7420 7768 696c 6520  e dataset while 
-000016c0: 6665 6174 7572 6520 7365 6c65 6374 696f  feature selectio
-000016d0: 6e20 6973 2065 6e61 626c 6564 2e20 436f  n is enabled. Co
-000016e0: 6e73 6964 6572 2072 6564 7563 696e 6720  nsider reducing 
-000016f0: 7468 6520 6d69 6e69 6d75 6d20 6e75 6d62  the minimum numb
-00001700: 6572 206f 6620 6665 6174 7572 6573 2074  er of features t
-00001710: 6f0a 2020 2020 2020 2020 2020 2020 7365  o.            se
-00001720: 6c65 6374 206f 7220 6469 7361 626c 696e  lect or disablin
-00001730: 6720 6665 6174 7572 6520 7365 6c65 6374  g feature select
-00001740: 696f 6e20 7669 6120 5472 6169 6e69 6e67  ion via Training
-00001750: 436f 6e66 6967 2e46 612b 0200 0053 4841  Config.Fa+...SHA
-00001760: 5020 7661 6c75 6573 2063 616e 6e6f 7420  P values cannot 
-00001770: 6265 2063 616c 6375 6c61 7465 6420 7768  be calculated wh
-00001780: 656e 2063 6174 6567 6f72 6963 616c 2065  en categorical e
-00001790: 6e63 6f64 696e 6720 7669 6120 4d4c 2061  ncoding via ML a
-000017a0: 6c67 6f72 6974 686d 2069 7320 656e 6162  lgorithm is enab
-000017b0: 6c65 6420 6475 6520 746f 0a20 2020 2020  led due to.     
-000017c0: 2020 2020 2020 2069 6e63 6f6d 7061 7469         incompati
-000017d0: 6269 6c69 7479 2077 6974 6820 7468 6520  bility with the 
-000017e0: 7368 6170 206c 6962 7261 7279 2e20 5365  shap library. Se
-000017f0: 6520 7468 6973 2047 6974 4875 6220 6973  e this GitHub is
-00001800: 7375 6520 666f 7220 6d6f 7265 2063 6f6e  sue for more con
-00001810: 7465 7874 3a0a 2020 2020 2020 2020 2020  text:.          
-00001820: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00001830: 2e63 6f6d 2f73 6c75 6e64 6265 7267 2f73  .com/slundberg/s
-00001840: 6861 702f 6973 7375 6573 2f32 3636 0a0a  hap/issues/266..
-00001850: 2020 2020 2020 2020 2020 2020 4361 6c63              Calc
-00001860: 756c 6174 696f 6e20 6f66 2053 6861 7020  ulation of Shap 
-00001870: 7661 6c75 6573 2068 6173 2062 6565 6e20  values has been 
-00001880: 6368 616e 6765 6420 746f 2066 616c 7365  changed to false
-00001890: 2e0a 2020 2020 2020 2020 2020 2020 436f  ..            Co
-000018a0: 6e73 6964 6572 2064 6973 6162 6c69 6e67  nsider disabling
-000018b0: 2063 6174 6567 6f72 6963 616c 2065 6e63   categorical enc
-000018c0: 6f64 696e 6720 7669 6120 4d4c 2061 6c67  oding via ML alg
-000018d0: 6f72 6974 686d 2069 6e20 7468 6520 5472  orithm in the Tr
-000018e0: 6169 6e69 6e67 436f 6e66 6967 2069 6620  ainingConfig if 
-000018f0: 7368 6170 2076 616c 7565 7320 6172 650a  shap values are.
-00001900: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-00001910: 6972 6564 2e20 416c 7465 726e 6174 6976  ired. Alternativ
-00001920: 656c 7920 7573 6520 5867 626f 6f73 7420  ely use Xgboost 
-00001930: 6173 2061 2063 7573 746f 6d20 6d6f 6465  as a custom mode
-00001940: 6c20 616e 6420 6361 6c63 756c 6174 6520  l and calculate 
-00001950: 7368 6170 2076 616c 7565 7320 6d61 6e75  shap values manu
-00001960: 616c 6c79 2076 6961 0a20 2020 2020 2020  ally via.       
-00001970: 2020 2020 2070 7265 645f 636f 6e74 7269       pred_contri
-00001980: 6273 3d54 7275 652e 7af0 4361 7465 676f  bs=True.z.Catego
-00001990: 7269 6361 6c20 656e 636f 6469 6e67 2076  rical encoding v
-000019a0: 6961 204d 4c20 616c 676f 7269 7468 6d20  ia ML algorithm 
-000019b0: 6973 2065 6e61 626c 6564 2e20 4d61 6b65  is enabled. Make
-000019c0: 2073 7572 6520 746f 2068 616e 646c 6520   sure to handle 
-000019d0: 6361 7465 676f 7269 6361 6c20 6665 6174  categorical feat
-000019e0: 7572 6573 0a20 2020 2020 2020 2020 2020  ures.           
-000019f0: 2077 6974 6869 6e20 7468 6520 7072 6f76   within the prov
-00001a00: 6964 6564 206d 6c20 6d6f 6465 6c20 6f72  ided ml model or
-00001a10: 2063 6f6e 7369 6465 7220 6469 7361 626c   consider disabl
-00001a20: 696e 6720 6361 7465 676f 7269 6361 6c20  ing categorical 
-00001a30: 656e 636f 6469 6e67 2076 6961 204d 4c20  encoding via ML 
-00001a40: 616c 676f 7269 7468 6d20 696e 2074 6865  algorithm in the
-00001a50: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
-00001a60: 696e 696e 6743 6f6e 6669 6720 616c 7465  iningConfig alte
-00001a70: 726e 6174 6976 656c 792e 7afd 4361 7465  rnatively.z.Cate
-00001a80: 676f 7269 6361 6c20 656e 636f 6469 6e67  gorical encoding
-00001a90: 2076 6961 204d 4c20 616c 676f 7269 7468   via ML algorith
-00001aa0: 6d20 6973 2065 6e61 626c 6564 2e20 4d61  m is enabled. Ma
-00001ab0: 6b65 2073 7572 6520 746f 2068 616e 646c  ke sure to handl
-00001ac0: 6520 6361 7465 676f 7269 6361 6c20 6665  e categorical fe
-00001ad0: 6174 7572 6573 0a20 2020 2020 2020 2020  atures.         
-00001ae0: 2020 2077 6974 6869 6e20 7468 6520 7072     within the pr
-00001af0: 6f76 6964 6564 206c 6173 7420 6d69 6c65  ovided last mile
-00001b00: 2063 6f6d 7075 7461 7469 6f6e 206f 7220   computation or 
-00001b10: 636f 6e73 6964 6572 2064 6973 6162 6c69  consider disabli
-00001b20: 6e67 2063 6174 6567 6f72 6963 616c 2065  ng categorical e
-00001b30: 6e63 6f64 696e 6720 7669 6120 4d4c 2061  ncoding via ML a
-00001b40: 6c67 6f72 6974 686d 2069 6e20 7468 650a  lgorithm in the.
-00001b50: 2020 2020 2020 2020 2020 2020 5472 6169              Trai
-00001b60: 6e69 6e67 436f 6e66 6967 2061 6c74 6572  ningConfig alter
-00001b70: 6e61 7469 7665 6c79 2e29 1072 2800 0000  natively.).r(...
-00001b80: 720a 0000 00da 1865 6e61 626c 655f 6665  r......enable_fe
-00001b90: 6174 7572 655f 7365 6c65 6374 696f 6eda  ature_selection.
-00001ba0: 0877 6172 6e69 6e67 73da 0477 6172 6eda  .warnings..warn.
-00001bb0: 0b55 7365 7257 6172 6e69 6e67 5a14 6879  .UserWarningZ.hy
-00001bc0: 7065 7274 756e 696e 675f 6376 5f66 6f6c  pertuning_cv_fol
-00001bd0: 6473 7227 0000 0072 2900 0000 da16 6d69  dsr'...r).....mi
-00001be0: 6e5f 6665 6174 7572 6573 5f74 6f5f 7365  n_features_to_se
-00001bf0: 6c65 6374 da03 6c65 6eda 0763 6f6c 756d  lect..len..colum
-00001c00: 6e73 da1d 6361 745f 656e 636f 6469 6e67  ns..cat_encoding
-00001c10: 5f76 6961 5f6d 6c5f 616c 676f 7269 7468  _via_ml_algorith
-00001c20: 6dda 1563 616c 6375 6c61 7465 5f73 6861  m..calculate_sha
-00001c30: 705f 7661 6c75 6573 7224 0000 0072 2500  p_valuesr$...r%.
-00001c40: 0000 2903 7231 0000 0072 3500 0000 da07  ..).r1...r5.....
-00001c50: 6d65 7373 6167 6572 3200 0000 7232 0000  messager2...r2..
-00001c60: 0072 3300 0000 da0e 696e 6974 6961 6c5f  .r3.....initial_
-00001c70: 6368 6563 6b73 6200 0000 734e 0000 0000  checksb...sN....
-00001c80: 0106 0108 0108 0104 0510 020c 0104 0310  ................
-00001c90: 0306 ff02 0204 fe02 0404 0410 0106 0104  ................
-00001ca0: 0410 0210 ff02 0206 fe02 0404 0310 0206  ................
-00001cb0: ff02 0206 fe02 0408 0104 0810 0112 0104  ................
-00001cc0: 0310 0206 ff04 0204 fe04 0404 037a 1742  .............z.B
-00001cd0: 6c75 6543 6173 742e 696e 6974 6961 6c5f  lueCast.initial_
-00001ce0: 6368 6563 6b73 2903 7235 0000 00da 0a74  checks).r5.....t
-00001cf0: 6172 6765 745f 636f 6c72 3600 0000 6303  arget_colr6...c.
-00001d00: 0000 0000 0000 0000 0000 0009 0000 0007  ................
-00001d10: 0000 0043 0000 0073 2803 0000 7400 8300  ...C...s(...t...
-00001d20: 0100 7401 8300 7d03 7c03 a002 7c01 a101  ..t...}.|...|...
-00001d30: 7d01 7c03 7c00 5f03 7c00 6a03 6a04 7252  }.|.|._.|.j.j.rR
-00001d40: 7c00 6a05 7c00 6a03 6a04 6b06 7252 7406  |.j.|.j.j.k.rRt.
-00001d50: 8300 7c00 5f07 7c00 6a07 a008 7c01 7c00  ..|._.|.j...|.|.
-00001d60: 6a05 1900 a101 7c01 7c00 6a05 3c00 7c00  j.....|.|.j.<.|.
-00001d70: 6a03 6a04 7c00 5f04 7c00 6a03 6a09 7c00  j.j.|._.|.j.j.|.
-00001d80: 5f09 7c00 6a0a 7374 740b 8300 7c00 5f0a  _.|.j.stt...|._.
-00001d90: 7c00 a00c 7c01 a101 0100 740d 7c01 7c02  |...|.....t.|.|.
-00001da0: 7c00 6a0e 7c00 6a0a 6a0f 7c00 6a0a 6a10  |.j.|.j.j.|.j.j.
-00001db0: 7c00 6a0a 6a11 8306 5c04 7d04 7d05 7d06  |.j.j...\.}.}.}.
-00001dc0: 7d07 7c00 6a12 9001 7232 7c00 6a12 a013  }.|.j...r2|.j...
-00001dd0: 7c04 7c06 a102 5c02 7d04 7d06 7c00 6a12  |.|...\.}.}.|.j.
-00001de0: 6a14 7c05 7c07 6401 6402 8d03 5c02 7d05  j.|.|.d.d...\.}.
-00001df0: 7d07 7401 8300 7d03 7c03 a002 7c04 a101  }.t...}.|...|...
-00001e00: 7d08 7c04 6a15 6403 6404 8d01 7c06 6a15  }.|.j.d.d...|.j.
-00001e10: 6403 6404 8d01 0200 7d04 7d06 7c05 6a15  d.d.....}.}.|.j.
-00001e20: 6403 6404 8d01 7c07 6a15 6403 6404 8d01  d.d...|.j.d.d...
-00001e30: 0200 7d05 7d07 7c02 7c03 6a04 6b06 9001  ..}.}.|.|.j.k...
-00001e40: 7232 7c03 6a04 a016 7c02 a101 0100 7417  r2|.j...|.....t.
-00001e50: 7c04 8301 7417 7c05 8301 0200 7d04 7d05  |...t.|.....}.}.
-00001e60: 7418 7c04 7c00 6a09 8302 7418 7c05 7c00  t.|.|.j...t.|.|.
-00001e70: 6a09 8302 0200 7d04 7d05 7419 8300 7c00  j.....}.}.t...|.
-00001e80: 5f1a 7c00 6a1a a01b 7c04 a101 0100 7c00  _.|.j...|.....|.
-00001e90: 6a1a a014 7c05 a101 7d05 7c00 6a04 6405  j...|...}.|.j.d.
-00001ea0: 6b09 9001 72c8 7c00 6a1c 6406 6b02 9001  k...r.|.j.d.k...
-00001eb0: 72c8 7c00 6a0a 6a1d 9001 73c8 741e 7c03  r.|.j.j...s.t.|.
-00001ec0: 6a04 8301 7c00 5f1f 7c00 6a1f a020 7c04  j...|._.|.j.. |.
-00001ed0: 7c06 a102 7d04 7c00 6a1f a021 7c05 a101  |...}.|.j..!|...
-00001ee0: 7d05 6e80 7c00 6a04 6405 6b09 9002 7212  }.n.|.j.d.k...r.
-00001ef0: 7c00 6a1c 6407 6b02 9002 7212 7c00 6a0a  |.j.d.k...r.|.j.
-00001f00: 6a1d 9002 7312 7422 7c03 6a04 8301 7c00  j...s.t"|.j...|.
-00001f10: 5f1f 7c00 6a1f a023 7c04 7c06 a102 7d04  _.|.j..#|.|...}.
-00001f20: 7c00 6a1f a024 7c05 a101 7d05 6e36 7c00  |.j..$|...}.n6|.
-00001f30: 6a0a 6a1d 9002 7248 7c04 7c00 6a04 1900  j.j...rH|.|.j...
-00001f40: a025 6408 a101 7c04 7c00 6a04 3c00 7c05  .%d...|.|.j.<.|.
-00001f50: 7c00 6a04 1900 a025 6408 a101 7c05 7c00  |.j....%d...|.|.
-00001f60: 6a04 3c00 7c00 6a26 9002 7278 7c00 6a26  j.<.|.j&..rx|.j&
-00001f70: a013 7c04 7c06 a102 5c02 7d04 7d06 7c00  ..|.|...\.}.}.|.
-00001f80: 6a26 6a14 7c05 7c07 6401 6402 8d03 5c02  j&j.|.|.d.d...\.
-00001f90: 7d05 7d07 7c00 6a27 9002 7396 7428 7c00  }.}.|.j'..s.t(|.
-00001fa0: 6a0a 6a10 7c00 6a0a 6a29 6409 8d02 7c00  j.j.|.j.j)d...|.
-00001fb0: 5f27 7c00 6a0a 6a2a 9002 72c6 7c00 6a27  _'|.j.j*..r.|.j'
-00001fc0: a013 7c04 7c06 a102 5c02 7d04 7d06 7c00  ..|.|...\.}.}.|.
-00001fd0: 6a27 6a14 7c05 6401 6402 8d02 5c02 7d05  j'j.|.d.d...\.}.
-00001fe0: 7d08 7c00 6a2b 9002 73e8 742c 7c00 6a1c  }.|.j+..s.t,|.j.
-00001ff0: 7c00 6a0a 7c00 6a2d 7c00 6a2e 640a 8d04  |.j.|.j-|.j.d...
-00002000: 7c00 5f2b 7c00 6a2b a01b 7c04 7c05 7c06  |._+|.j+..|.|.|.
-00002010: 7c07 a104 0100 7c00 6a0a 9003 721e 7c00  |.....|.j...r.|.
-00002020: 6a0a 6a2f 9003 721e 7430 7c00 6a2b 6a31  j.j/..r.t0|.j+j1
-00002030: 7c05 640b 8303 7c00 5f32 6403 7c00 5f33  |.d...|._2d.|._3
-00002040: 6405 5300 290c 7a19 5472 6169 6e20 6120  d.S.).z.Train a 
-00002050: 6675 6c6c 204d 4c20 7069 7065 6c69 6e65  full ML pipeline
-00002060: 2e46 a901 5a0e 7072 6564 6963 746f 6e5f  .F..Z.predicton_
-00002070: 6d6f 6465 54a9 01da 0464 726f 704e 721d  modeT....dropNr.
-00002080: 0000 0072 1e00 0000 da08 6361 7465 676f  ...r......catego
-00002090: 7279 2902 da0c 7261 6e64 6f6d 5f73 7461  ry)...random_sta
-000020a0: 7465 723e 0000 0029 0372 2800 0000 7229  ter>...).r(...r)
-000020b0: 0000 0072 2a00 0000 da04 7472 6565 2934  ...r*.....tree)4
-000020c0: 720f 0000 0072 1600 0000 5a1b 6669 745f  r....r....Z.fit_
-000020d0: 7472 616e 7366 6f72 6d5f 6665 6174 7572  transform_featur
-000020e0: 655f 7479 7065 7372 2c00 0000 7221 0000  e_typesr,...r!..
-000020f0: 0072 2000 0000 7214 0000 0072 2e00 0000  .r ...r....r....
-00002100: 5a1b 6669 745f 7472 616e 7366 6f72 6d5f  Z.fit_transform_
-00002110: 7461 7267 6574 5f6c 6162 656c 7372 2200  target_labelsr".
-00002120: 0000 7228 0000 0072 0a00 0000 7244 0000  ..r(...r....rD..
-00002130: 0072 1b00 0000 7223 0000 00da 0a74 7261  .r....r#.....tra
-00002140: 696e 5f73 697a 65da 1367 6c6f 6261 6c5f  in_size..global_
-00002150: 7261 6e64 6f6d 5f73 7461 7465 5a14 7472  random_stateZ.tr
-00002160: 6169 6e5f 7370 6c69 745f 7374 7261 7469  ain_split_strati
-00002170: 6679 7226 0000 00da 0d66 6974 5f74 7261  fyr&.....fit_tra
-00002180: 6e73 666f 726d da09 7472 616e 7366 6f72  nsform..transfor
-00002190: 6dda 0b72 6573 6574 5f69 6e64 6578 da06  m..reset_index..
-000021a0: 7265 6d6f 7665 7217 0000 0072 1300 0000  remover....r....
-000021b0: 7218 0000 0072 2f00 0000 da03 6669 7472  r....r/.....fitr
-000021c0: 1f00 0000 7241 0000 0072 1900 0000 722d  ....rA...r....r-
-000021d0: 0000 005a 1e66 6974 5f74 6172 6765 745f  ...Z.fit_target_
-000021e0: 656e 636f 6465 5f62 696e 6172 795f 636c  encode_binary_cl
-000021f0: 6173 73da 2474 7261 6e73 666f 726d 5f74  ass.$transform_t
-00002200: 6172 6765 745f 656e 636f 6465 5f62 696e  arget_encode_bin
-00002210: 6172 795f 636c 6173 7372 1a00 0000 5a1c  ary_classr....Z.
-00002220: 6669 745f 7461 7267 6574 5f65 6e63 6f64  fit_target_encod
-00002230: 655f 6d75 6c74 6963 6c61 7373 da22 7472  e_multiclass."tr
-00002240: 616e 7366 6f72 6d5f 7461 7267 6574 5f65  ansform_target_e
-00002250: 6e63 6f64 655f 6d75 6c74 6963 6c61 7373  ncode_multiclass
-00002260: da06 6173 7479 7065 7225 0000 0072 2700  ..astyper%...r'.
-00002270: 0000 7215 0000 0072 3e00 0000 723a 0000  ..r....r>...r:..
-00002280: 0072 2400 0000 7211 0000 0072 2900 0000  .r$...r....r)...
-00002290: 722a 0000 0072 4200 0000 720e 0000 00da  r*...rB...r.....
-000022a0: 056d 6f64 656c 7230 0000 0072 2b00 0000  .modelr0...r+...
-000022b0: 2909 7231 0000 0072 3500 0000 7245 0000  ).r1...r5...rE..
-000022c0: 0072 2c00 0000 da07 785f 7472 6169 6eda  .r,.....x_train.
-000022d0: 0678 5f74 6573 74da 0779 5f74 7261 696e  .x_test..y_train
-000022e0: da06 795f 7465 7374 da01 5f72 3200 0000  ..y_test.._r2...
-000022f0: 7232 0000 0072 3300 0000 7252 0000 00a6  r2...r3...rR....
-00002300: 0000 0073 d600 0000 0002 0601 0601 0a01  ...s............
-00002310: 0602 0801 0e01 0803 0601 08ff 02fe 0201  ................
-00002320: 04ff 0206 0a01 0a02 0601 0802 0a02 0201  ................
-00002330: 0201 0201 0401 0601 0601 06fa 0c09 0801  ................
-00002340: 1201 0601 0200 0200 02ff 0a03 0601 0a01  ................
-00002350: 0e01 02ff 0a03 0e01 02ff 0a03 0c01 0c02  ................
-00002360: 1201 0c01 0200 04ff 0804 0801 0c01 0c03  ................
-00002370: 08ff 0402 08fe 0403 06fd 0405 0c01 0e01  ................
-00002380: 0e02 08ff 0402 08fe 0403 06fd 0405 0c01  ................
-00002390: 0e01 0e01 0a01 1601 1602 0801 0601 0200  ................
-000023a0: 02ff 0803 0601 0200 0200 02ff 0a04 0801  ................
-000023b0: 0201 0601 06fe 0805 0a01 0601 0200 02ff  ................
-000023c0: 0803 0601 0200 02ff 0a04 0801 0201 0401  ................
-000023d0: 0401 0401 04fc 0806 1201 1201 1201 7a0c  ..............z.
-000023e0: 426c 7565 4361 7374 2e66 6974 2905 7235  BlueCast.fit).r5
-000023f0: 0000 00da 0764 665f 6576 616c da0b 7461  .....df_eval..ta
-00002400: 7267 6574 5f65 7661 6c72 4500 0000 7236  rget_evalrE...r6
-00002410: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
-00002420: 0800 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
-00002430: 007c 00a0 007c 017c 04a1 0201 007c 00a0  .|...|.|.....|..
-00002440: 017c 02a1 015c 027d 057d 0674 027c 036a  .|...\.}.}.t.|.j
-00002450: 037c 057c 0683 037d 077c 0753 0029 0161  .|.|...}.|.S.).a
-00002460: 8e02 0000 5472 6169 6e20 6120 6675 6c6c  ....Train a full
-00002470: 204d 4c20 7069 7065 6c69 6e65 2061 6e64   ML pipeline and
-00002480: 2065 7661 6c75 6174 6520 6f6e 2061 2068   evaluate on a h
-00002490: 6f6c 646f 7574 2073 6574 2e0a 0a20 2020  oldout set...   
-000024a0: 2020 2020 2054 6869 7320 6973 2061 2063       This is a c
-000024b0: 6f6e 7665 6e69 656e 6365 2066 756e 6374  onvenience funct
-000024c0: 696f 6e20 746f 2074 7261 696e 2061 6e64  ion to train and
-000024d0: 2065 7661 6c75 6174 6520 6f6e 2061 2068   evaluate on a h
-000024e0: 6f6c 646f 7574 2073 6574 2e20 4974 2069  oldout set. It i
-000024f0: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
-00002500: 2075 7365 2074 6869 7320 666f 7220 6d6f   use this for mo
-00002510: 6465 6c0a 2020 2020 2020 2020 6578 706c  del.        expl
-00002520: 6f72 6174 696f 6e2e 204f 6e20 7072 6f64  oration. On prod
-00002530: 7563 7469 6f6e 2074 6865 2073 696d 706c  uction the simpl
-00002540: 6520 6669 7428 2920 6675 6e63 7469 6f6e  e fit() function
-00002550: 2073 686f 756c 6420 6265 2075 7365 642e   should be used.
-00002560: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002570: 3a64 663a 2054 616b 6573 2061 2070 616e  :df: Takes a pan
-00002580: 6461 7320 4461 7461 4672 616d 6520 636f  das DataFrame co
-00002590: 6e74 6169 6e69 6e67 2074 6865 2074 7261  ntaining the tra
-000025a0: 696e 696e 6720 6461 7461 2061 6e64 2074  ining data and t
-000025b0: 6865 2074 6172 6765 7473 2e0a 2020 2020  he targets..    
-000025c0: 2020 2020 3a70 6172 616d 203a 6466 5f65      :param :df_e
-000025d0: 7661 6c3a 2054 616b 6573 2061 2070 616e  val: Takes a pan
-000025e0: 6461 7320 4461 7461 4672 616d 6520 636f  das DataFrame co
-000025f0: 6e74 6169 6e69 6e67 2074 6865 2065 7661  ntaining the eva
-00002600: 6c75 6174 696f 6e20 6461 7461 2c20 6275  luation data, bu
-00002610: 7420 6e6f 7420 7468 6520 7461 7267 6574  t not the target
-00002620: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
-00002630: 6d20 3a74 6172 6765 745f 6576 616c 3a20  m :target_eval: 
-00002640: 5461 6b65 7320 6120 7061 6e64 6173 2053  Takes a pandas S
-00002650: 6572 6965 7320 636f 6e74 6169 6e69 6e67  eries containing
-00002660: 2074 6865 2065 7661 6c75 6174 696f 6e20   the evaluation 
-00002670: 7461 7267 6574 732e 0a20 2020 2020 2020  targets..       
-00002680: 203a 7061 7261 6d20 3a74 6172 6765 745f   :param :target_
-00002690: 636f 6c3a 2054 616b 6573 2061 2073 7472  col: Takes a str
-000026a0: 696e 6720 636f 6e74 6169 6e69 6e67 2074  ing containing t
-000026b0: 6865 206e 616d 6520 6f66 2074 6865 2074  he name of the t
-000026c0: 6172 6765 7420 636f 6c75 6d6e 2069 6e73  arget column ins
-000026d0: 6964 6520 7468 6520 7472 6169 6e69 6e67  ide the training
-000026e0: 2064 6174 6120 6466 2e0a 2020 2020 2020   data df..      
-000026f0: 2020 2904 7252 0000 00da 0770 7265 6469    ).rR.....predi
-00002700: 6374 720d 0000 00da 0676 616c 7565 7329  ctr......values)
-00002710: 0872 3100 0000 7235 0000 0072 5c00 0000  .r1...r5...r\...
-00002720: 725d 0000 0072 4500 0000 da07 795f 7072  r]...rE.....y_pr
-00002730: 6f62 73da 0979 5f63 6c61 7373 6573 5a09  obs..y_classesZ.
-00002740: 6576 616c 5f64 6963 7472 3200 0000 7232  eval_dictr2...r2
-00002750: 0000 0072 3300 0000 da08 6669 745f 6576  ...r3.....fit_ev
-00002760: 616c 1601 0000 7308 0000 0000 100c 010e  al....s.........
-00002770: 010e 017a 1142 6c75 6543 6173 742e 6669  ...z.BlueCast.fi
-00002780: 745f 6576 616c 6302 0000 0000 0000 0000  t_evalc.........
-00002790: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-000027a0: 5801 0000 7400 8300 0100 7c00 6a01 7314  X...t.....|.j.s.
-000027b0: 7402 6401 8301 8201 7c00 6a03 7322 7402  t.d.....|.j.s"t.
-000027c0: 6402 8301 8201 7c00 6a01 6a04 7c01 7c00  d.....|.j.j.|.|.
-000027d0: 6a05 6701 6403 8d02 7d01 7c00 6a06 725c  j.g.d...}.|.j.r\
-000027e0: 7c00 6a06 6a07 7c01 6404 6405 8d02 5c02  |.j.j.|.d.d...\.
-000027f0: 7d01 7d02 7c01 6a08 6404 6406 8d01 7d01  }.}.|.j.d.d...}.
-00002800: 7409 7c01 8301 7d01 740a 7c01 7c00 6a0b  t.|...}.t.|.|.j.
-00002810: 8302 7d01 7c00 6a0c 7282 7c00 6a0c a007  ..}.|.j.r.|.j...
-00002820: 7c01 a101 7d01 7c00 6a0d 72ba 7c00 6a0e  |...}.|.j.r.|.j.
-00002830: 72ba 7c00 6a0f 6407 6b02 72ba 7410 7c00  r.|.j.d.k.r.t.|.
-00002840: 6a0e 7411 8302 72ba 7c00 6a03 6a12 73ba  j.t...r.|.j.j.s.
-00002850: 7c00 6a0e a013 7c01 a101 7d01 6e58 7c00  |.j...|...}.nX|.
-00002860: 6a0d 72f2 7c00 6a0e 72f2 7c00 6a0f 6408  j.r.|.j.r.|.j.d.
-00002870: 6b02 72f2 7410 7c00 6a0e 7414 8302 72f2  k.r.t.|.j.t...r.
-00002880: 7c00 6a03 6a12 73f2 7c00 6a0e a015 7c01  |.j.j.s.|.j...|.
-00002890: a101 7d01 6e20 7c00 6a03 6a12 9001 7212  ..}.n |.j.j...r.
-000028a0: 7c01 7c00 6a0d 1900 a016 6409 a101 7c01  |.|.j.....d...|.
-000028b0: 7c00 6a0d 3c00 7c00 6a17 9001 722e 7c00  |.j.<.|.j...r.|.
-000028c0: 6a17 6a07 7c01 6404 6405 8d02 5c02 7d01  j.j.|.d.d...\.}.
-000028d0: 7d02 7c00 6a18 9001 7254 7c00 6a03 6a19  }.|.j...rT|.j.j.
-000028e0: 9001 7254 7c00 6a18 6a07 7c01 6404 6405  ..rT|.j.j.|.d.d.
-000028f0: 8d02 5c02 7d01 7d02 7c01 5300 290a 7a37  ..\.}.}.|.S.).z7
-00002900: 5472 616e 7366 6f72 6d20 6e65 7720 6461  Transform new da
-00002910: 7461 2061 6363 6f72 6469 6e67 2074 6f20  ta according to 
-00002920: 7072 6570 726f 6365 7373 696e 6720 7069  preprocessing pi
-00002930: 7065 6c69 6e65 2efa 2a46 6561 7475 7265  peline..*Feature
-00002940: 2074 7970 6520 636f 6e76 6572 7465 7220   type converter 
-00002950: 636f 756c 6420 6e6f 7420 6265 2066 6f75  could not be fou
-00002960: 6e64 2e7a 2a54 7261 696e 696e 6720 636f  nd.z*Training co
-00002970: 6e66 6967 7572 6174 696f 6e20 636f 756c  nfiguration coul
-00002980: 6420 6e6f 7420 6265 2066 6f75 6e64 2e29  d not be found.)
-00002990: 015a 0b69 676e 6f72 655f 636f 6c73 5472  .Z.ignore_colsTr
-000029a0: 4600 0000 7247 0000 0072 1d00 0000 721e  F...rG...r....r.
-000029b0: 0000 0072 4900 0000 291a 720f 0000 0072  ...rI...).r....r
-000029c0: 2c00 0000 da09 4578 6365 7074 696f 6e72  ,.....Exceptionr
-000029d0: 2800 0000 5a17 7472 616e 7366 6f72 6d5f  (...Z.transform_
-000029e0: 6665 6174 7572 655f 7479 7065 7372 2000  feature_typesr .
-000029f0: 0000 7226 0000 0072 4f00 0000 7250 0000  ..r&...rO...rP..
-00002a00: 0072 1700 0000 7213 0000 0072 2200 0000  .r....r....r"...
-00002a10: 722f 0000 0072 2100 0000 722d 0000 0072  r/...r!...r-...r
-00002a20: 1f00 0000 da0a 6973 696e 7374 616e 6365  ......isinstance
-00002a30: 7219 0000 0072 4100 0000 7253 0000 0072  r....rA...rS...r
-00002a40: 1a00 0000 7254 0000 0072 5500 0000 7225  ....rT...rU...r%
-00002a50: 0000 0072 2700 0000 723a 0000 0029 0372  ...r'...r:...).r
-00002a60: 3100 0000 7235 0000 0072 5b00 0000 7232  1...r5...r[...r2
-00002a70: 0000 0072 3200 0000 7233 0000 00da 1274  ...r2...r3.....t
-00002a80: 7261 6e73 666f 726d 5f6e 6577 5f64 6174  ransform_new_dat
-00002a90: 612b 0100 0073 5a00 0000 0002 0601 0601  a+...sZ.........
-00002aa0: 0802 0601 0802 0601 0200 06ff 0604 0601  ................
-00002ab0: 1401 0c02 0801 0c02 0601 0c03 04ff 0202  ................
-00002ac0: 04fe 0203 08fd 0204 0afc 0205 06fb 0207  ................
-00002ad0: 0e02 04ff 0202 04fe 0203 08fd 0204 0afc  ................
-00002ae0: 0205 06fb 0207 0e01 0a01 1602 0801 1402  ................
-00002af0: 1201 1402 7a1b 426c 7565 4361 7374 2e74  ....z.BlueCast.t
-00002b00: 7261 6e73 666f 726d 5f6e 6577 5f64 6174  ransform_new_dat
-00002b10: 6163 0200 0000 0000 0000 0000 0000 0400  ac..............
-00002b20: 0000 0500 0000 4300 0000 7398 0000 007c  ......C...s....|
-00002b30: 006a 0073 0e74 0164 0183 0182 017c 006a  .j.s.t.d.....|.j
-00002b40: 0273 1c74 0164 0283 0182 017c 006a 0373  .s.t.d.....|.j.s
-00002b50: 2a74 0464 0383 0182 0174 0583 0001 007c  *t.d.....t.....|
-00002b60: 00a0 067c 01a1 017d 0174 0774 08a0 09a1  ...|...}.t.t....
-00002b70: 009b 0064 049d 0283 0101 007c 006a 00a0  ...d.......|.j..
-00002b80: 0a7c 01a1 015c 027d 027d 037c 006a 026a  .|...\.}.}.|.j.j
-00002b90: 0b72 907c 006a 0c7c 006a 026a 0b6b 0672  .r.|.j.|.j.j.k.r
-00002ba0: 907c 006a 0d72 907c 006a 0272 907c 006a  .|.j.r.|.j.r.|.j
-00002bb0: 0da0 0e74 0fa0 107c 03a1 01a1 017d 037c  ...t...|.....}.|
-00002bc0: 027c 0366 0253 0029 057a 9050 7265 6469  .|.f.S.).z.Predi
-00002bd0: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
-00002be0: 612e 0a0a 2020 2020 2020 2020 5265 7475  a...        Retu
-00002bf0: 726e 2074 6865 2070 7265 6469 6374 6564  rn the predicted
-00002c00: 2070 726f 6261 6269 6c69 7469 6573 2061   probabilities a
-00002c10: 6e64 2074 6865 2070 7265 6469 6374 6564  nd the predicted
-00002c20: 2063 6c61 7373 6573 3a0a 2020 2020 2020   classes:.      
-00002c30: 2020 795f 7072 6f62 732c 2079 5f63 6c61    y_probs, y_cla
-00002c40: 7373 6573 203d 2070 7265 6469 6374 2864  sses = predict(d
-00002c50: 6629 0a20 2020 2020 2020 207a 1b4d 6c20  f).        z.Ml 
-00002c60: 6d6f 6465 6c20 636f 756c 6420 6e6f 7420  model could not 
-00002c70: 6265 2066 6f75 6e64 7263 0000 007a 1563  be foundrc...z.c
-00002c80: 6f6e 665f 7472 6169 6e69 6e67 2069 7320  onf_training is 
-00002c90: 4e6f 6e65 7a0f 3a20 5072 6564 6963 7469  Nonez.: Predicti
-00002ca0: 6e67 2e2e 2e29 1172 2400 0000 7264 0000  ng...).r$...rd..
-00002cb0: 0072 2c00 0000 7228 0000 00da 0a56 616c  .r,...r(.....Val
-00002cc0: 7565 4572 726f 7272 0f00 0000 7266 0000  ueErrorr....rf..
-00002cd0: 0072 1000 0000 7202 0000 00da 0675 7463  .r....r......utc
-00002ce0: 6e6f 7772 5e00 0000 7221 0000 0072 2000  nowr^...r!...r .
-00002cf0: 0000 722e 0000 00da 1f6c 6162 656c 5f65  ..r......label_e
-00002d00: 6e63 6f64 6572 5f72 6576 6572 7365 5f74  ncoder_reverse_t
-00002d10: 7261 6e73 666f 726d da02 7064 da06 5365  ransform..pd..Se
-00002d20: 7269 6573 2904 7231 0000 0072 3500 0000  ries).r1...r5...
-00002d30: 7260 0000 0072 6100 0000 7232 0000 0072  r`...ra...r2...r
-00002d40: 3200 0000 7233 0000 0072 5e00 0000 5d01  2...r3...r^...].
-00002d50: 0000 732a 0000 0000 0606 0108 0206 0108  ..s*............
-00002d60: 0206 0108 0206 010a 0212 0110 0208 020c  ................
-00002d70: ff02 0204 fe02 0304 fd02 0506 0108 ff04  ................
-00002d80: 047a 1042 6c75 6543 6173 742e 7072 6564  .z.BlueCast.pred
-00002d90: 6963 7429 0a4e 4e4e 4e4e 4e4e 4e4e 4e29  ict).NNNNNNNNNN)
-00002da0: 1fda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00002db0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00002dc0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7206  ame__..__doc__r.
-00002dd0: 0000 0072 0900 0000 da03 7374 72da 0566  ...r......str..f
-00002de0: 6c6f 6174 da03 696e 7472 0700 0000 7205  loat..intr....r.
-00002df0: 0000 0072 1100 0000 7203 0000 0072 1200  ...r....r....r..
-00002e00: 0000 7215 0000 0072 0a00 0000 720c 0000  ..r....r....r...
-00002e10: 0072 0b00 0000 7234 0000 0072 6a00 0000  .r....r4...rj...
-00002e20: da09 4461 7461 4672 616d 6572 4400 0000  ..DataFramerD...
-00002e30: 7252 0000 0072 6b00 0000 7204 0000 0072  rR...rk...r....r
-00002e40: 6200 0000 7266 0000 0072 0800 0000 da02  b...rf...r......
-00002e50: 6e70 da07 6e64 6172 7261 7972 5e00 0000  np..ndarrayr^...
-00002e60: 7232 0000 0072 3200 0000 7232 0000 0072  r2...r2...r2...r
-00002e70: 3300 0000 721c 0000 0027 0000 0073 4a00  3...r....'...sJ.
-00002e80: 0000 0801 0418 0001 0001 0001 0001 0001  ................
-00002e90: 0003 0001 0001 0001 00f1 0202 0601 0c01  ................
-00002ea0: 1401 1401 0601 0e01 0601 0601 0201 0aff  ................
-00002eb0: 0203 0601 0601 06f1 0c26 1244 1472 0401  .........&.D.r..
-00002ec0: 0401 0401 0201 0afa 0c15 1432 721c 0000  ...........2r...
-00002ed0: 0029 3072 6f00 0000 723b 0000 0072 0200  .)0ro...r;...r..
-00002ee0: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
-00002ef0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00002f00: 0000 0072 0800 0000 7209 0000 00da 056e  ...r....r......n
-00002f10: 756d 7079 7274 0000 00da 0670 616e 6461  umpyrt.....panda
-00002f20: 7372 6a00 0000 5a1f 626c 7565 6361 7374  srj...Z.bluecast
-00002f30: 2e63 6f6e 6669 672e 7472 6169 6e69 6e67  .config.training
-00002f40: 5f63 6f6e 6669 6772 0a00 0000 720b 0000  _configr....r...
-00002f50: 0072 0c00 0000 5a20 626c 7565 6361 7374  .r....Z bluecast
-00002f60: 2e65 7661 6c75 6174 696f 6e2e 6576 616c  .evaluation.eval
-00002f70: 5f6d 6574 7269 6373 720d 0000 005a 1f62  _metricsr....Z.b
-00002f80: 6c75 6563 6173 742e 6576 616c 7561 7469  luecast.evaluati
-00002f90: 6f6e 2e73 6861 705f 7661 6c75 6573 720e  on.shap_valuesr.
-00002fa0: 0000 005a 2462 6c75 6563 6173 742e 6765  ...Z$bluecast.ge
-00002fb0: 6e65 7261 6c5f 7574 696c 732e 6765 6e65  neral_utils.gene
-00002fc0: 7261 6c5f 7574 696c 7372 0f00 0000 7210  ral_utilsr....r.
-00002fd0: 0000 005a 1d62 6c75 6563 6173 742e 6d6c  ...Z.bluecast.ml
-00002fe0: 5f6d 6f64 656c 6c69 6e67 2e78 6762 6f6f  _modelling.xgboo
-00002ff0: 7374 7211 0000 005a 1d62 6c75 6563 6173  str....Z.bluecas
-00003000: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
-00003010: 6375 7374 6f6d 7212 0000 005a 2862 6c75  customr....Z(blu
-00003020: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-00003030: 696e 672e 6461 7465 7469 6d65 5f66 6561  ing.datetime_fea
-00003040: 7475 7265 7372 1300 0000 5a2b 626c 7565  turesr....Z+blue
-00003050: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
-00003060: 6e67 2e65 6e63 6f64 655f 7461 7267 6574  ng.encode_target
-00003070: 5f6c 6162 656c 7372 1400 0000 5a28 626c  _labelsr....Z(bl
-00003080: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
-00003090: 7369 6e67 2e66 6561 7475 7265 5f73 656c  sing.feature_sel
-000030a0: 6563 7469 6f6e 7215 0000 005a 2462 6c75  ectionr....Z$blu
-000030b0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-000030c0: 696e 672e 6665 6174 7572 655f 7479 7065  ing.feature_type
-000030d0: 7372 1600 0000 5a25 626c 7565 6361 7374  sr....Z%bluecast
-000030e0: 2e70 7265 7072 6f63 6573 7369 6e67 2e6e  .preprocessing.n
-000030f0: 756c 6c73 5f61 6e64 5f69 6e66 7372 1700  ulls_and_infsr..
-00003100: 0000 5a24 626c 7565 6361 7374 2e70 7265  ..Z$bluecast.pre
-00003110: 7072 6f63 6573 7369 6e67 2e73 6368 656d  processing.schem
-00003120: 615f 6368 6563 6b73 7218 0000 005a 2662  a_checksr....Z&b
-00003130: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00003140: 7373 696e 672e 7461 7267 6574 5f65 6e63  ssing.target_enc
-00003150: 6f64 696e 6772 1900 0000 721a 0000 005a  odingr....r....Z
-00003160: 2762 6c75 6563 6173 742e 7072 6570 726f  'bluecast.prepro
-00003170: 6365 7373 696e 672e 7472 6169 6e5f 7465  cessing.train_te
-00003180: 7374 5f73 706c 6974 721b 0000 0072 1c00  st_splitr....r..
-00003190: 0000 7232 0000 0072 3200 0000 7232 0000  ..r2...r2...r2..
-000031a0: 0072 3300 0000 da08 3c6d 6f64 756c 653e  .r3.....<module>
-000031b0: 0100 0000 7328 0000 0004 0808 010c 0124  ....s(.........$
-000031c0: 0208 0108 0214 050c 010c 0110 010c 010c  ................
-000031d0: 010c 010c 010c 010c 010c 010c 0110 040c  ................
-000031e0: 03                                       .
+000008a0: 6d61 7469 6361 6c6c 792e 0a20 2020 203a  matically..    :
+000008b0: 7061 7261 6d20 3a64 6174 655f 636f 6c75  param :date_colu
+000008c0: 6d6e 733a 2054 616b 6573 2061 206c 6973  mns: Takes a lis
+000008d0: 7420 6f66 2073 7472 696e 6773 2063 6f6e  t of strings con
+000008e0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
+000008f0: 7320 6f66 2074 6865 2064 6174 6520 636f  s of the date co
+00000900: 6c75 6d6e 732e 2049 6620 6e6f 7420 7072  lumns. If not pr
+00000910: 6f76 6964 6564 2c0a 2020 2020 426c 7565  ovided,.    Blue
+00000920: 4361 7374 2077 696c 6c20 696e 6665 7220  Cast will infer 
+00000930: 7468 6573 6520 6175 746f 6d61 7469 6361  these automatica
+00000940: 6c6c 792e 0a20 2020 203a 7061 7261 6d20  lly..    :param 
+00000950: 3a74 696d 655f 7370 6c69 745f 636f 6c75  :time_split_colu
+00000960: 6d6e 3a20 5461 6b65 7320 6120 7374 7269  mn: Takes a stri
+00000970: 6e67 2063 6f6e 7461 696e 696e 6720 7468  ng containing th
+00000980: 6520 6e61 6d65 206f 6620 7468 6520 7469  e name of the ti
+00000990: 6d65 2073 706c 6974 2063 6f6c 756d 6e2e  me split column.
+000009a0: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+000009b0: 2c0a 2020 2020 426c 7565 4361 7374 2077  ,.    BlueCast w
+000009c0: 696c 6c20 6e6f 7420 7370 6c69 7420 7468  ill not split th
+000009d0: 6520 6461 7461 2062 7920 7469 6d65 206f  e data by time o
+000009e0: 7220 6f72 6465 722c 2062 7574 2064 6f20  r order, but do 
+000009f0: 6120 7261 6e64 6f6d 2073 706c 6974 2069  a random split i
+00000a00: 6e73 7465 6164 2e0a 2020 2020 3a70 6172  nstead..    :par
+00000a10: 616d 203a 6d6c 5f6d 6f64 656c 3a20 5461  am :ml_model: Ta
+00000a20: 6b65 7320 616e 2069 6e73 7461 6e63 6520  kes an instance 
+00000a30: 6f66 2061 2058 6762 6f6f 7374 4d6f 6465  of a XgboostMode
+00000a40: 6c20 636c 6173 732e 2049 6620 6e6f 7420  l class. If not 
+00000a50: 7072 6f76 6964 6564 2c20 426c 7565 4361  provided, BlueCa
+00000a60: 7374 2077 696c 6c20 696e 7374 616e 7469  st will instanti
+00000a70: 6174 6520 6f6e 652e 0a20 2020 2054 6869  ate one..    Thi
+00000a80: 7320 6973 2061 6e20 4150 4920 746f 2070  s is an API to p
+00000a90: 6173 7320 616e 7920 6d6f 6465 6c20 636c  ass any model cl
+00000aa0: 6173 732e 2049 6e68 6572 6974 2074 6865  ass. Inherit the
+00000ab0: 2062 6173 6563 6c61 7373 2066 726f 6d20   baseclass from 
+00000ac0: 6d6c 5f6d 6f64 656c 6c69 6e67 2e62 6173  ml_modelling.bas
+00000ad0: 655f 6d6f 6465 6c2e 4261 7365 4d6f 6465  e_model.BaseMode
+00000ae0: 6c2e 0a20 2020 203a 7061 7261 6d20 6375  l..    :param cu
+00000af0: 7374 6f6d 5f70 7265 7072 6f63 6573 736f  stom_preprocesso
+00000b00: 723a 2054 616b 6573 2061 6e20 696e 7374  r: Takes an inst
+00000b10: 616e 6365 206f 6620 6120 4375 7374 6f6d  ance of a Custom
+00000b20: 5072 6570 726f 6365 7373 696e 6720 636c  Preprocessing cl
+00000b30: 6173 732e 2041 6c6c 6f77 7320 7573 6572  ass. Allows user
+00000b40: 7320 746f 2069 6e6a 6563 7420 6375 7374  s to inject cust
+00000b50: 6f6d 0a20 2020 2070 7265 7072 6f63 6573  om.    preproces
+00000b60: 7369 6e67 2073 7465 7073 2077 6869 6368  sing steps which
+00000b70: 2074 616b 6520 706c 6163 6520 7269 6768   take place righ
+00000b80: 7420 6166 7465 7220 7468 6520 7472 6169  t after the trai
+00000b90: 6e20 7465 7374 2073 7069 742e 0a20 2020  n test spit..   
+00000ba0: 203a 7061 7261 6d20 6375 7374 6f6d 5f6c   :param custom_l
+00000bb0: 6173 745f 6d69 6c65 5f63 6f6d 7075 7461  ast_mile_computa
+00000bc0: 7469 6f6e 3a20 5461 6b65 7320 616e 2069  tion: Takes an i
+00000bd0: 6e73 7461 6e63 6520 6f66 2061 2043 7573  nstance of a Cus
+00000be0: 746f 6d50 7265 7072 6f63 6573 7369 6e67  tomPreprocessing
+00000bf0: 2063 6c61 7373 2e20 416c 6c6f 7773 2075   class. Allows u
+00000c00: 7365 7273 2074 6f20 696e 6a65 6374 2063  sers to inject c
+00000c10: 7573 746f 6d0a 2020 2020 7072 6570 726f  ustom.    prepro
+00000c20: 6365 7373 696e 6720 7374 6570 7320 7768  cessing steps wh
+00000c30: 6963 6820 7461 6b65 2070 6c61 6365 2072  ich take place r
+00000c40: 6967 6874 2062 6566 6f72 6520 7468 6520  ight before the 
+00000c50: 6d6f 6465 6c20 7472 6169 6e69 6e67 2e0a  model training..
+00000c60: 2020 2020 4e29 02da 0662 696e 6172 79da      N)...binary.
+00000c70: 0a6d 756c 7469 636c 6173 7329 0cda 0d63  .multiclass)...c
+00000c80: 6c61 7373 5f70 726f 626c 656d da0d 7461  lass_problem..ta
+00000c90: 7267 6574 5f63 6f6c 756d 6eda 0b63 6174  rget_column..cat
+00000ca0: 5f63 6f6c 756d 6e73 da0c 6461 7465 5f63  _columns..date_c
+00000cb0: 6f6c 756d 6e73 da11 7469 6d65 5f73 706c  olumns..time_spl
+00000cc0: 6974 5f63 6f6c 756d 6eda 086d 6c5f 6d6f  it_column..ml_mo
+00000cd0: 6465 6cda 1c63 7573 746f 6d5f 6c61 7374  del..custom_last
+00000ce0: 5f6d 696c 655f 636f 6d70 7574 6174 696f  _mile_computatio
+00000cf0: 6eda 1363 7573 746f 6d5f 7072 6570 726f  n..custom_prepro
+00000d00: 6365 7373 6f72 da17 6375 7374 6f6d 5f66  cessor..custom_f
+00000d10: 6561 7475 7265 5f73 656c 6563 746f 72da  eature_selector.
+00000d20: 0d63 6f6e 665f 7472 6169 6e69 6e67 da0c  .conf_training..
+00000d30: 636f 6e66 5f78 6762 6f6f 7374 da13 636f  conf_xgboost..co
+00000d40: 6e66 5f70 6172 616d 735f 7867 626f 6f73  nf_params_xgboos
+00000d50: 7463 0d00 0000 0000 0000 0000 0000 0d00  tc..............
+00000d60: 0000 0200 0000 4300 0000 7370 0000 007c  ......C...sp...|
+00000d70: 017c 005f 0064 017c 005f 017c 037c 005f  .|._.d.|._.|.|._
+00000d80: 027c 047c 005f 037c 057c 005f 047c 027c  .|.|._.|.|._.|.|
+00000d90: 005f 057c 0a7c 005f 067c 0b7c 005f 077c  ._.|.|._.|.|._.|
+00000da0: 0c7c 005f 0864 007c 005f 0964 007c 005f  .|._.d.|._.d.|._
+00000db0: 0a64 007c 005f 0b64 007c 005f 0c7c 067c  .d.|._.d.|._.|.|
+00000dc0: 005f 0d7c 077c 005f 0e7c 087c 005f 0f7c  ._.|.|._.|.|._.|
+00000dd0: 097c 005f 1064 007c 005f 1164 0053 0029  .|._.d.|._.d.S.)
+00000de0: 024e 4629 1272 1f00 0000 da0f 7072 6564  .NF).r......pred
+00000df0: 6963 7469 6f6e 5f6d 6f64 6572 2100 0000  iction_moder!...
+00000e00: 7222 0000 0072 2300 0000 7220 0000 0072  r"...r#...r ...r
+00000e10: 2800 0000 7229 0000 0072 2a00 0000 da12  (...r)...r*.....
+00000e20: 6665 6174 5f74 7970 655f 6465 7465 6374  feat_type_detect
+00000e30: 6f72 da0b 6361 745f 656e 636f 6465 72da  or..cat_encoder.
+00000e40: 1474 6172 6765 745f 6c61 6265 6c5f 656e  .target_label_en
+00000e50: 636f 6465 72da 0f73 6368 656d 615f 6465  coder..schema_de
+00000e60: 7465 6374 6f72 7224 0000 0072 2500 0000  tectorr$...r%...
+00000e70: 7226 0000 0072 2700 0000 da0b 7368 6170  r&...r'.....shap
+00000e80: 5f76 616c 7565 7329 0dda 0473 656c 6672  _values)...selfr
+00000e90: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
+00000ea0: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00000eb0: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00000ec0: 0072 2900 0000 722a 0000 00a9 0072 3200  .r)...r*.....r2.
+00000ed0: 0000 fa3e 2f68 6f6d 652f 7468 6f6d 6173  ...>/home/thomas
+00000ee0: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
+00000ef0: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
+00000f00: 626c 7565 7072 696e 7473 2f63 6173 742e  blueprints/cast.
+00000f10: 7079 da08 5f5f 696e 6974 5f5f 3c00 0000  py..__init__<...
+00000f20: 7326 0000 0000 1106 0106 0106 0106 0106  s&..............
+00000f30: 0106 0106 0106 0106 0106 0302 fe04 0306  ................
+00000f40: 0106 0106 0106 0106 0106 017a 1142 6c75  ...........z.Blu
+00000f50: 6543 6173 742e 5f5f 696e 6974 5f5f 2902  eCast.__init__).
+00000f60: da02 6466 da06 7265 7475 726e 6302 0000  ..df..returnc...
+00000f70: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000f80: 0043 0000 0073 3001 0000 7c00 6a00 730e  .C...s0...|.j.s.
+00000f90: 7401 8300 7c00 5f00 7c00 6a00 6a02 732a  t...|._.|.j.j.s*
+00000fa0: 6401 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+00000fb0: 8d03 0100 7c00 6a00 6a06 6404 6b02 724a  ....|.j.j.d.k.rJ
+00000fc0: 6405 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+00000fd0: 8d03 0100 7c00 6a00 6a02 726c 7c00 6a07  ....|.j.j.rl|.j.
+00000fe0: 736c 6406 7d02 7403 6a04 7c02 7405 6402  sld.}.t.j.|.t.d.
+00000ff0: 6403 8d03 0100 7c00 6a08 7386 6407 7d02  d.....|.j.s.d.}.
+00001000: 7403 6a04 7c02 7405 6402 6403 8d03 0100  t.j.|.t.d.d.....
+00001010: 7c00 6a00 6a09 740a 7c01 6a0b 8301 6b05  |.j.j.t.|.j...k.
+00001020: 72b4 7c00 6a00 6a02 72b4 6408 7d02 7403  r.|.j.j.r.d.}.t.
+00001030: 6a04 7c02 7405 6402 6403 8d03 0100 7c00  j.|.t.d.d.....|.
+00001040: 6a00 6a0c 72e0 7c00 6a00 6a0d 72e0 6409  j.j.r.|.j.j.r.d.
+00001050: 7c00 6a00 5f0d 640a 7d02 7403 6a04 7c02  |.j._.d.}.t.j.|.
+00001060: 7405 6402 6403 8d03 0100 7c00 6a00 6a0c  t.d.d.....|.j.j.
+00001070: 9001 7206 7c00 6a0e 9001 7206 640b 7d02  ..r.|.j...r.d.}.
+00001080: 7403 6a04 7c02 7405 6402 6403 8d03 0100  t.j.|.t.d.d.....
+00001090: 7c00 6a00 6a0c 9001 722c 7c00 6a0f 9001  |.j.j...r,|.j...
+000010a0: 722c 640c 7d02 7403 6a04 7c02 7405 6402  r,d.}.t.j.|.t.d.
+000010b0: 6403 8d03 0100 6400 5300 290d 4e61 9301  d.....d.S.).Na..
+000010c0: 0000 4665 6174 7572 6520 7365 6c65 6374  ..Feature select
+000010d0: 696f 6e20 6973 2064 6973 6162 6c65 642e  ion is disabled.
+000010e0: 2055 7064 6174 6520 7468 6520 5472 6169   Update the Trai
+000010f0: 6e69 6e67 436f 6e66 6967 2070 6172 616d  ningConfig param
+00001100: 2027 656e 6162 6c65 5f66 6561 7475 7265   'enable_feature
+00001110: 5f73 656c 6563 7469 6f6e 270a 2020 2020  _selection'.    
+00001120: 2020 2020 2020 2020 746f 2065 6e61 626c          to enabl
+00001130: 6520 6974 206f 7220 6d61 6b65 2075 7365  e it or make use
+00001140: 206f 6620 6120 6375 7374 6f6d 2070 7265   of a custom pre
+00001150: 7072 6f63 6573 736f 7220 746f 2064 6f20  processor to do 
+00001160: 6974 206d 616e 7561 6c6c 7920 6475 7269  it manually duri
+00001170: 6e67 2074 6865 206c 6173 7420 6d69 6c65  ng the last mile
+00001180: 2063 6f6d 7075 7461 7469 6f6e 7320 7374   computations st
+00001190: 6570 2e0a 2020 2020 2020 2020 2020 2020  ep..            
+000011a0: 4665 6174 7572 6520 7365 6c65 6374 696f  Feature selectio
+000011b0: 6e20 6973 2072 6563 6f6d 6d65 6e64 6564  n is recommended
+000011c0: 2066 6f72 2064 6174 6173 6574 7320 7769   for datasets wi
+000011d0: 7468 206d 616e 7920 6665 6174 7572 6573  th many features
+000011e0: 2028 3e31 3030 3029 2e20 466f 7220 6461   (>1000). For da
+000011f0: 7461 7365 7473 2077 6974 6820 6120 736d  tasets with a sm
+00001200: 616c 6c20 616d 6f75 6e74 0a20 2020 2020  all amount.     
+00001210: 2020 2020 2020 206f 6620 6665 6174 7572         of featur
+00001220: 6573 2066 6561 7475 7265 2073 656c 6563  es feature selec
+00001230: 7469 6f6e 2069 7320 6e6f 7420 7265 636f  tion is not reco
+00001240: 6d6d 656e 6465 642e 0a20 2020 2020 2020  mmended..       
+00001250: 2020 2020 20e9 0200 0000 2901 da0a 7374       .....)...st
+00001260: 6163 6b6c 6576 656c e901 0000 0061 0501  acklevel.....a..
+00001270: 0000 4372 6f73 7320 7661 6c69 6461 7469  ..Cross validati
+00001280: 6f6e 2069 7320 6469 7361 626c 6564 2e20  on is disabled. 
+00001290: 5570 6461 7465 2074 6865 2054 7261 696e  Update the Train
+000012a0: 696e 6743 6f6e 6669 6720 7061 7261 6d20  ingConfig param 
+000012b0: 2768 7970 6572 7475 6e69 6e67 5f63 765f  'hypertuning_cv_
+000012c0: 666f 6c64 7327 0a20 2020 2020 2020 2020  folds'.         
+000012d0: 2020 2074 6f20 656e 6162 6c65 2069 742e     to enable it.
+000012e0: 2043 726f 7373 2076 616c 6964 6174 696f   Cross validatio
+000012f0: 6e20 6973 2064 6973 6162 6c65 6420 6f6e  n is disabled on
+00001300: 2064 6566 6175 6c74 2074 6f20 616c 6c6f   default to allo
+00001310: 7720 6661 7374 2070 726f 746f 7479 7069  w fast prototypi
+00001320: 6e67 2e20 466f 7220 726f 6275 7374 2068  ng. For robust h
+00001330: 7970 6572 7061 7261 6d65 7465 720a 2020  yperparameter.  
+00001340: 2020 2020 2020 2020 2020 7475 6e69 6e67            tuning
+00001350: 2075 7369 6e67 2061 7420 6c65 6173 7420   using at least 
+00001360: 3520 666f 6c64 7320 6973 2072 6563 6f6d  5 folds is recom
+00001370: 6d65 6e64 6564 2e61 5f01 0000 4665 6174  mended.a_...Feat
+00001380: 7572 6520 7365 6c65 6374 696f 6e20 6973  ure selection is
+00001390: 2065 6e61 626c 6564 2062 7574 206e 6f20   enabled but no 
+000013a0: 6665 6174 7572 6520 7365 6c65 6374 6f72  feature selector
+000013b0: 2068 6173 2062 6565 6e20 7072 6f76 6964   has been provid
+000013c0: 6564 2e20 4661 6c6c 696e 6720 6261 636b  ed. Falling back
+000013d0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+000013e0: 6372 6f73 732d 7661 6c69 6461 7465 6420  cross-validated 
+000013f0: 6665 6174 7572 6520 656c 696d 696e 6174  feature eliminat
+00001400: 696f 6e2e 2053 7065 6369 6669 6361 6c6c  ion. Specificall
+00001410: 7920 666f 7220 736d 616c 6c20 6461 7461  y for small data
+00001420: 7365 7473 2063 6865 636b 2074 6865 206c  sets check the l
+00001430: 6f67 7320 746f 2076 6572 6966 7920 7468  ogs to verify th
+00001440: 6174 206e 6f74 2074 6f6f 0a20 2020 2020  at not too.     
+00001450: 2020 2020 2020 206d 616e 7920 6665 6174         many feat
+00001460: 7572 6573 2068 6176 6520 6265 656e 2072  ures have been r
+00001470: 656d 6f76 6564 2e20 4f74 6865 7277 6973  emoved. Otherwis
+00001480: 652c 2063 6f6e 7369 6465 7220 6469 7361  e, consider disa
+00001490: 626c 696e 6720 6665 6174 7572 6520 7365  bling feature se
+000014a0: 6c65 6374 696f 6e20 6f72 2070 726f 7669  lection or provi
+000014b0: 6469 6e67 2061 2063 7573 746f 6d0a 2020  ding a custom.  
+000014c0: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+000014d0: 6520 7365 6c65 6374 6f72 2e61 6501 0000  e selector.ae...
+000014e0: 4e6f 2058 6762 6f6f 7374 5475 6e65 5061  No XgboostTunePa
+000014f0: 7261 6d73 436f 6e66 6967 2068 6173 2062  ramsConfig has b
+00001500: 6565 6e20 7072 6f76 6964 6564 2e20 4661  een provided. Fa
+00001510: 6c6c 696e 6720 6261 636b 2074 6f20 6465  lling back to de
+00001520: 6661 756c 7420 7661 6c75 6573 2e20 4465  fault values. De
+00001530: 6661 756c 7420 7661 6c75 6573 0a20 2020  fault values.   
+00001540: 2020 2020 2020 2020 2068 6176 6520 6265           have be
+00001550: 656e 2063 686f 7365 6e20 746f 2073 7065  en chosen to spe
+00001560: 6564 2075 7020 7468 6520 7072 6f74 6f74  ed up the protot
+00001570: 7970 696e 672e 2046 6f72 2072 6f62 7573  yping. For robus
+00001580: 7420 6879 7065 7270 6172 616d 6574 6572  t hyperparameter
+00001590: 2074 756e 696e 6720 636f 6e73 6964 6572   tuning consider
+000015a0: 2070 726f 7669 6469 6e67 2061 2063 7573   providing a cus
+000015b0: 746f 6d0a 2020 2020 2020 2020 2020 2020  tom.            
+000015c0: 5867 626f 6f73 7454 756e 6550 6172 616d  XgboostTuneParam
+000015d0: 7343 6f6e 6669 6720 7769 7468 2061 2064  sConfig with a d
+000015e0: 6565 7065 7220 6879 7065 7270 6172 616d  eeper hyperparam
+000015f0: 6574 6572 2073 6561 7263 6820 7370 6163  eter search spac
+00001600: 6520 616e 6420 6120 6375 7374 6f6d 2054  e and a custom T
+00001610: 7261 696e 696e 6743 6f6e 6669 6720 746f  rainingConfig to
+00001620: 2065 6e61 626c 650a 2020 2020 2020 2020   enable.        
+00001630: 2020 2020 6372 6f73 732d 7661 6c69 6461      cross-valida
+00001640: 7469 6f6e 2e61 0f01 0000 5468 6520 6d69  tion.a....The mi
+00001650: 6e69 6d75 6d20 6e75 6d62 6572 206f 6620  nimum number of 
+00001660: 6665 6174 7572 6573 2074 6f20 7365 6c65  features to sele
+00001670: 6374 2069 7320 6772 6561 7465 7220 6f72  ct is greater or
+00001680: 2065 7175 616c 2074 6f20 7468 6520 6e75   equal to the nu
+00001690: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+000016a0: 2069 6e0a 2020 2020 2020 2020 2020 2020   in.            
+000016b0: 7468 6520 6461 7461 7365 7420 7768 696c  the dataset whil
+000016c0: 6520 6665 6174 7572 6520 7365 6c65 6374  e feature select
+000016d0: 696f 6e20 6973 2065 6e61 626c 6564 2e20  ion is enabled. 
+000016e0: 436f 6e73 6964 6572 2072 6564 7563 696e  Consider reducin
+000016f0: 6720 7468 6520 6d69 6e69 6d75 6d20 6e75  g the minimum nu
+00001700: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+00001710: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00001720: 7365 6c65 6374 206f 7220 6469 7361 626c  select or disabl
+00001730: 696e 6720 6665 6174 7572 6520 7365 6c65  ing feature sele
+00001740: 6374 696f 6e20 7669 6120 5472 6169 6e69  ction via Traini
+00001750: 6e67 436f 6e66 6967 2e46 612b 0200 0053  ngConfig.Fa+...S
+00001760: 4841 5020 7661 6c75 6573 2063 616e 6e6f  HAP values canno
+00001770: 7420 6265 2063 616c 6375 6c61 7465 6420  t be calculated 
+00001780: 7768 656e 2063 6174 6567 6f72 6963 616c  when categorical
+00001790: 2065 6e63 6f64 696e 6720 7669 6120 4d4c   encoding via ML
+000017a0: 2061 6c67 6f72 6974 686d 2069 7320 656e   algorithm is en
+000017b0: 6162 6c65 6420 6475 6520 746f 0a20 2020  abled due to.   
+000017c0: 2020 2020 2020 2020 2069 6e63 6f6d 7061           incompa
+000017d0: 7469 6269 6c69 7479 2077 6974 6820 7468  tibility with th
+000017e0: 6520 7368 6170 206c 6962 7261 7279 2e20  e shap library. 
+000017f0: 5365 6520 7468 6973 2047 6974 4875 6220  See this GitHub 
+00001800: 6973 7375 6520 666f 7220 6d6f 7265 2063  issue for more c
+00001810: 6f6e 7465 7874 3a0a 2020 2020 2020 2020  ontext:.        
+00001820: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
+00001830: 7562 2e63 6f6d 2f73 6c75 6e64 6265 7267  ub.com/slundberg
+00001840: 2f73 6861 702f 6973 7375 6573 2f32 3636  /shap/issues/266
+00001850: 0a0a 2020 2020 2020 2020 2020 2020 4361  ..            Ca
+00001860: 6c63 756c 6174 696f 6e20 6f66 2053 6861  lculation of Sha
+00001870: 7020 7661 6c75 6573 2068 6173 2062 6565  p values has bee
+00001880: 6e20 6368 616e 6765 6420 746f 2066 616c  n changed to fal
+00001890: 7365 2e0a 2020 2020 2020 2020 2020 2020  se..            
+000018a0: 436f 6e73 6964 6572 2064 6973 6162 6c69  Consider disabli
+000018b0: 6e67 2063 6174 6567 6f72 6963 616c 2065  ng categorical e
+000018c0: 6e63 6f64 696e 6720 7669 6120 4d4c 2061  ncoding via ML a
+000018d0: 6c67 6f72 6974 686d 2069 6e20 7468 6520  lgorithm in the 
+000018e0: 5472 6169 6e69 6e67 436f 6e66 6967 2069  TrainingConfig i
+000018f0: 6620 7368 6170 2076 616c 7565 7320 6172  f shap values ar
+00001900: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+00001910: 7175 6972 6564 2e20 416c 7465 726e 6174  quired. Alternat
+00001920: 6976 656c 7920 7573 6520 5867 626f 6f73  ively use Xgboos
+00001930: 7420 6173 2061 2063 7573 746f 6d20 6d6f  t as a custom mo
+00001940: 6465 6c20 616e 6420 6361 6c63 756c 6174  del and calculat
+00001950: 6520 7368 6170 2076 616c 7565 7320 6d61  e shap values ma
+00001960: 6e75 616c 6c79 2076 6961 0a20 2020 2020  nually via.     
+00001970: 2020 2020 2020 2070 7265 645f 636f 6e74         pred_cont
+00001980: 7269 6273 3d54 7275 652e 7af0 4361 7465  ribs=True.z.Cate
+00001990: 676f 7269 6361 6c20 656e 636f 6469 6e67  gorical encoding
+000019a0: 2076 6961 204d 4c20 616c 676f 7269 7468   via ML algorith
+000019b0: 6d20 6973 2065 6e61 626c 6564 2e20 4d61  m is enabled. Ma
+000019c0: 6b65 2073 7572 6520 746f 2068 616e 646c  ke sure to handl
+000019d0: 6520 6361 7465 676f 7269 6361 6c20 6665  e categorical fe
+000019e0: 6174 7572 6573 0a20 2020 2020 2020 2020  atures.         
+000019f0: 2020 2077 6974 6869 6e20 7468 6520 7072     within the pr
+00001a00: 6f76 6964 6564 206d 6c20 6d6f 6465 6c20  ovided ml model 
+00001a10: 6f72 2063 6f6e 7369 6465 7220 6469 7361  or consider disa
+00001a20: 626c 696e 6720 6361 7465 676f 7269 6361  bling categorica
+00001a30: 6c20 656e 636f 6469 6e67 2076 6961 204d  l encoding via M
+00001a40: 4c20 616c 676f 7269 7468 6d20 696e 2074  L algorithm in t
+00001a50: 6865 0a20 2020 2020 2020 2020 2020 2054  he.            T
+00001a60: 7261 696e 696e 6743 6f6e 6669 6720 616c  rainingConfig al
+00001a70: 7465 726e 6174 6976 656c 792e 7afd 4361  ternatively.z.Ca
+00001a80: 7465 676f 7269 6361 6c20 656e 636f 6469  tegorical encodi
+00001a90: 6e67 2076 6961 204d 4c20 616c 676f 7269  ng via ML algori
+00001aa0: 7468 6d20 6973 2065 6e61 626c 6564 2e20  thm is enabled. 
+00001ab0: 4d61 6b65 2073 7572 6520 746f 2068 616e  Make sure to han
+00001ac0: 646c 6520 6361 7465 676f 7269 6361 6c20  dle categorical 
+00001ad0: 6665 6174 7572 6573 0a20 2020 2020 2020  features.       
+00001ae0: 2020 2020 2077 6974 6869 6e20 7468 6520       within the 
+00001af0: 7072 6f76 6964 6564 206c 6173 7420 6d69  provided last mi
+00001b00: 6c65 2063 6f6d 7075 7461 7469 6f6e 206f  le computation o
+00001b10: 7220 636f 6e73 6964 6572 2064 6973 6162  r consider disab
+00001b20: 6c69 6e67 2063 6174 6567 6f72 6963 616c  ling categorical
+00001b30: 2065 6e63 6f64 696e 6720 7669 6120 4d4c   encoding via ML
+00001b40: 2061 6c67 6f72 6974 686d 2069 6e20 7468   algorithm in th
+00001b50: 650a 2020 2020 2020 2020 2020 2020 5472  e.            Tr
+00001b60: 6169 6e69 6e67 436f 6e66 6967 2061 6c74  ainingConfig alt
+00001b70: 6572 6e61 7469 7665 6c79 2e29 1072 2800  ernatively.).r(.
+00001b80: 0000 720a 0000 00da 1865 6e61 626c 655f  ..r......enable_
+00001b90: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
+00001ba0: 6eda 0877 6172 6e69 6e67 73da 0477 6172  n..warnings..war
+00001bb0: 6eda 0b55 7365 7257 6172 6e69 6e67 5a14  n..UserWarningZ.
+00001bc0: 6879 7065 7274 756e 696e 675f 6376 5f66  hypertuning_cv_f
+00001bd0: 6f6c 6473 7227 0000 0072 2900 0000 da16  oldsr'...r).....
+00001be0: 6d69 6e5f 6665 6174 7572 6573 5f74 6f5f  min_features_to_
+00001bf0: 7365 6c65 6374 da03 6c65 6eda 0763 6f6c  select..len..col
+00001c00: 756d 6e73 da1d 6361 745f 656e 636f 6469  umns..cat_encodi
+00001c10: 6e67 5f76 6961 5f6d 6c5f 616c 676f 7269  ng_via_ml_algori
+00001c20: 7468 6dda 1563 616c 6375 6c61 7465 5f73  thm..calculate_s
+00001c30: 6861 705f 7661 6c75 6573 7224 0000 0072  hap_valuesr$...r
+00001c40: 2500 0000 2903 7231 0000 0072 3500 0000  %...).r1...r5...
+00001c50: da07 6d65 7373 6167 6572 3200 0000 7232  ..messager2...r2
+00001c60: 0000 0072 3300 0000 da0e 696e 6974 6961  ...r3.....initia
+00001c70: 6c5f 6368 6563 6b73 6200 0000 734e 0000  l_checksb...sN..
+00001c80: 0000 0106 0108 0108 0104 0510 020c 0104  ................
+00001c90: 0310 0306 ff02 0204 fe02 0404 0410 0106  ................
+00001ca0: 0104 0410 0210 ff02 0206 fe02 0404 0310  ................
+00001cb0: 0206 ff02 0206 fe02 0408 0104 0810 0112  ................
+00001cc0: 0104 0310 0206 ff04 0204 fe04 0404 037a  ...............z
+00001cd0: 1742 6c75 6543 6173 742e 696e 6974 6961  .BlueCast.initia
+00001ce0: 6c5f 6368 6563 6b73 2903 7235 0000 00da  l_checks).r5....
+00001cf0: 0a74 6172 6765 745f 636f 6c72 3600 0000  .target_colr6...
+00001d00: 6303 0000 0000 0000 0000 0000 0009 0000  c...............
+00001d10: 0007 0000 0043 0000 0073 2803 0000 7400  .....C...s(...t.
+00001d20: 8300 0100 7401 8300 7d03 7c03 a002 7c01  ....t...}.|...|.
+00001d30: a101 7d01 7c03 7c00 5f03 7c00 6a03 6a04  ..}.|.|._.|.j.j.
+00001d40: 7252 7c00 6a05 7c00 6a03 6a04 6b06 7252  rR|.j.|.j.j.k.rR
+00001d50: 7406 8300 7c00 5f07 7c00 6a07 a008 7c01  t...|._.|.j...|.
+00001d60: 7c00 6a05 1900 a101 7c01 7c00 6a05 3c00  |.j.....|.|.j.<.
+00001d70: 7c00 6a03 6a04 7c00 5f04 7c00 6a03 6a09  |.j.j.|._.|.j.j.
+00001d80: 7c00 5f09 7c00 6a0a 7374 740b 8300 7c00  |._.|.j.stt...|.
+00001d90: 5f0a 7c00 a00c 7c01 a101 0100 740d 7c01  _.|...|.....t.|.
+00001da0: 7c02 7c00 6a0e 7c00 6a0a 6a0f 7c00 6a0a  |.|.j.|.j.j.|.j.
+00001db0: 6a10 7c00 6a0a 6a11 8306 5c04 7d04 7d05  j.|.j.j...\.}.}.
+00001dc0: 7d06 7d07 7c00 6a12 9001 7232 7c00 6a12  }.}.|.j...r2|.j.
+00001dd0: a013 7c04 7c06 a102 5c02 7d04 7d06 7c00  ..|.|...\.}.}.|.
+00001de0: 6a12 6a14 7c05 7c07 6401 6402 8d03 5c02  j.j.|.|.d.d...\.
+00001df0: 7d05 7d07 7401 8300 7d03 7c03 a002 7c04  }.}.t...}.|...|.
+00001e00: a101 7d08 7c04 6a15 6403 6404 8d01 7c06  ..}.|.j.d.d...|.
+00001e10: 6a15 6403 6404 8d01 0200 7d04 7d06 7c05  j.d.d.....}.}.|.
+00001e20: 6a15 6403 6404 8d01 7c07 6a15 6403 6404  j.d.d...|.j.d.d.
+00001e30: 8d01 0200 7d05 7d07 7c02 7c03 6a04 6b06  ....}.}.|.|.j.k.
+00001e40: 9001 7232 7c03 6a04 a016 7c02 a101 0100  ..r2|.j...|.....
+00001e50: 7417 7c04 8301 7417 7c05 8301 0200 7d04  t.|...t.|.....}.
+00001e60: 7d05 7418 7c04 7c00 6a09 8302 7418 7c05  }.t.|.|.j...t.|.
+00001e70: 7c00 6a09 8302 0200 7d04 7d05 7419 8300  |.j.....}.}.t...
+00001e80: 7c00 5f1a 7c00 6a1a a01b 7c04 a101 0100  |._.|.j...|.....
+00001e90: 7c00 6a1a a014 7c05 a101 7d05 7c00 6a04  |.j...|...}.|.j.
+00001ea0: 6405 6b09 9001 72c8 7c00 6a1c 6406 6b02  d.k...r.|.j.d.k.
+00001eb0: 9001 72c8 7c00 6a0a 6a1d 9001 73c8 741e  ..r.|.j.j...s.t.
+00001ec0: 7c03 6a04 8301 7c00 5f1f 7c00 6a1f a020  |.j...|._.|.j.. 
+00001ed0: 7c04 7c06 a102 7d04 7c00 6a1f a021 7c05  |.|...}.|.j..!|.
+00001ee0: a101 7d05 6e80 7c00 6a04 6405 6b09 9002  ..}.n.|.j.d.k...
+00001ef0: 7212 7c00 6a1c 6407 6b02 9002 7212 7c00  r.|.j.d.k...r.|.
+00001f00: 6a0a 6a1d 9002 7312 7422 7c03 6a04 8301  j.j...s.t"|.j...
+00001f10: 7c00 5f1f 7c00 6a1f a023 7c04 7c06 a102  |._.|.j..#|.|...
+00001f20: 7d04 7c00 6a1f a024 7c05 a101 7d05 6e36  }.|.j..$|...}.n6
+00001f30: 7c00 6a0a 6a1d 9002 7248 7c04 7c00 6a04  |.j.j...rH|.|.j.
+00001f40: 1900 a025 6408 a101 7c04 7c00 6a04 3c00  ...%d...|.|.j.<.
+00001f50: 7c05 7c00 6a04 1900 a025 6408 a101 7c05  |.|.j....%d...|.
+00001f60: 7c00 6a04 3c00 7c00 6a26 9002 7278 7c00  |.j.<.|.j&..rx|.
+00001f70: 6a26 a013 7c04 7c06 a102 5c02 7d04 7d06  j&..|.|...\.}.}.
+00001f80: 7c00 6a26 6a14 7c05 7c07 6401 6402 8d03  |.j&j.|.|.d.d...
+00001f90: 5c02 7d05 7d07 7c00 6a27 9002 7396 7428  \.}.}.|.j'..s.t(
+00001fa0: 7c00 6a0a 6a10 7c00 6a0a 6a29 6409 8d02  |.j.j.|.j.j)d...
+00001fb0: 7c00 5f27 7c00 6a0a 6a2a 9002 72c6 7c00  |._'|.j.j*..r.|.
+00001fc0: 6a27 a013 7c04 7c06 a102 5c02 7d04 7d06  j'..|.|...\.}.}.
+00001fd0: 7c00 6a27 6a14 7c05 6401 6402 8d02 5c02  |.j'j.|.d.d...\.
+00001fe0: 7d05 7d08 7c00 6a2b 9002 73e8 742c 7c00  }.}.|.j+..s.t,|.
+00001ff0: 6a1c 7c00 6a0a 7c00 6a2d 7c00 6a2e 640a  j.|.j.|.j-|.j.d.
+00002000: 8d04 7c00 5f2b 7c00 6a2b a01b 7c04 7c05  ..|._+|.j+..|.|.
+00002010: 7c06 7c07 a104 0100 7c00 6a0a 9003 721e  |.|.....|.j...r.
+00002020: 7c00 6a0a 6a2f 9003 721e 7430 7c00 6a2b  |.j.j/..r.t0|.j+
+00002030: 6a31 7c05 640b 8303 7c00 5f32 6403 7c00  j1|.d...|._2d.|.
+00002040: 5f33 6405 5300 290c 7a19 5472 6169 6e20  _3d.S.).z.Train 
+00002050: 6120 6675 6c6c 204d 4c20 7069 7065 6c69  a full ML pipeli
+00002060: 6e65 2e46 a901 5a0e 7072 6564 6963 746f  ne.F..Z.predicto
+00002070: 6e5f 6d6f 6465 54a9 01da 0464 726f 704e  n_modeT....dropN
+00002080: 721d 0000 0072 1e00 0000 da08 6361 7465  r....r......cate
+00002090: 676f 7279 2902 da0c 7261 6e64 6f6d 5f73  gory)...random_s
+000020a0: 7461 7465 723e 0000 0029 0372 2800 0000  tater>...).r(...
+000020b0: 7229 0000 0072 2a00 0000 da04 7472 6565  r)...r*.....tree
+000020c0: 2934 720f 0000 0072 1600 0000 5a1b 6669  )4r....r....Z.fi
+000020d0: 745f 7472 616e 7366 6f72 6d5f 6665 6174  t_transform_feat
+000020e0: 7572 655f 7479 7065 7372 2c00 0000 7221  ure_typesr,...r!
+000020f0: 0000 0072 2000 0000 7214 0000 0072 2e00  ...r ...r....r..
+00002100: 0000 5a1b 6669 745f 7472 616e 7366 6f72  ..Z.fit_transfor
+00002110: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
+00002120: 2200 0000 7228 0000 0072 0a00 0000 7244  "...r(...r....rD
+00002130: 0000 0072 1b00 0000 7223 0000 00da 0a74  ...r....r#.....t
+00002140: 7261 696e 5f73 697a 65da 1367 6c6f 6261  rain_size..globa
+00002150: 6c5f 7261 6e64 6f6d 5f73 7461 7465 5a14  l_random_stateZ.
+00002160: 7472 6169 6e5f 7370 6c69 745f 7374 7261  train_split_stra
+00002170: 7469 6679 7226 0000 00da 0d66 6974 5f74  tifyr&.....fit_t
+00002180: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
+00002190: 6f72 6dda 0b72 6573 6574 5f69 6e64 6578  orm..reset_index
+000021a0: da06 7265 6d6f 7665 7217 0000 0072 1300  ..remover....r..
+000021b0: 0000 7218 0000 0072 2f00 0000 da03 6669  ..r....r/.....fi
+000021c0: 7472 1f00 0000 7241 0000 0072 1900 0000  tr....rA...r....
+000021d0: 722d 0000 005a 1e66 6974 5f74 6172 6765  r-...Z.fit_targe
+000021e0: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
+000021f0: 636c 6173 73da 2474 7261 6e73 666f 726d  class.$transform
+00002200: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
+00002210: 696e 6172 795f 636c 6173 7372 1a00 0000  inary_classr....
+00002220: 5a1c 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
+00002230: 6f64 655f 6d75 6c74 6963 6c61 7373 da22  ode_multiclass."
+00002240: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
+00002250: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
+00002260: 7373 da06 6173 7479 7065 7225 0000 0072  ss..astyper%...r
+00002270: 2700 0000 7215 0000 0072 3e00 0000 723a  '...r....r>...r:
+00002280: 0000 0072 2400 0000 7211 0000 0072 2900  ...r$...r....r).
+00002290: 0000 722a 0000 0072 4200 0000 720e 0000  ..r*...rB...r...
+000022a0: 00da 056d 6f64 656c 7230 0000 0072 2b00  ...modelr0...r+.
+000022b0: 0000 2909 7231 0000 0072 3500 0000 7245  ..).r1...r5...rE
+000022c0: 0000 0072 2c00 0000 da07 785f 7472 6169  ...r,.....x_trai
+000022d0: 6eda 0678 5f74 6573 74da 0779 5f74 7261  n..x_test..y_tra
+000022e0: 696e da06 795f 7465 7374 da01 5f72 3200  in..y_test.._r2.
+000022f0: 0000 7232 0000 0072 3300 0000 7252 0000  ..r2...r3...rR..
+00002300: 00a6 0000 0073 d600 0000 0002 0601 0601  .....s..........
+00002310: 0a01 0602 0801 0e01 0803 0601 08ff 02fe  ................
+00002320: 0201 04ff 0206 0a01 0a02 0601 0802 0a02  ................
+00002330: 0201 0201 0201 0401 0601 0601 06fa 0c09  ................
+00002340: 0801 1201 0601 0200 0200 02ff 0a03 0601  ................
+00002350: 0a01 0e01 02ff 0a03 0e01 02ff 0a03 0c01  ................
+00002360: 0c02 1201 0c01 0200 04ff 0804 0801 0c01  ................
+00002370: 0c03 08ff 0402 08fe 0403 06fd 0405 0c01  ................
+00002380: 0e01 0e02 08ff 0402 08fe 0403 06fd 0405  ................
+00002390: 0c01 0e01 0e01 0a01 1601 1602 0801 0601  ................
+000023a0: 0200 02ff 0803 0601 0200 0200 02ff 0a04  ................
+000023b0: 0801 0201 0601 06fe 0805 0a01 0601 0200  ................
+000023c0: 02ff 0803 0601 0200 02ff 0a04 0801 0201  ................
+000023d0: 0401 0401 0401 04fc 0806 1201 1201 1201  ................
+000023e0: 7a0c 426c 7565 4361 7374 2e66 6974 2905  z.BlueCast.fit).
+000023f0: 7235 0000 00da 0764 665f 6576 616c da0b  r5.....df_eval..
+00002400: 7461 7267 6574 5f65 7661 6c72 4500 0000  target_evalrE...
+00002410: 7236 0000 0063 0500 0000 0000 0000 0000  r6...c..........
+00002420: 0000 0800 0000 0400 0000 4300 0000 732c  ..........C...s,
+00002430: 0000 007c 00a0 007c 017c 04a1 0201 007c  ...|...|.|.....|
+00002440: 00a0 017c 02a1 015c 027d 057d 0674 027c  ...|...\.}.}.t.|
+00002450: 036a 037c 057c 0683 037d 077c 0753 0029  .j.|.|...}.|.S.)
+00002460: 0161 8e02 0000 5472 6169 6e20 6120 6675  .a....Train a fu
+00002470: 6c6c 204d 4c20 7069 7065 6c69 6e65 2061  ll ML pipeline a
+00002480: 6e64 2065 7661 6c75 6174 6520 6f6e 2061  nd evaluate on a
+00002490: 2068 6f6c 646f 7574 2073 6574 2e0a 0a20   holdout set... 
+000024a0: 2020 2020 2020 2054 6869 7320 6973 2061         This is a
+000024b0: 2063 6f6e 7665 6e69 656e 6365 2066 756e   convenience fun
+000024c0: 6374 696f 6e20 746f 2074 7261 696e 2061  ction to train a
+000024d0: 6e64 2065 7661 6c75 6174 6520 6f6e 2061  nd evaluate on a
+000024e0: 2068 6f6c 646f 7574 2073 6574 2e20 4974   holdout set. It
+000024f0: 2069 7320 7265 636f 6d6d 656e 6465 6420   is recommended 
+00002500: 746f 2075 7365 2074 6869 7320 666f 7220  to use this for 
+00002510: 6d6f 6465 6c0a 2020 2020 2020 2020 6578  model.        ex
+00002520: 706c 6f72 6174 696f 6e2e 204f 6e20 7072  ploration. On pr
+00002530: 6f64 7563 7469 6f6e 2074 6865 2073 696d  oduction the sim
+00002540: 706c 6520 6669 7428 2920 6675 6e63 7469  ple fit() functi
+00002550: 6f6e 2073 686f 756c 6420 6265 2075 7365  on should be use
+00002560: 642e 0a20 2020 2020 2020 203a 7061 7261  d..        :para
+00002570: 6d20 3a64 663a 2054 616b 6573 2061 2070  m :df: Takes a p
+00002580: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
+00002590: 636f 6e74 6169 6e69 6e67 2074 6865 2074  containing the t
+000025a0: 7261 696e 696e 6720 6461 7461 2061 6e64  raining data and
+000025b0: 2074 6865 2074 6172 6765 7473 2e0a 2020   the targets..  
+000025c0: 2020 2020 2020 3a70 6172 616d 203a 6466        :param :df
+000025d0: 5f65 7661 6c3a 2054 616b 6573 2061 2070  _eval: Takes a p
+000025e0: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
+000025f0: 636f 6e74 6169 6e69 6e67 2074 6865 2065  containing the e
+00002600: 7661 6c75 6174 696f 6e20 6461 7461 2c20  valuation data, 
+00002610: 6275 7420 6e6f 7420 7468 6520 7461 7267  but not the targ
+00002620: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
+00002630: 7261 6d20 3a74 6172 6765 745f 6576 616c  ram :target_eval
+00002640: 3a20 5461 6b65 7320 6120 7061 6e64 6173  : Takes a pandas
+00002650: 2053 6572 6965 7320 636f 6e74 6169 6e69   Series containi
+00002660: 6e67 2074 6865 2065 7661 6c75 6174 696f  ng the evaluatio
+00002670: 6e20 7461 7267 6574 732e 0a20 2020 2020  n targets..     
+00002680: 2020 203a 7061 7261 6d20 3a74 6172 6765     :param :targe
+00002690: 745f 636f 6c3a 2054 616b 6573 2061 2073  t_col: Takes a s
+000026a0: 7472 696e 6720 636f 6e74 6169 6e69 6e67  tring containing
+000026b0: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+000026c0: 2074 6172 6765 7420 636f 6c75 6d6e 2069   target column i
+000026d0: 6e73 6964 6520 7468 6520 7472 6169 6e69  nside the traini
+000026e0: 6e67 2064 6174 6120 6466 2e0a 2020 2020  ng data df..    
+000026f0: 2020 2020 2904 7252 0000 00da 0770 7265      ).rR.....pre
+00002700: 6469 6374 720d 0000 00da 0676 616c 7565  dictr......value
+00002710: 7329 0872 3100 0000 7235 0000 0072 5c00  s).r1...r5...r\.
+00002720: 0000 725d 0000 0072 4500 0000 da07 795f  ..r]...rE.....y_
+00002730: 7072 6f62 73da 0979 5f63 6c61 7373 6573  probs..y_classes
+00002740: 5a09 6576 616c 5f64 6963 7472 3200 0000  Z.eval_dictr2...
+00002750: 7232 0000 0072 3300 0000 da08 6669 745f  r2...r3.....fit_
+00002760: 6576 616c 1601 0000 7308 0000 0000 100c  eval....s.......
+00002770: 010e 010e 017a 1142 6c75 6543 6173 742e  .....z.BlueCast.
+00002780: 6669 745f 6576 616c 6302 0000 0000 0000  fit_evalc.......
+00002790: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+000027a0: 0073 5801 0000 7400 8300 0100 7c00 6a01  .sX...t.....|.j.
+000027b0: 7314 7402 6401 8301 8201 7c00 6a03 7322  s.t.d.....|.j.s"
+000027c0: 7402 6402 8301 8201 7c00 6a01 6a04 7c01  t.d.....|.j.j.|.
+000027d0: 7c00 6a05 6701 6403 8d02 7d01 7c00 6a06  |.j.g.d...}.|.j.
+000027e0: 725c 7c00 6a06 6a07 7c01 6404 6405 8d02  r\|.j.j.|.d.d...
+000027f0: 5c02 7d01 7d02 7c01 6a08 6404 6406 8d01  \.}.}.|.j.d.d...
+00002800: 7d01 7409 7c01 8301 7d01 740a 7c01 7c00  }.t.|...}.t.|.|.
+00002810: 6a0b 8302 7d01 7c00 6a0c 7282 7c00 6a0c  j...}.|.j.r.|.j.
+00002820: a007 7c01 a101 7d01 7c00 6a0d 72ba 7c00  ..|...}.|.j.r.|.
+00002830: 6a0e 72ba 7c00 6a0f 6407 6b02 72ba 7410  j.r.|.j.d.k.r.t.
+00002840: 7c00 6a0e 7411 8302 72ba 7c00 6a03 6a12  |.j.t...r.|.j.j.
+00002850: 73ba 7c00 6a0e a013 7c01 a101 7d01 6e58  s.|.j...|...}.nX
+00002860: 7c00 6a0d 72f2 7c00 6a0e 72f2 7c00 6a0f  |.j.r.|.j.r.|.j.
+00002870: 6408 6b02 72f2 7410 7c00 6a0e 7414 8302  d.k.r.t.|.j.t...
+00002880: 72f2 7c00 6a03 6a12 73f2 7c00 6a0e a015  r.|.j.j.s.|.j...
+00002890: 7c01 a101 7d01 6e20 7c00 6a03 6a12 9001  |...}.n |.j.j...
+000028a0: 7212 7c01 7c00 6a0d 1900 a016 6409 a101  r.|.|.j.....d...
+000028b0: 7c01 7c00 6a0d 3c00 7c00 6a17 9001 722e  |.|.j.<.|.j...r.
+000028c0: 7c00 6a17 6a07 7c01 6404 6405 8d02 5c02  |.j.j.|.d.d...\.
+000028d0: 7d01 7d02 7c00 6a18 9001 7254 7c00 6a03  }.}.|.j...rT|.j.
+000028e0: 6a19 9001 7254 7c00 6a18 6a07 7c01 6404  j...rT|.j.j.|.d.
+000028f0: 6405 8d02 5c02 7d01 7d02 7c01 5300 290a  d...\.}.}.|.S.).
+00002900: 7a37 5472 616e 7366 6f72 6d20 6e65 7720  z7Transform new 
+00002910: 6461 7461 2061 6363 6f72 6469 6e67 2074  data according t
+00002920: 6f20 7072 6570 726f 6365 7373 696e 6720  o preprocessing 
+00002930: 7069 7065 6c69 6e65 2efa 2a46 6561 7475  pipeline..*Featu
+00002940: 7265 2074 7970 6520 636f 6e76 6572 7465  re type converte
+00002950: 7220 636f 756c 6420 6e6f 7420 6265 2066  r could not be f
+00002960: 6f75 6e64 2e7a 2a54 7261 696e 696e 6720  ound.z*Training 
+00002970: 636f 6e66 6967 7572 6174 696f 6e20 636f  configuration co
+00002980: 756c 6420 6e6f 7420 6265 2066 6f75 6e64  uld not be found
+00002990: 2e29 015a 0b69 676e 6f72 655f 636f 6c73  .).Z.ignore_cols
+000029a0: 5472 4600 0000 7247 0000 0072 1d00 0000  TrF...rG...r....
+000029b0: 721e 0000 0072 4900 0000 291a 720f 0000  r....rI...).r...
+000029c0: 0072 2c00 0000 da09 4578 6365 7074 696f  .r,.....Exceptio
+000029d0: 6e72 2800 0000 5a17 7472 616e 7366 6f72  nr(...Z.transfor
+000029e0: 6d5f 6665 6174 7572 655f 7479 7065 7372  m_feature_typesr
+000029f0: 2000 0000 7226 0000 0072 4f00 0000 7250   ...r&...rO...rP
+00002a00: 0000 0072 1700 0000 7213 0000 0072 2200  ...r....r....r".
+00002a10: 0000 722f 0000 0072 2100 0000 722d 0000  ..r/...r!...r-..
+00002a20: 0072 1f00 0000 da0a 6973 696e 7374 616e  .r......isinstan
+00002a30: 6365 7219 0000 0072 4100 0000 7253 0000  cer....rA...rS..
+00002a40: 0072 1a00 0000 7254 0000 0072 5500 0000  .r....rT...rU...
+00002a50: 7225 0000 0072 2700 0000 723a 0000 0029  r%...r'...r:...)
+00002a60: 0372 3100 0000 7235 0000 0072 5b00 0000  .r1...r5...r[...
+00002a70: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00002a80: 1274 7261 6e73 666f 726d 5f6e 6577 5f64  .transform_new_d
+00002a90: 6174 612b 0100 0073 5a00 0000 0002 0601  ata+...sZ.......
+00002aa0: 0601 0802 0601 0802 0601 0200 06ff 0604  ................
+00002ab0: 0601 1401 0c02 0801 0c02 0601 0c03 04ff  ................
+00002ac0: 0202 04fe 0203 08fd 0204 0afc 0205 06fb  ................
+00002ad0: 0207 0e02 04ff 0202 04fe 0203 08fd 0204  ................
+00002ae0: 0afc 0205 06fb 0207 0e01 0a01 1602 0801  ................
+00002af0: 1402 1201 1402 7a1b 426c 7565 4361 7374  ......z.BlueCast
+00002b00: 2e74 7261 6e73 666f 726d 5f6e 6577 5f64  .transform_new_d
+00002b10: 6174 6163 0200 0000 0000 0000 0000 0000  atac............
+00002b20: 0400 0000 0500 0000 4300 0000 7398 0000  ........C...s...
+00002b30: 007c 006a 0073 0e74 0164 0183 0182 017c  .|.j.s.t.d.....|
+00002b40: 006a 0273 1c74 0164 0283 0182 017c 006a  .j.s.t.d.....|.j
+00002b50: 0373 2a74 0464 0383 0182 0174 0583 0001  .s*t.d.....t....
+00002b60: 007c 00a0 067c 01a1 017d 0174 0774 08a0  .|...|...}.t.t..
+00002b70: 09a1 009b 0064 049d 0283 0101 007c 006a  .....d.......|.j
+00002b80: 00a0 0a7c 01a1 015c 027d 027d 037c 006a  ...|...\.}.}.|.j
+00002b90: 026a 0b72 907c 006a 0c7c 006a 026a 0b6b  .j.r.|.j.|.j.j.k
+00002ba0: 0672 907c 006a 0d72 907c 006a 0272 907c  .r.|.j.r.|.j.r.|
+00002bb0: 006a 0da0 0e74 0fa0 107c 03a1 01a1 017d  .j...t...|.....}
+00002bc0: 037c 027c 0366 0253 0029 057a 9050 7265  .|.|.f.S.).z.Pre
+00002bd0: 6469 6374 206f 6e20 756e 7365 656e 2064  dict on unseen d
+00002be0: 6174 612e 0a0a 2020 2020 2020 2020 5265  ata...        Re
+00002bf0: 7475 726e 2074 6865 2070 7265 6469 6374  turn the predict
+00002c00: 6564 2070 726f 6261 6269 6c69 7469 6573  ed probabilities
+00002c10: 2061 6e64 2074 6865 2070 7265 6469 6374   and the predict
+00002c20: 6564 2063 6c61 7373 6573 3a0a 2020 2020  ed classes:.    
+00002c30: 2020 2020 795f 7072 6f62 732c 2079 5f63      y_probs, y_c
+00002c40: 6c61 7373 6573 203d 2070 7265 6469 6374  lasses = predict
+00002c50: 2864 6629 0a20 2020 2020 2020 207a 1b4d  (df).        z.M
+00002c60: 6c20 6d6f 6465 6c20 636f 756c 6420 6e6f  l model could no
+00002c70: 7420 6265 2066 6f75 6e64 7263 0000 007a  t be foundrc...z
+00002c80: 1563 6f6e 665f 7472 6169 6e69 6e67 2069  .conf_training i
+00002c90: 7320 4e6f 6e65 7a0f 3a20 5072 6564 6963  s Nonez.: Predic
+00002ca0: 7469 6e67 2e2e 2e29 1172 2400 0000 7264  ting...).r$...rd
+00002cb0: 0000 0072 2c00 0000 7228 0000 00da 0a56  ...r,...r(.....V
+00002cc0: 616c 7565 4572 726f 7272 0f00 0000 7266  alueErrorr....rf
+00002cd0: 0000 0072 1000 0000 7202 0000 00da 0675  ...r....r......u
+00002ce0: 7463 6e6f 7772 5e00 0000 7221 0000 0072  tcnowr^...r!...r
+00002cf0: 2000 0000 722e 0000 00da 1f6c 6162 656c   ...r......label
+00002d00: 5f65 6e63 6f64 6572 5f72 6576 6572 7365  _encoder_reverse
+00002d10: 5f74 7261 6e73 666f 726d da02 7064 da06  _transform..pd..
+00002d20: 5365 7269 6573 2904 7231 0000 0072 3500  Series).r1...r5.
+00002d30: 0000 7260 0000 0072 6100 0000 7232 0000  ..r`...ra...r2..
+00002d40: 0072 3200 0000 7233 0000 0072 5e00 0000  .r2...r3...r^...
+00002d50: 5d01 0000 732a 0000 0000 0606 0108 0206  ]...s*..........
+00002d60: 0108 0206 0108 0206 010a 0212 0110 0208  ................
+00002d70: 020c ff02 0204 fe02 0304 fd02 0506 0108  ................
+00002d80: ff04 047a 1042 6c75 6543 6173 742e 7072  ...z.BlueCast.pr
+00002d90: 6564 6963 7429 0a4e 4e4e 4e4e 4e4e 4e4e  edict).NNNNNNNNN
+00002da0: 4e29 1fda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00002db0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00002dc0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00002dd0: 7206 0000 0072 0900 0000 da03 7374 72da  r....r......str.
+00002de0: 0566 6c6f 6174 da03 696e 7472 0700 0000  .float..intr....
+00002df0: 7205 0000 0072 1100 0000 7203 0000 0072  r....r....r....r
+00002e00: 1200 0000 7215 0000 0072 0a00 0000 720c  ....r....r....r.
+00002e10: 0000 0072 0b00 0000 7234 0000 0072 6a00  ...r....r4...rj.
+00002e20: 0000 da09 4461 7461 4672 616d 6572 4400  ....DataFramerD.
+00002e30: 0000 7252 0000 0072 6b00 0000 7204 0000  ..rR...rk...r...
+00002e40: 0072 6200 0000 7266 0000 0072 0800 0000  .rb...rf...r....
+00002e50: da02 6e70 da07 6e64 6172 7261 7972 5e00  ..np..ndarrayr^.
+00002e60: 0000 7232 0000 0072 3200 0000 7232 0000  ..r2...r2...r2..
+00002e70: 0072 3300 0000 721c 0000 0027 0000 0073  .r3...r....'...s
+00002e80: 4a00 0000 0801 0418 0001 0001 0001 0001  J...............
+00002e90: 0001 0003 0001 0001 0001 00f1 0202 0601  ................
+00002ea0: 0c01 1401 1401 0601 0e01 0601 0601 0201  ................
+00002eb0: 0aff 0203 0601 0601 06f1 0c26 1244 1472  ...........&.D.r
+00002ec0: 0401 0401 0401 0201 0afa 0c15 1432 721c  .............2r.
+00002ed0: 0000 0029 3072 6f00 0000 723b 0000 0072  ...)0ro...r;...r
+00002ee0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00002ef0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00002f00: 7207 0000 0072 0800 0000 7209 0000 00da  r....r....r.....
+00002f10: 056e 756d 7079 7274 0000 00da 0670 616e  .numpyrt.....pan
+00002f20: 6461 7372 6a00 0000 5a1f 626c 7565 6361  dasrj...Z.blueca
+00002f30: 7374 2e63 6f6e 6669 672e 7472 6169 6e69  st.config.traini
+00002f40: 6e67 5f63 6f6e 6669 6772 0a00 0000 720b  ng_configr....r.
+00002f50: 0000 0072 0c00 0000 5a20 626c 7565 6361  ...r....Z blueca
+00002f60: 7374 2e65 7661 6c75 6174 696f 6e2e 6576  st.evaluation.ev
+00002f70: 616c 5f6d 6574 7269 6373 720d 0000 005a  al_metricsr....Z
+00002f80: 1f62 6c75 6563 6173 742e 6576 616c 7561  .bluecast.evalua
+00002f90: 7469 6f6e 2e73 6861 705f 7661 6c75 6573  tion.shap_values
+00002fa0: 720e 0000 005a 2462 6c75 6563 6173 742e  r....Z$bluecast.
+00002fb0: 6765 6e65 7261 6c5f 7574 696c 732e 6765  general_utils.ge
+00002fc0: 6e65 7261 6c5f 7574 696c 7372 0f00 0000  neral_utilsr....
+00002fd0: 7210 0000 005a 1d62 6c75 6563 6173 742e  r....Z.bluecast.
+00002fe0: 6d6c 5f6d 6f64 656c 6c69 6e67 2e78 6762  ml_modelling.xgb
+00002ff0: 6f6f 7374 7211 0000 005a 1d62 6c75 6563  oostr....Z.bluec
+00003000: 6173 742e 7072 6570 726f 6365 7373 696e  ast.preprocessin
+00003010: 672e 6375 7374 6f6d 7212 0000 005a 2862  g.customr....Z(b
+00003020: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
+00003030: 7373 696e 672e 6461 7465 7469 6d65 5f66  ssing.datetime_f
+00003040: 6561 7475 7265 7372 1300 0000 5a2b 626c  eaturesr....Z+bl
+00003050: 7565 6361 7374 2e70 7265 7072 6f63 6573  uecast.preproces
+00003060: 7369 6e67 2e65 6e63 6f64 655f 7461 7267  sing.encode_targ
+00003070: 6574 5f6c 6162 656c 7372 1400 0000 5a28  et_labelsr....Z(
+00003080: 626c 7565 6361 7374 2e70 7265 7072 6f63  bluecast.preproc
+00003090: 6573 7369 6e67 2e66 6561 7475 7265 5f73  essing.feature_s
+000030a0: 656c 6563 7469 6f6e 7215 0000 005a 2462  electionr....Z$b
+000030b0: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
+000030c0: 7373 696e 672e 6665 6174 7572 655f 7479  ssing.feature_ty
+000030d0: 7065 7372 1600 0000 5a25 626c 7565 6361  pesr....Z%blueca
+000030e0: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+000030f0: 2e6e 756c 6c73 5f61 6e64 5f69 6e66 7372  .nulls_and_infsr
+00003100: 1700 0000 5a24 626c 7565 6361 7374 2e70  ....Z$bluecast.p
+00003110: 7265 7072 6f63 6573 7369 6e67 2e73 6368  reprocessing.sch
+00003120: 656d 615f 6368 6563 6b73 7218 0000 005a  ema_checksr....Z
+00003130: 2662 6c75 6563 6173 742e 7072 6570 726f  &bluecast.prepro
+00003140: 6365 7373 696e 672e 7461 7267 6574 5f65  cessing.target_e
+00003150: 6e63 6f64 696e 6772 1900 0000 721a 0000  ncodingr....r...
+00003160: 005a 2762 6c75 6563 6173 742e 7072 6570  .Z'bluecast.prep
+00003170: 726f 6365 7373 696e 672e 7472 6169 6e5f  rocessing.train_
+00003180: 7465 7374 5f73 706c 6974 721b 0000 0072  test_splitr....r
+00003190: 1c00 0000 7232 0000 0072 3200 0000 7232  ....r2...r2...r2
+000031a0: 0000 0072 3300 0000 da08 3c6d 6f64 756c  ...r3.....<modul
+000031b0: 653e 0100 0000 7328 0000 0004 0808 010c  e>....s(........
+000031c0: 0124 0208 0108 0214 050c 010c 0110 010c  .$..............
+000031d0: 010c 010c 010c 010c 010c 010c 010c 0110  ................
+000031e0: 040c 03                                  ...
```

### Comparing `bluecast-0.7/bluecast/blueprints/cast.py` & `bluecast-0.8/bluecast/blueprints/cast.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     """Run fully configured classification blueprint.
 
     Customization via class attributes is possible. Configs can be instantiated and provided to change Xgboost training.
     Default hyperparameter search space is relatively light-weight to speed up the prototyping.
     :param :class_problem: Takes a string containing the class problem type. Either "binary" or "multiclass".
     :param :target_column: Takes a string containing the name of the target column.
     :param :cat_columns: Takes a list of strings containing the names of the categorical columns. If not provided,
-    BlueCast will infer these automaically.
+    BlueCast will infer these automatically.
     :param :date_columns: Takes a list of strings containing the names of the date columns. If not provided,
-    BlueCast will infer these automaically.
+    BlueCast will infer these automatically.
     :param :time_split_column: Takes a string containing the name of the time split column. If not provided,
     BlueCast will not split the data by time or order, but do a random split instead.
     :param :ml_model: Takes an instance of a XgboostModel class. If not provided, BlueCast will instantiate one.
     This is an API to pass any model class. Inherit the baseclass from ml_modelling.base_model.BaseModel.
     :param custom_preprocessor: Takes an instance of a CustomPreprocessing class. Allows users to inject custom
     preprocessing steps which take place right after the train test spit.
     :param custom_last_mile_computation: Takes an instance of a CustomPreprocessing class. Allows users to inject custom
```

### Comparing `bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 10:56:32 2023 UTC, .py size: 3071 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6063 9d64 ff0b 0000  o.......`c.d....
+00000000: 550d 0d0a 0000 0000 e7a0 a364 740b 0000  U..........dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 6505 4700  d.d...d...Z.e.G.
 00000060: 6406 6407 8400 6407 8302 8301 5a07 6505  d.d...d.....Z.e.
 00000070: 4700 6408 6409 8400 6409 8302 8301 5a08  G.d.d...d.....Z.
@@ -41,208 +41,191 @@
 00000280: da04 4469 6374 da08 4f70 7469 6f6e 616c  ..Dict..Optional
 00000290: 2901 da09 6461 7461 636c 6173 7363 0000  )...dataclassc..
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 000002b0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
 000002c0: 005a 0264 015a 0364 0253 0029 03da 0643  .Z.d.Z.d.S.)...C
 000002d0: 6f6e 6669 6754 4e29 04da 085f 5f6e 616d  onfigTN)...__nam
 000002e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5f5a 1761  .__qualname__Z.a
+000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 1761  .__qualname__..a
 00000300: 7262 6974 7261 7279 5f74 7970 6573 5f61  rbitrary_types_a
-00000310: 6c6c 6f77 6564 a900 7209 0000 0072 0900  llowed..r....r..
+00000310: 6c6c 6f77 6564 a900 720a 0000 0072 0a00  llowed..r....r..
 00000320: 0000 fa45 2f68 6f6d 652f 7468 6f6d 6173  ...E/home/thomas
 00000330: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
 00000340: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
 00000350: 636f 6e66 6967 2f74 7261 696e 696e 675f  config/training_
 00000360: 636f 6e66 6967 2e70 7972 0500 0000 0d00  config.pyr......
-00000370: 0000 7304 0000 0008 0008 0172 0500 0000  ..s........r....
-00000380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000390: 0003 0000 0040 0000 0073 ba00 0000 6500  .....@...s....e.
-000003a0: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
-000003b0: 6505 6506 6403 3c00 6404 5a07 6508 6506  e.e.d.<.d.Z.e.e.
-000003c0: 6405 3c00 6406 5a09 6505 6506 6407 3c00  d.<.d.Z.e.e.d.<.
-000003d0: 6408 5a0a 6505 6506 6409 3c00 640a 5a0b  d.Z.e.e.d.<.d.Z.
-000003e0: 6505 6506 640b 3c00 6402 5a0c 6505 6506  e.e.d.<.d.Z.e.e.
-000003f0: 640c 3c00 6404 5a0d 6508 6506 640d 3c00  d.<.d.Z.e.e.d.<.
-00000400: 640e 5a0e 6508 6506 640f 3c00 6404 5a0f  d.Z.e.e.d.<.d.Z.
-00000410: 6508 6506 6410 3c00 6411 5a10 6511 6506  e.e.d.<.d.Z.e.e.
-00000420: 6412 3c00 6404 5a12 6508 6506 6413 3c00  d.<.d.Z.e.e.d.<.
-00000430: 6404 5a13 6508 6506 6414 3c00 6415 5a14  d.Z.e.e.d.<.d.Z.
-00000440: 6505 6506 6416 3c00 640e 5a15 6508 6506  e.e.d.<.d.Z.e.e.
-00000450: 6417 3c00 6418 5300 2919 da0e 5472 6169  d.<.d.S.)...Trai
-00000460: 6e69 6e67 436f 6e66 6967 7a23 4465 6669  ningConfigz#Defi
-00000470: 6e65 2067 656e 6572 616c 2074 7261 696e  ne general train
-00000480: 696e 6720 7061 7261 6d65 7465 7273 2ee9  ing parameters..
-00000490: 0a00 0000 da13 676c 6f62 616c 5f72 616e  ......global_ran
-000004a0: 646f 6d5f 7374 6174 6554 da17 7368 7566  dom_stateT..shuf
-000004b0: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
-000004c0: 696e 67e9 6400 0000 da1c 6879 7065 7270  ing.d.....hyperp
-000004d0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
-000004e0: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
-000004f0: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
-00000500: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
-00000510: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
-00000520: 756e 696e 675f 6376 5f66 6f6c 6473 da15  uning_cv_folds..
-00000530: 6561 726c 795f 7374 6f70 7069 6e67 5f72  early_stopping_r
-00000540: 6f75 6e64 73da 0e61 7574 6f74 756e 655f  ounds..autotune_
-00000550: 6d6f 6465 6c46 da18 656e 6162 6c65 5f66  modelF..enable_f
-00000560: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
-00000570: da15 6361 6c63 756c 6174 655f 7368 6170  ..calculate_shap
-00000580: 5f76 616c 7565 73e7 9a99 9999 9999 e93f  _values........?
-00000590: da0a 7472 6169 6e5f 7369 7a65 da14 7472  ..train_size..tr
-000005a0: 6169 6e5f 7370 6c69 745f 7374 7261 7469  ain_split_strati
-000005b0: 6679 da1d 7573 655f 6675 6c6c 5f64 6174  fy..use_full_dat
-000005c0: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
-000005d0: 6ce9 0500 0000 da16 6d69 6e5f 6665 6174  l.......min_feat
-000005e0: 7572 6573 5f74 6f5f 7365 6c65 6374 da1d  ures_to_select..
-000005f0: 6361 745f 656e 636f 6469 6e67 5f76 6961  cat_encoding_via
-00000600: 5f6d 6c5f 616c 676f 7269 7468 6d4e 2916  _ml_algorithmN).
-00000610: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
-00000620: 075f 5f64 6f63 5f5f 720d 0000 00da 0369  .__doc__r......i
-00000630: 6e74 da0f 5f5f 616e 6e6f 7461 7469 6f6e  nt..__annotation
-00000640: 735f 5f72 0e00 0000 da04 626f 6f6c 7210  s__r......boolr.
-00000650: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
-00000660: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000670: 0072 1900 0000 da05 666c 6f61 7472 1a00  .r......floatr..
-00000680: 0000 721b 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00000690: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-000006a0: 720a 0000 0072 0b00 0000 1100 0000 7320  r....r........s 
-000006b0: 0000 000a 0004 020c 020c 010c 010c 010c  ................
-000006c0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-000006d0: 0110 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
-000006e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000006f0: 0073 6201 0000 6500 5a01 6400 5a02 5500  .sb...e.Z.d.Z.U.
-00000700: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
-00000710: 6404 5a07 6505 6506 6405 3c00 6406 5a08  d.Z.e.e.d.<.d.Z.
-00000720: 6509 6506 6407 3c00 6408 5a0a 6509 6506  e.e.d.<.d.Z.e.e.
-00000730: 6409 3c00 640a 5a0b 6509 6506 640b 3c00  d.<.d.Z.e.e.d.<.
-00000740: 6408 5a0c 6509 6506 640c 3c00 6406 5a0d  d.Z.e.e.d.<.d.Z.
-00000750: 6509 6506 640d 3c00 6408 5a0e 6509 6506  e.e.d.<.d.Z.e.e.
-00000760: 640e 3c00 6402 5a0f 6505 6506 640f 3c00  d.<.d.Z.e.e.d.<.
-00000770: 6410 5a10 6505 6506 6411 3c00 6412 5a11  d.Z.e.e.d.<.d.Z.
-00000780: 6509 6506 6413 3c00 640a 5a12 6509 6506  e.e.d.<.d.Z.e.e.
-00000790: 6414 3c00 6412 5a13 6509 6506 6415 3c00  d.<.d.Z.e.e.d.<.
-000007a0: 640a 5a14 6509 6506 6416 3c00 6412 5a15  d.Z.e.e.d.<.d.Z.
-000007b0: 6509 6506 6417 3c00 640a 5a16 6509 6506  e.e.d.<.d.Z.e.e.
-000007c0: 6418 3c00 6412 5a17 6509 6506 6419 3c00  d.<.d.Z.e.e.d.<.
-000007d0: 640a 5a18 6509 6506 641a 3c00 6402 5a19  d.Z.e.e.d.<.d.Z.
-000007e0: 6505 6506 641b 3c00 641c 5a1a 6505 6506  e.e.d.<.d.Z.e.e.
-000007f0: 641d 3c00 641e 5a1b 6509 6506 641f 3c00  d.<.d.Z.e.e.d.<.
-00000800: 6402 5a1c 6505 6506 6420 3c00 6421 5a1d  d.Z.e.e.d <.d!Z.
-00000810: 6505 6506 6422 3c00 6423 5a1e 6505 6506  e.e.d"<.d#Z.e.e.
-00000820: 6424 3c00 6404 5a1f 6505 6506 6425 3c00  d$<.d.Z.e.e.d%<.
-00000830: 6426 5a20 6505 6506 6427 3c00 6428 5a21  d&Z e.e.d'<.d(Z!
-00000840: 6522 6506 6429 3c00 642a 5a23 6522 6506  e"e.d)<.d*Z#e"e.
-00000850: 642b 3c00 642c 5300 292d da17 5867 626f  d+<.d,S.)-..Xgbo
-00000860: 6f73 7454 756e 6550 6172 616d 7343 6f6e  ostTuneParamsCon
-00000870: 6669 677a 2a44 6566 696e 6520 6879 7065  figz*Define hype
-00000880: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
-00000890: 6720 7365 6172 6368 2073 7061 6365 2ee9  g search space..
-000008a0: 0200 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
-000008b0: 6d69 6ee9 0300 0000 da0d 6d61 785f 6465  min.......max_de
-000008c0: 7074 685f 6d61 7867 0000 0000 0000 0000  pth_maxg........
-000008d0: da09 616c 7068 615f 6d69 6e67 0000 0000  ..alpha_ming....
-000008e0: 0040 8f40 da09 616c 7068 615f 6d61 7867  .@.@..alpha_maxg
-000008f0: 0000 0000 0000 f03f da0a 6c61 6d62 6461  .......?..lambda
-00000900: 5f6d 696e da0a 6c61 6d62 6461 5f6d 6178  _min..lambda_max
-00000910: da09 6761 6d6d 615f 6d69 6eda 0967 616d  ..gamma_min..gam
-00000920: 6d61 5f6d 6178 da0e 6e75 6d5f 6c65 6176  ma_max..num_leav
-00000930: 6573 5f6d 696e e940 0000 00da 0e6e 756d  es_min.@.....num
-00000940: 5f6c 6561 7665 735f 6d61 7867 3333 3333  _leaves_maxg3333
-00000950: 3333 d33f da0e 7375 625f 7361 6d70 6c65  33.?..sub_sample
-00000960: 5f6d 696e da0e 7375 625f 7361 6d70 6c65  _min..sub_sample
-00000970: 5f6d 6178 da16 636f 6c5f 7361 6d70 6c65  _max..col_sample
-00000980: 5f62 795f 7472 6565 5f6d 696e da16 636f  _by_tree_min..co
-00000990: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
-000009a0: 5f6d 6178 da17 636f 6c5f 7361 6d70 6c65  _max..col_sample
-000009b0: 5f62 795f 6c65 7665 6c5f 6d69 6eda 1763  _by_level_min..c
-000009c0: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
-000009d0: 656c 5f6d 6178 da16 636f 6c5f 7361 6d70  el_max..col_samp
-000009e0: 6c65 5f62 795f 6e6f 6465 5f6d 696e da16  le_by_node_min..
-000009f0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
-00000a00: 6465 5f6d 6178 da15 6d69 6e5f 6368 696c  de_max..min_chil
-00000a10: 645f 7361 6d70 6c65 735f 6d69 6ee9 e803  d_samples_min...
-00000a20: 0000 da15 6d69 6e5f 6368 696c 645f 7361  ....min_child_sa
-00000a30: 6d70 6c65 735f 6d61 78e7 9a99 9999 9999  mples_max.......
-00000a40: b93f da03 6574 61da 0973 7465 7073 5f6d  .?..eta..steps_m
-00000a50: 696e 6950 c300 00da 0973 7465 7073 5f6d  iniP.....steps_m
-00000a60: 6178 7212 0000 00da 156e 756d 5f70 6172  axr......num_par
-00000a70: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
-00000a80: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-00000a90: 655f 6d61 7872 0100 0000 da0f 6d6f 6465  e_maxr......mode
-00000aa0: 6c5f 7665 7262 6f73 6974 79fa 0e6d 756c  l_verbosity..mul
-00000ab0: 7469 3a73 6f66 7470 726f 62da 0f6d 6f64  ti:softprob..mod
-00000ac0: 656c 5f6f 626a 6563 7469 7665 da08 6d6c  el_objective..ml
-00000ad0: 6f67 6c6f 7373 da11 6d6f 6465 6c5f 6576  ogloss..model_ev
-00000ae0: 616c 5f6d 6574 7269 634e 2924 7206 0000  al_metricN)$r...
-00000af0: 0072 0700 0000 7208 0000 0072 1f00 0000  .r....r....r....
-00000b00: 7226 0000 0072 2000 0000 7221 0000 0072  r&...r ...r!...r
-00000b10: 2800 0000 7229 0000 0072 2300 0000 722a  (...r)...r#...r*
-00000b20: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
-00000b30: 0000 722e 0000 0072 2f00 0000 7231 0000  ..r....r/...r1..
-00000b40: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00000b50: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00000b60: 3800 0000 7239 0000 0072 3a00 0000 723c  8...r9...r:...r<
-00000b70: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
-00000b80: 0000 7241 0000 0072 4200 0000 7243 0000  ..rA...rB...rC..
-00000b90: 0072 4500 0000 da03 7374 7272 4700 0000  .rE.....strrG...
-00000ba0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000bb0: 0a00 0000 7224 0000 0025 0000 0073 3c00  ....r$...%...s<.
-00000bc0: 0000 0a00 0402 0c02 0c01 0c01 0c01 0c01  ................
-00000bd0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000be0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000bf0: 0c01 0c01 0c01 0c01 0c01 0c01 1001 7224  ..............r$
-00000c00: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000c10: 0000 0000 0400 0000 4000 0000 73a0 0000  ........@...s...
-00000c20: 0065 005a 0164 005a 0255 0064 015a 0369  .e.Z.d.Z.U.d.Z.i
-00000c30: 0064 0264 0393 0164 0464 0593 0164 0664  .d.d...d.d...d.d
-00000c40: 0793 0164 0864 0993 0164 0a64 0b93 0164  ...d.d...d.d...d
-00000c50: 0c64 0d93 0164 0e64 0f93 0164 1064 0f93  .d...d.d...d.d..
-00000c60: 0164 1164 1293 0164 1364 1493 0164 1564  .d.d...d.d...d.d
-00000c70: 1493 0164 1664 1493 0164 1764 1493 0164  ...d.d...d.d...d
-00000c80: 1864 1993 0164 1a64 0f93 0164 1b64 1c93  .d...d.d...d.d..
-00000c90: 0164 1d64 1e93 015a 0464 1f5a 0565 0665  .d.d...Z.d.Z.e.e
-00000ca0: 0765 0865 0966 0219 0019 0065 0a64 203c  .e.e.f.....e.d <
-00000cb0: 0064 215a 0b65 0965 0a64 223c 0064 1f53  .d!Z.e.e.d"<.d.S
-00000cc0: 0029 23da 1758 6762 6f6f 7374 4669 6e61  .)#..XgboostFina
-00000cd0: 6c50 6172 616d 436f 6e66 6967 7a1e 4465  lParamConfigz.De
-00000ce0: 6669 6e65 2066 696e 616c 2068 7970 6572  fine final hyper
-00000cf0: 2070 6172 616d 6574 6572 732e da09 6f62   parameters...ob
-00000d00: 6a65 6374 6976 6572 4400 0000 da0b 6576  jectiverD.....ev
-00000d10: 616c 5f6d 6574 7269 6372 4600 0000 da07  al_metricrF.....
-00000d20: 7665 7262 6f73 6572 0100 0000 da0b 7472  verboser......tr
-00000d30: 6565 5f6d 6574 686f 64da 0565 7861 6374  ee_method..exact
-00000d40: da09 6e75 6d5f 636c 6173 7372 2500 0000  ..num_classr%...
-00000d50: da09 6d61 785f 6465 7074 6872 2700 0000  ..max_depthr'...
-00000d60: da05 616c 7068 6172 3d00 0000 da06 6c61  ..alphar=.....la
-00000d70: 6d62 6461 da0a 6e75 6d5f 6c65 6176 6573  mbda..num_leaves
-00000d80: e910 0000 00da 0973 7562 7361 6d70 6c65  .......subsample
-00000d90: 7218 0000 00da 1063 6f6c 7361 6d70 6c65  r......colsample
-00000da0: 5f62 7974 7265 65da 1163 6f6c 7361 6d70  _bytree..colsamp
-00000db0: 6c65 5f62 796c 6576 656c da10 636f 6c73  le_bylevel..cols
-00000dc0: 616d 706c 655f 6279 6e6f 6465 da11 6d69  ample_bynode..mi
-00000dd0: 6e5f 6368 696c 645f 7361 6d70 6c65 7372  n_child_samplesr
-00000de0: 0f00 0000 723e 0000 00da 0573 7465 7073  ....r>.....steps
-00000df0: 723b 0000 00da 116e 756d 5f70 6172 616c  r;.....num_paral
-00000e00: 6c65 6c5f 7472 6565 7212 0000 004e da0d  lel_treer....N..
-00000e10: 7361 6d70 6c65 5f77 6569 6768 7467 0000  sample_weightg..
-00000e20: 0000 0000 e03f da18 636c 6173 7369 6669  .....?..classifi
-00000e30: 6361 7469 6f6e 5f74 6872 6573 686f 6c64  cation_threshold
-00000e40: 290c 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
-00000e50: 0072 1f00 0000 da06 7061 7261 6d73 725c  .r......paramsr\
-00000e60: 0000 0072 0300 0000 7202 0000 0072 4800  ...r....r....rH.
-00000e70: 0000 7223 0000 0072 2100 0000 725d 0000  ..r#...r!...r]..
-00000e80: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000e90: 720a 0000 0072 4900 0000 4700 0000 734e  r....rI...G...sN
-00000ea0: 0000 000a 0004 0202 0204 0102 ff04 0202  ................
-00000eb0: fe04 0302 fd04 0402 fc04 0502 fb04 0602  ................
-00000ec0: fa04 0702 f904 0802 f804 0902 f704 0a02  ................
-00000ed0: f604 0b02 f504 0c02 f404 0d02 f304 0e02  ................
-00000ee0: f204 0f02 f104 1002 f004 1104 ef18 1310  ................
-00000ef0: 0172 4900 0000 4e29 0a72 1f00 0000 da06  .rI...N).r......
-00000f00: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
-00000f10: 5a14 7079 6461 6e74 6963 2e64 6174 6163  Z.pydantic.datac
-00000f20: 6c61 7373 6573 7204 0000 0072 0500 0000  lassesr....r....
-00000f30: 720b 0000 0072 2400 0000 7249 0000 0072  r....r$...rI...r
-00000f40: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00000f50: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000f60: 0073 1400 0000 0400 1007 0c02 0e03 0204  .s..............
-00000f70: 1001 0213 1001 0221 1401                 .......!..
+00000370: 0000 7302 0000 0008 0172 0500 0000 6300  ..s......r....c.
+00000380: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000390: 0000 0040 0000 0073 ba00 0000 6500 5a01  ...@...s....e.Z.
+000003a0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
+000003b0: 6506 6403 3c00 6404 5a07 6508 6506 6405  e.d.<.d.Z.e.e.d.
+000003c0: 3c00 6406 5a09 6505 6506 6407 3c00 6408  <.d.Z.e.e.d.<.d.
+000003d0: 5a0a 6505 6506 6409 3c00 640a 5a0b 6505  Z.e.e.d.<.d.Z.e.
+000003e0: 6506 640b 3c00 6402 5a0c 6505 6506 640c  e.d.<.d.Z.e.e.d.
+000003f0: 3c00 6404 5a0d 6508 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
+00000400: 5a0e 6508 6506 640f 3c00 6404 5a0f 6508  Z.e.e.d.<.d.Z.e.
+00000410: 6506 6410 3c00 6411 5a10 6511 6506 6412  e.d.<.d.Z.e.e.d.
+00000420: 3c00 6404 5a12 6508 6506 6413 3c00 640e  <.d.Z.e.e.d.<.d.
+00000430: 5a13 6508 6506 6414 3c00 6415 5a14 6505  Z.e.e.d.<.d.Z.e.
+00000440: 6506 6416 3c00 640e 5a15 6508 6506 6417  e.d.<.d.Z.e.e.d.
+00000450: 3c00 6418 5300 2919 da0e 5472 6169 6e69  <.d.S.)...Traini
+00000460: 6e67 436f 6e66 6967 7a23 4465 6669 6e65  ngConfigz#Define
+00000470: 2067 656e 6572 616c 2074 7261 696e 696e   general trainin
+00000480: 6720 7061 7261 6d65 7465 7273 2ee9 0a00  g parameters....
+00000490: 0000 da13 676c 6f62 616c 5f72 616e 646f  ....global_rando
+000004a0: 6d5f 7374 6174 6554 da17 7368 7566 666c  m_stateT..shuffl
+000004b0: 655f 6475 7269 6e67 5f74 7261 696e 696e  e_during_trainin
+000004c0: 67e9 6400 0000 da1c 6879 7065 7270 6172  g.d.....hyperpar
+000004d0: 616d 6574 6572 5f74 756e 696e 675f 726f  ameter_tuning_ro
+000004e0: 756e 6473 6910 0e00 00da 2668 7970 6572  undsi.....&hyper
+000004f0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+00000500: 5f6d 6178 5f72 756e 7469 6d65 5f73 6563  _max_runtime_sec
+00000510: 73e9 0100 0000 da14 6879 7065 7274 756e  s.......hypertun
+00000520: 696e 675f 6376 5f66 6f6c 6473 da15 6561  ing_cv_folds..ea
+00000530: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
+00000540: 6e64 73da 0e61 7574 6f74 756e 655f 6d6f  nds..autotune_mo
+00000550: 6465 6c46 da18 656e 6162 6c65 5f66 6561  delF..enable_fea
+00000560: 7475 7265 5f73 656c 6563 7469 6f6e da15  ture_selection..
+00000570: 6361 6c63 756c 6174 655f 7368 6170 5f76  calculate_shap_v
+00000580: 616c 7565 73e7 9a99 9999 9999 e93f da0a  alues........?..
+00000590: 7472 6169 6e5f 7369 7a65 da14 7472 6169  train_size..trai
+000005a0: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
+000005b0: da1d 7573 655f 6675 6c6c 5f64 6174 615f  ..use_full_data_
+000005c0: 666f 725f 6669 6e61 6c5f 6d6f 6465 6ce9  for_final_model.
+000005d0: 0500 0000 da16 6d69 6e5f 6665 6174 7572  ......min_featur
+000005e0: 6573 5f74 6f5f 7365 6c65 6374 da1d 6361  es_to_select..ca
+000005f0: 745f 656e 636f 6469 6e67 5f76 6961 5f6d  t_encoding_via_m
+00000600: 6c5f 616c 676f 7269 7468 6d4e 2916 7206  l_algorithmN).r.
+00000610: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
+00000620: 5f64 6f63 5f5f 720e 0000 00da 0369 6e74  _doc__r......int
+00000630: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00000640: 5f72 0f00 0000 da04 626f 6f6c 7211 0000  _r......boolr...
+00000650: 0072 1200 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000660: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000670: 1a00 0000 da05 666c 6f61 7472 1b00 0000  ......floatr....
+00000680: 721c 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000690: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000006a0: 0000 0072 0c00 0000 1100 0000 731e 0000  ...r........s...
+000006b0: 000a 0204 020c 010c 010c 010c 010c 010c  ................
+000006c0: 010c 010c 010c 010c 010c 010c 010c 0172  ...............r
+000006d0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000006e0: 0000 0000 0003 0000 0040 0000 0073 3201  .........@...s2.
+000006f0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000700: 6402 5a04 6505 6506 6403 3c00 6404 5a07  d.Z.e.e.d.<.d.Z.
+00000710: 6505 6506 6405 3c00 6406 5a08 6509 6506  e.e.d.<.d.Z.e.e.
+00000720: 6407 3c00 6408 5a0a 6509 6506 6409 3c00  d.<.d.Z.e.e.d.<.
+00000730: 6406 5a0b 6509 6506 640a 3c00 6408 5a0c  d.Z.e.e.d.<.d.Z.
+00000740: 6509 6506 640b 3c00 6402 5a0d 6505 6506  e.e.d.<.d.Z.e.e.
+00000750: 640c 3c00 640d 5a0e 6505 6506 640e 3c00  d.<.d.Z.e.e.d.<.
+00000760: 640f 5a0f 6509 6506 6410 3c00 6411 5a10  d.Z.e.e.d.<.d.Z.
+00000770: 6509 6506 6412 3c00 640f 5a11 6509 6506  e.e.d.<.d.Z.e.e.
+00000780: 6413 3c00 6411 5a12 6509 6506 6414 3c00  d.<.d.Z.e.e.d.<.
+00000790: 640f 5a13 6509 6506 6415 3c00 6411 5a14  d.Z.e.e.d.<.d.Z.
+000007a0: 6509 6506 6416 3c00 6406 5a15 6509 6506  e.e.d.<.d.Z.e.e.
+000007b0: 6417 3c00 6408 5a16 6509 6506 6418 3c00  d.<.d.Z.e.e.d.<.
+000007c0: 6419 5a17 6509 6506 641a 3c00 640f 5a18  d.Z.e.e.d.<.d.Z.
+000007d0: 6509 6506 641b 3c00 6402 5a19 6505 6506  e.e.d.<.d.Z.e.e.
+000007e0: 641c 3c00 641d 5a1a 6505 6506 641e 3c00  d.<.d.Z.e.e.d.<.
+000007f0: 641f 5a1b 6505 6506 6420 3c00 6421 5a1c  d.Z.e.e.d <.d!Z.
+00000800: 651d 6506 6422 3c00 6423 5a1e 651d 6506  e.e.d"<.d#Z.e.e.
+00000810: 6424 3c00 6425 5a1f 651d 6506 6426 3c00  d$<.d%Z.e.e.d&<.
+00000820: 6427 5300 2928 da17 5867 626f 6f73 7454  d'S.)(..XgboostT
+00000830: 756e 6550 6172 616d 7343 6f6e 6669 677a  uneParamsConfigz
+00000840: 2a44 6566 696e 6520 6879 7065 7270 6172  *Define hyperpar
+00000850: 616d 6574 6572 2074 756e 696e 6720 7365  ameter tuning se
+00000860: 6172 6368 2073 7061 6365 2ee9 0200 0000  arch space......
+00000870: da0d 6d61 785f 6465 7074 685f 6d69 6ee9  ..max_depth_min.
+00000880: 0600 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
+00000890: 6d61 7867 0000 0000 0000 0000 da09 616c  maxg..........al
+000008a0: 7068 615f 6d69 6e67 0000 0000 0000 2440  pha_ming......$@
+000008b0: da09 616c 7068 615f 6d61 78da 0a6c 616d  ..alpha_max..lam
+000008c0: 6264 615f 6d69 6eda 0a6c 616d 6264 615f  bda_min..lambda_
+000008d0: 6d61 78da 0e6e 756d 5f6c 6561 7665 735f  max..num_leaves_
+000008e0: 6d69 6ee9 4000 0000 da0e 6e75 6d5f 6c65  min.@.....num_le
+000008f0: 6176 6573 5f6d 6178 6733 3333 3333 33d3  aves_maxg333333.
+00000900: 3fda 0e73 7562 5f73 616d 706c 655f 6d69  ?..sub_sample_mi
+00000910: 6e67 0000 0000 0000 f03f da0e 7375 625f  ng.......?..sub_
+00000920: 7361 6d70 6c65 5f6d 6178 da16 636f 6c5f  sample_max..col_
+00000930: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
+00000940: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
+00000950: 795f 7472 6565 5f6d 6178 da17 636f 6c5f  y_tree_max..col_
+00000960: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
+00000970: 6d69 6eda 1763 6f6c 5f73 616d 706c 655f  min..col_sample_
+00000980: 6279 5f6c 6576 656c 5f6d 6178 da14 6d69  by_level_max..mi
+00000990: 6e5f 6368 696c 645f 7765 6967 6874 5f6d  n_child_weight_m
+000009a0: 696e da14 6d69 6e5f 6368 696c 645f 7765  in..min_child_we
+000009b0: 6967 6874 5f6d 6178 67fc a9f1 d24d 6250  ight_maxg....MbP
+000009c0: 3fda 0765 7461 5f6d 696e da07 6574 615f  ?..eta_min..eta_
+000009d0: 6d61 78da 0973 7465 7073 5f6d 696e e9e8  max..steps_min..
+000009e0: 0300 00da 0973 7465 7073 5f6d 6178 7201  .....steps_maxr.
+000009f0: 0000 00da 0f6d 6f64 656c 5f76 6572 626f  .....model_verbo
+00000a00: 7369 7479 fa0e 6d75 6c74 693a 736f 6674  sity..multi:soft
+00000a10: 7072 6f62 da0f 6d6f 6465 6c5f 6f62 6a65  prob..model_obje
+00000a20: 6374 6976 65da 086d 6c6f 676c 6f73 73da  ctive..mlogloss.
+00000a30: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
+00000a40: 6963 da06 6762 7472 6565 da07 626f 6f73  ic..gbtree..boos
+00000a50: 7465 724e 2920 7206 0000 0072 0700 0000  terN) r....r....
+00000a60: 7208 0000 0072 2000 0000 7227 0000 0072  r....r ...r'...r
+00000a70: 2100 0000 7222 0000 0072 2900 0000 722a  !...r"...r)...r*
+00000a80: 0000 0072 2400 0000 722b 0000 0072 2c00  ...r$...r+...r,.
+00000a90: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
+00000aa0: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
+00000ab0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+00000ac0: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
+00000ad0: 0000 0072 3b00 0000 723d 0000 0072 3e00  ...r;...r=...r>.
+00000ae0: 0000 7240 0000 00da 0373 7472 7242 0000  ..r@.....strrB..
+00000af0: 0072 4400 0000 720a 0000 0072 0a00 0000  .rD...r....r....
+00000b00: 720a 0000 0072 0b00 0000 7225 0000 0025  r....r....r%...%
+00000b10: 0000 0073 3200 0000 0a02 0402 0c01 0c01  ...s2...........
+00000b20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000b30: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000b40: 0c01 0c01 0c01 0c01 0c01 7225 0000 0063  ..........r%...c
+00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b60: 1200 0000 4000 0000 735e 0000 0065 005a  ....@...s^...e.Z
+00000b70: 0164 005a 0255 0064 015a 0364 0264 0364  .d.Z.U.d.Z.d.d.d
+00000b80: 0464 0564 0664 0764 0864 0864 0964 0a64  .d.d.d.d.d.d.d.d
+00000b90: 0a64 0a64 0a64 0b64 0864 0c64 0d64 0e9c  .d.d.d.d.d.d.d..
+00000ba0: 115a 0464 0f5a 0565 0665 0765 0865 0966  .Z.d.Z.e.e.e.e.f
+00000bb0: 0219 0019 0065 0a64 103c 0064 115a 0b65  .....e.d.<.d.Z.e
+00000bc0: 0965 0a64 123c 0064 0f53 0029 13da 1758  .e.d.<.d.S.)...X
+00000bd0: 6762 6f6f 7374 4669 6e61 6c50 6172 616d  gboostFinalParam
+00000be0: 436f 6e66 6967 7a1e 4465 6669 6e65 2066  Configz.Define f
+00000bf0: 696e 616c 2068 7970 6572 2070 6172 616d  inal hyper param
+00000c00: 6574 6572 732e 723f 0000 0072 4100 0000  eters.r?...rA...
+00000c10: 7201 0000 00da 0565 7861 6374 7226 0000  r......exactr&..
+00000c20: 00e9 0300 0000 679a 9999 9999 99b9 3fe9  ......g.......?.
+00000c30: 1000 0000 7219 0000 0072 1000 0000 723c  ....r....r....r<
+00000c40: 0000 0072 1300 0000 2911 da09 6f62 6a65  ...r....)...obje
+00000c50: 6374 6976 65da 0b65 7661 6c5f 6d65 7472  ctive..eval_metr
+00000c60: 6963 da07 7665 7262 6f73 65da 0b74 7265  ic..verbose..tre
+00000c70: 655f 6d65 7468 6f64 da09 6e75 6d5f 636c  e_method..num_cl
+00000c80: 6173 73da 096d 6178 5f64 6570 7468 da05  ass..max_depth..
+00000c90: 616c 7068 61da 066c 616d 6264 61da 0a6e  alpha..lambda..n
+00000ca0: 756d 5f6c 6561 7665 73da 0973 7562 7361  um_leaves..subsa
+00000cb0: 6d70 6c65 da10 636f 6c73 616d 706c 655f  mple..colsample_
+00000cc0: 6279 7472 6565 da11 636f 6c73 616d 706c  bytree..colsampl
+00000cd0: 655f 6279 6c65 7665 6cda 1063 6f6c 7361  e_bylevel..colsa
+00000ce0: 6d70 6c65 5f62 796e 6f64 65da 116d 696e  mple_bynode..min
+00000cf0: 5f63 6869 6c64 5f73 616d 706c 6573 da03  _child_samples..
+00000d00: 6574 61da 0573 7465 7073 da11 6e75 6d5f  eta..steps..num_
+00000d10: 7061 7261 6c6c 656c 5f74 7265 654e da0d  parallel_treeN..
+00000d20: 7361 6d70 6c65 5f77 6569 6768 7467 0000  sample_weightg..
+00000d30: 0000 0000 e03f da18 636c 6173 7369 6669  .....?..classifi
+00000d40: 6361 7469 6f6e 5f74 6872 6573 686f 6c64  cation_threshold
+00000d50: 290c 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
+00000d60: 0072 2000 0000 da06 7061 7261 6d73 725b  .r .....paramsr[
+00000d70: 0000 0072 0300 0000 7202 0000 0072 4500  ...r....r....rE.
+00000d80: 0000 7224 0000 0072 2200 0000 725c 0000  ..r$...r"...r\..
+00000d90: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000da0: 720b 0000 0072 4600 0000 4300 0000 732a  r....rF...C...s*
+00000db0: 0000 000a 0204 0302 0102 0102 0102 0102  ................
+00000dc0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000dd0: 0102 0102 0102 0102 ef06 1318 0172 4600  .............rF.
+00000de0: 0000 4e29 0a72 2000 0000 da06 7479 7069  ..N).r .....typi
+00000df0: 6e67 7202 0000 0072 0300 0000 da14 7079  ngr....r......py
+00000e00: 6461 6e74 6963 2e64 6174 6163 6c61 7373  dantic.dataclass
+00000e10: 6573 7204 0000 0072 0500 0000 720c 0000  esr....r....r...
+00000e20: 0072 2500 0000 7246 0000 0072 0a00 0000  .r%...rF...r....
+00000e30: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
+00000e40: 083c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00000e50: 0000 0407 1002 0c03 0e04 0201 1013 0201  ................
+00000e60: 101d 0201                                ....
```

### Comparing `bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-38.pyc` & `bluecast-0.8/bluecast/config/__pycache__/training_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 29 15:32:18 2023 UTC, .py size: 2873 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 02a4 9d64 390b 0000  U..........d9...
+00000000: 6f0d 0d0a 0000 0000 e7a0 a364 740b 0000  o..........dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 6505 4700  d.d...d...Z.e.G.
 00000060: 6406 6407 8400 6407 8302 8301 5a07 6505  d.d...d.....Z.e.
 00000070: 4700 6408 6409 8400 6409 8302 8301 5a08  G.d.d...d.....Z.
@@ -41,186 +41,197 @@
 00000280: da04 4469 6374 da08 4f70 7469 6f6e 616c  ..Dict..Optional
 00000290: 2901 da09 6461 7461 636c 6173 7363 0000  )...dataclassc..
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 000002b0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
 000002c0: 005a 0264 015a 0364 0253 0029 03da 0643  .Z.d.Z.d.S.)...C
 000002d0: 6f6e 6669 6754 4e29 04da 085f 5f6e 616d  onfigTN)...__nam
 000002e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 1761  .__qualname__..a
+000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5f5a 1761  .__qualname__Z.a
 00000300: 7262 6974 7261 7279 5f74 7970 6573 5f61  rbitrary_types_a
-00000310: 6c6c 6f77 6564 a900 720a 0000 0072 0a00  llowed..r....r..
+00000310: 6c6c 6f77 6564 a900 7209 0000 0072 0900  llowed..r....r..
 00000320: 0000 fa45 2f68 6f6d 652f 7468 6f6d 6173  ...E/home/thomas
 00000330: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
 00000340: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
 00000350: 636f 6e66 6967 2f74 7261 696e 696e 675f  config/training_
 00000360: 636f 6e66 6967 2e70 7972 0500 0000 0d00  config.pyr......
-00000370: 0000 7302 0000 0008 0172 0500 0000 6300  ..s......r....c.
-00000380: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000390: 0000 0040 0000 0073 ba00 0000 6500 5a01  ...@...s....e.Z.
-000003a0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
-000003b0: 6506 6403 3c00 6404 5a07 6508 6506 6405  e.d.<.d.Z.e.e.d.
-000003c0: 3c00 6406 5a09 6505 6506 6407 3c00 6408  <.d.Z.e.e.d.<.d.
-000003d0: 5a0a 6505 6506 6409 3c00 640a 5a0b 6505  Z.e.e.d.<.d.Z.e.
-000003e0: 6506 640b 3c00 6402 5a0c 6505 6506 640c  e.d.<.d.Z.e.e.d.
-000003f0: 3c00 6404 5a0d 6508 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
-00000400: 5a0e 6508 6506 640f 3c00 6404 5a0f 6508  Z.e.e.d.<.d.Z.e.
-00000410: 6506 6410 3c00 6411 5a10 6511 6506 6412  e.d.<.d.Z.e.e.d.
-00000420: 3c00 6404 5a12 6508 6506 6413 3c00 6404  <.d.Z.e.e.d.<.d.
-00000430: 5a13 6508 6506 6414 3c00 6415 5a14 6505  Z.e.e.d.<.d.Z.e.
-00000440: 6506 6416 3c00 640e 5a15 6508 6506 6417  e.d.<.d.Z.e.e.d.
-00000450: 3c00 6418 5300 2919 da0e 5472 6169 6e69  <.d.S.)...Traini
-00000460: 6e67 436f 6e66 6967 7a23 4465 6669 6e65  ngConfigz#Define
-00000470: 2067 656e 6572 616c 2074 7261 696e 696e   general trainin
-00000480: 6720 7061 7261 6d65 7465 7273 2ee9 0a00  g parameters....
-00000490: 0000 da13 676c 6f62 616c 5f72 616e 646f  ....global_rando
-000004a0: 6d5f 7374 6174 6554 da17 7368 7566 666c  m_stateT..shuffl
-000004b0: 655f 6475 7269 6e67 5f74 7261 696e 696e  e_during_trainin
-000004c0: 67e9 6400 0000 da1c 6879 7065 7270 6172  g.d.....hyperpar
-000004d0: 616d 6574 6572 5f74 756e 696e 675f 726f  ameter_tuning_ro
-000004e0: 756e 6473 6910 0e00 00da 2668 7970 6572  undsi.....&hyper
-000004f0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
-00000500: 5f6d 6178 5f72 756e 7469 6d65 5f73 6563  _max_runtime_sec
-00000510: 73e9 0100 0000 da14 6879 7065 7274 756e  s.......hypertun
-00000520: 696e 675f 6376 5f66 6f6c 6473 da15 6561  ing_cv_folds..ea
-00000530: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
-00000540: 6e64 73da 0e61 7574 6f74 756e 655f 6d6f  nds..autotune_mo
-00000550: 6465 6c46 da18 656e 6162 6c65 5f66 6561  delF..enable_fea
-00000560: 7475 7265 5f73 656c 6563 7469 6f6e da15  ture_selection..
-00000570: 6361 6c63 756c 6174 655f 7368 6170 5f76  calculate_shap_v
-00000580: 616c 7565 73e7 9a99 9999 9999 e93f da0a  alues........?..
-00000590: 7472 6169 6e5f 7369 7a65 da14 7472 6169  train_size..trai
-000005a0: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
-000005b0: da1d 7573 655f 6675 6c6c 5f64 6174 615f  ..use_full_data_
-000005c0: 666f 725f 6669 6e61 6c5f 6d6f 6465 6ce9  for_final_model.
-000005d0: 0500 0000 da16 6d69 6e5f 6665 6174 7572  ......min_featur
-000005e0: 6573 5f74 6f5f 7365 6c65 6374 da1d 6361  es_to_select..ca
-000005f0: 745f 656e 636f 6469 6e67 5f76 6961 5f6d  t_encoding_via_m
-00000600: 6c5f 616c 676f 7269 7468 6d4e 2916 7206  l_algorithmN).r.
-00000610: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
-00000620: 5f64 6f63 5f5f 720e 0000 00da 0369 6e74  _doc__r......int
-00000630: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000640: 5f72 0f00 0000 da04 626f 6f6c 7211 0000  _r......boolr...
-00000650: 0072 1200 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000660: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000670: 1a00 0000 da05 666c 6f61 7472 1b00 0000  ......floatr....
-00000680: 721c 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000690: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-000006a0: 0000 0072 0c00 0000 1100 0000 731e 0000  ...r........s...
-000006b0: 000a 0204 020c 010c 010c 010c 010c 010c  ................
-000006c0: 010c 010c 010c 010c 010c 010c 010c 0172  ...............r
-000006d0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000006e0: 0000 0000 0003 0000 0040 0000 0073 1a01  .........@...s..
-000006f0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000700: 6402 5a04 6505 6506 6403 3c00 6404 5a07  d.Z.e.e.d.<.d.Z.
-00000710: 6505 6506 6405 3c00 6406 5a08 6509 6506  e.e.d.<.d.Z.e.e.
-00000720: 6407 3c00 6408 5a0a 6509 6506 6409 3c00  d.<.d.Z.e.e.d.<.
-00000730: 6406 5a0b 6509 6506 640a 3c00 6408 5a0c  d.Z.e.e.d.<.d.Z.
-00000740: 6509 6506 640b 3c00 6402 5a0d 6505 6506  e.e.d.<.d.Z.e.e.
-00000750: 640c 3c00 640d 5a0e 6505 6506 640e 3c00  d.<.d.Z.e.e.d.<.
-00000760: 640f 5a0f 6509 6506 6410 3c00 6411 5a10  d.Z.e.e.d.<.d.Z.
-00000770: 6509 6506 6412 3c00 640f 5a11 6509 6506  e.e.d.<.d.Z.e.e.
-00000780: 6413 3c00 6411 5a12 6509 6506 6414 3c00  d.<.d.Z.e.e.d.<.
-00000790: 640f 5a13 6509 6506 6415 3c00 6411 5a14  d.Z.e.e.d.<.d.Z.
-000007a0: 6509 6506 6416 3c00 6406 5a15 6509 6506  e.e.d.<.d.Z.e.e.
-000007b0: 6417 3c00 6408 5a16 6509 6506 6418 3c00  d.<.d.Z.e.e.d.<.
-000007c0: 6419 5a17 6509 6506 641a 3c00 6402 5a18  d.Z.e.e.d.<.d.Z.
-000007d0: 6505 6506 641b 3c00 641c 5a19 6505 6506  e.e.d.<.d.Z.e.e.
-000007e0: 641d 3c00 641e 5a1a 6505 6506 641f 3c00  d.<.d.Z.e.e.d.<.
-000007f0: 6420 5a1b 651c 6506 6421 3c00 6422 5a1d  d Z.e.e.d!<.d"Z.
-00000800: 651c 6506 6423 3c00 6424 5300 2925 da17  e.e.d#<.d$S.)%..
-00000810: 5867 626f 6f73 7454 756e 6550 6172 616d  XgboostTuneParam
-00000820: 7343 6f6e 6669 677a 2a44 6566 696e 6520  sConfigz*Define 
-00000830: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
-00000840: 756e 696e 6720 7365 6172 6368 2073 7061  uning search spa
-00000850: 6365 2ee9 0200 0000 da0d 6d61 785f 6465  ce........max_de
-00000860: 7074 685f 6d69 6ee9 0600 0000 da0d 6d61  pth_min.......ma
-00000870: 785f 6465 7074 685f 6d61 7867 0000 0000  x_depth_maxg....
-00000880: 0000 0000 da09 616c 7068 615f 6d69 6e67  ......alpha_ming
-00000890: 0000 0000 0000 2440 da09 616c 7068 615f  ......$@..alpha_
-000008a0: 6d61 78da 0a6c 616d 6264 615f 6d69 6eda  max..lambda_min.
-000008b0: 0a6c 616d 6264 615f 6d61 78da 0e6e 756d  .lambda_max..num
-000008c0: 5f6c 6561 7665 735f 6d69 6ee9 4000 0000  _leaves_min.@...
-000008d0: da0e 6e75 6d5f 6c65 6176 6573 5f6d 6178  ..num_leaves_max
-000008e0: 6733 3333 3333 33d3 3fda 0e73 7562 5f73  g333333.?..sub_s
-000008f0: 616d 706c 655f 6d69 6e67 0000 0000 0000  ample_ming......
-00000900: f03f da0e 7375 625f 7361 6d70 6c65 5f6d  .?..sub_sample_m
-00000910: 6178 da16 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
-00000920: 795f 7472 6565 5f6d 696e da16 636f 6c5f  y_tree_min..col_
-00000930: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
-00000940: 6178 da17 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
-00000950: 795f 6c65 7665 6c5f 6d69 6eda 1763 6f6c  y_level_min..col
-00000960: 5f73 616d 706c 655f 6279 5f6c 6576 656c  _sample_by_level
-00000970: 5f6d 6178 da14 6d69 6e5f 6368 696c 645f  _max..min_child_
-00000980: 7765 6967 6874 5f6d 696e da14 6d69 6e5f  weight_min..min_
-00000990: 6368 696c 645f 7765 6967 6874 5f6d 6178  child_weight_max
-000009a0: e79a 9999 9999 99b9 3fda 0365 7461 da09  ........?..eta..
-000009b0: 7374 6570 735f 6d69 6e69 50c3 0000 da09  steps_miniP.....
-000009c0: 7374 6570 735f 6d61 7872 0100 0000 da0f  steps_maxr......
-000009d0: 6d6f 6465 6c5f 7665 7262 6f73 6974 79fa  model_verbosity.
-000009e0: 0e6d 756c 7469 3a73 6f66 7470 726f 62da  .multi:softprob.
-000009f0: 0f6d 6f64 656c 5f6f 626a 6563 7469 7665  .model_objective
-00000a00: da08 6d6c 6f67 6c6f 7373 da11 6d6f 6465  ..mlogloss..mode
-00000a10: 6c5f 6576 616c 5f6d 6574 7269 634e 291e  l_eval_metricN).
-00000a20: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00000a30: 2000 0000 7227 0000 0072 2100 0000 7222   ...r'...r!...r"
-00000a40: 0000 0072 2900 0000 722a 0000 0072 2400  ...r)...r*...r$.
-00000a50: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00000a60: 0072 2e00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00000a70: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
-00000a80: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
-00000a90: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
-00000aa0: 0000 723d 0000 0072 3f00 0000 da03 7374  ..r=...r?.....st
-00000ab0: 7272 4100 0000 720a 0000 0072 0a00 0000  rrA...r....r....
-00000ac0: 720a 0000 0072 0b00 0000 7225 0000 0025  r....r....r%...%
-00000ad0: 0000 0073 2e00 0000 0a02 0402 0c01 0c01  ...s............
-00000ae0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000af0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000b00: 0c01 0c01 0c01 7225 0000 0063 0000 0000  ......r%...c....
-00000b10: 0000 0000 0000 0000 0000 0000 1200 0000  ................
-00000b20: 4000 0000 735e 0000 0065 005a 0164 005a  @...s^...e.Z.d.Z
-00000b30: 0255 0064 015a 0364 0264 0364 0464 0564  .U.d.Z.d.d.d.d.d
-00000b40: 0664 0764 0864 0864 0964 0a64 0a64 0a64  .d.d.d.d.d.d.d.d
-00000b50: 0a64 0b64 0864 0c64 0d64 0e9c 115a 0464  .d.d.d.d.d...Z.d
-00000b60: 0f5a 0565 0665 0765 0865 0966 0219 0019  .Z.e.e.e.e.f....
-00000b70: 0065 0a64 103c 0064 115a 0b65 0965 0a64  .e.d.<.d.Z.e.e.d
-00000b80: 123c 0064 0f53 0029 13da 1758 6762 6f6f  .<.d.S.)...Xgboo
-00000b90: 7374 4669 6e61 6c50 6172 616d 436f 6e66  stFinalParamConf
-00000ba0: 6967 7a1e 4465 6669 6e65 2066 696e 616c  igz.Define final
-00000bb0: 2068 7970 6572 2070 6172 616d 6574 6572   hyper parameter
-00000bc0: 732e 723e 0000 0072 4000 0000 7201 0000  s.r>...r@...r...
-00000bd0: 00da 0565 7861 6374 7226 0000 00e9 0300  ...exactr&......
-00000be0: 0000 7239 0000 00e9 1000 0000 7219 0000  ..r9........r...
-00000bf0: 0072 1000 0000 69e8 0300 0072 1300 0000  .r....i....r....
-00000c00: 2911 da09 6f62 6a65 6374 6976 65da 0b65  )...objective..e
-00000c10: 7661 6c5f 6d65 7472 6963 da07 7665 7262  val_metric..verb
-00000c20: 6f73 65da 0b74 7265 655f 6d65 7468 6f64  ose..tree_method
-00000c30: da09 6e75 6d5f 636c 6173 73da 096d 6178  ..num_class..max
-00000c40: 5f64 6570 7468 da05 616c 7068 61da 066c  _depth..alpha..l
-00000c50: 616d 6264 61da 0a6e 756d 5f6c 6561 7665  ambda..num_leave
-00000c60: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
-00000c70: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
-00000c80: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
-00000c90: 6cda 1063 6f6c 7361 6d70 6c65 5f62 796e  l..colsample_byn
-00000ca0: 6f64 65da 116d 696e 5f63 6869 6c64 5f73  ode..min_child_s
-00000cb0: 616d 706c 6573 723a 0000 00da 0573 7465  amplesr:.....ste
-00000cc0: 7073 da11 6e75 6d5f 7061 7261 6c6c 656c  ps..num_parallel
-00000cd0: 5f74 7265 654e da0d 7361 6d70 6c65 5f77  _treeN..sample_w
-00000ce0: 6569 6768 7467 0000 0000 0000 e03f da18  eightg.......?..
-00000cf0: 636c 6173 7369 6669 6361 7469 6f6e 5f74  classification_t
-00000d00: 6872 6573 686f 6c64 290c 7206 0000 0072  hreshold).r....r
-00000d10: 0700 0000 7208 0000 0072 2000 0000 da06  ....r....r .....
-00000d20: 7061 7261 6d73 7257 0000 0072 0300 0000  paramsrW...r....
-00000d30: 7202 0000 0072 4200 0000 7224 0000 0072  r....rB...r$...r
-00000d40: 2200 0000 7258 0000 0072 0a00 0000 720a  "...rX...r....r.
-00000d50: 0000 0072 0a00 0000 720b 0000 0072 4300  ...r....r....rC.
-00000d60: 0000 4100 0000 732a 0000 000a 0204 0302  ..A...s*........
-00000d70: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000d80: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000d90: ef06 1318 0172 4300 0000 4e29 0a72 2000  .....rC...N).r .
-00000da0: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
-00000db0: 0300 0000 da14 7079 6461 6e74 6963 2e64  ......pydantic.d
-00000dc0: 6174 6163 6c61 7373 6573 7204 0000 0072  ataclassesr....r
-00000dd0: 0500 0000 720c 0000 0072 2500 0000 7243  ....r....r%...rC
-00000de0: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
-00000df0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000e00: 3e01 0000 0073 1200 0000 0407 1002 0c03  >....s..........
-00000e10: 0e04 0201 1013 0201 101b 0201            ............
+00000370: 0000 7304 0000 0008 0008 0172 0500 0000  ..s........r....
+00000380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000390: 0003 0000 0040 0000 0073 ba00 0000 6500  .....@...s....e.
+000003a0: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
+000003b0: 6505 6506 6403 3c00 6404 5a07 6508 6506  e.e.d.<.d.Z.e.e.
+000003c0: 6405 3c00 6406 5a09 6505 6506 6407 3c00  d.<.d.Z.e.e.d.<.
+000003d0: 6408 5a0a 6505 6506 6409 3c00 640a 5a0b  d.Z.e.e.d.<.d.Z.
+000003e0: 6505 6506 640b 3c00 6402 5a0c 6505 6506  e.e.d.<.d.Z.e.e.
+000003f0: 640c 3c00 6404 5a0d 6508 6506 640d 3c00  d.<.d.Z.e.e.d.<.
+00000400: 640e 5a0e 6508 6506 640f 3c00 6404 5a0f  d.Z.e.e.d.<.d.Z.
+00000410: 6508 6506 6410 3c00 6411 5a10 6511 6506  e.e.d.<.d.Z.e.e.
+00000420: 6412 3c00 6404 5a12 6508 6506 6413 3c00  d.<.d.Z.e.e.d.<.
+00000430: 640e 5a13 6508 6506 6414 3c00 6415 5a14  d.Z.e.e.d.<.d.Z.
+00000440: 6505 6506 6416 3c00 640e 5a15 6508 6506  e.e.d.<.d.Z.e.e.
+00000450: 6417 3c00 6418 5300 2919 da0e 5472 6169  d.<.d.S.)...Trai
+00000460: 6e69 6e67 436f 6e66 6967 7a23 4465 6669  ningConfigz#Defi
+00000470: 6e65 2067 656e 6572 616c 2074 7261 696e  ne general train
+00000480: 696e 6720 7061 7261 6d65 7465 7273 2ee9  ing parameters..
+00000490: 0a00 0000 da13 676c 6f62 616c 5f72 616e  ......global_ran
+000004a0: 646f 6d5f 7374 6174 6554 da17 7368 7566  dom_stateT..shuf
+000004b0: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
+000004c0: 696e 67e9 6400 0000 da1c 6879 7065 7270  ing.d.....hyperp
+000004d0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
+000004e0: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
+000004f0: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
+00000500: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
+00000510: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
+00000520: 756e 696e 675f 6376 5f66 6f6c 6473 da15  uning_cv_folds..
+00000530: 6561 726c 795f 7374 6f70 7069 6e67 5f72  early_stopping_r
+00000540: 6f75 6e64 73da 0e61 7574 6f74 756e 655f  ounds..autotune_
+00000550: 6d6f 6465 6c46 da18 656e 6162 6c65 5f66  modelF..enable_f
+00000560: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
+00000570: da15 6361 6c63 756c 6174 655f 7368 6170  ..calculate_shap
+00000580: 5f76 616c 7565 73e7 9a99 9999 9999 e93f  _values........?
+00000590: da0a 7472 6169 6e5f 7369 7a65 da14 7472  ..train_size..tr
+000005a0: 6169 6e5f 7370 6c69 745f 7374 7261 7469  ain_split_strati
+000005b0: 6679 da1d 7573 655f 6675 6c6c 5f64 6174  fy..use_full_dat
+000005c0: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
+000005d0: 6ce9 0500 0000 da16 6d69 6e5f 6665 6174  l.......min_feat
+000005e0: 7572 6573 5f74 6f5f 7365 6c65 6374 da1d  ures_to_select..
+000005f0: 6361 745f 656e 636f 6469 6e67 5f76 6961  cat_encoding_via
+00000600: 5f6d 6c5f 616c 676f 7269 7468 6d4e 2916  _ml_algorithmN).
+00000610: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000620: 075f 5f64 6f63 5f5f 720d 0000 00da 0369  .__doc__r......i
+00000630: 6e74 da0f 5f5f 616e 6e6f 7461 7469 6f6e  nt..__annotation
+00000640: 735f 5f72 0e00 0000 da04 626f 6f6c 7210  s__r......boolr.
+00000650: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
+00000660: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000670: 0072 1900 0000 da05 666c 6f61 7472 1a00  .r......floatr..
+00000680: 0000 721b 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000690: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+000006a0: 720a 0000 0072 0b00 0000 1100 0000 7320  r....r........s 
+000006b0: 0000 000a 0004 020c 020c 010c 010c 010c  ................
+000006c0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+000006d0: 0110 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
+000006e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000006f0: 0073 3201 0000 6500 5a01 6400 5a02 5500  .s2...e.Z.d.Z.U.
+00000700: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
+00000710: 6404 5a07 6505 6506 6405 3c00 6406 5a08  d.Z.e.e.d.<.d.Z.
+00000720: 6509 6506 6407 3c00 6408 5a0a 6509 6506  e.e.d.<.d.Z.e.e.
+00000730: 6409 3c00 6406 5a0b 6509 6506 640a 3c00  d.<.d.Z.e.e.d.<.
+00000740: 6408 5a0c 6509 6506 640b 3c00 6402 5a0d  d.Z.e.e.d.<.d.Z.
+00000750: 6505 6506 640c 3c00 640d 5a0e 6505 6506  e.e.d.<.d.Z.e.e.
+00000760: 640e 3c00 640f 5a0f 6509 6506 6410 3c00  d.<.d.Z.e.e.d.<.
+00000770: 6411 5a10 6509 6506 6412 3c00 640f 5a11  d.Z.e.e.d.<.d.Z.
+00000780: 6509 6506 6413 3c00 6411 5a12 6509 6506  e.e.d.<.d.Z.e.e.
+00000790: 6414 3c00 640f 5a13 6509 6506 6415 3c00  d.<.d.Z.e.e.d.<.
+000007a0: 6411 5a14 6509 6506 6416 3c00 6406 5a15  d.Z.e.e.d.<.d.Z.
+000007b0: 6509 6506 6417 3c00 6408 5a16 6509 6506  e.e.d.<.d.Z.e.e.
+000007c0: 6418 3c00 6419 5a17 6509 6506 641a 3c00  d.<.d.Z.e.e.d.<.
+000007d0: 640f 5a18 6509 6506 641b 3c00 6402 5a19  d.Z.e.e.d.<.d.Z.
+000007e0: 6505 6506 641c 3c00 641d 5a1a 6505 6506  e.e.d.<.d.Z.e.e.
+000007f0: 641e 3c00 641f 5a1b 6505 6506 6420 3c00  d.<.d.Z.e.e.d <.
+00000800: 6421 5a1c 651d 6506 6422 3c00 6423 5a1e  d!Z.e.e.d"<.d#Z.
+00000810: 651d 6506 6424 3c00 6425 5a1f 651d 6506  e.e.d$<.d%Z.e.e.
+00000820: 6426 3c00 6427 5300 2928 da17 5867 626f  d&<.d'S.)(..Xgbo
+00000830: 6f73 7454 756e 6550 6172 616d 7343 6f6e  ostTuneParamsCon
+00000840: 6669 677a 2a44 6566 696e 6520 6879 7065  figz*Define hype
+00000850: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
+00000860: 6720 7365 6172 6368 2073 7061 6365 2ee9  g search space..
+00000870: 0200 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
+00000880: 6d69 6ee9 0600 0000 da0d 6d61 785f 6465  min.......max_de
+00000890: 7074 685f 6d61 7867 0000 0000 0000 0000  pth_maxg........
+000008a0: da09 616c 7068 615f 6d69 6e67 0000 0000  ..alpha_ming....
+000008b0: 0000 2440 da09 616c 7068 615f 6d61 78da  ..$@..alpha_max.
+000008c0: 0a6c 616d 6264 615f 6d69 6eda 0a6c 616d  .lambda_min..lam
+000008d0: 6264 615f 6d61 78da 0e6e 756d 5f6c 6561  bda_max..num_lea
+000008e0: 7665 735f 6d69 6ee9 4000 0000 da0e 6e75  ves_min.@.....nu
+000008f0: 6d5f 6c65 6176 6573 5f6d 6178 6733 3333  m_leaves_maxg333
+00000900: 3333 33d3 3fda 0e73 7562 5f73 616d 706c  333.?..sub_sampl
+00000910: 655f 6d69 6e67 0000 0000 0000 f03f da0e  e_ming.......?..
+00000920: 7375 625f 7361 6d70 6c65 5f6d 6178 da16  sub_sample_max..
+00000930: 636f 6c5f 7361 6d70 6c65 5f62 795f 7472  col_sample_by_tr
+00000940: 6565 5f6d 696e da16 636f 6c5f 7361 6d70  ee_min..col_samp
+00000950: 6c65 5f62 795f 7472 6565 5f6d 6178 da17  le_by_tree_max..
+00000960: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
+00000970: 7665 6c5f 6d69 6eda 1763 6f6c 5f73 616d  vel_min..col_sam
+00000980: 706c 655f 6279 5f6c 6576 656c 5f6d 6178  ple_by_level_max
+00000990: da14 6d69 6e5f 6368 696c 645f 7765 6967  ..min_child_weig
+000009a0: 6874 5f6d 696e da14 6d69 6e5f 6368 696c  ht_min..min_chil
+000009b0: 645f 7765 6967 6874 5f6d 6178 67fc a9f1  d_weight_maxg...
+000009c0: d24d 6250 3fda 0765 7461 5f6d 696e da07  .MbP?..eta_min..
+000009d0: 6574 615f 6d61 78da 0973 7465 7073 5f6d  eta_max..steps_m
+000009e0: 696e e9e8 0300 00da 0973 7465 7073 5f6d  in.......steps_m
+000009f0: 6178 7201 0000 00da 0f6d 6f64 656c 5f76  axr......model_v
+00000a00: 6572 626f 7369 7479 fa0e 6d75 6c74 693a  erbosity..multi:
+00000a10: 736f 6674 7072 6f62 da0f 6d6f 6465 6c5f  softprob..model_
+00000a20: 6f62 6a65 6374 6976 65da 086d 6c6f 676c  objective..mlogl
+00000a30: 6f73 73da 116d 6f64 656c 5f65 7661 6c5f  oss..model_eval_
+00000a40: 6d65 7472 6963 da06 6762 7472 6565 da07  metric..gbtree..
+00000a50: 626f 6f73 7465 724e 2920 7206 0000 0072  boosterN) r....r
+00000a60: 0700 0000 7208 0000 0072 1f00 0000 7226  ....r....r....r&
+00000a70: 0000 0072 2000 0000 7221 0000 0072 2800  ...r ...r!...r(.
+00000a80: 0000 7229 0000 0072 2300 0000 722a 0000  ..r)...r#...r*..
+00000a90: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000aa0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+00000ab0: 3200 0000 7233 0000 0072 3400 0000 7235  2...r3...r4...r5
+00000ac0: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
+00000ad0: 0000 7239 0000 0072 3a00 0000 723c 0000  ..r9...r:...r<..
+00000ae0: 0072 3d00 0000 723f 0000 00da 0373 7472  .r=...r?.....str
+00000af0: 7241 0000 0072 4300 0000 7209 0000 0072  rA...rC...r....r
+00000b00: 0900 0000 7209 0000 0072 0a00 0000 7224  ....r....r....r$
+00000b10: 0000 0025 0000 0073 3400 0000 0a00 0402  ...%...s4.......
+00000b20: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000b30: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000b40: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1001  ................
+00000b50: 7224 0000 0063 0000 0000 0000 0000 0000  r$...c..........
+00000b60: 0000 0000 0000 0400 0000 4000 0000 73a0  ..........@...s.
+00000b70: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00000b80: 0369 0064 0264 0393 0164 0464 0593 0164  .i.d.d...d.d...d
+00000b90: 0664 0793 0164 0864 0993 0164 0a64 0b93  .d...d.d...d.d..
+00000ba0: 0164 0c64 0d93 0164 0e64 0f93 0164 1064  .d.d...d.d...d.d
+00000bb0: 0f93 0164 1164 1293 0164 1364 1493 0164  ...d.d...d.d...d
+00000bc0: 1564 1493 0164 1664 1493 0164 1764 1493  .d...d.d...d.d..
+00000bd0: 0164 1864 1993 0164 1a64 0f93 0164 1b64  .d.d...d.d...d.d
+00000be0: 1c93 0164 1d64 1e93 015a 0464 1f5a 0565  ...d.d...Z.d.Z.e
+00000bf0: 0665 0765 0865 0966 0219 0019 0065 0a64  .e.e.e.f.....e.d
+00000c00: 203c 0064 215a 0b65 0965 0a64 223c 0064   <.d!Z.e.e.d"<.d
+00000c10: 1f53 0029 23da 1758 6762 6f6f 7374 4669  .S.)#..XgboostFi
+00000c20: 6e61 6c50 6172 616d 436f 6e66 6967 7a1e  nalParamConfigz.
+00000c30: 4465 6669 6e65 2066 696e 616c 2068 7970  Define final hyp
+00000c40: 6572 2070 6172 616d 6574 6572 732e da09  er parameters...
+00000c50: 6f62 6a65 6374 6976 6572 3e00 0000 da0b  objectiver>.....
+00000c60: 6576 616c 5f6d 6574 7269 6372 4000 0000  eval_metricr@...
+00000c70: da07 7665 7262 6f73 6572 0100 0000 da0b  ..verboser......
+00000c80: 7472 6565 5f6d 6574 686f 64da 0565 7861  tree_method..exa
+00000c90: 6374 da09 6e75 6d5f 636c 6173 7372 2500  ct..num_classr%.
+00000ca0: 0000 da09 6d61 785f 6465 7074 68e9 0300  ....max_depth...
+00000cb0: 0000 da05 616c 7068 6167 9a99 9999 9999  ....alphag......
+00000cc0: b93f da06 6c61 6d62 6461 da0a 6e75 6d5f  .?..lambda..num_
+00000cd0: 6c65 6176 6573 e910 0000 00da 0973 7562  leaves.......sub
+00000ce0: 7361 6d70 6c65 7218 0000 00da 1063 6f6c  sampler......col
+00000cf0: 7361 6d70 6c65 5f62 7974 7265 65da 1163  sample_bytree..c
+00000d00: 6f6c 7361 6d70 6c65 5f62 796c 6576 656c  olsample_bylevel
+00000d10: da10 636f 6c73 616d 706c 655f 6279 6e6f  ..colsample_byno
+00000d20: 6465 da11 6d69 6e5f 6368 696c 645f 7361  de..min_child_sa
+00000d30: 6d70 6c65 7372 0f00 0000 da03 6574 61da  mplesr......eta.
+00000d40: 0573 7465 7073 723b 0000 00da 116e 756d  .stepsr;.....num
+00000d50: 5f70 6172 616c 6c65 6c5f 7472 6565 7212  _parallel_treer.
+00000d60: 0000 004e da0d 7361 6d70 6c65 5f77 6569  ...N..sample_wei
+00000d70: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
+00000d80: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
+00000d90: 6573 686f 6c64 290c 7206 0000 0072 0700  eshold).r....r..
+00000da0: 0000 7208 0000 0072 1f00 0000 da06 7061  ..r....r......pa
+00000db0: 7261 6d73 725a 0000 0072 0300 0000 7202  ramsrZ...r....r.
+00000dc0: 0000 0072 4400 0000 7223 0000 0072 2100  ...rD...r#...r!.
+00000dd0: 0000 725b 0000 0072 0900 0000 7209 0000  ..r[...r....r...
+00000de0: 0072 0900 0000 720a 0000 0072 4500 0000  .r....r....rE...
+00000df0: 4300 0000 734e 0000 000a 0004 0202 0204  C...sN..........
+00000e00: 0102 ff04 0202 fe04 0302 fd04 0402 fc04  ................
+00000e10: 0502 fb04 0602 fa04 0702 f904 0802 f804  ................
+00000e20: 0902 f704 0a02 f604 0b02 f504 0c02 f404  ................
+00000e30: 0d02 f304 0e02 f204 0f02 f104 1002 f004  ................
+00000e40: 1104 ef18 1310 0172 4500 0000 4e29 0a72  .......rE...N).r
+00000e50: 1f00 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
+00000e60: 0072 0300 0000 5a14 7079 6461 6e74 6963  .r....Z.pydantic
+00000e70: 2e64 6174 6163 6c61 7373 6573 7204 0000  .dataclassesr...
+00000e80: 0072 0500 0000 720b 0000 0072 2400 0000  .r....r....r$...
+00000e90: 7245 0000 0072 0900 0000 7209 0000 0072  rE...r....r....r
+00000ea0: 0900 0000 720a 0000 00da 083c 6d6f 6475  ....r......<modu
+00000eb0: 6c65 3e01 0000 0073 1400 0000 0400 1007  le>....s........
+00000ec0: 0c02 0e03 0204 1001 0213 1001 021d 1401  ................
```

### Comparing `bluecast-0.7/bluecast/eda/__pycache__/analyse.cpython-310.pyc` & `bluecast-0.8/bluecast/eda/__pycache__/analyse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 10:32:55 2023 UTC, .py size: 3708 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d75d 9d64 7c0e 0000  o........].d|...
+00000000: 6f0d 0d0a 0000 0000 9874 9e64 7c0e 0000  o........t.d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 5a04 6400 6401 6c05 5a06 6400 6401 6c07  Z.d.d.l.Z.d.d.l.
 00000050: 5a08 6402 6506 6a09 6403 650a 6404 6401  Z.d.e.j.d.e.d.d.
 00000060: 6606 6405 6406 8404 5a0b 6402 6506 6a09  f.d.d...Z.d.e.j.
 00000070: 6403 650a 6404 6401 6606 6407 6408 8404  d.e.d.d.f.d.d...
```

### Comparing `bluecast-0.7/bluecast/eda/analyse.py` & `bluecast-0.8/bluecast/eda/analyse.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc` & `bluecast-0.8/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-0.8/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/eval_metrics.py` & `bluecast-0.8/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/evaluation/shap_values.py` & `bluecast-0.8/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-0.8/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/general_utils/general_utils.py` & `bluecast-0.8/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-0.8/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 10:56:32 2023 UTC, .py size: 14974 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6063 9d64 7e3a 0000  o.......`c.d~:..
+00000000: 6f0d 0d0a 0000 0000 2ac8 a264 6338 0000  o.......*..dc8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -228,354 +228,341 @@
 00000e30: 0e04 0e01 0802 0a01 0401 0201 0201 0201  ................
 00000e40: 0601 08fc 0407 0201 0201 0601 06fd 0406  ................
 00000e50: 0201 0201 0601 06fd 1005 0c02 0401 0601  ................
 00000e60: 0201 0a01 0601 0201 0afb 0408 0601 0201  ................
 00000e70: 0a01 0601 0201 08fb 0807 0601 7a10 5867  ............z.Xg
 00000e80: 626f 6f73 744d 6f64 656c 2e66 6974 6305  boostModel.fitc.
 00000e90: 0000 0000 0000 0000 0000 000b 0000 000a  ................
-00000ea0: 0000 0003 0000 0073 e801 0000 7400 7401  .......s....t.t.
+00000ea0: 0000 0003 0000 0073 d201 0000 7400 7401  .......s....t.t.
 00000eb0: a002 a100 9b00 6401 9d02 8301 0100 8801  ......d.........
 00000ec0: 6a03 720f 8801 6a04 7313 7405 6402 8301  j.r...j.s.t.d...
 00000ed0: 8201 7406 6a07 7c02 8804 8801 6a04 6a08  ..t.j.|.....j.j.
 00000ee0: 6403 8d03 8900 7409 8300 8902 8801 a00a  d.....t.........
 00000ef0: a100 0100 8801 6a03 722d 8801 6a04 722d  ......j.r-..j.r-
 00000f00: 8801 6a0b 7331 7405 6404 8301 8201 8700  ..j.s1t.d.......
 00000f10: 8701 8702 8703 8704 8705 6606 6405 6406  ..........f.d.d.
 00000f20: 8408 7d05 6407 7d06 740c 6a0d 6a0e 6408  ..}.d.}.t.j.j.d.
 00000f30: 8801 6a04 6a0f 6409 8d02 7d07 740c 6a10  ..j.j.d...}.t.j.
 00000f40: 640a 7c07 7c06 9b00 640b 9d02 640c 8d03  d.|.|...d...d...
 00000f50: 7d08 7c08 6a11 7c05 8801 6a04 6a12 8801  }.|.j.|...j.j...
-00000f60: 6a04 6a13 6408 6408 640d 8d05 0100 7a16  j.j.d.d.d.....z.
+00000f60: 6a04 6a13 640d 640d 640e 8d05 0100 7a16  j.j.d.d.d.....z.
 00000f70: 740c 6a14 a015 7c08 a101 7d09 7c09 a016  t.j...|...}.|...
 00000f80: a100 0100 740c 6a14 a017 7c08 a101 7d09  ....t.j...|...}.
 00000f90: 7c09 a016 a100 0100 5700 6e0c 0400 7418  |.......W.n...t.
 00000fa0: 7419 7405 6603 7983 0100 0100 0100 5900  t.t.f.y.......Y.
-00000fb0: 6e01 7700 7c08 6a1a 6a1b 7d0a 6900 640e  n.w.|.j.j.}.i.d.
-00000fc0: 8801 6a0b 6a1c 9301 640f 8801 6a0b 6a1d  ..j.j...d...j.j.
-00000fd0: 9301 6410 8801 6a0b 6a1e 9301 6411 8802  ..d...j.j...d...
-00000fe0: 9301 6412 8805 a01f a100 9301 6413 7c0a  ..d.........d.|.
-00000ff0: 6413 1900 9301 6414 7c0a 6414 1900 9301  d.....d.|.d.....
-00001000: 6415 7c0a 6415 1900 9301 6416 7c0a 6416  d.|.d.....d.|.d.
-00001010: 1900 9301 6417 7c0a 6417 1900 9301 6418  ....d.|.d.....d.
-00001020: 7c0a 6418 1900 9301 6419 7c0a 6419 1900  |.d.....d.|.d...
-00001030: 9301 641a 7c0a 641a 1900 9301 641b 7c0a  ..d.|.d.....d.|.
-00001040: 641b 1900 9301 641c 7c0a 641c 1900 9301  d.....d.|.d.....
-00001050: 641d 8801 6a0b 6a20 9301 641e 7c0a 641e  d...j.j ..d.|.d.
-00001060: 1900 9301 641f 7c0a 641f 1900 6901 a501  ....d.|.d...i...
-00001070: 8801 6a03 5f1b 7421 6420 8801 6a03 6a1b  ..j._.t!d ..j.j.
-00001080: 8302 0100 7c0a 6421 1900 8801 6a03 5f22  ....|.d!....j._"
-00001090: 6422 5300 2923 7a7b 5475 6e65 2068 7970  d"S.)#z{Tune hyp
-000010a0: 6572 7061 7261 6d65 7465 7273 2e0a 0a20  erparameters... 
-000010b0: 2020 2020 2020 2041 6e20 616c 7465 726e         An altern
-000010c0: 6174 6976 6520 636f 6e66 6967 2063 616e  ative config can
-000010d0: 2062 6520 7072 6f76 6964 6564 2074 6f20   be provided to 
-000010e0: 6f76 6572 7772 6974 6520 7468 6520 6879  overwrite the hy
-000010f0: 7065 7270 6172 616d 6574 6572 2073 6561  perparameter sea
-00001100: 7263 6820 7370 6163 652e 0a20 2020 2020  rch space..     
-00001110: 2020 207a 2f3a 2053 7461 7274 2068 7970     z/: Start hyp
-00001120: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
-00001130: 6e67 206f 6620 5867 626f 6f73 7420 6d6f  ng of Xgboost mo
-00001140: 6465 6c2e 7227 0000 0072 2c00 0000 7a39  del.r'...r,...z9
-00001150: 4174 206c 6561 7374 206f 6e65 206f 6620  At least one of 
-00001160: 7468 6520 636f 6e66 6967 7320 6973 204e  the configs is N
-00001170: 6f6e 652c 2077 6869 6368 2069 7320 6e6f  one, which is no
-00001180: 7420 616c 6c6f 7765 6463 0100 0000 0000  t allowedc......
-00001190: 0000 0000 0000 0c00 0000 0a00 0000 1300  ................
-000011a0: 0000 7362 0200 0069 0064 0188 016a 006a  ..sb...i.d...j.j
-000011b0: 0193 0164 0288 016a 006a 0293 0164 0388  ...d...j.j...d..
-000011c0: 016a 006a 0393 0164 0488 0293 0164 0588  .j.j...d.....d..
-000011d0: 05a0 04a1 0093 0164 067c 00a0 0564 0688  .......d.|...d..
-000011e0: 016a 006a 0688 016a 006a 07a1 0393 0164  .j.j...j.j.....d
-000011f0: 077c 00a0 0864 0788 016a 006a 0988 016a  .|...d...j.j...j
-00001200: 006a 0aa1 0393 0164 087c 00a0 0864 0888  .j.....d.|...d..
-00001210: 016a 006a 0b88 016a 006a 0ca1 0393 0164  .j.j...j.j.....d
-00001220: 097c 00a0 0864 0988 016a 006a 0d88 016a  .|...d...j.j...j
-00001230: 006a 0ea1 0393 0164 0a7c 00a0 0564 0a88  .j.....d.|...d..
-00001240: 016a 006a 0f88 016a 006a 10a1 0393 0164  .j.j...j.j.....d
-00001250: 0b7c 00a0 0864 0b88 016a 006a 1188 016a  .|...d...j.j...j
-00001260: 006a 12a1 0393 0164 0c7c 00a0 0864 0c88  .j.....d.|...d..
-00001270: 016a 006a 1388 016a 006a 14a1 0393 0164  .j.j...j.j.....d
-00001280: 0d7c 00a0 0864 0d88 016a 006a 1588 016a  .|...d...j.j...j
-00001290: 006a 16a1 0393 0164 0e7c 00a0 0864 0e88  .j.....d.|...d..
-000012a0: 016a 006a 1788 016a 006a 18a1 0393 0164  .j.j...j.j.....d
-000012b0: 0f7c 00a0 0564 0f88 016a 006a 1988 016a  .|...d...j.j...j
-000012c0: 006a 1aa1 0393 0164 1088 016a 006a 1b93  .j.....d...j.j..
-000012d0: 0164 117c 00a0 0564 1188 016a 006a 1c88  .d.|...d...j.j..
-000012e0: 016a 006a 1da1 0393 0164 127c 00a0 0564  .j.j.....d.|...d
-000012f0: 1288 016a 006a 1e88 016a 006a 1fa1 0369  ...j.j...j.j...i
-00001300: 01a5 017d 017c 00a0 2064 1364 1464 1567  ...}.|.. d.d.d.g
-00001310: 02a1 027d 027c 0272 ca88 01a0 2188 05a1  ...}.|.r....!...
-00001320: 017d 0374 226a 2388 0388 057c 0388 016a  .}.t"j#....|...j
-00001330: 246a 2564 168d 047d 046e 0a74 226a 2388  $j%d...}.n.t"j#.
-00001340: 0388 0588 016a 246a 2564 178d 037d 0474  .....j$j%d...}.t
-00001350: 266a 27a0 287c 0064 18a1 027d 0588 016a  &j'.(|.d...}...j
-00001360: 246a 2964 196b 0290 0172 157c 0464 1a66  $j)d.k...r.|.d.f
-00001370: 0288 0064 1b66 0267 027d 0674 226a 2a7c  ...d.f.g.}.t"j*|
-00001380: 017c 047c 0164 1119 0088 016a 246a 2b7c  .|.|.d.....j$j+|
-00001390: 067c 0567 0188 016a 006a 0364 1c8d 077d  .|.g...j.j.d...}
-000013a0: 077c 07a0 2c88 00a1 017d 0874 2da0 2e64  .|..,....}.t-..d
-000013b0: 1d64 1e84 007c 0844 0083 01a1 017d 0974  .d...|.D.....}.t
-000013c0: 2f88 047c 0983 0264 1f14 007d 0a7c 0a53  /..|...d...}.|.S
-000013d0: 0074 226a 307c 017c 047c 0164 1119 0088  .t"j0|.|.|.d....
-000013e0: 016a 246a 2964 1488 016a 246a 317c 0567  .j$j)d...j$j1|.g
-000013f0: 0188 016a 246a 3264 208d 087d 0b7c 0b64  ...j$j2d ..}.|.d
-00001400: 2119 00a0 33a1 0053 0029 224e da09 6f62  !...3..S.)"N..ob
-00001410: 6a65 6374 6976 65da 0b65 7661 6c5f 6d65  jective..eval_me
-00001420: 7472 6963 da07 7665 7262 6f73 65da 0b74  tric..verbose..t
-00001430: 7265 655f 6d65 7468 6f64 da09 6e75 6d5f  ree_method..num_
-00001440: 636c 6173 73da 096d 6178 5f64 6570 7468  class..max_depth
-00001450: da05 616c 7068 61da 066c 616d 6264 61da  ..alpha..lambda.
-00001460: 0567 616d 6d61 da0a 6e75 6d5f 6c65 6176  .gamma..num_leav
-00001470: 6573 da09 7375 6273 616d 706c 65da 1063  es..subsample..c
-00001480: 6f6c 7361 6d70 6c65 5f62 7974 7265 65da  olsample_bytree.
-00001490: 1163 6f6c 7361 6d70 6c65 5f62 796c 6576  .colsample_bylev
-000014a0: 656c da10 636f 6c73 616d 706c 655f 6279  el..colsample_by
-000014b0: 6e6f 6465 da11 6d69 6e5f 6368 696c 645f  node..min_child_
-000014c0: 7361 6d70 6c65 73da 0365 7461 7230 0000  samples..etar0..
-000014d0: 00da 116e 756d 5f70 6172 616c 6c65 6c5f  ...num_parallel_
-000014e0: 7472 6565 723b 0000 0054 4672 2800 0000  treer;...TFr(...
-000014f0: 722c 0000 007a 0d74 6573 742d 6d6c 6f67  r,...z.test-mlog
-00001500: 6c6f 7373 722f 0000 0072 2d00 0000 722e  lossr/...r-...r.
-00001510: 0000 0029 0572 3100 0000 7232 0000 0072  ...).r1...r2...r
-00001520: 3300 0000 da09 6361 6c6c 6261 636b 73da  3.....callbacks.
-00001530: 0c76 6572 626f 7365 5f65 7661 6c63 0100  .verbose_evalc..
-00001540: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001550: 0000 5300 0000 f316 0000 0067 007c 005d  ..S........g.|.]
-00001560: 077d 0174 00a0 017c 01a1 0191 0271 0253  .}.t...|.....q.S
-00001570: 0072 1800 0000 a902 da02 6e70 da06 6172  .r........np..ar
-00001580: 676d 6178 a902 da02 2e30 da04 6c69 6e65  gmax.....0..line
-00001590: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-000015a0: 0a3c 6c69 7374 636f 6d70 3e0a 0100 00f3  .<listcomp>.....
-000015b0: 0200 0000 1600 7a3c 5867 626f 6f73 744d  ......z<XgboostM
-000015c0: 6f64 656c 2e61 7574 6f74 756e 652e 3c6c  odel.autotune.<l
-000015d0: 6f63 616c 733e 2e6f 626a 6563 7469 7665  ocals>.objective
-000015e0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000015f0: 6f6d 703e e9ff ffff ff29 0872 4000 0000  omp>.....).r@...
-00001600: da06 6474 7261 696e 7231 0000 00da 056e  ..dtrainr1.....n
-00001610: 666f 6c64 da09 6173 5f70 616e 6461 73da  fold..as_pandas.
-00001620: 0473 6565 6472 5600 0000 da07 7368 7566  .seedrV.....shuf
-00001630: 666c 657a 1274 6573 742d 6d6c 6f67 6c6f  flez.test-mloglo
-00001640: 7373 2d6d 6561 6e29 3472 1400 0000 da0f  ss-mean)4r......
-00001650: 6d6f 6465 6c5f 6f62 6a65 6374 6976 65da  model_objective.
-00001660: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
-00001670: 6963 da0f 6d6f 6465 6c5f 7665 7262 6f73  ic..model_verbos
-00001680: 6974 79da 076e 756e 6971 7565 5a0b 7375  ity..nuniqueZ.su
-00001690: 6767 6573 745f 696e 74da 0d6d 6178 5f64  ggest_int..max_d
-000016a0: 6570 7468 5f6d 696e da0d 6d61 785f 6465  epth_min..max_de
-000016b0: 7074 685f 6d61 785a 0d73 7567 6765 7374  pth_maxZ.suggest
-000016c0: 5f66 6c6f 6174 da09 616c 7068 615f 6d69  _float..alpha_mi
-000016d0: 6eda 0961 6c70 6861 5f6d 6178 da0a 6c61  n..alpha_max..la
-000016e0: 6d62 6461 5f6d 696e da0a 6c61 6d62 6461  mbda_min..lambda
-000016f0: 5f6d 6178 da09 6761 6d6d 615f 6d69 6eda  _max..gamma_min.
-00001700: 0967 616d 6d61 5f6d 6178 da0e 6e75 6d5f  .gamma_max..num_
-00001710: 6c65 6176 6573 5f6d 696e da0e 6e75 6d5f  leaves_min..num_
-00001720: 6c65 6176 6573 5f6d 6178 da0e 7375 625f  leaves_max..sub_
-00001730: 7361 6d70 6c65 5f6d 696e da0e 7375 625f  sample_min..sub_
-00001740: 7361 6d70 6c65 5f6d 6178 da16 636f 6c5f  sample_max..col_
-00001750: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
-00001760: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
-00001770: 795f 7472 6565 5f6d 6178 da17 636f 6c5f  y_tree_max..col_
-00001780: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
-00001790: 6d69 6eda 1763 6f6c 5f73 616d 706c 655f  min..col_sample_
-000017a0: 6279 5f6c 6576 656c 5f6d 6178 da16 636f  by_level_max..co
-000017b0: 6c5f 7361 6d70 6c65 5f62 795f 6e6f 6465  l_sample_by_node
-000017c0: 5f6d 696e da16 636f 6c5f 7361 6d70 6c65  _min..col_sample
-000017d0: 5f62 795f 6e6f 6465 5f6d 6178 da15 6d69  _by_node_max..mi
-000017e0: 6e5f 6368 696c 645f 7361 6d70 6c65 735f  n_child_samples_
-000017f0: 6d69 6eda 156d 696e 5f63 6869 6c64 5f73  min..min_child_s
-00001800: 616d 706c 6573 5f6d 6178 7254 0000 00da  amples_maxrT....
-00001810: 0973 7465 7073 5f6d 696e da09 7374 6570  .steps_min..step
-00001820: 735f 6d61 78da 156e 756d 5f70 6172 616c  s_max..num_paral
-00001830: 6c65 6c5f 7472 6565 5f6d 696e da15 6e75  lel_tree_min..nu
-00001840: 6d5f 7061 7261 6c6c 656c 5f74 7265 655f  m_parallel_tree_
-00001850: 6d61 785a 1373 7567 6765 7374 5f63 6174  maxZ.suggest_cat
-00001860: 6567 6f72 6963 616c 7221 0000 0072 3c00  egoricalr!...r<.
-00001870: 0000 723d 0000 0072 1300 0000 723e 0000  ..r=...r....r>..
-00001880: 00da 066f 7074 756e 615a 0b69 6e74 6567  ...optunaZ.integ
-00001890: 7261 7469 6f6e 5a16 5847 426f 6f73 7450  rationZ.XGBoostP
-000018a0: 7275 6e69 6e67 4361 6c6c 6261 636b 723f  runingCallbackr?
-000018b0: 0000 0072 2d00 0000 7232 0000 00da 0770  ...r-...r2.....p
-000018c0: 7265 6469 6374 725a 0000 00da 0761 7361  redictrZ.....asa
-000018d0: 7272 6179 7207 0000 00da 0263 76da 1367  rrayr......cv..g
-000018e0: 6c6f 6261 6c5f 7261 6e64 6f6d 5f73 7461  lobal_random_sta
-000018f0: 7465 da17 7368 7566 666c 655f 6475 7269  te..shuffle_duri
-00001900: 6e67 5f74 7261 696e 696e 67da 046d 6561  ng_training..mea
-00001910: 6e29 0cda 0574 7269 616c da05 7061 7261  n)...trial..para
-00001920: 6d72 3b00 0000 7220 0000 0072 4100 0000  mr;...r ...rA...
-00001930: 5a10 7072 756e 696e 675f 6361 6c6c 6261  Z.pruning_callba
-00001940: 636b 7243 0000 0072 1600 0000 da05 7072  ckrC...r......pr
-00001950: 6564 73da 0b70 7265 645f 6c61 6265 6c73  eds..pred_labels
-00001960: 5a07 6d61 7474 6865 77da 0672 6573 756c  Z.matthew..resul
-00001970: 74a9 0672 4200 0000 7217 0000 005a 0874  t..rB...r....Z.t
-00001980: 7261 696e 5f6f 6e72 2300 0000 7226 0000  rain_onr#...r&..
-00001990: 0072 2500 0000 7218 0000 0072 1900 0000  .r%...r....r....
-000019a0: 7245 0000 00ad 0000 0073 f000 0000 0201  rE.......s......
-000019b0: 0801 02ff 0802 02fe 0803 02fd 0404 02fc  ................
-000019c0: 0805 02fb 0606 0201 0601 0601 02fd 02fa  ................
-000019d0: 060b 0e01 02ff 02f5 060e 0e01 02ff 02f2  ................
-000019e0: 0611 0e01 02ff 02ef 0614 0201 0601 0601  ................
-000019f0: 02fd 02ec 0619 0201 0601 0601 02fd 02e7  ................
-00001a00: 061e 0201 0601 0601 02fd 02e2 0623 0201  .............#..
-00001a10: 0601 0601 02fd 02dd 0628 0201 0601 0601  .........(......
-00001a20: 02fd 02d8 062d 0201 0601 0601 02fd 02d3  .....-..........
-00001a30: 0832 02ce 0633 0e01 02ff 02cd 0636 0201  .2...3.......6..
-00001a40: 0601 0601 02fd 06ca 103c 0401 0a01 0401  .........<......
-00001a50: 0201 0201 0201 0601 08fc 0407 0201 0201  ................
-00001a60: 0601 06fd 0606 0401 04ff 0e04 1001 0401  ................
-00001a70: 0201 0201 0601 0601 0201 0401 0601 06f9  ................
-00001a80: 0a09 1401 0e01 0401 0402 0201 0201 0601  ................
-00001a90: 0602 0201 0601 0401 0601 06f7 0c0c 7a28  ..............z(
-00001aa0: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
-00001ab0: 6f74 756e 652e 3c6c 6f63 616c 733e 2e6f  otune.<locals>.o
-00001ac0: 626a 6563 7469 7665 da07 7867 626f 6f73  bjective..xgboos
-00001ad0: 7454 2902 5a0c 6d75 6c74 6976 6172 6961  tT).Z.multivaria
-00001ae0: 7465 7265 0000 00da 086d 696e 696d 697a  tere.....minimiz
-00001af0: 657a 0720 7475 6e69 6e67 2903 da09 6469  ez. tuning)...di
-00001b00: 7265 6374 696f 6eda 0773 616d 706c 6572  rection..sampler
-00001b10: 5a0a 7374 7564 795f 6e61 6d65 2904 da08  Z.study_name)...
-00001b20: 6e5f 7472 6961 6c73 da07 7469 6d65 6f75  n_trials..timeou
-00001b30: 745a 0e67 635f 6166 7465 725f 7472 6961  tZ.gc_after_tria
-00001b40: 6c5a 1173 686f 775f 7072 6f67 7265 7373  lZ.show_progress
-00001b50: 5f62 6172 7245 0000 0072 4600 0000 7247  _barrE...rF...rG
-00001b60: 0000 0072 4800 0000 7249 0000 0072 4a00  ...rH...rI...rJ.
-00001b70: 0000 724b 0000 0072 4c00 0000 724d 0000  ..rK...rL...rM..
-00001b80: 0072 4e00 0000 724f 0000 0072 5000 0000  .rN...rO...rP...
-00001b90: 7251 0000 0072 5200 0000 7253 0000 0072  rQ...rR...rS...r
-00001ba0: 5400 0000 7230 0000 0072 5500 0000 7a0d  T...r0...rU...z.
-00001bb0: 4265 7374 2070 6172 616d 733a 2072 3b00  Best params: r;.
-00001bc0: 0000 4e29 2372 0d00 0000 7202 0000 0072  ..N)#r....r....r
-00001bd0: 1e00 0000 7215 0000 0072 1300 0000 7234  ....r....r....r4
-00001be0: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
-00001bf0: 0000 720c 0000 0072 2200 0000 7214 0000  ..r....r"...r...
-00001c00: 0072 8300 0000 5a08 7361 6d70 6c65 7273  .r....Z.samplers
-00001c10: 5a0a 5450 4553 616d 706c 6572 7287 0000  Z.TPESamplerr...
-00001c20: 005a 0c63 7265 6174 655f 7374 7564 79da  .Z.create_study.
-00001c30: 086f 7074 696d 697a 65da 1c68 7970 6572  .optimize..hyper
-00001c40: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
-00001c50: 5f72 6f75 6e64 73da 2668 7970 6572 7061  _rounds.&hyperpa
-00001c60: 7261 6d65 7465 725f 7475 6e69 6e67 5f6d  rameter_tuning_m
-00001c70: 6178 5f72 756e 7469 6d65 5f73 6563 735a  ax_runtime_secsZ
-00001c80: 0d76 6973 7561 6c69 7a61 7469 6f6e 5a19  .visualizationZ.
-00001c90: 706c 6f74 5f6f 7074 696d 697a 6174 696f  plot_optimizatio
-00001ca0: 6e5f 6869 7374 6f72 79da 0473 686f 775a  n_history..showZ
-00001cb0: 1670 6c6f 745f 7061 7261 6d5f 696d 706f  .plot_param_impo
-00001cc0: 7274 616e 6365 73da 115a 6572 6f44 6976  rtances..ZeroDiv
-00001cd0: 6973 696f 6e45 7272 6f72 da0c 5275 6e74  isionError..Runt
-00001ce0: 696d 6545 7272 6f72 5a0a 6265 7374 5f74  imeErrorZ.best_t
-00001cf0: 7269 616c 7240 0000 0072 6700 0000 7268  rialr@...rg...rh
-00001d00: 0000 0072 6900 0000 726a 0000 0072 5400  ...ri...rj...rT.
-00001d10: 0000 7237 0000 0072 3b00 0000 290b 7217  ..r7...r;...).r.
-00001d20: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00001d30: 0000 7226 0000 0072 4500 0000 da09 616c  ..r&...rE.....al
-00001d40: 676f 7269 7468 6d72 9300 0000 5a05 7374  gorithmr....Z.st
-00001d50: 7564 79da 0366 6967 5a12 7867 626f 6f73  udy..figZ.xgboos
-00001d60: 745f 6265 7374 5f70 6172 616d 7218 0000  t_best_paramr...
-00001d70: 0072 8f00 0000 7219 0000 0072 3600 0000  .r....r....r6...
-00001d80: 8c00 0000 73ac 0000 0012 0b0c 0108 0104  ....s...........
-00001d90: 0202 0102 0106 0106 fd06 0508 0204 0302  ................
-00001da0: ff04 0202 fe04 0302 fd02 0502 0104 ff16  ................
-00001db0: 0404 6f06 0108 0106 ff04 0302 0102 0108  ..o.............
-00001dc0: 0106 fd04 0602 0106 0106 0102 0102 0106  ................
-00001dd0: fb02 070c 0108 010c 010c 0112 0104 0102  ................
-00001de0: ff08 0302 0108 0102 ff08 0202 fe08 0302  ................
-00001df0: fd04 0402 fc08 0502 fb04 0602 0102 ff02  ................
-00001e00: fa08 0902 f708 0a02 f608 0b02 f508 0c02  ................
-00001e10: f408 0d02 f308 0e02 f208 0f02 f108 1002  ................
-00001e20: f008 1102 ef08 1202 ee08 1302 ed08 140a  ................
-00001e30: ec0e 1610 017a 1558 6762 6f6f 7374 4d6f  .....z.XgboostMo
-00001e40: 6465 6c2e 6175 746f 7475 6e65 da02 6466  del.autotune..df
-00001e50: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-00001e60: 0004 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
-00001e70: 7401 a002 a100 9b00 6401 9d02 8301 0100  t.......d.......
-00001e80: 7c00 6a03 720f 7c00 6a04 7313 7405 6402  |.j.r.|.j.s.t.d.
-00001e90: 8301 8201 7406 6a07 7c01 7c00 6a04 6a08  ....t.j.|.|.j.j.
-00001ea0: 6403 8d02 7d02 7c00 6a09 7323 740a 6404  d...}.|.j.s#t.d.
-00001eb0: 8301 8201 7c00 6a0b 732a 740a 6405 8301  ....|.j.s*t.d...
-00001ec0: 8201 7c00 6a09 a00c 7c02 a101 7d03 7c00  ..|.j...|...}.|.
-00001ed0: 6a0d 6406 6b02 7246 740e a00f 6407 6408  j.d.k.rFt...d.d.
-00001ee0: 8400 7c03 4400 8301 a101 7d04 7c04 7c00  ..|.D.....}.|.|.
-00001ef0: 6a0b 6a10 6b04 7d05 6e0c 7c03 7d04 740e  j.j.k.}.n.|.}.t.
-00001f00: a00f 6409 6408 8400 7c03 4400 8301 a101  ..d.d...|.D.....
-00001f10: 7d05 7411 640a 8301 0100 7c04 7c05 6602  }.t.d.....|.|.f.
-00001f20: 5300 290b 7a17 5072 6564 6963 7420 6f6e  S.).z.Predict on
-00001f30: 2075 6e73 6565 6e20 6461 7461 2e7a 333a   unseen data.z3:
-00001f40: 2053 7461 7274 2070 7265 6469 6374 696e   Start predictin
-00001f50: 6720 6f6e 206e 6577 2064 6174 6120 7573  g on new data us
-00001f60: 696e 6720 5867 626f 6f73 7420 6d6f 6465  ing Xgboost mode
-00001f70: 6c2e 7227 0000 0029 0172 2b00 0000 7a20  l.r'...).r+...z 
-00001f80: 4e6f 2074 7261 696e 6564 206d 6f64 656c  No trained model
-00001f90: 2068 6173 2062 6565 6e20 666f 756e 642e   has been found.
-00001fa0: 7a2b 4e6f 206d 6f64 656c 2063 6f6e 6669  z+No model confi
-00001fb0: 6775 7261 7469 6f6e 2066 696c 6520 6861  guration file ha
-00001fc0: 7320 6265 656e 2066 6f75 6e64 2e72 1100  s been found.r..
-00001fd0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001fe0: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-00001ff0: 6700 7c00 5d06 7d01 7c01 6400 1900 9102  g.|.].}.|.d.....
-00002000: 7102 5300 2901 722f 0000 0072 1800 0000  q.S.).r/...r....
-00002010: 725c 0000 0072 1800 0000 7218 0000 0072  r\...r....r....r
-00002020: 1900 0000 725f 0000 0064 0100 0073 0200  ....r_...d...s..
-00002030: 0000 1400 7a28 5867 626f 6f73 744d 6f64  ....z(XgboostMod
-00002040: 656c 2e70 7265 6469 6374 2e3c 6c6f 6361  el.predict.<loca
-00002050: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
-00002060: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00002070: 0000 0053 0000 0072 5800 0000 7218 0000  ...S...rX...r...
-00002080: 0072 5900 0000 725c 0000 0072 1800 0000  .rY...r\...r....
-00002090: 7218 0000 0072 1900 0000 725f 0000 006a  r....r....r_...j
-000020a0: 0100 0072 6000 0000 7a13 4669 6e69 7368  ...r`...z.Finish
-000020b0: 6564 2070 7265 6469 6374 696e 6729 1272  ed predicting).r
-000020c0: 0d00 0000 7202 0000 0072 1e00 0000 7214  ....r....r....r.
-000020d0: 0000 0072 1300 0000 7234 0000 0072 3c00  ...r....r4...r<.
-000020e0: 0000 723d 0000 0072 3e00 0000 7216 0000  ..r=...r>...r...
-000020f0: 00da 0945 7863 6570 7469 6f6e 7215 0000  ...Exceptionr...
-00002100: 0072 8400 0000 7210 0000 0072 5a00 0000  .r....r....rZ...
-00002110: 7285 0000 00da 1863 6c61 7373 6966 6963  r......classific
-00002120: 6174 696f 6e5f 7468 7265 7368 6f6c 6472  ation_thresholdr
-00002130: 3700 0000 2906 7217 0000 0072 9e00 0000  7...).r....r....
-00002140: 7242 0000 005a 0d70 6172 7469 616c 5f70  rB...Z.partial_p
-00002150: 726f 6273 5a0f 7072 6564 6963 7465 645f  robsZ.predicted_
-00002160: 7072 6f62 73da 1170 7265 6469 6374 6564  probs..predicted
-00002170: 5f63 6c61 7373 6573 7218 0000 0072 1800  _classesr....r..
-00002180: 0000 7219 0000 0072 8400 0000 4f01 0000  ..r....r....O...
-00002190: 732c 0000 0002 020c 0104 ff0c 0308 0104  s,..............
-000021a0: 0202 0106 0106 fe06 0508 0106 0208 010c  ................
-000021b0: 020a 0114 010a 0204 ff04 0414 0108 0108  ................
-000021c0: 017a 1458 6762 6f6f 7374 4d6f 6465 6c2e  .z.XgboostModel.
-000021d0: 7072 6564 6963 7429 034e 4e4e 291a da08  predict).NNN)...
-000021e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000021f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00002200: 5f5f da07 5f5f 646f 635f 5f72 0400 0000  __..__doc__r....
-00002210: 7205 0000 0072 0900 0000 720b 0000 0072  r....r....r....r
-00002220: 0a00 0000 721a 0000 0072 3900 0000 da06  ....r....r9.....
-00002230: 5365 7269 6573 7203 0000 00da 0373 7472  Seriesr......str
-00002240: da05 666c 6f61 7472 2100 0000 7222 0000  ..floatr!...r"..
-00002250: 00da 0944 6174 6146 7261 6d65 723c 0000  ...DataFramer<..
-00002260: 00da 0742 6f6f 7374 6572 7244 0000 0072  ...BoosterrD...r
-00002270: 3600 0000 7206 0000 0072 5a00 0000 da07  6...r....rZ.....
-00002280: 6e64 6172 7261 7972 8400 0000 7218 0000  ndarrayr....r...
-00002290: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-000022a0: 720f 0000 001a 0000 0073 5000 0000 0800  r........sP.....
-000022b0: 0401 0205 0201 0201 04fb 0602 02fe 0603  ................
-000022c0: 02fd 0604 02fc 0605 0afb 1c0d 0808 0215  ................
-000022d0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
-000022e0: 0406 0afa 0245 0402 02fe 0403 02fd 0404  .....E..........
-000022f0: 02fc 0405 02fb 0206 0afa 007f 2444 720f  ............$Dr.
-00002300: 0000 0029 1c72 a500 0000 7202 0000 00da  ...).r....r.....
-00002310: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
-00002320: 0072 0500 0000 7206 0000 00da 056e 756d  .r....r......num
-00002330: 7079 725a 0000 0072 8300 0000 da06 7061  pyrZ...r......pa
-00002340: 6e64 6173 7239 0000 0072 9000 0000 723c  ndasr9...r....r<
-00002350: 0000 00da 0f73 6b6c 6561 726e 2e6d 6574  .....sklearn.met
-00002360: 7269 6373 7207 0000 00da 0d73 6b6c 6561  ricsr......sklea
-00002370: 726e 2e75 7469 6c73 7208 0000 00da 1f62  rn.utilsr......b
-00002380: 6c75 6563 6173 742e 636f 6e66 6967 2e74  luecast.config.t
-00002390: 7261 696e 696e 675f 636f 6e66 6967 7209  raining_configr.
-000023a0: 0000 0072 0a00 0000 720b 0000 00da 2462  ...r....r.....$b
-000023b0: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
-000023c0: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
-000023d0: 696c 7372 0c00 0000 720d 0000 00da 2262  ilsr....r....."b
-000023e0: 6c75 6563 6173 742e 6d6c 5f6d 6f64 656c  luecast.ml_model
-000023f0: 6c69 6e67 2e62 6173 655f 636c 6173 7365  ling.base_classe
-00002400: 7372 0e00 0000 720f 0000 0072 1800 0000  sr....r....r....
-00002410: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00002420: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
-00002430: 0000 0400 0c06 1801 0802 0801 0801 0801  ................
-00002440: 0c01 0c01 1402 1005 0c01 1403            ............
+00000fb0: 6e01 7700 7c08 6a1a 6a1b 7d0a 6900 640f  n.w.|.j.j.}.i.d.
+00000fc0: 8801 6a0b 6a1c 9301 6410 8801 6a0b 6a1d  ..j.j...d...j.j.
+00000fd0: 9301 6411 8801 6a0b 6a1e 9301 6412 8801  ..d...j.j...d...
+00000fe0: 6a0b 6a1f 9301 6413 8802 9301 6414 8805  j.j...d.....d...
+00000ff0: a020 a100 9301 6415 7c0a 6415 1900 9301  . ....d.|.d.....
+00001000: 6416 7c0a 6416 1900 9301 6417 7c0a 6417  d.|.d.....d.|.d.
+00001010: 1900 9301 6418 7c0a 6418 1900 9301 6419  ....d.|.d.....d.
+00001020: 7c0a 6419 1900 9301 641a 7c0a 641a 1900  |.d.....d.|.d...
+00001030: 9301 641b 7c0a 641b 1900 9301 641c 7c0a  ..d.|.d.....d.|.
+00001040: 641c 1900 9301 641d 7c0a 641d 1900 9301  d.....d.|.d.....
+00001050: 641e 7c0a 641e 1900 9301 8801 6a03 5f1b  d.|.d.......j._.
+00001060: 7421 641f 8801 6a03 6a1b 8302 0100 7c0a  t!d...j.j.....|.
+00001070: 6420 1900 8801 6a03 5f22 6421 5300 2922  d ....j._"d!S.)"
+00001080: 7a7b 5475 6e65 2068 7970 6572 7061 7261  z{Tune hyperpara
+00001090: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
+000010a0: 2041 6e20 616c 7465 726e 6174 6976 6520   An alternative 
+000010b0: 636f 6e66 6967 2063 616e 2062 6520 7072  config can be pr
+000010c0: 6f76 6964 6564 2074 6f20 6f76 6572 7772  ovided to overwr
+000010d0: 6974 6520 7468 6520 6879 7065 7270 6172  ite the hyperpar
+000010e0: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
+000010f0: 6163 652e 0a20 2020 2020 2020 207a 2f3a  ace..        z/:
+00001100: 2053 7461 7274 2068 7970 6572 7061 7261   Start hyperpara
+00001110: 6d65 7465 7220 7475 6e69 6e67 206f 6620  meter tuning of 
+00001120: 5867 626f 6f73 7420 6d6f 6465 6c2e 7227  Xgboost model.r'
+00001130: 0000 0072 2c00 0000 7a39 4174 206c 6561  ...r,...z9At lea
+00001140: 7374 206f 6e65 206f 6620 7468 6520 636f  st one of the co
+00001150: 6e66 6967 7320 6973 204e 6f6e 652c 2077  nfigs is None, w
+00001160: 6869 6368 2069 7320 6e6f 7420 616c 6c6f  hich is not allo
+00001170: 7765 6463 0100 0000 0000 0000 0000 0000  wedc............
+00001180: 0c00 0000 0a00 0000 1300 0000 733e 0200  ............s>..
+00001190: 0069 0064 0188 016a 006a 0193 0164 0288  .i.d...j.j...d..
+000011a0: 016a 006a 0293 0164 0388 016a 006a 0393  .j.j...d...j.j..
+000011b0: 0164 0488 016a 006a 0493 0164 0588 0293  .d...j.j...d....
+000011c0: 0164 0688 05a0 05a1 0093 0164 077c 00a0  .d.........d.|..
+000011d0: 0664 0788 016a 006a 0788 016a 006a 08a1  .d...j.j...j.j..
+000011e0: 0393 0164 087c 00a0 0964 0888 016a 006a  ...d.|...d...j.j
+000011f0: 0a88 016a 006a 0ba1 0393 0164 097c 00a0  ...j.j.....d.|..
+00001200: 0664 0988 016a 006a 0c88 016a 006a 0da1  .d...j.j...j.j..
+00001210: 0393 0164 0a7c 00a0 0664 0a88 016a 006a  ...d.|...d...j.j
+00001220: 0e88 016a 006a 0fa1 0393 0164 0b7c 00a0  ...j.j.....d.|..
+00001230: 0664 0b88 016a 006a 1088 016a 006a 11a1  .d...j.j...j.j..
+00001240: 0393 0164 0c7c 00a0 0964 0c88 016a 006a  ...d.|...d...j.j
+00001250: 1288 016a 006a 13a1 0393 0164 0d7c 00a0  ...j.j.....d.|..
+00001260: 0664 0d88 016a 006a 1488 016a 006a 15a1  .d...j.j...j.j..
+00001270: 0393 0164 0e7c 00a0 0664 0e88 016a 006a  ...d.|...d...j.j
+00001280: 1688 016a 006a 17a1 0393 0164 0f7c 00a0  ...j.j.....d.|..
+00001290: 0664 0f88 016a 006a 1888 016a 006a 19a1  .d...j.j...j.j..
+000012a0: 0393 0164 107c 00a0 0964 1088 016a 006a  ...d.|...d...j.j
+000012b0: 1a88 016a 006a 1ba1 0393 017d 017c 00a0  ...j.j.....}.|..
+000012c0: 1c64 1164 1264 1367 02a1 027d 027c 0272  .d.d.d.g...}.|.r
+000012d0: b188 01a0 1d88 05a1 017d 0374 1e6a 1f88  .........}.t.j..
+000012e0: 0388 057c 0388 016a 206a 2164 148d 047d  ...|...j j!d...}
+000012f0: 046e 0a74 1e6a 1f88 0388 0588 016a 206a  .n.t.j.......j j
+00001300: 2164 158d 037d 0474 226a 23a0 247c 0064  !d...}.t"j#.$|.d
+00001310: 16a1 027d 0588 016a 206a 2564 176b 0272  ...}...j j%d.k.r
+00001320: fb7c 0464 1866 0288 0064 1966 0267 027d  .|.d.f...d.f.g.}
+00001330: 0674 1e6a 267c 017c 047c 0164 1019 0088  .t.j&|.|.|.d....
+00001340: 016a 206a 277c 067c 0567 0188 016a 006a  .j j'|.|.g...j.j
+00001350: 0464 1a8d 077d 077c 07a0 2888 00a1 017d  .d...}.|..(....}
+00001360: 0874 29a0 2a64 1b64 1c84 007c 0844 0083  .t).*d.d...|.D..
+00001370: 01a1 017d 0974 2b88 047c 0983 0264 1d14  ...}.t+..|...d..
+00001380: 007d 0a7c 0a53 0074 1e6a 2c7c 017c 047c  .}.|.S.t.j,|.|.|
+00001390: 0164 1019 0088 016a 206a 2564 1288 016a  .d.....j j%d...j
+000013a0: 206a 2d7c 0567 0188 016a 206a 2e64 1e8d   j-|.g...j j.d..
+000013b0: 087d 0b7c 0b64 1f19 00a0 2fa1 007c 0b64  .}.|.d..../..|.d
+000013c0: 1f19 00a0 30a1 0064 2013 0017 0053 0029  ....0..d ....S.)
+000013d0: 214e da09 6f62 6a65 6374 6976 65da 0762  !N..objective..b
+000013e0: 6f6f 7374 6572 da0b 6576 616c 5f6d 6574  ooster..eval_met
+000013f0: 7269 63da 0776 6572 626f 7365 da0b 7472  ric..verbose..tr
+00001400: 6565 5f6d 6574 686f 64da 096e 756d 5f63  ee_method..num_c
+00001410: 6c61 7373 da03 6574 61da 096d 6178 5f64  lass..eta..max_d
+00001420: 6570 7468 da05 616c 7068 61da 066c 616d  epth..alpha..lam
+00001430: 6264 61da 106d 696e 5f63 6869 6c64 5f77  bda..min_child_w
+00001440: 6569 6768 74da 0a6e 756d 5f6c 6561 7665  eight..num_leave
+00001450: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
+00001460: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
+00001470: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
+00001480: 6c72 3000 0000 723b 0000 0054 4672 2800  lr0...r;...TFr(.
+00001490: 0000 722c 0000 007a 0d74 6573 742d 6d6c  ..r,...z.test-ml
+000014a0: 6f67 6c6f 7373 722f 0000 0072 2d00 0000  oglossr/...r-...
+000014b0: 722e 0000 0029 0572 3100 0000 7232 0000  r....).r1...r2..
+000014c0: 0072 3300 0000 da09 6361 6c6c 6261 636b  .r3.....callback
+000014d0: 73da 0c76 6572 626f 7365 5f65 7661 6c63  s..verbose_evalc
+000014e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000014f0: 0500 0000 5300 0000 f316 0000 0067 007c  ....S........g.|
+00001500: 005d 077d 0174 00a0 017c 01a1 0191 0271  .].}.t...|.....q
+00001510: 0253 0072 1800 0000 a902 da02 6e70 da06  .S.r........np..
+00001520: 6172 676d 6178 a902 da02 2e30 da04 6c69  argmax.....0..li
+00001530: 6e65 7218 0000 0072 1800 0000 7219 0000  ner....r....r...
+00001540: 00da 0a3c 6c69 7374 636f 6d70 3e00 0100  ...<listcomp>...
+00001550: 00f3 0200 0000 1600 7a3c 5867 626f 6f73  ........z<Xgboos
+00001560: 744d 6f64 656c 2e61 7574 6f74 756e 652e  tModel.autotune.
+00001570: 3c6c 6f63 616c 733e 2e6f 626a 6563 7469  <locals>.objecti
+00001580: 7665 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ve.<locals>.<lis
+00001590: 7463 6f6d 703e e9ff ffff ff29 0872 4000  tcomp>.....).r@.
+000015a0: 0000 da06 6474 7261 696e 7231 0000 00da  ....dtrainr1....
+000015b0: 056e 666f 6c64 da09 6173 5f70 616e 6461  .nfold..as_panda
+000015c0: 73da 0473 6565 6472 5400 0000 da07 7368  s..seedrT.....sh
+000015d0: 7566 666c 657a 1274 6573 742d 6d6c 6f67  ufflez.test-mlog
+000015e0: 6c6f 7373 2d6d 6561 6e67 6666 6666 6666  loss-meangffffff
+000015f0: e63f 2931 7214 0000 00da 0f6d 6f64 656c  .?)1r......model
+00001600: 5f6f 626a 6563 7469 7665 7246 0000 00da  _objectiverF....
+00001610: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
+00001620: 6963 da0f 6d6f 6465 6c5f 7665 7262 6f73  ic..model_verbos
+00001630: 6974 79da 076e 756e 6971 7565 5a0d 7375  ity..nuniqueZ.su
+00001640: 6767 6573 745f 666c 6f61 74da 0765 7461  ggest_float..eta
+00001650: 5f6d 696e da07 6574 615f 6d61 785a 0b73  _min..eta_maxZ.s
+00001660: 7567 6765 7374 5f69 6e74 da0d 6d61 785f  uggest_int..max_
+00001670: 6465 7074 685f 6d69 6eda 0d6d 6178 5f64  depth_min..max_d
+00001680: 6570 7468 5f6d 6178 da09 616c 7068 615f  epth_max..alpha_
+00001690: 6d69 6eda 0961 6c70 6861 5f6d 6178 da0a  min..alpha_max..
+000016a0: 6c61 6d62 6461 5f6d 696e da0a 6c61 6d62  lambda_min..lamb
+000016b0: 6461 5f6d 6178 da14 6d69 6e5f 6368 696c  da_max..min_chil
+000016c0: 645f 7765 6967 6874 5f6d 696e da14 6d69  d_weight_min..mi
+000016d0: 6e5f 6368 696c 645f 7765 6967 6874 5f6d  n_child_weight_m
+000016e0: 6178 da0e 6e75 6d5f 6c65 6176 6573 5f6d  ax..num_leaves_m
+000016f0: 696e da0e 6e75 6d5f 6c65 6176 6573 5f6d  in..num_leaves_m
+00001700: 6178 da0e 7375 625f 7361 6d70 6c65 5f6d  ax..sub_sample_m
+00001710: 696e da0e 7375 625f 7361 6d70 6c65 5f6d  in..sub_sample_m
+00001720: 6178 da16 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
+00001730: 795f 7472 6565 5f6d 696e da16 636f 6c5f  y_tree_min..col_
+00001740: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
+00001750: 6178 da17 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
+00001760: 795f 6c65 7665 6c5f 6d69 6eda 1763 6f6c  y_level_min..col
+00001770: 5f73 616d 706c 655f 6279 5f6c 6576 656c  _sample_by_level
+00001780: 5f6d 6178 da09 7374 6570 735f 6d69 6eda  _max..steps_min.
+00001790: 0973 7465 7073 5f6d 6178 5a13 7375 6767  .steps_maxZ.sugg
+000017a0: 6573 745f 6361 7465 676f 7269 6361 6c72  est_categoricalr
+000017b0: 2100 0000 723c 0000 0072 3d00 0000 7213  !...r<...r=...r.
+000017c0: 0000 0072 3e00 0000 da06 6f70 7475 6e61  ...r>.....optuna
+000017d0: 5a0b 696e 7465 6772 6174 696f 6e5a 1658  Z.integrationZ.X
+000017e0: 4742 6f6f 7374 5072 756e 696e 6743 616c  GBoostPruningCal
+000017f0: 6c62 6163 6b72 3f00 0000 722d 0000 0072  lbackr?...r-...r
+00001800: 3200 0000 da07 7072 6564 6963 7472 5800  2.....predictrX.
+00001810: 0000 da07 6173 6172 7261 7972 0700 0000  ....asarrayr....
+00001820: da02 6376 da13 676c 6f62 616c 5f72 616e  ..cv..global_ran
+00001830: 646f 6d5f 7374 6174 65da 1773 6875 6666  dom_state..shuff
+00001840: 6c65 5f64 7572 696e 675f 7472 6169 6e69  le_during_traini
+00001850: 6e67 da04 6d65 616e da03 7374 6429 0cda  ng..mean..std)..
+00001860: 0574 7269 616c da05 7061 7261 6d72 3b00  .trial..paramr;.
+00001870: 0000 7220 0000 0072 4100 0000 5a10 7072  ..r ...rA...Z.pr
+00001880: 756e 696e 675f 6361 6c6c 6261 636b 7243  uning_callbackrC
+00001890: 0000 0072 1600 0000 da05 7072 6564 73da  ...r......preds.
+000018a0: 0b70 7265 645f 6c61 6265 6c73 5a07 6d61  .pred_labelsZ.ma
+000018b0: 7474 6865 77da 0672 6573 756c 74a9 0672  tthew..result..r
+000018c0: 4200 0000 7217 0000 005a 0874 7261 696e  B...r....Z.train
+000018d0: 5f6f 6e72 2300 0000 7226 0000 0072 2500  _onr#...r&...r%.
+000018e0: 0000 7218 0000 0072 1900 0000 7245 0000  ..r....r....rE..
+000018f0: 00ad 0000 0073 dc00 0000 0201 0801 02ff  .....s..........
+00001900: 0802 02fe 0803 02fd 0804 02fc 0405 02fb  ................
+00001910: 0806 02fa 0607 0e01 02ff 02f9 060a 0201  ................
+00001920: 0601 0601 02fd 02f6 060f 0e01 02ff 02f1  ................
+00001930: 0612 0e01 02ff 02ee 0615 0201 0601 0601  ................
+00001940: 02fd 02eb 061a 0201 0601 0601 02fd 02e6  ................
+00001950: 061f 0201 0601 0601 02fd 02e1 0624 0201  .............$..
+00001960: 0601 0601 02fd 02dc 0629 0201 0601 0601  .........)......
+00001970: 02fd 02d7 062e 0e01 02ff 04d2 1032 0401  .............2..
+00001980: 0a01 0401 0201 0201 0201 0601 08fc 0407  ................
+00001990: 0201 0201 0601 06fd 0606 0401 04ff 0c04  ................
+000019a0: 1001 0401 0201 0201 0601 0601 0201 0401  ................
+000019b0: 0601 06f9 0a09 1401 0e01 0401 0402 0201  ................
+000019c0: 0201 0601 0602 0201 0601 0401 0601 06f7  ................
+000019d0: 0a0c 0e01 04ff 7a28 5867 626f 6f73 744d  ......z(XgboostM
+000019e0: 6f64 656c 2e61 7574 6f74 756e 652e 3c6c  odel.autotune.<l
+000019f0: 6f63 616c 733e 2e6f 626a 6563 7469 7665  ocals>.objective
+00001a00: da07 7867 626f 6f73 7446 2902 5a0c 6d75  ..xgboostF).Z.mu
+00001a10: 6c74 6976 6172 6961 7465 7263 0000 00da  ltivariaterc....
+00001a20: 086d 696e 696d 697a 657a 0720 7475 6e69  .minimizez. tuni
+00001a30: 6e67 2903 da09 6469 7265 6374 696f 6eda  ng)...direction.
+00001a40: 0773 616d 706c 6572 5a0a 7374 7564 795f  .samplerZ.study_
+00001a50: 6e61 6d65 5429 04da 086e 5f74 7269 616c  nameT)...n_trial
+00001a60: 73da 0774 696d 656f 7574 5a0e 6763 5f61  s..timeoutZ.gc_a
+00001a70: 6674 6572 5f74 7269 616c 5a11 7368 6f77  fter_trialZ.show
+00001a80: 5f70 726f 6772 6573 735f 6261 7272 4500  _progress_barrE.
+00001a90: 0000 7246 0000 0072 4700 0000 7248 0000  ..rF...rG...rH..
+00001aa0: 0072 4900 0000 724a 0000 0072 4c00 0000  .rI...rJ...rL...
+00001ab0: 724d 0000 0072 4e00 0000 7250 0000 0072  rM...rN...rP...r
+00001ac0: 5100 0000 7252 0000 0072 5300 0000 724f  Q...rR...rS...rO
+00001ad0: 0000 0072 4b00 0000 7230 0000 007a 0d42  ...rK...r0...z.B
+00001ae0: 6573 7420 7061 7261 6d73 3a20 723b 0000  est params: r;..
+00001af0: 004e 2923 720d 0000 0072 0200 0000 721e  .N)#r....r....r.
+00001b00: 0000 0072 1500 0000 7213 0000 0072 3400  ...r....r....r4.
+00001b10: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00001b20: 0072 0c00 0000 7222 0000 0072 1400 0000  .r....r"...r....
+00001b30: 727d 0000 005a 0873 616d 706c 6572 735a  r}...Z.samplersZ
+00001b40: 0a54 5045 5361 6d70 6c65 7272 8100 0000  .TPESamplerr....
+00001b50: 5a0c 6372 6561 7465 5f73 7475 6479 da08  Z.create_study..
+00001b60: 6f70 7469 6d69 7a65 da1c 6879 7065 7270  optimize..hyperp
+00001b70: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
+00001b80: 726f 756e 6473 da26 6879 7065 7270 6172  rounds.&hyperpar
+00001b90: 616d 6574 6572 5f74 756e 696e 675f 6d61  ameter_tuning_ma
+00001ba0: 785f 7275 6e74 696d 655f 7365 6373 5a0d  x_runtime_secsZ.
+00001bb0: 7669 7375 616c 697a 6174 696f 6e5a 1970  visualizationZ.p
+00001bc0: 6c6f 745f 6f70 7469 6d69 7a61 7469 6f6e  lot_optimization
+00001bd0: 5f68 6973 746f 7279 da04 7368 6f77 5a16  _history..showZ.
+00001be0: 706c 6f74 5f70 6172 616d 5f69 6d70 6f72  plot_param_impor
+00001bf0: 7461 6e63 6573 da11 5a65 726f 4469 7669  tances..ZeroDivi
+00001c00: 7369 6f6e 4572 726f 72da 0c52 756e 7469  sionError..Runti
+00001c10: 6d65 4572 726f 725a 0a62 6573 745f 7472  meErrorZ.best_tr
+00001c20: 6961 6c72 4000 0000 7265 0000 0072 4600  ialr@...re...rF.
+00001c30: 0000 7266 0000 0072 6700 0000 7268 0000  ..rf...rg...rh..
+00001c40: 0072 3700 0000 723b 0000 0029 0b72 1700  .r7...r;...).r..
+00001c50: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
+00001c60: 0072 2600 0000 7245 0000 00da 0961 6c67  .r&...rE.....alg
+00001c70: 6f72 6974 686d 728e 0000 005a 0573 7475  orithmr....Z.stu
+00001c80: 6479 da03 6669 675a 1278 6762 6f6f 7374  dy..figZ.xgboost
+00001c90: 5f62 6573 745f 7061 7261 6d72 1800 0000  _best_paramr....
+00001ca0: 728a 0000 0072 1900 0000 7236 0000 008c  r....r....r6....
+00001cb0: 0000 0073 a400 0000 120b 0c01 0801 0402  ...s............
+00001cc0: 0201 0201 0601 06fd 0605 0802 0403 02ff  ................
+00001cd0: 0402 02fe 0403 02fd 0205 0201 04ff 1604  ................
+00001ce0: 0467 0601 0801 06ff 0403 0201 0201 0801  .g..............
+00001cf0: 06fd 0406 0201 0601 0601 0201 0201 06fb  ................
+00001d00: 0207 0c01 0801 0c01 0c01 1201 0401 02ff  ................
+00001d10: 0803 0201 0801 02ff 0802 02fe 0803 02fd  ................
+00001d20: 0804 02fc 0405 02fb 0806 02fa 0407 0201  ................
+00001d30: 02ff 02f9 080a 02f6 080b 02f5 080c 02f4  ................
+00001d40: 080d 02f3 080e 02f2 080f 02f1 0810 02f0  ................
+00001d50: 0811 02ef 0812 08ee 0e14 1001 7a15 5867  ............z.Xg
+00001d60: 626f 6f73 744d 6f64 656c 2e61 7574 6f74  boostModel.autot
+00001d70: 756e 65da 0264 6663 0200 0000 0000 0000  une..dfc........
+00001d80: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
+00001d90: 73b4 0000 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
+00001da0: 019d 0283 0101 007c 006a 0372 0f7c 006a  .......|.j.r.|.j
+00001db0: 0473 1374 0564 0283 0182 0174 066a 077c  .s.t.d.....t.j.|
+00001dc0: 017c 006a 046a 0864 038d 027d 027c 006a  .|.j.j.d...}.|.j
+00001dd0: 0973 2374 0a64 0483 0182 017c 006a 0b73  .s#t.d.....|.j.s
+00001de0: 2a74 0a64 0583 0182 017c 006a 09a0 0c7c  *t.d.....|.j...|
+00001df0: 02a1 017d 037c 006a 0d64 066b 0272 4674  ...}.|.j.d.k.rFt
+00001e00: 0ea0 0f64 0764 0884 007c 0344 0083 01a1  ...d.d...|.D....
+00001e10: 017d 047c 047c 006a 0b6a 106b 047d 056e  .}.|.|.j.j.k.}.n
+00001e20: 0c7c 037d 0474 0ea0 0f64 0964 0884 007c  .|.}.t...d.d...|
+00001e30: 0344 0083 01a1 017d 0574 1164 0a83 0101  .D.....}.t.d....
+00001e40: 007c 047c 0566 0253 0029 0b7a 1750 7265  .|.|.f.S.).z.Pre
+00001e50: 6469 6374 206f 6e20 756e 7365 656e 2064  dict on unseen d
+00001e60: 6174 612e 7a33 3a20 5374 6172 7420 7072  ata.z3: Start pr
+00001e70: 6564 6963 7469 6e67 206f 6e20 6e65 7720  edicting on new 
+00001e80: 6461 7461 2075 7369 6e67 2058 6762 6f6f  data using Xgboo
+00001e90: 7374 206d 6f64 656c 2e72 2700 0000 2901  st model.r'...).
+00001ea0: 722b 0000 007a 204e 6f20 7472 6169 6e65  r+...z No traine
+00001eb0: 6420 6d6f 6465 6c20 6861 7320 6265 656e  d model has been
+00001ec0: 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f 6465   found.z+No mode
+00001ed0: 6c20 636f 6e66 6967 7572 6174 696f 6e20  l configuration 
+00001ee0: 6669 6c65 2068 6173 2062 6565 6e20 666f  file has been fo
+00001ef0: 756e 642e 7211 0000 0063 0100 0000 0000  und.r....c......
+00001f00: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00001f10: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
+00001f20: 0164 0019 0091 0271 0253 0029 0172 2f00  .d.....q.S.).r/.
+00001f30: 0000 7218 0000 0072 5a00 0000 7218 0000  ..r....rZ...r...
+00001f40: 0072 1800 0000 7219 0000 0072 5d00 0000  .r....r....r]...
+00001f50: 5a01 0000 7302 0000 0014 007a 2858 6762  Z...s......z(Xgb
+00001f60: 6f6f 7374 4d6f 6465 6c2e 7072 6564 6963  oostModel.predic
+00001f70: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
+00001f80: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
+00001f90: 0000 0200 0000 0500 0000 5300 0000 7256  ..........S...rV
+00001fa0: 0000 0072 1800 0000 7257 0000 0072 5a00  ...r....rW...rZ.
+00001fb0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001fc0: 0072 5d00 0000 6001 0000 725e 0000 007a  .r]...`...r^...z
+00001fd0: 1346 696e 6973 6865 6420 7072 6564 6963  .Finished predic
+00001fe0: 7469 6e67 2912 720d 0000 0072 0200 0000  ting).r....r....
+00001ff0: 721e 0000 0072 1400 0000 7213 0000 0072  r....r....r....r
+00002000: 3400 0000 723c 0000 0072 3d00 0000 723e  4...r<...r=...r>
+00002010: 0000 0072 1600 0000 da09 4578 6365 7074  ...r......Except
+00002020: 696f 6e72 1500 0000 727e 0000 0072 1000  ionr....r~...r..
+00002030: 0000 7258 0000 0072 7f00 0000 da18 636c  ..rX...r......cl
+00002040: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
+00002050: 6573 686f 6c64 7237 0000 0029 0672 1700  esholdr7...).r..
+00002060: 0000 7299 0000 0072 4200 0000 5a0d 7061  ..r....rB...Z.pa
+00002070: 7274 6961 6c5f 7072 6f62 735a 0f70 7265  rtial_probsZ.pre
+00002080: 6469 6374 6564 5f70 726f 6273 da11 7072  dicted_probs..pr
+00002090: 6564 6963 7465 645f 636c 6173 7365 7372  edicted_classesr
+000020a0: 1800 0000 7218 0000 0072 1900 0000 727e  ....r....r....r~
+000020b0: 0000 0045 0100 0073 2c00 0000 0202 0c01  ...E...s,.......
+000020c0: 04ff 0c03 0801 0402 0201 0601 06fe 0605  ................
+000020d0: 0801 0602 0801 0c02 0a01 1401 0a02 04ff  ................
+000020e0: 0404 1401 0801 0801 7a14 5867 626f 6f73  ........z.Xgboos
+000020f0: 744d 6f64 656c 2e70 7265 6469 6374 2903  tModel.predict).
+00002100: 4e4e 4e29 1ada 085f 5f6e 616d 655f 5fda  NNN)...__name__.
+00002110: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00002120: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00002130: 5f5f 7204 0000 0072 0500 0000 7209 0000  __r....r....r...
+00002140: 0072 0b00 0000 720a 0000 0072 1a00 0000  .r....r....r....
+00002150: 7239 0000 00da 0653 6572 6965 7372 0300  r9.....Seriesr..
+00002160: 0000 da03 7374 72da 0566 6c6f 6174 7221  ....str..floatr!
+00002170: 0000 0072 2200 0000 da09 4461 7461 4672  ...r".....DataFr
+00002180: 616d 6572 3c00 0000 da07 426f 6f73 7465  amer<.....Booste
+00002190: 7272 4400 0000 7236 0000 0072 0600 0000  rrD...r6...r....
+000021a0: 7258 0000 00da 076e 6461 7272 6179 727e  rX.....ndarrayr~
+000021b0: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
+000021c0: 0000 7219 0000 0072 0f00 0000 1a00 0000  ..r....r........
+000021d0: 7350 0000 0008 0004 0102 0502 0102 0104  sP..............
+000021e0: fb06 0202 fe06 0302 fd06 0402 fc06 050a  ................
+000021f0: fb1c 0d08 0802 1504 0202 fe04 0302 fd04  ................
+00002200: 0402 fc04 0502 fb04 060a fa02 4504 0202  ............E...
+00002210: fe04 0302 fd04 0402 fc04 0502 fb02 060a  ................
+00002220: fa00 7f24 3a72 0f00 0000 291c 72a0 0000  ...$:r....).r...
+00002230: 0072 0200 0000 da06 7479 7069 6e67 7203  .r......typingr.
+00002240: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
+00002250: 0000 da05 6e75 6d70 7972 5800 0000 727d  ....numpyrX...r}
+00002260: 0000 00da 0670 616e 6461 7372 3900 0000  .....pandasr9...
+00002270: 728b 0000 0072 3c00 0000 da0f 736b 6c65  r....r<.....skle
+00002280: 6172 6e2e 6d65 7472 6963 7372 0700 0000  arn.metricsr....
+00002290: da0d 736b 6c65 6172 6e2e 7574 696c 7372  ..sklearn.utilsr
+000022a0: 0800 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+000022b0: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+000022c0: 6f6e 6669 6772 0900 0000 720a 0000 0072  onfigr....r....r
+000022d0: 0b00 0000 da24 626c 7565 6361 7374 2e67  .....$bluecast.g
+000022e0: 656e 6572 616c 5f75 7469 6c73 2e67 656e  eneral_utils.gen
+000022f0: 6572 616c 5f75 7469 6c73 720c 0000 0072  eral_utilsr....r
+00002300: 0d00 0000 da22 626c 7565 6361 7374 2e6d  ....."bluecast.m
+00002310: 6c5f 6d6f 6465 6c6c 696e 672e 6261 7365  l_modelling.base
+00002320: 5f63 6c61 7373 6573 720e 0000 0072 0f00  _classesr....r..
+00002330: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00002340: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00002350: 0100 0000 731a 0000 0004 000c 0618 0108  ....s...........
+00002360: 0208 0108 0108 010c 010c 0114 0210 050c  ................
+00002370: 0114 03                                  ...
```

### Comparing `bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-0.8/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 29 15:05:26 2023 UTC, .py size: 14107 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b69d 9d64 1b37 0000  U..........d.7..
+00000000: 550d 0d0a 0000 0000 2ac8 a264 6338 0000  U.......*..dc8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -147,15 +147,15 @@
 00000920: 0212 0106 0108 0114 0212 0206 0108 0114  ................
 00000930: 0212 0206 0108 0114 027a 1d58 6762 6f6f  .........z.Xgboo
 00000940: 7374 4d6f 6465 6c2e 6368 6563 6b5f 6c6f  stModel.check_lo
 00000950: 6164 5f63 6f6e 6673 2905 da07 785f 7472  ad_confs)...x_tr
 00000960: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
 00000970: 7261 696e da06 795f 7465 7374 721c 0000  rain..y_testr...
 00000980: 0063 0500 0000 0000 0000 0000 0000 0900  .c..............
-00000990: 0000 0700 0000 4300 0000 7352 0100 0074  ......C...sR...t
+00000990: 0000 0700 0000 4300 0000 7358 0100 0074  ......C...sX...t
 000009a0: 0074 01a0 02a1 009b 0064 019d 0283 0101  .t.......d......
 000009b0: 007c 00a0 03a1 0001 007c 006a 0472 267c  .|.......|.j.r&|
 000009c0: 006a 0573 2e74 0664 0283 0182 017c 006a  .j.s.t.d.....|.j
 000009d0: 056a 0772 467c 00a0 087c 017c 027c 037c  .j.rF|...|.|.|.|
 000009e0: 04a1 0401 0074 0964 0383 0101 0074 0964  .....t.d.....t.d
 000009f0: 0483 0101 007c 006a 056a 0a72 8c74 0074  .....|.j.j.r.t.t
 00000a00: 01a0 02a1 009b 0064 059d 0283 0101 0074  .......d.......t
@@ -166,392 +166,399 @@
 00000a50: 047d 066e 1474 0f6a 107c 017c 037c 006a  .}.n.t.j.|.|.|.j
 00000a60: 056a 1164 078d 037d 0674 0f6a 107c 027c  .j.d...}.t.j.|.|
 00000a70: 047c 006a 056a 1164 078d 037d 077c 0664  .|.j.j.d...}.|.d
 00000a80: 0866 027c 0764 0966 0267 027d 087c 006a  .f.|.d.f.g.}.|.j
 00000a90: 056a 1264 0a6b 0290 0172 2474 0f6a 137c  .j.d.k...r$t.j.|
 00000aa0: 006a 046a 147c 067c 006a 046a 1464 0b19  .j.j.|.|.j.j.d..
 00000ab0: 007c 006a 056a 157c 0864 0c8d 057c 005f  .|.j.j.|.d...|._
-00000ac0: 166e 2074 0f6a 137c 006a 046a 147c 067c  .n t.j.|.j.j.|.|
-00000ad0: 006a 046a 1464 0b19 007c 0864 0d8d 047c  .j.j.d...|.d...|
-00000ae0: 005f 1674 0964 0e83 0101 007c 006a 1653  ._.t.d.....|.j.S
-00000af0: 0029 0f7a 3f54 7261 696e 2058 6762 6f6f  .).z?Train Xgboo
-00000b00: 7374 206d 6f64 656c 2e20 496e 636c 7564  st model. Includ
-00000b10: 6573 2068 7970 6572 7061 7261 6d65 7465  es hyperparamete
-00000b20: 7220 7475 6e69 6e67 206f 6e20 6465 6661  r tuning on defa
-00000b30: 756c 742e 7a1e 3a20 5374 6172 7420 6669  ult.z.: Start fi
-00000b40: 7474 696e 6720 5867 626f 6f73 7420 6d6f  tting Xgboost mo
-00000b50: 6465 6c2e fa2c 636f 6e66 5f70 6172 616d  del..,conf_param
-00000b60: 735f 7867 626f 6f73 7420 6f72 2063 6f6e  s_xgboost or con
-00000b70: 665f 7472 6169 6e69 6e67 2069 7320 4e6f  f_training is No
-00000b80: 6e65 7a1e 4669 6e69 7368 6564 2068 7970  nez.Finished hyp
-00000b90: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
-00000ba0: 6e67 7a0e 5374 6172 7420 7472 6169 6e69  ngz.Start traini
-00000bb0: 6e67 7a7f 3a20 556e 696f 6e20 7472 6169  ngz.: Union trai
-00000bc0: 6e20 616e 6420 7465 7374 2064 6174 6120  n and test data 
-00000bd0: 666f 7220 6669 6e61 6c20 6d6f 6465 6c20  for final model 
-00000be0: 7472 6169 6e69 6e67 2062 6173 6564 206f  training based o
-00000bf0: 6e20 5472 6169 6e69 6e67 436f 6e66 6967  n TrainingConfig
-00000c00: 0a20 2020 2020 2020 2020 2020 2020 7061  .             pa
-00000c10: 7261 6d20 2775 7365 5f66 756c 6c5f 6461  ram 'use_full_da
-00000c20: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
-00000c30: 656c 27a9 03da 056c 6162 656c da06 7765  el'....label..we
-00000c40: 6967 6874 da12 656e 6162 6c65 5f63 6174  ight..enable_cat
-00000c50: 6567 6f72 6963 616c a902 7229 0000 0072  egorical..r)...r
-00000c60: 2b00 0000 da05 7472 6169 6eda 0474 6573  +.....train..tes
-00000c70: 74e9 0100 0000 da05 7374 6570 7329 03da  t.......steps)..
-00000c80: 0f6e 756d 5f62 6f6f 7374 5f72 6f75 6e64  .num_boost_round
-00000c90: da15 6561 726c 795f 7374 6f70 7069 6e67  ..early_stopping
-00000ca0: 5f72 6f75 6e64 73da 0565 7661 6c73 2902  _rounds..evals).
-00000cb0: 7231 0000 0072 3300 0000 7a11 4669 6e69  r1...r3...z.Fini
-00000cc0: 7368 6564 2074 7261 696e 696e 6729 1772  shed training).r
-00000cd0: 0d00 0000 7202 0000 0072 1e00 0000 7222  ....r....r....r"
-00000ce0: 0000 0072 1500 0000 7213 0000 00da 0a56  ...r....r......V
-00000cf0: 616c 7565 4572 726f 72da 0e61 7574 6f74  alueError..autot
-00000d00: 756e 655f 6d6f 6465 6cda 0861 7574 6f74  une_model..autot
-00000d10: 756e 65da 0570 7269 6e74 da1d 7573 655f  une..print..use_
-00000d20: 6675 6c6c 5f64 6174 615f 666f 725f 6669  full_data_for_fi
-00000d30: 6e61 6c5f 6d6f 6465 6cda 0270 64da 0663  nal_model..pd..c
-00000d40: 6f6e 6361 74da 0d73 616d 706c 655f 7765  oncat..sample_we
-00000d50: 6967 6874 7221 0000 00da 0378 6762 da07  ightr!.....xgb..
-00000d60: 444d 6174 7269 78da 1d63 6174 5f65 6e63  DMatrix..cat_enc
-00000d70: 6f64 696e 675f 7669 615f 6d6c 5f61 6c67  oding_via_ml_alg
-00000d80: 6f72 6974 686d da14 6879 7065 7274 756e  orithm..hypertun
-00000d90: 696e 675f 6376 5f66 6f6c 6473 722d 0000  ing_cv_foldsr-..
-00000da0: 00da 0670 6172 616d 7372 3200 0000 7216  ...paramsr2...r.
-00000db0: 0000 0029 0972 1700 0000 7223 0000 0072  ...).r....r#...r
-00000dc0: 2400 0000 7225 0000 0072 2600 0000 7220  $...r%...r&...r 
-00000dd0: 0000 00da 0764 5f74 7261 696e da06 645f  .....d_train..d_
-00000de0: 7465 7374 da08 6576 616c 5f73 6574 7218  test..eval_setr.
-00000df0: 0000 0072 1800 0000 7219 0000 00da 0366  ...r....r......f
-00000e00: 6974 4700 0000 7362 0000 0000 0812 0108  itG...sb........
-00000e10: 020c 0108 0208 0110 0208 0208 0108 0102  ................
-00000e20: 010c ff04 040e 010e 0208 010a 0104 0102  ................
-00000e30: 0102 0102 0106 fc08 0704 0102 0102 0106  ................
-00000e40: fd06 0604 0102 0102 0106 fd06 0510 020e  ................
-00000e50: 0104 0106 0102 010a 0106 0102 fb0a 0804  ................
-00000e60: 0106 0102 010a 0202 fb08 0708 017a 1058  .............z.X
-00000e70: 6762 6f6f 7374 4d6f 6465 6c2e 6669 7463  gboostModel.fitc
-00000e80: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
-00000e90: 1000 0000 0300 0000 7392 0100 0074 0074  ........s....t.t
-00000ea0: 01a0 02a1 009b 0064 019d 0283 0101 0088  .......d........
-00000eb0: 016a 0372 1e88 016a 0473 2674 0564 0283  .j.r...j.s&t.d..
-00000ec0: 0182 0174 066a 077c 0288 0488 016a 046a  ...t.j.|.....j.j
-00000ed0: 0864 038d 0389 0074 0983 0089 0288 01a0  .d.....t........
-00000ee0: 0aa1 0001 0088 016a 0372 5a88 016a 0472  .......j.rZ..j.r
-00000ef0: 5a88 016a 0b73 6274 0564 0483 0182 0187  Z..j.sbt.d......
-00000f00: 0087 0187 0287 0387 0487 0566 0664 0564  ...........f.d.d
-00000f10: 0684 087d 0564 077d 0674 0c6a 0d6a 0e64  ...}.d.}.t.j.j.d
-00000f20: 0888 016a 046a 0f64 098d 027d 0774 0c6a  ...j.j.d...}.t.j
-00000f30: 1064 0a7c 077c 069b 0064 0b9d 0264 0c8d  .d.|.|...d...d..
-00000f40: 037d 087c 086a 117c 0588 016a 046a 1288  .}.|.j.|...j.j..
-00000f50: 016a 046a 1364 0d64 0d64 0e8d 0501 007a  .j.j.d.d.d.....z
-00000f60: 2c74 0c6a 14a0 157c 08a1 017d 097c 09a0  ,t.j...|...}.|..
-00000f70: 16a1 0001 0074 0c6a 14a0 177c 08a1 017d  .....t.j...|...}
-00000f80: 097c 09a0 16a1 0001 0057 006e 1c04 0074  .|.......W.n...t
-00000f90: 1874 1974 0566 036b 0a90 0172 0a01 0001  .t.t.f.k...r....
-00000fa0: 0001 0059 006e 0258 007c 086a 1a6a 1b7d  ...Y.n.X.|.j.j.}
-00000fb0: 0a88 016a 0b6a 1c88 016a 0b6a 1d88 016a  ...j.j...j.j...j
-00000fc0: 0b6a 1e88 0288 05a0 1fa1 007c 0a64 0f19  .j.........|.d..
-00000fd0: 007c 0a64 1019 007c 0a64 1119 007c 0a64  .|.d...|.d...|.d
-00000fe0: 1219 007c 0a64 1319 007c 0a64 1419 007c  ...|.d...|.d...|
-00000ff0: 0a64 1519 007c 0a64 1619 0088 016a 0b6a  .d...|.d.....j.j
-00001000: 207c 0a64 1719 0064 189c 0f88 016a 035f   |.d...d.....j._
-00001010: 1b74 2164 1988 016a 036a 1b83 0201 007c  .t!d...j.j.....|
-00001020: 0a64 1a19 0088 016a 035f 2264 1b53 0029  .d.....j._"d.S.)
-00001030: 1c7a 7b54 756e 6520 6879 7065 7270 6172  .z{Tune hyperpar
-00001040: 616d 6574 6572 732e 0a0a 2020 2020 2020  ameters...      
-00001050: 2020 416e 2061 6c74 6572 6e61 7469 7665    An alternative
-00001060: 2063 6f6e 6669 6720 6361 6e20 6265 2070   config can be p
-00001070: 726f 7669 6465 6420 746f 206f 7665 7277  rovided to overw
-00001080: 7269 7465 2074 6865 2068 7970 6572 7061  rite the hyperpa
-00001090: 7261 6d65 7465 7220 7365 6172 6368 2073  rameter search s
-000010a0: 7061 6365 2e0a 2020 2020 2020 2020 7a2f  pace..        z/
-000010b0: 3a20 5374 6172 7420 6879 7065 7270 6172  : Start hyperpar
-000010c0: 616d 6574 6572 2074 756e 696e 6720 6f66  ameter tuning of
-000010d0: 2058 6762 6f6f 7374 206d 6f64 656c 2e72   Xgboost model.r
-000010e0: 2700 0000 722c 0000 007a 3941 7420 6c65  '...r,...z9At le
-000010f0: 6173 7420 6f6e 6520 6f66 2074 6865 2063  ast one of the c
-00001100: 6f6e 6669 6773 2069 7320 4e6f 6e65 2c20  onfigs is None, 
-00001110: 7768 6963 6820 6973 206e 6f74 2061 6c6c  which is not all
-00001120: 6f77 6564 6301 0000 0000 0000 0000 0000  owedc...........
-00001130: 000c 0000 0013 0000 0013 0000 0073 e401  .............s..
-00001140: 0000 8801 6a00 6a01 8801 6a00 6a02 8801  ....j.j...j.j...
-00001150: 6a00 6a03 8802 8805 a004 a100 7c00 a005  j.j.........|...
-00001160: 6401 8801 6a00 6a06 8801 6a00 6a07 a103  d...j.j...j.j...
-00001170: 7c00 a008 6402 8801 6a00 6a09 8801 6a00  |...d...j.j...j.
-00001180: 6a0a a103 7c00 a008 6403 8801 6a00 6a0b  j...|...d...j.j.
-00001190: 8801 6a00 6a0c a103 7c00 a008 6404 8801  ..j.j...|...d...
-000011a0: 6a00 6a0d 8801 6a00 6a0e a103 7c00 a005  j.j...j.j...|...
-000011b0: 6405 8801 6a00 6a0f 8801 6a00 6a10 a103  d...j.j...j.j...
-000011c0: 7c00 a008 6406 8801 6a00 6a11 8801 6a00  |...d...j.j...j.
-000011d0: 6a12 a103 7c00 a008 6407 8801 6a00 6a13  j...|...d...j.j.
-000011e0: 8801 6a00 6a14 a103 7c00 a008 6408 8801  ..j.j...|...d...
-000011f0: 6a00 6a15 8801 6a00 6a16 a103 8801 6a00  j.j...j.j.....j.
-00001200: 6a17 7c00 a005 6409 8801 6a00 6a18 8801  j.|...d...j.j...
-00001210: 6a00 6a19 a103 640a 9c0f 7d01 7c00 a01a  j.j...d...}.|...
-00001220: 640b 640c 640d 6702 a102 7d02 7c02 9001  d.d.d.g...}.|...
-00001230: 7212 8801 a01b 8805 a101 7d03 741c 6a1d  r.........}.t.j.
-00001240: 8803 8805 7c03 8801 6a1e 6a1f 640e 8d04  ....|...j.j.d...
-00001250: 7d04 6e14 741c 6a1d 8803 8805 8801 6a1e  }.n.t.j.......j.
-00001260: 6a1f 640f 8d03 7d04 7420 6a21 a022 7c00  j.d...}.t j!."|.
-00001270: 6410 a102 7d05 8801 6a1e 6a23 6411 6b02  d...}...j.j#d.k.
-00001280: 9001 72a8 7c04 6412 6602 8800 6413 6602  ..r.|.d.f...d.f.
-00001290: 6702 7d06 741c 6a24 7c01 7c04 7c01 6409  g.}.t.j$|.|.|.d.
-000012a0: 1900 8801 6a1e 6a25 7c06 7c05 6701 8801  ....j.j%|.|.g...
-000012b0: 6a00 6a03 6414 8d07 7d07 7c07 a026 8800  j.j.d...}.|..&..
-000012c0: a101 7d08 7427 a028 6415 6416 8400 7c08  ..}.t'.(d.d...|.
-000012d0: 4400 8301 a101 7d09 7429 8804 7c09 8302  D.....}.t)..|...
-000012e0: 6417 1400 7d0a 7c0a 5300 741c 6a2a 7c01  d...}.|.S.t.j*|.
-000012f0: 7c04 7c01 6409 1900 8801 6a1e 6a23 640c  |.|.d.....j.j#d.
-00001300: 8801 6a1e 6a2b 7c05 6701 8801 6a1e 6a2c  ..j.j+|.g...j.j,
-00001310: 6418 8d08 7d0b 7c0b 6419 1900 a02d a100  d...}.|.d....-..
-00001320: 5300 6400 5300 291a 4eda 096d 6178 5f64  S.d.S.).N..max_d
-00001330: 6570 7468 da05 616c 7068 61da 066c 616d  epth..alpha..lam
-00001340: 6264 61da 106d 696e 5f63 6869 6c64 5f77  bda..min_child_w
-00001350: 6569 6768 74da 0a6e 756d 5f6c 6561 7665  eight..num_leave
-00001360: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
-00001370: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
-00001380: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
-00001390: 6c72 3000 0000 290f da09 6f62 6a65 6374  lr0...)...object
-000013a0: 6976 65da 0b65 7661 6c5f 6d65 7472 6963  ive..eval_metric
-000013b0: da07 7665 7262 6f73 65da 0b74 7265 655f  ..verbose..tree_
-000013c0: 6d65 7468 6f64 da09 6e75 6d5f 636c 6173  method..num_clas
-000013d0: 7372 4500 0000 7246 0000 0072 4700 0000  srE...rF...rG...
-000013e0: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
-000013f0: 4b00 0000 724c 0000 00da 0365 7461 7230  K...rL.....etar0
-00001400: 0000 0072 3b00 0000 5446 7228 0000 0072  ...r;...TFr(...r
-00001410: 2c00 0000 7a0d 7465 7374 2d6d 6c6f 676c  ,...z.test-mlogl
-00001420: 6f73 7372 2f00 0000 722d 0000 0072 2e00  ossr/...r-...r..
-00001430: 0000 2905 7231 0000 0072 3200 0000 7233  ..).r1...r2...r3
-00001440: 0000 00da 0963 616c 6c62 6163 6b73 da0c  .....callbacks..
-00001450: 7665 7262 6f73 655f 6576 616c 6301 0000  verbose_evalc...
-00001460: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001470: 0053 0000 0073 1600 0000 6700 7c00 5d0e  .S...s....g.|.].
-00001480: 7d01 7400 a001 7c01 a101 9102 7104 5300  }.t...|.....q.S.
-00001490: 7218 0000 00a9 02da 026e 70da 0661 7267  r........np..arg
-000014a0: 6d61 78a9 02da 022e 30da 046c 696e 6572  max.....0..liner
-000014b0: 1800 0000 7218 0000 0072 1900 0000 da0a  ....r....r......
-000014c0: 3c6c 6973 7463 6f6d 703e fb00 0000 7304  <listcomp>....s.
-000014d0: 0000 0006 0002 007a 3c58 6762 6f6f 7374  .......z<Xgboost
-000014e0: 4d6f 6465 6c2e 6175 746f 7475 6e65 2e3c  Model.autotune.<
-000014f0: 6c6f 6361 6c73 3e2e 6f62 6a65 6374 6976  locals>.objectiv
-00001500: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00001510: 636f 6d70 3ee9 ffff ffff 2908 7240 0000  comp>.....).r@..
-00001520: 00da 0664 7472 6169 6e72 3100 0000 da05  ...dtrainr1.....
-00001530: 6e66 6f6c 64da 0961 735f 7061 6e64 6173  nfold..as_pandas
-00001540: da04 7365 6564 7253 0000 00da 0773 6875  ..seedrS.....shu
-00001550: 6666 6c65 7a12 7465 7374 2d6d 6c6f 676c  fflez.test-mlogl
-00001560: 6f73 732d 6d65 616e 292e 7214 0000 00da  oss-mean).r.....
-00001570: 0f6d 6f64 656c 5f6f 626a 6563 7469 7665  .model_objective
-00001580: da11 6d6f 6465 6c5f 6576 616c 5f6d 6574  ..model_eval_met
-00001590: 7269 63da 0f6d 6f64 656c 5f76 6572 626f  ric..model_verbo
-000015a0: 7369 7479 da07 6e75 6e69 7175 65da 0b73  sity..nunique..s
-000015b0: 7567 6765 7374 5f69 6e74 da0d 6d61 785f  uggest_int..max_
-000015c0: 6465 7074 685f 6d69 6eda 0d6d 6178 5f64  depth_min..max_d
-000015d0: 6570 7468 5f6d 6178 da0d 7375 6767 6573  epth_max..sugges
-000015e0: 745f 666c 6f61 74da 0961 6c70 6861 5f6d  t_float..alpha_m
-000015f0: 696e da09 616c 7068 615f 6d61 78da 0a6c  in..alpha_max..l
-00001600: 616d 6264 615f 6d69 6eda 0a6c 616d 6264  ambda_min..lambd
-00001610: 615f 6d61 78da 146d 696e 5f63 6869 6c64  a_max..min_child
-00001620: 5f77 6569 6768 745f 6d69 6eda 146d 696e  _weight_min..min
-00001630: 5f63 6869 6c64 5f77 6569 6768 745f 6d61  _child_weight_ma
-00001640: 78da 0e6e 756d 5f6c 6561 7665 735f 6d69  x..num_leaves_mi
-00001650: 6eda 0e6e 756d 5f6c 6561 7665 735f 6d61  n..num_leaves_ma
-00001660: 78da 0e73 7562 5f73 616d 706c 655f 6d69  x..sub_sample_mi
-00001670: 6eda 0e73 7562 5f73 616d 706c 655f 6d61  n..sub_sample_ma
-00001680: 78da 1663 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
-00001690: 5f74 7265 655f 6d69 6eda 1663 6f6c 5f73  _tree_min..col_s
-000016a0: 616d 706c 655f 6279 5f74 7265 655f 6d61  ample_by_tree_ma
-000016b0: 78da 1763 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
-000016c0: 5f6c 6576 656c 5f6d 696e da17 636f 6c5f  _level_min..col_
-000016d0: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
-000016e0: 6d61 7872 5200 0000 da09 7374 6570 735f  maxrR.....steps_
-000016f0: 6d69 6eda 0973 7465 7073 5f6d 6178 da13  min..steps_max..
-00001700: 7375 6767 6573 745f 6361 7465 676f 7269  suggest_categori
-00001710: 6361 6c72 2100 0000 723c 0000 0072 3d00  calr!...r<...r=.
-00001720: 0000 7213 0000 0072 3e00 0000 da06 6f70  ..r....r>.....op
-00001730: 7475 6e61 da0b 696e 7465 6772 6174 696f  tuna..integratio
-00001740: 6eda 1658 4742 6f6f 7374 5072 756e 696e  n..XGBoostPrunin
-00001750: 6743 616c 6c62 6163 6b72 3f00 0000 722d  gCallbackr?...r-
-00001760: 0000 0072 3200 0000 da07 7072 6564 6963  ...r2.....predic
-00001770: 7472 5600 0000 da07 6173 6172 7261 7972  trV.....asarrayr
-00001780: 0700 0000 da02 6376 da13 676c 6f62 616c  ......cv..global
-00001790: 5f72 616e 646f 6d5f 7374 6174 65da 1773  _random_state..s
-000017a0: 6875 6666 6c65 5f64 7572 696e 675f 7472  huffle_during_tr
-000017b0: 6169 6e69 6e67 da04 6d65 616e 290c da05  aining..mean)...
-000017c0: 7472 6961 6cda 0570 6172 616d 723b 0000  trial..paramr;..
-000017d0: 0072 2000 0000 7241 0000 00da 1070 7275  .r ...rA.....pru
-000017e0: 6e69 6e67 5f63 616c 6c62 6163 6b72 4300  ning_callbackrC.
-000017f0: 0000 7216 0000 00da 0570 7265 6473 da0b  ..r......preds..
-00001800: 7072 6564 5f6c 6162 656c 73da 076d 6174  pred_labels..mat
-00001810: 7468 6577 da06 7265 7375 6c74 a906 7242  thew..result..rB
-00001820: 0000 0072 1700 0000 da08 7472 6169 6e5f  ...r......train_
-00001830: 6f6e 7223 0000 0072 2600 0000 7225 0000  onr#...r&...r%..
-00001840: 0072 1800 0000 7219 0000 0072 4d00 0000  .r....r....rM...
-00001850: ad00 0000 73c0 0000 0000 0206 0106 0106  ....s...........
-00001860: 0102 0106 0104 0102 0106 0106 fd02 0504  ................
-00001870: 0102 0006 0006 ff02 0304 0102 0006 0006  ................
-00001880: ff02 0304 0102 0006 0006 ff02 0304 0102  ................
-00001890: 0106 0106 fd02 0504 0102 0106 0106 fd02  ................
-000018a0: 0504 0102 0106 0106 fd02 0504 0102 0106  ................
-000018b0: 0106 fd02 0506 0104 0102 0006 0006 ff02  ................
-000018c0: d706 2d10 0106 010a 0104 0102 0102 0102  ..-.............
-000018d0: 0106 fc08 0704 0102 0102 0106 fd06 0606  ................
-000018e0: 0102 0002 ff04 040e 0110 0104 0102 0102  ................
-000018f0: 0106 0106 0102 0104 0106 f906 090a 0114  ................
-00001900: 010e 0104 0204 0102 0102 0106 0206 0102  ................
-00001910: 0106 0104 0106 f706 0c7a 2858 6762 6f6f  .........z(Xgboo
-00001920: 7374 4d6f 6465 6c2e 6175 746f 7475 6e65  stModel.autotune
-00001930: 2e3c 6c6f 6361 6c73 3e2e 6f62 6a65 6374  .<locals>.object
-00001940: 6976 65da 0778 6762 6f6f 7374 4629 02da  ive..xgboostF)..
-00001950: 0c6d 756c 7469 7661 7269 6174 6572 6000  .multivariater`.
-00001960: 0000 da08 6d69 6e69 6d69 7a65 7a07 2074  ....minimizez. t
-00001970: 756e 696e 6729 03da 0964 6972 6563 7469  uning)...directi
-00001980: 6f6e da07 7361 6d70 6c65 72da 0a73 7475  on..sampler..stu
-00001990: 6479 5f6e 616d 6554 2904 da08 6e5f 7472  dy_nameT)...n_tr
-000019a0: 6961 6c73 da07 7469 6d65 6f75 74da 0e67  ials..timeout..g
-000019b0: 635f 6166 7465 725f 7472 6961 6cda 1173  c_after_trial..s
-000019c0: 686f 775f 7072 6f67 7265 7373 5f62 6172  how_progress_bar
-000019d0: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
-000019e0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
-000019f0: 0000 0072 4800 0000 7230 0000 0029 0f72  ...rH...r0...).r
-00001a00: 4d00 0000 724e 0000 0072 4f00 0000 7250  M...rN...rO...rP
-00001a10: 0000 0072 5100 0000 7245 0000 0072 4600  ...rQ...rE...rF.
-00001a20: 0000 7247 0000 0072 4900 0000 724a 0000  ..rG...rI...rJ..
-00001a30: 0072 4b00 0000 724c 0000 0072 4800 0000  .rK...rL...rH...
-00001a40: 7252 0000 0072 3000 0000 7a0d 4265 7374  rR...r0...z.Best
-00001a50: 2070 6172 616d 733a 2072 3b00 0000 4e29   params: r;...N)
-00001a60: 2372 0d00 0000 7202 0000 0072 1e00 0000  #r....r....r....
-00001a70: 7215 0000 0072 1300 0000 7234 0000 0072  r....r....r4...r
-00001a80: 3c00 0000 723d 0000 0072 3e00 0000 720c  <...r=...r>...r.
-00001a90: 0000 0072 2200 0000 7214 0000 0072 7b00  ...r"...r....r{.
-00001aa0: 0000 da08 7361 6d70 6c65 7273 da0a 5450  ....samplers..TP
-00001ab0: 4553 616d 706c 6572 7281 0000 00da 0c63  ESamplerr......c
-00001ac0: 7265 6174 655f 7374 7564 79da 086f 7074  reate_study..opt
-00001ad0: 696d 697a 65da 1c68 7970 6572 7061 7261  imize..hyperpara
-00001ae0: 6d65 7465 725f 7475 6e69 6e67 5f72 6f75  meter_tuning_rou
-00001af0: 6e64 73da 2668 7970 6572 7061 7261 6d65  nds.&hyperparame
-00001b00: 7465 725f 7475 6e69 6e67 5f6d 6178 5f72  ter_tuning_max_r
-00001b10: 756e 7469 6d65 5f73 6563 73da 0d76 6973  untime_secs..vis
-00001b20: 7561 6c69 7a61 7469 6f6e da19 706c 6f74  ualization..plot
-00001b30: 5f6f 7074 696d 697a 6174 696f 6e5f 6869  _optimization_hi
-00001b40: 7374 6f72 79da 0473 686f 77da 1670 6c6f  story..show..plo
-00001b50: 745f 7061 7261 6d5f 696d 706f 7274 616e  t_param_importan
-00001b60: 6365 73da 115a 6572 6f44 6976 6973 696f  ces..ZeroDivisio
-00001b70: 6e45 7272 6f72 da0c 5275 6e74 696d 6545  nError..RuntimeE
-00001b80: 7272 6f72 da0a 6265 7374 5f74 7269 616c  rror..best_trial
-00001b90: 7240 0000 0072 6200 0000 7263 0000 0072  r@...rb...rc...r
-00001ba0: 6400 0000 7265 0000 0072 5200 0000 7237  d...re...rR...r7
-00001bb0: 0000 0072 3b00 0000 290b 7217 0000 0072  ...r;...).r....r
-00001bc0: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
-00001bd0: 0000 0072 4d00 0000 da09 616c 676f 7269  ...rM.....algori
-00001be0: 7468 6d72 9100 0000 da05 7374 7564 79da  thmr......study.
-00001bf0: 0366 6967 5a12 7867 626f 6f73 745f 6265  .figZ.xgboost_be
-00001c00: 7374 5f70 6172 616d 7218 0000 0072 8b00  st_paramr....r..
-00001c10: 0000 7219 0000 0072 3600 0000 8c00 0000  ..r....r6.......
-00001c20: 7382 0000 0000 0b12 010c 0108 0204 0102  s...............
-00001c30: 0102 0106 fd06 0506 0208 0304 ff02 0204  ................
-00001c40: fe02 0304 fd02 0502 0102 ff04 0416 6004  ..............`.
-00001c50: 0106 0102 0006 ff06 0304 0102 0102 0108  ................
-00001c60: fd06 0604 0102 0106 0106 0102 0102 fb06  ................
-00001c70: 0702 010c 0108 010c 010c 0116 0106 0208  ................
-00001c80: 0206 0106 0106 0102 0106 0102 0102 ff02  ................
-00001c90: 0306 0106 0106 0106 0106 0106 0106 0106  ................
-00001ca0: 0106 ef0a 130e 017a 1558 6762 6f6f 7374  .......z.Xgboost
-00001cb0: 4d6f 6465 6c2e 6175 746f 7475 6e65 2902  Model.autotune).
-00001cc0: da02 6466 721c 0000 0063 0200 0000 0000  ..dfr....c......
-00001cd0: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
-00001ce0: 0000 73b4 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
-00001cf0: 0064 019d 0283 0101 007c 006a 0372 1e7c  .d.......|.j.r.|
-00001d00: 006a 0473 2674 0564 0283 0182 0174 066a  .j.s&t.d.....t.j
-00001d10: 077c 017c 006a 046a 0864 038d 027d 027c  .|.|.j.j.d...}.|
-00001d20: 006a 0973 4674 0a64 0483 0182 017c 006a  .j.sFt.d.....|.j
-00001d30: 0b73 5474 0a64 0583 0182 017c 006a 09a0  .sTt.d.....|.j..
-00001d40: 0c7c 02a1 017d 037c 006a 0d64 066b 0272  .|...}.|.j.d.k.r
-00001d50: 8c74 0ea0 0f64 0764 0884 007c 0344 0083  .t...d.d...|.D..
-00001d60: 01a1 017d 047c 047c 006a 0b6a 106b 047d  ...}.|.|.j.j.k.}
-00001d70: 056e 187c 037d 0474 0ea0 0f64 0964 0884  .n.|.}.t...d.d..
-00001d80: 007c 0344 0083 01a1 017d 0574 1164 0a83  .|.D.....}.t.d..
-00001d90: 0101 007c 047c 0566 0253 0029 0b7a 1750  ...|.|.f.S.).z.P
-00001da0: 7265 6469 6374 206f 6e20 756e 7365 656e  redict on unseen
-00001db0: 2064 6174 612e 7a33 3a20 5374 6172 7420   data.z3: Start 
-00001dc0: 7072 6564 6963 7469 6e67 206f 6e20 6e65  predicting on ne
-00001dd0: 7720 6461 7461 2075 7369 6e67 2058 6762  w data using Xgb
-00001de0: 6f6f 7374 206d 6f64 656c 2e72 2700 0000  oost model.r'...
-00001df0: 2901 722b 0000 007a 204e 6f20 7472 6169  ).r+...z No trai
-00001e00: 6e65 6420 6d6f 6465 6c20 6861 7320 6265  ned model has be
-00001e10: 656e 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f  en found.z+No mo
-00001e20: 6465 6c20 636f 6e66 6967 7572 6174 696f  del configuratio
-00001e30: 6e20 6669 6c65 2068 6173 2062 6565 6e20  n file has been 
-00001e40: 666f 756e 642e 7210 0000 0063 0100 0000  found.r....c....
-00001e50: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001e60: 5300 0000 7314 0000 0067 007c 005d 0c7d  S...s....g.|.].}
-00001e70: 017c 0164 0019 0091 0271 0453 0029 0172  .|.d.....q.S.).r
-00001e80: 2f00 0000 7218 0000 0072 5800 0000 7218  /...r....rX...r.
-00001e90: 0000 0072 1800 0000 7219 0000 0072 5b00  ...r....r....r[.
-00001ea0: 0000 5201 0000 7304 0000 0006 0002 007a  ..R...s........z
-00001eb0: 2858 6762 6f6f 7374 4d6f 6465 6c2e 7072  (XgboostModel.pr
-00001ec0: 6564 6963 742e 3c6c 6f63 616c 733e 2e3c  edict.<locals>.<
-00001ed0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
-00001ee0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00001ef0: 0000 7316 0000 0067 007c 005d 0e7d 0174  ..s....g.|.].}.t
-00001f00: 00a0 017c 01a1 0191 0271 0453 0072 1800  ...|.....q.S.r..
-00001f10: 0000 7255 0000 0072 5800 0000 7218 0000  ..rU...rX...r...
-00001f20: 0072 1800 0000 7219 0000 0072 5b00 0000  .r....r....r[...
-00001f30: 5801 0000 7304 0000 0006 0002 007a 1346  X...s........z.F
-00001f40: 696e 6973 6865 6420 7072 6564 6963 7469  inished predicti
-00001f50: 6e67 2912 720d 0000 0072 0200 0000 721e  ng).r....r....r.
-00001f60: 0000 0072 1400 0000 7213 0000 0072 3400  ...r....r....r4.
-00001f70: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
-00001f80: 0072 1600 0000 da09 4578 6365 7074 696f  .r......Exceptio
-00001f90: 6e72 1500 0000 727e 0000 0072 1200 0000  nr....r~...r....
-00001fa0: 7256 0000 0072 7f00 0000 da18 636c 6173  rV...r......clas
-00001fb0: 7369 6669 6361 7469 6f6e 5f74 6872 6573  sification_thres
-00001fc0: 686f 6c64 7237 0000 0029 0672 1700 0000  holdr7...).r....
-00001fd0: 72a7 0000 0072 4200 0000 da0d 7061 7274  r....rB.....part
-00001fe0: 6961 6c5f 7072 6f62 73da 0f70 7265 6469  ial_probs..predi
-00001ff0: 6374 6564 5f70 726f 6273 da11 7072 6564  cted_probs..pred
-00002000: 6963 7465 645f 636c 6173 7365 7372 1800  icted_classesr..
-00002010: 0000 7218 0000 0072 1900 0000 727e 0000  ..r....r....r~..
-00002020: 003d 0100 0073 2c00 0000 0002 0201 0cff  .=...s,.........
-00002030: 0403 0c01 0802 0401 0201 06fe 0605 0601  ................
-00002040: 0802 0601 0802 0c01 0a01 1402 0aff 0404  ................
-00002050: 0401 1401 0801 7a14 5867 626f 6f73 744d  ......z.XgboostM
-00002060: 6f64 656c 2e70 7265 6469 6374 2903 4e4e  odel.predict).NN
-00002070: 4e29 1ada 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00002080: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00002090: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-000020a0: 7204 0000 0072 0500 0000 7209 0000 0072  r....r....r....r
-000020b0: 0b00 0000 720a 0000 0072 1a00 0000 7239  ....r....r....r9
-000020c0: 0000 00da 0653 6572 6965 7372 0300 0000  .....Seriesr....
-000020d0: da03 7374 72da 0566 6c6f 6174 7221 0000  ..str..floatr!..
-000020e0: 0072 2200 0000 da09 4461 7461 4672 616d  .r".....DataFram
-000020f0: 6572 3c00 0000 da07 426f 6f73 7465 7272  er<.....Boosterr
-00002100: 4400 0000 7236 0000 0072 0600 0000 7256  D...r6...r....rV
-00002110: 0000 00da 076e 6461 7272 6179 727e 0000  .....ndarrayr~..
-00002120: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00002130: 7219 0000 0072 0f00 0000 1a00 0000 7334  r....r........s4
-00002140: 0000 0008 0104 0500 0100 0100 fb02 0206  ................
-00002150: 0106 0106 0106 fb0c 0d1a 0808 1704 0104  ................
-00002160: 0104 0104 0104 fa0c 4704 0104 0104 0104  ........G.......
-00002170: 0102 fa0c 7f00 3272 0f00 0000 291c 72b0  ......2r....).r.
-00002180: 0000 0072 0200 0000 da06 7479 7069 6e67  ...r......typing
-00002190: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-000021a0: 0600 0000 da05 6e75 6d70 7972 5600 0000  ......numpyrV...
-000021b0: 727b 0000 00da 0670 616e 6461 7372 3900  r{.....pandasr9.
-000021c0: 0000 728d 0000 0072 3c00 0000 da0f 736b  ..r....r<.....sk
-000021d0: 6c65 6172 6e2e 6d65 7472 6963 7372 0700  learn.metricsr..
-000021e0: 0000 5a0d 736b 6c65 6172 6e2e 7574 696c  ..Z.sklearn.util
-000021f0: 7372 0800 0000 da1f 626c 7565 6361 7374  sr......bluecast
-00002200: 2e63 6f6e 6669 672e 7472 6169 6e69 6e67  .config.training
-00002210: 5f63 6f6e 6669 6772 0900 0000 720a 0000  _configr....r...
-00002220: 0072 0b00 0000 da24 626c 7565 6361 7374  .r.....$bluecast
-00002230: 2e67 656e 6572 616c 5f75 7469 6c73 2e67  .general_utils.g
-00002240: 656e 6572 616c 5f75 7469 6c73 720c 0000  eneral_utilsr...
-00002250: 0072 0d00 0000 5a22 626c 7565 6361 7374  .r....Z"bluecast
-00002260: 2e6d 6c5f 6d6f 6465 6c6c 696e 672e 6261  .ml_modelling.ba
-00002270: 7365 5f63 6c61 7373 6573 720e 0000 0072  se_classesr....r
-00002280: 0f00 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
-00002290: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
-000022a0: 653e 0100 0000 7318 0000 0004 060c 0118  e>....s.........
-000022b0: 0208 0108 0108 0108 010c 010c 0214 0510  ................
-000022c0: 010c 03                                  ...
+00000ac0: 166e 2674 0f6a 137c 006a 046a 147c 067c  .n&t.j.|.j.j.|.|
+00000ad0: 006a 046a 1464 0b19 007c 006a 056a 157c  .j.j.d...|.j.j.|
+00000ae0: 0864 0c8d 057c 005f 1674 0964 0d83 0101  .d...|._.t.d....
+00000af0: 007c 006a 1653 0029 0e7a 3f54 7261 696e  .|.j.S.).z?Train
+00000b00: 2058 6762 6f6f 7374 206d 6f64 656c 2e20   Xgboost model. 
+00000b10: 496e 636c 7564 6573 2068 7970 6572 7061  Includes hyperpa
+00000b20: 7261 6d65 7465 7220 7475 6e69 6e67 206f  rameter tuning o
+00000b30: 6e20 6465 6661 756c 742e 7a1e 3a20 5374  n default.z.: St
+00000b40: 6172 7420 6669 7474 696e 6720 5867 626f  art fitting Xgbo
+00000b50: 6f73 7420 6d6f 6465 6c2e fa2c 636f 6e66  ost model..,conf
+00000b60: 5f70 6172 616d 735f 7867 626f 6f73 7420  _params_xgboost 
+00000b70: 6f72 2063 6f6e 665f 7472 6169 6e69 6e67  or conf_training
+00000b80: 2069 7320 4e6f 6e65 7a1e 4669 6e69 7368   is Nonez.Finish
+00000b90: 6564 2068 7970 6572 7061 7261 6d65 7465  ed hyperparamete
+00000ba0: 7220 7475 6e69 6e67 7a0e 5374 6172 7420  r tuningz.Start 
+00000bb0: 7472 6169 6e69 6e67 7a7f 3a20 556e 696f  trainingz.: Unio
+00000bc0: 6e20 7472 6169 6e20 616e 6420 7465 7374  n train and test
+00000bd0: 2064 6174 6120 666f 7220 6669 6e61 6c20   data for final 
+00000be0: 6d6f 6465 6c20 7472 6169 6e69 6e67 2062  model training b
+00000bf0: 6173 6564 206f 6e20 5472 6169 6e69 6e67  ased on Training
+00000c00: 436f 6e66 6967 0a20 2020 2020 2020 2020  Config.         
+00000c10: 2020 2020 7061 7261 6d20 2775 7365 5f66      param 'use_f
+00000c20: 756c 6c5f 6461 7461 5f66 6f72 5f66 696e  ull_data_for_fin
+00000c30: 616c 5f6d 6f64 656c 27a9 03da 056c 6162  al_model'....lab
+00000c40: 656c da06 7765 6967 6874 da12 656e 6162  el..weight..enab
+00000c50: 6c65 5f63 6174 6567 6f72 6963 616c a902  le_categorical..
+00000c60: 7229 0000 0072 2b00 0000 da05 7472 6169  r)...r+.....trai
+00000c70: 6eda 0474 6573 74e9 0100 0000 da05 7374  n..test.......st
+00000c80: 6570 7329 03da 0f6e 756d 5f62 6f6f 7374  eps)...num_boost
+00000c90: 5f72 6f75 6e64 da15 6561 726c 795f 7374  _round..early_st
+00000ca0: 6f70 7069 6e67 5f72 6f75 6e64 73da 0565  opping_rounds..e
+00000cb0: 7661 6c73 7a11 4669 6e69 7368 6564 2074  valsz.Finished t
+00000cc0: 7261 696e 696e 6729 1772 0d00 0000 7202  raining).r....r.
+00000cd0: 0000 0072 1e00 0000 7222 0000 0072 1500  ...r....r"...r..
+00000ce0: 0000 7213 0000 00da 0a56 616c 7565 4572  ..r......ValueEr
+00000cf0: 726f 72da 0e61 7574 6f74 756e 655f 6d6f  ror..autotune_mo
+00000d00: 6465 6cda 0861 7574 6f74 756e 65da 0570  del..autotune..p
+00000d10: 7269 6e74 da1d 7573 655f 6675 6c6c 5f64  rint..use_full_d
+00000d20: 6174 615f 666f 725f 6669 6e61 6c5f 6d6f  ata_for_final_mo
+00000d30: 6465 6cda 0270 64da 0663 6f6e 6361 74da  del..pd..concat.
+00000d40: 0d73 616d 706c 655f 7765 6967 6874 7221  .sample_weightr!
+00000d50: 0000 00da 0378 6762 da07 444d 6174 7269  .....xgb..DMatri
+00000d60: 78da 1d63 6174 5f65 6e63 6f64 696e 675f  x..cat_encoding_
+00000d70: 7669 615f 6d6c 5f61 6c67 6f72 6974 686d  via_ml_algorithm
+00000d80: da14 6879 7065 7274 756e 696e 675f 6376  ..hypertuning_cv
+00000d90: 5f66 6f6c 6473 722d 0000 00da 0670 6172  _foldsr-.....par
+00000da0: 616d 7372 3200 0000 7216 0000 0029 0972  amsr2...r....).r
+00000db0: 1700 0000 7223 0000 0072 2400 0000 7225  ....r#...r$...r%
+00000dc0: 0000 0072 2600 0000 7220 0000 00da 0764  ...r&...r .....d
+00000dd0: 5f74 7261 696e da06 645f 7465 7374 da08  _train..d_test..
+00000de0: 6576 616c 5f73 6574 7218 0000 0072 1800  eval_setr....r..
+00000df0: 0000 7219 0000 00da 0366 6974 4700 0000  ..r......fitG...
+00000e00: 7364 0000 0000 0812 0108 020c 0108 0208  sd..............
+00000e10: 0110 0208 0208 0108 0102 010c ff04 040e  ................
+00000e20: 010e 0208 010a 0104 0102 0102 0102 0106  ................
+00000e30: fc08 0704 0102 0102 0106 fd06 0604 0102  ................
+00000e40: 0102 0106 fd06 0510 020e 0104 0106 0102  ................
+00000e50: 010a 0106 0102 fb0a 0804 0106 0102 010a  ................
+00000e60: 0106 0102 fb08 0708 017a 1058 6762 6f6f  .........z.Xgboo
+00000e70: 7374 4d6f 6465 6c2e 6669 7463 0500 0000  stModel.fitc....
+00000e80: 0000 0000 0000 0000 0b00 0000 1100 0000  ................
+00000e90: 0300 0000 7398 0100 0074 0074 01a0 02a1  ....s....t.t....
+00000ea0: 009b 0064 019d 0283 0101 0088 016a 0372  ...d.........j.r
+00000eb0: 1e88 016a 0473 2674 0564 0283 0182 0174  ...j.s&t.d.....t
+00000ec0: 066a 077c 0288 0488 016a 046a 0864 038d  .j.|.....j.j.d..
+00000ed0: 0389 0074 0983 0089 0288 01a0 0aa1 0001  ...t............
+00000ee0: 0088 016a 0372 5a88 016a 0472 5a88 016a  ...j.rZ..j.rZ..j
+00000ef0: 0b73 6274 0564 0483 0182 0187 0087 0187  .sbt.d..........
+00000f00: 0287 0387 0487 0566 0664 0564 0684 087d  .......f.d.d...}
+00000f10: 0564 077d 0674 0c6a 0d6a 0e64 0888 016a  .d.}.t.j.j.d...j
+00000f20: 046a 0f64 098d 027d 0774 0c6a 1064 0a7c  .j.d...}.t.j.d.|
+00000f30: 077c 069b 0064 0b9d 0264 0c8d 037d 087c  .|...d...d...}.|
+00000f40: 086a 117c 0588 016a 046a 1288 016a 046a  .j.|...j.j...j.j
+00000f50: 1364 0d64 0d64 0e8d 0501 007a 2c74 0c6a  .d.d.d.....z,t.j
+00000f60: 14a0 157c 08a1 017d 097c 09a0 16a1 0001  ...|...}.|......
+00000f70: 0074 0c6a 14a0 177c 08a1 017d 097c 09a0  .t.j...|...}.|..
+00000f80: 16a1 0001 0057 006e 1c04 0074 1874 1974  .....W.n...t.t.t
+00000f90: 0566 036b 0a90 0172 0a01 0001 0001 0059  .f.k...r.......Y
+00000fa0: 006e 0258 007c 086a 1a6a 1b7d 0a88 016a  .n.X.|.j.j.}...j
+00000fb0: 0b6a 1c88 016a 0b6a 1d88 016a 0b6a 1e88  .j...j.j...j.j..
+00000fc0: 016a 0b6a 1f88 0288 05a0 20a1 007c 0a64  .j.j...... ..|.d
+00000fd0: 0f19 007c 0a64 1019 007c 0a64 1119 007c  ...|.d...|.d...|
+00000fe0: 0a64 1219 007c 0a64 1319 007c 0a64 1419  .d...|.d...|.d..
+00000ff0: 007c 0a64 1519 007c 0a64 1619 007c 0a64  .|.d...|.d...|.d
+00001000: 1719 007c 0a64 1819 0064 199c 1088 016a  ...|.d...d.....j
+00001010: 035f 1b74 2164 1a88 016a 036a 1b83 0201  ._.t!d...j.j....
+00001020: 007c 0a64 1b19 0088 016a 035f 2264 1c53  .|.d.....j._"d.S
+00001030: 0029 1d7a 7b54 756e 6520 6879 7065 7270  .).z{Tune hyperp
+00001040: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+00001050: 2020 2020 416e 2061 6c74 6572 6e61 7469      An alternati
+00001060: 7665 2063 6f6e 6669 6720 6361 6e20 6265  ve config can be
+00001070: 2070 726f 7669 6465 6420 746f 206f 7665   provided to ove
+00001080: 7277 7269 7465 2074 6865 2068 7970 6572  rwrite the hyper
+00001090: 7061 7261 6d65 7465 7220 7365 6172 6368  parameter search
+000010a0: 2073 7061 6365 2e0a 2020 2020 2020 2020   space..        
+000010b0: 7a2f 3a20 5374 6172 7420 6879 7065 7270  z/: Start hyperp
+000010c0: 6172 616d 6574 6572 2074 756e 696e 6720  arameter tuning 
+000010d0: 6f66 2058 6762 6f6f 7374 206d 6f64 656c  of Xgboost model
+000010e0: 2e72 2700 0000 722c 0000 007a 3941 7420  .r'...r,...z9At 
+000010f0: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
+00001100: 2063 6f6e 6669 6773 2069 7320 4e6f 6e65   configs is None
+00001110: 2c20 7768 6963 6820 6973 206e 6f74 2061  , which is not a
+00001120: 6c6c 6f77 6564 6301 0000 0000 0000 0000  llowedc.........
+00001130: 0000 000c 0000 0014 0000 0013 0000 0073  ...............s
+00001140: 0802 0000 8801 6a00 6a01 8801 6a00 6a02  ......j.j...j.j.
+00001150: 8801 6a00 6a03 8801 6a00 6a04 8802 8805  ..j.j...j.j.....
+00001160: a005 a100 7c00 a006 6401 8801 6a00 6a07  ....|...d...j.j.
+00001170: 8801 6a00 6a08 a103 7c00 a009 6402 8801  ..j.j...|...d...
+00001180: 6a00 6a0a 8801 6a00 6a0b a103 7c00 a006  j.j...j.j...|...
+00001190: 6403 8801 6a00 6a0c 8801 6a00 6a0d a103  d...j.j...j.j...
+000011a0: 7c00 a006 6404 8801 6a00 6a0e 8801 6a00  |...d...j.j...j.
+000011b0: 6a0f a103 7c00 a006 6405 8801 6a00 6a10  j...|...d...j.j.
+000011c0: 8801 6a00 6a11 a103 7c00 a009 6406 8801  ..j.j...|...d...
+000011d0: 6a00 6a12 8801 6a00 6a13 a103 7c00 a006  j.j...j.j...|...
+000011e0: 6407 8801 6a00 6a14 8801 6a00 6a15 a103  d...j.j...j.j...
+000011f0: 7c00 a006 6408 8801 6a00 6a16 8801 6a00  |...d...j.j...j.
+00001200: 6a17 a103 7c00 a006 6409 8801 6a00 6a18  j...|...d...j.j.
+00001210: 8801 6a00 6a19 a103 7c00 a009 640a 8801  ..j.j...|...d...
+00001220: 6a00 6a1a 8801 6a00 6a1b a103 640b 9c10  j.j...j.j...d...
+00001230: 7d01 7c00 a01c 640c 640d 640e 6702 a102  }.|...d.d.d.g...
+00001240: 7d02 7c02 9001 7226 8801 a01d 8805 a101  }.|...r&........
+00001250: 7d03 741e 6a1f 8803 8805 7c03 8801 6a20  }.t.j.....|...j 
+00001260: 6a21 640f 8d04 7d04 6e14 741e 6a1f 8803  j!d...}.n.t.j...
+00001270: 8805 8801 6a20 6a21 6410 8d03 7d04 7422  ....j j!d...}.t"
+00001280: 6a23 a024 7c00 6411 a102 7d05 8801 6a20  j#.$|.d...}...j 
+00001290: 6a25 6412 6b02 9001 72bc 7c04 6413 6602  j%d.k...r.|.d.f.
+000012a0: 8800 6414 6602 6702 7d06 741e 6a26 7c01  ..d.f.g.}.t.j&|.
+000012b0: 7c04 7c01 640a 1900 8801 6a20 6a27 7c06  |.|.d.....j j'|.
+000012c0: 7c05 6701 8801 6a00 6a04 6415 8d07 7d07  |.g...j.j.d...}.
+000012d0: 7c07 a028 8800 a101 7d08 7429 a02a 6416  |..(....}.t).*d.
+000012e0: 6417 8400 7c08 4400 8301 a101 7d09 742b  d...|.D.....}.t+
+000012f0: 8804 7c09 8302 6418 1400 7d0a 7c0a 5300  ..|...d...}.|.S.
+00001300: 741e 6a2c 7c01 7c04 7c01 640a 1900 8801  t.j,|.|.|.d.....
+00001310: 6a20 6a25 640d 8801 6a20 6a2d 7c05 6701  j j%d...j j-|.g.
+00001320: 8801 6a20 6a2e 6419 8d08 7d0b 7c0b 641a  ..j j.d...}.|.d.
+00001330: 1900 a02f a100 7c0b 641a 1900 a030 a100  .../..|.d....0..
+00001340: 641b 1300 1700 5300 6400 5300 291c 4eda  d.....S.d.S.).N.
+00001350: 0365 7461 da09 6d61 785f 6465 7074 68da  .eta..max_depth.
+00001360: 0561 6c70 6861 da06 6c61 6d62 6461 da10  .alpha..lambda..
+00001370: 6d69 6e5f 6368 696c 645f 7765 6967 6874  min_child_weight
+00001380: da0a 6e75 6d5f 6c65 6176 6573 da09 7375  ..num_leaves..su
+00001390: 6273 616d 706c 65da 1063 6f6c 7361 6d70  bsample..colsamp
+000013a0: 6c65 5f62 7974 7265 65da 1163 6f6c 7361  le_bytree..colsa
+000013b0: 6d70 6c65 5f62 796c 6576 656c 7230 0000  mple_bylevelr0..
+000013c0: 0029 10da 096f 626a 6563 7469 7665 da07  .)...objective..
+000013d0: 626f 6f73 7465 72da 0b65 7661 6c5f 6d65  booster..eval_me
+000013e0: 7472 6963 da07 7665 7262 6f73 65da 0b74  tric..verbose..t
+000013f0: 7265 655f 6d65 7468 6f64 da09 6e75 6d5f  ree_method..num_
+00001400: 636c 6173 7372 4500 0000 7246 0000 0072  classrE...rF...r
+00001410: 4700 0000 7248 0000 0072 4900 0000 724a  G...rH...rI...rJ
+00001420: 0000 0072 4b00 0000 724c 0000 0072 4d00  ...rK...rL...rM.
+00001430: 0000 7230 0000 0072 3b00 0000 5446 7228  ..r0...r;...TFr(
+00001440: 0000 0072 2c00 0000 7a0d 7465 7374 2d6d  ...r,...z.test-m
+00001450: 6c6f 676c 6f73 7372 2f00 0000 722d 0000  loglossr/...r-..
+00001460: 0072 2e00 0000 2905 7231 0000 0072 3200  .r....).r1...r2.
+00001470: 0000 7233 0000 00da 0963 616c 6c62 6163  ..r3.....callbac
+00001480: 6b73 da0c 7665 7262 6f73 655f 6576 616c  ks..verbose_eval
+00001490: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000014a0: 0005 0000 0053 0000 0073 1600 0000 6700  .....S...s....g.
+000014b0: 7c00 5d0e 7d01 7400 a001 7c01 a101 9102  |.].}.t...|.....
+000014c0: 7104 5300 7218 0000 00a9 02da 026e 70da  q.S.r........np.
+000014d0: 0661 7267 6d61 78a9 02da 022e 30da 046c  .argmax.....0..l
+000014e0: 696e 6572 1800 0000 7218 0000 0072 1900  iner....r....r..
+000014f0: 0000 da0a 3c6c 6973 7463 6f6d 703e 0001  ....<listcomp>..
+00001500: 0000 7304 0000 0006 0002 007a 3c58 6762  ..s........z<Xgb
+00001510: 6f6f 7374 4d6f 6465 6c2e 6175 746f 7475  oostModel.autotu
+00001520: 6e65 2e3c 6c6f 6361 6c73 3e2e 6f62 6a65  ne.<locals>.obje
+00001530: 6374 6976 652e 3c6c 6f63 616c 733e 2e3c  ctive.<locals>.<
+00001540: 6c69 7374 636f 6d70 3ee9 ffff ffff 2908  listcomp>.....).
+00001550: 7240 0000 00da 0664 7472 6169 6e72 3100  r@.....dtrainr1.
+00001560: 0000 da05 6e66 6f6c 64da 0961 735f 7061  ....nfold..as_pa
+00001570: 6e64 6173 da04 7365 6564 7254 0000 00da  ndas..seedrT....
+00001580: 0773 6875 6666 6c65 7a12 7465 7374 2d6d  .shufflez.test-m
+00001590: 6c6f 676c 6f73 732d 6d65 616e 6766 6666  logloss-meangfff
+000015a0: 6666 66e6 3f29 3172 1400 0000 da0f 6d6f  fff.?)1r......mo
+000015b0: 6465 6c5f 6f62 6a65 6374 6976 6572 4f00  del_objectiverO.
+000015c0: 0000 da11 6d6f 6465 6c5f 6576 616c 5f6d  ....model_eval_m
+000015d0: 6574 7269 63da 0f6d 6f64 656c 5f76 6572  etric..model_ver
+000015e0: 626f 7369 7479 da07 6e75 6e69 7175 65da  bosity..nunique.
+000015f0: 0d73 7567 6765 7374 5f66 6c6f 6174 da07  .suggest_float..
+00001600: 6574 615f 6d69 6eda 0765 7461 5f6d 6178  eta_min..eta_max
+00001610: da0b 7375 6767 6573 745f 696e 74da 0d6d  ..suggest_int..m
+00001620: 6178 5f64 6570 7468 5f6d 696e da0d 6d61  ax_depth_min..ma
+00001630: 785f 6465 7074 685f 6d61 78da 0961 6c70  x_depth_max..alp
+00001640: 6861 5f6d 696e da09 616c 7068 615f 6d61  ha_min..alpha_ma
+00001650: 78da 0a6c 616d 6264 615f 6d69 6eda 0a6c  x..lambda_min..l
+00001660: 616d 6264 615f 6d61 78da 146d 696e 5f63  ambda_max..min_c
+00001670: 6869 6c64 5f77 6569 6768 745f 6d69 6eda  hild_weight_min.
+00001680: 146d 696e 5f63 6869 6c64 5f77 6569 6768  .min_child_weigh
+00001690: 745f 6d61 78da 0e6e 756d 5f6c 6561 7665  t_max..num_leave
+000016a0: 735f 6d69 6eda 0e6e 756d 5f6c 6561 7665  s_min..num_leave
+000016b0: 735f 6d61 78da 0e73 7562 5f73 616d 706c  s_max..sub_sampl
+000016c0: 655f 6d69 6eda 0e73 7562 5f73 616d 706c  e_min..sub_sampl
+000016d0: 655f 6d61 78da 1663 6f6c 5f73 616d 706c  e_max..col_sampl
+000016e0: 655f 6279 5f74 7265 655f 6d69 6eda 1663  e_by_tree_min..c
+000016f0: 6f6c 5f73 616d 706c 655f 6279 5f74 7265  ol_sample_by_tre
+00001700: 655f 6d61 78da 1763 6f6c 5f73 616d 706c  e_max..col_sampl
+00001710: 655f 6279 5f6c 6576 656c 5f6d 696e da17  e_by_level_min..
+00001720: 636f 6c5f 7361 6d70 6c65 5f62 795f 6c65  col_sample_by_le
+00001730: 7665 6c5f 6d61 78da 0973 7465 7073 5f6d  vel_max..steps_m
+00001740: 696e da09 7374 6570 735f 6d61 78da 1373  in..steps_max..s
+00001750: 7567 6765 7374 5f63 6174 6567 6f72 6963  uggest_categoric
+00001760: 616c 7221 0000 0072 3c00 0000 723d 0000  alr!...r<...r=..
+00001770: 0072 1300 0000 723e 0000 00da 066f 7074  .r....r>.....opt
+00001780: 756e 61da 0b69 6e74 6567 7261 7469 6f6e  una..integration
+00001790: da16 5847 426f 6f73 7450 7275 6e69 6e67  ..XGBoostPruning
+000017a0: 4361 6c6c 6261 636b 723f 0000 0072 2d00  Callbackr?...r-.
+000017b0: 0000 7232 0000 00da 0770 7265 6469 6374  ..r2.....predict
+000017c0: 7257 0000 00da 0761 7361 7272 6179 7207  rW.....asarrayr.
+000017d0: 0000 00da 0263 76da 1367 6c6f 6261 6c5f  .....cv..global_
+000017e0: 7261 6e64 6f6d 5f73 7461 7465 da17 7368  random_state..sh
+000017f0: 7566 666c 655f 6475 7269 6e67 5f74 7261  uffle_during_tra
+00001800: 696e 696e 67da 046d 6561 6eda 0373 7464  ining..mean..std
+00001810: 290c da05 7472 6961 6cda 0570 6172 616d  )...trial..param
+00001820: 723b 0000 0072 2000 0000 7241 0000 00da  r;...r ...rA....
+00001830: 1070 7275 6e69 6e67 5f63 616c 6c62 6163  .pruning_callbac
+00001840: 6b72 4300 0000 7216 0000 00da 0570 7265  krC...r......pre
+00001850: 6473 da0b 7072 6564 5f6c 6162 656c 73da  ds..pred_labels.
+00001860: 076d 6174 7468 6577 da06 7265 7375 6c74  .matthew..result
+00001870: a906 7242 0000 0072 1700 0000 da08 7472  ..rB...r......tr
+00001880: 6169 6e5f 6f6e 7223 0000 0072 2600 0000  ain_onr#...r&...
+00001890: 7225 0000 0072 1800 0000 7219 0000 0072  r%...r....r....r
+000018a0: 4e00 0000 ad00 0000 73ce 0000 0000 0206  N.......s.......
+000018b0: 0106 0106 0106 0102 0106 0104 0102 0006  ................
+000018c0: 0006 ff02 0304 0102 0106 0106 fd02 0504  ................
+000018d0: 0102 0006 0006 ff02 0304 0102 0006 0006  ................
+000018e0: ff02 0304 0102 0106 0106 fd02 0504 0102  ................
+000018f0: 0106 0106 fd02 0504 0102 0106 0106 fd02  ................
+00001900: 0504 0102 0106 0106 fd02 0504 0102 0106  ................
+00001910: 0106 fd02 0504 0102 0006 0006 ff02 d206  ................
+00001920: 3210 0106 010a 0104 0102 0102 0102 0106  2...............
+00001930: fc08 0704 0102 0102 0106 fd06 0606 0102  ................
+00001940: 0002 ff04 040e 0110 0104 0102 0102 0106  ................
+00001950: 0106 0102 0104 0106 f906 090a 0114 010e  ................
+00001960: 0104 0204 0102 0102 0106 0206 0102 0106  ................
+00001970: 0104 0106 f706 0c0a 010e ff7a 2858 6762  ...........z(Xgb
+00001980: 6f6f 7374 4d6f 6465 6c2e 6175 746f 7475  oostModel.autotu
+00001990: 6e65 2e3c 6c6f 6361 6c73 3e2e 6f62 6a65  ne.<locals>.obje
+000019a0: 6374 6976 65da 0778 6762 6f6f 7374 4629  ctive..xgboostF)
+000019b0: 02da 0c6d 756c 7469 7661 7269 6174 6572  ...multivariater
+000019c0: 6100 0000 da08 6d69 6e69 6d69 7a65 7a07  a.....minimizez.
+000019d0: 2074 756e 696e 6729 03da 0964 6972 6563   tuning)...direc
+000019e0: 7469 6f6e da07 7361 6d70 6c65 72da 0a73  tion..sampler..s
+000019f0: 7475 6479 5f6e 616d 6554 2904 da08 6e5f  tudy_nameT)...n_
+00001a00: 7472 6961 6c73 da07 7469 6d65 6f75 74da  trials..timeout.
+00001a10: 0e67 635f 6166 7465 725f 7472 6961 6cda  .gc_after_trial.
+00001a20: 1173 686f 775f 7072 6f67 7265 7373 5f62  .show_progress_b
+00001a30: 6172 7246 0000 0072 4700 0000 7248 0000  arrF...rG...rH..
+00001a40: 0072 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
+00001a50: 724d 0000 0072 4900 0000 7245 0000 0072  rM...rI...rE...r
+00001a60: 3000 0000 2910 724e 0000 0072 4f00 0000  0...).rN...rO...
+00001a70: 7250 0000 0072 5100 0000 7252 0000 0072  rP...rQ...rR...r
+00001a80: 5300 0000 7246 0000 0072 4700 0000 7248  S...rF...rG...rH
+00001a90: 0000 0072 4a00 0000 724b 0000 0072 4c00  ...rJ...rK...rL.
+00001aa0: 0000 724d 0000 0072 4900 0000 7245 0000  ..rM...rI...rE..
+00001ab0: 0072 3000 0000 7a0d 4265 7374 2070 6172  .r0...z.Best par
+00001ac0: 616d 733a 2072 3b00 0000 4e29 2372 0d00  ams: r;...N)#r..
+00001ad0: 0000 7202 0000 0072 1e00 0000 7215 0000  ..r....r....r...
+00001ae0: 0072 1300 0000 7234 0000 0072 3c00 0000  .r....r4...r<...
+00001af0: 723d 0000 0072 3e00 0000 720c 0000 0072  r=...r>...r....r
+00001b00: 2200 0000 7214 0000 0072 7e00 0000 da08  "...r....r~.....
+00001b10: 7361 6d70 6c65 7273 da0a 5450 4553 616d  samplers..TPESam
+00001b20: 706c 6572 7284 0000 00da 0c63 7265 6174  plerr......creat
+00001b30: 655f 7374 7564 79da 086f 7074 696d 697a  e_study..optimiz
+00001b40: 65da 1c68 7970 6572 7061 7261 6d65 7465  e..hyperparamete
+00001b50: 725f 7475 6e69 6e67 5f72 6f75 6e64 73da  r_tuning_rounds.
+00001b60: 2668 7970 6572 7061 7261 6d65 7465 725f  &hyperparameter_
+00001b70: 7475 6e69 6e67 5f6d 6178 5f72 756e 7469  tuning_max_runti
+00001b80: 6d65 5f73 6563 73da 0d76 6973 7561 6c69  me_secs..visuali
+00001b90: 7a61 7469 6f6e da19 706c 6f74 5f6f 7074  zation..plot_opt
+00001ba0: 696d 697a 6174 696f 6e5f 6869 7374 6f72  imization_histor
+00001bb0: 79da 0473 686f 77da 1670 6c6f 745f 7061  y..show..plot_pa
+00001bc0: 7261 6d5f 696d 706f 7274 616e 6365 73da  ram_importances.
+00001bd0: 115a 6572 6f44 6976 6973 696f 6e45 7272  .ZeroDivisionErr
+00001be0: 6f72 da0c 5275 6e74 696d 6545 7272 6f72  or..RuntimeError
+00001bf0: da0a 6265 7374 5f74 7269 616c 7240 0000  ..best_trialr@..
+00001c00: 0072 6300 0000 724f 0000 0072 6400 0000  .rc...rO...rd...
+00001c10: 7265 0000 0072 6600 0000 7237 0000 0072  re...rf...r7...r
+00001c20: 3b00 0000 290b 7217 0000 0072 2300 0000  ;...).r....r#...
+00001c30: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00001c40: 4e00 0000 da09 616c 676f 7269 7468 6d72  N.....algorithmr
+00001c50: 9500 0000 da05 7374 7564 79da 0366 6967  ......study..fig
+00001c60: 5a12 7867 626f 6f73 745f 6265 7374 5f70  Z.xgboost_best_p
+00001c70: 6172 616d 7218 0000 0072 8f00 0000 7219  aramr....r....r.
+00001c80: 0000 0072 3600 0000 8c00 0000 7384 0000  ...r6.......s...
+00001c90: 0000 0b12 010c 0108 0204 0102 0102 0106  ................
+00001ca0: fd06 0506 0208 0304 ff02 0204 fe02 0304  ................
+00001cb0: fd02 0502 0102 ff04 0416 6704 0106 0102  ..........g.....
+00001cc0: 0006 ff06 0304 0102 0102 0108 fd06 0604  ................
+00001cd0: 0102 0106 0106 0102 0102 fb06 0702 010c  ................
+00001ce0: 0108 010c 010c 0116 0106 0208 0206 0106  ................
+00001cf0: 0106 0106 0102 0106 0102 0102 ff02 0306  ................
+00001d00: 0106 0106 0106 0106 0106 0106 0106 0106  ................
+00001d10: ee0a 140e 017a 1558 6762 6f6f 7374 4d6f  .....z.XgboostMo
+00001d20: 6465 6c2e 6175 746f 7475 6e65 2902 da02  del.autotune)...
+00001d30: 6466 721c 0000 0063 0200 0000 0000 0000  dfr....c........
+00001d40: 0000 0000 0600 0000 0400 0000 4300 0000  ............C...
+00001d50: 73b4 0000 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
+00001d60: 019d 0283 0101 007c 006a 0372 1e7c 006a  .......|.j.r.|.j
+00001d70: 0473 2674 0564 0283 0182 0174 066a 077c  .s&t.d.....t.j.|
+00001d80: 017c 006a 046a 0864 038d 027d 027c 006a  .|.j.j.d...}.|.j
+00001d90: 0973 4674 0a64 0483 0182 017c 006a 0b73  .sFt.d.....|.j.s
+00001da0: 5474 0a64 0583 0182 017c 006a 09a0 0c7c  Tt.d.....|.j...|
+00001db0: 02a1 017d 037c 006a 0d64 066b 0272 8c74  ...}.|.j.d.k.r.t
+00001dc0: 0ea0 0f64 0764 0884 007c 0344 0083 01a1  ...d.d...|.D....
+00001dd0: 017d 047c 047c 006a 0b6a 106b 047d 056e  .}.|.|.j.j.k.}.n
+00001de0: 187c 037d 0474 0ea0 0f64 0964 0884 007c  .|.}.t...d.d...|
+00001df0: 0344 0083 01a1 017d 0574 1164 0a83 0101  .D.....}.t.d....
+00001e00: 007c 047c 0566 0253 0029 0b7a 1750 7265  .|.|.f.S.).z.Pre
+00001e10: 6469 6374 206f 6e20 756e 7365 656e 2064  dict on unseen d
+00001e20: 6174 612e 7a33 3a20 5374 6172 7420 7072  ata.z3: Start pr
+00001e30: 6564 6963 7469 6e67 206f 6e20 6e65 7720  edicting on new 
+00001e40: 6461 7461 2075 7369 6e67 2058 6762 6f6f  data using Xgboo
+00001e50: 7374 206d 6f64 656c 2e72 2700 0000 2901  st model.r'...).
+00001e60: 722b 0000 007a 204e 6f20 7472 6169 6e65  r+...z No traine
+00001e70: 6420 6d6f 6465 6c20 6861 7320 6265 656e  d model has been
+00001e80: 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f 6465   found.z+No mode
+00001e90: 6c20 636f 6e66 6967 7572 6174 696f 6e20  l configuration 
+00001ea0: 6669 6c65 2068 6173 2062 6565 6e20 666f  file has been fo
+00001eb0: 756e 642e 7210 0000 0063 0100 0000 0000  und.r....c......
+00001ec0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00001ed0: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
+00001ee0: 0164 0019 0091 0271 0453 0029 0172 2f00  .d.....q.S.).r/.
+00001ef0: 0000 7218 0000 0072 5900 0000 7218 0000  ..r....rY...r...
+00001f00: 0072 1800 0000 7219 0000 0072 5c00 0000  .r....r....r\...
+00001f10: 5a01 0000 7304 0000 0006 0002 007a 2858  Z...s........z(X
+00001f20: 6762 6f6f 7374 4d6f 6465 6c2e 7072 6564  gboostModel.pred
+00001f30: 6963 742e 3c6c 6f63 616c 733e 2e3c 6c69  ict.<locals>.<li
+00001f40: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+00001f50: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001f60: 7316 0000 0067 007c 005d 0e7d 0174 00a0  s....g.|.].}.t..
+00001f70: 017c 01a1 0191 0271 0453 0072 1800 0000  .|.....q.S.r....
+00001f80: 7256 0000 0072 5900 0000 7218 0000 0072  rV...rY...r....r
+00001f90: 1800 0000 7219 0000 0072 5c00 0000 6001  ....r....r\...`.
+00001fa0: 0000 7304 0000 0006 0002 007a 1346 696e  ..s........z.Fin
+00001fb0: 6973 6865 6420 7072 6564 6963 7469 6e67  ished predicting
+00001fc0: 2912 720d 0000 0072 0200 0000 721e 0000  ).r....r....r...
+00001fd0: 0072 1400 0000 7213 0000 0072 3400 0000  .r....r....r4...
+00001fe0: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+00001ff0: 1600 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
+00002000: 1500 0000 7281 0000 0072 1200 0000 7257  ....r....r....rW
+00002010: 0000 0072 8200 0000 da18 636c 6173 7369  ...r......classi
+00002020: 6669 6361 7469 6f6e 5f74 6872 6573 686f  fication_thresho
+00002030: 6c64 7237 0000 0029 0672 1700 0000 72ab  ldr7...).r....r.
+00002040: 0000 0072 4200 0000 da0d 7061 7274 6961  ...rB.....partia
+00002050: 6c5f 7072 6f62 73da 0f70 7265 6469 6374  l_probs..predict
+00002060: 6564 5f70 726f 6273 da11 7072 6564 6963  ed_probs..predic
+00002070: 7465 645f 636c 6173 7365 7372 1800 0000  ted_classesr....
+00002080: 7218 0000 0072 1900 0000 7281 0000 0045  r....r....r....E
+00002090: 0100 0073 2c00 0000 0002 0201 0cff 0403  ...s,...........
+000020a0: 0c01 0802 0401 0201 06fe 0605 0601 0802  ................
+000020b0: 0601 0802 0c01 0a01 1402 0aff 0404 0401  ................
+000020c0: 1401 0801 7a14 5867 626f 6f73 744d 6f64  ....z.XgboostMod
+000020d0: 656c 2e70 7265 6469 6374 2903 4e4e 4e29  el.predict).NNN)
+000020e0: 1ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000020f0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00002100: 616d 655f 5fda 075f 5f64 6f63 5f5f 7204  ame__..__doc__r.
+00002110: 0000 0072 0500 0000 7209 0000 0072 0b00  ...r....r....r..
+00002120: 0000 720a 0000 0072 1a00 0000 7239 0000  ..r....r....r9..
+00002130: 00da 0653 6572 6965 7372 0300 0000 da03  ...Seriesr......
+00002140: 7374 72da 0566 6c6f 6174 7221 0000 0072  str..floatr!...r
+00002150: 2200 0000 da09 4461 7461 4672 616d 6572  ".....DataFramer
+00002160: 3c00 0000 da07 426f 6f73 7465 7272 4400  <.....BoosterrD.
+00002170: 0000 7236 0000 0072 0600 0000 7257 0000  ..r6...r....rW..
+00002180: 00da 076e 6461 7272 6179 7281 0000 0072  ...ndarrayr....r
+00002190: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+000021a0: 0000 0072 0f00 0000 1a00 0000 7334 0000  ...r........s4..
+000021b0: 0008 0104 0500 0100 0100 fb02 0206 0106  ................
+000021c0: 0106 0106 fb0c 0d1a 0808 1704 0104 0104  ................
+000021d0: 0104 0104 fa0c 4704 0104 0104 0104 0102  ......G.........
+000021e0: fa0c 7f00 3a72 0f00 0000 291c 72b4 0000  ....:r....).r...
+000021f0: 0072 0200 0000 da06 7479 7069 6e67 7203  .r......typingr.
+00002200: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
+00002210: 0000 da05 6e75 6d70 7972 5700 0000 727e  ....numpyrW...r~
+00002220: 0000 00da 0670 616e 6461 7372 3900 0000  .....pandasr9...
+00002230: 7291 0000 0072 3c00 0000 da0f 736b 6c65  r....r<.....skle
+00002240: 6172 6e2e 6d65 7472 6963 7372 0700 0000  arn.metricsr....
+00002250: 5a0d 736b 6c65 6172 6e2e 7574 696c 7372  Z.sklearn.utilsr
+00002260: 0800 0000 da1f 626c 7565 6361 7374 2e63  ......bluecast.c
+00002270: 6f6e 6669 672e 7472 6169 6e69 6e67 5f63  onfig.training_c
+00002280: 6f6e 6669 6772 0900 0000 720a 0000 0072  onfigr....r....r
+00002290: 0b00 0000 da24 626c 7565 6361 7374 2e67  .....$bluecast.g
+000022a0: 656e 6572 616c 5f75 7469 6c73 2e67 656e  eneral_utils.gen
+000022b0: 6572 616c 5f75 7469 6c73 720c 0000 0072  eral_utilsr....r
+000022c0: 0d00 0000 5a22 626c 7565 6361 7374 2e6d  ....Z"bluecast.m
+000022d0: 6c5f 6d6f 6465 6c6c 696e 672e 6261 7365  l_modelling.base
+000022e0: 5f63 6c61 7373 6573 720e 0000 0072 0f00  _classesr....r..
+000022f0: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00002300: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00002310: 0100 0000 7318 0000 0004 060c 0118 0208  ....s...........
+00002320: 0108 0108 0108 010c 010c 0214 0510 010c  ................
+00002330: 03                                       .
```

### Comparing `bluecast-0.7/bluecast/ml_modelling/base_classes.py` & `bluecast-0.8/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/ml_modelling/xgboost.py` & `bluecast-0.8/bluecast/ml_modelling/xgboost.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 evals=eval_set,
             )
         else:
             self.model = xgb.train(
                 self.conf_params_xgboost.params,
                 d_train,
                 num_boost_round=self.conf_params_xgboost.params["steps"],
-                # early_stopping_rounds=self.conf_training.early_stopping_rounds,
+                early_stopping_rounds=self.conf_training.early_stopping_rounds,
                 evals=eval_set,
             )
         print("Finished training")
         return self.model
 
     def autotune(
         self,
@@ -169,18 +169,22 @@
             raise ValueError(
                 "At least one of the configs is None, which is not allowed"
             )
 
         def objective(trial):
             param = {
                 "objective": self.conf_xgboost.model_objective,
+                "booster": self.conf_xgboost.booster,
                 "eval_metric": self.conf_xgboost.model_eval_metric,
                 "verbose": self.conf_xgboost.model_verbosity,
                 "tree_method": train_on,
                 "num_class": y_train.nunique(),
+                "eta": trial.suggest_float(
+                    "eta", self.conf_xgboost.eta_min, self.conf_xgboost.eta_max
+                ),
                 "max_depth": trial.suggest_int(
                     "max_depth",
                     self.conf_xgboost.max_depth_min,
                     self.conf_xgboost.max_depth_max,
                 ),
                 "alpha": trial.suggest_float(
                     "alpha", self.conf_xgboost.alpha_min, self.conf_xgboost.alpha_max
@@ -209,15 +213,14 @@
                     self.conf_xgboost.col_sample_by_tree_max,
                 ),
                 "colsample_bylevel": trial.suggest_float(
                     "colsample_bylevel",
                     self.conf_xgboost.col_sample_by_level_min,
                     self.conf_xgboost.col_sample_by_level_max,
                 ),
-                "eta": self.conf_xgboost.eta,
                 "steps": trial.suggest_int(
                     "steps", self.conf_xgboost.steps_min, self.conf_xgboost.steps_max
                 ),
             }
             sample_weight = trial.suggest_categorical("sample_weight", [True, False])
             if sample_weight:
                 classes_weights = self.calculate_class_weights(y_train)
@@ -262,15 +265,17 @@
                     nfold=self.conf_training.hypertuning_cv_folds,
                     as_pandas=True,
                     seed=self.conf_training.global_random_state,
                     callbacks=[pruning_callback],
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
-                return result["test-mlogloss-mean"].mean()
+                return result["test-mlogloss-mean"].mean() + (
+                    result["test-mlogloss-mean"].std() ** 0.7
+                )
 
         algorithm = "xgboost"
         sampler = optuna.samplers.TPESampler(
             multivariate=False, seed=self.conf_training.global_random_state
         )
         study = optuna.create_study(
             direction="minimize",
@@ -292,29 +297,30 @@
             fig.show()
         except (ZeroDivisionError, RuntimeError, ValueError):
             pass
 
         xgboost_best_param = study.best_trial.params
         self.conf_params_xgboost.params = {
             "objective": self.conf_xgboost.model_objective,  # OR  'binary:logistic' #the loss function being used
+            "booster": self.conf_xgboost.booster,
             "eval_metric": self.conf_xgboost.model_eval_metric,
             "verbose": self.conf_xgboost.model_verbosity,
             "tree_method": train_on,  # use GPU for training
             "num_class": y_train.nunique(),
             "max_depth": xgboost_best_param[
                 "max_depth"
             ],  # maximum depth of the decision trees being trained
             "alpha": xgboost_best_param["alpha"],
             "lambda": xgboost_best_param["lambda"],
             "num_leaves": xgboost_best_param["num_leaves"],
             "subsample": xgboost_best_param["subsample"],
             "colsample_bytree": xgboost_best_param["colsample_bytree"],
             "colsample_bylevel": xgboost_best_param["colsample_bylevel"],
             "min_child_weight": xgboost_best_param["min_child_weight"],
-            "eta": self.conf_xgboost.eta,
+            "eta": xgboost_best_param["eta"],
             "steps": xgboost_best_param["steps"],
         }
         print("Best params: ", self.conf_params_xgboost.params)
         self.conf_params_xgboost.sample_weight = xgboost_best_param["sample_weight"]
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data."""
```

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-0.8/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/custom.py` & `bluecast-0.8/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/datetime_features.py` & `bluecast-0.8/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.8/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/feature_selection.py` & `bluecast-0.8/bluecast/preprocessing/feature_selection.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/feature_types.py` & `bluecast-0.8/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.8/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/schema_checks.py` & `bluecast-0.8/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/target_encoding.py` & `bluecast-0.8/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/preprocessing/train_test_split.py` & `bluecast-0.8/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 10:57:29 2023 UTC, .py size: 1176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9963 9d64 9804 0000  o........c.d....
+00000000: 6f0d 0d0a 0000 0000 9874 9e64 9804 0000  o........t.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
 00000060: 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c 6d0d  l.Z.d.d.l.m.Z.m.
 00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6400 6404  Z.m.Z.m.Z...d.d.
```

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 28 11:19:35 2023 UTC, .py size: 6677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4717 9c64 151a 0000  o.......G..d....
+00000000: 6f0d 0d0a 0000 0000 9874 9e64 151a 0000  o........t.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
 00000060: 6400 6401 6c0b 5a0c 6400 6401 6c0d 5a0d  d.d.l.Z.d.d.l.Z.
 00000070: 6400 6401 6c0e 5a0f 6400 6403 6c10 6d11  d.d.l.Z.d.d.l.m.
```

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.8/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.8/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/make_data/create_data.py` & `bluecast-0.8/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_analyse.py` & `bluecast-0.8/bluecast/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_cast.py` & `bluecast-0.8/bluecast/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.8/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.8/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_datetime_features.py` & `bluecast-0.8/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.8/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.8/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_load_for_production.py` & `bluecast-0.8/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.8/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_save_to_production.py` & `bluecast-0.8/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_schema_checks.py` & `bluecast-0.8/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_shap_explanations.py` & `bluecast-0.8/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.8/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.8/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/bluecast/tests/test_train_test_split.py` & `bluecast-0.8/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.7/pyproject.toml` & `bluecast-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.7"
+version = "0.8"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `bluecast-0.7/PKG-INFO` & `bluecast-0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.7
+Version: 0.8
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -61,15 +61,17 @@
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
     * [Explanatory analysis](#explanatory-analysis)
     * [Enable cross-validation](#enable-cross-validation)
+    * [Use multi-model blended pipeline](#use-multi-model-blended-pipeline)
     * [Categorical encoding](#categorical-encoding)
+    * [Custom training configuration](#custom--training-configuration)
     * [Custom preprocessing](#custom-preprocessing)
     * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
@@ -119,20 +121,15 @@
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 ### Advanced usage
 
 #### Explanatory analysis
 
-BlueCast offers a simple way to get a first overview of the data. This is
-
-#### Enable cross-validation
-
-While the default behaviour of BlueCast is to use a simple
-train-test-split, cross-validation can be enabled easily:
+BlueCast offers a simple way to get a first overview of the data:
 
 ```sh
 from bluecast.eda.analyse import (
     bi_variate_plots,
     correlation_heatmap,
     correlation_to_target,
     univariate_plots,
@@ -165,25 +162,77 @@
 # show correlation to target
 correlation_to_target(train_data.loc[
             :, feat_type_detector.num_columns
         ],
         "EC1",)
 ```
 
+#### Enable cross-validation
+
+While the default behaviour of BlueCast is to use a simple
+train-test-split, cross-validation can be enabled easily:
+
+```sh
+from bluecast.blueprints.cast import BlueCast
+from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
+
+
+# Create a custom training config and adjust general training parameters
+train_config = TrainingConfig()
+train_config.hypertuning_cv_folds = 5 # default is 1
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCast(
+        class_problem="binary",
+        target_column="target"
+        conf_training=train_config,
+    )
+
+automl.fit(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
+#### Use multi-model blended pipeline
+
+By default, BlueCast trains a single model. However, it is possible to
+train multiple models with one call for extra robustness. `BlueCastCV`
+has a `fit` and a `fit_eval` method. The `fit_eval` method trains the
+models, but also provides out-of-fold validation. Also `BlueCastCV`
+allows to pass custom configurations.
+
+```sh
+from bluecast.blueprints.cast import BlueCastCV
+from bluecast.config.training_config import TrainingConfig, XgboostTuneParamsConfig
+
+# Pass the custom configs to the BlueCast class
+automl = BlueCastCV(
+        class_problem="binary",
+        #conf_training=train_config,
+        #conf_xgboost=xgboost_param_config,
+        #custom_preprocessor=custom_preprocessor, # this takes place right after test_train_split
+        #custom_last_mile_computation=custom_last_mile_computation, # last step before model training/prediction
+        #custom_feature_selector=custom_feature_selector,
+    )
+
+# this class has a train method:
+# automl.fit(df_train, target_col="target")
+
+automl.fit_eval(df_train, target_col="target")
+y_probs, y_classes = automl.predict(df_val)
+```
+
 #### Categorical encoding
 
 By default, BlueCast uses target encoding.
 This behaviour can be changed in the TrainingConfig by setting `cat_encoding_via_ml_algorithm`
 to True. This will change the expectations of `custom_last_mile_computation` though.
 If `cat_encoding_via_ml_algorithm` is set to False, `custom_last_mile_computation`
 will receive numerical features only as target encoding will apply before. If `cat_encoding_via_ml_algorithm`
 is True (default setting) `custom_last_mile_computation` will receive categorical
-features as well, because Xgboost#s inbuilt categorical encoding will be used.
-
-```sh
+features as well, because Xgboost's inbuilt categorical encoding will be used.
 
 #### Custom  training configuration
 
 Despite e2eml, BlueCast allows easy customization. Users can adjust the
 configuration and just pass it to the `BlueCast` class. Here is an example:
 
 ```sh
```

