# Comparing `tmp/pyreal-0.4.2.tar.gz` & `tmp/pyreal-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreal-0.4.2.tar", max compression
+gzip compressed data, was "pyreal-0.4.3.tar", max compression
```

## Comparing `pyreal-0.4.2.tar` & `pyreal-0.4.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0      165 2023-06-22 16:21:54.970868 pyreal-0.4.2/AUTHORS.rst
--rw-r--r--   0        0        0        9 2023-06-22 16:21:54.970868 pyreal-0.4.2/HISTORY.md
--rw-r--r--   0        0        0     1075 2023-06-22 16:21:54.970868 pyreal-0.4.2/LICENSE
--rw-r--r--   0        0        0     4242 2023-06-22 16:21:54.970868 pyreal-0.4.2/README.md
--rw-r--r--   0        0        0     1787 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      240 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/__init__.py
--rw-r--r--   0        0        0     3042 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/explainer_challenge.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/gfi/__init__.py
--rw-r--r--   0        0        0      436 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
--rw-r--r--   0        0        0      430 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/lfc/__init__.py
--rw-r--r--   0        0        0      439 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
--rw-r--r--   0        0        0      436 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
--rw-r--r--   0        0        0     1623 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/dataset.py
--rw-r--r--   0        0        0      610 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/download_datasets_script.py
--rw-r--r--   0        0        0     5213 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/main.py
--rw-r--r--   0        0        0    15073 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
--rw-r--r--   0        0        0     1652 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/adult_logistic_regression.pkl
--rw-r--r--   0        0        0     3108 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
--rw-r--r--   0        0        0     1244 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
--rw-r--r--   0        0        0      941 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
--rw-r--r--   0        0        0      881 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/breast-w_logistic_regression.pkl
--rw-r--r--   0        0        0     1116 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/cmc_logistic_regression.pkl
--rw-r--r--   0        0        0    62681 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
--rw-r--r--   0        0        0     1180 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
--rw-r--r--   0        0        0     1300 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/credit-g_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/diabetes_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/electricity_logistic_regression.pkl
--rw-r--r--   0        0        0     4528 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
--rw-r--r--   0        0        0     3423 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
--rw-r--r--   0        0        0      948 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/ilpd_logistic_regression.pkl
--rw-r--r--   0        0        0   129793 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/isolet_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/jm1_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/kc1_logistic_regression.pkl
--rw-r--r--   0        0        0      977 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/kc2_logistic_regression.pkl
--rw-r--r--   0        0        0     1396 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
--rw-r--r--   0        0        0     4636 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/letter_logistic_regression.pkl
--rw-r--r--   0        0        0     4865 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/madelon_logistic_regression.pkl
--rw-r--r--   0        0        0    18351 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
--rw-r--r--   0        0        0     7151 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
--rw-r--r--   0        0        0     1551 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
--rw-r--r--   0        0        0     4831 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
--rw-r--r--   0        0        0    63793 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
--rw-r--r--   0        0        0     1807 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/nomao_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/optdigits_logistic_regression.pkl
--rw-r--r--   0        0        0     1439 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/pc1_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/pc3_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/pc4_logistic_regression.pkl
--rw-r--r--   0        0        0     2351 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/pendigits_logistic_regression.pkl
--rw-r--r--   0        0        0      900 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/phoneme_logistic_regression.pkl
--rw-r--r--   0        0        0     1191 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
--rw-r--r--   0        0        0     2703 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/satimage_logistic_regression.pkl
--rw-r--r--   0        0        0    21553 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/semeion_logistic_regression.pkl
--rw-r--r--   0        0        0     1228 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/sick_logistic_regression.pkl
--rw-r--r--   0        0        0     1319 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/spambase_logistic_regression.pkl
--rw-r--r--   0        0        0     7738 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/splice_logistic_regression.pkl
--rw-r--r--   0        0        0     1025 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
--rw-r--r--   0        0        0     1444 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/vehicle_logistic_regression.pkl
--rw-r--r--   0        0        0     3384 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/vowel_logistic_regression.pkl
--rw-r--r--   0        0        0     1695 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/models/wdbc_logistic_regression.pkl
--rw-r--r--   0        0        0      145 2023-06-22 16:21:54.974868 pyreal-0.4.2/pyreal/benchmark/models.py
--rw-r--r--   0        0        0    10056 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10104 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
--rw-r--r--   0        0        0    10111 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
--rw-r--r--   0        0        0    10072 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0    10069 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10073 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0     1186 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/benchmark/task.py
--rw-r--r--   0        0        0     2315 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/__init__.py
--rw-r--r--   0        0        0    20704 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/base.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/dte/__init__.py
--rw-r--r--   0        0        0     3338 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/dte/base.py
--rw-r--r--   0        0        0     3019 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/dte/decision_tree_explainer.py
--rw-r--r--   0        0        0     3448 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/dte/surrogate_decision_tree.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/example/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/example/base.py
--rw-r--r--   0        0        0     2359 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/example/similar_examples.py
--rw-r--r--   0        0        0     4883 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/generic_explainer.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/gfi/__init__.py
--rw-r--r--   0        0        0     4301 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/gfi/base.py
--rw-r--r--   0        0        0     2984 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/gfi/global_feature_importance.py
--rw-r--r--   0        0        0     2237 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/gfi/permutation_feature_importance.py
--rw-r--r--   0        0        0     3729 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/gfi/shap_feature_importance.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/lfc/__init__.py
--rw-r--r--   0        0        0     4990 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/lfc/base.py
--rw-r--r--   0        0        0     3135 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/lfc/local_feature_contribution.py
--rw-r--r--   0        0        0     4425 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/lfc/shap_feature_contribution.py
--rw-r--r--   0        0        0     3354 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/lfc/simple_counterfactual_contribution.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/pdp/__init__.py
--rw-r--r--   0        0        0     3625 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/pdp/base.py
--rw-r--r--   0        0        0     2796 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/pdp/partial_dependence.py
--rw-r--r--   0        0        0     1929 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/pdp/partial_dependence_explainer.py
--rw-r--r--   0        0        0      372 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/time_series/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/time_series/saliency/__init__.py
--rw-r--r--   0        0        0     4689 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/time_series/saliency/base.py
--rw-r--r--   0        0        0     5623 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
--rw-r--r--   0        0        0     5916 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/realapp/__init__.py
--rw-r--r--   0        0        0    25369 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/realapp/realapp.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/sample_applications/__init__.py
--rw-r--r--   0        0        0     8997 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/sample_applications/ames_housing.py
--rw-r--r--   0        0        0     1769 2023-06-22 16:21:54.978868 pyreal-0.4.2/pyreal/sample_applications/california_housing.py
--rw-r--r--   0        0        0   460673 2023-06-22 16:21:54.982869 pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/data.csv
--rw-r--r--   0        0        0    13637 2023-06-22 16:21:54.982869 pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/data_description.txt
--rw-r--r--   0        0        0     3431 2023-06-22 16:21:54.982869 pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
--rw-r--r--   0        0        0    14681 2023-06-22 16:21:54.982869 pyreal-0.4.2/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
--rw-r--r--   0        0        0  1217129 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/data_cal_housing/california.csv
--rw-r--r--   0        0        0    68558 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/data_student/data.csv
--rw-r--r--   0        0        0     1514 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/data_student/students.csv
--rw-r--r--   0        0        0    60300 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/data_titanic/data.csv
--rw-r--r--   0        0        0     4570 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/student_performance.py
--rw-r--r--   0        0        0     3183 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/sample_applications/titanic.py
--rw-r--r--   0        0        0     1837 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/__init__.py
--rw-r--r--   0        0        0    16940 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/base.py
--rw-r--r--   0        0        0     5376 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/feature_select.py
--rw-r--r--   0        0        0     2726 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/impute.py
--rw-r--r--   0        0        0    15396 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/one_hot_encode.py
--rw-r--r--   0        0        0     2171 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/pad.py
--rw-r--r--   0        0        0     6565 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/sax.py
--rw-r--r--   0        0        0    16182 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/time_series_formatter.py
--rw-r--r--   0        0        0      469 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/type_cast.py
--rw-r--r--   0        0        0     1344 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/transformers/wrappers.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/__init__.py
--rw-r--r--   0        0        0     4137 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/base.py
--rw-r--r--   0        0        0      987 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/decision_tree.py
--rw-r--r--   0        0        0     2989 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/example_based.py
--rw-r--r--   0        0        0     5184 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/feature_based.py
--rw-r--r--   0        0        0     3084 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/feature_value_based.py
--rw-r--r--   0        0        0      646 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/types/explanations/time_series_saliency.py
--rw-r--r--   0        0        0        0 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/utils/__init__.py
--rw-r--r--   0        0        0     7810 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/utils/_plot_tree.py
--rw-r--r--   0        0        0     1968 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/utils/dataloader.py
--rw-r--r--   0        0        0     1821 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/utils/model_utils.py
--rw-r--r--   0        0        0      520 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/visualize/__init__.py
--rw-r--r--   0        0        0    14256 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/visualize/feature_based_vis.py
--rw-r--r--   0        0        0     2576 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/visualize/time_series_vis.py
--rw-r--r--   0        0        0     2687 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/visualize/tree_vis.py
--rw-r--r--   0        0        0      870 2023-06-22 16:21:54.990869 pyreal-0.4.2/pyreal/visualize/visualize_config.py
--rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 pyreal-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-07-05 17:31:15.912947 pyreal-0.4.3/AUTHORS.rst
+-rw-r--r--   0        0        0        9 2023-07-05 17:31:15.912947 pyreal-0.4.3/HISTORY.md
+-rw-r--r--   0        0        0     1075 2023-07-05 17:31:15.912947 pyreal-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4242 2023-07-05 17:31:15.912947 pyreal-0.4.3/README.md
+-rw-r--r--   0        0        0     1787 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/__init__.py
+-rw-r--r--   0        0        0     3042 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/explainer_challenge.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
+-rw-r--r--   0        0        0      430 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
+-rw-r--r--   0        0        0      436 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
+-rw-r--r--   0        0        0     1623 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/dataset.py
+-rw-r--r--   0        0        0      610 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/download_datasets_script.py
+-rw-r--r--   0        0        0     5213 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/main.py
+-rw-r--r--   0        0        0    15073 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
+-rw-r--r--   0        0        0     1652 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/adult_logistic_regression.pkl
+-rw-r--r--   0        0        0     3108 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
+-rw-r--r--   0        0        0     1244 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
+-rw-r--r--   0        0        0      941 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
+-rw-r--r--   0        0        0      881 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/breast-w_logistic_regression.pkl
+-rw-r--r--   0        0        0     1116 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/cmc_logistic_regression.pkl
+-rw-r--r--   0        0        0    62681 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
+-rw-r--r--   0        0        0     1180 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
+-rw-r--r--   0        0        0     1300 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/credit-g_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/diabetes_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/electricity_logistic_regression.pkl
+-rw-r--r--   0        0        0     4528 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
+-rw-r--r--   0        0        0     3423 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
+-rw-r--r--   0        0        0      948 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/ilpd_logistic_regression.pkl
+-rw-r--r--   0        0        0   129793 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/isolet_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/jm1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kc1_logistic_regression.pkl
+-rw-r--r--   0        0        0      977 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kc2_logistic_regression.pkl
+-rw-r--r--   0        0        0     1396 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
+-rw-r--r--   0        0        0     4636 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/letter_logistic_regression.pkl
+-rw-r--r--   0        0        0     4865 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/madelon_logistic_regression.pkl
+-rw-r--r--   0        0        0    18351 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
+-rw-r--r--   0        0        0     7151 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
+-rw-r--r--   0        0        0     1551 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
+-rw-r--r--   0        0        0     4831 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
+-rw-r--r--   0        0        0    63793 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
+-rw-r--r--   0        0        0     1807 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/nomao_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/optdigits_logistic_regression.pkl
+-rw-r--r--   0        0        0     1439 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc3_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc4_logistic_regression.pkl
+-rw-r--r--   0        0        0     2351 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pendigits_logistic_regression.pkl
+-rw-r--r--   0        0        0      900 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/phoneme_logistic_regression.pkl
+-rw-r--r--   0        0        0     1191 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
+-rw-r--r--   0        0        0     2703 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/satimage_logistic_regression.pkl
+-rw-r--r--   0        0        0    21553 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/semeion_logistic_regression.pkl
+-rw-r--r--   0        0        0     1228 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/sick_logistic_regression.pkl
+-rw-r--r--   0        0        0     1319 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/spambase_logistic_regression.pkl
+-rw-r--r--   0        0        0     7738 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/splice_logistic_regression.pkl
+-rw-r--r--   0        0        0     1025 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
+-rw-r--r--   0        0        0     1444 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/vehicle_logistic_regression.pkl
+-rw-r--r--   0        0        0     3384 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/vowel_logistic_regression.pkl
+-rw-r--r--   0        0        0     1695 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/wdbc_logistic_regression.pkl
+-rw-r--r--   0        0        0      145 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models.py
+-rw-r--r--   0        0        0    10056 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10104 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
+-rw-r--r--   0        0        0    10111 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
+-rw-r--r--   0        0        0    10072 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10069 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10073 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0     1186 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/task.py
+-rw-r--r--   0        0        0     2315 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/__init__.py
+-rw-r--r--   0        0        0    20704 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/base.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/__init__.py
+-rw-r--r--   0        0        0     3338 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/base.py
+-rw-r--r--   0        0        0     3019 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/decision_tree_explainer.py
+-rw-r--r--   0        0        0     3448 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/surrogate_decision_tree.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/base.py
+-rw-r--r--   0        0        0     2819 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/similar_examples.py
+-rw-r--r--   0        0        0     4883 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/generic_explainer.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/__init__.py
+-rw-r--r--   0        0        0     4301 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/base.py
+-rw-r--r--   0        0        0     2984 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/global_feature_importance.py
+-rw-r--r--   0        0        0     2237 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/permutation_feature_importance.py
+-rw-r--r--   0        0        0     3729 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/shap_feature_importance.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/__init__.py
+-rw-r--r--   0        0        0     4990 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/base.py
+-rw-r--r--   0        0        0     3135 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/local_feature_contribution.py
+-rw-r--r--   0        0        0     4425 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/shap_feature_contribution.py
+-rw-r--r--   0        0        0     3354 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/simple_counterfactual_contribution.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/__init__.py
+-rw-r--r--   0        0        0     3625 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/base.py
+-rw-r--r--   0        0        0     2796 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence.py
+-rw-r--r--   0        0        0     1929 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence_explainer.py
+-rw-r--r--   0        0        0      372 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/__init__.py
+-rw-r--r--   0        0        0     4689 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/base.py
+-rw-r--r--   0        0        0     5623 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
+-rw-r--r--   0        0        0     5916 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/realapp/__init__.py
+-rw-r--r--   0        0        0    26048 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/realapp/realapp.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/__init__.py
+-rw-r--r--   0        0        0     8997 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/ames_housing.py
+-rw-r--r--   0        0        0     1769 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/california_housing.py
+-rw-r--r--   0        0        0   460673 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data.csv
+-rw-r--r--   0        0        0    13637 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data_description.txt
+-rw-r--r--   0        0        0     3431 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
+-rw-r--r--   0        0        0    14681 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
+-rw-r--r--   0        0        0  1217129 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/california.csv
+-rw-r--r--   0        0        0    68558 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_student/data.csv
+-rw-r--r--   0        0        0     1514 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_student/students.csv
+-rw-r--r--   0        0        0    60300 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_titanic/data.csv
+-rw-r--r--   0        0        0     4570 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/student_performance.py
+-rw-r--r--   0        0        0     3183 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/titanic.py
+-rw-r--r--   0        0        0     1837 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/__init__.py
+-rw-r--r--   0        0        0    17977 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/base.py
+-rw-r--r--   0        0        0     5376 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/feature_select.py
+-rw-r--r--   0        0        0     2726 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/impute.py
+-rw-r--r--   0        0        0    18490 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/one_hot_encode.py
+-rw-r--r--   0        0        0     2171 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/pad.py
+-rw-r--r--   0        0        0     6565 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/sax.py
+-rw-r--r--   0        0        0    16182 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/time_series_formatter.py
+-rw-r--r--   0        0        0      469 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/type_cast.py
+-rw-r--r--   0        0        0     2055 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/wrappers.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/__init__.py
+-rw-r--r--   0        0        0     4137 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/base.py
+-rw-r--r--   0        0        0      987 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/decision_tree.py
+-rw-r--r--   0        0        0     2989 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/example_based.py
+-rw-r--r--   0        0        0     5184 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/feature_based.py
+-rw-r--r--   0        0        0     3084 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/feature_value_based.py
+-rw-r--r--   0        0        0      646 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/time_series_saliency.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/__init__.py
+-rw-r--r--   0        0        0     7810 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/_plot_tree.py
+-rw-r--r--   0        0        0     1968 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/dataloader.py
+-rw-r--r--   0        0        0     1821 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/model_utils.py
+-rw-r--r--   0        0        0      520 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/__init__.py
+-rw-r--r--   0        0        0    14256 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/feature_based_vis.py
+-rw-r--r--   0        0        0     2576 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/time_series_vis.py
+-rw-r--r--   0        0        0     2687 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/tree_vis.py
+-rw-r--r--   0        0        0      870 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/visualize_config.py
+-rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 pyreal-0.4.3/PKG-INFO
```

### Comparing `pyreal-0.4.2/LICENSE` & `pyreal-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/README.md` & `pyreal-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyproject.toml` & `pyreal-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 maintainers = [
   "MIT Data To AI Lab <dailabmit@gmail.com>",
 ]
 
 description = "Library for evaluating and deploying human readable machine learning explanations."
 name = "pyreal"
