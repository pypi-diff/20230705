# Comparing `tmp/nzpyida-0.3.6.tar.gz` & `tmp/nzpyida-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.3.6.tar", last modified: Mon May 29 14:25:47 2023, max compression
+gzip compressed data, was "nzpyida-0.9.tar", last modified: Wed Jul  5 11:16:15 2023, max compression
```

## Comparing `nzpyida-0.3.6.tar` & `nzpyida-0.9.tar`

### file list

```diff
@@ -1,158 +1,160 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.762159 nzpyida-0.3.6/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.6/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.6/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.6/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:25:47.762226 nzpyida-0.3.6/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.3.6/README.md
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.738536 nzpyida-0.3.6/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.6/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.741168 nzpyida-0.3.6/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.6/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.6/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2638 2023-05-25 14:48:09.000000 nzpyida-0.3.6/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.743181 nzpyida-0.3.6/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.6/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.745180 nzpyida-0.3.6/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.746293 nzpyida-0.3.6/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.746473 nzpyida-0.3.6/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.747185 nzpyida-0.3.6/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     1833 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.3.6/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.747691 nzpyida-0.3.6/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.750089 nzpyida-0.3.6/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/glm.py
--rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.754220 nzpyida-0.3.6/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     3591 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-05-17 10:45:26.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_cross_validation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_glm.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.754975 nzpyida-0.3.6/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)    10906 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.3.6/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.756726 nzpyida-0.3.6/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.6/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.758039 nzpyida-0.3.6/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.3.6/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.762024 nzpyida-0.3.6/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.6/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.6/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.6/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.6/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.743975 nzpyida-0.3.6/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4775 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-29 14:25:47.762509 nzpyida-0.3.6/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3318 2023-05-29 14:25:35.000000 nzpyida-0.3.6/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.534450 nzpyida-0.9/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.9/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5487 2023-07-05 11:16:15.534538 nzpyida-0.9/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9/README.md
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.504958 nzpyida-0.9/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.508213 nzpyida-0.9/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-07-05 11:15:08.000000 nzpyida-0.9/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/geoFrame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/geoSeries.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.9/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.512233 nzpyida-0.9/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.9/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.515486 nzpyida-0.9/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.517166 nzpyida-0.9/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.517349 nzpyida-0.9/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.518141 nzpyida-0.9/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.518752 nzpyida-0.9/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.521901 nzpyida-0.9/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    29001 2023-06-20 14:25:25.000000 nzpyida-0.9/nzpyida/analytics/predictive/bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-05-29 14:08:02.000000 nzpyida-0.9/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.525720 nzpyida-0.9/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     3591 2023-05-29 14:08:02.000000 nzpyida-0.9/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-05-17 10:45:26.000000 nzpyida-0.9/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6678 2023-06-20 14:25:25.000000 nzpyida-0.9/nzpyida/analytics/tests/test_bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.9/nzpyida/analytics/tests/test_cross_validation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.9/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.9/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.526223 nzpyida-0.9/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10727 2023-06-20 14:25:25.000000 nzpyida-0.9/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.9/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.527713 nzpyida-0.9/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.9/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.529139 nzpyida-0.9/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.9/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.534231 nzpyida-0.9/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.9/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.9/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.9/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.9/nzpyida/tests/test_geoFrame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.9/nzpyida/tests/test_geoSeries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.9/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-05 11:16:15.513195 nzpyida-0.9/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5487 2023-07-05 11:16:15.000000 nzpyida-0.9/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4875 2023-07-05 11:16:15.000000 nzpyida-0.9/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-05 11:16:15.000000 nzpyida-0.9/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-05 11:16:15.000000 nzpyida-0.9/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-05 11:16:15.000000 nzpyida-0.9/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      177 2023-07-05 11:16:15.534817 nzpyida-0.9/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3316 2023-07-05 11:15:08.000000 nzpyida-0.9/setup.py
```

### Comparing `nzpyida-0.3.6/LICENSE.txt` & `nzpyida-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/PKG-INFO` & `nzpyida-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.6
+Version: 0.9
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.3.6/README.md` & `nzpyida-0.9/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/.DS_Store` & `nzpyida-0.9/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/Makefile` & `nzpyida-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/make.bat` & `nzpyida-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/base.rst` & `nzpyida-0.9/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/conf.py` & `nzpyida-0.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 author = u''
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u'0.3'
+version = u'0.9'
 # The full version, including alpha/beta/rc tags.
