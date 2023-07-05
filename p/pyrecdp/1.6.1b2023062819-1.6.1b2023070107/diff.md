# Comparing `tmp/pyrecdp-1.6.1b2023062819.tar.gz` & `tmp/pyrecdp-1.6.1b2023070107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.6.1b2023062819.tar", last modified: Wed Jun 28 19:00:32 2023, max compression
+gzip compressed data, was "pyrecdp-1.6.1b2023070107.tar", last modified: Fri Jun 30 23:18:30 2023, max compression
```

## Comparing `pyrecdp-1.6.1b2023062819.tar` & `pyrecdp-1.6.1b2023070107.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023062819/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-28 16:32:55.000000 pyrecdp-1.6.1b2023062819/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.796166 pyrecdp-1.6.1b2023062819/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023062819/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.796166 pyrecdp-1.6.1b2023062819/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4030 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13943 2023-06-28 16:32:55.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4523 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3106 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     3008 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     6782 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-27 20:36:34.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4141 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-06-26 20:30:14.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-06-28 16:32:55.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-26 21:12:36.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-26 21:12:48.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-06-27 20:36:34.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4398 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.800166 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54072 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8699 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.796166 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-28 19:00:32.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3614 2023-06-28 19:00:32.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 19:00:32.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:27:26.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-28 19:00:32.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 19:00:32.000000 pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-28 16:32:55.000000 pyrecdp-1.6.1b2023062819/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 19:00:32.804166 pyrecdp-1.6.1b2023062819/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 16:32:55.000000 pyrecdp-1.6.1b2023062819/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-27 20:35:25.000000 pyrecdp-1.6.1b2023062819/tests/test_autofe.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-06-27 20:35:25.000000 pyrecdp-1.6.1b2023062819/tests/test_feature_estimator.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-27 22:22:59.000000 pyrecdp-1.6.1b2023062819/tests/test_feature_profiler.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-27 20:35:25.000000 pyrecdp-1.6.1b2023062819/tests/test_feature_wrangler.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-27 20:35:25.000000 pyrecdp-1.6.1b2023062819/tests/test_pipeline_json.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-06-26 18:39:00.000000 pyrecdp-1.6.1b2023062819/tests/test_relational_builder.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-02 20:28:07.000000 pyrecdp-1.6.1b2023062819/tests/test_spark_dataprocessor.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-28 19:00:17.000000 pyrecdp-1.6.1b2023062819/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023070107/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-02 20:11:31.000000 pyrecdp-1.6.1b2023070107/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-30 21:06:39.000000 pyrecdp-1.6.1b2023070107/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    13999 2023-06-30 00:30:49.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4523 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-06-29 21:19:32.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-30 00:37:42.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-06-30 17:24:14.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/parallel_iterator.py
+-rw-r--r--   0 root         (0) root         (0)     5939 2023-06-29 22:50:40.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-06-30 18:42:09.000000 pyrecdp-1.6.1b2023070107/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-29 22:31:54.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-06-30 15:52:33.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-30 02:14:52.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-29 22:51:31.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-06-29 20:57:59.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-06-30 20:29:52.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-30 17:44:38.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-06-30 19:21:59.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     4742 2023-06-29 22:28:23.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54072 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8699 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.688970 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 20:27:26.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-30 23:18:30.000000 pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 23:18:30.692970 pyrecdp-1.6.1b2023070107/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_autofe.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-29 20:28:26.000000 pyrecdp-1.6.1b2023070107/tests/test_spark_dataprocessor.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-30 23:18:24.000000 pyrecdp-1.6.1b2023070107/version
```

### Comparing `pyrecdp-1.6.1b2023062819/LICENSE` & `pyrecdp-1.6.1b2023070107/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/PKG-INFO` & `pyrecdp-1.6.1b2023070107/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023062819
+Version: 1.6.1b2023070107
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrecdp-1.6.1b2023062819/README.md` & `pyrecdp-1.6.1b2023070107/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.6.1b2023070107/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/__init__.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/BasePipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,34 +53,40 @@
         # Set properties for BasePipeline
         if not input_is_path:
             original_data = self.dataset[main_table]
         else:
             original_data = sample_read(self.dataset[main_table])
         
         self.feature_columns = [i for i in original_data.columns if i != self.y]