-version = "0.4.2"
+version = "0.4.3"
 
 license = ""
 
 readme = "README.md"
 
 documentation = "https://sibyl-dev.github.io/pyreal"
 homepage = "https://sibyl-ml.dev/"
```

### Comparing `pyreal-0.4.2/pyreal/benchmark/challenges/explainer_challenge.py` & `pyreal-0.4.3/pyreal/benchmark/challenges/explainer_challenge.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/dataset.py` & `pyreal-0.4.3/pyreal/benchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/download_datasets_script.py` & `pyreal-0.4.3/pyreal/benchmark/download_datasets_script.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/main.py` & `pyreal-0.4.3/pyreal/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/adult_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/adult_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/balance-scale_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/balance-scale_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/breast-w_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/breast-w_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/cmc_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/cmc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/cnae-9_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/cnae-9_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/credit-approval_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/credit-approval_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/credit-g_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/credit-g_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/diabetes_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/diabetes_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/electricity_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/electricity_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/ilpd_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/ilpd_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/isolet_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/isolet_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/jm1_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/jm1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/kc1_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/kc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/kc2_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/kc2_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/letter_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/letter_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/madelon_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/madelon_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/mnist_784_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/mnist_784_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/nomao_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/nomao_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/optdigits_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/optdigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/pc1_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/pc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/pc3_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/pc3_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/pc4_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/pc4_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/pendigits_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/pendigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/phoneme_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/phoneme_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/satimage_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/satimage_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/semeion_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/semeion_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/sick_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/sick_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/spambase_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/spambase_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/splice_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/splice_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/vehicle_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/vehicle_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/vowel_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/vowel_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/models/wdbc_logistic_regression.pkl` & `pyreal-0.4.3/pyreal/benchmark/models/wdbc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge` & `pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/benchmark/task.py` & `pyreal-0.4.3/pyreal/benchmark/task.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/__init__.py` & `pyreal-0.4.3/pyreal/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/base.py` & `pyreal-0.4.3/pyreal/explainers/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/dte/base.py` & `pyreal-0.4.3/pyreal/explainers/dte/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/dte/decision_tree_explainer.py` & `pyreal-0.4.3/pyreal/explainers/dte/decision_tree_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/dte/surrogate_decision_tree.py` & `pyreal-0.4.3/pyreal/explainers/dte/surrogate_decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/example/base.py` & `pyreal-0.4.3/pyreal/explainers/example/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/example/similar_examples.py` & `pyreal-0.4.3/pyreal/explainers/example/similar_examples.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from sklearn.neighbors import KDTree
+from sklearn.preprocessing import StandardScaler
 
 from pyreal.explainers.example.base import ExampleBasedBase
 from pyreal.types.explanations.example_based import SimilarExampleExplanation
 
 
 class SimilarExamples(ExampleBasedBase):
     """
@@ -13,19 +14,23 @@
     SimilarExamples explainers expect data to be entirely numeric
 
     Args:
         model (string filepath or model object):
            Filepath to the pickled model to explain, or model object with .predict() function
         x_train_orig (DataFrame of size (n_instances, n_features)):
             Training set in original form.
+        standardize (Boolean):
+            If True, standardize the data when selected similar examples
         **kwargs: see base Explainer args
     """
 
