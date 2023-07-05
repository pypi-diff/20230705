# Comparing `tmp/mlfoundry-0.9.0rc1.tar.gz` & `tmp/mlfoundry-0.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.0rc1.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.1rc1.tar", max compression
```

## Comparing `mlfoundry-0.9.0rc1.tar` & `mlfoundry-0.9.1rc1.tar`

### file list

```diff
@@ -1,114 +1,100 @@
--rw-r--r--   0        0        0     3158 2023-06-09 11:01:51.323648 mlfoundry-0.9.0rc1/README.md
--rw-r--r--   0        0        0      991 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    20613 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1392 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/enums.py
--rw-r--r--   0        0        0      383 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7978 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15275 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    44772 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46176 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/schema.py
--rw-r--r--   0        0        0    10031 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3551 2023-06-09 11:02:10.840067 mlfoundry-0.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 mlfoundry-0.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3165 2023-07-05 07:41:23.976091 mlfoundry-0.9.1rc1/README.md
+-rw-r--r--   0        0        0      941 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    29009 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1840 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      813 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2768 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/constants.py
+-rw-r--r--   0        0        0     1392 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/enums.py
+-rw-r--r--   0        0        0      383 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      153 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     8173 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    15463 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0       50 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-07-05 07:41:23.992091 mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    45909 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    47426 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4468 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0    10048 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-07-05 07:41:23.996091 mlfoundry-0.9.1rc1/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3307 2023-07-05 07:41:35.964101 mlfoundry-0.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4629 1970-01-01 00:00:00.000000 mlfoundry-0.9.1rc1/PKG-INFO
```

### Comparing `mlfoundry-0.9.0rc1/README.md` & `mlfoundry-0.9.1rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 # Development instructions
 
 ```
 git clone https://github.com/truefoundry/mlfoundry.git
 cd mlfoundry
 virtualenv venv
 source venv/bin/activate
-pip install poetry
+pip install poetry==1.4.2
 poetry install
 pre-commit install
 ```
 
 # Run Manual QA
 ```
 git clone https://github.com/truefoundry/mlf-test
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/__init__.py` & `mlfoundry-0.9.1rc1/mlfoundry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from mlfoundry.log_types.artifacts.artifact import ArtifactPath, ArtifactVersion
 from mlfoundry.log_types.artifacts.model import CustomMetric, ModelSchema, ModelVersion
 from mlfoundry.logger import init_logger
 from mlfoundry.login import login
 from mlfoundry.mlfoundry_api import get_client
 from mlfoundry.mlfoundry_run import MlFoundryRun
 from mlfoundry.monitoring.entities import Actual, Prediction, PredictionData
-from mlfoundry.schema import Schema
 from mlfoundry.version import __version__
 
 __all__ = [
     "FileFormat",
     "ModelFramework",
     "DataSlice",
     "ModelType",
-    "Schema",
     "get_client",
     "__version__",
     "MlFoundryRun",
     "login",
     "Image",
     "Plot",
     "Prediction",
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/__main__.py` & `mlfoundry-0.9.1rc1/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/amplitude.py` & `mlfoundry-0.9.1rc1/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.1rc1/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import math
 import mmap
 import os
 import posixpath
+import tempfile
 import typing
 import uuid
-from concurrent.futures import FIRST_EXCEPTION, ThreadPoolExecutor, wait
+from concurrent.futures import FIRST_EXCEPTION, Future, ThreadPoolExecutor, wait
+from shutil import rmtree
 from threading import Event
-from typing import List, NamedTuple, Optional, Tuple
+from typing import Any, Callable, List, NamedTuple, Optional, Tuple
 
 import requests
 from mlflow.entities import (
     ArtifactType,
     FileInfo,
     MultiPartUpload,
     MultiPartUploadStorageProvider,
     SignedURL,
 )
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.tracking import MlflowClient
-from mlflow.utils.file_utils import (
-    download_file_using_http_uri,
-    relative_path_to_artifact_path,
+from mlflow.utils.file_utils import relative_path_to_artifact_path
+from mlflow.utils.rest_utils import (
+    augmented_raise_for_status,
+    cloud_storage_http_request,
 )
-from mlflow.utils.rest_utils import cloud_storage_http_request
 from tqdm.utils import CallbackIOWrapper
 
 from mlfoundry.env_vars import DISABLE_MULTIPART_UPLOAD
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.logger import logger
 from mlfoundry.tracking.entities import ArtifactCredential
 from mlfoundry.tracking.truefoundry_rest_store import TruefoundryRestStore
@@ -49,15 +51,17 @@
 # Finalize the Multipart upload using the finalize signed url returned
 # by Create Multipart Upload or get a new one.
 _MAX_NUM_PARTS_FOR_MULTIPART = 1000
 
 # Azure Maximum size of a block in a block blob	4000 MiB
 # GCP/S3 Maximum size of an individual part in a multipart upload 5 GiB
 _MAX_PART_SIZE_BYTES_FOR_MULTIPART = 4 * 1024 * 1024 * 1000
+
 _MAX_WORKERS_FOR_UPLOAD = max(min(32, os.cpu_count() * 2), 4)
+_MAX_WORKERS_FOR_DOWNLOAD = max(min(32, os.cpu_count() * 2), 4)
 
 
 def _allign_part_size_with_mmap_allocation_granularity(part_size: int) -> int:
     modulo = part_size % mmap.ALLOCATIONGRANULARITY
     if modulo == 0:
         return part_size
 
@@ -142,15 +146,15 @@
             raise MlFoundryException(
                 f"remote_file_path cannot be None or empty str {remote_file_path}"
             )
 
         artifact_credential = self.rest_store.get_artifact_read_credentials(
             run_id=self._extract_run_id(self.artifact_uri), path=remote_file_path
         )
-        download_file_using_http_uri(
+        _download_file_using_http_uri(
             http_uri=artifact_credential.signed_uri, download_path=local_path
         )
 
 
 class _PartNumberEtag(NamedTuple):
     part_number: int
     etag: str
@@ -227,14 +231,34 @@
         wrapped_file = CallbackIOWrapper(callback, file, "read")
         with cloud_storage_http_request(
             "put", signed_url.url, data=wrapped_file
         ) as response:
             response.raise_for_status()
 
 
+def _download_file_using_http_uri(
+    http_uri, download_path, chunk_size=100000000, callback: Callable[[], Any] = None
+):
+    """
+    Downloads a file specified using the `http_uri` to a local `download_path`. This function
+    uses a `chunk_size` to ensure an OOM error is not raised a large file is downloaded.
+    Note : This function is meant to download files using presigned urls from various cloud
+            providers.
+    """
+    with cloud_storage_http_request("get", http_uri, stream=True) as response:
+        augmented_raise_for_status(response)
+        with open(download_path, "wb") as output_file:
+            for chunk in response.iter_content(chunk_size=chunk_size):
+                if callback:
+                    callback()
+                if not chunk:
+                    break
+                output_file.write(chunk)
+
+
 class _CallbackIOWrapperForMultiPartUpload(CallbackIOWrapper):
     def __init__(self, callback, stream, method, length: int):
         self.wrapper_setattr("_length", length)
         super().__init__(callback, stream, method)
 
     def __len__(self):
         return self.wrapper_getattr("_length")
@@ -549,19 +573,176 @@
     def log_artifact(self, local_file: str, artifact_path: Optional[str] = None):
         self._log_artifact(
             local_file=local_file,
             artifact_path=artifact_path,
             multipart_info=_decide_file_parts(local_file),
         )
 
-    def _download_file(self, remote_file_path: str, local_path: str):
+    def download_artifacts(self, artifact_path, dst_path=None, overwrite: bool = False):
+        """
+        Download an artifact file or directory to a local directory if applicable, and return a
+        local path for it. The caller is responsible for managing the lifecycle of the downloaded artifacts.
+
+        :param artifact_path: Relative source path to the desired artifacts.
+        :param dst_path: Absolute path of the local filesystem destination directory to which to
+                         download the specified artifacts. This directory must already exist.
+                         If unspecified, the artifacts will either be downloaded to a new
+                         uniquely-named directory on the local filesystem or will be returned
+                         directly in the case of the LocalArtifactRepository.
+
+        :return: Absolute path of the local filesystem location containing the desired artifacts.
+        """
+        is_dir_temp = False
+        if dst_path is None:
+            dst_path = tempfile.mkdtemp()
+            is_dir_temp = True
+
+        dst_path = os.path.abspath(dst_path)
+        if is_dir_temp:
+            logger.info(
+                f"Using temporary directory {dst_path} as the download directory"
+            )
+
+        if not os.path.exists(dst_path):
+            raise MlFoundryException(
+                message=(
+                    "The destination path for downloaded artifacts does not"
+                    " exist! Destination path: {dst_path}".format(dst_path=dst_path)
+                ),
+            )
+        elif not os.path.isdir(dst_path):
+            raise MlFoundryException(
+                message=(
+                    "The destination path for downloaded artifacts must be a directory!"
+                    " Destination path: {dst_path}".format(dst_path=dst_path)
+                ),
+            )
+
+        try:
+            # Check if the artifacts points to a directory
+            if self._is_directory(artifact_path):
+                futures, file_paths, abort_event = [], [], Event()
+
+                # Check if any file is being overwritten before downloading them
+                for file_path, download_dest_path in self._get_file_paths_recur(
+                    src_artifact_dir_path=artifact_path, dst_local_dir_path=dst_path
+                ):
+                    final_file_path = os.path.join(download_dest_path, file_path)
+
+                    # There would be no overwrite if temp directory is being used
+                    if (
+                        not is_dir_temp
+                        and os.path.exists(final_file_path)
+                        and not overwrite
+                    ):
+                        raise MlFoundryException(
+                            f"File already exists at {final_file_path}, aborting download "
+                            f"(set `overwrite` flag to overwrite this and any subsequent files)"
+                        )
+                    file_paths.append((file_path, download_dest_path))
+
+                with ThreadPoolExecutor(_MAX_WORKERS_FOR_DOWNLOAD) as executor:
+                    for file_path, download_dest_path in file_paths:
+                        future = executor.submit(
+                            self._download_artifact,
+                            src_artifact_path=file_path,
+                            dst_local_dir_path=download_dest_path,
+                            abort_event=abort_event,
+                        )
+                        futures.append(future)
+
+                    done, not_done = wait(futures, return_when=FIRST_EXCEPTION)
+                    if len(not_done) > 0:
+                        abort_event.set()
+                    for future in not_done:
+                        future.cancel()
+                    for future in done:
+                        if future.exception() is not None:
+                            raise future.exception()
+
+                    output_dir = os.path.join(dst_path, artifact_path)
+                    return output_dir
+            else:
+                return self._download_artifact(
+                    src_artifact_path=artifact_path, dst_local_dir_path=dst_path
+                )
+        except Exception as err:
+            if is_dir_temp:
+                logger.info(
+                    f"Error encountered, removing temporary download directory at {dst_path}"
+                )
+                rmtree(dst_path)  # remove temp directory alongside it's contents
+            raise err
+
+    def _download_file(
+        self, remote_file_path: str, local_path: str, abort_event: Event = None
+    ):
+        def abort_event_callback():
+            if abort_event and abort_event.is_set():
+                raise Exception("aborting download")
+
         if not remote_file_path:
             raise MlFoundryException(
                 f"remote_file_path cannot be None or empty str {remote_file_path}"
             )
         # TODO (chiragjn): Re-implement download from parent to take advantage of getting multiple signed urls at once
         #                  However care also needs to be taken to expose and pass in proper expiry because the user
         #                  user might be on slow connections or downloading many files sequentially might eat up time
         signed_url = self._tracking_client.get_signed_urls_for_artifact_version_read(
             version_id=self.version_id, paths=[remote_file_path]
         )[0]
-        download_file_using_http_uri(http_uri=signed_url.url, download_path=local_path)
+        logger.info("Downloading %s to %s", remote_file_path, local_path)
+        _download_file_using_http_uri(
+            http_uri=signed_url.url,
+            download_path=local_path,
+            callback=abort_event_callback,
+        )
+        logger.debug("Downloaded %s to %s", remote_file_path, local_path)
+
+    def _download_artifact(
+        self, src_artifact_path, dst_local_dir_path, abort_event=None
+    ):
+        """
+        Download the file artifact specified by `src_artifact_path` to the local filesystem
+        directory specified by `dst_local_dir_path`.
+        :param src_artifact_path: A relative, POSIX-style path referring to a file artifact
+                                    stored within the repository's artifact root location.
+                                    `src_artifact_path` should be specified relative to the
+                                    repository's artifact root location.
+        :param dst_local_dir_path: Absolute path of the local filesystem destination directory
+                                    to which to download the specified artifact. The downloaded
+                                    artifact may be written to a subdirectory of
+                                    `dst_local_dir_path` if `src_artifact_path` contains
+                                    subdirectories.
+        :return: A local filesystem path referring to the downloaded file.
+        """
+        local_destination_file_path = self._create_download_destination(
+            src_artifact_path=src_artifact_path, dst_local_dir_path=dst_local_dir_path
+        )
+        self._download_file(
+            remote_file_path=src_artifact_path,
+            local_path=local_destination_file_path,
+            abort_event=abort_event,
+        )
+        return local_destination_file_path
+
+    def _get_file_paths_recur(self, src_artifact_dir_path, dst_local_dir_path):
+        local_dir = os.path.join(dst_local_dir_path, src_artifact_dir_path)
+        dir_content = (
+            [  # prevent infinite loop, sometimes the dir is recursively included
+                file_info
+                for file_info in self.list_artifacts(src_artifact_dir_path)
+                if file_info.path != "." and file_info.path != src_artifact_dir_path
+            ]
+        )
+        if not dir_content:  # empty dir
+            if not os.path.exists(local_dir):
+                os.makedirs(local_dir, exist_ok=True)
+        else:
+            for file_info in dir_content:
+                if file_info.is_dir:
+                    yield from self._get_file_paths_recur(
+                        src_artifact_dir_path=file_info.path,
+                        dst_local_dir_path=dst_local_dir_path,
+                    )
+                else:
+                    yield (file_info.path, dst_local_dir_path)
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/background/interface.py` & `mlfoundry-0.9.1rc1/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/background/sender.py` & `mlfoundry-0.9.1rc1/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/background/utils.py` & `mlfoundry-0.9.1rc1/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.1rc1/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.1rc1/mlfoundry/cli/commands/login.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Optional
 
 import click
 
+from mlfoundry import env_vars
 from mlfoundry.login import login as login_
 
 
 @click.command(short_help="Store API key in the local file system")
 @click.option(
     "--tracking_uri",
     "--host",
     "tracking_uri",
     type=str,
-    default=None,
+    required=True,
+    envvar=env_vars.TRACKING_HOST_GLOBAL,
     help="Tracking server host",
 )
 @click.option(
     "--relogin",
     is_flag=True,
     show_default=True,
     default=False,
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/constants.py` & `mlfoundry-0.9.1rc1/mlfoundry/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 PROB_MULTI_DIMENSIONAL_METRICS = (
     "prob_multi_dimensional_metrics"  # multi dimensional metrics
 )
 PROB_NON_MULTI_DIMENSIONAL_METRICS = (
     "prob_non_multi_dimensional_metrics"  # non-multi dimensional metrics
 )
 
+LATEST_ARTIFACT_OR_MODEL_VERSION = "latest"
 
 ACTUAL_PREDICTION_COUNTS = "actuals_predictions_counts"
 MLF_FOLDER_NAME = "mlf"
 MLRUNS_FOLDER = "mlruns"
 MLRUNS_FOLDER_NAME = Path(os.path.join(MLF_FOLDER_NAME, MLRUNS_FOLDER))
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/enums.py` & `mlfoundry-0.9.1rc1/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.1rc1/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/git_info.py` & `mlfoundry-0.9.1rc1/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.1rc1/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.1rc1/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.1rc1/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,41 +124,47 @@
     def created_at(self) -> datetime.datetime:
         return self._artifact_version.created_at
 
     @property
     def updated_at(self) -> datetime.datetime:
         return self._artifact_version.updated_at
 
-    def raw_download(self, path: Optional[Union[str, Path]]) -> str:
+    def raw_download(
+        self, path: Optional[Union[str, Path]], overwrite: bool = False
+    ) -> str:
         logger.info(
             "Downloading artifact version contents, this might take a while ..."
         )
         mlfa_repo = MlFoundryArtifactsRepository(
             version_id=self._artifact_version.id, mlflow_client=self._mlflow_client
         )
-        return mlfa_repo.download_artifacts(artifact_path="", dst_path=path)
+        return mlfa_repo.download_artifacts(
+            artifact_path="", dst_path=path, overwrite=overwrite
+        )
 
     def _download(
-        self, path: Optional[Union[str, Path]]
+        self, path: Optional[Union[str, Path]], overwrite: bool = False
     ) -> Tuple[ArtifactVersionInternalMetadata, str]:
         self._ensure_not_deleted()
-        download_dir = self.raw_download(path=path)
+        download_dir = self.raw_download(path=path, overwrite=overwrite)
         internal_metadata_path = os.path.join(download_dir, INTERNAL_METADATA_PATH)
         if not os.path.exists(internal_metadata_path):
             raise MlFoundryException(
                 f"Artifact version seems to be corrupted or in invalid format due to missing artifact metadata. "
                 f"You can still use .raw_download(path='/your/path/here') to download and inspect files."
             )
         with open(internal_metadata_path) as f:
             internal_metadata = ArtifactVersionInternalMetadata.parse_obj(json.load(f))
         download_path = os.path.join(download_dir, internal_metadata.files_dir)
         return internal_metadata, download_path
 
-    def download(self, path: Optional[Union[str, Path]]) -> str:
-        _, download_path = self._download(path=path)
+    def download(
+        self, path: Optional[Union[str, Path]] = None, overwrite: bool = False
+    ) -> str:
+        _, download_path = self._download(path=path, overwrite=overwrite)
         return download_path
 
     def delete(self) -> bool:
         self._ensure_not_deleted()
         self._mlflow_client.delete_artifact_version(
             version_id=self._artifact_version.id
         )
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,26 +175,30 @@
     def created_at(self) -> datetime.datetime:
         return self._model_version.created_at
 
     @property
     def updated_at(self) -> datetime.datetime:
         return self._model_version.updated_at
 
-    def raw_download(self, path: Optional[Union[str, Path]]) -> str:
+    def raw_download(
+        self, path: Optional[Union[str, Path]], overwrite: bool = False
+    ) -> str:
         logger.info("Downloading model version contents, this might take a while ...")
         mlfa_repo = MlFoundryArtifactsRepository(
             version_id=self._model_version.id, mlflow_client=self._mlflow_client
         )
-        return mlfa_repo.download_artifacts(artifact_path="", dst_path=path)
+        return mlfa_repo.download_artifacts(
+            artifact_path="", dst_path=path, overwrite=overwrite
+        )
 
     def _download(
-        self, path: Optional[Union[str, Path]]
+        self, path: Optional[Union[str, Path]], overwrite: bool = False
     ) -> Tuple[ModelVersionInternalMetadata, ModelVersionDownloadInfo]:
         self._ensure_not_deleted()
-        download_dir = self.raw_download(path=path)
+        download_dir = self.raw_download(path=path, overwrite=overwrite)
         internal_metadata_path = os.path.join(download_dir, INTERNAL_METADATA_PATH)
         if not os.path.exists(internal_metadata_path):
             raise MlFoundryException(
                 f"Model version seems to be corrupted or in invalid format due to missing model metadata. "
                 f"You can still use .raw_download(path='/your/path/here') to download and inspect files."
             )
         with open(internal_metadata_path) as f:
@@ -204,16 +208,18 @@
             model_dir=os.path.join(
                 download_dir, internal_metadata.files_dir, internal_metadata.model_dir
             ),
             model_framework=internal_metadata.framework,
         )
         return internal_metadata, download_info
 
-    def download(self, path: Optional[Union[str, Path]]) -> ModelVersionDownloadInfo:
-        _, download_info = self._download(path=path)
+    def download(
+        self, path: Optional[Union[str, Path]], overwrite: bool = False
+    ) -> ModelVersionDownloadInfo:
+        _, download_info = self._download(path=path, overwrite=overwrite)
         return download_info
 
     def load(self, **load_model_kwargs):
         from mlfoundry.frameworks import get_model_registry
 
         internal_metadata, download_info = self._download(path=None)
         if internal_metadata.model_is_null:
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.1rc1/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/login.py` & `mlfoundry-0.9.1rc1/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.1rc1/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.1rc1/mlfoundry/mlfoundry_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 Besides running pytest
 """
 from __future__ import annotations
 
 import os
 import warnings
-from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import (
     Any,
     Dict,
     Generator,
     Iterator,
     List,
@@ -21,36 +20,28 @@
     Tuple,
     Union,
 )
 
 import coolname
 import mlflow
 import pandas as pd
-from mlflow.entities import (
-    Artifact,
-    ArtifactType,
-    CustomMetric,
-    Experiment,
-    Model,
-    ModelSchema,
-)
+from mlflow.entities import Artifact, ArtifactType, CustomMetric, Model, ModelSchema
 from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, env_vars
 from mlfoundry.enums import ModelFramework, ViewType
 from mlfoundry.env_vars import TRACKING_HOST_GLOBAL
 from mlfoundry.exceptions import MlflowException, MlFoundryException
 from mlfoundry.internal_namespace import NAMESPACE
 from mlfoundry.log_types.artifacts.artifact import ArtifactPath, ArtifactVersion
 from mlfoundry.log_types.artifacts.general_artifact import _log_artifact_version
 from mlfoundry.log_types.artifacts.model import ModelVersion, _log_model_version
 from mlfoundry.logger import logger
 from mlfoundry.mlfoundry_run import MlFoundryRun
-from mlfoundry.monitoring.entities import Actual, Prediction
 from mlfoundry.monitoring.store import MonitoringClient
 from mlfoundry.session import Session, get_active_session, init_session
 from mlfoundry.tracking.servicefoundry_service import ServicefoundryService
 
 
 def _get_internal_env_vars_values() -> Dict[str, str]:
     env = {}
@@ -76,20 +67,14 @@
     ### Get client
     ```python
     import mlfoundry
 
     client = mlfoundry.get_client()
     ```
     """
-    # TODO (chiragjn): Will potentially need to make MlFoundry (and possibly MlFoundryRun) a Singleton instance.
-    #                  Since this sets the tracking URI in global namespace, if someone were to call
-    #                  get_client again with different tracking uri, the ongoing run's data will start getting
-    #                  pushed to another datastore. Or we should not allow passing in tracking URI and just have
-    #                  fixed online and offline clients
-
     user_id = amplitude.NO_USER
 
     session = None
 
     # NOTE: hack to run tests
     if os.getenv(TRACKING_HOST_GLOBAL, "").startswith("file:"):
         tracking_uri = os.getenv(TRACKING_HOST_GLOBAL)
@@ -127,14 +112,27 @@
         raise MlFoundryException(
             f"ml_repo must be string type and not empty. "
             f"Got {type(project_name)} type with value {project_name!r}"
         )
     return project_name
 
 
+def _resolve_version(version: Union[int, str]) -> int:
+    if not isinstance(version, int) and not (
+        isinstance(version, str) and version.isnumeric()
+    ):
+        raise MlFoundryException(
+            f"version must be an integer or string containing numbers only. Got {version!r}"
+        )
+    final_version = int(version)
+    if final_version <= 0:
+        raise ValueError("version must be greater than 0")
+    return final_version
+
+
 class MlFoundry:
     """MlFoundry."""
 
     def __init__(self, session: Optional[Session] = None):
         """__init__.
 
         Args:
@@ -318,22 +316,24 @@
         else:
             tags = {}
 
         tags.update(_get_internal_env_vars_values())
         run = self.mlflow_client.create_run(ml_repo_id, name=run_name, tags=tags)
         mlf_run_id = run.info.run_id
 
-        mlf_run = MlFoundryRun(ml_repo_id, mlf_run_id, **kwargs)
+        mlf_run = MlFoundryRun(
+            experiment_id=ml_repo_id, run_id=mlf_run_id, auto_end=True, **kwargs
+        )
         # TODO(Rizwan): Revisit this once run lifecycle is formalised
         mlf_run._add_git_info()
         mlf_run._add_python_mlf_version()
         logger.info(f"Run {run.info.fqn!r} has started.")
         return mlf_run
 
-    def get_run(self, run_id: str) -> MlFoundryRun:
+    def get_run_by_id(self, run_id: str) -> MlFoundryRun:
         """Get an existing `run` by the `run_id`.
 
         Args:
             run_id (str): run_id or fqn of an existing `run`.
 
         Returns:
             MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
@@ -370,14 +370,40 @@
         """
         run = self.mlflow_client.get_run_by_fqn(run_fqn)
         return MlFoundryRun(
             experiment_id=run.info.experiment_id,
             run_id=run.info.run_id,
         )
 
+    def get_run_by_name(
+        self,
+        ml_repo: str,
+        run_name: str,
+    ) -> MlFoundryRun:
+        """Get an existing `run` by `run_name`.
+
+        Args:
+            ml_repo (str): name of an the project of which the run is part of.
+            run_name (str): the name of the run required
+
+        Returns:
+            MlFoundryRun: An instance of `MlFoundryRun` class which represents a `run`.
+        """
+        ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo)
+
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+
+        run = self.mlflow_client.get_run_by_name(
+            experiment_id=ml_repo_id, run_name=run_name
+        )
+        return MlFoundryRun(
+            experiment_id=run.info.experiment_id,
+            run_id=run.info.run_id,
+        )
+
     def get_all_runs(
         self,
         ml_repo: Optional[str] = None,
         project_name: Optional[str] = None,
     ) -> pd.DataFrame:
         """Returns all the run name and id present under a project.
 
@@ -427,14 +453,16 @@
     def search_runs(
         self,
         ml_repo: Optional[str] = None,
         filter_string: str = "",
         run_view_type: str = "ACTIVE_ONLY",
         order_by: Sequence[str] = ("attribute.start_time DESC",),
         project_name: Optional[str] = None,
+        job_run_name: Optional[str] = None,
+        max_results: Optional[int] = None,
     ) -> Generator[MlFoundryRun, None, None]:
         """
         The user must have `READ` access to the project.
         Returns a Generator that returns a MLFoundryRun on each next call.
         All the runs under a project which matches the filter string and the run_view_type are returned.
 
         Args:
@@ -450,14 +478,18 @@
             run_view_type (str, optional): one of the following values "ACTIVE_ONLY", "DELETED_ONLY", or "ALL" runs.
             order_by (List[str], optional):
                 List of columns to order by (e.g., "metrics.rmse"). Currently supported values
                 are metric.key, parameter.key, tag.key, attribute.key. The ``order_by`` column
                 can contain an optional ``DESC`` or ``ASC`` value. The default is ``ASC``.
                 The default ordering is to sort by ``start_time DESC``.
 
+            job_run_name (str): Name of the job which are associated with the runs to get that runs
+
+            max_results (int): max_results on the total numbers of run yielded through filter
+
         Examples:
             ```python
             import mlfoundry as mlf
 
             client = mlf.get_client()
             with client.create_run(ml_repo="my-project", run_name="run-1") as run1:
                 run1.log_metrics(metric_dict={"accuracy": 0.74, "loss": 0.6})