-        feature_data = original_data[self.feature_columns]
+        #feature_data = original_data[self.feature_columns]
             
         self.generators = []
         self.pipeline = DiGraph()
         if not input_is_path:
             op = 'DataFrame'
             config = main_table
         else:
             op = 'DataLoader'
             config = {'table_name': main_table, 'file_path': self.dataset[main_table]}
         
         cur_id = 0
         self.pipeline[cur_id] = Operation(
-            cur_id, None, output = DataFrameSchema(feature_data), op = op, config = config)
+            cur_id, None, output = DataFrameSchema(original_data), op = op, config = config)
 
         if len(self.dataset) > 1:
             self.supplementary = dict((k, v) for k, v in self.dataset.items() if k != main_table)
         else:
             self.supplementary = None
         self.rdp = None
+
+    def update_label(self):
+        leaf_idx = self.pipeline.convert_to_node_chain()[-1]
+        pa_schema = self.pipeline[leaf_idx].output
+        label_list = [pa_field.name for pa_field in pa_schema if pa_field.is_label]
+        self.y = label_list[0]
      
     def fit_analyze(self, *args, **kwargs):
         child = list(self.pipeline.keys())[-1]
         max_id = child
         to_run = []
         for i in range(len(self.generators)):
             for generator in self.generators[i]:
@@ -263,16 +269,14 @@
                     if isinstance(op, DataFrameOperation):
                         if data:
                             input_df = data
                         else:
                             input_df = self.dataset if start_op_idx == -1 else {'main_table': self.transformed_cache}
                         input_df = deepcopy(input_df) if no_cache else input_df
                         op.set(input_df)
-                    if isinstance(op, TargetEncodeOperation):
-                        op.set(self.y)
                     with Timer(f"execute {op}"):
                         op.execute_pd(executable_pipeline)
             if transformed_end == -1:
                 df = executable_sequence[-1].cache
             else:
                 df = executable_pipeline[transformed_end].cache
         elif engine_type == 'spark':
@@ -286,16 +290,14 @@
                     if isinstance(op, DataFrameOperation):
                         if data:
                             input_df = data
                         else:
                             input_df = self.dataset if start_op_idx == -1 else {'main_table': self.transformed_cache}
                         input_df = deepcopy(input_df) if no_cache else input_df
                         op.set(input_df)
-                    if isinstance(op, TargetEncodeOperation):
-                        op.set(self.y)
                     print(f"append {op}")
                     op.execute_spark(executable_pipeline, self.rdp)
                 if transformed_end == -1:
                     ret = executable_sequence[-1].cache
                 else:
                     ret = executable_pipeline[transformed_end].cache
                 if isinstance(ret, SparkDataFrame):
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureProfiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         X = DataFrameAPI().instiate(self.dataset[self.main_table])
         sampled_data = X.may_sample()
 
         self.pipeline[child].output.append(SeriesSchema(sampled_data[self.y]))
         
         # firstly, call data profiler to analyze data
         for generator in self.data_profiler:
-            self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, sampled_data)
+            self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, sampled_data, self.y)
             
         child, max_id = super().fit_analyze(*args, **kwargs)
     
     def visualize_analyze(self, engine_type = 'pandas', display = True):
         feature_data = self.fit_transform(engine_type)
         self.data_stats = StatisticsFeatureGenerator().update_feature_statistics(feature_data, self.dataset[self.main_table][self.y])
         if not self.data_stats:
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/FeatureWrangler.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 logging.basicConfig(format='%(asctime)s %(levelname)s:%(message)s', level=logging.ERROR, datefmt='%I:%M:%S')
 logger = logging.getLogger(__name__)
 
 class FeatureWrangler(BasePipeline):
     def __init__(self, dataset, label, *args, **kwargs):
         super().__init__(dataset, label)
         self.data_profiler = [cls() for cls in feature_infer_list]