-    def __init__(self, model, x_train_orig=None, **kwargs):
+    def __init__(self, model, x_train_orig=None, standardize=False, **kwargs):
         self.explainer = None
+        self.standardize = standardize
+        self.standardizer = None
         super(SimilarExamples, self).__init__(model, x_train_orig, **kwargs)
 
     def fit(self, x_train_orig=None, y_train=None):
         """
         Fit the explainer
 
         Args:
@@ -33,14 +38,17 @@
                 Training set to fit on, required if not provided on initialization
             y_train:
                 Targets of training set, required if not provided on initialization
         """
         x_train_orig, y_train = self._get_training_data(x_train_orig, y_train)
 
         dataset = self.transform_to_x_algorithm(x_train_orig)
+        if self.standardize:
+            self.standardizer = StandardScaler()
+            dataset = self.standardizer.fit_transform(dataset)
         self.explainer = KDTree(dataset)
         self.y_train = y_train
         self.x_train_orig = x_train_orig
 
         return self
 
     def get_explanation(self, x_orig, n=5):
@@ -54,13 +62,14 @@
                 Number of neighbors to return
         Returns:
             SimilarExamples
         """
         if self.explainer is None:
             raise AttributeError("Instance has no explainer. Must call fit() before produce()")
         x = self.transform_to_x_algorithm(x_orig)
-
+        if self.standardize:
+            x = self.standardizer.transform(x)
         inds = self.explainer.query(x, k=n, return_distance=False)
         explanation = {}
         for i in range(len(inds)):
             explanation[i] = (self.x_train_orig.iloc[inds[i], :], self.y_train.iloc[inds[i]])
         return SimilarExampleExplanation(explanation)
```

### Comparing `pyreal-0.4.2/pyreal/explainers/generic_explainer.py` & `pyreal-0.4.3/pyreal/explainers/generic_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/gfi/base.py` & `pyreal-0.4.3/pyreal/explainers/gfi/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/gfi/global_feature_importance.py` & `pyreal-0.4.3/pyreal/explainers/gfi/global_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/gfi/permutation_feature_importance.py` & `pyreal-0.4.3/pyreal/explainers/gfi/permutation_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/gfi/shap_feature_importance.py` & `pyreal-0.4.3/pyreal/explainers/gfi/shap_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/lfc/base.py` & `pyreal-0.4.3/pyreal/explainers/lfc/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/lfc/local_feature_contribution.py` & `pyreal-0.4.3/pyreal/explainers/lfc/local_feature_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/lfc/shap_feature_contribution.py` & `pyreal-0.4.3/pyreal/explainers/lfc/shap_feature_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/lfc/simple_counterfactual_contribution.py` & `pyreal-0.4.3/pyreal/explainers/lfc/simple_counterfactual_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/pdp/base.py` & `pyreal-0.4.3/pyreal/explainers/pdp/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/pdp/partial_dependence.py` & `pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/pdp/partial_dependence_explainer.py` & `pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/time_series/saliency/base.py` & `pyreal-0.4.3/pyreal/explainers/time_series/saliency/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py` & `pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py` & `pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/realapp/realapp.py` & `pyreal-0.4.3/pyreal/realapp/realapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,17 +424,17 @@
         preds_dict = {}
         for i, row_id in enumerate(ids):
             preds_dict[row_id] = preds[i]
         return preds_dict
 
     def prepare_feature_contributions(
         self,
-        model_id=None,
         x_train_orig=None,
         y_train=None,
+        model_id=None,
         algorithm=None,
         shap_type=None,
         training_size=None,
     ):
         """
         Initialize and fit a local feature contribution explainer
 