@@ -482,14 +514,23 @@
             # Search for the subset of runs with logged accuracy metric greater than 0.7 and order by accuracy in Descending  order
             filter_string = "metrics.accuracy > 0.7"
             order_by = ["metric.accuracy DESC"]
             runs = client.search_runs(
                 ml_repo="my-project", filter_string=filter_string, order_by=order_by
             )
 
+            filter_string = "metrics.accuracy > 0.7"
+            runs = client.search_runs(
+                ml_repo="transformers", order_by=order_by ,job_run_name='job_run_name', filter_string=filter_string
+            )
+
+            order_by = ["metric.accuracy DESC"]
+            runs = client.search_runs(
+                ml_repo="my-project", filter_string=filter_string, order_by=order_by, max_results=10
+            )
             ```
 
         Returns:
             Genarator[MlFoundryRun, None, None]: MLFoundryRuns matching the search query.
         """
         ml_repo = _resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         try:
@@ -506,33 +547,114 @@
             logger.warning(f"ML Repo with name {ml_repo} does not exist")
             return
 
         ml_repo_id = ml_repo_obj.experiment_id
 
         page_token = None
         done = False
+        if job_run_name:
+            if filter_string == "":
+                filter_string = f"tags.TFY_INTERNAL_JOB_RUN_NAME = '{job_run_name}'"
+            else:
+                filter_string += (
+                    f" and tags.TFY_INTERNAL_JOB_RUN_NAME = '{job_run_name}'"
+                )
         while not done:
             all_runs = self.mlflow_client.search_runs(
                 experiment_ids=[ml_repo_id],
                 filter_string=filter_string,
                 run_view_type=run_view_type,
-                max_results=SEARCH_MAX_RESULTS_DEFAULT,
+                max_results=min(SEARCH_MAX_RESULTS_DEFAULT, max_results)
+                if max_results
+                else SEARCH_MAX_RESULTS_DEFAULT,
                 order_by=order_by,
                 page_token=page_token,
             )
             page_token = all_runs.token
             for run in all_runs:
+                if max_results is not None:
+                    max_results -= 1
                 yield MlFoundryRun(run.info.experiment_id, run.info.run_id)
-            done = page_token is None
+            done = page_token is None or max_results == 0
 
     @staticmethod
     def get_tracking_uri():
         """get_tracking_uri."""
         return mlflow.tracking.get_tracking_uri()
 
+    def get_model_version(
+        self,
+        ml_repo: str,
+        model_name: str,
+        version: Union[str, int] = constants.LATEST_ARTIFACT_OR_MODEL_VERSION,
+    ) -> Optional[ModelVersion]:
+        """
+        Get the model version to download contents or load it in memory
+
+        Args:
+            ml_repo (str): ML Repo to which model is logged
+            model_name (str): Model Name
+            version (str | int): Model Version to fetch (default is the latest version)
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version(ml_repo="ml-repo-name", name="model-name", version=1)
+
+            # load the model into memory
+            clf = model_version.load()
+
+            # download the model to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = model_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        resolved_version = None
+        if version != constants.LATEST_ARTIFACT_OR_MODEL_VERSION:
+            resolved_version = _resolve_version(version=version)
+
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+        return self.mlflow_client.get_model_version(
+            experiment_id=int(ml_repo_id),
+            model_name=model_name,
+            version=resolved_version,
+        )
+
+    def get_model_version_by_fqn(self, fqn: str) -> ModelVersion:
+        """
+        Get the model version to download contents or load it in memory
+
+        Args:
+            fqn (str): Fully qualified name of the model version.
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_model_version_by_fqn(fqn="model:truefoundry/user/my-classification-project/my-sklearn-model:1")
+
+            # load the model into memory
+            clf = model_version.load()
+
+            # download the model to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = model_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        return ModelVersion.from_fqn(fqn=fqn)
+
     def get_model(self, fqn: str) -> ModelVersion:
         """
         Get the model version to download contents or load it in memory
 
         Args:
             fqn (str): Fully qualified name of the model version.
 
@@ -550,16 +672,18 @@
 
             # download the model to disk
             temp = tempfile.TemporaryDirectory()
             download_info = model_version.download(path=temp.name)
             print(download_info)
             ```
         """
-        # TODO (chiragjn): This API is called get_model and it returns ModelVersion
-        #   This will cause confusion later when we have to eventually introduce APIs to get the parent Model class
+        warning_message = "get_model will be deprecated in a future release. Please use get_model_version instead"
+        warnings.warn(
+            message=warning_message, category=DeprecationWarning, stacklevel=2
+        )
         return ModelVersion.from_fqn(fqn)
 
     def list_model_versions(self, ml_repo: str, name: str) -> Iterator[ModelVersion]:
         ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
         models = self.mlflow_client.list_models(ml_repo_id=ml_repo_id, name=name)
         if not models or len(models) == 0:
             err_msg = f"Model Does Not Exist for ml_repo={ml_repo}, name={name}"
@@ -616,14 +740,84 @@
             )
             page_token = model_versions.token
             for model_version in model_versions:
                 yield ModelVersion(model_version=model_version, model=model)
             if not model_versions or not page_token:
                 done = True
 
+    def get_artifact_version(
+        self,
+        ml_repo: str,
+        artifact_name: str,
+        artifact_type: Optional[ArtifactType] = ArtifactType.ARTIFACT,
+        version: Union[str, int] = constants.LATEST_ARTIFACT_OR_MODEL_VERSION,
+    ) -> Optional[ArtifactVersion]:
+        """
+        Get the model version to download contents or load it in memory
+
+        Args:
+            ml_repo (str): ML Repo to which artifact is logged
+            artifact_name (str): Artifact Name
+            artifact_type (str): The type of artifact to fetch (acceptable values: "artifact", "model", "plot", "image")
+            version (str | int): Artifact Version to fetch (default is the latest version)
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            model_version = client.get_artifact_version(ml_repo="ml-repo-name", name="artifact-name", version=1)
+
+            # load the model into memory
+            clf = model_version.load()
+
+            # download the model to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = model_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        resolved_version = None
+        if version != constants.LATEST_ARTIFACT_OR_MODEL_VERSION:
+            resolved_version = _resolve_version(version=version)
+
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+        return self.mlflow_client.get_artifact_version(
+            experiment_id=int(ml_repo_id),
+            artifact_name=artifact_name,
+            artifact_type=artifact_type,
+            version=resolved_version,
+        )
+
+    def get_artifact_version_by_fqn(self, fqn: str) -> ArtifactVersion:
+        """
+        Get the artifact version to download contents
+
+        Args:
+            fqn (str): Fully qualified name of the artifact version.
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            artifact_version = client.get_artifact_version_by_fqn(fqn="artifact:truefoundry/user/my-classification-project/sklearn-artifact:1")
+
+            # download the artifact to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = artifact_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        return ArtifactVersion.from_fqn(fqn=fqn)
+
     def get_artifact(self, fqn: str) -> ArtifactVersion:
         """
         Get the artifact version to download contents
 
         Args:
             fqn (str): Fully qualified name of the artifact version.
 
