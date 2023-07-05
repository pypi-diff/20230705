# Comparing `tmp/dataiku-scoring-11.4.4.tar.gz` & `tmp/dataiku-scoring-12.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataiku-scoring-11.4.4.tar", last modified: Tue Jul  4 10:44:01 2023, max compression
+gzip compressed data, was "dist/dataiku-scoring-12.0.1.tar", last modified: Wed Jul  5 08:18:34 2023, max compression
```

## Comparing `dataiku-scoring-11.4.4.tar` & `dataiku-scoring-12.0.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1098 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/PKG-INFO
--rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/requirements.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)       65 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/MANIFEST.in
--rw-r--r--   0 kevinremy   (502) staff       (20)      214 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/README.md
--rw-r--r--   0 kevinremy   (502) staff       (20)       27 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/NOTICE.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)      876 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/setup.py
--rw-r--r--   0 kevinremy   (502) staff       (20)       38 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/setup.cfg
--rw-r--r--   0 kevinremy   (502) staff       (20)      169 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/HISTORY.txt
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1098 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/PKG-INFO
--rw-r--r--   0 kevinremy   (502) staff       (20)     2506 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/requires.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)       15 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/top_level.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)        1 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataiku_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 kevinremy   (502) staff       (20)      524 2023-04-06 10:00:29.000000 dataiku-scoring-11.4.4/LICENSE.txt
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/
--rw-r--r--   0 kevinremy   (502) staff       (20)     1103 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     4771 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/decision_tree_model.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1157 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/generic_mlp.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1597 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/logistic.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      672 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      903 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      848 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_classifier.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1581 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_classifier.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      576 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/common.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      429 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/linear_regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      258 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_regressor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      708 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_classifier.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/
--rw-r--r--   0 kevinremy   (502) staff       (20)     2357 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)    10732 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/classification.py
--rw-r--r--   0 kevinremy   (502) staff       (20)    11000 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/dss_flavor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      681 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     6912 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/mlflow/common.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1069 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/__init__.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/
--rw-r--r--   0 kevinremy   (502) staff       (20)      239 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/math_utils.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      242 2023-06-15 08:28:03.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     5406 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/prediction_result.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1413 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/tokenizer.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1380 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/scoring_data.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2323 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/utils/indexed_matrix.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/models/
--rw-r--r--   0 kevinremy   (502) staff       (20)      880 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/binary.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      205 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/regression.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2457 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/models/mlflow.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      334 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/multiclass.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      635 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     6240 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/models/partitioned.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     3964 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/model.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2409 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/models/common.py
-drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-04 10:44:01.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/
--rw-r--r--   0 kevinremy   (502) staff       (20)      928 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/rescale.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2080 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/derive_rescale.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      759 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/flag.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2471 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_tfidf.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      783 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectors_unfold.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1399 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/categorical_encode.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1423 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/normalize.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1047 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/cat_cat_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1290 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/derive.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1241 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/__init__.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1205 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/impute.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      996 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessor.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1023 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/num_num_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1131 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/dummify.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      711 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/binarize.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1679 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/selection.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      864 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/num_cat_interaction.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2098 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/datetime_cyclical.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1302 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessings.py
--rw-r--r--   0 kevinremy   (502) staff       (20)      995 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/drop_rows.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     5038 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/prepare_input.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     2863 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/calibration.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     1246 2023-04-07 20:10:33.000000 dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_word_count.py
--rw-r--r--   0 kevinremy   (502) staff       (20)     9455 2023-07-04 10:43:38.000000 dataiku-scoring-11.4.4/dataikuscoring/load.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1222 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/requirements.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       65 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/MANIFEST.in
+-rw-r--r--   0 kevinremy   (502) staff       (20)      214 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/README.md
+-rw-r--r--   0 kevinremy   (502) staff       (20)       27 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/NOTICE.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      876 2023-07-04 13:43:10.000000 dataiku-scoring-12.0.1/setup.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)       38 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/setup.cfg
+-rw-r--r--   0 kevinremy   (502) staff       (20)      245 2023-07-04 13:43:10.000000 dataiku-scoring-12.0.1/HISTORY.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1222 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2506 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        6 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/requires.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)       15 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/top_level.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)        1 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataiku_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinremy   (502) staff       (20)      524 2023-04-06 10:00:29.000000 dataiku-scoring-12.0.1/LICENSE.txt
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1103 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     4771 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/decision_tree_model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1157 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/generic_mlp.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1597 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/logistic.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      672 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      903 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      848 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1581 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_classifier.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      576 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      429 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/linear_regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      258 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_regressor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      708 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_classifier.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2469 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    10845 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/classification.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)    11000 2023-07-04 13:20:45.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/dss_flavor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      681 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     7867 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/mlflow/common.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1069 2023-07-04 13:20:45.000000 dataiku-scoring-12.0.1/dataikuscoring/__init__.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      239 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/math_utils.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      242 2023-06-15 08:28:03.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     6491 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/prediction_result.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1413 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/tokenizer.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1379 2023-07-05 08:11:52.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/scoring_data.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2323 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/utils/indexed_matrix.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/models/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      880 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/binary.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      205 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/regression.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2457 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/mlflow.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      334 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/multiclass.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      635 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     6240 2023-06-30 10:38:01.000000 dataiku-scoring-12.0.1/dataikuscoring/models/partitioned.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     3964 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/model.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2409 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/models/common.py
+drwxr-xr-x   0 kevinremy   (502) staff       (20)        0 2023-07-05 08:18:34.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/
+-rw-r--r--   0 kevinremy   (502) staff       (20)      928 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2080 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/derive_rescale.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      759 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/flag.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2471 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_tfidf.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      783 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectors_unfold.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1399 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/categorical_encode.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1423 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/normalize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1047 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/cat_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1290 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/derive.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1241 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/__init__.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1205 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/impute.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      996 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessor.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1023 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/num_num_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1131 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/dummify.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      711 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/binarize.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1679 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/selection.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      864 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/num_cat_interaction.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2098 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/datetime_cyclical.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1302 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessings.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)      995 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/drop_rows.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     5038 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/prepare_input.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     2863 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/calibration.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     1246 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_word_count.py
+-rw-r--r--   0 kevinremy   (502) staff       (20)     9455 2023-04-07 20:10:33.000000 dataiku-scoring-12.0.1/dataikuscoring/load.py
```

### Comparing `dataiku-scoring-11.4.4/PKG-INFO` & `dataiku-scoring-12.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 11.4.4
+Version: 12.0.1
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Description: # Dataiku ML Scoring Python library
         