@@ -527,17 +527,17 @@
             force_refit=force_refit,
             training_size=training_size,
             prepare_kwargs={"shap_type": shap_type},
         )
 
     def prepare_feature_importance(
         self,
-        model_id=None,
         x_train_orig=None,
         y_train=None,
+        model_id=None,
         algorithm=None,
         shap_type=None,
         training_size=None,
     ):
         """
         Initialize and fit a global feature importance explainer
 
@@ -625,19 +625,20 @@
             force_refit=force_refit,
             training_size=training_size,
             prepare_kwargs={"shap_type": shap_type},
         )
 
     def prepare_similar_examples(
         self,
-        model_id=None,
         x_train_orig=None,
         y_train=None,
+        model_id=None,
         algorithm=None,
         training_size=None,
+        standardize=False,
     ):
         """
         Initialize and fit a nearest neighbor explainer
 
         Args:
             model_id (int or string):
                 Model id to explain
@@ -645,14 +646,17 @@
                 Training data, if not provided at initialization.
             y_train (DataFrame or Series):
                 Training targets, if not provided at initialization
             algorithm (string):
                 NN algorithm to use (current options: [nn])
             training_size (int):
                 Number of rows to use in fitting explainer
+            standardize (Boolean):
+                If True, standardize data before using it to get similar examples.
+                Recommended if model-ready data is not already standardized
 
         Returns:
             A fit SimilarExamples explainer
         """
         if algorithm is None:
             algorithm = "nn"
 
@@ -663,26 +667,28 @@
             self.models[model_id],
             transformers=self.transformers,
             feature_descriptions=self.feature_descriptions,
             e_algorithm=algorithm,
             classes=self.classes,
             class_descriptions=self.class_descriptions,
             training_size=training_size,
+            standardize=standardize,
         )
         explainer.fit(self._get_x_train_orig(x_train_orig), self._get_y_train(y_train))
         self._add_explainer("se", algorithm, explainer)
         return explainer
 
     def produce_similar_examples(
         self,
         x_orig,
         model_id=None,
         x_train_orig=None,
         y_train=None,
         n=3,
+        standardize=False,
         algorithm=None,
         force_refit=False,
     ):
         """
         Produce a SimilarExamples explainer
 
         Args:
@@ -692,14 +698,17 @@
                 ID of model to explain
             x_train_orig (DataFrame):
                 Data to fit on, if not provided during initialization
             y_train (DataFrame or Series):
                 Training targets to fit on, if not provided during initialization
             n (int):
                 Number of similar examples to return
+            standardize (Boolean):
+                If True, standardize data before using it to get similar examples.
+                Recommended if model-ready data is not already standardized
             algorithm (string):
                 Name of algorithm
             force_refit (Boolean):
                 If True, initialize and fit a new explainer even if the appropriate explainer
                 already exists
 
         Returns:
@@ -714,27 +723,30 @@
             self.prepare_similar_examples,
             format_similar_examples_output,
             x_orig=x_orig,
             model_id=model_id,
             x_train_orig=x_train_orig,
             y_train=y_train,
             force_refit=force_refit,
+            prepare_kwargs={"standardize": standardize},
             produce_kwargs={"n": n},
         )
 
     def _get_x_train_orig(self, x_train_orig):
         """
         Helper function to get the appropriate x_orig or raise errors if something goes wrong
         Args:
             x_train_orig (DataFrame or None):
                 Provided DataFrame
         Returns:
             The dataframe to use (x_orig or self.x_train_orig), may be None if neither is given
         """
         if x_train_orig is not None:
+            if self.id_column is not None and self.id_column in x_train_orig:
+                return x_train_orig.drop(columns=self.id_column)
             return x_train_orig
         else:
             return self.X_train_orig
 
     def _get_y_train(self, y_train):
         """
         Helper function to get the appropriate y or raise errors if something goes wrong
```

### Comparing `pyreal-0.4.2/pyreal/sample_applications/ames_housing.py` & `pyreal-0.4.3/pyreal/sample_applications/ames_housing.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/california_housing.py` & `pyreal-0.4.3/pyreal/sample_applications/california_housing.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/data.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/data_description.txt` & `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data_description.txt`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_cal_housing/california.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/california.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_student/data.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_student/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_student/students.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_student/students.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/data_titanic/data.csv` & `pyreal-0.4.3/pyreal/sample_applications/data_titanic/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/student_performance.py` & `pyreal-0.4.3/pyreal/sample_applications/student_performance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/sample_applications/titanic.py` & `pyreal-0.4.3/pyreal/sample_applications/titanic.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/__init__.py` & `pyreal-0.4.3/pyreal/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/base.py` & `pyreal-0.4.3/pyreal/transformers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,41 @@
         Returns:
             (DataFrame of shape (n_instances, n_transformed_features):
                 The transformed dataset
         """
         self.fit(x, **fit_params)
         return self.data_transform(x)
 