@@ -638,16 +832,18 @@
 
             # download the artifact to disk
             temp = tempfile.TemporaryDirectory()
             download_info = artifact_version.download(path=temp.name)
             print(download_info)
             ```
         """
-        # TODO (chiragjn): This API is called get_artifact and it returns ArtifactVersion
-        #   This will cause confusion later when we have to eventually introduce APIs to get the parent Artifact class
+        warning_message = "get_artifact will be deprecated in a future release. Please use get_artifact_version instead"
+        warnings.warn(
+            message=warning_message, category=DeprecationWarning, stacklevel=2
+        )
         return ArtifactVersion.from_fqn(fqn)
 
     def list_artifact_versions(
         self,
         ml_repo: str,
         name: str,
         artifact_type: Optional[ArtifactType] = ArtifactType.ARTIFACT,
@@ -946,160 +1142,7 @@
             metadata=metadata,
             model_schema=model_schema,
             custom_metrics=custom_metrics,
             step=None,
         )
         logger.info(f"Logged model successfully with fqn {model_version.fqn!r}")
         return model_version
-
-    def log_predictions(
-        self, model_version_fqn: str, predictions: List[Union[Prediction, Dict]]
-    ):
-        """log_predictions.
-
-        Args:
-            model_version_fqn (str): fqn of model_version where data needs to be logged
-            predictions (List[mlf.Prediction]): List of prediction packets of class mlf.Prediction or dictionary
-
-        example:
-            ```python
-            import mlfoundry as mlf
-            client = mlf.get_client()
-
-            client.log_predictions(
-                model_version_fqn = "",
-                predictions = [
-                    mlf.Prediction(
-                        data_id = uuid.uuid4().hex,
-                        features = {
-                            "feature1": "class1",
-                            "feature2": 3.33,
-                        },
-                        prediction_data = {
-                            "value": "pred_class1",
-                            "probabilities": {
-                                "pred_class1": 0.2,
-                                "pred_class2": 0.8
-                            },
-                            "shap_values": {}
-                        },
-                        occurred_at = datetime.utcnow(),
-                        raw_data = {"data": "any_data"}
-                    )
-                ]
-            )
-            ```
-
-        """
-
-        self.monitoring_client.log_predictions(
-            model_version_fqn=model_version_fqn, predictions=predictions
-        )
-
-    def log_actuals(self, model_version_fqn: str, actuals: List[Union[Actual, Dict]]):
-        """log_actuals.
-
-        Args:
-            model_version_fqn (str): fqn of model_version where data needs to be logged
-            actuals: (List[mlf.Actual]): List of actual packets of class mlf.Actual or a dictionary
-
-        example:
-            ```python
-            import mlfoundry as mlf
-            client = mlf.get_client()
-            data_id = uuid.uuid4().hex
-            client.log_predictions(
-                model_version_fqn = "",
-                predictions = [
-                    mlf.Prediction(
-                        data_id = data_id,
-                        features = {
-                            "feature1": "class1",
-                            "feature2": 3.33,
-                        },
-                        prediction_data = {
-                            "value": "pred_class1",
-                            "probabilities": {
-                                "pred_class1": 0.2,
-                                "pred_class2": 0.8
-                            },
-                            "shap_values": {}
-                        },
-                        occurred_at = datetime.utcnow(),
-                        raw_data = {"data": "any_data"}
-                    )
-                ]
-            )
-            client.log_actuals(
-                model_version_fqn = "",
-                actuals = [
-                    mlf.Actual(
-                        data_id = data_id,
-                        value = "pred_class2"
-                    )
-                ]
-            )
-            ```
-        """
-
-        self.monitoring_client.log_actuals(
-            model_version_fqn=model_version_fqn, actuals=actuals
-        )
-
-    def generate_hash_from_data(
-        self, features: Dict, timestamp: Optional[datetime] = None
-    ):
-        """generate_hash_from_data.
-
-        Args:
-            features (Dict): features for which you want to generate a unique hash
-            timestamp (Optional[datetime]): Optionally pass a timestamp to generate unique has for features and a timestamp
-
-        example:
-            ```python
-            import mlfoundry as mlf
-            client = mlf.get_client()
-            data_id = mlf.generate_hash_from_data(
-                features = {
-                    "features1": 1.22,
-                    "feature2" : "class2"
-                }
-            )
-            ```
-        """
-        return self.monitoring_client.generate_hash_from_data(
-            features=features, timestamp=timestamp
-        )
-
-    def get_inference_dataset(
-        self,
-        model_fqn: str,
-        start_time: Optional[datetime] = None,
-        end_time: Optional[datetime] = None,
-        actual_value_required: bool = False,
-    ):
-        """get_inference_dataset.
-        Args:
-            model_fqn(str): fqn of model for which inference data is required
-            start_time(Optional[datetime]): start_time for "occurred_at" field of the prediction
-            end_time(Optional[datetime]): start_time for "occurred_at" field of the prediction
-            actual_value_required (Optional[bool]): if true, returns inference data rows with both predictions and actuals logged, default false
-        example:
-            ```python
-            import mlfoundry as mlf
-            client = mlf.get_client()
-            inference_data = client.get_inference_dataset(model_fqn="")
-            ```
-        """
-
-        # ToDo (@nikp1172) add better logging, consider edge cases for timezones for start_time/end_time
-        if not end_time:
-            end_time = datetime.now(tz=timezone.utc)
-        if not start_time:
-            start_time = end_time - timedelta(days=7)
-            logger.info(f"start_time not passed, initializing to {start_time}")
-        return self.monitoring_client.get_inference_dataset(
-            model_fqn=model_fqn,
-            start_time=start_time,
-            end_time=end_time,
-            actual_value_required=actual_value_required,
-        )
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.1rc1/mlfoundry/mlfoundry_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import os
 import platform
 import re
 import time
+import uuid
+import warnings
 from pathlib import Path
 from typing import (
     Any,
     Collection,
     Dict,
     Iterable,
+    Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
-from urllib.parse import urlencode, urljoin, urlsplit, urlunsplit
+from urllib.parse import urljoin, urlsplit
 
 import mlflow
 from mlflow.entities import (
+    Artifact,
+    ArtifactType,
+    ArtifactVersionStatus,
     CustomMetric,
     Metric,
     ModelSchema,
     Param,
     RunInfo,
     RunStatus,
     RunTag,
@@ -44,79 +50,97 @@
     flatten_dict,
     log_artifact_blob,
     process_params,
 )
 from mlfoundry.session import ACTIVE_RUNS
 
 
+def _ensure_not_deleted(method):
+    def check_deleted_or_not(self, *args, **kwargs):
+        if self._deleted:
+            raise MlFoundryException(f"Run was deleted, cannot access a deleted Run")
+        else:
+            return method(self, *args, **kwargs)
+
+    return check_deleted_or_not
+
+
 class MlFoundryRun:
     """MlFoundryRun."""
 
     VALID_PARAM_AND_METRIC_NAMES = re.compile(r"^[A-Za-z0-9_\-\. /]+$")
 
     def __init__(
         self,
         experiment_id: str,
         run_id: str,
+        auto_end: bool = False,
         **kwargs,
     ):
         """__init__.
 
         Args:
             experiment_id (str): experiment_id
             run_id (str): run_id
+            auto_end (bool): If to end the run at garbage collection or process end (atexit)
         """
-
         self._experiment_id = str(experiment_id)
+        self._run_id = run_id
+        self._auto_end = auto_end
         # TODO (chiragjn): mlflow_client be a protected/private member
         self.mlflow_client = MlflowClient()
-        self._project_name = self.mlflow_client.get_experiment(self._experiment_id).name
-        self._run_id = run_id
         self._run_info: Optional[RunInfo] = None
-
-        from mlfoundry.dataset import TabularDatasetDriver
-
-        self._dataset_module: TabularDatasetDriver = TabularDatasetDriver(
-            mlflow_client=self.mlflow_client, run_id=run_id
-        )
-
+        self._deleted = False
         self._terminate_called = False
-        ACTIVE_RUNS.add_run(self)
+        if self._auto_end:
+            ACTIVE_RUNS.add_run(self)
         print(f"Link to the dashboard for the run: {self.dashboard_link}")
 
     def _get_run_info(self) -> RunInfo:
         if self._run_info is not None:
             return self._run_info
 
         self._run_info = self.mlflow_client.get_run(self.run_id).info
         return self._run_info
 
     @property
+    @_ensure_not_deleted
     def run_id(self) -> str:
         return self._run_id
 
     @property
+    @_ensure_not_deleted
     def run_name(self) -> str:
         return self._get_run_info().name
 
     @property
+    @_ensure_not_deleted
     def fqn(self) -> str:
         return self._get_run_info().fqn
 
     @property
+    @_ensure_not_deleted
     def status(self) -> str:
         return self.mlflow_client.get_run(self.run_id).info.status
 
     @property
+    @_ensure_not_deleted
     def ml_repo(self) -> str:
-        return self._project_name
+        return self.mlflow_client.get_experiment(self._experiment_id).name
 
+    @property
+    @_ensure_not_deleted
+    def auto_end(self) -> bool:
+        return self._auto_end
+
+    @_ensure_not_deleted
     def __repr__(self) -> str:
         return f"<{type(self).__name__} at 0x{id(self):x}: run={self.fqn!r}>"
 
+    @_ensure_not_deleted
     def __enter__(self):
         return self
 
     def _terminate_run_if_running(self, termination_status: RunStatus):
         """_terminate_run_if_running.
 
         Args:
@@ -144,27 +168,29 @@
         print(f"Finished run: {self.fqn!r}, Dashboard: {self.dashboard_link}")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         status = RunStatus.FINISHED if exc_type is None else RunStatus.FAILED
         self._terminate_run_if_running(status)
 
     def __del__(self):
-        # TODO (chiragjn): Should this be marked as FINISHED or KILLED?
-        self._terminate_run_if_running(RunStatus.FINISHED)
+        if self._auto_end:
+            self._terminate_run_if_running(RunStatus.FINISHED)
 
     @property
+    @_ensure_not_deleted
     def dashboard_link(self) -> str:
         """Get Mlfoundry dashboard link for a `run`"""
 
         base_url = "{uri.scheme}://{uri.netloc}/".format(
             uri=urlsplit(mlflow.get_tracking_uri())
         )
 
         return urljoin(base_url, f"mlfoundry/{self._experiment_id}/run/{self.run_id}/")
 
+    @_ensure_not_deleted
     def end(self, status: RunStatus = RunStatus.FINISHED):
         """End a `run`.
 
         This function marks the run as `FINISHED`.
 
         Example:
         ```python