@@ -12,14 +12,20 @@
         
         To use this library, you need to first export your model to Python from Dataiku.
         
         
         Changelog
         ==========
         
+        
+        12.0.1 (2023-07-04)
+        -------------------
+        
+        * Initial release for DSS 12.0.1
+        
         11.4.4 (2023-07-04)
         -------------------
         
         * Initial release for DSS 11.4.4
         
         11.1.0 (2022-10-20)
         -------------------
```

### Comparing `dataiku-scoring-11.4.4/setup.py` & `dataiku-scoring-12.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 long_description = (open('README.md').read() + '\n\n' +
                     open('HISTORY.txt').read())
 
-VERSION = "11.4.4"
+VERSION = "12.0.1"
 
 setuptools.setup(
     name='dataiku-scoring',
     version=VERSION,
     license="Apache Software License",
     packages=setuptools.find_packages(),
     description="Dataiku ML Scoring Python library",
```

### Comparing `dataiku-scoring-11.4.4/dataiku_scoring.egg-info/PKG-INFO` & `dataiku-scoring-12.0.1/dataiku_scoring.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dataiku-scoring
-Version: 11.4.4
+Version: 12.0.1
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Description: # Dataiku ML Scoring Python library
         
@@ -12,14 +12,20 @@
         
         To use this library, you need to first export your model to Python from Dataiku.
         
         
         Changelog
         ==========
         
+        
+        12.0.1 (2023-07-04)
+        -------------------
+        
+        * Initial release for DSS 12.0.1
+        
         11.4.4 (2023-07-04)
         -------------------
         
         * Initial release for DSS 11.4.4
         
         11.1.0 (2022-10-20)
         -------------------
```

### Comparing `dataiku-scoring-11.4.4/dataiku_scoring.egg-info/SOURCES.txt` & `dataiku-scoring-12.0.1/dataiku_scoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/LICENSE.txt` & `dataiku-scoring-12.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_regressor.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/decision_tree_model.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/generic_mlp.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/generic_mlp.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/logistic.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/logistic.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_regressor.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/__init__.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/mlp_classifier.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/gradient_boosting_classifier.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/gradient_boosting_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/common.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/algorithms/forest_classifier.py` & `dataiku-scoring-12.0.1/dataikuscoring/algorithms/forest_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/mlflow/regression.py` & `dataiku-scoring-12.0.1/dataikuscoring/mlflow/regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import logging
 import pandas as pd
 import numpy as np
 
-from dataikuscoring.mlflow.common import DisableMLflowTypeEnforcement
+from dataikuscoring.mlflow.common import DisableMLflowTypeEnforcement, convert_date_features
 from dataikuscoring.utils.scoring_data import ScoringData
 from dataikuscoring.utils.prediction_result import PredictionResult
 
 logger = logging.getLogger(__name__)
 
 
 def mlflow_regression_predict_to_scoring_data(mlflow_model, imported_model_meta, input_df):
     """
     Returns a ScoringData containing predictions for a MLflow model.
     Performs "interpretation" of the MLflow output.
 
     Requires a prediction type on the MLflow model
     """
+    input_df = input_df.copy()
+    convert_date_features(imported_model_meta, input_df)
 
     logging.info("Predicting it")
 
     with DisableMLflowTypeEnforcement():
         output = mlflow_model.predict(input_df)
 
     if isinstance(output, pd.DataFrame):
@@ -49,15 +51,15 @@
 
     preds = mlflow_raw_preds
     pred_df = pd.DataFrame({"prediction": preds})
 
     if np.isnan(pred_df.to_numpy()).any():
         raise Exception("MLflow model predicted NaN probabilities")
 
-    logger.info("Final pred_df: %s " % pred_df)
+    logger.debug("Final pred_df: %s " % pred_df)
 
     # Fix indexing to match the input_df
     pred_df.index = input_df.index
     if isinstance(preds, pd.Series):
         preds.index = input_df.index
 
     prediction_result = PredictionResult(preds)
```

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/mlflow/classification.py` & `dataiku-scoring-12.0.1/dataikuscoring/mlflow/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import pandas as pd
 import numpy as np
 
-from dataikuscoring.mlflow.common import DisableMLflowTypeEnforcement
+from dataikuscoring.mlflow.common import DisableMLflowTypeEnforcement, convert_date_features
 from dataikuscoring.utils.scoring_data import ScoringData
 from dataikuscoring.utils.prediction_result import ClassificationPredictionResult
 
 logger = logging.getLogger(__name__)
 
 
 def mlflow_try_to_get_probas(input_df, mlflow_model, labels_map):
@@ -63,14 +63,16 @@
         logger.info("MLflow model is %s" % mlflow_model)
         logger.info("MLflow model is class %s" % type(mlflow_model._model_impl))
 
     return probas, probas_raw
 
 
 def mlflow_classification_predict_to_scoring_data(mlflow_model, imported_model_meta, input_df, threshold=None):
+    input_df = input_df.copy()
+    convert_date_features(imported_model_meta, input_df)
     """
     Returns a ScoringData containing predictions and probas for a MLflow model.
     Performs "interpretation" of the MLflow output.
 
     Requires a prediction type on the MLflow model
     """
 
@@ -190,25 +192,25 @@
     if imported_model_meta["predictionType"] == "BINARY_CLASSIFICATION":
         if probas is not None and threshold is not None:
             logger.info("Overriding prediction using probabilities and threshold={}".format(threshold))
 
             probas_one = probas["proba_%s" % int_to_label_map[1]]
             preds = (probas_one > threshold).astype(np.int)
             pred_df = pd.DataFrame({"prediction": preds})
-            logger.info("Computed pred df %s" % pred_df)
+            logger.debug("Computed pred df %s" % pred_df)
             pred_df["prediction"].replace(int_to_label_map, inplace=True)
             logger.info("Computed cleanpred df %s" % pred_df["prediction"].dtype)
 
     if np.isnan(preds).any():
         raise Exception("MLflow model predicted NaN values")
 
     if probas is not None and np.isnan(probas.to_numpy()).any():
         raise Exception("MLflow model predicted NaN probabilities")
 
-    logger.info("Final pred_df: %s " % pred_df)
+    logger.debug("Final pred_df: %s " % pred_df)
     logger.info("lTIM = %s " % (imported_model_meta["labelToIntMap"]))
 
     # Fix indexing to match the input_df
     preds.index = input_df.index
     pred_df.index = input_df.index
     if probas is not None:
         probas.index = input_df.index
```

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/mlflow/dss_flavor.py` & `dataiku-scoring-12.0.1/dataikuscoring/mlflow/dss_flavor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/mlflow/__init__.py` & `dataiku-scoring-12.0.1/dataikuscoring/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/mlflow/common.py` & `dataiku-scoring-12.0.1/dataikuscoring/mlflow/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 import json
+from datetime import datetime
+
 import pandas as pd
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 class DisableMLflowTypeEnforcement(object):
     def __enter__(self):
@@ -139,7 +141,28 @@
                 tensors_list = [tensor.tolist() for tensor in list(output)]
             return pd.DataFrame({"prediction": tensors_list})
         else:
             raise Exception("Can't handle MLflow model output of shape=%s" % (shape,))
 
     else:
         raise Exception("Can't handle MLflow model output: %s" % type(output))
+
+
+def convert_date_features(imported_model_meta, input_df):
+    """
+    Converts features declared in imported_model_meta as 'date' feature types to 'real' datetime64 in input_df.
+    Don't touch columns that are not declared as 'date' feature types.
+    """
+    for feature in imported_model_meta['features']:
+        if feature['type'] == 'date':
+            if pd.api.types.is_numeric_dtype(input_df[feature['name']].dtype):
+                input_df[feature['name']] = epoch_to_datetime(input_df[feature['name']], input_df[feature['name']])
+            else:
+                input_df[feature['name']] = pd.to_datetime(input_df[feature['name']])
+
+
+def epoch_to_datetime(series, orig_series):
+    if hasattr(orig_series.dtype, 'tz'):
+        epoch = datetime(1900, 1, 1, tzinfo=orig_series.dtype.tz) # expect that it's UTC
+    else:
+        epoch = datetime(1900, 1, 1)
+    return (series * np.timedelta64(1, 's')) + epoch
```

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/__init__.py` & `dataiku-scoring-12.0.1/dataikuscoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/utils/prediction_result.py` & `dataiku-scoring-12.0.1/dataikuscoring/utils/prediction_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import numpy as np
 import pandas as pd
 import six
 from abc import abstractmethod
 from abc import ABCMeta
 
 
+PREDICTION = "prediction"
+PROBABILITIES = "probabilities"
+
+
 @six.add_metaclass(ABCMeta)
 class AbstractPredictionResult(object):
 
     @property
     @abstractmethod
     def preds(self):
         """
@@ -31,14 +35,27 @@
 
     @abstractmethod
     def is_empty(self):
         """
         :rtype: bool
         """
 
+    @abstractmethod
+    def as_dataframe(self):
+        """
+        Builds & returns a DataFrame representation of the result:
+        WARNING:
+          * This dataframe has no notion of index because it is built out of numpy arrays so will have
+            a pristine range index and MUST be indexed afterwards
+          * For classification, proba columns are returned as a tuple ("probabilities", "class_name"), which differs
+            from the usual "proba_className"
+        :return: the prediction result as a DataFrame
+        :rtype: pd.DataFrame
+        """
+
     @staticmethod
     def concat(prediction_results):
         """
         :type prediction_results: list[AbstractPredictionResult]
         :rtype: AbstractPredictionResult
         """
         if len(prediction_results) == 0:
@@ -49,14 +66,17 @@
             raise ValueError("All prediction result should be of same class")
 
         return prediction_result_class._concat(prediction_results)
 
 
 class PredictionResult(AbstractPredictionResult):
 
+    def as_dataframe(self):
+        return pd.DataFrame({PREDICTION: self.preds})
+
     def __init__(self, preds):
         """
         :type preds: np.ndarray
         """
         self._preds = preds
 
     @property
@@ -126,14 +146,23 @@
 
     def is_empty(self):
         if self._preds is not None:
             return self._preds.shape[0] == 0
         else:
             return self._unmapped_preds.shape[0] == 0
 
+    def as_dataframe(self):
+        preds_df = pd.DataFrame(({PREDICTION: self.preds}))
+        if not self.has_probas():
+            return preds_df
+        else:
+            columns = [(PROBABILITIES, clazz) for clazz in self._classes]
+            probas_df = pd.DataFrame(data=self.probas, columns=columns)
+            return pd.concat([preds_df, probas_df], axis=1)
+
     @staticmethod
     def _concat_items(items_list):
         """
         :type items_list: list[np.ndarray|None]
         :rtype: np.ndarray or None
         """
         if items_list[0] is None:
```

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/utils/tokenizer.py` & `dataiku-scoring-12.0.1/dataikuscoring/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/utils/scoring_data.py` & `dataiku-scoring-12.0.1/dataikuscoring/utils/scoring_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class ScoringData(object):
     def __init__(self, is_empty=False, prediction_result=None, valid_y=None, valid_sample_weights=None, preds_df=None,
                  probas_df=None, decisions_and_cuts=None, reason=None, valid_unprocessed=None):
         """
         :type is_empty: bool
-        :type prediction_result: dataikuscoring.mlflow.prediction_result.AbstractPredictionResult or None
+        :type prediction_result: dataikuscoring.utils.prediction_result.AbstractPredictionResult or None
         :type valid_y: pd.Series or None
         :type valid_sample_weights: pd.Series or None
         :type preds_df: pd.DataFrame or None
         :type probas_df: pd.DataFrame or None
         :type decisions_and_cuts: DecisionsAndCuts or None
         :type reason: str
         :type valid_unprocessed: pandas.DataFrame
```

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/utils/indexed_matrix.py` & `dataiku-scoring-12.0.1/dataikuscoring/utils/indexed_matrix.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/binary.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/binary.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/mlflow.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/mlflow.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/__init__.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/partitioned.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/partitioned.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/model.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/models/common.py` & `dataiku-scoring-12.0.1/dataikuscoring/models/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/rescale.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/derive_rescale.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/derive_rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/flag.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/flag.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_tfidf.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_tfidf.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/vectors_unfold.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/vectors_unfold.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/categorical_encode.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/categorical_encode.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/normalize.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/normalize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/cat_cat_interaction.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/cat_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/derive.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/derive.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/__init__.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/impute.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/impute.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessor.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/num_num_interaction.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/num_num_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/dummify.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/dummify.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/binarize.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/binarize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/selection.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/selection.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/num_cat_interaction.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/num_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/datetime_cyclical.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/datetime_cyclical.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/preprocessings.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/preprocessings.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/drop_rows.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/drop_rows.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/prepare_input.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/prepare_input.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/calibration.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/calibration.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/processors/vectorize_word_count.py` & `dataiku-scoring-12.0.1/dataikuscoring/processors/vectorize_word_count.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-11.4.4/dataikuscoring/load.py` & `dataiku-scoring-12.0.1/dataikuscoring/load.py`

 * *Files identical despite different names*