+    def inverse_data_transform(self, x_new):
+        """
+        Wrapper for inverse_data_transform.
+        Transforms data `x_new` from new feature space back into the original feature space.
+        Args:
+            x_new (DataFrame of shape (n_instances, n_transformed_features)):
+                The dataset to inverse-transform
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The inverse-transformed dataset
+        """
+        raise NotImplementedError("Inverse transform is not defined for this Transformer.")
+
+    def inverse_transform(self, x_new):
+        """
+        Transforms data `x_new` from new feature space back into the original feature space.
+        Args:
+            x_new (DataFrame of shape (n_instances, n_transformed_features)):
+                The dataset to inverse-transform
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The inverse-transformed dataset
+        """
+        return self.inverse_data_transform(x_new)
+
     def inverse_transform_explanation(self, explanation):
         """
         Transforms the explanation from the second feature space handled by this transformer
         to the first.
 
         Args:
             explanation (Explanation):
```

### Comparing `pyreal-0.4.2/pyreal/transformers/feature_select.py` & `pyreal-0.4.3/pyreal/transformers/feature_select.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/impute.py` & `pyreal-0.4.3/pyreal/transformers/impute.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/one_hot_encode.py` & `pyreal-0.4.3/pyreal/transformers/one_hot_encode.py`

 * *Files 22% similar despite different names*

```diff
@@ -112,14 +112,16 @@
             columns (dataframe column label type or list of dataframe column label type):
                 Label of column to select, or an ordered list of column labels to select
         """
         self.ohe = SklearnOneHotEncoder(sparse_output=False)
         if columns is not None and not isinstance(columns, (list, tuple, np.ndarray, pd.Index)):
             columns = [columns]
         self.columns = columns
+        self.orig_columns = None
+        self.onehot_columns = None
         super().__init__(**kwargs)
 
     def fit(self, x, **params):
         """
         Fit this transformer to data
 
         Args:
@@ -128,15 +130,17 @@
 
         Returns:
             None
         """
 
         if self.columns is None:
             self.columns = x.columns
+        self.orig_columns = x.columns
         self.ohe.fit(x[self.columns])
+        self.onehot_columns = self.ohe.get_feature_names_out(self.columns)
         return super().fit(x)
 
     def data_transform(self, x):
         """
         One-hot encode `x`.
         Args:
             x (DataFrame of shape (n_instances, n_features)):
@@ -146,20 +150,39 @@
             DataFrame of shape (n_instances, n_transformed_features):
                 The one-hot encoded dataset
         """
 
         if not self.fitted:
             raise RuntimeError("Must fit one hot encoder before transforming")
         x_to_encode = x[self.columns]
-        columns = self.ohe.get_feature_names_out(x_to_encode.columns)
         index = x_to_encode.index
         x_cat_ohe = self.ohe.transform(x_to_encode)
-        x_cat_ohe = pd.DataFrame(x_cat_ohe, columns=columns, index=index)
+        x_cat_ohe = pd.DataFrame(x_cat_ohe, columns=self.onehot_columns, index=index)
         return pd.concat([x.drop(self.columns, axis="columns"), x_cat_ohe], axis=1)
 
+    def inverse_data_transform(self, x_new):
+        """
+        Transforms one-hot encoded data `x_new` back into the original feature space.
+        Args:
+            x_new (DataFrame of shape (n_instances, n_transformed_features)):
+                The one-hot encoded dataset
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The inverse-transformed dataset
+        """
+        if not self.fitted:
+            raise RuntimeError("Must fit one hot encoder before performing inverse transform")
+        index = x_new.index
+        x_orig = self.ohe.inverse_transform(x_new[self.onehot_columns])
+        x_orig = pd.DataFrame(x_orig, columns=self.columns, index=index)
+        unordered_x = pd.concat([x_new.drop(self.onehot_columns, axis="columns"), x_orig], axis=1)
+
+        return unordered_x[self.orig_columns]
+
     def inverse_transform_explanation_additive_feature_contribution(self, explanation):
         """
         Combine the contributions of one-hot-encoded features through adding to get the
         contributions of the original categorical feature.
 
         Args:
             explanation (AdditiveFeatureContributionExplanation):
@@ -320,14 +343,42 @@
             else:
                 ohe_feature_dict = self.mappings.categorical_to_one_hot[col]
                 for ohe_feature in ohe_feature_dict:
                     ohe_data[ohe_feature] = np.zeros(num_rows, dtype=bool)
                     ohe_data[ohe_feature][np.where(values == ohe_feature_dict[ohe_feature])] = True
         return pd.DataFrame(ohe_data)
 
+    def inverse_data_transform(self, x_onehot):
+        """
+        Transforms one-hot encoded data `x_onehot` back into categorical form.
+        Args:
+            x_onehot (DataFrame of shape (n_instances, n_transformed_features)):
+                The one-hot encoded dataset
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The dataset in categorical form
+        """
+        cat_data = {}
+        cols = x_onehot.columns
+        num_rows = x_onehot.shape[0]
+
+        for col in cols:
+            if col not in self.mappings.one_hot_to_categorical:
+                cat_data[col] = x_onehot[col]
+            else:
+                new_name = self.mappings.one_hot_to_categorical[col][0]
+                if new_name not in cat_data:
+                    cat_data[new_name] = np.empty(num_rows, dtype="object")
+                # TODO: add functionality to handle defaults
+                cat_data[new_name][np.where(x_onehot[col] == 1)] = (
+                    self.mappings.one_hot_to_categorical[col][1]
+                )
+        return pd.DataFrame(cat_data)
+
     def inverse_transform_explanation_additive_feature_contribution(self, explanation):
         explanation = pd.DataFrame(explanation.get())
         if explanation.ndim == 1:
             explanation = explanation.reshape(1, -1)
         for original_feature in self.mappings.categorical_to_one_hot.keys():
             encoded_features = self.mappings.categorical_to_one_hot[original_feature].keys()
             summed_contribution = explanation[encoded_features].sum(axis=1)
@@ -377,14 +428,39 @@
                     cat_data[new_name] = np.empty(num_rows, dtype="object")
                 # TODO: add functionality to handle defaults
                 cat_data[new_name][np.where(x[col] == 1)] = self.mappings.one_hot_to_categorical[
                     col
                 ][1]
         return pd.DataFrame(cat_data)
 
+    def inverse_data_transform(self, x_cat):
+        """
+        Transforms one-hot decoded data `x_cat` back into one-hot encoded form.
+        Args:
+            x_cat (DataFrame of shape (n_instances, n_transformed_features)):
+                The dataset to transform
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The one-hot encoded dataset
+        """
+        cols = x_cat.columns
+        num_rows = x_cat.shape[0]
+        ohe_data = {}
+        for col in cols:
+            values = x_cat[col]
+            if col not in self.mappings.categorical_to_one_hot:
+                ohe_data[col] = values
+            else:
+                ohe_feature_dict = self.mappings.categorical_to_one_hot[col]
+                for ohe_feature in ohe_feature_dict:
+                    ohe_data[ohe_feature] = np.zeros(num_rows, dtype=bool)
+                    ohe_data[ohe_feature][np.where(values == ohe_feature_dict[ohe_feature])] = True
+        return pd.DataFrame(ohe_data)
+
     def transform_explanation_additive_feature_contribution(self, explanation):
         """
         Transforms additive contribution explanations
 
         Args:
             explanation (AdditiveFeatureContributionExplanation):
                 The explanation to be transformed