@@ -193,14 +219,91 @@
             # Model training code
             ...
         # `run` will be automatically marked as `FINISHED` or `FAILED`.
         ```
         """
         self._terminate_run_if_running(status)
 
+    @_ensure_not_deleted
+    def delete(self) -> None:
+        """
+        This function permanently delete the run
+
+        Example:
+        ```python
+        import mlfoundry
+
+        client = mlfoundry.get_client()
+        client.create_ml_repo('iris-learning')
+        run = client.create_run(ml_repo="iris-learning", run_name="svm-model1")
+        run.log_params({"learning_rate": 0.001})
+        run.log_metrics({"accuracy": 0.7, "loss": 0.6})
+
+        run.delete()
+        ```
+
+        In case we try to call or acess any other function of that run after deleting
+        then it will through MlfoundryException
+
+        Example:
+        ```python
+        import mlfoundry
+
+        client = mlfoundry.get_client()
+        client.create_ml_repo('iris-learning')
+        run = client.create_run(ml_repo="iris-learning", run_name="svm-model1")
+        run.log_params({"learning_rate": 0.001})
+        run.log_metrics({"accuracy": 0.7, "loss": 0.6})
+
+        run.delete()
+        run.log_params({"learning_rate": 0.001})
+        ```
+        """
+        try:
+            name = self.run_name
+            self.mlflow_client.hard_delete_run(self.run_id)
+            logger.info(f"Run {name} was deleted successfully")
+            ACTIVE_RUNS.remove_run(self)
+            self._deleted = True
+            self._auto_end = False
+
+        except Exception as ex:
+            logger.warning(f"Failed to delete the run {name} because of {ex}")
+            raise
+
+    @_ensure_not_deleted
+    def list_artifact_versions(
+        self,
+        artifact_type: Optional[List[ArtifactType]] = None,
+    ) -> Iterator[ArtifactVersion]:
+        page_token, done = None, False
+        while not done:
+            artifact_versions = self.mlflow_client.list_artifact_versions(
+                run_ids=[self.run_id],
+                artifact_types=artifact_type,
+                page_token=page_token,
+            )
+            for artifact_version in artifact_versions:
+                yield ArtifactVersion.from_fqn(artifact_version.artifact_fqn)
+            done = page_token is None
+
+    @_ensure_not_deleted
+    def list_model_versions(
+        self,
+    ) -> Iterator[ModelVersion]:
+        page_token, done = 10, None, False
+        while not done:
+            model_versions = self.mlflow_client.list_model_versions(
+                page_token=page_token,
+                run_ids=[self.run_id],
+            )
+            for model_version in model_versions:
+                yield ModelVersion.from_fqn(fqn=model_version.model_fqn)
+            done = page_token is None
+
     def _add_git_info(self, root_path: Optional[str] = None):
         """_add_git_info.
 
         Args:
             root_path (Optional[str]): root_path
         """
         root_path = root_path or os.getcwd()
@@ -251,14 +354,15 @@
                 )
             )
         else:
             logger.warning("Failed to get MLFoundry version.")
 
         self.mlflow_client.log_batch(run_id=self.run_id, tags=tags)
 
+    @_ensure_not_deleted
     def download_artifact_deprecated(
         self, path: str, dest_path: Optional[str] = None
     ) -> str:
         """Downloads a logged `artifact` associated with the current `run`.
 
         Args:
             path (str): Source artifact path.
@@ -298,14 +402,15 @@
                 self.run_id, path=path, dst_path=dest_path
             )
         else:
             raise MlFoundryException(
                 f"Destination path {dest_path} should be an existing directory."
             )
 
+    @_ensure_not_deleted
     def log_artifact_deprecated(
         self, local_path: str, artifact_path: Optional[str] = None
     ):
         """Logs an artifact for the current `run`.
 
         An `artifact` is a local file or directory. This function stores the `artifact`
         at the remote artifact storage.
@@ -334,14 +439,15 @@
         run.log_artifact(local_path="artifact.txt", artifact_path="my-artifacts")
 
         run.end()
         ```
         """
         # TODO (chiragjn): this api is a little bit confusing, artifact_path is always considered to be a directory
         # which means passing local_path="a/b/c/d.txt", artifact_path="x/y/z.txt" will result in x/y/z.txt/d.txt
+
         if artifact_path is not None:
             NAMESPACE.validate_namespace_not_used(path=artifact_path)
         if os.path.isfile(local_path):
             _to = os.path.join(artifact_path or "", os.path.basename(local_path))
             logger.info(
                 f"Logging {local_path!r} file as artifact to {_to!r}, this might take a while ..."
             )
@@ -357,14 +463,15 @@
                 self.run_id, local_dir=local_path, artifact_path=artifact_path
             )
         else:
             raise MlFoundryException(
                 f"local path {local_path} should be an existing file or directory"
             )
 
+    @_ensure_not_deleted
     def log_artifact(
         self,
         name: str,
         artifact_paths: List[
             Union[Tuple[str], Tuple[str, Optional[str]], ArtifactPath]
         ],
         description: Optional[str] = None,
@@ -443,134 +550,15 @@
             name=name,
             artifact_paths=artifact_paths,
             description=description,
             metadata=metadata,
             step=step,
         )
 
-    def log_dataset(
-        self,
-        dataset_name: str,
-        features,
-        predictions=None,
-        actuals=None,
-        only_stats: bool = False,
-    ):
-        """Log a tabular dataset for the current `run`.
-
-        Log a dataset associated with a run. A dataset is a collection of features,
-        predictions and actuals. Datasets are uniquely identified by the `dataset_name`
-        under a run. They are immutable, once successfully logged, overwriting it is not allowed.
-        Mixed types are not allowed in features, actuals and predictions. However, there can be
-        missing data in the form of None, NaN, NA.
-
-        The statistics can be visualized in the mlfoundry dashboard.
-
-        Args:
-            dataset_name (str): Name of the dataset. Dataset name should only contain
-                letters(a-b, A-B), numbers (0-9), underscores (_) and hyphens (-).
-            features: Features associated with this dataset.
-                This should be either pandas DataFrame or should be of a
-                data type which can be converted to a DataFrame.
-            predictions (Iterable,optional): Predictions associated with this dataset and run. This
-                should be either pandas Series or should be of a data type which
-                can be converted to a Series. This is an optional argument.
-            actuals (Iterable, optional): Actuals associated with this dataset and run. This
-                should be either pandas Series or should be of a data type which
-                can be converted to a Series. This is an optional argument.
-            only_stats (bool, optional): If True, then the dataset
-                (features, predictions, actuals) is not saved. Only statistics and
-                the dataset schema will be persisted. Default is False.
-
-        Examples:
-        ```python
-        import mlfoundry
-
-        client = mlfoundry.get_client()
-        run = client.create_run(
-            ml_repo="my-classification-project", run_name="svm-with-rbf-kernel"
-        )
-
-        features = [
-            {"feature_1": 1, "feature_2": 1.2, "feature_3": "high"},
-            {"feature_1": 2, "feature_2": 3.5, "feature_3": "medium"},
-        ]
-        run.log_dataset(
-            dataset_name="train",
-            features=features,
-            actuals=[1.2, 1.3],
-            predictions=[3.1, 4.5],
-        )
-
-        run.end()
-        ```
-        """
-        amplitude.track(amplitude.Event.LOG_DATASET)
-        logger.info("Logging Dataset, this might take a while ...")
-        self._dataset_module.log_dataset(
-            dataset_name=dataset_name,
-            features=features,
-            predictions=predictions,
-            actuals=actuals,
-            only_stats=only_stats,
-        )
-        logger.info("Dataset logged successfully")
-        split = urlsplit(self.dashboard_link)
-        dashboard_link = urlunsplit(
-            (
-                split.scheme,
-                split.netloc,
-                split.path,
-                urlencode({"tab": "data-feature-metrics"}),
-                None,
-            )
-        )
-        print(f"To visualize the logged dataset, click on the link {dashboard_link}")
-
-    def get_dataset(self, dataset_name: str) -> Optional["mlfoundry.dataset.DataSet"]:
-        """Get a logged dataset by `dataset_name`.
-
-        Args:
-            dataset_name (str): Name of the dataset.
-
-        Returns:
-            Optional[DataSet]: Returns logged dataset as an instance of
-                the `DataSet` class. If the dataset was not logged or
-                `only_stats` was set to `True` while logging the dataset,
-                the function will return `None`.
-
-        Examples:
-        ```python
-        import mlfoundry
-
-        client = mlfoundry.get_client()
-        run = client.create_run(
-            ml_repo="my-classification-project", run_name="svm-with-rbf-kernel"
-        )
-
-        features = [
-            {"feature_1": 1, "feature_2": 1.2, "feature_3": "high"},
-            {"feature_1": 2, "feature_2": 3.5, "feature_3": "medium"},
-        ]
-        run.log_dataset(
-            dataset_name="train",
-            features=features,
-            actuals=[1.2, 1.3],
-            predictions=[3.1, 4.5],
-        )
-        dataset = run.get_dataset("train")
-        print(dataset.features) # This will be in Pandas DataFrame type.
-        print(dataset.predictions) # This will be in Pandas Series type.
-        print(dataset.actuals) # This will be in Pandas Series type.
-        run.end()
-        ```
-        """
-        amplitude.track(amplitude.Event.LOG_DATASET)
-        return self._dataset_module.get_dataset(dataset_name=dataset_name)
-
+    @_ensure_not_deleted
     def log_metrics(self, metric_dict: Dict[str, Union[int, float]], step: int = 0):
         """Log metrics for the current `run`.
 
         A metric is defined by a metric name (such as "training-loss") and a
         floating point or integral value (such as `1.2`). A metric is associated
         with a `step` which is the training iteration at which the metric was
         calculated.