-release = u'0.3'
+release = u'0.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'english'
```

### Comparing `nzpyida-0.3.6/docs/source/frame.rst` & `nzpyida-0.9/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/geoFrame.rst` & `nzpyida-0.9/docs/source/geoFrame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/geoSeries.rst` & `nzpyida-0.9/docs/source/geoSeries.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/geospatial.rst` & `nzpyida-0.9/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/ibm.png` & `nzpyida-0.9/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/index.rst` & `nzpyida-0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/install.rst` & `nzpyida-0.9/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/kc.ico` & `nzpyida-0.9/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/legal.rst` & `nzpyida-0.9/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/predictive.rst` & `nzpyida-0.9/docs/source/predictive.rst`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,22 @@
 -----------------------------------------------------
 
 .. automodule:: nzpyida.analytics.predictive.timeseries
    :members:
    :undoc-members:
    :show-inheritance:
 
+Tree Bayesian Networks
+-----------------------------------------------------
+
+.. automodule:: nzpyida.analytics.predictive.bayesian_networks
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Generalized Linear Models
 -----------------------------------------------------
 
 .. automodule:: nzpyida.analytics.predictive.glm
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `nzpyida-0.3.6/docs/source/start.rst` & `nzpyida-0.9/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/docs/source/utils.rst` & `nzpyida-0.9/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/__init__.py` & `nzpyida-0.9/nzpyida/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/__init__.py` & `nzpyida-0.9/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/apply.py` & `nzpyida-0.9/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.9/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.9/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.9/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.9/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.9/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.9/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/groupedapply.py` & `nzpyida-0.9/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/install.py` & `nzpyida-0.9/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/result_builder.py` & `nzpyida-0.9/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/shaper.py` & `nzpyida-0.9/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/tapply.py` & `nzpyida-0.9/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/tapply_class.py` & `nzpyida-0.9/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.9/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/aggregation.py` & `nzpyida-0.9/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/__init__.py` & `nzpyida-0.9/nzpyida/analytics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from .predictive.linear_regression import LinearRegression
 from .predictive.naive_bayes import NaiveBayesClassifier
 from .predictive.association_rules import ARule
 from .predictive.bisecting_kmeans import BisectingKMeans
 from .predictive.regression_trees import DecisionTreeRegressor
 from .predictive.two_step_clustering import TwoStepClustering
 from .predictive.timeseries import TimeSeries
+from .predictive.bayesian_networks import TreeBayesNetwork, BinaryTreeBayesNetwork, \
+MultiTreeBayesNetwork, TreeBayesNetwork1G, TreeBayesNetwork1G2P, TreeBayesNetwork2G, \
+TreeAgumentedNetwork
 from .predictive.glm import BernoulliRegressor, BinomialRegressor, \
     NegativeBinomialRegressor, GaussianRegressor, GammaRegressor, \
     PoissonRegressor, WaldRegressor
 from .exploration.distribution import bitable, moments, histogram, outliers
 from .exploration.distribution import quantile, unitable
 from .transform.discretization import EFDisc, EMDisc, EWDisc
 from .transform.discretization import ef_disc, em_disc, ew_disc