-        self.pre_feature = [cls() for cls in label_feature_generator_list]
         # If we provided multiple datasets in this workload
         self.generators.append([cls() for cls in pre_feature_generator_list])
         self.generators.append([cls() for cls in transformation_generator_list])
         self.generators.append([cls() for cls in pre_enocode_feature_generator_list])
         self.generators.append([cls() for cls in local_encode_generator_list])
         self.generators.append([cls() for cls in global_dict_index_generator_list])
         self.generators.append([cls() for cls in post_feature_generator_list])
@@ -29,33 +28,13 @@
     def fit_analyze(self, *args, **kwargs): 
         child = list(self.pipeline.keys())[-1]
         max_id = child
         # sample data
         X = DataFrameAPI().instiate(self.dataset[self.main_table])
         sampled_data = X.may_sample()
         
-        if self.y is not None:
-            # insert label process to pipeline            
-            cur_id = child
-            original_first_op = copy.deepcopy(self.pipeline[cur_id])
-            self.pipeline[cur_id].output = [SeriesSchema(sampled_data[self.y])]
-            
-            for generator in self.data_profiler:
-                self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, pd.DataFrame(sampled_data[self.y]))
-            for generator in self.pre_feature:
-                self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id)
-            
-            cur_id = max_id + 1
-            original_first_op.idx = cur_id
-            original_first_op.op = "DataFrame"
-            original_first_op.children = [child]
-            self.y = [i.name for i in self.pipeline[child].output][0]
-            self.pipeline[cur_id] = original_first_op            
-            max_id = cur_id
-            child = cur_id
-            sampled_data = sampled_data[self.feature_columns]
-        
-        # firstly, call data profiler to analyze data
         for generator in self.data_profiler:
-            self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, sampled_data)
+            self.pipeline, child, max_id = generator.fit_prepare(self.pipeline, [child], max_id, sampled_data, self.y)
         print("Feature List generated, using analyzed feature tags to create data pipeline")
-        return super().fit_analyze(*args, **kwargs)
+        ret = super().fit_analyze(*args, **kwargs)
+        self.update_label()
+        return ret
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/core/dataframe.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/core/di_graph.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/core/schema.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/core/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,23 @@
 
     def __repr__(self):
         return f"{self.mydump()}"
    
     @property
     def dtype_str(self):
         return str(dict((k, v) for k, v in self.config.items() if v))
-         
+
+    @property
+    def is_label(self):
+        return 'is_label' in self.config and self.config['is_label']
+
+    @property
+    def is_categorical_label(self):
+        return 'is_categorical_label' in self.config and self.config['is_categorical_label']
+
     @property
     def is_boolean(self):
         return 'is_boolean' in self.config and self.config['is_boolean']
 
     @property
     def is_string(self):
         return 'is_string' in self.config and self.config['is_string']
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/core/utils.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,14 +190,22 @@
     try:
         proc_(sample_data)
     except Exception as e:
         #print(e)
         return False
     return True
  
+def is_unique(s):
+    if isinstance(s, pd.Series):
+        return len(s.unique()) == 1
+    elif isinstance(s, pd.DataFrame) and len(s.columns) == 1:
+        return len(s[s.columns[0]].unque()) == 1
+    else:
+        return False
+
 class Timer:
     level = 0
     viewer = None
 
     def __init__(self, name):
         self.name = name
         if Timer.viewer:
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/base_api.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .drop import DropUselessFeatureGenerator
 from .name import RenameFeatureGenerator
 from .fillna import FillNaFeatureGenerator
 from .type import TypeCheckFeatureGenerator,TypeConvertFeatureGenerator
 from .nlp import DecodedTextFeatureGenerator, TextFeatureGenerator
 from .geograph import GeoFeatureGenerator, CoordinatesInferFeatureGenerator
 from .relation import RelationalFeatureGenerator