@@ -631,14 +619,15 @@
         except MlflowException as e:
             raise MlFoundryException(e.message).with_traceback(
                 e.__traceback__
             ) from None
 
         logger.info("Metrics logged successfully")
 
+    @_ensure_not_deleted
     def log_params(self, param_dict: ParamsType, flatten_params: bool = False):
         """Logs parameters for the run.
 
         Parameters or Hyperparameters can be thought of as configurations for a run.
         For example, the type of kernel used in a SVM model is a parameter.
         A Parameter is defined by a name and a string value. Parameters are
         also immutable, we cannot overwrite parameter value for a parameter
@@ -713,14 +702,15 @@
             )
         except MlflowException as e:
             raise MlFoundryException(e.message).with_traceback(
                 e.__traceback__
             ) from None
         logger.info("Parameters logged successfully")
 
+    @_ensure_not_deleted
     def set_tags(self, tags: Dict[str, str]):
         """Set tags for the current `run`.
 
         Tags are "labels" for a run. A tag is represented by a tag name and value.
 
         Args:
             tags (Dict[str, str]): A tag name to value map.
@@ -749,14 +739,15 @@
             self.mlflow_client.log_batch(
                 run_id=self.run_id, metrics=[], params=[], tags=tags_arr
             )
         except MlflowException as e:
             raise MlFoundryException(e.message) from e
         logger.info("Tags set successfully")
 
