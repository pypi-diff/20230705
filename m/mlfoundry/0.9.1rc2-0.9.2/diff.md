# Comparing `tmp/mlfoundry-0.9.1rc2.tar.gz` & `tmp/mlfoundry-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.1rc2.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.2.tar", max compression
```

## Comparing `mlfoundry-0.9.1rc2.tar` & `mlfoundry-0.9.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     3165 2023-07-05 09:34:43.984519 mlfoundry-0.9.1rc2/README.md
--rw-r--r--   0        0        0      941 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    29009 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1840 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      813 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2768 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/constants.py
--rw-r--r--   0        0        0     1392 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/enums.py
--rw-r--r--   0        0        0      383 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      153 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     8173 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-07-05 09:34:44.000519 mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15463 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0       50 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    45909 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    47426 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4468 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/run_utils.py
--rw-r--r--   0        0        0    10048 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-07-05 09:34:44.004519 mlfoundry-0.9.1rc2/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3307 2023-07-05 09:34:55.248649 mlfoundry-0.9.1rc2/pyproject.toml
--rw-r--r--   0        0        0     4629 1970-01-01 00:00:00.000000 mlfoundry-0.9.1rc2/PKG-INFO
+-rw-r--r--   0        0        0     3165 2023-07-05 12:46:31.848489 mlfoundry-0.9.2/README.md
+-rw-r--r--   0        0        0      941 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    29009 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1840 2023-07-05 12:46:31.864490 mlfoundry-0.9.2/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      813 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2768 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/constants.py
+-rw-r--r--   0        0        0     1392 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/enums.py
+-rw-r--r--   0        0        0      383 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      153 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     8173 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    15463 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5952 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0       50 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    45880 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    47398 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4468 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0    10048 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-07-05 12:46:31.868490 mlfoundry-0.9.2/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3304 2023-07-05 12:46:43.128831 mlfoundry-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 mlfoundry-0.9.2/PKG-INFO
```

### Comparing `mlfoundry-0.9.1rc2/README.md` & `mlfoundry-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/__init__.py` & `mlfoundry-0.9.2/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/__main__.py` & `mlfoundry-0.9.2/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/amplitude.py` & `mlfoundry-0.9.2/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.2/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/background/interface.py` & `mlfoundry-0.9.2/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/background/sender.py` & `mlfoundry-0.9.2/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.2/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/background/utils.py` & `mlfoundry-0.9.2/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.2/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.2/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.2/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/constants.py` & `mlfoundry-0.9.2/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/enums.py` & `mlfoundry-0.9.2/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.2/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/git_info.py` & `mlfoundry-0.9.2/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.2/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.2/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.2/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.2/mlfoundry/log_types/artifacts/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,18 +92,18 @@
         dest_path = dest_path or ""
         normalized_path = os.path.normpath(dest_path)
         if dest_path.endswith(os.sep) or dest_path.endswith(posixpath.sep):
             normalized_path += os.sep
         dest_path = normalized_path.lstrip(os.sep)
 
         if model_dir and dest_path.startswith(model_dir):
-            raise MlFoundryException(
+            logger.warning(
                 f"Destination path {dest_path!r} in `additional_files` conflicts with "
                 f"reserved path {model_dir!r}/ which is being used to serialize the model. "
-                f"Please provide a different destination path."
+                f"This might cause errors"
             )
 
         files_abs_dir = os.path.join(root_dir, files_dir)
         dest_abs_path = os.path.join(files_abs_dir, dest_path)
 
         if os.path.isfile(src_path):
             _src = src_path
```

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.2/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.2/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.2/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.2/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.2/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.2/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/login.py` & `mlfoundry-0.9.2/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.2/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.2/mlfoundry/mlfoundry_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1044,18 +1044,17 @@
                 of (source path, destination path) to add additional files and folders
                 to the model version contents. The first member of the pair should be a file or directory path
                 and the second member should be the path inside the model versions contents to upload to.
                 The model version contents are arranged like follows
                 .
                 └── model/
                     └── # model files are serialized here
-                └── # any additional files and folders can be added here
+                └── # any additional files and folders can be added here.
 
-                To avoid corrupting any model files, the "model/" directory is reserved and additional files cannot be
-                added to it.
+                You can also add additional files to model/ subdirectory by specifying the destination path as model/
 
                 E.g. >>> client.log_model(
                      ...     ml_repo="sample-repo", name="xyz", model=clf, framework="sklearn",
                      ...     additional_files=[("foo.txt", "foo/bar/foo.txt"), ("tokenizer/", "foo/tokenizer/")]
                      ... )
                 would result in
                 .
```

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.2/mlfoundry/mlfoundry_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -930,18 +930,18 @@
                 of (source path, destination path) to add additional files and folders
                 to the model version contents. The first member of the pair should be a file or directory path
                 and the second member should be the path inside the model versions contents to upload to.
                 The model version contents are arranged like follows
                 .
                 └── model/
                     └── # model files are serialized here
-                └── # any additional files and folders can be added here
+                └── # any additional files and folders can be added here.
+
+                You can also add additional files to model/ subdirectory by specifying the destination path as model/
 
-                To avoid corrupting any model files, the "model/" directory is reserved and additional files cannot be
-                added to it.
 
                 E.g. >>> run.log_model(
                      ...     name="xyz", model=clf, framework="sklearn",
                      ...     additional_files=[("foo.txt", "foo/bar/foo.txt"), ("tokenizer/", "foo/tokenizer/")]
                      ... )
                 would result in
                 .
```

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.2/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.2/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.2/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.2/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/run_utils.py` & `mlfoundry-0.9.2/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/session.py` & `mlfoundry-0.9.2/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.2/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.2/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.2/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.2/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.2/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.1rc2/pyproject.toml` & `mlfoundry-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.1rc2" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.2" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -30,15 +30,15 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.35"
+tfy-mlflow-client = "0.0.36"
 # Check and try to eliminate libs below this comment
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.21.0"
 pytest = ">=7.2.0,<7.3.0"
```

### Comparing `mlfoundry-0.9.1rc2/PKG-INFO` & `mlfoundry-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.1rc2
+Version: 0.9.2
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,15 @@
 Requires-Dist: pandas (>=1.0.0,<2.0.0) ; python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0) ; python_version >= "3.10"
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.35)
+Requires-Dist: tfy-mlflow-client (==0.0.36)
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
 
 ![](https://github.com/MyName/my-project/workflows/Project%20Tests/badge.svg)
```