-from .encode import OneHotFeatureGenerator, ListOneHotFeatureGenerator, TargetEncodeFeatureGenerator, LabelEncodeFeatureGenerator
+from .encode import OneHotFeatureGenerator, ListOneHotFeatureGenerator, TargetEncodeFeatureGenerator, LabelEncodeFeatureGenerator, CountEncodeFeatureGenerator
 from .feature_transform import ConvertToNumberFeatureGenerator
 
 relation_builder_list = [
     RelationalFeatureGenerator
 ]
 
 profiler_feature_generator_list = [
@@ -44,21 +44,23 @@
 
 local_encode_generator_list = [
     OneHotFeatureGenerator,
     ListOneHotFeatureGenerator,
 ]
 
 pre_enocode_feature_generator_list = [
-    DropUselessFeatureGenerator,
+    #DropUselessFeatureGenerator,
 ]
 
 global_dict_index_generator_list = [
+    LabelEncodeFeatureGenerator,
     BinnedFeatureGenerator,
     CategoryFeatureGenerator,
-    TargetEncodeFeatureGenerator
+    TargetEncodeFeatureGenerator,
+    CountEncodeFeatureGenerator
 ]
 
 post_feature_generator_list = [
     RenameFeatureGenerator
 ]
 
 final_generator_list = [
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/category.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         folder = 'pipeline_default'
         ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
             if pa_field.is_categorical_and_string:
                 feature = pa_field.name
-                out_schema = SeriesSchema(f"{feature}__idx", pd.CategoricalDtype())
+                out_schema = SeriesSchema(f"{feature}__idx", int)
                 feature_in_out[feature] = (f"{folder}/{feature}_categorify_dict", out_schema.name)
                 is_useful = True
                 ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
             config = feature_in_out
             pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'categorify', config = config)
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/encode.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         folder = 'pipeline_default'
         for idx, pa_field in enumerate(pa_schema):
-            if pa_field.is_string:
+            if pa_field.is_string and pa_field.is_label:
                 feature = pa_field.name
-                out_schema = SeriesSchema(f"{feature}", pd.CategoricalDtype())
+                config = {}
+                config = pa_field.copy_config_to(config)
+                config['is_string'] = False
+                out_schema = SeriesSchema(f"{feature}", int)
+                out_schema.copy_config_from(config)
                 feature_in_out[feature] = (f"{folder}/{feature}_categorify_dict", feature)
                 is_useful = True
                 pa_schema[idx] = out_schema
         if is_useful:
             cur_idx = max_idx + 1
             config = feature_in_out
             pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'categorify', config = config)
@@ -81,20 +85,49 @@
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
         feature_in_out = {}
         ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
-            if pa_field.is_categorical_and_string:
+            if pa_field.is_categorical:
                 feature = pa_field.name
-                out_schema = SeriesSchema(f"{feature}__TE", pd.CategoricalDtype())
+                out_schema = SeriesSchema(f"{feature}__TE", float)
                 feature_in_out[feature] = out_schema.name
                 is_useful = True
                 ret_pa_schema.append(out_schema)
         if is_useful:
+            # find label column
+            label_list = [pa_field.name for pa_field in pa_schema if pa_field.is_label]
             cur_idx = max_idx + 1
-            config = feature_in_out
+            config = {}
+            config['feature_in_out'] = feature_in_out
+            config['label'] = label_list[0]
             pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'target_encode', config = config)
             return pipeline, cur_idx, cur_idx
         else:
+            return pipeline, children[0], max_idx
+
+class CountEncodeFeatureGenerator(super_class):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.feature_in = []
+
+    def fit_prepare(self, pipeline, children, max_idx):
+        is_useful = False
+        pa_schema = pipeline[children[0]].output
+        feature_in_out = {}
+        ret_pa_schema = copy.deepcopy(pa_schema)
+        for pa_field in pa_schema:
+            if pa_field.is_categorical:
+                feature = pa_field.name
+                out_schema = SeriesSchema(f"{feature}__CE", int)
+                feature_in_out[feature] = out_schema.name
+                is_useful = True
+                ret_pa_schema.append(out_schema)
+        if is_useful:
+            cur_idx = max_idx + 1
+            config = feature_in_out
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'count_encode', config = config)
+            return pipeline, cur_idx, cur_idx
+        else:
             return pipeline, children[0], max_idx
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         from .drop import DropOperation
         from .fillna import FillNaOperation
         from .featuretools_adaptor import FeaturetoolsOperation
         from .geograph import HaversineOperation
         from .type import TypeInferOperation
         from .tuple import TupleOperation
         from .custom import CustomOperation