+    @_ensure_not_deleted
     def get_tags(self) -> Dict[str, str]:
         """Returns all the tags set for the current `run`.
 
         Returns:
             Dict[str, str]: A dictionary containing tags. The keys in the dictionary
                 are tag names and the values are corresponding tag values.
 
@@ -775,14 +766,15 @@
         ```
         """
         amplitude.track(amplitude.Event.GET_TAGS)
 
         run = self.mlflow_client.get_run(self.run_id)
         return run.data.tags
 
+    @_ensure_not_deleted
     def auto_log_metrics(
         self,
         model_type: enums.ModelType,
         data_slice: enums.DataSlice,
         predictions: Collection[Any],
         actuals: Optional[Collection[Any]] = None,
         class_names: Optional[List[str]] = None,
@@ -814,14 +806,15 @@
             run_id=self.run_id,
             blob=metrics.json(),
             file_name=constants.ALM_METRICS_FILE_NAME,
             artifact_path=metric_path,
         )
         return metrics
 
+    @_ensure_not_deleted
     def get_metrics(
         self, metric_names: Optional[Iterable[str]] = None
     ) -> Dict[str, List[Metric]]:
         """Get metrics logged for the current `run` grouped by metric name.
 
         Args:
             metric_names (Optional[Iterable[str]], optional): A list of metric names
@@ -870,14 +863,15 @@
         valid_metrics = metric_names - unknown_metrics
         for metric_name in valid_metrics:
             metrics_dict[metric_name] = self.mlflow_client.get_metric_history(
                 self.run_id, metric_name
             )
         return metrics_dict
 
+    @_ensure_not_deleted
     def get_params(self) -> Dict[str, str]:
         """Get all the params logged for the current `run`.
 
         Returns:
             Dict[str, str]: A dictionary containing the parameters. The keys in the dictionary
                 are parameter names and the values are corresponding parameter values.
 