```

### Comparing `pyreal-0.4.2/pyreal/transformers/pad.py` & `pyreal-0.4.3/pyreal/transformers/pad.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/sax.py` & `pyreal-0.4.3/pyreal/transformers/sax.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/time_series_formatter.py` & `pyreal-0.4.3/pyreal/transformers/time_series_formatter.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/transformers/wrappers.py` & `pyreal-0.4.3/pyreal/transformers/wrappers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 
 from pyreal.transformers import Transformer
 
 
 class DataFrameWrapper(Transformer):
     """
@@ -43,7 +44,24 @@
 
         Returns:
             DataFrame of shape (n_instances, n_transformed_features):
                 The transformed dataset
         """
         transformed_np = self.wrapped_transformer.transform(x)
         return pd.DataFrame(transformed_np, columns=x.columns, index=x.index)
+
+    def inverse_data_transform(self, x_new):
+        """
+        Inverese transform `x_new` using the wrapped transformer
+        Args:
+            x_new (DataFrame of shape (n_instances, n_transformed_features)):
+                The dataset to inverse transform
+
+        Returns:
+            DataFrame of shape (n_instances, n_features):
+                The dataset after inverse transform
+        """
+        inv_transformed_data = self.wrapped_transformer.inverse_transform(x_new)
+        if isinstance(inv_transformed_data, np.ndarray):
+            return pd.DataFrame(inv_transformed_data, columns=x_new.columns, index=x_new.index)
+        else:
+            return inv_transformed_data
```

### Comparing `pyreal-0.4.2/pyreal/types/explanations/base.py` & `pyreal-0.4.3/pyreal/types/explanations/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/types/explanations/decision_tree.py` & `pyreal-0.4.3/pyreal/types/explanations/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/types/explanations/example_based.py` & `pyreal-0.4.3/pyreal/types/explanations/example_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/types/explanations/feature_based.py` & `pyreal-0.4.3/pyreal/types/explanations/feature_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/types/explanations/feature_value_based.py` & `pyreal-0.4.3/pyreal/types/explanations/feature_value_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/types/explanations/time_series_saliency.py` & `pyreal-0.4.3/pyreal/types/explanations/time_series_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/utils/_plot_tree.py` & `pyreal-0.4.3/pyreal/utils/_plot_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/utils/dataloader.py` & `pyreal-0.4.3/pyreal/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/utils/model_utils.py` & `pyreal-0.4.3/pyreal/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/visualize/__init__.py` & `pyreal-0.4.3/pyreal/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/visualize/feature_based_vis.py` & `pyreal-0.4.3/pyreal/visualize/feature_based_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/visualize/time_series_vis.py` & `pyreal-0.4.3/pyreal/visualize/time_series_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/visualize/tree_vis.py` & `pyreal-0.4.3/pyreal/visualize/tree_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/pyreal/visualize/visualize_config.py` & `pyreal-0.4.3/pyreal/visualize/visualize_config.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.2/PKG-INFO` & `pyreal-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreal
-Version: 0.4.2
+Version: 0.4.3
 Summary: Library for evaluating and deploying human readable machine learning explanations.
 Home-page: https://sibyl-ml.dev/
 Keywords: pyreal,Pyreal
 Author: Alexandra Zytek
 Author-email: zyteka@mit.edu
 Maintainer: MIT Data To AI Lab
 Maintainer-email: dailabmit@gmail.com
```