```

### Comparing `nzpyida-0.3.6/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.9/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.9/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.9/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/model_manager.py` & `nzpyida-0.9/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.9/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.9/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.9/nzpyida/analytics/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.9/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/glm.py` & `nzpyida-0.9/nzpyida/analytics/predictive/glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.9/nzpyida/analytics/predictive/kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.9/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.9/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.9/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.9/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.9/nzpyida/analytics/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.9/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.9/nzpyida/analytics/predictive/timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.9/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/conftest.py` & `nzpyida-0.9/nzpyida/analytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_cross_validation.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_glm.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.9/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.9/nzpyida/analytics/transform/discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.9/nzpyida/analytics/transform/preparation.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,16 @@
         'randseed': rand_seed
     }
     return call_proc_df_in_out(proc='RANDOM_SAMPLE', in_df=in_df, params=params,
                                out_table=out_table, copy_indexer=True)[0]
 
 
 def train_test_split(in_df: IdaDataFrame, out_table_train: str=None, out_table_test: str=None,
-                     id_column: str = None, fraction: float = 0.5, rand_seed: float = None,
-                     out_table_type: str = 'table') -> Tuple[IdaDataFrame, IdaDataFrame]:
+                     id_column: str = None, fraction: float = 0.5, 
+                     rand_seed: float = None) -> Tuple[IdaDataFrame, IdaDataFrame]:
     """
     Parameters
     ----------
     in_df : IdaDataFrame
         the input data frame
 
     out_table_train : str, optional
@@ -214,17 +214,14 @@
 
     fraction : float, optional
         the fraction of the data to that goes to the training dataframe
 
     rand_seed : int, optional
         the seed of the random function
 
-    out_table_type : str, optional
-        the type of the output tables. It can be 'table' or 'temporary'
-
     Returns
     -------
     IdaDataFrame
         the data frame with train data
     
     IdaDataFrame
         the data frame with test data
@@ -250,16 +247,15 @@
         out_table_test = make_temp_table_name()
 
     params = {
         'intable': temp_view_name,
         'traintable': out_table_train,
         'testtable': out_table_test,
         'id': id_column,
-        'fraction': fraction,
-        'outtabletype': out_table_type,
+        'fraction': fraction
     }
 
     if isinstance(rand_seed, float):
         params['seed'] = rand_seed
 
     params_s = map_to_props(params)
```

### Comparing `nzpyida-0.3.6/nzpyida/analytics/utils.py` & `nzpyida-0.9/nzpyida/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/base.py` & `nzpyida-0.9/nzpyida/base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/exceptions.py` & `nzpyida-0.9/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/__init__.py` & `nzpyida-0.9/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.9/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/entropy.py` & `nzpyida-0.9/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.9/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/gini.py` & `nzpyida-0.9/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.9/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/private.py` & `nzpyida-0.9/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.9/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/feature_selection/tstats.py` & `nzpyida-0.9/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/filtering.py` & `nzpyida-0.9/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/frame.py` & `nzpyida-0.9/nzpyida/frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/indexing.py` & `nzpyida-0.9/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/internals.py` & `nzpyida-0.9/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/__init__.py` & `nzpyida-0.9/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/iris.py` & `nzpyida-0.9/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/iris.txt` & `nzpyida-0.9/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/swiss.py` & `nzpyida-0.9/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/swiss.txt` & `nzpyida-0.9/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/titanic.py` & `nzpyida-0.9/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sampledata/titanic.txt` & `nzpyida-0.9/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/series.py` & `nzpyida-0.9/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/sql.py` & `nzpyida-0.9/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/statistics.py` & `nzpyida-0.9/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/conftest.py` & `nzpyida-0.9/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_aggregation.py` & `nzpyida-0.9/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_association_rules.py` & `nzpyida-0.9/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_base.py` & `nzpyida-0.9/nzpyida/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.9/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_base_private.py` & `nzpyida-0.9/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.9/nzpyida/tests/test_base_table_manipulation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.9/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_filtering.py` & `nzpyida-0.9/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_frame.py` & `nzpyida-0.9/nzpyida/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.9/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_frame_private.py` & `nzpyida-0.9/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_geoFrame.py` & `nzpyida-0.9/nzpyida/tests/test_geoFrame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_geoSeries.py` & `nzpyida-0.9/nzpyida/tests/test_geoSeries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_indexing.py` & `nzpyida-0.9/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_internals.py` & `nzpyida-0.9/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_kmeans.py` & `nzpyida-0.9/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.9/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_series.py` & `nzpyida-0.9/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_sorting.py` & `nzpyida-0.9/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_statistics.py` & `nzpyida-0.9/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/tests/test_utils.py` & `nzpyida-0.9/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida/utils.py` & `nzpyida-0.9/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.6/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.9/nzpyida.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.6
+Version: 0.9
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.3.6/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.9/nzpyida.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 nzpyida/analytics/model_manager.py
 nzpyida/analytics/utils.py
 nzpyida/analytics/exploration/__init__.py
 nzpyida/analytics/exploration/distribution.py
 nzpyida/analytics/exploration/relation_identification.py
 nzpyida/analytics/predictive/__init__.py
 nzpyida/analytics/predictive/association_rules.py
+nzpyida/analytics/predictive/bayesian_networks.py
 nzpyida/analytics/predictive/bisecting_kmeans.py
 nzpyida/analytics/predictive/classification.py
 nzpyida/analytics/predictive/decision_trees.py
 nzpyida/analytics/predictive/glm.py
 nzpyida/analytics/predictive/kmeans.py
 nzpyida/analytics/predictive/knn.py
 nzpyida/analytics/predictive/linear_regression.py
@@ -79,14 +80,15 @@
 nzpyida/analytics/predictive/regression.py
 nzpyida/analytics/predictive/regression_trees.py
 nzpyida/analytics/predictive/timeseries.py
 nzpyida/analytics/predictive/two_step_clustering.py
 nzpyida/analytics/tests/conftest.py
 nzpyida/analytics/tests/test_association_rules.py
 nzpyida/analytics/tests/test_auto_delete_context.py
+nzpyida/analytics/tests/test_bayesian_networks.py
 nzpyida/analytics/tests/test_bisecting_kmeans.py
 nzpyida/analytics/tests/test_cross_validation.py
 nzpyida/analytics/tests/test_decision_trees.py
 nzpyida/analytics/tests/test_discretization.py
 nzpyida/analytics/tests/test_glm.py
 nzpyida/analytics/tests/test_kmeans.py
 nzpyida/analytics/tests/test_knn.py
```

### Comparing `nzpyida-0.3.6/setup.py` & `nzpyida-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
       ]
 
 setup(name='nzpyida',
-      version='0.3.6',
+      version='0.9',
       install_requires=['pandas','numpy','future','six','pypyodbc','pyodbc', 'lazy', 'nzpy'],
 
       extras_require={
         'jdbc':['JayDeBeApi==1.*', 'Jpype1==0.6.3'],
         'test':['pytest', 'flaky==3.4.0'],
         'doc':['sphinx', 'ipython', 'numpydoc', 'sphinx_rtd_theme']
       },
```