@@ -895,14 +889,15 @@
         run.end()
         ```
         """
         amplitude.track(amplitude.Event.GET_PARAMS)
         run = self.mlflow_client.get_run(self.run_id)
         return run.data.params
 
+    @_ensure_not_deleted
     def log_model(
         self,
         *,
         name: str,
         model: Any,
         framework: Optional[Union[enums.ModelFramework, str]],
         model_save_kwargs: Optional[Dict[str, Any]] = None,
@@ -1031,14 +1026,15 @@
             model_schema=model_schema,
             custom_metrics=custom_metrics,
             step=step,
         )
         logger.info(f"Logged model successfully with fqn {model_version.fqn!r}")
         return model_version
 
+    @_ensure_not_deleted
     def log_images(self, images: Dict[str, Image], step: int = 0):
         """Log images under the current `run` at the given `step`.
 
         Use this function to log images for a `run`. `PIL` package is needed to log images.
         To install the `PIL` package, run `pip install pillow`.
 
         Args:
@@ -1077,14 +1073,15 @@
         ```
         """
         for key, image in images.items():
             if not isinstance(image, Image):
                 raise MlFoundryException("image should be of type `mlfoundry.Image`")
             image.save(run=self, key=key, step=step)
 
+    @_ensure_not_deleted
     def log_plots(
         self,
         plots: Dict[
             str,
             Union[
                 "matplotlib.pyplot",
                 "matplotlib.figure.Figure",
@@ -1167,14 +1164,72 @@
         run.end()
         ```
         """
         for key, plot in plots.items():
             plot = Plot(plot) if not isinstance(plot, Plot) else plot
             plot.save(run=self, key=key, step=step)
 