-        from .encode import OnehotEncodeOperation, ListOnehotEncodeOperation, TargetEncodeOperation
+        from .encode import OnehotEncodeOperation, ListOnehotEncodeOperation, TargetEncodeOperation, CountEncodeOperation
         from pyrecdp.primitives.estimators.lightgbm import LightGBM
 
         operations_ = {
             'DataFrame': DataFrameOperation,
             'DataLoader': DataLoader,
             'merge': MergeOperation,
             'rename': RenameOperation,
@@ -53,14 +53,15 @@
             'haversine': HaversineOperation,
             'tuple': TupleOperation,
             'type_infer': TypeInferOperation,
             'lightgbm': LightGBM,
             'onehot_encode': OnehotEncodeOperation,
             'list_onehot_encode': ListOnehotEncodeOperation,
             'target_encode': TargetEncodeOperation,
+            'count_encode': CountEncodeOperation,
             'custom_operator': CustomOperation
         }
 
         if self.op in operations_:
             return operations_[self.op](self)
         else:
             try:
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/category.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from .base import BaseOperation
 import pandas as pd
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyrecdp.core.utils import *
 import copy
+from sklearn.preprocessing import LabelEncoder
+from pyrecdp.core.parallel_iterator import ParallelIterator
+from IPython.display import display
 
 class CategorifyOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self.feature_in_out = self.op.config
         self.support_spark_dataframe = False
         self.support_spark_rdd = False
-    
+
+    @classmethod
+    def label_encode(cls, item):
+        feature, df_x, dict_path, feature_out = item
+        encoder = LabelEncoder()
+        ret = pd.DataFrame()
+        ret[feature_out] = encoder.fit_transform(df_x)
+        ret.index = df_x.index
+        return ret
+
     def get_function_pd(self):
         feature_in_out = copy.deepcopy(self.feature_in_out)
         def categorify(df):
-            from sklearn.preprocessing import LabelEncoder
-            for feature, (dict_path, feature_out) in feature_in_out.items():
-                encoder = LabelEncoder()
-                encoder = get_encoder_np(encoder, dict_path)
-                encoder.fit(df[feature])
-                save_encoder_np(encoder, dict_path)
-                df[f"{feature_out}"] = pd.Series(encoder.transform(df[feature]))
-                
+            df_features = [(col, df[col], dict_path, feature_out) for col, (dict_path, feature_out) in feature_in_out.items()]
+            results = ParallelIterator.execute(df_features, CategorifyOperation.label_encode, len(df_features), "Categorify")
+            df = df.loc[:, ~df.columns.isin([sdf.columns[0] for sdf in results])]
+            df = pd.concat([df] + results, axis=1)
             return df