+    @_ensure_not_deleted
+    def use_model_version_by_fqn(self, fqn: str) -> ModelVersion:
+        """
+        Get the model version to download contents or load it in memory
+
+        Args:
+            fqn (str): Fully qualified name of the model version.
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            run = client.create_run(ml_repo="my-new-project")
+            model_version = run.use_model_version_by_fqn(fqn="model:truefoundry/user/my-classification-project/my-sklearn-model:1")
+
+            # load the model into memory
+            clf = model_version.load()
+
+            # download the model to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = model_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        # TODO (chiragjn): implement event logging
+        return ModelVersion.from_fqn(fqn)
+
+    @_ensure_not_deleted
+    def use_artifact_version_by_fqn(self, fqn: str) -> ArtifactVersion:
+        """
+        Get the artifact version to download contents
+
+        Args:
+            fqn (str): Fully qualified name of the artifact version.
+
+        Examples:
+
+            ```python
+            import tempfile
+            import mlfoundry
+
+            client = mlfoundry.get_client()
+            run = client.create_run(ml_repo="my-new-project")
+            artifact_version = run.use_artifact_version_by_fqn(fqn="artifact:truefoundry/user/my-classification-project/sklearn-artifact:1")
+
+            # download the artifact to disk
+            temp = tempfile.TemporaryDirectory()
+            download_info = artifact_version.download(path=temp.name)
+            print(download_info)
+            ```
+        """
+        # TODO (chiragjn): implement event logging
+        return ArtifactVersion.from_fqn(fqn)
+
+    @_ensure_not_deleted
     def use_model(self, fqn: str) -> ModelVersion:
         """
         Get the model version to download contents or load it in memory
 
         Args:
             fqn (str): Fully qualified name of the model version.
 
@@ -1193,17 +1248,22 @@
 
             # download the model to disk
             temp = tempfile.TemporaryDirectory()
             download_info = model_version.download(path=temp.name)
             print(download_info)
             ```
         """
+        warning_message = "use_model will be deprecated in a future release. Please use use_model_version_by_fqn instead"
+        warnings.warn(
+            message=warning_message, category=DeprecationWarning, stacklevel=2
+        )
         # TODO (chiragjn): implement event logging
         return ModelVersion.from_fqn(fqn)
 
+    @_ensure_not_deleted
     def use_artifact(self, fqn: str) -> ArtifactVersion:
         """
         Get the artifact version to download contents
 
         Args:
             fqn (str): Fully qualified name of the artifact version.
 
@@ -1219,9 +1279,13 @@
 
             # download the artifact to disk
             temp = tempfile.TemporaryDirectory()
             download_info = artifact_version.download(path=temp.name)
             print(download_info)
             ```
         """
+        warning_message = "use_artifact will be deprecated in a future release. Please use use_artifact_version_by_fqn instead"
+        warnings.warn(
+            message=warning_message, category=DeprecationWarning, stacklevel=2
+        )
         # TODO (chiragjn): implement event logging
         return ArtifactVersion.from_fqn(fqn)
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.1rc1/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.1rc1/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/run_utils.py` & `mlfoundry-0.9.1rc1/mlfoundry/run_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     except Exception as ex:
         msg = error_message or f"Error importing module {module_name}"
         if required:
             raise MlFoundryException(msg) from ex
 
 
 def resolve_tracking_uri(tracking_uri: typing.Optional[str]):
-    return (
-        tracking_uri
-        or os.getenv(env_vars.TRACKING_HOST_GLOBAL)
-        or constants.DEFAULT_TRACKING_URI
-    )
+    if not tracking_uri and not os.getenv(env_vars.TRACKING_HOST_GLOBAL):
+        raise ValueError(
+            f"Either `host` should be provided by --host <value>, or `{env_vars.TRACKING_HOST_GLOBAL}` env must be set"
+        )
+    return tracking_uri or os.getenv(env_vars.TRACKING_HOST_GLOBAL)
 
 
 def append_path_to_rest_tracking_uri(tracking_uri: str):
     if urlsplit(tracking_uri).netloc.startswith("localhost"):
         return tracking_uri
     return urljoin(tracking_uri, "/api/ml")
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/session.py` & `mlfoundry-0.9.1rc1/mlfoundry/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             if run.run_id in self._active_runs:
                 del self._active_runs[run.run_id]
 
     def close_active_runs(self):
         with SESSION_LOCK:
             for run_ref in list(self._active_runs.values()):
                 run = run_ref()
-                if run:
+                if run and run.auto_end:
                     run.end()
             self._active_runs.clear()
 
 
 ACTIVE_RUNS = ActiveRuns()
 atexit.register(ACTIVE_RUNS.close_active_runs)
```

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.1rc1/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.1rc1/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.1rc1/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.1rc1/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.1rc1/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0rc1/pyproject.toml` & `mlfoundry-0.9.1rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.0rc1" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.1rc1" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -22,35 +22,26 @@
 filelock = ">=3.8.0,<4.0.0"
 numpy = ">=1.17.0,<2.0.0"
 pandas = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.0.0,<2.0.0", python = "<3.10" },
     { version = ">=1.4.0,<2.0.0", python = ">=3.10" },
 ]
-protobuf = ">=3.19.0,<3.21.0"
 psutil = ">=5.9.0,<6.0.0"
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.32"
+tfy-mlflow-client = "0.0.34"
 # Check and try to eliminate libs below this comment
-boto3 = ">=1.14.1,<2.0.0"
-fastparquet = ">=0.8.0,<=2022.12.0"
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
-pyarrow = ">=5.0.0,<11.0.0"
-whylogs = [
-    { version = ">=0.6.15,<1.0.0", python = "<3.10" },
-    { version = ">=1.0.0,<2.0.0", python = ">=3.10" }
-]
-
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.21.0"
 pytest = ">=7.2.0,<7.3.0"
 Pillow = ">=9.1.1,<10.0.0"
 doq = ">=0.9.1,<1.0.0"
 ipython = ">=7.10.0"
```

### Comparing `mlfoundry-0.9.0rc1/PKG-INFO` & `mlfoundry-0.9.1rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.0rc1
+Version: 0.9.1rc1
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.26,<4.0.0)
 Requires-Dist: amplitude-tracker (==0.0.7)
-Requires-Dist: boto3 (>=1.14.1,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: coolname (>=1.1.0,<2.0.0)
-Requires-Dist: fastparquet (>=0.8.0,<=2022.12.0)
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0)
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: packaging (>=20.0,<24.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0) ; python_version < "3.10"
 Requires-Dist: pandas (>=1.4.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: protobuf (>=3.19.0,<3.21.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
-Requires-Dist: pyarrow (>=5.0.0,<11.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.32)
-Requires-Dist: whylogs (>=0.6.15,<1.0.0) ; python_version < "3.10"
-Requires-Dist: whylogs (>=1.0.0,<2.0.0) ; python_version >= "3.10"
+Requires-Dist: tfy-mlflow-client (==0.0.34)
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
 
 ![](https://github.com/MyName/my-project/workflows/Project%20Tests/badge.svg)
 
@@ -157,15 +151,15 @@
 # Development instructions
 
 ```
 git clone https://github.com/truefoundry/mlfoundry.git
 cd mlfoundry
 virtualenv venv
 source venv/bin/activate
-pip install poetry
+pip install poetry==1.4.2
 poetry install
 pre-commit install
 ```
 
 # Run Manual QA
 ```
 git clone https://github.com/truefoundry/mlf-test
```