+
         return categorify
 
 class GroupedCategorifyOperation(BaseOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
         self.feature_in_out = self.op.config
         self.support_spark_dataframe = False
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/geograph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from .base import BaseOperation
-import pandas as pd
-from pyspark.sql import DataFrame as SparkDataFrame
-from pyspark import RDD
+from .featuretools_adaptor import FeaturetoolsOperation
 import copy
- 
-class DropOperation(BaseOperation):
+from pyrecdp.core.utils import class_name_fix
+
+class HaversineOperation(FeaturetoolsOperation):
     def __init__(self, op_base):
         super().__init__(op_base)
-        self.feature_in = self.op.config
-        self.support_spark_dataframe = True
-        self.support_spark_rdd = True
-        self.fast_without_dpp = True
 
     def get_function_pd(self):
-        feature_in = copy.deepcopy(self.feature_in)
-        def drop_useless_feature(df):
-            return df.drop(columns = feature_in)
-        return drop_useless_feature
-    
-    def get_function_spark(self, rdp):
-        def drop_feature(df):
-            return df.drop(*self.feature_in)
-        return drop_feature
+        feature_in_out_map = copy.deepcopy(self.feature_in_out_map)
+        def generate_ft_feature(df):
+            for inputs_str, op in feature_in_out_map.items():
+                inputs = eval(inputs_str)
+                op_object = class_name_fix(op[1])()
+                df[op[0]] = op_object(df[inputs[0]], df[inputs[1]])
+            return df
+        return generate_ft_feature
+
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,32 +99,39 @@
     
     return False
          
 class TypeInferFeatureGenerator():
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
    
-    def fit_prepare(self, pipeline, children, max_idx, df):
+    def fit_prepare(self, pipeline, children, max_idx, df, y = None):
         ret_pa_fields = []
         pa_schema = pipeline[children[0]].output
         for pa_field, feature_name in tqdm(zip(pa_schema, df.columns), total=len(df.columns)):
             config = {}
-            if try_datetime(df[feature_name]):
-                config['is_datetime'] = True
-            if try_category(df[feature_name]):
-                config['is_categorical'] = True
-            if try_numeric(df[feature_name]):
-                config['is_numeric'] = True
-            elif try_re_numeric(df[feature_name]):
-                config['is_re_numeric'] = True
-            config['is_list_string'] = try_list_string(df[feature_name])
-            if config['is_list_string'] is False:
-                skip = ('is_numeric' in config and config['is_numeric']) or ('is_re_numeric' in config and config['is_re_numeric'])
-                if not skip:
-                    config['is_onehot'] = try_onehot(df[feature_name])
+            # Add y_label to y column
+            if feature_name == y:
+                config['is_label'] = True
+                if pa_field.is_string:
+                    config['is_categorical_label'] = True
+            else:
+                if try_datetime(df[feature_name]):
+                    config['is_datetime'] = True
+                if try_category(df[feature_name]):
+                    config['is_categorical'] = True
+                if try_numeric(df[feature_name]):
+                    config['is_numeric'] = True
+                elif try_re_numeric(df[feature_name]):
+                    config['is_re_numeric'] = True
+                    config['is_categorical'] = False
+                config['is_list_string'] = try_list_string(df[feature_name])
+                if config['is_list_string'] is False:
+                    skip = ('is_numeric' in config and config['is_numeric']) or ('is_re_numeric' in config and config['is_re_numeric'])
+                    if not skip:
+                        config['is_onehot'] = try_onehot(df[feature_name])
             
             pa_field.copy_config_from(config)
             ret_pa_fields.append(pa_field)
         
         # append to pipeline
         cur_idx = max_idx + 1
         config = [x.mydump() for x in ret_pa_fields]
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.6.1b2023070107/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023062819
+Version: 1.6.1b2023070107
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrecdp-1.6.1b2023062819/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.6.1b2023070107/pyrecdp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pyrecdp/autofe/FeatureProfiler.py
 pyrecdp/autofe/FeatureWrangler.py
 pyrecdp/autofe/RelationalBuilder.py
 pyrecdp/autofe/__init__.py
 pyrecdp/core/__init__.py
 pyrecdp/core/dataframe.py
 pyrecdp/core/di_graph.py
+pyrecdp/core/parallel_iterator.py
 pyrecdp/core/schema.py
 pyrecdp/core/utils.py
 pyrecdp/datasets/CESM_breast_cancer.py
 pyrecdp/datasets/__init__.py
 pyrecdp/datasets/amazon_product_review.py
 pyrecdp/datasets/base_api.py
 pyrecdp/datasets/download.py
```

### Comparing `pyrecdp-1.6.1b2023062819/setup.py` & `pyrecdp-1.6.1b2023070107/setup.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_autofe.py` & `pyrecdp-1.6.1b2023070107/tests/test_autofe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_feature_estimator.py` & `pyrecdp-1.6.1b2023070107/tests/test_feature_estimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_feature_profiler.py` & `pyrecdp-1.6.1b2023070107/tests/test_feature_profiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_feature_wrangler.py` & `pyrecdp-1.6.1b2023070107/tests/test_feature_wrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_pipeline_json.py` & `pyrecdp-1.6.1b2023070107/tests/test_pipeline_json.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_relational_builder.py` & `pyrecdp-1.6.1b2023070107/tests/test_relational_builder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023062819/tests/test_spark_dataprocessor.py` & `pyrecdp-1.6.1b2023070107/tests/test_spark_dataprocessor.py`

 * *Files identical despite different names*

