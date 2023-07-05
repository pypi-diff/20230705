# Comparing `tmp/google-cloud-automl-2.8.3.tar.gz` & `tmp/google-cloud-automl-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automl-2.8.3.tar", last modified: Mon Oct 10 16:28:05 2022, max compression
+gzip compressed data, was "google-cloud-automl-2.9.0.tar", last modified: Thu Dec 15 22:35:34 2022, max compression
```

## Comparing `google-cloud-automl-2.8.3.tar` & `google-cloud-automl-2.9.0.tar`

### file list

```diff
@@ -1,149 +1,152 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.973733 google-cloud-automl-2.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4642 2022-10-10 16:28:05.973733 google-cloud-automl-2.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3718 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.945741 google-cloud-automl-2.8.3/google/
--rw-rw-r--   0 root         (0)     1003      748 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.945741 google-cloud-automl-2.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.949740 google-cloud-automl-2.8.3/google/cloud/automl/
--rw-rw-r--   0 root         (0)     1003     9596 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl/__init__.py
--rw-rw-r--   0 root         (0)     1003       80 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.949740 google-cloud-automl-2.8.3/google/cloud/automl_v1/
--rw-rw-r--   0 root         (0)     1003     7628 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5626 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       80 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.949740 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.949740 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/
--rw-rw-r--   0 root         (0)     1003      737 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/__init__.py
--rw-rw-r--   0 root         (0)     1003   101606 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/async_client.py
--rw-rw-r--   0 root         (0)     1003   111843 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/client.py
--rw-rw-r--   0 root         (0)     1003    15773 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.949740 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17521 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33739 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34435 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.953739 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/
--rw-rw-r--   0 root         (0)     1003      781 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    29213 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    38191 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.953739 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6869 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15780 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16091 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.957738 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/
--rw-rw-r--   0 root         (0)     1003     5901 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4388 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/annotation_payload.py
--rw-rw-r--   0 root         (0)     1003     1701 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/annotation_spec.py
--rw-rw-r--   0 root         (0)     1003    11088 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/classification.py
--rw-rw-r--   0 root         (0)     1003     8821 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/data_items.py
--rw-rw-r--   0 root         (0)     1003     6325 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     5151 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/detection.py
--rw-rw-r--   0 root         (0)     1003     2056 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    13359 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/image.py
--rw-rw-r--   0 root         (0)     1003    60612 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/io.py
--rw-rw-r--   0 root         (0)     1003     6739 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/model.py
--rw-rw-r--   0 root         (0)     1003     6599 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/model_evaluation.py
--rw-rw-r--   0 root         (0)     1003    10460 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/operations.py
--rw-rw-r--   0 root         (0)     1003    11189 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/prediction_service.py
--rw-rw-r--   0 root         (0)     1003    17589 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     2951 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text.py
--rw-rw-r--   0 root         (0)     1003     3731 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_extraction.py
--rw-rw-r--   0 root         (0)     1003     1737 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_segment.py
--rw-rw-r--   0 root         (0)     1003     4268 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_sentiment.py
--rw-rw-r--   0 root         (0)     1003     3327 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1/types/translation.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.957738 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/
--rw-rw-r--   0 root         (0)     1003    10780 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7190 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       80 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.957738 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.957738 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/
--rw-rw-r--   0 root         (0)     1003      737 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/__init__.py
--rw-rw-r--   0 root         (0)     1003   129510 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/async_client.py
--rw-rw-r--   0 root         (0)     1003   141190 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/client.py
--rw-rw-r--   0 root         (0)     1003    26054 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.961737 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/
--rw-rw-r--   0 root         (0)     1003     1122 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21681 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41416 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    42299 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.961737 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/
--rw-rw-r--   0 root         (0)     1003      781 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    28672 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37650 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.961737 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6874 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15356 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15667 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.961737 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/
--rw-rw-r--   0 root         (0)     1003        0 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/__init__.py
--rw-rw-r--   0 root         (0)     1003     5631 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/gcs_client.py
--rw-rw-r--   0 root         (0)     1003   130534 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/tables_client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     8243 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5663 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/annotation_payload.py
--rw-rw-r--   0 root         (0)     1003     1707 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/annotation_spec.py
--rw-rw-r--   0 root         (0)     1003    13900 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/classification.py
--rw-rw-r--   0 root         (0)     1003     3876 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/column_spec.py
--rw-rw-r--   0 root         (0)     1003    11034 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_items.py
--rw-rw-r--   0 root         (0)     1003    10498 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_stats.py
--rw-rw-r--   0 root         (0)     1003     4628 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_types.py
--rw-rw-r--   0 root         (0)     1003     7129 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     8908 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/detection.py
--rw-rw-r--   0 root         (0)     1003     2066 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    12372 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/image.py
--rw-rw-r--   0 root         (0)     1003    58843 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/io.py
--rw-rw-r--   0 root         (0)     1003     7223 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/model.py
--rw-rw-r--   0 root         (0)     1003     7722 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/model_evaluation.py
--rw-rw-r--   0 root         (0)     1003    13014 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/operations.py
--rw-rw-r--   0 root         (0)     1003    11351 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/prediction_service.py
--rw-rw-r--   0 root         (0)     1003     1173 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/ranges.py
--rw-rw-r--   0 root         (0)     1003     1899 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/regression.py
--rw-rw-r--   0 root         (0)     1003    25402 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/service.py
--rw-rw-r--   0 root         (0)     1003     3613 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/table_spec.py
--rw-rw-r--   0 root         (0)     1003    17334 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/tables.py
--rw-rw-r--   0 root         (0)     1003     1636 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/temporal.py
--rw-rw-r--   0 root         (0)     1003     3380 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text.py
--rw-rw-r--   0 root         (0)     1003     3751 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text_extraction.py
--rw-rw-r--   0 root         (0)     1003     1742 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text_segment.py
--rw-rw-r--   0 root         (0)     1003     4524 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text_sentiment.py
--rw-rw-r--   0 root         (0)     1003     3340 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/translation.py
--rw-rw-r--   0 root         (0)     1003     1506 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/video.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/
--rw-r--r--   0 root         (0)     1003     4642 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5719 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      330 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:28:05.000000 google-cloud-automl-2.8.3/google_cloud_automl.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/scripts/
--rw-rw-r--   0 root         (0)     1003     7032 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/scripts/fixup_automl_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     7464 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/scripts/fixup_automl_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:28:05.973733 google-cloud-automl-2.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2769 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.945741 google-cloud-automl-2.8.3/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.945741 google-cloud-automl-2.8.3/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/tests/system/gapic/v1beta1/
--rw-rw-r--   0 root         (0)     1003    11353 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/system/gapic/v1beta1/test_system_tables_client_v1.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.969734 google-cloud-automl-2.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.973733 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   231199 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/test_auto_ml.py
--rw-rw-r--   0 root         (0)     1003    73071 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/test_prediction_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:05.973733 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   297732 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/test_auto_ml.py
--rw-rw-r--   0 root         (0)     1003    73205 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/test_prediction_service.py
--rw-rw-r--   0 root         (0)     1003     6861 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/test_gcs_client_v1beta1.py
--rw-rw-r--   0 root         (0)     1003    70421 2022-10-10 16:24:44.000000 google-cloud-automl-2.8.3/tests/unit/test_tables_client_v1beta1.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.805445 google-cloud-automl-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4650 2022-12-15 22:35:34.805445 google-cloud-automl-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3718 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      748 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.777438 google-cloud-automl-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/google/cloud/automl/
+-rw-rw-r--   0 root         (0)     1003     9705 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/google/cloud/automl_v1/
+-rw-rw-r--   0 root         (0)     1003     7737 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5626 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.785440 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/
+-rw-rw-r--   0 root         (0)     1003      737 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003   102820 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112979 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/client.py
+-rw-rw-r--   0 root         (0)     1003    15773 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.785440 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17401 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33839 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34522 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.785440 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/
+-rw-rw-r--   0 root         (0)     1003      781 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29385 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    38461 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.785440 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6749 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15880 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16178 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.789441 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5901 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4666 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/annotation_payload.py
+-rw-rw-r--   0 root         (0)     1003     1768 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/annotation_spec.py
+-rw-rw-r--   0 root         (0)     1003    11552 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/classification.py
+-rw-rw-r--   0 root         (0)     1003     9164 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/data_items.py
+-rw-rw-r--   0 root         (0)     1003     6768 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003     5414 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/detection.py
+-rw-rw-r--   0 root         (0)     1003     2166 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    13525 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/image.py
+-rw-rw-r--   0 root         (0)     1003    60862 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/io.py
+-rw-rw-r--   0 root         (0)     1003     7243 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/model.py
+-rw-rw-r--   0 root         (0)     1003     7003 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/model_evaluation.py
+-rw-rw-r--   0 root         (0)     1003    11008 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/operations.py
+-rw-rw-r--   0 root         (0)     1003    11570 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/prediction_service.py
+-rw-rw-r--   0 root         (0)     1003    18233 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3078 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text.py
+-rw-rw-r--   0 root         (0)     1003     3917 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_extraction.py
+-rw-rw-r--   0 root         (0)     1003     1804 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_segment.py
+-rw-rw-r--   0 root         (0)     1003     4470 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_sentiment.py
+-rw-rw-r--   0 root         (0)     1003     3442 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1/types/translation.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.789441 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/
+-rw-rw-r--   0 root         (0)     1003    10889 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7190 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.789441 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.789441 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/
+-rw-rw-r--   0 root         (0)     1003      737 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/__init__.py
+-rw-rw-r--   0 root         (0)     1003   131093 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/async_client.py
+-rw-rw-r--   0 root         (0)     1003   142635 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/client.py
+-rw-rw-r--   0 root         (0)     1003    26054 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.793442 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/
+-rw-rw-r--   0 root         (0)     1003     1122 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21566 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41516 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    42386 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.793442 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/
+-rw-rw-r--   0 root         (0)     1003      781 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28849 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37925 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.793442 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6759 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15456 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15754 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.793442 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/
+-rw-rw-r--   0 root         (0)     1003        0 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5631 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/gcs_client.py
+-rw-rw-r--   0 root         (0)     1003   130534 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/tables_client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     8243 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6097 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/annotation_payload.py
+-rw-rw-r--   0 root         (0)     1003     1774 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/annotation_spec.py
+-rw-rw-r--   0 root         (0)     1003    14426 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/classification.py
+-rw-rw-r--   0 root         (0)     1003     4070 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/column_spec.py
+-rw-rw-r--   0 root         (0)     1003    11471 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_items.py
+-rw-rw-r--   0 root         (0)     1003    11005 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_stats.py
+-rw-rw-r--   0 root         (0)     1003     4769 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_types.py
+-rw-rw-r--   0 root         (0)     1003     7725 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003     9311 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/detection.py
+-rw-rw-r--   0 root         (0)     1003     2176 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    12538 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/image.py
+-rw-rw-r--   0 root         (0)     1003    59231 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/io.py
+-rw-rw-r--   0 root         (0)     1003     7869 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/model.py
+-rw-rw-r--   0 root         (0)     1003     8214 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/model_evaluation.py
+-rw-rw-r--   0 root         (0)     1003    13658 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/operations.py
+-rw-rw-r--   0 root         (0)     1003    11732 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/prediction_service.py
+-rw-rw-r--   0 root         (0)     1003     1239 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/ranges.py
+-rw-rw-r--   0 root         (0)     1003     1986 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/regression.py
+-rw-rw-r--   0 root         (0)     1003    26420 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3735 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/table_spec.py
+-rw-rw-r--   0 root         (0)     1003    17818 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/tables.py
+-rw-rw-r--   0 root         (0)     1003     1734 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/temporal.py
+-rw-rw-r--   0 root         (0)     1003     3512 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text.py
+-rw-rw-r--   0 root         (0)     1003     3937 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_extraction.py
+-rw-rw-r--   0 root         (0)     1003     1809 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_segment.py
+-rw-rw-r--   0 root         (0)     1003     4755 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_sentiment.py
+-rw-rw-r--   0 root         (0)     1003     3455 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/translation.py
+-rw-rw-r--   0 root         (0)     1003     1558 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/video.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/
+-rw-r--r--   0 root         (0)     1003     4650 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5841 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      355 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-15 22:35:34.000000 google-cloud-automl-2.9.0/google_cloud_automl.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     7032 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/scripts/fixup_automl_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     7464 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/scripts/fixup_automl_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-15 22:35:34.805445 google-cloud-automl-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3144 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.781439 google-cloud-automl-2.9.0/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/tests/system/gapic/v1beta1/
+-rw-rw-r--   0 root         (0)     1003    11353 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/system/gapic/v1beta1/test_system_tables_client_v1.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.801444 google-cloud-automl-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.805445 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   231253 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/test_auto_ml.py
+-rw-rw-r--   0 root         (0)     1003    73071 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/test_prediction_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-15 22:35:34.805445 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   297786 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/test_auto_ml.py
+-rw-rw-r--   0 root         (0)     1003    73205 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/test_prediction_service.py
+-rw-rw-r--   0 root         (0)     1003     6861 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/test_gcs_client_v1beta1.py
+-rw-rw-r--   0 root         (0)     1003    70421 2022-12-15 22:31:58.000000 google-cloud-automl-2.9.0/tests/unit/test_tables_client_v1beta1.py
```

### Comparing `google-cloud-automl-2.8.3/LICENSE` & `google-cloud-automl-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/MANIFEST.in` & `google-cloud-automl-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/PKG-INFO` & `google-cloud-automl-2.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: google-cloud-automl
-Version: 2.8.3
-Summary: Cloud AutoML API client library
+Version: 2.9.0
+Summary: Google Cloud Automl API client library
 Home-page: https://github.com/googleapis/python-automl
 Author: Google LLC
-Author-email: googleapis-packages@oogle.com
+Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-cloud-automl-2.8.3/README.rst` & `google-cloud-automl-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/__init__.py` & `google-cloud-automl-2.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.automl import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.automl_v1.services.auto_ml.client import AutoMlClient
 from google.cloud.automl_v1.services.auto_ml.async_client import AutoMlAsyncClient
 from google.cloud.automl_v1.services.prediction_service.client import (
     PredictionServiceClient,
 )
 from google.cloud.automl_v1.services.prediction_service.async_client import (
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.automl import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.auto_ml import AutoMlClient
 from .services.auto_ml import AutoMlAsyncClient
 from .services.prediction_service import PredictionServiceClient
 from .services.prediction_service import PredictionServiceAsyncClient
 
 from .types.annotation_payload import AnnotationPayload
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/gapic_metadata.json` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/async_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -185,17 +196,17 @@
     get_transport_class = functools.partial(
         type(AutoMlClient).get_transport_class, type(AutoMlClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, AutoMlTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto ml client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -231,20 +242,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def create_dataset(
         self,
-        request: Union[service.CreateDatasetRequest, dict] = None,
+        request: Optional[Union[service.CreateDatasetRequest, dict]] = None,
         *,
-        parent: str = None,
-        dataset: gca_dataset.Dataset = None,
+        parent: Optional[str] = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -271,21 +282,21 @@
                 )
 
                 # Make the request
                 operation = client.create_dataset(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.CreateDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.CreateDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.CreateDataset][google.cloud.automl.v1.AutoMl.CreateDataset].
             parent (:class:`str`):
                 Required. The resource name of the
                 project to create the dataset for.
 
                 This corresponds to the ``parent`` field
@@ -360,19 +371,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_dataset(
         self,
-        request: Union[service.GetDatasetRequest, dict] = None,
+        request: Optional[Union[service.GetDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
         r"""Gets a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -396,15 +407,15 @@
                 # Make the request
                 response = await client.get_dataset(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.GetDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.GetDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetDataset][google.cloud.automl.v1.AutoMl.GetDataset].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset to retrieve.
 
                 This corresponds to the ``name`` field
@@ -474,19 +485,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_datasets(
         self,
-        request: Union[service.ListDatasetsRequest, dict] = None,
+        request: Optional[Union[service.ListDatasetsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsAsyncPager:
         r"""Lists datasets in a project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -511,15 +522,15 @@
                 page_result = client.list_datasets(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ListDatasetsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ListDatasetsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListDatasets][google.cloud.automl.v1.AutoMl.ListDatasets].
             parent (:class:`str`):
                 Required. The resource name of the
                 project from which to list datasets.
 
                 This corresponds to the ``parent`` field
@@ -599,20 +610,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_dataset(
         self,
-        request: Union[service.UpdateDatasetRequest, dict] = None,
+        request: Optional[Union[service.UpdateDatasetRequest, dict]] = None,
         *,
-        dataset: gca_dataset.Dataset = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Updates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -640,15 +651,15 @@
                 # Make the request
                 response = await client.update_dataset(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.UpdateDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.UpdateDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UpdateDataset][google.cloud.automl.v1.AutoMl.UpdateDataset]
             dataset (:class:`google.cloud.automl_v1.types.Dataset`):
                 Required. The dataset which replaces
                 the resource on the server.
 
                 This corresponds to the ``dataset`` field
@@ -719,19 +730,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_dataset(
         self,
-        request: Union[service.DeleteDatasetRequest, dict] = None,
+        request: Optional[Union[service.DeleteDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a dataset and all of its contents. Returns empty
         response in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
@@ -757,21 +768,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_dataset(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.DeleteDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.DeleteDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeleteDataset][google.cloud.automl.v1.AutoMl.DeleteDataset].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset to delete.
 
                 This corresponds to the ``name`` field
@@ -857,20 +868,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def import_data(
         self,
-        request: Union[service.ImportDataRequest, dict] = None,
+        request: Optional[Union[service.ImportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.InputConfig = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.InputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Imports data into a dataset. For Tables this method can only be
         called on an empty Dataset.
 
         For Tables:
 
@@ -905,21 +916,21 @@
                 )
 
                 # Make the request
                 operation = client.import_data(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ImportDataRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ImportDataRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ImportData][google.cloud.automl.v1.AutoMl.ImportData].
             name (:class:`str`):
                 Required. Dataset name. Dataset must
                 already exist. All imported annotations
                 and examples will be added.
 
@@ -1006,20 +1017,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def export_data(
         self,
-        request: Union[service.ExportDataRequest, dict] = None,
+        request: Optional[Union[service.ExportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.OutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.OutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Exports dataset's data to the provided output location. Returns
         an empty response in the
         [response][google.longrunning.Operation.response] field when it
         completes.
 
@@ -1048,21 +1059,21 @@
                 )
 
                 # Make the request
                 operation = client.export_data(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ExportDataRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ExportDataRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ExportData][google.cloud.automl.v1.AutoMl.ExportData].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset.
 
                 This corresponds to the ``name`` field
@@ -1147,19 +1158,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_annotation_spec(
         self,
-        request: Union[service.GetAnnotationSpecRequest, dict] = None,
+        request: Optional[Union[service.GetAnnotationSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> annotation_spec.AnnotationSpec:
         r"""Gets an annotation spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1183,15 +1194,15 @@
                 # Make the request
                 response = await client.get_annotation_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.GetAnnotationSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.GetAnnotationSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetAnnotationSpec][google.cloud.automl.v1.AutoMl.GetAnnotationSpec].
             name (:class:`str`):
                 Required. The resource name of the
                 annotation spec to retrieve.
 
                 This corresponds to the ``name`` field
@@ -1257,20 +1268,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_model(
         self,
-        request: Union[service.CreateModelRequest, dict] = None,
+        request: Optional[Union[service.CreateModelRequest, dict]] = None,
         *,
-        parent: str = None,
-        model: gca_model.Model = None,
+        parent: Optional[str] = None,
+        model: Optional[gca_model.Model] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a model. Returns a Model in the
         [response][google.longrunning.Operation.response] field when it
         completes. When you create a model, several model evaluations
         are created for it: a global evaluation, and one evaluation for
         each annotation spec.
@@ -1296,21 +1307,21 @@
                 )
 
                 # Make the request
                 operation = client.create_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.CreateModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.CreateModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.CreateModel][google.cloud.automl.v1.AutoMl.CreateModel].
             parent (:class:`str`):
                 Required. Resource name of the parent
                 project where the model is being
                 created.
 
@@ -1387,19 +1398,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_model(
         self,
-        request: Union[service.GetModelRequest, dict] = None,
+        request: Optional[Union[service.GetModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model.Model:
         r"""Gets a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1423,15 +1434,15 @@
                 # Make the request
                 response = await client.get_model(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.GetModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.GetModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetModel][google.cloud.automl.v1.AutoMl.GetModel].
             name (:class:`str`):
                 Required. Resource name of the model.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1497,19 +1508,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_models(
         self,
-        request: Union[service.ListModelsRequest, dict] = None,
+        request: Optional[Union[service.ListModelsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelsAsyncPager:
         r"""Lists models.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1534,15 +1545,15 @@
                 page_result = client.list_models(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ListModelsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ListModelsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListModels][google.cloud.automl.v1.AutoMl.ListModels].
             parent (:class:`str`):
                 Required. Resource name of the
                 project, from which to list the models.
 
                 This corresponds to the ``parent`` field
@@ -1622,19 +1633,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_model(
         self,
-        request: Union[service.DeleteModelRequest, dict] = None,
+        request: Optional[Union[service.DeleteModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a model. Returns ``google.protobuf.Empty`` in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
 
@@ -1659,21 +1670,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.DeleteModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.DeleteModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeleteModel][google.cloud.automl.v1.AutoMl.DeleteModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 being deleted.
 
                 This corresponds to the ``name`` field
@@ -1759,20 +1770,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_model(
         self,
-        request: Union[service.UpdateModelRequest, dict] = None,
+        request: Optional[Union[service.UpdateModelRequest, dict]] = None,
         *,
-        model: gca_model.Model = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        model: Optional[gca_model.Model] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_model.Model:
         r"""Updates a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1795,15 +1806,15 @@
                 # Make the request
                 response = await client.update_model(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.UpdateModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.UpdateModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UpdateModel][google.cloud.automl.v1.AutoMl.UpdateModel]
             model (:class:`google.cloud.automl_v1.types.Model`):
                 Required. The model which replaces
                 the resource on the server.
 
                 This corresponds to the ``model`` field
@@ -1872,19 +1883,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def deploy_model(
         self,
-        request: Union[service.DeployModelRequest, dict] = None,
+        request: Optional[Union[service.DeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deploys a model. If a model is already deployed, deploying it
         with the same parameters has no effect. Deploying with different
         parametrs (as e.g. changing
         [node_number][google.cloud.automl.v1p1beta.ImageObjectDetectionModelDeploymentMetadata.node_number])
         will reset the deployment state without pausing the model's
@@ -1919,21 +1930,21 @@
                 )
 
                 # Make the request
                 operation = client.deploy_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.DeployModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.DeployModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeployModel][google.cloud.automl.v1.AutoMl.DeployModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 to deploy.
 
                 This corresponds to the ``name`` field
@@ -2009,19 +2020,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def undeploy_model(
         self,
-        request: Union[service.UndeployModelRequest, dict] = None,
+        request: Optional[Union[service.UndeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Undeploys a model. If the model is not deployed this method has
         no effect.
 
         Only applicable for Text Classification, Image Object Detection
         and Tables; all other domains manage deployment automatically.
@@ -2051,21 +2062,21 @@
                 )
 
                 # Make the request
                 operation = client.undeploy_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.UndeployModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.UndeployModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UndeployModel][google.cloud.automl.v1.AutoMl.UndeployModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 to undeploy.
 
                 This corresponds to the ``name`` field
@@ -2141,20 +2152,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def export_model(
         self,
-        request: Union[service.ExportModelRequest, dict] = None,
+        request: Optional[Union[service.ExportModelRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ModelExportOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ModelExportOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Exports a trained, "export-able", model to a user specified
         Google Cloud Storage location. A model is considered export-able
         if and only if it has an export format defined for it in
         [ModelExportOutputConfig][google.cloud.automl.v1.ModelExportOutputConfig].
 
@@ -2187,21 +2198,21 @@
                 )
 
                 # Make the request
                 operation = client.export_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ExportModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ExportModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ExportModel][google.cloud.automl.v1.AutoMl.ExportModel].
                 Models need to be enabled for exporting, otherwise an
                 error code will be returned.
             name (:class:`str`):
                 Required. The resource name of the
                 model to export.
@@ -2288,19 +2299,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_model_evaluation(
         self,
-        request: Union[service.GetModelEvaluationRequest, dict] = None,
+        request: Optional[Union[service.GetModelEvaluationRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model_evaluation.ModelEvaluation:
         r"""Gets a model evaluation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2324,15 +2335,15 @@
                 # Make the request
                 response = await client.get_model_evaluation(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.GetModelEvaluationRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.GetModelEvaluationRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetModelEvaluation][google.cloud.automl.v1.AutoMl.GetModelEvaluation].
             name (:class:`str`):
                 Required. Resource name for the model
                 evaluation.
 
                 This corresponds to the ``name`` field
@@ -2398,20 +2409,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_model_evaluations(
         self,
-        request: Union[service.ListModelEvaluationsRequest, dict] = None,
+        request: Optional[Union[service.ListModelEvaluationsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelEvaluationsAsyncPager:
         r"""Lists model evaluations.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2437,15 +2448,15 @@
                 page_result = client.list_model_evaluations(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.ListModelEvaluationsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.ListModelEvaluationsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListModelEvaluations][google.cloud.automl.v1.AutoMl.ListModelEvaluations].
             parent (:class:`str`):
                 Required. Resource name of the model
                 to list the model evaluations for. If
                 modelId is set as "-", this will list
                 model evaluations from across all models
@@ -2553,18 +2564,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoMlAsyncClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -71,15 +83,15 @@
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[AutoMlTransport]]
     _transport_registry["grpc"] = AutoMlGrpcTransport
     _transport_registry["grpc_asyncio"] = AutoMlGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[AutoMlTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -431,30 +443,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, AutoMlTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, AutoMlTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto ml client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, AutoMlTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -476,14 +488,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -528,20 +541,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def create_dataset(
         self,
-        request: Union[service.CreateDatasetRequest, dict] = None,
+        request: Optional[Union[service.CreateDatasetRequest, dict]] = None,
         *,
-        parent: str = None,
-        dataset: gca_dataset.Dataset = None,
+        parent: Optional[str] = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -657,19 +670,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_dataset(
         self,
-        request: Union[service.GetDatasetRequest, dict] = None,
+        request: Optional[Union[service.GetDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
         r"""Gets a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -761,19 +774,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_datasets(
         self,
-        request: Union[service.ListDatasetsRequest, dict] = None,
+        request: Optional[Union[service.ListDatasetsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsPager:
         r"""Lists datasets in a project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -876,20 +889,20 @@
         )
 
         # Done; return the response.
         return response
 
     def update_dataset(
         self,
-        request: Union[service.UpdateDatasetRequest, dict] = None,
+        request: Optional[Union[service.UpdateDatasetRequest, dict]] = None,
         *,
-        dataset: gca_dataset.Dataset = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Updates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -996,19 +1009,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_dataset(
         self,
-        request: Union[service.DeleteDatasetRequest, dict] = None,
+        request: Optional[Union[service.DeleteDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a dataset and all of its contents. Returns empty
         response in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
@@ -1124,20 +1137,20 @@
         )
 
         # Done; return the response.
         return response
 
     def import_data(
         self,
-        request: Union[service.ImportDataRequest, dict] = None,
+        request: Optional[Union[service.ImportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.InputConfig = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.InputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Imports data into a dataset. For Tables this method can only be
         called on an empty Dataset.
 
         For Tables:
 
@@ -1273,20 +1286,20 @@
         )
 
         # Done; return the response.
         return response
 
     def export_data(
         self,
-        request: Union[service.ExportDataRequest, dict] = None,
+        request: Optional[Union[service.ExportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.OutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.OutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Exports dataset's data to the provided output location. Returns
         an empty response in the
         [response][google.longrunning.Operation.response] field when it
         completes.
 
@@ -1414,19 +1427,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_annotation_spec(
         self,
-        request: Union[service.GetAnnotationSpecRequest, dict] = None,
+        request: Optional[Union[service.GetAnnotationSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> annotation_spec.AnnotationSpec:
         r"""Gets an annotation spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1514,20 +1527,20 @@
         )
 
         # Done; return the response.
         return response
 
     def create_model(
         self,
-        request: Union[service.CreateModelRequest, dict] = None,
+        request: Optional[Union[service.CreateModelRequest, dict]] = None,
         *,
-        parent: str = None,
-        model: gca_model.Model = None,
+        parent: Optional[str] = None,
+        model: Optional[gca_model.Model] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a model. Returns a Model in the
         [response][google.longrunning.Operation.response] field when it
         completes. When you create a model, several model evaluations
         are created for it: a global evaluation, and one evaluation for
         each annotation spec.
@@ -1644,19 +1657,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_model(
         self,
-        request: Union[service.GetModelRequest, dict] = None,
+        request: Optional[Union[service.GetModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model.Model:
         r"""Gets a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1744,19 +1757,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_models(
         self,
-        request: Union[service.ListModelsRequest, dict] = None,
+        request: Optional[Union[service.ListModelsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelsPager:
         r"""Lists models.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1859,19 +1872,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_model(
         self,
-        request: Union[service.DeleteModelRequest, dict] = None,
+        request: Optional[Union[service.DeleteModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a model. Returns ``google.protobuf.Empty`` in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
 
@@ -1986,20 +1999,20 @@
         )
 
         # Done; return the response.
         return response
 
     def update_model(
         self,
-        request: Union[service.UpdateModelRequest, dict] = None,
+        request: Optional[Union[service.UpdateModelRequest, dict]] = None,
         *,
-        model: gca_model.Model = None,
-        update_mask: field_mask_pb2.FieldMask = None,
+        model: Optional[gca_model.Model] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_model.Model:
         r"""Updates a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2099,19 +2112,19 @@
         )
 
         # Done; return the response.
         return response
 
     def deploy_model(
         self,
-        request: Union[service.DeployModelRequest, dict] = None,
+        request: Optional[Union[service.DeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deploys a model. If a model is already deployed, deploying it
         with the same parameters has no effect. Deploying with different
         parametrs (as e.g. changing
         [node_number][google.cloud.automl.v1p1beta.ImageObjectDetectionModelDeploymentMetadata.node_number])
         will reset the deployment state without pausing the model's
@@ -2236,19 +2249,19 @@
         )
 
         # Done; return the response.
         return response
 
     def undeploy_model(
         self,
-        request: Union[service.UndeployModelRequest, dict] = None,
+        request: Optional[Union[service.UndeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Undeploys a model. If the model is not deployed this method has
         no effect.
 
         Only applicable for Text Classification, Image Object Detection
         and Tables; all other domains manage deployment automatically.
@@ -2368,20 +2381,20 @@
         )
 
         # Done; return the response.
         return response
 
     def export_model(
         self,
-        request: Union[service.ExportModelRequest, dict] = None,
+        request: Optional[Union[service.ExportModelRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ModelExportOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ModelExportOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Exports a trained, "export-able", model to a user specified
         Google Cloud Storage location. A model is considered export-able
         if and only if it has an export format defined for it in
         [ModelExportOutputConfig][google.cloud.automl.v1.ModelExportOutputConfig].
 
@@ -2515,19 +2528,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_model_evaluation(
         self,
-        request: Union[service.GetModelEvaluationRequest, dict] = None,
+        request: Optional[Union[service.GetModelEvaluationRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model_evaluation.ModelEvaluation:
         r"""Gets a model evaluation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2615,20 +2628,20 @@
         )
 
         # Done; return the response.
         return response
 
     def list_model_evaluations(
         self,
-        request: Union[service.ListModelEvaluationsRequest, dict] = None,
+        request: Optional[Union[service.ListModelEvaluationsRequest, dict]] = None,
         *,
-        parent: str = None,
-        filter: str = None,
+        parent: Optional[str] = None,
+        filter: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelEvaluationsPager:
         r"""Lists model evaluations.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2767,18 +2780,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoMlClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/pagers.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/base.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
@@ -31,36 +32,31 @@
 from google.cloud.automl_v1.types import dataset as gca_dataset
 from google.cloud.automl_v1.types import model
 from google.cloud.automl_v1.types import model as gca_model
 from google.cloud.automl_v1.types import model_evaluation
 from google.cloud.automl_v1.types import service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class AutoMlTransport(abc.ABC):
     """Abstract transport class for AutoMl."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "automl.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/grpc.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -200,16 +200,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/auto_ml/transports/grpc_asyncio.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/auto_ml/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -110,23 +110,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/async_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -163,17 +174,17 @@
     get_transport_class = functools.partial(
         type(PredictionServiceClient).get_transport_class, type(PredictionServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, PredictionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -209,21 +220,21 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        payload: data_items.ExamplePayload = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        payload: Optional[data_items.ExamplePayload] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_service.PredictResponse:
         r"""Perform an online prediction. The prediction result is directly
         returned in the response. Available for following ML scenarios,
         and their expected request payloads:
 
         AutoML Vision Classification
@@ -287,15 +298,15 @@
                 # Make the request
                 response = await client.predict(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.PredictRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.PredictRequest, dict]]):
                 The request object. Request message for
                 [PredictionService.Predict][google.cloud.automl.v1.PredictionService.Predict].
             name (:class:`str`):
                 Required. Name of the model requested
                 to serve the prediction.
 
                 This corresponds to the ``name`` field
@@ -306,15 +317,15 @@
                 prediction on. The payload must match
                 the problem type that the model was
                 trained to solve.
 
                 This corresponds to the ``payload`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (:class:`Mapping[str, str]`):
+            params (:class:`MutableMapping[str, str]`):
                 Additional domain-specific parameters, any string must
                 be up to 25000 characters long.
 
                 AutoML Vision Classification
 
                 ``score_threshold`` : (float) A value from 0.0 to 1.0.
                 When the model makes predictions for an image, it will
@@ -401,22 +412,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_predict(
         self,
-        request: Union[prediction_service.BatchPredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.BatchPredictRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.BatchPredictInputConfig = None,
-        output_config: io.BatchPredictOutputConfig = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.BatchPredictInputConfig] = None,
+        output_config: Optional[io.BatchPredictOutputConfig] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Perform a batch prediction. Unlike the online
         [Predict][google.cloud.automl.v1.PredictionService.Predict],
         batch prediction result won't be immediately available in the
         response. Instead, a long running operation object is returned.
         User can poll the operation result via
@@ -465,21 +476,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_predict(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1.types.BatchPredictRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1.types.BatchPredictRequest, dict]]):
                 The request object. Request message for
                 [PredictionService.BatchPredict][google.cloud.automl.v1.PredictionService.BatchPredict].
             name (:class:`str`):
                 Required. Name of the model requested
                 to serve the batch prediction.
 
                 This corresponds to the ``name`` field
@@ -496,15 +507,15 @@
                 Required. The Configuration
                 specifying where output predictions
                 should be written.
 
                 This corresponds to the ``output_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (:class:`Mapping[str, str]`):
+            params (:class:`MutableMapping[str, str]`):
                 Additional domain-specific parameters for the
                 predictions, any string must be up to 25000 characters
                 long.
 
                 AutoML Natural Language Classification
 
                 ``score_threshold`` : (float) A value from 0.0 to 1.0.
@@ -665,18 +676,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceAsyncClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -58,15 +70,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[PredictionServiceTransport]]
     _transport_registry["grpc"] = PredictionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = PredictionServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[PredictionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -337,30 +349,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, PredictionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, PredictionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, PredictionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -382,14 +394,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -434,21 +447,21 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        payload: data_items.ExamplePayload = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        payload: Optional[data_items.ExamplePayload] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_service.PredictResponse:
         r"""Perform an online prediction. The prediction result is directly
         returned in the response. Available for following ML scenarios,
         and their expected request payloads:
 
         AutoML Vision Classification
@@ -531,15 +544,15 @@
                 prediction on. The payload must match
                 the problem type that the model was
                 trained to solve.
 
                 This corresponds to the ``payload`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (Mapping[str, str]):
+            params (MutableMapping[str, str]):
                 Additional domain-specific parameters, any string must
                 be up to 25000 characters long.
 
                 AutoML Vision Classification
 
                 ``score_threshold`` : (float) A value from 0.0 to 1.0.
                 When the model makes predictions for an image, it will
@@ -625,22 +638,22 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_predict(
         self,
-        request: Union[prediction_service.BatchPredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.BatchPredictRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.BatchPredictInputConfig = None,
-        output_config: io.BatchPredictOutputConfig = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.BatchPredictInputConfig] = None,
+        output_config: Optional[io.BatchPredictOutputConfig] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Perform a batch prediction. Unlike the online
         [Predict][google.cloud.automl.v1.PredictionService.Predict],
         batch prediction result won't be immediately available in the
         response. Instead, a long running operation object is returned.
         User can poll the operation result via
@@ -720,15 +733,15 @@
                 Required. The Configuration
                 specifying where output predictions
                 should be written.
 
                 This corresponds to the ``output_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (Mapping[str, str]):
+            params (MutableMapping[str, str]):
                 Additional domain-specific parameters for the
                 predictions, any string must be up to 25000 characters
                 long.
 
                 AutoML Natural Language Classification
 
                 ``score_threshold`` : (float) A value from 0.0 to 1.0.
@@ -895,18 +908,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/base.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,50 +11,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.automl_v1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.automl_v1.types import prediction_service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class PredictionServiceTransport(abc.ABC):
     """Abstract transport class for PredictionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "automl.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/grpc.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -183,16 +183,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/services/prediction_service/transports/grpc_asyncio.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/services/prediction_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -93,23 +93,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/annotation_payload.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/annotation_payload.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import classification as gca_classification
 from google.cloud.automl_v1.types import detection
 from google.cloud.automl_v1.types import text_extraction as gca_text_extraction
 from google.cloud.automl_v1.types import text_sentiment as gca_text_sentiment
 from google.cloud.automl_v1.types import translation as gca_translation
@@ -75,48 +77,48 @@
             when the model was trained. Because this field returns a
             value at model training time, for different models trained
             using the same dataset, the returned value could be
             different as model owner could update the ``display_name``
             between any two model training.
     """
 
-    translation = proto.Field(
+    translation: gca_translation.TranslationAnnotation = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="detail",
         message=gca_translation.TranslationAnnotation,
     )
-    classification = proto.Field(
+    classification: gca_classification.ClassificationAnnotation = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="detail",
         message=gca_classification.ClassificationAnnotation,
     )
-    image_object_detection = proto.Field(
+    image_object_detection: detection.ImageObjectDetectionAnnotation = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="detail",
         message=detection.ImageObjectDetectionAnnotation,
     )
-    text_extraction = proto.Field(
+    text_extraction: gca_text_extraction.TextExtractionAnnotation = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="detail",
         message=gca_text_extraction.TextExtractionAnnotation,
     )
-    text_sentiment = proto.Field(
+    text_sentiment: gca_text_sentiment.TextSentimentAnnotation = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="detail",
         message=gca_text_sentiment.TextSentimentAnnotation,
     )
-    annotation_spec_id = proto.Field(
+    annotation_spec_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/annotation_spec.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/ranges.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,49 +9,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.automl.v1",
+    package="google.cloud.automl.v1beta1",
     manifest={
-        "AnnotationSpec",
+        "DoubleRange",
     },
 )
 
 
-class AnnotationSpec(proto.Message):
-    r"""A definition of an annotation spec.
+class DoubleRange(proto.Message):
+    r"""A range between two double numbers.
 
     Attributes:
-        name (str):
-            Output only. Resource name of the annotation spec. Form:
-            'projects/{project_id}/locations/{location_id}/datasets/{dataset_id}/annotationSpecs/{annotation_spec_id}'
-        display_name (str):
-            Required. The name of the annotation spec to show in the
-            interface. The name can be up to 32 characters long and must
-            match the regexp ``[a-zA-Z0-9_]+``.
-        example_count (int):
-            Output only. The number of examples in the
-            parent dataset labeled by the annotation spec.
+        start (float):
+            Start of the range, inclusive.
+        end (float):
+            End of the range, exclusive.
     """
 
-    name = proto.Field(
-        proto.STRING,
+    start: float = proto.Field(
+        proto.DOUBLE,
         number=1,
     )
-    display_name = proto.Field(
-        proto.STRING,
+    end: float = proto.Field(
+        proto.DOUBLE,
         number=2,
     )
-    example_count = proto.Field(
-        proto.INT32,
-        number=9,
-    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/classification.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
     manifest={
         "ClassificationType",
@@ -43,15 +45,15 @@
             confidence that the annotation is positive. If a
             user approves an annotation as negative or
             positive, the score value remains unchanged. If
             a user creates an annotation, the score is 0 for
             negative or 1 for positive.
     """
 
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
 
 
 class ClassificationEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for classification problems. Note: For
@@ -65,30 +67,30 @@
             evaluation.
         au_roc (float):
             Output only. The Area Under Receiver
             Operating Characteristic curve metric.
             Micro-averaged for the overall evaluation.
         log_loss (float):
             Output only. The Log Loss metric.
-        confidence_metrics_entry (Sequence[google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfidenceMetricsEntry]):
+        confidence_metrics_entry (MutableSequence[google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfidenceMetricsEntry]):
             Output only. Metrics for each confidence_threshold in
             0.00,0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 and
             position_threshold = INT32_MAX_VALUE. ROC and
             precision-recall curves, and other aggregated metrics are
             derived from them. The confidence metrics entries may also
             be supplied for additional values of position_threshold, but
             from these no aggregated metrics are computed.
         confusion_matrix (google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
             Output only. Confusion matrix of the
             evaluation. Only set for MULTICLASS
             classification problems where number of labels
             is no more than 10.
             Only set for model level evaluation, not for
             evaluation per label.
-        annotation_spec_id (Sequence[str]):
+        annotation_spec_id (MutableSequence[str]):
             Output only. The annotation spec ids used for
             this evaluation.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
         r"""Metrics for a single confidence threshold.
 
@@ -146,152 +148,156 @@
                 label.
             true_negative_count (int):
                 Output only. The number of labels that were
                 not created by the model, but if they would,
                 they would not match a ground truth label.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        position_threshold = proto.Field(
+        position_threshold: int = proto.Field(
             proto.INT32,
             number=14,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        false_positive_rate = proto.Field(
+        false_positive_rate: float = proto.Field(
             proto.FLOAT,
             number=8,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
-        recall_at1 = proto.Field(
+        recall_at1: float = proto.Field(
             proto.FLOAT,
             number=5,
         )
-        precision_at1 = proto.Field(
+        precision_at1: float = proto.Field(
             proto.FLOAT,
             number=6,
         )
-        false_positive_rate_at1 = proto.Field(
+        false_positive_rate_at1: float = proto.Field(
             proto.FLOAT,
             number=9,
         )
-        f1_score_at1 = proto.Field(
+        f1_score_at1: float = proto.Field(
             proto.FLOAT,
             number=7,
         )
-        true_positive_count = proto.Field(
+        true_positive_count: int = proto.Field(
             proto.INT64,
             number=10,
         )
-        false_positive_count = proto.Field(
+        false_positive_count: int = proto.Field(
             proto.INT64,
             number=11,
         )
-        false_negative_count = proto.Field(
+        false_negative_count: int = proto.Field(
             proto.INT64,
             number=12,
         )
-        true_negative_count = proto.Field(
+        true_negative_count: int = proto.Field(
             proto.INT64,
             number=13,
         )
 
     class ConfusionMatrix(proto.Message):
         r"""Confusion matrix of the model running the classification.
 
         Attributes:
-            annotation_spec_id (Sequence[str]):
+            annotation_spec_id (MutableSequence[str]):
                 Output only. IDs of the annotation specs used in the
                 confusion matrix. For Tables CLASSIFICATION
                 [prediction_type][google.cloud.automl.v1p1beta.TablesModelMetadata.prediction_type]
                 only list of [annotation_spec_display_name-s][] is
                 populated.
-            display_name (Sequence[str]):
+            display_name (MutableSequence[str]):
                 Output only. Display name of the annotation specs used in
                 the confusion matrix, as they were at the moment of the
                 evaluation. For Tables CLASSIFICATION
                 [prediction_type-s][google.cloud.automl.v1p1beta.TablesModelMetadata.prediction_type],
                 distinct values of the target column at the moment of the
                 model evaluation are populated here.
-            row (Sequence[google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfusionMatrix.Row]):
+            row (MutableSequence[google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfusionMatrix.Row]):
                 Output only. Rows in the confusion matrix. The number of
                 rows is equal to the size of ``annotation_spec_id``.
                 ``row[i].example_count[j]`` is the number of examples that
                 have ground truth of the ``annotation_spec_id[i]`` and are
                 predicted as ``annotation_spec_id[j]`` by the model being
                 evaluated.
         """
 
         class Row(proto.Message):
             r"""Output only. A row in the confusion matrix.
 
             Attributes:
-                example_count (Sequence[int]):
+                example_count (MutableSequence[int]):
                     Output only. Value of the specific cell in the confusion
                     matrix. The number of values each row has (i.e. the length
                     of the row) is equal to the length of the
                     ``annotation_spec_id`` field or, if that one is not
                     populated, length of the
                     [display_name][google.cloud.automl.v1.ClassificationEvaluationMetrics.ConfusionMatrix.display_name]
                     field.
             """
 
-            example_count = proto.RepeatedField(
+            example_count: MutableSequence[int] = proto.RepeatedField(
                 proto.INT32,
                 number=1,
             )
 
-        annotation_spec_id = proto.RepeatedField(
+        annotation_spec_id: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
-        display_name = proto.RepeatedField(
+        display_name: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=3,
         )
-        row = proto.RepeatedField(
+        row: MutableSequence[
+            "ClassificationEvaluationMetrics.ConfusionMatrix.Row"
+        ] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message="ClassificationEvaluationMetrics.ConfusionMatrix.Row",
         )
 
-    au_prc = proto.Field(
+    au_prc: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    au_roc = proto.Field(
+    au_roc: float = proto.Field(
         proto.FLOAT,
         number=6,
     )
-    log_loss = proto.Field(
+    log_loss: float = proto.Field(
         proto.FLOAT,
         number=7,
     )
-    confidence_metrics_entry = proto.RepeatedField(
+    confidence_metrics_entry: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ConfidenceMetricsEntry,
     )
-    confusion_matrix = proto.Field(
+    confusion_matrix: ConfusionMatrix = proto.Field(
         proto.MESSAGE,
         number=4,
         message=ConfusionMatrix,
     )
-    annotation_spec_id = proto.RepeatedField(
+    annotation_spec_id: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=5,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/data_items.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/data_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import geometry
 from google.cloud.automl_v1.types import io
 from google.cloud.automl_v1.types import text_segment as gca_text_segment
 
 
@@ -46,20 +48,20 @@
             representation, whereas JSON representations use base64.
 
             This field is a member of `oneof`_ ``data``.
         thumbnail_uri (str):
             Output only. HTTP URI to the thumbnail image.
     """
 
-    image_bytes = proto.Field(
+    image_bytes: bytes = proto.Field(
         proto.BYTES,
         number=1,
         oneof="data",
     )
-    thumbnail_uri = proto.Field(
+    thumbnail_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class TextSnippet(proto.Message):
     r"""A representation of a text snippet.
@@ -76,23 +78,23 @@
             determined from the type of the uploaded
             [content][google.cloud.automl.v1.TextSnippet.content].
         content_uri (str):
             Output only. HTTP URI where you can download
             the content.
     """
 
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    content_uri = proto.Field(
+    content_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class DocumentDimensions(proto.Message):
     r"""Message that describes dimension of a document.
@@ -111,39 +113,39 @@
     class DocumentDimensionUnit(proto.Enum):
         r"""Unit of the document dimension."""
         DOCUMENT_DIMENSION_UNIT_UNSPECIFIED = 0
         INCH = 1
         CENTIMETER = 2
         POINT = 3
 
-    unit = proto.Field(
+    unit: DocumentDimensionUnit = proto.Field(
         proto.ENUM,
         number=1,
         enum=DocumentDimensionUnit,
     )
-    width = proto.Field(
+    width: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    height = proto.Field(
+    height: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 class Document(proto.Message):
     r"""A structured text document e.g. a PDF.
 
     Attributes:
         input_config (google.cloud.automl_v1.types.DocumentInputConfig):
             An input config specifying the content of the
             document.
         document_text (google.cloud.automl_v1.types.TextSnippet):
             The plain text version of this document.
-        layout (Sequence[google.cloud.automl_v1.types.Document.Layout]):
+        layout (MutableSequence[google.cloud.automl_v1.types.Document.Layout]):
             Describes the layout of the document. Sorted by
             [page_number][].
         document_dimensions (google.cloud.automl_v1.types.DocumentDimensions):
             The dimensions of the page in the document.
         page_count (int):
             Number of pages in the document.
     """
@@ -188,55 +190,55 @@
             FORM_FIELD_NAME = 4
             FORM_FIELD_CONTENTS = 5
             TABLE = 6
             TABLE_HEADER = 7
             TABLE_ROW = 8
             TABLE_CELL = 9
 
-        text_segment = proto.Field(
+        text_segment: gca_text_segment.TextSegment = proto.Field(
             proto.MESSAGE,
             number=1,
             message=gca_text_segment.TextSegment,
         )
-        page_number = proto.Field(
+        page_number: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        bounding_poly = proto.Field(
+        bounding_poly: geometry.BoundingPoly = proto.Field(
             proto.MESSAGE,
             number=3,
             message=geometry.BoundingPoly,
         )
-        text_segment_type = proto.Field(
+        text_segment_type: "Document.Layout.TextSegmentType" = proto.Field(
             proto.ENUM,
             number=4,
             enum="Document.Layout.TextSegmentType",
         )
 
-    input_config = proto.Field(
+    input_config: io.DocumentInputConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=io.DocumentInputConfig,
     )
-    document_text = proto.Field(
+    document_text: "TextSnippet" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="TextSnippet",
     )
-    layout = proto.RepeatedField(
+    layout: MutableSequence[Layout] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=Layout,
     )
-    document_dimensions = proto.Field(
+    document_dimensions: "DocumentDimensions" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="DocumentDimensions",
     )
-    page_count = proto.Field(
+    page_count: int = proto.Field(
         proto.INT32,
         number=5,
     )
 
 
 class ExamplePayload(proto.Message):
     r"""Example data used for training or prediction.
@@ -259,27 +261,27 @@
             This field is a member of `oneof`_ ``payload``.
         document (google.cloud.automl_v1.types.Document):
             Example document.
 
             This field is a member of `oneof`_ ``payload``.
     """
 
-    image = proto.Field(
+    image: "Image" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="payload",
         message="Image",
     )
-    text_snippet = proto.Field(
+    text_snippet: "TextSnippet" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="payload",
         message="TextSnippet",
     )
-    document = proto.Field(
+    document: "Document" = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="payload",
         message="Document",
     )
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/dataset.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import image
 from google.cloud.automl_v1.types import text
 from google.cloud.automl_v1.types import translation
 from google.protobuf import timestamp_pb2  # type: ignore
 
@@ -88,89 +90,93 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Timestamp when this dataset was
             created.
         etag (str):
             Used to perform consistent read-modify-write
             updates. If not set, a blind "overwrite" update
             happens.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata to organize your dataset.
             Label keys and values can be no longer than 64
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
             keys must start with a letter.
             See https://goo.gl/xmQnxf for more information
             on and examples of labels.
     """
 
-    translation_dataset_metadata = proto.Field(
+    translation_dataset_metadata: translation.TranslationDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=23,
         oneof="dataset_metadata",
         message=translation.TranslationDatasetMetadata,
     )
-    image_classification_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=24,
-        oneof="dataset_metadata",
-        message=image.ImageClassificationDatasetMetadata,
-    )
-    text_classification_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=25,
-        oneof="dataset_metadata",
-        message=text.TextClassificationDatasetMetadata,
+    image_classification_dataset_metadata: image.ImageClassificationDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=24,
+            oneof="dataset_metadata",
+            message=image.ImageClassificationDatasetMetadata,
+        )
+    )
+    text_classification_dataset_metadata: text.TextClassificationDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=25,
+            oneof="dataset_metadata",
+            message=text.TextClassificationDatasetMetadata,
+        )
     )
-    image_object_detection_dataset_metadata = proto.Field(
+    image_object_detection_dataset_metadata: image.ImageObjectDetectionDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=26,
         oneof="dataset_metadata",
         message=image.ImageObjectDetectionDatasetMetadata,
     )
-    text_extraction_dataset_metadata = proto.Field(
+    text_extraction_dataset_metadata: text.TextExtractionDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=28,
         oneof="dataset_metadata",
         message=text.TextExtractionDatasetMetadata,
     )
-    text_sentiment_dataset_metadata = proto.Field(
+    text_sentiment_dataset_metadata: text.TextSentimentDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=30,
         oneof="dataset_metadata",
         message=text.TextSentimentDatasetMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    example_count = proto.Field(
+    example_count: int = proto.Field(
         proto.INT32,
         number=21,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=14,
         message=timestamp_pb2.Timestamp,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=17,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=39,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/detection.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import geometry
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
@@ -37,20 +39,20 @@
             object location.
         score (float):
             Output only. The confidence that this annotation is positive
             for the parent example, value in [0, 1], higher means higher
             positivity confidence.
     """
 
-    bounding_box = proto.Field(
+    bounding_box: geometry.BoundingPoly = proto.Field(
         proto.MESSAGE,
         number=1,
         message=geometry.BoundingPoly,
     )
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class BoundingBoxMetricsEntry(proto.Message):
     r"""Bounding box matching model metrics for a single
@@ -61,15 +63,15 @@
         iou_threshold (float):
             Output only. The intersection-over-union
             threshold value used to compute this metrics
             entry.
         mean_average_precision (float):
             Output only. The mean average precision, most often close to
             au_prc.
-        confidence_metrics_entries (Sequence[google.cloud.automl_v1.types.BoundingBoxMetricsEntry.ConfidenceMetricsEntry]):
+        confidence_metrics_entries (MutableSequence[google.cloud.automl_v1.types.BoundingBoxMetricsEntry.ConfidenceMetricsEntry]):
             Output only. Metrics for each label-match
             confidence_threshold from
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99. Precision-recall
             curve is derived from them.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
@@ -86,40 +88,42 @@
                 Output only. Precision under the given
                 confidence threshold.
             f1_score (float):
                 Output only. The harmonic mean of recall and
                 precision.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
 
-    iou_threshold = proto.Field(
+    iou_threshold: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    mean_average_precision = proto.Field(
+    mean_average_precision: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    confidence_metrics_entries = proto.RepeatedField(
+    confidence_metrics_entries: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ConfidenceMetricsEntry,
     )
 
 
 class ImageObjectDetectionEvaluationMetrics(proto.Message):
@@ -127,35 +131,37 @@
     Evaluates prediction quality of labeled bounding boxes.
 
     Attributes:
         evaluated_bounding_box_count (int):
             Output only. The total number of bounding
             boxes (i.e. summed over all images) the ground
             truth used to create this evaluation had.
-        bounding_box_metrics_entries (Sequence[google.cloud.automl_v1.types.BoundingBoxMetricsEntry]):
+        bounding_box_metrics_entries (MutableSequence[google.cloud.automl_v1.types.BoundingBoxMetricsEntry]):
             Output only. The bounding boxes match metrics
             for each Intersection-over-union threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 and each
             label confidence threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 pair.
         bounding_box_mean_average_precision (float):
             Output only. The single metric for bounding boxes
             evaluation: the mean_average_precision averaged over all
             bounding_box_metrics_entries.
     """
 
-    evaluated_bounding_box_count = proto.Field(
+    evaluated_bounding_box_count: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    bounding_box_metrics_entries = proto.RepeatedField(
+    bounding_box_metrics_entries: MutableSequence[
+        "BoundingBoxMetricsEntry"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="BoundingBoxMetricsEntry",
     )
-    bounding_box_mean_average_precision = proto.Field(
+    bounding_box_mean_average_precision: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/geometry.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
     manifest={
         "NormalizedVertex",
@@ -36,36 +38,36 @@
     Attributes:
         x (float):
             Required. Horizontal coordinate.
         y (float):
             Required. Vertical coordinate.
     """
 
-    x = proto.Field(
+    x: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    y = proto.Field(
+    y: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class BoundingPoly(proto.Message):
     r"""A bounding polygon of a detected object on a plane. On output both
     vertices and normalized_vertices are provided. The polygon is formed
     by connecting vertices in the order they are listed.
 
     Attributes:
-        normalized_vertices (Sequence[google.cloud.automl_v1.types.NormalizedVertex]):
+        normalized_vertices (MutableSequence[google.cloud.automl_v1.types.NormalizedVertex]):
             Output only . The bounding polygon normalized
             vertices.
     """
 
-    normalized_vertices = proto.RepeatedField(
+    normalized_vertices: MutableSequence["NormalizedVertex"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="NormalizedVertex",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/image.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import classification
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
@@ -35,15 +37,15 @@
     r"""Dataset metadata that is specific to image classification.
 
     Attributes:
         classification_type (google.cloud.automl_v1.types.ClassificationType):
             Required. Type of the classification problem.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=1,
         enum=classification.ClassificationType,
     )
 
 
 class ImageObjectDetectionDatasetMetadata(proto.Message):
@@ -139,39 +141,39 @@
             model per each node on which it is deployed.
         node_count (int):
             Output only. The number of nodes this model is deployed on.
             A node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the node_qps field.
     """
 
-    base_model_id = proto.Field(
+    base_model_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    train_budget_milli_node_hours = proto.Field(
+    train_budget_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=16,
     )
-    train_cost_milli_node_hours = proto.Field(
+    train_cost_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=17,
     )
-    stop_reason = proto.Field(
+    stop_reason: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    model_type = proto.Field(
+    model_type: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    node_qps = proto.Field(
+    node_qps: float = proto.Field(
         proto.DOUBLE,
         number=13,
     )
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=14,
     )
 
 
 class ImageObjectDetectionModelMetadata(proto.Message):
     r"""Model metadata specific to image object detection.
@@ -244,35 +246,35 @@
             Output only. The actual train cost of
             creating this model, expressed in milli node
             hours, i.e. 1,000 value in this field means 1
             node hour. Guaranteed to not exceed the train
             budget.
     """
 
-    model_type = proto.Field(
+    model_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    node_qps = proto.Field(
+    node_qps: float = proto.Field(
         proto.DOUBLE,
         number=4,
     )
-    stop_reason = proto.Field(
+    stop_reason: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    train_budget_milli_node_hours = proto.Field(
+    train_budget_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    train_cost_milli_node_hours = proto.Field(
+    train_cost_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=7,
     )
 
 
 class ImageClassificationModelDeploymentMetadata(proto.Message):
     r"""Model deployment metadata specific to Image Classification.
@@ -282,15 +284,15 @@
             Input only. The number of nodes to deploy the model on. A
             node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the model's
             [node_qps][google.cloud.automl.v1.ImageClassificationModelMetadata.node_qps].
             Must be between 1 and 100, inclusive on both ends.
     """
 
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
 
 
 class ImageObjectDetectionModelDeploymentMetadata(proto.Message):
     r"""Model deployment metadata specific to Image Object Detection.
@@ -300,14 +302,14 @@
             Input only. The number of nodes to deploy the model on. A
             node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the model's
             [qps_per_node][google.cloud.automl.v1.ImageObjectDetectionModelMetadata.qps_per_node].
             Must be between 1 and 100, inclusive on both ends.
     """
 
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/io.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
     manifest={
         "InputConfig",
@@ -716,36 +718,36 @@
             The Google Cloud Storage location for the input content. For
             [AutoMl.ImportData][google.cloud.automl.v1.AutoMl.ImportData],
             ``gcs_source`` points to a CSV file with a structure
             described in
             [InputConfig][google.cloud.automl.v1.InputConfig].
 
             This field is a member of `oneof`_ ``source``.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional domain-specific parameters describing the
             semantic of the imported data, any string must be up to
             25000 characters long.
 
             .. raw:: html
 
                 <h4>AutoML Tables</h4>
 
             ``schema_inference_version`` : (integer) This value must be
             supplied. The version of the algorithm to use for the
             initial inference of the column data types of the imported
             table. Allowed values: "1".
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class BatchPredictInputConfig(proto.Message):
@@ -1083,15 +1085,15 @@
         gcs_source (google.cloud.automl_v1.types.GcsSource):
             Required. The Google Cloud Storage location
             for the input content.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
 
 
@@ -1105,15 +1107,15 @@
             document file. Only a single path should be
             given.
             Max supported size: 512MB.
 
             Supported extensions: .PDF.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="GcsSource",
     )
 
 
 class OutputConfig(proto.Message):
@@ -1154,15 +1156,15 @@
             export_data-- where timestamp is in YYYY-MM-DDThh:mm:ss.sssZ
             ISO-8601 format. All export output will be written into that
             directory.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -1430,15 +1432,15 @@
             Required. The Google Cloud Storage location
             of the directory where the output is to be
             written to.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
 
 
@@ -1496,53 +1498,53 @@
             -  docker - Used for Docker containers. Use the params field
                to customize the container. The container is verified to
                work correctly on ubuntu 16.04 operating system. See more
                at `containers
                quickstart <https://cloud.google.com/vision/automl/docs/containers-gcs-quickstart>`__
 
             -  core_ml - Used for iOS mobile devices.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional model-type and format specific parameters
             describing the requirements for the to be exported model
             files, any string must be up to 25000 characters long.
 
             -  For ``docker`` format: ``cpu_architecture`` - (string)
                "x86_64" (default). ``gpu_architecture`` - (string)
                "none" (default), "nvidia".
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    model_format = proto.Field(
+    model_format: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class GcsSource(proto.Message):
     r"""The Google Cloud Storage location for the input content.
 
     Attributes:
-        input_uris (Sequence[str]):
+        input_uris (MutableSequence[str]):
             Required. Google Cloud Storage URIs to input files, up to
             2000 characters long. Accepted forms:
 
             -  Full object path, e.g. gs://bucket/directory/object.csv
     """
 
-    input_uris = proto.RepeatedField(
+    input_uris: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class GcsDestination(proto.Message):
     r"""The Google Cloud Storage location where the output is to be
@@ -1554,14 +1556,14 @@
             to 2000 characters long. Accepted forms:
 
             -  Prefix path: gs://bucket/directory The requesting user
                must have write permission to the bucket. The directory
                is created if it doesn't exist.
     """
 
-    output_uri_prefix = proto.Field(
+    output_uri_prefix: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/model.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import image
 from google.cloud.automl_v1.types import text
 from google.cloud.automl_v1.types import translation
 from google.protobuf import timestamp_pb2  # type: ignore
 
@@ -87,15 +89,15 @@
             Output only. Deployment state of the model. A
             model can only serve prediction requests after
             it gets deployed.
         etag (str):
             Used to perform a consistent
             read-modify-write updates. If not set, a blind
             "overwrite" update happens.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Optional. The labels with user-defined
             metadata to organize your model.
             Label keys and values can be no longer than 64
             characters (Unicode codepoints), can only
             contain lowercase letters, numeric characters,
             underscores and dashes. International characters
             are allowed. Label values are optional. Label
@@ -106,82 +108,88 @@
 
     class DeploymentState(proto.Enum):
         r"""Deployment state of the model."""
         DEPLOYMENT_STATE_UNSPECIFIED = 0
         DEPLOYED = 1
         UNDEPLOYED = 2
 
-    translation_model_metadata = proto.Field(
+    translation_model_metadata: translation.TranslationModelMetadata = proto.Field(
         proto.MESSAGE,
         number=15,
         oneof="model_metadata",
         message=translation.TranslationModelMetadata,
     )
-    image_classification_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=13,
-        oneof="model_metadata",
-        message=image.ImageClassificationModelMetadata,
-    )
-    text_classification_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=14,
-        oneof="model_metadata",
-        message=text.TextClassificationModelMetadata,
-    )
-    image_object_detection_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=20,
-        oneof="model_metadata",
-        message=image.ImageObjectDetectionModelMetadata,
+    image_classification_model_metadata: image.ImageClassificationModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=13,
+            oneof="model_metadata",
+            message=image.ImageClassificationModelMetadata,
+        )
+    )
+    text_classification_model_metadata: text.TextClassificationModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=14,
+            oneof="model_metadata",
+            message=text.TextClassificationModelMetadata,
+        )
+    )
+    image_object_detection_model_metadata: image.ImageObjectDetectionModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=20,
+            oneof="model_metadata",
+            message=image.ImageObjectDetectionModelMetadata,
+        )
     )
-    text_extraction_model_metadata = proto.Field(
+    text_extraction_model_metadata: text.TextExtractionModelMetadata = proto.Field(
         proto.MESSAGE,
         number=19,
         oneof="model_metadata",
         message=text.TextExtractionModelMetadata,
     )
-    text_sentiment_model_metadata = proto.Field(
+    text_sentiment_model_metadata: text.TextSentimentModelMetadata = proto.Field(
         proto.MESSAGE,
         number=22,
         oneof="model_metadata",
         message=text.TextSentimentModelMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    dataset_id = proto.Field(
+    dataset_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=11,
         message=timestamp_pb2.Timestamp,
     )
-    deployment_state = proto.Field(
+    deployment_state: DeploymentState = proto.Field(
         proto.ENUM,
         number=8,
         enum=DeploymentState,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=10,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=34,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/model_evaluation.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/model_evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import classification
 from google.cloud.automl_v1.types import detection
 from google.cloud.automl_v1.types import text_extraction
 from google.cloud.automl_v1.types import text_sentiment
 from google.cloud.automl_v1.types import translation
@@ -103,61 +105,65 @@
             annotation_spec_id not set) this is the total number of all
             examples used for evaluation. Otherwise, this is the count
             of examples that according to the ground truth were
             annotated by the
             [annotation_spec_id][google.cloud.automl.v1.ModelEvaluation.annotation_spec_id].
     """
 
-    classification_evaluation_metrics = proto.Field(
+    classification_evaluation_metrics: classification.ClassificationEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="metrics",
         message=classification.ClassificationEvaluationMetrics,
     )
-    translation_evaluation_metrics = proto.Field(
-        proto.MESSAGE,
-        number=9,
-        oneof="metrics",
-        message=translation.TranslationEvaluationMetrics,
+    translation_evaluation_metrics: translation.TranslationEvaluationMetrics = (
+        proto.Field(
+            proto.MESSAGE,
+            number=9,
+            oneof="metrics",
+            message=translation.TranslationEvaluationMetrics,
+        )
     )
-    image_object_detection_evaluation_metrics = proto.Field(
+    image_object_detection_evaluation_metrics: detection.ImageObjectDetectionEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=12,
         oneof="metrics",
         message=detection.ImageObjectDetectionEvaluationMetrics,
     )
-    text_sentiment_evaluation_metrics = proto.Field(
-        proto.MESSAGE,
-        number=11,
-        oneof="metrics",
-        message=text_sentiment.TextSentimentEvaluationMetrics,
+    text_sentiment_evaluation_metrics: text_sentiment.TextSentimentEvaluationMetrics = (
+        proto.Field(
+            proto.MESSAGE,
+            number=11,
+            oneof="metrics",
+            message=text_sentiment.TextSentimentEvaluationMetrics,
+        )
     )
-    text_extraction_evaluation_metrics = proto.Field(
+    text_extraction_evaluation_metrics: text_extraction.TextExtractionEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=13,
         oneof="metrics",
         message=text_extraction.TextExtractionEvaluationMetrics,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    annotation_spec_id = proto.Field(
+    annotation_spec_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=15,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    evaluated_example_count = proto.Field(
+    evaluated_example_count: int = proto.Field(
         proto.INT32,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/operations.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import io
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
 
@@ -84,97 +86,97 @@
         export_model_details (google.cloud.automl_v1.types.ExportModelOperationMetadata):
             Details of ExportModel operation.
 
             This field is a member of `oneof`_ ``details``.
         progress_percent (int):
             Output only. Progress of operation. Range: [0, 100]. Not
             used currently.
-        partial_failures (Sequence[google.rpc.status_pb2.Status]):
+        partial_failures (MutableSequence[google.rpc.status_pb2.Status]):
             Output only. Partial failures encountered.
             E.g. single files that couldn't be read.
             This field should never exceed 20 entries.
             Status details field will contain standard GCP
             error details.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the operation was
             created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the operation was
             updated for the last time.
     """
 
-    delete_details = proto.Field(
+    delete_details: "DeleteOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="details",
         message="DeleteOperationMetadata",
     )
-    deploy_model_details = proto.Field(
+    deploy_model_details: "DeployModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=24,
         oneof="details",
         message="DeployModelOperationMetadata",
     )
-    undeploy_model_details = proto.Field(
+    undeploy_model_details: "UndeployModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=25,
         oneof="details",
         message="UndeployModelOperationMetadata",
     )
-    create_model_details = proto.Field(
+    create_model_details: "CreateModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="details",
         message="CreateModelOperationMetadata",
     )
-    create_dataset_details = proto.Field(
+    create_dataset_details: "CreateDatasetOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=30,
         oneof="details",
         message="CreateDatasetOperationMetadata",
     )
-    import_data_details = proto.Field(
+    import_data_details: "ImportDataOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=15,
         oneof="details",
         message="ImportDataOperationMetadata",
     )
-    batch_predict_details = proto.Field(
+    batch_predict_details: "BatchPredictOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=16,
         oneof="details",
         message="BatchPredictOperationMetadata",
     )
-    export_data_details = proto.Field(
+    export_data_details: "ExportDataOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=21,
         oneof="details",
         message="ExportDataOperationMetadata",
     )
-    export_model_details = proto.Field(
+    export_model_details: "ExportModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=22,
         oneof="details",
         message="ExportModelOperationMetadata",
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=13,
     )
-    partial_failures = proto.RepeatedField(
+    partial_failures: MutableSequence[status_pb2.Status] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=status_pb2.Status,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteOperationMetadata(proto.Message):
@@ -222,21 +224,21 @@
                 The full path of the Google Cloud Storage
                 directory created, into which the exported data
                 is written.
 
                 This field is a member of `oneof`_ ``output_location``.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
             oneof="output_location",
         )
 
-    output_info = proto.Field(
+    output_info: ExportDataOutputInfo = proto.Field(
         proto.MESSAGE,
         number=1,
         message=ExportDataOutputInfo,
     )
 
 
 class BatchPredictOperationMetadata(proto.Message):
@@ -263,26 +265,26 @@
                 The full path of the Google Cloud Storage
                 directory created, into which the prediction
                 output is written.
 
                 This field is a member of `oneof`_ ``output_location``.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
             oneof="output_location",
         )
 
-    input_config = proto.Field(
+    input_config: io.BatchPredictInputConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=io.BatchPredictInputConfig,
     )
-    output_info = proto.Field(
+    output_info: BatchPredictOutputInfo = proto.Field(
         proto.MESSAGE,
         number=2,
         message=BatchPredictOutputInfo,
     )
 
 
 class ExportModelOperationMetadata(proto.Message):
@@ -301,20 +303,20 @@
         Attributes:
             gcs_output_directory (str):
                 The full path of the Google Cloud Storage
                 directory created, into which the model will be
                 exported.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    output_info = proto.Field(
+    output_info: ExportModelOutputInfo = proto.Field(
         proto.MESSAGE,
         number=2,
         message=ExportModelOutputInfo,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/prediction_service.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/prediction_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import annotation_payload
 from google.cloud.automl_v1.types import data_items
 from google.cloud.automl_v1.types import io
 
 
@@ -39,15 +41,15 @@
         name (str):
             Required. Name of the model requested to
             serve the prediction.
         payload (google.cloud.automl_v1.types.ExamplePayload):
             Required. Payload to perform a prediction on.
             The payload must match the problem type that the
             model was trained to solve.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional domain-specific parameters, any string must be up
             to 25000 characters long.
 
             AutoML Vision Classification
 
             ``score_threshold`` : (float) A value from 0.0 to 1.0. When
             the model makes predictions for an image, it will only
@@ -70,50 +72,50 @@
             ``feature_importance`` : (boolean) Whether
             [feature_importance][google.cloud.automl.v1.TablesModelColumnInfo.feature_importance]
             is populated in the returned list of
             [TablesAnnotation][google.cloud.automl.v1.TablesAnnotation]
             objects. The default is false.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    payload = proto.Field(
+    payload: data_items.ExamplePayload = proto.Field(
         proto.MESSAGE,
         number=2,
         message=data_items.ExamplePayload,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=3,
     )
 
 
 class PredictResponse(proto.Message):
     r"""Response message for
     [PredictionService.Predict][google.cloud.automl.v1.PredictionService.Predict].
 
     Attributes:
-        payload (Sequence[google.cloud.automl_v1.types.AnnotationPayload]):
+        payload (MutableSequence[google.cloud.automl_v1.types.AnnotationPayload]):
             Prediction result.
             AutoML Translation and AutoML Natural Language
             Sentiment Analysis return precisely one payload.
         preprocessed_input (google.cloud.automl_v1.types.ExamplePayload):
             The preprocessed example that AutoML actually makes
             prediction on. Empty if AutoML does not preprocess the input
             example.
 
             For AutoML Natural Language (Classification, Entity
             Extraction, and Sentiment Analysis), if the input is a
             document, the recognized text is returned in the
             [document_text][google.cloud.automl.v1.Document.document_text]
             property.
-        metadata (Mapping[str, str]):
+        metadata (MutableMapping[str, str]):
             Additional domain-specific prediction response metadata.
 
             AutoML Vision Object Detection
 
             ``max_bounding_box_count`` : (int64) The maximum number of
             bounding boxes to return per image.
 
@@ -126,25 +128,27 @@
             are relative to the training data, so e.g. if all data was
             positive then -1 is also positive (though the least).
             ``sentiment_score`` is not the same as "score" and
             "magnitude" from Sentiment Analysis in the Natural Language
             API.
     """
 
-    payload = proto.RepeatedField(
+    payload: MutableSequence[
+        annotation_payload.AnnotationPayload
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=annotation_payload.AnnotationPayload,
     )
-    preprocessed_input = proto.Field(
+    preprocessed_input: data_items.ExamplePayload = proto.Field(
         proto.MESSAGE,
         number=3,
         message=data_items.ExamplePayload,
     )
-    metadata = proto.MapField(
+    metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class BatchPredictRequest(proto.Message):
@@ -157,15 +161,15 @@
             serve the batch prediction.
         input_config (google.cloud.automl_v1.types.BatchPredictInputConfig):
             Required. The input configuration for batch
             prediction.
         output_config (google.cloud.automl_v1.types.BatchPredictOutputConfig):
             Required. The Configuration specifying where
             output predictions should be written.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional domain-specific parameters for the predictions,
             any string must be up to 25000 characters long.
 
             AutoML Natural Language Classification
 
             ``score_threshold`` : (float) A value from 0.0 to 1.0. When
             the model makes predictions for a text snippet, it will only
@@ -242,57 +246,57 @@
 
             ``min_bounding_box_size`` : (float) Only bounding boxes with
             shortest edge at least that long as a relative value of
             video frame size are returned. Value in 0 to 1 range.
             Default is 0.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_config = proto.Field(
+    input_config: io.BatchPredictInputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.BatchPredictInputConfig,
     )
-    output_config = proto.Field(
+    output_config: io.BatchPredictOutputConfig = proto.Field(
         proto.MESSAGE,
         number=4,
         message=io.BatchPredictOutputConfig,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=5,
     )
 
 
 class BatchPredictResult(proto.Message):
     r"""Result of the Batch Predict. This message is returned in
     [response][google.longrunning.Operation.response] of the operation
     returned by the
     [PredictionService.BatchPredict][google.cloud.automl.v1.PredictionService.BatchPredict].
 
     Attributes:
-        metadata (Mapping[str, str]):
+        metadata (MutableMapping[str, str]):
             Additional domain-specific prediction response metadata.
 
             AutoML Vision Object Detection
 
             ``max_bounding_box_count`` : (int64) The maximum number of
             bounding boxes returned per image.
 
             AutoML Video Intelligence Object Tracking
 
             ``max_bounding_box_count`` : (int64) The maximum number of
             bounding boxes returned per frame.
     """
 
-    metadata = proto.MapField(
+    metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/service.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import dataset as gca_dataset
 from google.cloud.automl_v1.types import image
 from google.cloud.automl_v1.types import io
 from google.cloud.automl_v1.types import model as gca_model
 from google.cloud.automl_v1.types import model_evaluation as gca_model_evaluation
@@ -59,19 +61,19 @@
         parent (str):
             Required. The resource name of the project to
             create the dataset for.
         dataset (google.cloud.automl_v1.types.Dataset):
             Required. The dataset to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    dataset = proto.Field(
+    dataset: gca_dataset.Dataset = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gca_dataset.Dataset,
     )
 
 
 class GetDatasetRequest(proto.Message):
@@ -80,15 +82,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the dataset to
             retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListDatasetsRequest(proto.Message):
     r"""Request message for
@@ -116,55 +118,55 @@
             return Typically obtained via
             [ListDatasetsResponse.next_page_token][google.cloud.automl.v1.ListDatasetsResponse.next_page_token]
             of the previous
             [AutoMl.ListDatasets][google.cloud.automl.v1.AutoMl.ListDatasets]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListDatasetsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListDatasets][google.cloud.automl.v1.AutoMl.ListDatasets].
 
     Attributes:
-        datasets (Sequence[google.cloud.automl_v1.types.Dataset]):
+        datasets (MutableSequence[google.cloud.automl_v1.types.Dataset]):
             The datasets read.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListDatasetsRequest.page_token][google.cloud.automl.v1.ListDatasetsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    datasets = proto.RepeatedField(
+    datasets: MutableSequence[gca_dataset.Dataset] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_dataset.Dataset,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class UpdateDatasetRequest(proto.Message):
     r"""Request message for
@@ -175,20 +177,20 @@
             Required. The dataset which replaces the
             resource on the server.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. The update mask applies to the
             resource.
     """
 
-    dataset = proto.Field(
+    dataset: gca_dataset.Dataset = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gca_dataset.Dataset,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteDatasetRequest(proto.Message):
@@ -197,15 +199,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the dataset to
             delete.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ImportDataRequest(proto.Message):
     r"""Request message for
@@ -217,19 +219,19 @@
             exist. All imported annotations and examples
             will be added.
         input_config (google.cloud.automl_v1.types.InputConfig):
             Required. The desired input location and its
             domain specific semantics, if any.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_config = proto.Field(
+    input_config: io.InputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.InputConfig,
     )
 
 
 class ExportDataRequest(proto.Message):
@@ -239,19 +241,19 @@
     Attributes:
         name (str):
             Required. The resource name of the dataset.
         output_config (google.cloud.automl_v1.types.OutputConfig):
             Required. The desired output location.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    output_config = proto.Field(
+    output_config: io.OutputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.OutputConfig,
     )
 
 
 class GetAnnotationSpecRequest(proto.Message):
@@ -260,15 +262,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the annotation
             spec to retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CreateModelRequest(proto.Message):
     r"""Request message for
@@ -278,19 +280,19 @@
         parent (str):
             Required. Resource name of the parent project
             where the model is being created.
         model (google.cloud.automl_v1.types.Model):
             Required. The model to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: gca_model.Model = proto.Field(
         proto.MESSAGE,
         number=4,
         message=gca_model.Model,
     )
 
 
 class GetModelRequest(proto.Message):
@@ -298,15 +300,15 @@
     [AutoMl.GetModel][google.cloud.automl.v1.AutoMl.GetModel].
 
     Attributes:
         name (str):
             Required. Resource name of the model.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListModelsRequest(proto.Message):
     r"""Request message for
@@ -337,55 +339,55 @@
             return Typically obtained via
             [ListModelsResponse.next_page_token][google.cloud.automl.v1.ListModelsResponse.next_page_token]
             of the previous
             [AutoMl.ListModels][google.cloud.automl.v1.AutoMl.ListModels]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListModelsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListModels][google.cloud.automl.v1.AutoMl.ListModels].
 
     Attributes:
-        model (Sequence[google.cloud.automl_v1.types.Model]):
+        model (MutableSequence[google.cloud.automl_v1.types.Model]):
             List of models in the requested page.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListModelsRequest.page_token][google.cloud.automl.v1.ListModelsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    model = proto.RepeatedField(
+    model: MutableSequence[gca_model.Model] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_model.Model,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class DeleteModelRequest(proto.Message):
     r"""Request message for
@@ -393,15 +395,15 @@
 
     Attributes:
         name (str):
             Required. Resource name of the model being
             deleted.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateModelRequest(proto.Message):
     r"""Request message for
@@ -412,20 +414,20 @@
             Required. The model which replaces the
             resource on the server.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. The update mask applies to the
             resource.
     """
 
-    model = proto.Field(
+    model: gca_model.Model = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gca_model.Model,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class DeployModelRequest(proto.Message):
@@ -451,27 +453,27 @@
 
             This field is a member of `oneof`_ ``model_deployment_metadata``.
         name (str):
             Required. Resource name of the model to
             deploy.
     """
 
-    image_object_detection_model_deployment_metadata = proto.Field(
+    image_object_detection_model_deployment_metadata: image.ImageObjectDetectionModelDeploymentMetadata = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="model_deployment_metadata",
         message=image.ImageObjectDetectionModelDeploymentMetadata,
     )
-    image_classification_model_deployment_metadata = proto.Field(
+    image_classification_model_deployment_metadata: image.ImageClassificationModelDeploymentMetadata = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="model_deployment_metadata",
         message=image.ImageClassificationModelDeploymentMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UndeployModelRequest(proto.Message):
     r"""Request message for
@@ -479,15 +481,15 @@
 
     Attributes:
         name (str):
             Required. Resource name of the model to
             undeploy.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExportModelRequest(proto.Message):
     r"""Request message for
@@ -500,19 +502,19 @@
             Required. The resource name of the model to
             export.
         output_config (google.cloud.automl_v1.types.ModelExportOutputConfig):
             Required. The desired output location and
             configuration.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    output_config = proto.Field(
+    output_config: io.ModelExportOutputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.ModelExportOutputConfig,
     )
 
 
 class GetModelEvaluationRequest(proto.Message):
@@ -521,15 +523,15 @@
 
     Attributes:
         name (str):
             Required. Resource name for the model
             evaluation.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListModelEvaluationsRequest(proto.Message):
     r"""Request message for
@@ -561,57 +563,59 @@
             return. Typically obtained via
             [ListModelEvaluationsResponse.next_page_token][google.cloud.automl.v1.ListModelEvaluationsResponse.next_page_token]
             of the previous
             [AutoMl.ListModelEvaluations][google.cloud.automl.v1.AutoMl.ListModelEvaluations]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListModelEvaluationsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListModelEvaluations][google.cloud.automl.v1.AutoMl.ListModelEvaluations].
 
     Attributes:
-        model_evaluation (Sequence[google.cloud.automl_v1.types.ModelEvaluation]):
+        model_evaluation (MutableSequence[google.cloud.automl_v1.types.ModelEvaluation]):
             List of model evaluations in the requested
             page.
         next_page_token (str):
             A token to retrieve next page of results. Pass to the
             [ListModelEvaluationsRequest.page_token][google.cloud.automl.v1.ListModelEvaluationsRequest.page_token]
             field of a new
             [AutoMl.ListModelEvaluations][google.cloud.automl.v1.AutoMl.ListModelEvaluations]
             request to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    model_evaluation = proto.RepeatedField(
+    model_evaluation: MutableSequence[
+        gca_model_evaluation.ModelEvaluation
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_model_evaluation.ModelEvaluation,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import classification
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
@@ -35,15 +37,15 @@
     r"""Dataset metadata for classification.
 
     Attributes:
         classification_type (google.cloud.automl_v1.types.ClassificationType):
             Required. Type of the classification problem.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=1,
         enum=classification.ClassificationType,
     )
 
 
 class TextClassificationModelMetadata(proto.Message):
@@ -51,15 +53,15 @@
 
     Attributes:
         classification_type (google.cloud.automl_v1.types.ClassificationType):
             Output only. Classification type of the
             dataset used to train this model.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=3,
         enum=classification.ClassificationType,
     )
 
 
 class TextExtractionDatasetMetadata(proto.Message):
@@ -80,15 +82,15 @@
             range of sentiments that will be used is between 0 and
             sentiment_max (inclusive on both ends), and all the values
             in the range must be represented in the dataset before a
             model can be created. sentiment_max value must be between 1
             and 10 (inclusive).
     """
 
-    sentiment_max = proto.Field(
+    sentiment_max: int = proto.Field(
         proto.INT32,
         number=1,
     )
 
 
 class TextSentimentModelMetadata(proto.Message):
     r"""Model metadata that is specific to text sentiment."""
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_extraction.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_extraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import text_segment as gca_text_segment
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
@@ -41,34 +43,34 @@
             This field is a member of `oneof`_ ``annotation``.
         score (float):
             Output only. A confidence estimate between
             0.0 and 1.0. A higher value means greater
             confidence in correctness of the annotation.
     """
 
-    text_segment = proto.Field(
+    text_segment: gca_text_segment.TextSegment = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="annotation",
         message=gca_text_segment.TextSegment,
     )
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
 
 
 class TextExtractionEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for text extraction problems.
 
     Attributes:
         au_prc (float):
             Output only. The Area under precision recall
             curve metric.
-        confidence_metrics_entries (Sequence[google.cloud.automl_v1.types.TextExtractionEvaluationMetrics.ConfidenceMetricsEntry]):
+        confidence_metrics_entries (MutableSequence[google.cloud.automl_v1.types.TextExtractionEvaluationMetrics.ConfidenceMetricsEntry]):
             Output only. Metrics that have confidence
             thresholds. Precision-recall curve can be
             derived from it.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
         r"""Metrics for a single confidence threshold.
@@ -86,36 +88,38 @@
                 Output only. Precision under the given
                 confidence threshold.
             f1_score (float):
                 Output only. The harmonic mean of recall and
                 precision.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=5,
         )
 
-    au_prc = proto.Field(
+    au_prc: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    confidence_metrics_entries = proto.RepeatedField(
+    confidence_metrics_entries: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=ConfidenceMetricsEntry,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_segment.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
     manifest={
         "TextSegment",
@@ -38,22 +40,22 @@
         end_offset (int):
             Required. Zero-based character index of the first character
             past the end of the text segment (counting character from
             the beginning of the text). The character at the end_offset
             is NOT included in the text segment.
     """
 
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    start_offset = proto.Field(
+    start_offset: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    end_offset = proto.Field(
+    end_offset: int = proto.Field(
         proto.INT64,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/text_sentiment.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_sentiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
-from google.cloud.automl_v1.types import classification
+from google.cloud.automl_v1beta1.types import classification
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.automl.v1",
+    package="google.cloud.automl.v1beta1",
     manifest={
         "TextSentimentAnnotation",
         "TextSentimentEvaluationMetrics",
     },
 )
 
 
 class TextSentimentAnnotation(proto.Message):
     r"""Contains annotation details specific to text sentiment.
 
     Attributes:
         sentiment (int):
             Output only. The sentiment with the semantic, as given to
             the
-            [AutoMl.ImportData][google.cloud.automl.v1.AutoMl.ImportData]
+            [AutoMl.ImportData][google.cloud.automl.v1beta1.AutoMl.ImportData]
             when populating the dataset from which the model used for
             the prediction had been trained. The sentiment values are
             between 0 and
             Dataset.text_sentiment_dataset_metadata.sentiment_max
             (inclusive), with higher value meaning more positive
             sentiment. They are completely relative, i.e. 0 means least
             positive sentiment and sentiment_max means the most positive
@@ -46,15 +48,15 @@
             e.g. if train data had only negative sentiment, then
             sentiment_max, would be still negative (although least
             negative). The sentiment shouldn't be confused with "score"
             or "magnitude" from the previous Natural Language Sentiment
             Analysis API.
     """
 
-    sentiment = proto.Field(
+    sentiment: int = proto.Field(
         proto.INT32,
         number=1,
     )
 
 
 class TextSentimentEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for text sentiment problems.
@@ -79,50 +81,59 @@
             Output only. Linear weighted kappa. Only set
             for the overall model evaluation, not for
             evaluation of a single annotation spec.
         quadratic_kappa (float):
             Output only. Quadratic weighted kappa. Only
             set for the overall model evaluation, not for
             evaluation of a single annotation spec.
-        confusion_matrix (google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
+        confusion_matrix (google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
             Output only. Confusion matrix of the
             evaluation. Only set for the overall model
             evaluation, not for evaluation of a single
             annotation spec.
+        annotation_spec_id (MutableSequence[str]):
+            Output only. The annotation spec ids used for
+            this evaluation. Deprecated .
     """
 
-    precision = proto.Field(
+    precision: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    recall = proto.Field(
+    recall: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    f1_score = proto.Field(
+    f1_score: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    mean_absolute_error = proto.Field(
+    mean_absolute_error: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    mean_squared_error = proto.Field(
+    mean_squared_error: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
-    linear_kappa = proto.Field(
+    linear_kappa: float = proto.Field(
         proto.FLOAT,
         number=6,
     )
-    quadratic_kappa = proto.Field(
+    quadratic_kappa: float = proto.Field(
         proto.FLOAT,
         number=7,
     )
-    confusion_matrix = proto.Field(
-        proto.MESSAGE,
-        number=8,
-        message=classification.ClassificationEvaluationMetrics.ConfusionMatrix,
+    confusion_matrix: classification.ClassificationEvaluationMetrics.ConfusionMatrix = (
+        proto.Field(
+            proto.MESSAGE,
+            number=8,
+            message=classification.ClassificationEvaluationMetrics.ConfusionMatrix,
+        )
+    )
+    annotation_spec_id: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=9,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1/types/translation.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/translation.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1.types import data_items
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1",
@@ -37,19 +39,19 @@
             Required. The BCP-47 language code of the
             source language.
         target_language_code (str):
             Required. The BCP-47 language code of the
             target language.
     """
 
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class TranslationEvaluationMetrics(proto.Message):
     r"""Evaluation metrics for the dataset.
@@ -57,19 +59,19 @@
     Attributes:
         bleu_score (float):
             Output only. BLEU score.
         base_bleu_score (float):
             Output only. BLEU score for base model.
     """
 
-    bleu_score = proto.Field(
+    bleu_score: float = proto.Field(
         proto.DOUBLE,
         number=1,
     )
-    base_bleu_score = proto.Field(
+    base_bleu_score: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
 
 
 class TranslationModelMetadata(proto.Message):
     r"""Model metadata that is specific to translation.
@@ -85,37 +87,37 @@
             The source language (The BCP-47 language code)
             that is used for training.
         target_language_code (str):
             Output only. The target language (The BCP-47
             language code) that is used for training.
     """
 
-    base_model = proto.Field(
+    base_model: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslationAnnotation(proto.Message):
     r"""Annotation details specific to translation.
 
     Attributes:
         translated_content (google.cloud.automl_v1.types.TextSnippet):
             Output only . The translated content.
     """
 
-    translated_content = proto.Field(
+    translated_content: data_items.TextSnippet = proto.Field(
         proto.MESSAGE,
         number=1,
         message=data_items.TextSnippet,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.automl import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.auto_ml import AutoMlClient
 from .services.auto_ml import AutoMlAsyncClient
 from .services.prediction_service import PredictionServiceClient
 from .services.tables.gcs_client import GcsClient
 from .services.tables.tables_client import TablesClient
 from .services.prediction_service import PredictionServiceAsyncClient
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/gapic_metadata.json` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/async_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -197,17 +208,17 @@
     get_transport_class = functools.partial(
         type(AutoMlClient).get_transport_class, type(AutoMlClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, AutoMlTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto ml client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -243,20 +254,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def create_dataset(
         self,
-        request: Union[service.CreateDatasetRequest, dict] = None,
+        request: Optional[Union[service.CreateDatasetRequest, dict]] = None,
         *,
-        parent: str = None,
-        dataset: gca_dataset.Dataset = None,
+        parent: Optional[str] = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Creates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -285,15 +296,15 @@
                 # Make the request
                 response = await client.create_dataset(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.CreateDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.CreateDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.CreateDataset][google.cloud.automl.v1beta1.AutoMl.CreateDataset].
             parent (:class:`str`):
                 Required. The resource name of the
                 project to create the dataset for.
 
                 This corresponds to the ``parent`` field
@@ -360,19 +371,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_dataset(
         self,
-        request: Union[service.GetDatasetRequest, dict] = None,
+        request: Optional[Union[service.GetDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
         r"""Gets a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -396,15 +407,15 @@
                 # Make the request
                 response = await client.get_dataset(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetDataset][google.cloud.automl.v1beta1.AutoMl.GetDataset].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset to retrieve.
 
                 This corresponds to the ``name`` field
@@ -474,19 +485,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_datasets(
         self,
-        request: Union[service.ListDatasetsRequest, dict] = None,
+        request: Optional[Union[service.ListDatasetsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsAsyncPager:
         r"""Lists datasets in a project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -511,15 +522,15 @@
                 page_result = client.list_datasets(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ListDatasetsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ListDatasetsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListDatasets][google.cloud.automl.v1beta1.AutoMl.ListDatasets].
             parent (:class:`str`):
                 Required. The resource name of the
                 project from which to list datasets.
 
                 This corresponds to the ``parent`` field
@@ -599,19 +610,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_dataset(
         self,
-        request: Union[service.UpdateDatasetRequest, dict] = None,
+        request: Optional[Union[service.UpdateDatasetRequest, dict]] = None,
         *,
-        dataset: gca_dataset.Dataset = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Updates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -639,15 +650,15 @@
                 # Make the request
                 response = await client.update_dataset(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.UpdateDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.UpdateDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UpdateDataset][google.cloud.automl.v1beta1.AutoMl.UpdateDataset]
             dataset (:class:`google.cloud.automl_v1beta1.types.Dataset`):
                 Required. The dataset which replaces
                 the resource on the server.
 
                 This corresponds to the ``dataset`` field
@@ -709,19 +720,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_dataset(
         self,
-        request: Union[service.DeleteDatasetRequest, dict] = None,
+        request: Optional[Union[service.DeleteDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a dataset and all of its contents. Returns empty
         response in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
@@ -747,21 +758,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_dataset(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.DeleteDatasetRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.DeleteDatasetRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeleteDataset][google.cloud.automl.v1beta1.AutoMl.DeleteDataset].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset to delete.
 
                 This corresponds to the ``name`` field
@@ -847,20 +858,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def import_data(
         self,
-        request: Union[service.ImportDataRequest, dict] = None,
+        request: Optional[Union[service.ImportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.InputConfig = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.InputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Imports data into a dataset. For Tables this method can only be
         called on an empty Dataset.
 
         For Tables:
 
@@ -891,21 +902,21 @@
                 )
 
                 # Make the request
                 operation = client.import_data(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ImportDataRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ImportDataRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ImportData][google.cloud.automl.v1beta1.AutoMl.ImportData].
             name (:class:`str`):
                 Required. Dataset name. Dataset must
                 already exist. All imported annotations
                 and examples will be added.
 
@@ -992,20 +1003,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def export_data(
         self,
-        request: Union[service.ExportDataRequest, dict] = None,
+        request: Optional[Union[service.ExportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.OutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.OutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Exports dataset's data to the provided output location. Returns
         an empty response in the
         [response][google.longrunning.Operation.response] field when it
         completes.
 
@@ -1030,21 +1041,21 @@
                 )
 
                 # Make the request
                 operation = client.export_data(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ExportDataRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ExportDataRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ExportData][google.cloud.automl.v1beta1.AutoMl.ExportData].
             name (:class:`str`):
                 Required. The resource name of the
                 dataset.
 
                 This corresponds to the ``name`` field
@@ -1129,19 +1140,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_annotation_spec(
         self,
-        request: Union[service.GetAnnotationSpecRequest, dict] = None,
+        request: Optional[Union[service.GetAnnotationSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> annotation_spec.AnnotationSpec:
         r"""Gets an annotation spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1165,15 +1176,15 @@
                 # Make the request
                 response = await client.get_annotation_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetAnnotationSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetAnnotationSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetAnnotationSpec][google.cloud.automl.v1beta1.AutoMl.GetAnnotationSpec].
             name (:class:`str`):
                 Required. The resource name of the
                 annotation spec to retrieve.
 
                 This corresponds to the ``name`` field
@@ -1239,19 +1250,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_table_spec(
         self,
-        request: Union[service.GetTableSpecRequest, dict] = None,
+        request: Optional[Union[service.GetTableSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> table_spec.TableSpec:
         r"""Gets a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1275,15 +1286,15 @@
                 # Make the request
                 response = await client.get_table_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetTableSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetTableSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetTableSpec][google.cloud.automl.v1beta1.AutoMl.GetTableSpec].
             name (:class:`str`):
                 Required. The resource name of the
                 table spec to retrieve.
 
                 This corresponds to the ``name`` field
@@ -1359,19 +1370,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_table_specs(
         self,
-        request: Union[service.ListTableSpecsRequest, dict] = None,
+        request: Optional[Union[service.ListTableSpecsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListTableSpecsAsyncPager:
         r"""Lists table specs in a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1396,15 +1407,15 @@
                 page_result = client.list_table_specs(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ListTableSpecsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ListTableSpecsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListTableSpecs][google.cloud.automl.v1beta1.AutoMl.ListTableSpecs].
             parent (:class:`str`):
                 Required. The resource name of the
                 dataset to list table specs from.
 
                 This corresponds to the ``parent`` field
@@ -1484,19 +1495,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_table_spec(
         self,
-        request: Union[service.UpdateTableSpecRequest, dict] = None,
+        request: Optional[Union[service.UpdateTableSpecRequest, dict]] = None,
         *,
-        table_spec: gca_table_spec.TableSpec = None,
+        table_spec: Optional[gca_table_spec.TableSpec] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_table_spec.TableSpec:
         r"""Updates a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1519,15 +1530,15 @@
                 # Make the request
                 response = await client.update_table_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.UpdateTableSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.UpdateTableSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UpdateTableSpec][google.cloud.automl.v1beta1.AutoMl.UpdateTableSpec]
             table_spec (:class:`google.cloud.automl_v1beta1.types.TableSpec`):
                 Required. The table spec which
                 replaces the resource on the server.
 
                 This corresponds to the ``table_spec`` field
@@ -1595,19 +1606,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_column_spec(
         self,
-        request: Union[service.GetColumnSpecRequest, dict] = None,
+        request: Optional[Union[service.GetColumnSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> column_spec.ColumnSpec:
         r"""Gets a column spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1631,15 +1642,15 @@
                 # Make the request
                 response = await client.get_column_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetColumnSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetColumnSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetColumnSpec][google.cloud.automl.v1beta1.AutoMl.GetColumnSpec].
             name (:class:`str`):
                 Required. The resource name of the
                 column spec to retrieve.
 
                 This corresponds to the ``name`` field
@@ -1707,19 +1718,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_column_specs(
         self,
-        request: Union[service.ListColumnSpecsRequest, dict] = None,
+        request: Optional[Union[service.ListColumnSpecsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListColumnSpecsAsyncPager:
         r"""Lists column specs in a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1744,15 +1755,15 @@
                 page_result = client.list_column_specs(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ListColumnSpecsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ListColumnSpecsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListColumnSpecs][google.cloud.automl.v1beta1.AutoMl.ListColumnSpecs].
             parent (:class:`str`):
                 Required. The resource name of the
                 table spec to list column specs from.
 
                 This corresponds to the ``parent`` field
@@ -1832,19 +1843,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def update_column_spec(
         self,
-        request: Union[service.UpdateColumnSpecRequest, dict] = None,
+        request: Optional[Union[service.UpdateColumnSpecRequest, dict]] = None,
         *,
-        column_spec: gca_column_spec.ColumnSpec = None,
+        column_spec: Optional[gca_column_spec.ColumnSpec] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_column_spec.ColumnSpec:
         r"""Updates a column spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1867,15 +1878,15 @@
                 # Make the request
                 response = await client.update_column_spec(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.UpdateColumnSpecRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.UpdateColumnSpecRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UpdateColumnSpec][google.cloud.automl.v1beta1.AutoMl.UpdateColumnSpec]
             column_spec (:class:`google.cloud.automl_v1beta1.types.ColumnSpec`):
                 Required. The column spec which
                 replaces the resource on the server.
 
                 This corresponds to the ``column_spec`` field
@@ -1935,20 +1946,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def create_model(
         self,
-        request: Union[service.CreateModelRequest, dict] = None,
+        request: Optional[Union[service.CreateModelRequest, dict]] = None,
         *,
-        parent: str = None,
-        model: gca_model.Model = None,
+        parent: Optional[str] = None,
+        model: Optional[gca_model.Model] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Creates a model. Returns a Model in the
         [response][google.longrunning.Operation.response] field when it
         completes. When you create a model, several model evaluations
         are created for it: a global evaluation, and one evaluation for
         each annotation spec.
@@ -1974,21 +1985,21 @@
                 )
 
                 # Make the request
                 operation = client.create_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.CreateModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.CreateModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.CreateModel][google.cloud.automl.v1beta1.AutoMl.CreateModel].
             parent (:class:`str`):
                 Required. Resource name of the parent
                 project where the model is being
                 created.
 
@@ -2065,19 +2076,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_model(
         self,
-        request: Union[service.GetModelRequest, dict] = None,
+        request: Optional[Union[service.GetModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model.Model:
         r"""Gets a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2101,15 +2112,15 @@
                 # Make the request
                 response = await client.get_model(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetModel][google.cloud.automl.v1beta1.AutoMl.GetModel].
             name (:class:`str`):
                 Required. Resource name of the model.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -2175,19 +2186,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_models(
         self,
-        request: Union[service.ListModelsRequest, dict] = None,
+        request: Optional[Union[service.ListModelsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelsAsyncPager:
         r"""Lists models.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2212,15 +2223,15 @@
                 page_result = client.list_models(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ListModelsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ListModelsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListModels][google.cloud.automl.v1beta1.AutoMl.ListModels].
             parent (:class:`str`):
                 Required. Resource name of the
                 project, from which to list the models.
 
                 This corresponds to the ``parent`` field
@@ -2300,19 +2311,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_model(
         self,
-        request: Union[service.DeleteModelRequest, dict] = None,
+        request: Optional[Union[service.DeleteModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deletes a model. Returns ``google.protobuf.Empty`` in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
 
@@ -2337,21 +2348,21 @@
                 )
 
                 # Make the request
                 operation = client.delete_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.DeleteModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.DeleteModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeleteModel][google.cloud.automl.v1beta1.AutoMl.DeleteModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 being deleted.
 
                 This corresponds to the ``name`` field
@@ -2437,19 +2448,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def deploy_model(
         self,
-        request: Union[service.DeployModelRequest, dict] = None,
+        request: Optional[Union[service.DeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Deploys a model. If a model is already deployed, deploying it
         with the same parameters has no effect. Deploying with different
         parametrs (as e.g. changing
 
         [node_number][google.cloud.automl.v1beta1.ImageObjectDetectionModelDeploymentMetadata.node_number])
@@ -2485,21 +2496,21 @@
                 )
 
                 # Make the request
                 operation = client.deploy_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.DeployModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.DeployModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.DeployModel][google.cloud.automl.v1beta1.AutoMl.DeployModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 to deploy.
 
                 This corresponds to the ``name`` field
@@ -2575,19 +2586,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def undeploy_model(
         self,
-        request: Union[service.UndeployModelRequest, dict] = None,
+        request: Optional[Union[service.UndeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Undeploys a model. If the model is not deployed this method has
         no effect.
 
         Only applicable for Text Classification, Image Object Detection
         and Tables; all other domains manage deployment automatically.
@@ -2617,21 +2628,21 @@
                 )
 
                 # Make the request
                 operation = client.undeploy_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.UndeployModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.UndeployModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.UndeployModel][google.cloud.automl.v1beta1.AutoMl.UndeployModel].
             name (:class:`str`):
                 Required. Resource name of the model
                 to undeploy.
 
                 This corresponds to the ``name`` field
@@ -2707,20 +2718,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def export_model(
         self,
-        request: Union[service.ExportModelRequest, dict] = None,
+        request: Optional[Union[service.ExportModelRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ModelExportOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ModelExportOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Exports a trained, "export-able", model to a user specified
         Google Cloud Storage location. A model is considered export-able
         if and only if it has an export format defined for it in
 
         [ModelExportOutputConfig][google.cloud.automl.v1beta1.ModelExportOutputConfig].
@@ -2750,21 +2761,21 @@
                 )
 
                 # Make the request
                 operation = client.export_model(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ExportModelRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ExportModelRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ExportModel][google.cloud.automl.v1beta1.AutoMl.ExportModel].
                 Models need to be enabled for exporting, otherwise an
                 error code will be returned.
             name (:class:`str`):
                 Required. The resource name of the
                 model to export.
@@ -2851,20 +2862,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def export_evaluated_examples(
         self,
-        request: Union[service.ExportEvaluatedExamplesRequest, dict] = None,
+        request: Optional[Union[service.ExportEvaluatedExamplesRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ExportEvaluatedExamplesOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ExportEvaluatedExamplesOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Exports examples on which the model was evaluated (i.e. which
         were in the TEST set of the dataset the model was created from),
         together with their ground truth annotations and the annotations
         created (predicted) by the model. The examples, ground truth and
         predictions are exported in the state they were at the moment
@@ -2900,21 +2911,21 @@
                 )
 
                 # Make the request
                 operation = client.export_evaluated_examples(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ExportEvaluatedExamplesRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ExportEvaluatedExamplesRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ExportEvaluatedExamples][google.cloud.automl.v1beta1.AutoMl.ExportEvaluatedExamples].
             name (:class:`str`):
                 Required. The resource name of the
                 model whose evaluated examples are to be
                 exported.
 
@@ -3000,19 +3011,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_model_evaluation(
         self,
-        request: Union[service.GetModelEvaluationRequest, dict] = None,
+        request: Optional[Union[service.GetModelEvaluationRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model_evaluation.ModelEvaluation:
         r"""Gets a model evaluation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -3036,15 +3047,15 @@
                 # Make the request
                 response = await client.get_model_evaluation(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.GetModelEvaluationRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.GetModelEvaluationRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.GetModelEvaluation][google.cloud.automl.v1beta1.AutoMl.GetModelEvaluation].
             name (:class:`str`):
                 Required. Resource name for the model
                 evaluation.
 
                 This corresponds to the ``name`` field
@@ -3110,19 +3121,19 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_model_evaluations(
         self,
-        request: Union[service.ListModelEvaluationsRequest, dict] = None,
+        request: Optional[Union[service.ListModelEvaluationsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelEvaluationsAsyncPager:
         r"""Lists model evaluations.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -3147,15 +3158,15 @@
                 page_result = client.list_model_evaluations(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.ListModelEvaluationsRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.ListModelEvaluationsRequest, dict]]):
                 The request object. Request message for
                 [AutoMl.ListModelEvaluations][google.cloud.automl.v1beta1.AutoMl.ListModelEvaluations].
             parent (:class:`str`):
                 Required. Resource name of the model
                 to list the model evaluations for. If
                 modelId is set as "-", this will list
                 model evaluations from across all models
@@ -3233,18 +3244,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoMlAsyncClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -79,15 +91,15 @@
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[AutoMlTransport]]
     _transport_registry["grpc"] = AutoMlGrpcTransport
     _transport_registry["grpc_asyncio"] = AutoMlGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[AutoMlTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -489,30 +501,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, AutoMlTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, AutoMlTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the auto ml client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, AutoMlTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -534,14 +546,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -586,20 +599,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def create_dataset(
         self,
-        request: Union[service.CreateDatasetRequest, dict] = None,
+        request: Optional[Union[service.CreateDatasetRequest, dict]] = None,
         *,
-        parent: str = None,
-        dataset: gca_dataset.Dataset = None,
+        parent: Optional[str] = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Creates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -703,19 +716,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_dataset(
         self,
-        request: Union[service.GetDatasetRequest, dict] = None,
+        request: Optional[Union[service.GetDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
         r"""Gets a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -807,19 +820,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_datasets(
         self,
-        request: Union[service.ListDatasetsRequest, dict] = None,
+        request: Optional[Union[service.ListDatasetsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsPager:
         r"""Lists datasets in a project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -922,19 +935,19 @@
         )
 
         # Done; return the response.
         return response
 
     def update_dataset(
         self,
-        request: Union[service.UpdateDatasetRequest, dict] = None,
+        request: Optional[Union[service.UpdateDatasetRequest, dict]] = None,
         *,
-        dataset: gca_dataset.Dataset = None,
+        dataset: Optional[gca_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_dataset.Dataset:
         r"""Updates a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1032,19 +1045,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_dataset(
         self,
-        request: Union[service.DeleteDatasetRequest, dict] = None,
+        request: Optional[Union[service.DeleteDatasetRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a dataset and all of its contents. Returns empty
         response in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
@@ -1160,20 +1173,20 @@
         )
 
         # Done; return the response.
         return response
 
     def import_data(
         self,
-        request: Union[service.ImportDataRequest, dict] = None,
+        request: Optional[Union[service.ImportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.InputConfig = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.InputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Imports data into a dataset. For Tables this method can only be
         called on an empty Dataset.
 
         For Tables:
 
@@ -1305,20 +1318,20 @@
         )
 
         # Done; return the response.
         return response
 
     def export_data(
         self,
-        request: Union[service.ExportDataRequest, dict] = None,
+        request: Optional[Union[service.ExportDataRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.OutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.OutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Exports dataset's data to the provided output location. Returns
         an empty response in the
         [response][google.longrunning.Operation.response] field when it
         completes.
 
@@ -1442,19 +1455,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_annotation_spec(
         self,
-        request: Union[service.GetAnnotationSpecRequest, dict] = None,
+        request: Optional[Union[service.GetAnnotationSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> annotation_spec.AnnotationSpec:
         r"""Gets an annotation spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1542,19 +1555,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_table_spec(
         self,
-        request: Union[service.GetTableSpecRequest, dict] = None,
+        request: Optional[Union[service.GetTableSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> table_spec.TableSpec:
         r"""Gets a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1652,19 +1665,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_table_specs(
         self,
-        request: Union[service.ListTableSpecsRequest, dict] = None,
+        request: Optional[Union[service.ListTableSpecsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListTableSpecsPager:
         r"""Lists table specs in a dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1767,19 +1780,19 @@
         )
 
         # Done; return the response.
         return response
 
     def update_table_spec(
         self,
-        request: Union[service.UpdateTableSpecRequest, dict] = None,
+        request: Optional[Union[service.UpdateTableSpecRequest, dict]] = None,
         *,
-        table_spec: gca_table_spec.TableSpec = None,
+        table_spec: Optional[gca_table_spec.TableSpec] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_table_spec.TableSpec:
         r"""Updates a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1878,19 +1891,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_column_spec(
         self,
-        request: Union[service.GetColumnSpecRequest, dict] = None,
+        request: Optional[Union[service.GetColumnSpecRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> column_spec.ColumnSpec:
         r"""Gets a column spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -1980,19 +1993,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_column_specs(
         self,
-        request: Union[service.ListColumnSpecsRequest, dict] = None,
+        request: Optional[Union[service.ListColumnSpecsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListColumnSpecsPager:
         r"""Lists column specs in a table spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2095,19 +2108,19 @@
         )
 
         # Done; return the response.
         return response
 
     def update_column_spec(
         self,
-        request: Union[service.UpdateColumnSpecRequest, dict] = None,
+        request: Optional[Union[service.UpdateColumnSpecRequest, dict]] = None,
         *,
-        column_spec: gca_column_spec.ColumnSpec = None,
+        column_spec: Optional[gca_column_spec.ColumnSpec] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gca_column_spec.ColumnSpec:
         r"""Updates a column spec.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2198,20 +2211,20 @@
         )
 
         # Done; return the response.
         return response
 
     def create_model(
         self,
-        request: Union[service.CreateModelRequest, dict] = None,
+        request: Optional[Union[service.CreateModelRequest, dict]] = None,
         *,
-        parent: str = None,
-        model: gca_model.Model = None,
+        parent: Optional[str] = None,
+        model: Optional[gca_model.Model] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Creates a model. Returns a Model in the
         [response][google.longrunning.Operation.response] field when it
         completes. When you create a model, several model evaluations
         are created for it: a global evaluation, and one evaluation for
         each annotation spec.
@@ -2328,19 +2341,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_model(
         self,
-        request: Union[service.GetModelRequest, dict] = None,
+        request: Optional[Union[service.GetModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model.Model:
         r"""Gets a model.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2428,19 +2441,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_models(
         self,
-        request: Union[service.ListModelsRequest, dict] = None,
+        request: Optional[Union[service.ListModelsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelsPager:
         r"""Lists models.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -2543,19 +2556,19 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_model(
         self,
-        request: Union[service.DeleteModelRequest, dict] = None,
+        request: Optional[Union[service.DeleteModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deletes a model. Returns ``google.protobuf.Empty`` in the
         [response][google.longrunning.Operation.response] field when it
         completes, and ``delete_details`` in the
         [metadata][google.longrunning.Operation.metadata] field.
 
@@ -2670,19 +2683,19 @@
         )
 
         # Done; return the response.
         return response
 
     def deploy_model(
         self,
-        request: Union[service.DeployModelRequest, dict] = None,
+        request: Optional[Union[service.DeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Deploys a model. If a model is already deployed, deploying it
         with the same parameters has no effect. Deploying with different
         parametrs (as e.g. changing
 
         [node_number][google.cloud.automl.v1beta1.ImageObjectDetectionModelDeploymentMetadata.node_number])
@@ -2808,19 +2821,19 @@
         )
 
         # Done; return the response.
         return response
 
     def undeploy_model(
         self,
-        request: Union[service.UndeployModelRequest, dict] = None,
+        request: Optional[Union[service.UndeployModelRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Undeploys a model. If the model is not deployed this method has
         no effect.
 
         Only applicable for Text Classification, Image Object Detection
         and Tables; all other domains manage deployment automatically.
@@ -2940,20 +2953,20 @@
         )
 
         # Done; return the response.
         return response
 
     def export_model(
         self,
-        request: Union[service.ExportModelRequest, dict] = None,
+        request: Optional[Union[service.ExportModelRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ModelExportOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ModelExportOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Exports a trained, "export-able", model to a user specified
         Google Cloud Storage location. A model is considered export-able
         if and only if it has an export format defined for it in
 
         [ModelExportOutputConfig][google.cloud.automl.v1beta1.ModelExportOutputConfig].
@@ -3084,20 +3097,20 @@
         )
 
         # Done; return the response.
         return response
 
     def export_evaluated_examples(
         self,
-        request: Union[service.ExportEvaluatedExamplesRequest, dict] = None,
+        request: Optional[Union[service.ExportEvaluatedExamplesRequest, dict]] = None,
         *,
-        name: str = None,
-        output_config: io.ExportEvaluatedExamplesOutputConfig = None,
+        name: Optional[str] = None,
+        output_config: Optional[io.ExportEvaluatedExamplesOutputConfig] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Exports examples on which the model was evaluated (i.e. which
         were in the TEST set of the dataset the model was created from),
         together with their ground truth annotations and the annotations
         created (predicted) by the model. The examples, ground truth and
         predictions are exported in the state they were at the moment
@@ -3235,19 +3248,19 @@
         )
 
         # Done; return the response.
         return response
 
     def get_model_evaluation(
         self,
-        request: Union[service.GetModelEvaluationRequest, dict] = None,
+        request: Optional[Union[service.GetModelEvaluationRequest, dict]] = None,
         *,
-        name: str = None,
+        name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> model_evaluation.ModelEvaluation:
         r"""Gets a model evaluation.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -3335,19 +3348,19 @@
         )
 
         # Done; return the response.
         return response
 
     def list_model_evaluations(
         self,
-        request: Union[service.ListModelEvaluationsRequest, dict] = None,
+        request: Optional[Union[service.ListModelEvaluationsRequest, dict]] = None,
         *,
-        parent: str = None,
+        parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListModelEvaluationsPager:
         r"""Lists model evaluations.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
@@ -3465,18 +3478,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("AutoMlClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/pagers.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/base.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
@@ -34,36 +35,31 @@
 from google.cloud.automl_v1beta1.types import model
 from google.cloud.automl_v1beta1.types import model_evaluation
 from google.cloud.automl_v1beta1.types import service
 from google.cloud.automl_v1beta1.types import table_spec
 from google.cloud.automl_v1beta1.types import table_spec as gca_table_spec
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class AutoMlTransport(abc.ABC):
     """Abstract transport class for AutoMl."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "automl.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -203,16 +203,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc_asyncio.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/auto_ml/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -113,23 +113,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/async_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -163,17 +174,17 @@
     get_transport_class = functools.partial(
         type(PredictionServiceClient).get_transport_class, type(PredictionServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, PredictionServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -209,21 +220,21 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        payload: data_items.ExamplePayload = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        payload: Optional[data_items.ExamplePayload] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_service.PredictResponse:
         r"""Perform an online prediction. The prediction result will be
         directly returned in the response. Available for following ML
         problems, and their expected request payloads:
 
         -  Image Classification - Image in .JPEG, .GIF or .PNG format,
@@ -271,15 +282,15 @@
                 # Make the request
                 response = await client.predict(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.PredictRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.PredictRequest, dict]]):
                 The request object. Request message for
                 [PredictionService.Predict][google.cloud.automl.v1beta1.PredictionService.Predict].
             name (:class:`str`):
                 Required. Name of the model requested
                 to serve the prediction.
 
                 This corresponds to the ``name`` field
@@ -290,15 +301,15 @@
                 prediction on. The payload must match
                 the problem type that the model was
                 trained to solve.
 
                 This corresponds to the ``payload`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (:class:`Mapping[str, str]`):
+            params (:class:`MutableMapping[str, str]`):
                 Additional domain-specific parameters, any string must
                 be up to 25000 characters long.
 
                 -  For Image Classification:
 
                    ``score_threshold`` - (float) A value from 0.0 to
                    1.0. When the model makes predictions for an image,
@@ -378,22 +389,22 @@
         )
 
         # Done; return the response.
         return response
 
     async def batch_predict(
         self,
-        request: Union[prediction_service.BatchPredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.BatchPredictRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.BatchPredictInputConfig = None,
-        output_config: io.BatchPredictOutputConfig = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.BatchPredictInputConfig] = None,
+        output_config: Optional[io.BatchPredictOutputConfig] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
         r"""Perform a batch prediction. Unlike the online
         [Predict][google.cloud.automl.v1beta1.PredictionService.Predict],
         batch prediction result won't be immediately available in the
         response. Instead, a long running operation object is returned.
         User can poll the operation result via
@@ -431,21 +442,21 @@
                 )
 
                 # Make the request
                 operation = client.batch_predict(request=request)
 
                 print("Waiting for operation to complete...")
 
-                response = await operation.result()
+                response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.automl_v1beta1.types.BatchPredictRequest, dict]):
+            request (Optional[Union[google.cloud.automl_v1beta1.types.BatchPredictRequest, dict]]):
                 The request object. Request message for
                 [PredictionService.BatchPredict][google.cloud.automl.v1beta1.PredictionService.BatchPredict].
             name (:class:`str`):
                 Required. Name of the model requested
                 to serve the batch prediction.
 
                 This corresponds to the ``name`` field
@@ -462,15 +473,15 @@
                 Required. The Configuration
                 specifying where output predictions
                 should be written.
 
                 This corresponds to the ``output_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (:class:`Mapping[str, str]`):
+            params (:class:`MutableMapping[str, str]`):
                 Required. Additional domain-specific parameters for the
                 predictions, any string must be up to 25000 characters
                 long.
 
                 -  For Text Classification:
 
                    ``score_threshold`` - (float) A value from 0.0 to
@@ -630,18 +641,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceAsyncClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -58,15 +70,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[PredictionServiceTransport]]
     _transport_registry["grpc"] = PredictionServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = PredictionServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[PredictionServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -337,30 +349,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, PredictionServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, PredictionServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the prediction service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, PredictionServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -382,14 +394,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -434,21 +447,21 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def predict(
         self,
-        request: Union[prediction_service.PredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.PredictRequest, dict]] = None,
         *,
-        name: str = None,
-        payload: data_items.ExamplePayload = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        payload: Optional[data_items.ExamplePayload] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> prediction_service.PredictResponse:
         r"""Perform an online prediction. The prediction result will be
         directly returned in the response. Available for following ML
         problems, and their expected request payloads:
 
         -  Image Classification - Image in .JPEG, .GIF or .PNG format,
@@ -515,15 +528,15 @@
                 prediction on. The payload must match
                 the problem type that the model was
                 trained to solve.
 
                 This corresponds to the ``payload`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (Mapping[str, str]):
+            params (MutableMapping[str, str]):
                 Additional domain-specific parameters, any string must
                 be up to 25000 characters long.
 
                 -  For Image Classification:
 
                    ``score_threshold`` - (float) A value from 0.0 to
                    1.0. When the model makes predictions for an image,
@@ -602,22 +615,22 @@
         )
 
         # Done; return the response.
         return response
 
     def batch_predict(
         self,
-        request: Union[prediction_service.BatchPredictRequest, dict] = None,
+        request: Optional[Union[prediction_service.BatchPredictRequest, dict]] = None,
         *,
-        name: str = None,
-        input_config: io.BatchPredictInputConfig = None,
-        output_config: io.BatchPredictOutputConfig = None,
-        params: Mapping[str, str] = None,
+        name: Optional[str] = None,
+        input_config: Optional[io.BatchPredictInputConfig] = None,
+        output_config: Optional[io.BatchPredictOutputConfig] = None,
+        params: Optional[MutableMapping[str, str]] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
         r"""Perform a batch prediction. Unlike the online
         [Predict][google.cloud.automl.v1beta1.PredictionService.Predict],
         batch prediction result won't be immediately available in the
         response. Instead, a long running operation object is returned.
         User can poll the operation result via
@@ -686,15 +699,15 @@
                 Required. The Configuration
                 specifying where output predictions
                 should be written.
 
                 This corresponds to the ``output_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            params (Mapping[str, str]):
+            params (MutableMapping[str, str]):
                 Required. Additional domain-specific parameters for the
                 predictions, any string must be up to 25000 characters
                 long.
 
                 -  For Text Classification:
 
                    ``score_threshold`` - (float) A value from 0.0 to
@@ -860,18 +873,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("PredictionServiceClient",)
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/base.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,50 +11,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.automl_v1beta1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core import operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.automl_v1beta1.types import prediction_service
 from google.longrunning import operations_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-cloud-automl",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class PredictionServiceTransport(abc.ABC):
     """Abstract transport class for PredictionService."""
 
     AUTH_SCOPES = ("https://www.googleapis.com/auth/cloud-platform",)
 
     DEFAULT_HOST: str = "automl.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -183,16 +183,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc_asyncio.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/prediction_service/transports/grpc_asyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -93,23 +93,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "automl.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/gcs_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/gcs_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/services/tables/tables_client.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/services/tables/tables_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/__init__.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/annotation_payload.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/annotation_payload.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import classification as gca_classification
 from google.cloud.automl_v1beta1.types import detection
 from google.cloud.automl_v1beta1.types import tables as gca_tables
 from google.cloud.automl_v1beta1.types import text_extraction as gca_text_extraction
 from google.cloud.automl_v1beta1.types import text_sentiment as gca_text_sentiment
@@ -89,66 +91,68 @@
             when the model was trained. Because this field returns a
             value at model training time, for different models trained
             using the same dataset, the returned value could be
             different as model owner could update the ``display_name``
             between any two model training.
     """
 
-    translation = proto.Field(
+    translation: gca_translation.TranslationAnnotation = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="detail",
         message=gca_translation.TranslationAnnotation,
     )
-    classification = proto.Field(
+    classification: gca_classification.ClassificationAnnotation = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="detail",
         message=gca_classification.ClassificationAnnotation,
     )
-    image_object_detection = proto.Field(
+    image_object_detection: detection.ImageObjectDetectionAnnotation = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="detail",
         message=detection.ImageObjectDetectionAnnotation,
     )
-    video_classification = proto.Field(
-        proto.MESSAGE,
-        number=9,
-        oneof="detail",
-        message=gca_classification.VideoClassificationAnnotation,
+    video_classification: gca_classification.VideoClassificationAnnotation = (
+        proto.Field(
+            proto.MESSAGE,
+            number=9,
+            oneof="detail",
+            message=gca_classification.VideoClassificationAnnotation,
+        )
     )
-    video_object_tracking = proto.Field(
+    video_object_tracking: detection.VideoObjectTrackingAnnotation = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="detail",
         message=detection.VideoObjectTrackingAnnotation,
     )
-    text_extraction = proto.Field(
+    text_extraction: gca_text_extraction.TextExtractionAnnotation = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="detail",
         message=gca_text_extraction.TextExtractionAnnotation,
     )
-    text_sentiment = proto.Field(
+    text_sentiment: gca_text_sentiment.TextSentimentAnnotation = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="detail",
         message=gca_text_sentiment.TextSentimentAnnotation,
     )
-    tables = proto.Field(
+    tables: gca_tables.TablesAnnotation = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="detail",
         message=gca_tables.TablesAnnotation,
     )
-    annotation_spec_id = proto.Field(
+    annotation_spec_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/annotation_spec.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/annotation_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,50 +9,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.automl.v1beta1",
+    package="google.cloud.automl.v1",
     manifest={
         "AnnotationSpec",
     },
 )
 
 
 class AnnotationSpec(proto.Message):
     r"""A definition of an annotation spec.
 
     Attributes:
         name (str):
             Output only. Resource name of the annotation spec. Form:
-
             'projects/{project_id}/locations/{location_id}/datasets/{dataset_id}/annotationSpecs/{annotation_spec_id}'
         display_name (str):
             Required. The name of the annotation spec to show in the
             interface. The name can be up to 32 characters long and must
             match the regexp ``[a-zA-Z0-9_]+``.
         example_count (int):
             Output only. The number of examples in the
             parent dataset labeled by the annotation spec.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    example_count = proto.Field(
+    example_count: int = proto.Field(
         proto.INT32,
         number=9,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/classification.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import temporal
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -46,15 +48,15 @@
             confidence that the annotation is positive. If a
             user approves an annotation as negative or
             positive, the score value remains unchanged. If
             a user creates an annotation, the score is 0 for
             negative or 1 for positive.
     """
 
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
 
 
 class VideoClassificationAnnotation(proto.Message):
     r"""Contains annotation details specific to video classification.
@@ -92,24 +94,24 @@
             Output only . The classification details of
             this annotation.
         time_segment (google.cloud.automl_v1beta1.types.TimeSegment):
             Output only . The time segment of the video
             to which the annotation applies.
     """
 
-    type_ = proto.Field(
+    type_: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    classification_annotation = proto.Field(
+    classification_annotation: "ClassificationAnnotation" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="ClassificationAnnotation",
     )
-    time_segment = proto.Field(
+    time_segment: temporal.TimeSegment = proto.Field(
         proto.MESSAGE,
         number=3,
         message=temporal.TimeSegment,
     )
 
 
 class ClassificationEvaluationMetrics(proto.Message):
@@ -128,30 +130,30 @@
             the overall evaluation. Deprecated.
         au_roc (float):
             Output only. The Area Under Receiver
             Operating Characteristic curve metric.
             Micro-averaged for the overall evaluation.
         log_loss (float):
             Output only. The Log Loss metric.
-        confidence_metrics_entry (Sequence[google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfidenceMetricsEntry]):
+        confidence_metrics_entry (MutableSequence[google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfidenceMetricsEntry]):
             Output only. Metrics for each confidence_threshold in
             0.00,0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 and
             position_threshold = INT32_MAX_VALUE. ROC and
             precision-recall curves, and other aggregated metrics are
             derived from them. The confidence metrics entries may also
             be supplied for additional values of position_threshold, but
             from these no aggregated metrics are computed.
         confusion_matrix (google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
             Output only. Confusion matrix of the
             evaluation. Only set for MULTICLASS
             classification problems where number of labels
             is no more than 10.
             Only set for model level evaluation, not for
             evaluation per label.
-        annotation_spec_id (Sequence[str]):
+        annotation_spec_id (MutableSequence[str]):
             Output only. The annotation spec ids used for
             this evaluation.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
         r"""Metrics for a single confidence threshold.
 
@@ -209,158 +211,162 @@
                 label.
             true_negative_count (int):
                 Output only. The number of labels that were
                 not created by the model, but if they would,
                 they would not match a ground truth label.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        position_threshold = proto.Field(
+        position_threshold: int = proto.Field(
             proto.INT32,
             number=14,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        false_positive_rate = proto.Field(
+        false_positive_rate: float = proto.Field(
             proto.FLOAT,
             number=8,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
-        recall_at1 = proto.Field(
+        recall_at1: float = proto.Field(
             proto.FLOAT,
             number=5,
         )
-        precision_at1 = proto.Field(
+        precision_at1: float = proto.Field(
             proto.FLOAT,
             number=6,
         )
-        false_positive_rate_at1 = proto.Field(
+        false_positive_rate_at1: float = proto.Field(
             proto.FLOAT,
             number=9,
         )
-        f1_score_at1 = proto.Field(
+        f1_score_at1: float = proto.Field(
             proto.FLOAT,
             number=7,
         )
-        true_positive_count = proto.Field(
+        true_positive_count: int = proto.Field(
             proto.INT64,
             number=10,
         )
-        false_positive_count = proto.Field(
+        false_positive_count: int = proto.Field(
             proto.INT64,
             number=11,
         )
-        false_negative_count = proto.Field(
+        false_negative_count: int = proto.Field(
             proto.INT64,
             number=12,
         )
-        true_negative_count = proto.Field(
+        true_negative_count: int = proto.Field(
             proto.INT64,
             number=13,
         )
 
     class ConfusionMatrix(proto.Message):
         r"""Confusion matrix of the model running the classification.
 
         Attributes:
-            annotation_spec_id (Sequence[str]):
+            annotation_spec_id (MutableSequence[str]):
                 Output only. IDs of the annotation specs used in the
                 confusion matrix. For Tables CLASSIFICATION
 
                 [prediction_type][google.cloud.automl.v1beta1.TablesModelMetadata.prediction_type]
                 only list of [annotation_spec_display_name-s][] is
                 populated.
-            display_name (Sequence[str]):
+            display_name (MutableSequence[str]):
                 Output only. Display name of the annotation specs used in
                 the confusion matrix, as they were at the moment of the
                 evaluation. For Tables CLASSIFICATION
 
                 [prediction_type-s][google.cloud.automl.v1beta1.TablesModelMetadata.prediction_type],
                 distinct values of the target column at the moment of the
                 model evaluation are populated here.
-            row (Sequence[google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfusionMatrix.Row]):
+            row (MutableSequence[google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfusionMatrix.Row]):
                 Output only. Rows in the confusion matrix. The number of
                 rows is equal to the size of ``annotation_spec_id``.
                 ``row[i].example_count[j]`` is the number of examples that
                 have ground truth of the ``annotation_spec_id[i]`` and are
                 predicted as ``annotation_spec_id[j]`` by the model being
                 evaluated.
         """
 
         class Row(proto.Message):
             r"""Output only. A row in the confusion matrix.
 
             Attributes:
-                example_count (Sequence[int]):
+                example_count (MutableSequence[int]):
                     Output only. Value of the specific cell in the confusion
                     matrix. The number of values each row has (i.e. the length
                     of the row) is equal to the length of the
                     ``annotation_spec_id`` field or, if that one is not
                     populated, length of the
                     [display_name][google.cloud.automl.v1beta1.ClassificationEvaluationMetrics.ConfusionMatrix.display_name]
                     field.
             """
 
-            example_count = proto.RepeatedField(
+            example_count: MutableSequence[int] = proto.RepeatedField(
                 proto.INT32,
                 number=1,
             )
 
-        annotation_spec_id = proto.RepeatedField(
+        annotation_spec_id: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=1,
         )
-        display_name = proto.RepeatedField(
+        display_name: MutableSequence[str] = proto.RepeatedField(
             proto.STRING,
             number=3,
         )
-        row = proto.RepeatedField(
+        row: MutableSequence[
+            "ClassificationEvaluationMetrics.ConfusionMatrix.Row"
+        ] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message="ClassificationEvaluationMetrics.ConfusionMatrix.Row",
         )
 
-    au_prc = proto.Field(
+    au_prc: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    base_au_prc = proto.Field(
+    base_au_prc: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    au_roc = proto.Field(
+    au_roc: float = proto.Field(
         proto.FLOAT,
         number=6,
     )
-    log_loss = proto.Field(
+    log_loss: float = proto.Field(
         proto.FLOAT,
         number=7,
     )
-    confidence_metrics_entry = proto.RepeatedField(
+    confidence_metrics_entry: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ConfidenceMetricsEntry,
     )
-    confusion_matrix = proto.Field(
+    confusion_matrix: ConfusionMatrix = proto.Field(
         proto.MESSAGE,
         number=4,
         message=ConfusionMatrix,
     )
-    annotation_spec_id = proto.RepeatedField(
+    annotation_spec_id: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=5,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/column_spec.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/column_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import data_stats as gca_data_stats
 from google.cloud.automl_v1beta1.types import data_types
 
 
 __protobuf__ = proto.module(
@@ -49,15 +51,15 @@
             digits 0-9, underscores(_), and forward slashes(/), and must
             start with a letter or a digit.
         data_stats (google.cloud.automl_v1beta1.types.DataStats):
             Output only. Stats of the series of values in the column.
             This field may be stale, see the ancestor's
             Dataset.tables_dataset_metadata.stats_update_time field for
             the timestamp at which these stats were last updated.
-        top_correlated_columns (Sequence[google.cloud.automl_v1beta1.types.ColumnSpec.CorrelatedColumn]):
+        top_correlated_columns (MutableSequence[google.cloud.automl_v1beta1.types.ColumnSpec.CorrelatedColumn]):
             Deprecated.
         etag (str):
             Used to perform consistent read-modify-write
             updates. If not set, a blind "overwrite" update
             happens.
     """
 
@@ -70,47 +72,47 @@
                 The column_spec_id of the correlated column, which belongs
                 to the same table as the in-context column.
             correlation_stats (google.cloud.automl_v1beta1.types.CorrelationStats):
                 Correlation between this and the in-context
                 column.
         """
 
-        column_spec_id = proto.Field(
+        column_spec_id: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        correlation_stats = proto.Field(
+        correlation_stats: gca_data_stats.CorrelationStats = proto.Field(
             proto.MESSAGE,
             number=2,
             message=gca_data_stats.CorrelationStats,
         )
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    data_type = proto.Field(
+    data_type: data_types.DataType = proto.Field(
         proto.MESSAGE,
         number=2,
         message=data_types.DataType,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    data_stats = proto.Field(
+    data_stats: gca_data_stats.DataStats = proto.Field(
         proto.MESSAGE,
         number=4,
         message=gca_data_stats.DataStats,
     )
-    top_correlated_columns = proto.RepeatedField(
+    top_correlated_columns: MutableSequence[CorrelatedColumn] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message=CorrelatedColumn,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_items.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_items.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import geometry
 from google.cloud.automl_v1beta1.types import io
 from google.cloud.automl_v1beta1.types import text_segment as gca_text_segment
 from google.protobuf import struct_pb2  # type: ignore
 
@@ -57,26 +59,26 @@
             image.
 
             This field is a member of `oneof`_ ``data``.
         thumbnail_uri (str):
             Output only. HTTP URI to the thumbnail image.
     """
 
-    image_bytes = proto.Field(
+    image_bytes: bytes = proto.Field(
         proto.BYTES,
         number=1,
         oneof="data",
     )
-    input_config = proto.Field(
+    input_config: io.InputConfig = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="data",
         message=io.InputConfig,
     )
-    thumbnail_uri = proto.Field(
+    thumbnail_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class TextSnippet(proto.Message):
     r"""A representation of a text snippet.
@@ -93,23 +95,23 @@
             determined from the type of the uploaded
             [content][google.cloud.automl.v1beta1.TextSnippet.content].
         content_uri (str):
             Output only. HTTP URI where you can download
             the content.
     """
 
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    mime_type = proto.Field(
+    mime_type: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    content_uri = proto.Field(
+    content_uri: str = proto.Field(
         proto.STRING,
         number=4,
     )
 
 
 class DocumentDimensions(proto.Message):
     r"""Message that describes dimension of a document.
@@ -128,39 +130,39 @@
     class DocumentDimensionUnit(proto.Enum):
         r"""Unit of the document dimension."""
         DOCUMENT_DIMENSION_UNIT_UNSPECIFIED = 0
         INCH = 1
         CENTIMETER = 2
         POINT = 3
 
-    unit = proto.Field(
+    unit: DocumentDimensionUnit = proto.Field(
         proto.ENUM,
         number=1,
         enum=DocumentDimensionUnit,
     )
-    width = proto.Field(
+    width: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    height = proto.Field(
+    height: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 class Document(proto.Message):
     r"""A structured text document e.g. a PDF.
 
     Attributes:
         input_config (google.cloud.automl_v1beta1.types.DocumentInputConfig):
             An input config specifying the content of the
             document.
         document_text (google.cloud.automl_v1beta1.types.TextSnippet):
             The plain text version of this document.
-        layout (Sequence[google.cloud.automl_v1beta1.types.Document.Layout]):
+        layout (MutableSequence[google.cloud.automl_v1beta1.types.Document.Layout]):
             Describes the layout of the document. Sorted by
             [page_number][].
         document_dimensions (google.cloud.automl_v1beta1.types.DocumentDimensions):
             The dimensions of the page in the document.
         page_count (int):
             Number of pages in the document.
     """
@@ -206,87 +208,87 @@
             FORM_FIELD_NAME = 4
             FORM_FIELD_CONTENTS = 5
             TABLE = 6
             TABLE_HEADER = 7
             TABLE_ROW = 8
             TABLE_CELL = 9
 
-        text_segment = proto.Field(
+        text_segment: gca_text_segment.TextSegment = proto.Field(
             proto.MESSAGE,
             number=1,
             message=gca_text_segment.TextSegment,
         )
-        page_number = proto.Field(
+        page_number: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        bounding_poly = proto.Field(
+        bounding_poly: geometry.BoundingPoly = proto.Field(
             proto.MESSAGE,
             number=3,
             message=geometry.BoundingPoly,
         )
-        text_segment_type = proto.Field(
+        text_segment_type: "Document.Layout.TextSegmentType" = proto.Field(
             proto.ENUM,
             number=4,
             enum="Document.Layout.TextSegmentType",
         )
 
-    input_config = proto.Field(
+    input_config: io.DocumentInputConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=io.DocumentInputConfig,
     )
-    document_text = proto.Field(
+    document_text: "TextSnippet" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="TextSnippet",
     )
-    layout = proto.RepeatedField(
+    layout: MutableSequence[Layout] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=Layout,
     )
-    document_dimensions = proto.Field(
+    document_dimensions: "DocumentDimensions" = proto.Field(
         proto.MESSAGE,
         number=4,
         message="DocumentDimensions",
     )
-    page_count = proto.Field(
+    page_count: int = proto.Field(
         proto.INT32,
         number=5,
     )
 
 
 class Row(proto.Message):
     r"""A representation of a row in a relational table.
 
     Attributes:
-        column_spec_ids (Sequence[str]):
+        column_spec_ids (MutableSequence[str]):
             The resource IDs of the column specs describing the columns
             of the row. If set must contain, but possibly in a different
             order, all input feature
 
             [column_spec_ids][google.cloud.automl.v1beta1.TablesModelMetadata.input_feature_column_specs]
             of the Model this row is being passed to. Note: The below
             ``values`` field must match order of this field, if this
             field is set.
-        values (Sequence[google.protobuf.struct_pb2.Value]):
+        values (MutableSequence[google.protobuf.struct_pb2.Value]):
             Required. The values of the row cells, given in the same
             order as the column_spec_ids, or, if not set, then in the
             same order as input feature
 
             [column_specs][google.cloud.automl.v1beta1.TablesModelMetadata.input_feature_column_specs]
             of the Model this row is being passed to.
     """
 
-    column_spec_ids = proto.RepeatedField(
+    column_spec_ids: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=2,
     )
-    values = proto.RepeatedField(
+    values: MutableSequence[struct_pb2.Value] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=struct_pb2.Value,
     )
 
 
 class ExamplePayload(proto.Message):
@@ -314,33 +316,33 @@
             This field is a member of `oneof`_ ``payload``.
         row (google.cloud.automl_v1beta1.types.Row):
             Example relational table row.
 
             This field is a member of `oneof`_ ``payload``.
     """
 
-    image = proto.Field(
+    image: "Image" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="payload",
         message="Image",
     )
-    text_snippet = proto.Field(
+    text_snippet: "TextSnippet" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="payload",
         message="TextSnippet",
     )
-    document = proto.Field(
+    document: "Document" = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="payload",
         message="Document",
     )
-    row = proto.Field(
+    row: "Row" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="payload",
         message="Row",
     )
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_stats.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "DataStats",
@@ -71,78 +73,78 @@
             The number of distinct values.
         null_value_count (int):
             The number of values that are null.
         valid_value_count (int):
             The number of values that are valid.
     """
 
-    float64_stats = proto.Field(
+    float64_stats: "Float64Stats" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="stats",
         message="Float64Stats",
     )
-    string_stats = proto.Field(
+    string_stats: "StringStats" = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="stats",
         message="StringStats",
     )
-    timestamp_stats = proto.Field(
+    timestamp_stats: "TimestampStats" = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="stats",
         message="TimestampStats",
     )
-    array_stats = proto.Field(
+    array_stats: "ArrayStats" = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="stats",
         message="ArrayStats",
     )
-    struct_stats = proto.Field(
+    struct_stats: "StructStats" = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="stats",
         message="StructStats",
     )
-    category_stats = proto.Field(
+    category_stats: "CategoryStats" = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="stats",
         message="CategoryStats",
     )
-    distinct_value_count = proto.Field(
+    distinct_value_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    null_value_count = proto.Field(
+    null_value_count: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    valid_value_count = proto.Field(
+    valid_value_count: int = proto.Field(
         proto.INT64,
         number=9,
     )
 
 
 class Float64Stats(proto.Message):
     r"""The data statistics of a series of FLOAT64 values.
 
     Attributes:
         mean (float):
             The mean of the series.
         standard_deviation (float):
             The standard deviation of the series.
-        quantiles (Sequence[float]):
+        quantiles (MutableSequence[float]):
             Ordered from 0 to k k-quantile values of the data series of
             n values. The value at index i is, approximately, the
             i*n/k-th smallest value in the series; for i = 0 and i = k
             these are, respectively, the min and max values.
-        histogram_buckets (Sequence[google.cloud.automl_v1beta1.types.Float64Stats.HistogramBucket]):
+        histogram_buckets (MutableSequence[google.cloud.automl_v1beta1.types.Float64Stats.HistogramBucket]):
             Histogram buckets of the data series. Sorted by the min
             value of the bucket, ascendingly, and the number of the
             buckets is dynamically generated. The buckets are
             non-overlapping and completely cover whole FLOAT64 range
             with min of first bucket being ``"-Infinity"``, and max of
             the last one being ``"Infinity"``.
     """
@@ -157,51 +159,51 @@
                 The maximum value of the bucket, exclusive unless max =
                 ``"Infinity"``, in which case it's inclusive.
             count (int):
                 The number of data values that are in the
                 bucket, i.e. are between min and max values.
         """
 
-        min_ = proto.Field(
+        min_: float = proto.Field(
             proto.DOUBLE,
             number=1,
         )
-        max_ = proto.Field(
+        max_: float = proto.Field(
             proto.DOUBLE,
             number=2,
         )
-        count = proto.Field(
+        count: int = proto.Field(
             proto.INT64,
             number=3,
         )
 
-    mean = proto.Field(
+    mean: float = proto.Field(
         proto.DOUBLE,
         number=1,
     )
-    standard_deviation = proto.Field(
+    standard_deviation: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
-    quantiles = proto.RepeatedField(
+    quantiles: MutableSequence[float] = proto.RepeatedField(
         proto.DOUBLE,
         number=3,
     )
-    histogram_buckets = proto.RepeatedField(
+    histogram_buckets: MutableSequence[HistogramBucket] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message=HistogramBucket,
     )
 
 
 class StringStats(proto.Message):
     r"""The data statistics of a series of STRING values.
 
     Attributes:
-        top_unigram_stats (Sequence[google.cloud.automl_v1beta1.types.StringStats.UnigramStats]):
+        top_unigram_stats (MutableSequence[google.cloud.automl_v1beta1.types.StringStats.UnigramStats]):
             The statistics of the top 20 unigrams, ordered by
             [count][google.cloud.automl.v1beta1.StringStats.UnigramStats.count].
     """
 
     class UnigramStats(proto.Message):
         r"""The statistics of a unigram.
 
@@ -209,59 +211,59 @@
             value (str):
                 The unigram.
             count (int):
                 The number of occurrences of this unigram in
                 the series.
         """
 
-        value = proto.Field(
+        value: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        count = proto.Field(
+        count: int = proto.Field(
             proto.INT64,
             number=2,
         )
 
-    top_unigram_stats = proto.RepeatedField(
+    top_unigram_stats: MutableSequence[UnigramStats] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=UnigramStats,
     )
 
 
 class TimestampStats(proto.Message):
     r"""The data statistics of a series of TIMESTAMP values.
 
     Attributes:
-        granular_stats (Mapping[str, google.cloud.automl_v1beta1.types.TimestampStats.GranularStats]):
+        granular_stats (MutableMapping[str, google.cloud.automl_v1beta1.types.TimestampStats.GranularStats]):
             The string key is the pre-defined granularity. Currently
             supported: hour_of_day, day_of_week, month_of_year.
             Granularities finer that the granularity of timestamp data
             are not populated (e.g. if timestamps are at day
             granularity, then hour_of_day is not populated).
     """
 
     class GranularStats(proto.Message):
         r"""Stats split by a defined in context granularity.
 
         Attributes:
-            buckets (Mapping[int, int]):
+            buckets (MutableMapping[int, int]):
                 A map from granularity key to example count for that key.
                 E.g. for hour_of_day ``13`` means 1pm, or for month_of_year
                 ``5`` means May).
         """
 
-        buckets = proto.MapField(
+        buckets: MutableMapping[int, int] = proto.MapField(
             proto.INT32,
             proto.INT64,
             number=1,
         )
 
-    granular_stats = proto.MapField(
+    granular_stats: MutableMapping[str, GranularStats] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=1,
         message=GranularStats,
     )
 
 
@@ -271,44 +273,44 @@
     Attributes:
         member_stats (google.cloud.automl_v1beta1.types.DataStats):
             Stats of all the values of all arrays, as if
             they were a single long series of data. The type
             depends on the element type of the array.
     """
 
-    member_stats = proto.Field(
+    member_stats: "DataStats" = proto.Field(
         proto.MESSAGE,
         number=2,
         message="DataStats",
     )
 
 
 class StructStats(proto.Message):
     r"""The data statistics of a series of STRUCT values.
 
     Attributes:
-        field_stats (Mapping[str, google.cloud.automl_v1beta1.types.DataStats]):
+        field_stats (MutableMapping[str, google.cloud.automl_v1beta1.types.DataStats]):
             Map from a field name of the struct to data
             stats aggregated over series of all data in that
             field across all the structs.
     """
 
-    field_stats = proto.MapField(
+    field_stats: MutableMapping[str, "DataStats"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=1,
         message="DataStats",
     )
 
 
 class CategoryStats(proto.Message):
     r"""The data statistics of a series of CATEGORY values.
 
     Attributes:
-        top_category_stats (Sequence[google.cloud.automl_v1beta1.types.CategoryStats.SingleCategoryStats]):
+        top_category_stats (MutableSequence[google.cloud.automl_v1beta1.types.CategoryStats.SingleCategoryStats]):
             The statistics of the top 20 CATEGORY values, ordered by
 
             [count][google.cloud.automl.v1beta1.CategoryStats.SingleCategoryStats.count].
     """
 
     class SingleCategoryStats(proto.Message):
         r"""The statistics of a single CATEGORY value.
@@ -317,24 +319,24 @@
             value (str):
                 The CATEGORY value.
             count (int):
                 The number of occurrences of this value in
                 the series.
         """
 
-        value = proto.Field(
+        value: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        count = proto.Field(
+        count: int = proto.Field(
             proto.INT64,
             number=2,
         )
 
-    top_category_stats = proto.RepeatedField(
+    top_category_stats: MutableSequence[SingleCategoryStats] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=SingleCategoryStats,
     )
 
 
 class CorrelationStats(proto.Message):
@@ -344,14 +346,14 @@
 
     Attributes:
         cramers_v (float):
             The correlation value using the Cramer's V
             measure.
     """
 
-    cramers_v = proto.Field(
+    cramers_v: float = proto.Field(
         proto.DOUBLE,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/data_types.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/data_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "TypeCode",
@@ -89,55 +91,55 @@
             [TypeCode][google.cloud.automl.v1beta1.TypeCode] for this
             type.
         nullable (bool):
             If true, this DataType can also be ``NULL``. In .CSV files
             ``NULL`` value is expressed as an empty string.
     """
 
-    list_element_type = proto.Field(
+    list_element_type: "DataType" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="details",
         message="DataType",
     )
-    struct_type = proto.Field(
+    struct_type: "StructType" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="details",
         message="StructType",
     )
-    time_format = proto.Field(
+    time_format: str = proto.Field(
         proto.STRING,
         number=5,
         oneof="details",
     )
-    type_code = proto.Field(
+    type_code: "TypeCode" = proto.Field(
         proto.ENUM,
         number=1,
         enum="TypeCode",
     )
-    nullable = proto.Field(
+    nullable: bool = proto.Field(
         proto.BOOL,
         number=4,
     )
 
 
 class StructType(proto.Message):
     r"""``StructType`` defines the DataType-s of a
     [STRUCT][google.cloud.automl.v1beta1.TypeCode.STRUCT] type.
 
     Attributes:
-        fields (Mapping[str, google.cloud.automl_v1beta1.types.DataType]):
+        fields (MutableMapping[str, google.cloud.automl_v1beta1.types.DataType]):
             Unordered map of struct field names to their
             data types. Fields cannot be added or removed
             via Update. Their names and data types are still
             mutable.
     """
 
-    fields = proto.MapField(
+    fields: MutableMapping[str, "DataType"] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=1,
         message="DataType",
     )
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/dataset.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import image
 from google.cloud.automl_v1beta1.types import tables
 from google.cloud.automl_v1beta1.types import text
 from google.cloud.automl_v1beta1.types import translation
 from google.cloud.automl_v1beta1.types import video
@@ -106,89 +108,97 @@
             created.
         etag (str):
             Used to perform consistent read-modify-write
             updates. If not set, a blind "overwrite" update
             happens.
     """
 
-    translation_dataset_metadata = proto.Field(
+    translation_dataset_metadata: translation.TranslationDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=23,
         oneof="dataset_metadata",
         message=translation.TranslationDatasetMetadata,
     )
-    image_classification_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=24,
-        oneof="dataset_metadata",
-        message=image.ImageClassificationDatasetMetadata,
-    )
-    text_classification_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=25,
-        oneof="dataset_metadata",
-        message=text.TextClassificationDatasetMetadata,
+    image_classification_dataset_metadata: image.ImageClassificationDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=24,
+            oneof="dataset_metadata",
+            message=image.ImageClassificationDatasetMetadata,
+        )
+    )
+    text_classification_dataset_metadata: text.TextClassificationDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=25,
+            oneof="dataset_metadata",
+            message=text.TextClassificationDatasetMetadata,
+        )
     )
-    image_object_detection_dataset_metadata = proto.Field(
+    image_object_detection_dataset_metadata: image.ImageObjectDetectionDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=26,
         oneof="dataset_metadata",
         message=image.ImageObjectDetectionDatasetMetadata,
     )
-    video_classification_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=31,
-        oneof="dataset_metadata",
-        message=video.VideoClassificationDatasetMetadata,
-    )
-    video_object_tracking_dataset_metadata = proto.Field(
-        proto.MESSAGE,
-        number=29,
-        oneof="dataset_metadata",
-        message=video.VideoObjectTrackingDatasetMetadata,
+    video_classification_dataset_metadata: video.VideoClassificationDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=31,
+            oneof="dataset_metadata",
+            message=video.VideoClassificationDatasetMetadata,
+        )
+    )
+    video_object_tracking_dataset_metadata: video.VideoObjectTrackingDatasetMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=29,
+            oneof="dataset_metadata",
+            message=video.VideoObjectTrackingDatasetMetadata,
+        )
     )
-    text_extraction_dataset_metadata = proto.Field(
+    text_extraction_dataset_metadata: text.TextExtractionDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=28,
         oneof="dataset_metadata",
         message=text.TextExtractionDatasetMetadata,
     )
-    text_sentiment_dataset_metadata = proto.Field(
+    text_sentiment_dataset_metadata: text.TextSentimentDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=30,
         oneof="dataset_metadata",
         message=text.TextSentimentDatasetMetadata,
     )
-    tables_dataset_metadata = proto.Field(
+    tables_dataset_metadata: tables.TablesDatasetMetadata = proto.Field(
         proto.MESSAGE,
         number=33,
         oneof="dataset_metadata",
         message=tables.TablesDatasetMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    description = proto.Field(
+    description: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    example_count = proto.Field(
+    example_count: int = proto.Field(
         proto.INT32,
         number=21,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=14,
         message=timestamp_pb2.Timestamp,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=17,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/detection.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import geometry
 from google.protobuf import duration_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -40,20 +42,20 @@
             object location.
         score (float):
             Output only. The confidence that this annotation is positive
             for the parent example, value in [0, 1], higher means higher
             positivity confidence.
     """
 
-    bounding_box = proto.Field(
+    bounding_box: geometry.BoundingPoly = proto.Field(
         proto.MESSAGE,
         number=1,
         message=geometry.BoundingPoly,
     )
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class VideoObjectTrackingAnnotation(proto.Message):
     r"""Annotation details for video object tracking.
@@ -82,29 +84,29 @@
             for the video at the time_offset, value in [0, 1], higher
             means higher positivity confidence. For annotations created
             by the user the score is 1. When user approves an
             annotation, the original float score is kept (and not
             changed to 1).
     """
 
-    instance_id = proto.Field(
+    instance_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    time_offset = proto.Field(
+    time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
-    bounding_box = proto.Field(
+    bounding_box: geometry.BoundingPoly = proto.Field(
         proto.MESSAGE,
         number=3,
         message=geometry.BoundingPoly,
     )
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
 
 
 class BoundingBoxMetricsEntry(proto.Message):
     r"""Bounding box matching model metrics for a single
@@ -115,15 +117,15 @@
         iou_threshold (float):
             Output only. The intersection-over-union
             threshold value used to compute this metrics
             entry.
         mean_average_precision (float):
             Output only. The mean average precision, most often close to
             au_prc.
-        confidence_metrics_entries (Sequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry.ConfidenceMetricsEntry]):
+        confidence_metrics_entries (MutableSequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry.ConfidenceMetricsEntry]):
             Output only. Metrics for each label-match
             confidence_threshold from
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99. Precision-recall
             curve is derived from them.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
@@ -140,40 +142,42 @@
                 Output only. Precision under the given
                 confidence threshold.
             f1_score (float):
                 Output only. The harmonic mean of recall and
                 precision.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=2,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
 
-    iou_threshold = proto.Field(
+    iou_threshold: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    mean_average_precision = proto.Field(
+    mean_average_precision: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    confidence_metrics_entries = proto.RepeatedField(
+    confidence_metrics_entries: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=ConfidenceMetricsEntry,
     )
 
 
 class ImageObjectDetectionEvaluationMetrics(proto.Message):
@@ -181,36 +185,38 @@
     Evaluates prediction quality of labeled bounding boxes.
 
     Attributes:
         evaluated_bounding_box_count (int):
             Output only. The total number of bounding
             boxes (i.e. summed over all images) the ground
             truth used to create this evaluation had.
-        bounding_box_metrics_entries (Sequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry]):
+        bounding_box_metrics_entries (MutableSequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry]):
             Output only. The bounding boxes match metrics
             for each Intersection-over-union threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 and each
             label confidence threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 pair.
         bounding_box_mean_average_precision (float):
             Output only. The single metric for bounding boxes
             evaluation: the mean_average_precision averaged over all
             bounding_box_metrics_entries.
     """
 
-    evaluated_bounding_box_count = proto.Field(
+    evaluated_bounding_box_count: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    bounding_box_metrics_entries = proto.RepeatedField(
+    bounding_box_metrics_entries: MutableSequence[
+        "BoundingBoxMetricsEntry"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="BoundingBoxMetricsEntry",
     )
-    bounding_box_mean_average_precision = proto.Field(
+    bounding_box_mean_average_precision: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 class VideoObjectTrackingEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for video object tracking problems.
@@ -222,39 +228,41 @@
         evaluated_frame_count (int):
             Output only. The number of video frames used
             to create this evaluation.
         evaluated_bounding_box_count (int):
             Output only. The total number of bounding
             boxes (i.e. summed over all frames) the ground
             truth used to create this evaluation had.
-        bounding_box_metrics_entries (Sequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry]):
+        bounding_box_metrics_entries (MutableSequence[google.cloud.automl_v1beta1.types.BoundingBoxMetricsEntry]):
             Output only. The bounding boxes match metrics
             for each Intersection-over-union threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 and each
             label confidence threshold
             0.05,0.10,...,0.95,0.96,0.97,0.98,0.99 pair.
         bounding_box_mean_average_precision (float):
             Output only. The single metric for bounding boxes
             evaluation: the mean_average_precision averaged over all
             bounding_box_metrics_entries.
     """
 
-    evaluated_frame_count = proto.Field(
+    evaluated_frame_count: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    evaluated_bounding_box_count = proto.Field(
+    evaluated_bounding_box_count: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    bounding_box_metrics_entries = proto.RepeatedField(
+    bounding_box_metrics_entries: MutableSequence[
+        "BoundingBoxMetricsEntry"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=4,
         message="BoundingBoxMetricsEntry",
     )
-    bounding_box_mean_average_precision = proto.Field(
+    bounding_box_mean_average_precision: float = proto.Field(
         proto.FLOAT,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/geometry.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/geometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "NormalizedVertex",
@@ -36,36 +38,36 @@
     Attributes:
         x (float):
             Required. Horizontal coordinate.
         y (float):
             Required. Vertical coordinate.
     """
 
-    x = proto.Field(
+    x: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    y = proto.Field(
+    y: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
 
 
 class BoundingPoly(proto.Message):
     r"""A bounding polygon of a detected object on a plane. On output both
     vertices and normalized_vertices are provided. The polygon is formed
     by connecting vertices in the order they are listed.
 
     Attributes:
-        normalized_vertices (Sequence[google.cloud.automl_v1beta1.types.NormalizedVertex]):
+        normalized_vertices (MutableSequence[google.cloud.automl_v1beta1.types.NormalizedVertex]):
             Output only . The bounding polygon normalized
             vertices.
     """
 
-    normalized_vertices = proto.RepeatedField(
+    normalized_vertices: MutableSequence["NormalizedVertex"] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message="NormalizedVertex",
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/image.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import classification
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -35,15 +37,15 @@
     r"""Dataset metadata that is specific to image classification.
 
     Attributes:
         classification_type (google.cloud.automl_v1beta1.types.ClassificationType):
             Required. Type of the classification problem.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=1,
         enum=classification.ClassificationType,
     )
 
 
 class ImageObjectDetectionDatasetMetadata(proto.Message):
@@ -123,39 +125,39 @@
             model per each node on which it is deployed.
         node_count (int):
             Output only. The number of nodes this model is deployed on.
             A node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the node_qps field.
     """
 
-    base_model_id = proto.Field(
+    base_model_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    train_budget = proto.Field(
+    train_budget: int = proto.Field(
         proto.INT64,
         number=2,
     )
-    train_cost = proto.Field(
+    train_cost: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    stop_reason = proto.Field(
+    stop_reason: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    model_type = proto.Field(
+    model_type: str = proto.Field(
         proto.STRING,
         number=7,
     )
-    node_qps = proto.Field(
+    node_qps: float = proto.Field(
         proto.DOUBLE,
         number=13,
     )
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=14,
     )
 
 
 class ImageObjectDetectionModelMetadata(proto.Message):
     r"""Model metadata specific to image object detection.
@@ -228,35 +230,35 @@
             Output only. The actual train cost of
             creating this model, expressed in milli node
             hours, i.e. 1,000 value in this field means 1
             node hour. Guaranteed to not exceed the train
             budget.
     """
 
-    model_type = proto.Field(
+    model_type: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    node_qps = proto.Field(
+    node_qps: float = proto.Field(
         proto.DOUBLE,
         number=4,
     )
-    stop_reason = proto.Field(
+    stop_reason: str = proto.Field(
         proto.STRING,
         number=5,
     )
-    train_budget_milli_node_hours = proto.Field(
+    train_budget_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    train_cost_milli_node_hours = proto.Field(
+    train_cost_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=7,
     )
 
 
 class ImageClassificationModelDeploymentMetadata(proto.Message):
     r"""Model deployment metadata specific to Image Classification.
@@ -267,15 +269,15 @@
             node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the model's
 
             [node_qps][google.cloud.automl.v1beta1.ImageClassificationModelMetadata.node_qps].
             Must be between 1 and 100, inclusive on both ends.
     """
 
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
 
 
 class ImageObjectDetectionModelDeploymentMetadata(proto.Message):
     r"""Model deployment metadata specific to Image Object Detection.
@@ -286,14 +288,14 @@
             node is an abstraction of a machine resource, which can
             handle online prediction QPS as given in the model's
 
             [qps_per_node][google.cloud.automl.v1beta1.ImageObjectDetectionModelMetadata.qps_per_node].
             Must be between 1 and 100, inclusive on both ends.
     """
 
-    node_count = proto.Field(
+    node_count: int = proto.Field(
         proto.INT64,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/io.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "InputConfig",
@@ -349,39 +351,39 @@
             described in the comment.
 
             This field is a member of `oneof`_ ``source``.
         bigquery_source (google.cloud.automl_v1beta1.types.BigQuerySource):
             The BigQuery location for the input content.
 
             This field is a member of `oneof`_ ``source``.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional domain-specific parameters describing the
             semantic of the imported data, any string must be up to
             25000 characters long.
 
             -  For Tables: ``schema_inference_version`` - (integer)
                Required. The version of the algorithm that should be
                used for the initial inference of the schema (columns'
                DataTypes) of the table the data is being imported into.
                Allowed values: "1".
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
-    bigquery_source = proto.Field(
+    bigquery_source: "BigQuerySource" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="source",
         message="BigQuerySource",
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class BatchPredictInputConfig(proto.Message):
@@ -552,21 +554,21 @@
             This field is a member of `oneof`_ ``source``.
         bigquery_source (google.cloud.automl_v1beta1.types.BigQuerySource):
             The BigQuery location for the input content.
 
             This field is a member of `oneof`_ ``source``.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="GcsSource",
     )
-    bigquery_source = proto.Field(
+    bigquery_source: "BigQuerySource" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="BigQuerySource",
     )
 
 
@@ -578,15 +580,15 @@
         gcs_source (google.cloud.automl_v1beta1.types.GcsSource):
             The Google Cloud Storage location of the
             document file. Only a single path should be
             given. Max supported size: 512MB.
             Supported extensions: .PDF.
     """
 
-    gcs_source = proto.Field(
+    gcs_source: "GcsSource" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="GcsSource",
     )
 
 
 class OutputConfig(proto.Message):
@@ -636,21 +638,21 @@
         bigquery_destination (google.cloud.automl_v1beta1.types.BigQueryDestination):
             The BigQuery location where the output is to
             be written to.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    bigquery_destination = proto.Field(
+    bigquery_destination: "BigQueryDestination" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="destination",
         message="BigQueryDestination",
     )
 
 
@@ -958,21 +960,21 @@
         bigquery_destination (google.cloud.automl_v1beta1.types.BigQueryDestination):
             The BigQuery location where the output is to
             be written to.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    bigquery_destination = proto.Field(
+    bigquery_destination: "BigQueryDestination" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="destination",
         message="BigQueryDestination",
     )
 
 
@@ -1062,41 +1064,41 @@
                work correctly on ubuntu 16.04 operating system. See more
                at [containers
 
             quickstart](https:
             //cloud.google.com/vision/automl/docs/containers-gcs-quickstart)
 
             -  core_ml - Used for iOS mobile devices.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional model-type and format specific parameters
             describing the requirements for the to be exported model
             files, any string must be up to 25000 characters long.
 
             -  For ``docker`` format: ``cpu_architecture`` - (string)
                "x86_64" (default). ``gpu_architecture`` - (string)
                "none" (default), "nvidia".
     """
 
-    gcs_destination = proto.Field(
+    gcs_destination: "GcsDestination" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="destination",
         message="GcsDestination",
     )
-    gcr_destination = proto.Field(
+    gcr_destination: "GcrDestination" = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="destination",
         message="GcrDestination",
     )
-    model_format = proto.Field(
+    model_format: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class ExportEvaluatedExamplesOutputConfig(proto.Message):
@@ -1136,34 +1138,34 @@
         bigquery_destination (google.cloud.automl_v1beta1.types.BigQueryDestination):
             The BigQuery location where the output is to
             be written to.
 
             This field is a member of `oneof`_ ``destination``.
     """
 
-    bigquery_destination = proto.Field(
+    bigquery_destination: "BigQueryDestination" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="destination",
         message="BigQueryDestination",
     )
 
 
 class GcsSource(proto.Message):
     r"""The Google Cloud Storage location for the input content.
 
     Attributes:
-        input_uris (Sequence[str]):
+        input_uris (MutableSequence[str]):
             Required. Google Cloud Storage URIs to input files, up to
             2000 characters long. Accepted forms:
 
             -  Full object path, e.g. gs://bucket/directory/object.csv
     """
 
-    input_uris = proto.RepeatedField(
+    input_uris: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=1,
     )
 
 
 class BigQuerySource(proto.Message):
     r"""The BigQuery location for the input content.
@@ -1172,15 +1174,15 @@
         input_uri (str):
             Required. BigQuery URI to a table, up to 2000 characters
             long. Accepted forms:
 
             -  BigQuery path e.g. bq://projectId.bqDatasetId.bqTableId
     """
 
-    input_uri = proto.Field(
+    input_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GcsDestination(proto.Message):
     r"""The Google Cloud Storage location where the output is to be
@@ -1192,15 +1194,15 @@
             to 2000 characters long. Accepted forms:
 
             -  Prefix path: gs://bucket/directory The requesting user
                must have write permission to the bucket. The directory
                is created if it doesn't exist.
     """
 
-    output_uri_prefix = proto.Field(
+    output_uri_prefix: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class BigQueryDestination(proto.Message):
     r"""The BigQuery location for the output content.
@@ -1209,15 +1211,15 @@
         output_uri (str):
             Required. BigQuery URI to a project, up to 2000 characters
             long. Accepted forms:
 
             -  BigQuery path e.g. bq://projectId
     """
 
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GcrDestination(proto.Message):
     r"""The GCR location where the image must be pushed to.
@@ -1234,14 +1236,14 @@
             -  [HOSTNAME]/[PROJECT-ID]/[IMAGE]
             -  [HOSTNAME]/[PROJECT-ID]/[IMAGE]:[TAG]
 
             The requesting user must have permission to push images the
             project.
     """
 
-    output_uri = proto.Field(
+    output_uri: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/model.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import image
 from google.cloud.automl_v1beta1.types import tables
 from google.cloud.automl_v1beta1.types import text
 from google.cloud.automl_v1beta1.types import translation
 from google.cloud.automl_v1beta1.types import video
@@ -105,91 +107,101 @@
 
     class DeploymentState(proto.Enum):
         r"""Deployment state of the model."""
         DEPLOYMENT_STATE_UNSPECIFIED = 0
         DEPLOYED = 1
         UNDEPLOYED = 2
 
-    translation_model_metadata = proto.Field(
+    translation_model_metadata: translation.TranslationModelMetadata = proto.Field(
         proto.MESSAGE,
         number=15,
         oneof="model_metadata",
         message=translation.TranslationModelMetadata,
     )
-    image_classification_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=13,
-        oneof="model_metadata",
-        message=image.ImageClassificationModelMetadata,
-    )
-    text_classification_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=14,
-        oneof="model_metadata",
-        message=text.TextClassificationModelMetadata,
-    )
-    image_object_detection_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=20,
-        oneof="model_metadata",
-        message=image.ImageObjectDetectionModelMetadata,
-    )
-    video_classification_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=23,
-        oneof="model_metadata",
-        message=video.VideoClassificationModelMetadata,
-    )
-    video_object_tracking_model_metadata = proto.Field(
-        proto.MESSAGE,
-        number=21,
-        oneof="model_metadata",
-        message=video.VideoObjectTrackingModelMetadata,
+    image_classification_model_metadata: image.ImageClassificationModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=13,
+            oneof="model_metadata",
+            message=image.ImageClassificationModelMetadata,
+        )
+    )
+    text_classification_model_metadata: text.TextClassificationModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=14,
+            oneof="model_metadata",
+            message=text.TextClassificationModelMetadata,
+        )
+    )
+    image_object_detection_model_metadata: image.ImageObjectDetectionModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=20,
+            oneof="model_metadata",
+            message=image.ImageObjectDetectionModelMetadata,
+        )
+    )
+    video_classification_model_metadata: video.VideoClassificationModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=23,
+            oneof="model_metadata",
+            message=video.VideoClassificationModelMetadata,
+        )
+    )
+    video_object_tracking_model_metadata: video.VideoObjectTrackingModelMetadata = (
+        proto.Field(
+            proto.MESSAGE,
+            number=21,
+            oneof="model_metadata",
+            message=video.VideoObjectTrackingModelMetadata,
+        )
     )
-    text_extraction_model_metadata = proto.Field(
+    text_extraction_model_metadata: text.TextExtractionModelMetadata = proto.Field(
         proto.MESSAGE,
         number=19,
         oneof="model_metadata",
         message=text.TextExtractionModelMetadata,
     )
-    tables_model_metadata = proto.Field(
+    tables_model_metadata: tables.TablesModelMetadata = proto.Field(
         proto.MESSAGE,
         number=24,
         oneof="model_metadata",
         message=tables.TablesModelMetadata,
     )
-    text_sentiment_model_metadata = proto.Field(
+    text_sentiment_model_metadata: text.TextSentimentModelMetadata = proto.Field(
         proto.MESSAGE,
         number=22,
         oneof="model_metadata",
         message=text.TextSentimentModelMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    dataset_id = proto.Field(
+    dataset_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=11,
         message=timestamp_pb2.Timestamp,
     )
-    deployment_state = proto.Field(
+    deployment_state: DeploymentState = proto.Field(
         proto.ENUM,
         number=8,
         enum=DeploymentState,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/model_evaluation.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/model_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import classification
 from google.cloud.automl_v1beta1.types import detection
 from google.cloud.automl_v1beta1.types import regression
 from google.cloud.automl_v1beta1.types import text_extraction
 from google.cloud.automl_v1beta1.types import text_sentiment
@@ -120,73 +122,77 @@
             examples used for evaluation. Otherwise, this is the count
             of examples that according to the ground truth were
             annotated by the
 
             [annotation_spec_id][google.cloud.automl.v1beta1.ModelEvaluation.annotation_spec_id].
     """
 
-    classification_evaluation_metrics = proto.Field(
+    classification_evaluation_metrics: classification.ClassificationEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="metrics",
         message=classification.ClassificationEvaluationMetrics,
     )
-    regression_evaluation_metrics = proto.Field(
+    regression_evaluation_metrics: regression.RegressionEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=24,
         oneof="metrics",
         message=regression.RegressionEvaluationMetrics,
     )
-    translation_evaluation_metrics = proto.Field(
-        proto.MESSAGE,
-        number=9,
-        oneof="metrics",
-        message=translation.TranslationEvaluationMetrics,
+    translation_evaluation_metrics: translation.TranslationEvaluationMetrics = (
+        proto.Field(
+            proto.MESSAGE,
+            number=9,
+            oneof="metrics",
+            message=translation.TranslationEvaluationMetrics,
+        )
     )
-    image_object_detection_evaluation_metrics = proto.Field(
+    image_object_detection_evaluation_metrics: detection.ImageObjectDetectionEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=12,
         oneof="metrics",
         message=detection.ImageObjectDetectionEvaluationMetrics,
     )
-    video_object_tracking_evaluation_metrics = proto.Field(
+    video_object_tracking_evaluation_metrics: detection.VideoObjectTrackingEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=14,
         oneof="metrics",
         message=detection.VideoObjectTrackingEvaluationMetrics,
     )
-    text_sentiment_evaluation_metrics = proto.Field(
-        proto.MESSAGE,
-        number=11,
-        oneof="metrics",
-        message=text_sentiment.TextSentimentEvaluationMetrics,
+    text_sentiment_evaluation_metrics: text_sentiment.TextSentimentEvaluationMetrics = (
+        proto.Field(
+            proto.MESSAGE,
+            number=11,
+            oneof="metrics",
+            message=text_sentiment.TextSentimentEvaluationMetrics,
+        )
     )
-    text_extraction_evaluation_metrics = proto.Field(
+    text_extraction_evaluation_metrics: text_extraction.TextExtractionEvaluationMetrics = proto.Field(
         proto.MESSAGE,
         number=13,
         oneof="metrics",
         message=text_extraction.TextExtractionEvaluationMetrics,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    annotation_spec_id = proto.Field(
+    annotation_spec_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=15,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=5,
         message=timestamp_pb2.Timestamp,
     )
-    evaluated_example_count = proto.Field(
+    evaluated_example_count: int = proto.Field(
         proto.INT32,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/operations.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import io
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
 
@@ -84,97 +86,99 @@
         export_evaluated_examples_details (google.cloud.automl_v1beta1.types.ExportEvaluatedExamplesOperationMetadata):
             Details of ExportEvaluatedExamples operation.
 
             This field is a member of `oneof`_ ``details``.
         progress_percent (int):
             Output only. Progress of operation. Range: [0, 100]. Not
             used currently.
-        partial_failures (Sequence[google.rpc.status_pb2.Status]):
+        partial_failures (MutableSequence[google.rpc.status_pb2.Status]):
             Output only. Partial failures encountered.
             E.g. single files that couldn't be read.
             This field should never exceed 20 entries.
             Status details field will contain standard GCP
             error details.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the operation was
             created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the operation was
             updated for the last time.
     """
 
-    delete_details = proto.Field(
+    delete_details: "DeleteOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="details",
         message="DeleteOperationMetadata",
     )
-    deploy_model_details = proto.Field(
+    deploy_model_details: "DeployModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=24,
         oneof="details",
         message="DeployModelOperationMetadata",
     )
-    undeploy_model_details = proto.Field(
+    undeploy_model_details: "UndeployModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=25,
         oneof="details",
         message="UndeployModelOperationMetadata",
     )
-    create_model_details = proto.Field(
+    create_model_details: "CreateModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="details",
         message="CreateModelOperationMetadata",
     )
-    import_data_details = proto.Field(
+    import_data_details: "ImportDataOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=15,
         oneof="details",
         message="ImportDataOperationMetadata",
     )
-    batch_predict_details = proto.Field(
+    batch_predict_details: "BatchPredictOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=16,
         oneof="details",
         message="BatchPredictOperationMetadata",
     )
-    export_data_details = proto.Field(
+    export_data_details: "ExportDataOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=21,
         oneof="details",
         message="ExportDataOperationMetadata",
     )
-    export_model_details = proto.Field(
+    export_model_details: "ExportModelOperationMetadata" = proto.Field(
         proto.MESSAGE,
         number=22,
         oneof="details",
         message="ExportModelOperationMetadata",
     )
-    export_evaluated_examples_details = proto.Field(
-        proto.MESSAGE,
-        number=26,
-        oneof="details",
-        message="ExportEvaluatedExamplesOperationMetadata",
+    export_evaluated_examples_details: "ExportEvaluatedExamplesOperationMetadata" = (
+        proto.Field(
+            proto.MESSAGE,
+            number=26,
+            oneof="details",
+            message="ExportEvaluatedExamplesOperationMetadata",
+        )
     )
-    progress_percent = proto.Field(
+    progress_percent: int = proto.Field(
         proto.INT32,
         number=13,
     )
-    partial_failures = proto.RepeatedField(
+    partial_failures: MutableSequence[status_pb2.Status] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=status_pb2.Status,
     )
-    create_time = proto.Field(
+    create_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=3,
         message=timestamp_pb2.Timestamp,
     )
-    update_time = proto.Field(
+    update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=4,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class DeleteOperationMetadata(proto.Message):
@@ -228,26 +232,26 @@
                 The path of the BigQuery dataset created, in
                 bq://projectId.bqDatasetId format, into which
                 the exported data is written.
 
                 This field is a member of `oneof`_ ``output_location``.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
             oneof="output_location",
         )
-        bigquery_output_dataset = proto.Field(
+        bigquery_output_dataset: str = proto.Field(
             proto.STRING,
             number=2,
             oneof="output_location",
         )
 
-    output_info = proto.Field(
+    output_info: ExportDataOutputInfo = proto.Field(
         proto.MESSAGE,
         number=1,
         message=ExportDataOutputInfo,
     )
 
 
 class BatchPredictOperationMetadata(proto.Message):
@@ -285,31 +289,31 @@
                 The path of the BigQuery dataset created, in
                 bq://projectId.bqDatasetId format, into which
                 the prediction output is written.
 
                 This field is a member of `oneof`_ ``output_location``.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
             oneof="output_location",
         )
-        bigquery_output_dataset = proto.Field(
+        bigquery_output_dataset: str = proto.Field(
             proto.STRING,
             number=2,
             oneof="output_location",
         )
 
-    input_config = proto.Field(
+    input_config: io.BatchPredictInputConfig = proto.Field(
         proto.MESSAGE,
         number=1,
         message=io.BatchPredictInputConfig,
     )
-    output_info = proto.Field(
+    output_info: BatchPredictOutputInfo = proto.Field(
         proto.MESSAGE,
         number=2,
         message=BatchPredictOutputInfo,
     )
 
 
 class ExportModelOperationMetadata(proto.Message):
@@ -329,20 +333,20 @@
         Attributes:
             gcs_output_directory (str):
                 The full path of the Google Cloud Storage
                 directory created, into which the model will be
                 exported.
         """
 
-        gcs_output_directory = proto.Field(
+        gcs_output_directory: str = proto.Field(
             proto.STRING,
             number=1,
         )
 
-    output_info = proto.Field(
+    output_info: ExportModelOutputInfo = proto.Field(
         proto.MESSAGE,
         number=2,
         message=ExportModelOutputInfo,
     )
 
 
 class ExportEvaluatedExamplesOperationMetadata(proto.Message):
@@ -364,20 +368,20 @@
             bigquery_output_dataset (str):
                 The path of the BigQuery dataset created, in
                 bq://projectId.bqDatasetId format, into which
                 the output of export evaluated examples is
                 written.
         """
 
-        bigquery_output_dataset = proto.Field(
+        bigquery_output_dataset: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
-    output_info = proto.Field(
+    output_info: ExportEvaluatedExamplesOutputInfo = proto.Field(
         proto.MESSAGE,
         number=2,
         message=ExportEvaluatedExamplesOutputInfo,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/prediction_service.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/prediction_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import annotation_payload
 from google.cloud.automl_v1beta1.types import data_items
 from google.cloud.automl_v1beta1.types import io
 
 
@@ -39,15 +41,15 @@
         name (str):
             Required. Name of the model requested to
             serve the prediction.
         payload (google.cloud.automl_v1beta1.types.ExamplePayload):
             Required. Payload to perform a prediction on.
             The payload must match the problem type that the
             model was trained to solve.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Additional domain-specific parameters, any string must be up
             to 25000 characters long.
 
             -  For Image Classification:
 
                ``score_threshold`` - (float) A value from 0.0 to 1.0.
                When the model makes predictions for an image, it will
@@ -64,48 +66,48 @@
                limited by server.
 
             -  For Tables: feature_importance - (boolean) Whether
                feature importance should be populated in the returned
                TablesAnnotation. The default is false.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    payload = proto.Field(
+    payload: data_items.ExamplePayload = proto.Field(
         proto.MESSAGE,
         number=2,
         message=data_items.ExamplePayload,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=3,
     )
 
 
 class PredictResponse(proto.Message):
     r"""Response message for
     [PredictionService.Predict][google.cloud.automl.v1beta1.PredictionService.Predict].
 
     Attributes:
-        payload (Sequence[google.cloud.automl_v1beta1.types.AnnotationPayload]):
+        payload (MutableSequence[google.cloud.automl_v1beta1.types.AnnotationPayload]):
             Prediction result.
             Translation and Text Sentiment will return
             precisely one payload.
         preprocessed_input (google.cloud.automl_v1beta1.types.ExamplePayload):
             The preprocessed example that AutoML actually makes
             prediction on. Empty if AutoML does not preprocess the input
             example.
 
             -  For Text Extraction: If the input is a .pdf file, the
                OCR'ed text will be provided in
                [document_text][google.cloud.automl.v1beta1.Document.document_text].
-        metadata (Mapping[str, str]):
+        metadata (MutableMapping[str, str]):
             Additional domain-specific prediction response metadata.
 
             -  For Image Object Detection: ``max_bounding_box_count`` -
                (int64) At most that many bounding boxes per image could
                have been returned.
 
             -  For Text Sentiment: ``sentiment_score`` - (float,
@@ -116,25 +118,27 @@
                training data, so e.g. if all data was positive then -1
                will be also positive (though the least). The
                sentiment_score shouldn't be confused with "score" or
                "magnitude" from the previous Natural Language Sentiment
                Analysis API.
     """
 
-    payload = proto.RepeatedField(
+    payload: MutableSequence[
+        annotation_payload.AnnotationPayload
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=annotation_payload.AnnotationPayload,
     )
-    preprocessed_input = proto.Field(
+    preprocessed_input: data_items.ExamplePayload = proto.Field(
         proto.MESSAGE,
         number=3,
         message=data_items.ExamplePayload,
     )
-    metadata = proto.MapField(
+    metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=2,
     )
 
 
 class BatchPredictRequest(proto.Message):
@@ -147,15 +151,15 @@
             serve the batch prediction.
         input_config (google.cloud.automl_v1beta1.types.BatchPredictInputConfig):
             Required. The input configuration for batch
             prediction.
         output_config (google.cloud.automl_v1beta1.types.BatchPredictOutputConfig):
             Required. The Configuration specifying where
             output predictions should be written.
-        params (Mapping[str, str]):
+        params (MutableMapping[str, str]):
             Required. Additional domain-specific parameters for the
             predictions, any string must be up to 25000 characters long.
 
             -  For Text Classification:
 
                ``score_threshold`` - (float) A value from 0.0 to 1.0.
                When the model makes predictions for a text snippet, it
@@ -227,55 +231,55 @@
                be returned per frame. Default is 100, the requested
                value may be limited by server. ``min_bounding_box_size``
                - (float) Only bounding boxes with shortest edge at least
                that long as a relative value of video frame size will be
                returned. Value in 0 to 1 range. Default is 0.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_config = proto.Field(
+    input_config: io.BatchPredictInputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.BatchPredictInputConfig,
     )
-    output_config = proto.Field(
+    output_config: io.BatchPredictOutputConfig = proto.Field(
         proto.MESSAGE,
         number=4,
         message=io.BatchPredictOutputConfig,
     )
-    params = proto.MapField(
+    params: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=5,
     )
 
 
 class BatchPredictResult(proto.Message):
     r"""Result of the Batch Predict. This message is returned in
     [response][google.longrunning.Operation.response] of the operation
     returned by the
     [PredictionService.BatchPredict][google.cloud.automl.v1beta1.PredictionService.BatchPredict].
 
     Attributes:
-        metadata (Mapping[str, str]):
+        metadata (MutableMapping[str, str]):
             Additional domain-specific prediction response metadata.
 
             -  For Image Object Detection: ``max_bounding_box_count`` -
                (int64) At most that many bounding boxes per image could
                have been returned.
 
             -  For Video Object Tracking: ``max_bounding_box_count`` -
                (int64) At most that many bounding boxes per frame could
                have been returned.
     """
 
-    metadata = proto.MapField(
+    metadata: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/ranges.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_segment.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,39 +9,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
-        "DoubleRange",
+        "TextSegment",
     },
 )
 
 
-class DoubleRange(proto.Message):
-    r"""A range between two double numbers.
+class TextSegment(proto.Message):
+    r"""A contiguous part of a text (string), assuming it has an
+    UTF-8 NFC encoding.
 
     Attributes:
-        start (float):
-            Start of the range, inclusive.
-        end (float):
-            End of the range, exclusive.
+        content (str):
+            Output only. The content of the TextSegment.
+        start_offset (int):
+            Required. Zero-based character index of the
+            first character of the text segment (counting
+            characters from the beginning of the text).
+        end_offset (int):
+            Required. Zero-based character index of the first character
+            past the end of the text segment (counting character from
+            the beginning of the text). The character at the end_offset
+            is NOT included in the text segment.
     """
 
-    start = proto.Field(
-        proto.DOUBLE,
+    content: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    start_offset: int = proto.Field(
+        proto.INT64,
         number=1,
     )
-    end = proto.Field(
-        proto.DOUBLE,
+    end_offset: int = proto.Field(
+        proto.INT64,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/regression.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/regression.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "RegressionEvaluationMetrics",
@@ -38,30 +40,30 @@
             positive.
         r_squared (float):
             Output only. R squared.
         root_mean_squared_log_error (float):
             Output only. Root mean squared log error.
     """
 
-    root_mean_squared_error = proto.Field(
+    root_mean_squared_error: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    mean_absolute_error = proto.Field(
+    mean_absolute_error: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    mean_absolute_percentage_error = proto.Field(
+    mean_absolute_percentage_error: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    r_squared = proto.Field(
+    r_squared: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    root_mean_squared_log_error = proto.Field(
+    root_mean_squared_log_error: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/service.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import column_spec as gca_column_spec
 from google.cloud.automl_v1beta1.types import dataset as gca_dataset
 from google.cloud.automl_v1beta1.types import image
 from google.cloud.automl_v1beta1.types import io
 from google.cloud.automl_v1beta1.types import model as gca_model
@@ -69,19 +71,19 @@
         parent (str):
             Required. The resource name of the project to
             create the dataset for.
         dataset (google.cloud.automl_v1beta1.types.Dataset):
             Required. The dataset to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    dataset = proto.Field(
+    dataset: gca_dataset.Dataset = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gca_dataset.Dataset,
     )
 
 
 class GetDatasetRequest(proto.Message):
@@ -90,15 +92,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the dataset to
             retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListDatasetsRequest(proto.Message):
     r"""Request message for
@@ -126,55 +128,55 @@
             return Typically obtained via
             [ListDatasetsResponse.next_page_token][google.cloud.automl.v1beta1.ListDatasetsResponse.next_page_token]
             of the previous
             [AutoMl.ListDatasets][google.cloud.automl.v1beta1.AutoMl.ListDatasets]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListDatasetsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListDatasets][google.cloud.automl.v1beta1.AutoMl.ListDatasets].
 
     Attributes:
-        datasets (Sequence[google.cloud.automl_v1beta1.types.Dataset]):
+        datasets (MutableSequence[google.cloud.automl_v1beta1.types.Dataset]):
             The datasets read.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListDatasetsRequest.page_token][google.cloud.automl.v1beta1.ListDatasetsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    datasets = proto.RepeatedField(
+    datasets: MutableSequence[gca_dataset.Dataset] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_dataset.Dataset,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class UpdateDatasetRequest(proto.Message):
     r"""Request message for
@@ -184,20 +186,20 @@
         dataset (google.cloud.automl_v1beta1.types.Dataset):
             Required. The dataset which replaces the
             resource on the server.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The update mask applies to the resource.
     """
 
-    dataset = proto.Field(
+    dataset: gca_dataset.Dataset = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gca_dataset.Dataset,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteDatasetRequest(proto.Message):
@@ -206,15 +208,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the dataset to
             delete.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ImportDataRequest(proto.Message):
     r"""Request message for
@@ -226,19 +228,19 @@
             exist. All imported annotations and examples
             will be added.
         input_config (google.cloud.automl_v1beta1.types.InputConfig):
             Required. The desired input location and its
             domain specific semantics, if any.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    input_config = proto.Field(
+    input_config: io.InputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.InputConfig,
     )
 
 
 class ExportDataRequest(proto.Message):
@@ -248,19 +250,19 @@
     Attributes:
         name (str):
             Required. The resource name of the dataset.
         output_config (google.cloud.automl_v1beta1.types.OutputConfig):
             Required. The desired output location.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    output_config = proto.Field(
+    output_config: io.OutputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.OutputConfig,
     )
 
 
 class GetAnnotationSpecRequest(proto.Message):
@@ -269,15 +271,15 @@
 
     Attributes:
         name (str):
             Required. The resource name of the annotation
             spec to retrieve.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class GetTableSpecRequest(proto.Message):
     r"""Request message for
@@ -287,19 +289,19 @@
         name (str):
             Required. The resource name of the table spec
             to retrieve.
         field_mask (google.protobuf.field_mask_pb2.FieldMask):
             Mask specifying which fields to read.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    field_mask = proto.Field(
+    field_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class ListTableSpecsRequest(proto.Message):
@@ -323,60 +325,60 @@
             return. Typically obtained from the
             [ListTableSpecsResponse.next_page_token][google.cloud.automl.v1beta1.ListTableSpecsResponse.next_page_token]
             field of the previous
             [AutoMl.ListTableSpecs][google.cloud.automl.v1beta1.AutoMl.ListTableSpecs]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    field_mask = proto.Field(
+    field_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListTableSpecsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListTableSpecs][google.cloud.automl.v1beta1.AutoMl.ListTableSpecs].
 
     Attributes:
-        table_specs (Sequence[google.cloud.automl_v1beta1.types.TableSpec]):
+        table_specs (MutableSequence[google.cloud.automl_v1beta1.types.TableSpec]):
             The table specs read.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListTableSpecsRequest.page_token][google.cloud.automl.v1beta1.ListTableSpecsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    table_specs = proto.RepeatedField(
+    table_specs: MutableSequence[gca_table_spec.TableSpec] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_table_spec.TableSpec,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class UpdateTableSpecRequest(proto.Message):
     r"""Request message for
@@ -386,20 +388,20 @@
         table_spec (google.cloud.automl_v1beta1.types.TableSpec):
             Required. The table spec which replaces the
             resource on the server.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The update mask applies to the resource.
     """
 
-    table_spec = proto.Field(
+    table_spec: gca_table_spec.TableSpec = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gca_table_spec.TableSpec,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class GetColumnSpecRequest(proto.Message):
@@ -410,19 +412,19 @@
         name (str):
             Required. The resource name of the column
             spec to retrieve.
         field_mask (google.protobuf.field_mask_pb2.FieldMask):
             Mask specifying which fields to read.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    field_mask = proto.Field(
+    field_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class ListColumnSpecsRequest(proto.Message):
@@ -446,60 +448,60 @@
             return. Typically obtained from the
             [ListColumnSpecsResponse.next_page_token][google.cloud.automl.v1beta1.ListColumnSpecsResponse.next_page_token]
             field of the previous
             [AutoMl.ListColumnSpecs][google.cloud.automl.v1beta1.AutoMl.ListColumnSpecs]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    field_mask = proto.Field(
+    field_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListColumnSpecsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListColumnSpecs][google.cloud.automl.v1beta1.AutoMl.ListColumnSpecs].
 
     Attributes:
-        column_specs (Sequence[google.cloud.automl_v1beta1.types.ColumnSpec]):
+        column_specs (MutableSequence[google.cloud.automl_v1beta1.types.ColumnSpec]):
             The column specs read.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListColumnSpecsRequest.page_token][google.cloud.automl.v1beta1.ListColumnSpecsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    column_specs = proto.RepeatedField(
+    column_specs: MutableSequence[gca_column_spec.ColumnSpec] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_column_spec.ColumnSpec,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class UpdateColumnSpecRequest(proto.Message):
     r"""Request message for
@@ -509,20 +511,20 @@
         column_spec (google.cloud.automl_v1beta1.types.ColumnSpec):
             Required. The column spec which replaces the
             resource on the server.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             The update mask applies to the resource.
     """
 
-    column_spec = proto.Field(
+    column_spec: gca_column_spec.ColumnSpec = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gca_column_spec.ColumnSpec,
     )
-    update_mask = proto.Field(
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=2,
         message=field_mask_pb2.FieldMask,
     )
 
 
 class CreateModelRequest(proto.Message):
@@ -533,19 +535,19 @@
         parent (str):
             Required. Resource name of the parent project
             where the model is being created.
         model (google.cloud.automl_v1beta1.types.Model):
             Required. The model to create.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    model = proto.Field(
+    model: gca_model.Model = proto.Field(
         proto.MESSAGE,
         number=4,
         message=gca_model.Model,
     )
 
 
 class GetModelRequest(proto.Message):
@@ -553,15 +555,15 @@
     [AutoMl.GetModel][google.cloud.automl.v1beta1.AutoMl.GetModel].
 
     Attributes:
         name (str):
             Required. Resource name of the model.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListModelsRequest(proto.Message):
     r"""Request message for
@@ -592,55 +594,55 @@
             return Typically obtained via
             [ListModelsResponse.next_page_token][google.cloud.automl.v1beta1.ListModelsResponse.next_page_token]
             of the previous
             [AutoMl.ListModels][google.cloud.automl.v1beta1.AutoMl.ListModels]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListModelsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListModels][google.cloud.automl.v1beta1.AutoMl.ListModels].
 
     Attributes:
-        model (Sequence[google.cloud.automl_v1beta1.types.Model]):
+        model (MutableSequence[google.cloud.automl_v1beta1.types.Model]):
             List of models in the requested page.
         next_page_token (str):
             A token to retrieve next page of results. Pass to
             [ListModelsRequest.page_token][google.cloud.automl.v1beta1.ListModelsRequest.page_token]
             to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    model = proto.RepeatedField(
+    model: MutableSequence[gca_model.Model] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_model.Model,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class DeleteModelRequest(proto.Message):
     r"""Request message for
@@ -648,15 +650,15 @@
 
     Attributes:
         name (str):
             Required. Resource name of the model being
             deleted.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class DeployModelRequest(proto.Message):
     r"""Request message for
@@ -681,27 +683,27 @@
 
             This field is a member of `oneof`_ ``model_deployment_metadata``.
         name (str):
             Required. Resource name of the model to
             deploy.
     """
 
-    image_object_detection_model_deployment_metadata = proto.Field(
+    image_object_detection_model_deployment_metadata: image.ImageObjectDetectionModelDeploymentMetadata = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="model_deployment_metadata",
         message=image.ImageObjectDetectionModelDeploymentMetadata,
     )
-    image_classification_model_deployment_metadata = proto.Field(
+    image_classification_model_deployment_metadata: image.ImageClassificationModelDeploymentMetadata = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="model_deployment_metadata",
         message=image.ImageClassificationModelDeploymentMetadata,
     )
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UndeployModelRequest(proto.Message):
     r"""Request message for
@@ -709,15 +711,15 @@
 
     Attributes:
         name (str):
             Required. Resource name of the model to
             undeploy.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ExportModelRequest(proto.Message):
     r"""Request message for
@@ -730,19 +732,19 @@
             Required. The resource name of the model to
             export.
         output_config (google.cloud.automl_v1beta1.types.ModelExportOutputConfig):
             Required. The desired output location and
             configuration.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    output_config = proto.Field(
+    output_config: io.ModelExportOutputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.ModelExportOutputConfig,
     )
 
 
 class ExportEvaluatedExamplesRequest(proto.Message):
@@ -754,19 +756,19 @@
             Required. The resource name of the model
             whose evaluated examples are to be exported.
         output_config (google.cloud.automl_v1beta1.types.ExportEvaluatedExamplesOutputConfig):
             Required. The desired output location and
             configuration.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    output_config = proto.Field(
+    output_config: io.ExportEvaluatedExamplesOutputConfig = proto.Field(
         proto.MESSAGE,
         number=3,
         message=io.ExportEvaluatedExamplesOutputConfig,
     )
 
 
 class GetModelEvaluationRequest(proto.Message):
@@ -775,15 +777,15 @@
 
     Attributes:
         name (str):
             Required. Resource name for the model
             evaluation.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListModelEvaluationsRequest(proto.Message):
     r"""Request message for
@@ -814,57 +816,59 @@
             return. Typically obtained via
             [ListModelEvaluationsResponse.next_page_token][google.cloud.automl.v1beta1.ListModelEvaluationsResponse.next_page_token]
             of the previous
             [AutoMl.ListModelEvaluations][google.cloud.automl.v1beta1.AutoMl.ListModelEvaluations]
             call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=4,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 class ListModelEvaluationsResponse(proto.Message):
     r"""Response message for
     [AutoMl.ListModelEvaluations][google.cloud.automl.v1beta1.AutoMl.ListModelEvaluations].
 
     Attributes:
-        model_evaluation (Sequence[google.cloud.automl_v1beta1.types.ModelEvaluation]):
+        model_evaluation (MutableSequence[google.cloud.automl_v1beta1.types.ModelEvaluation]):
             List of model evaluations in the requested
             page.
         next_page_token (str):
             A token to retrieve next page of results. Pass to the
             [ListModelEvaluationsRequest.page_token][google.cloud.automl.v1beta1.ListModelEvaluationsRequest.page_token]
             field of a new
             [AutoMl.ListModelEvaluations][google.cloud.automl.v1beta1.AutoMl.ListModelEvaluations]
             request to obtain that page.
     """
 
     @property
     def raw_page(self):
         return self
 
-    model_evaluation = proto.RepeatedField(
+    model_evaluation: MutableSequence[
+        gca_model_evaluation.ModelEvaluation
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gca_model_evaluation.ModelEvaluation,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/table_spec.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/table_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import io
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -59,49 +61,49 @@
             Output only. The number of valid rows (i.e.
             without values that don't match DataType-s of
             their columns).
         column_count (int):
             Output only. The number of columns of the
             table. That is, the number of child
             ColumnSpec-s.
-        input_configs (Sequence[google.cloud.automl_v1beta1.types.InputConfig]):
+        input_configs (MutableSequence[google.cloud.automl_v1beta1.types.InputConfig]):
             Output only. Input configs via which data
             currently residing in the table had been
             imported.
         etag (str):
             Used to perform consistent read-modify-write
             updates. If not set, a blind "overwrite" update
             happens.
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    time_column_spec_id = proto.Field(
+    time_column_spec_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    row_count = proto.Field(
+    row_count: int = proto.Field(
         proto.INT64,
         number=3,
     )
-    valid_row_count = proto.Field(
+    valid_row_count: int = proto.Field(
         proto.INT64,
         number=4,
     )
-    column_count = proto.Field(
+    column_count: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    input_configs = proto.RepeatedField(
+    input_configs: MutableSequence[io.InputConfig] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message=io.InputConfig,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/tables.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import column_spec
 from google.cloud.automl_v1beta1.types import data_stats
 from google.cloud.automl_v1beta1.types import ranges
 from google.protobuf import struct_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
@@ -76,15 +78,15 @@
             Note that if a given ml use distribution makes it impossible
             to create a "good" model, that call will error describing
             the issue. If both this column_spec_id and primary table's
             time_column_spec_id are not set, then all rows are treated
             as ``UNASSIGNED``. NOTE: Updates of this field will
             instantly affect any other users concurrently working with
             the dataset.
-        target_column_correlations (Mapping[str, google.cloud.automl_v1beta1.types.CorrelationStats]):
+        target_column_correlations (MutableMapping[str, google.cloud.automl_v1beta1.types.CorrelationStats]):
             Output only. Correlations between
 
             [TablesDatasetMetadata.target_column_spec_id][google.cloud.automl.v1beta1.TablesDatasetMetadata.target_column_spec_id],
             and other columns of the
 
             [TablesDatasetMetadataprimary_table][google.cloud.automl.v1beta1.TablesDatasetMetadata.primary_table_spec_id].
             Only set if the target column is set. Mapping from other
@@ -98,37 +100,39 @@
             ColumnSpec.data_stats and ColumnSpec.top_correlated_columns
             fields were last (re-)generated. Any changes that happened
             to the dataset afterwards are not reflected in these fields
             values. The regeneration happens in the background on a best
             effort basis.
     """
 
-    primary_table_spec_id = proto.Field(
+    primary_table_spec_id: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    target_column_spec_id = proto.Field(
+    target_column_spec_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    weight_column_spec_id = proto.Field(
+    weight_column_spec_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    ml_use_column_spec_id = proto.Field(
+    ml_use_column_spec_id: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    target_column_correlations = proto.MapField(
+    target_column_correlations: MutableMapping[
+        str, data_stats.CorrelationStats
+    ] = proto.MapField(
         proto.STRING,
         proto.MESSAGE,
         number=6,
         message=data_stats.CorrelationStats,
     )
-    stats_update_time = proto.Field(
+    stats_update_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=7,
         message=timestamp_pb2.Timestamp,
     )
 
 
 class TablesModelMetadata(proto.Message):
@@ -159,15 +163,15 @@
             model is predicting. Snapshotted when model creation
             started. Only 3 fields are used: name - May be set on
             CreateModel, if it's not then the ColumnSpec corresponding
             to the current target_column_spec_id of the dataset the
             model is trained from is used. If neither is set,
             CreateModel will error. display_name - Output only.
             data_type - Output only.
-        input_feature_column_specs (Sequence[google.cloud.automl_v1beta1.types.ColumnSpec]):
+        input_feature_column_specs (MutableSequence[google.cloud.automl_v1beta1.types.ColumnSpec]):
             Column specs of the dataset's primary table's columns, on
             which the model is trained and which are used as the input
             for predictions. The
 
             [target_column][google.cloud.automl.v1beta1.TablesModelMetadata.target_column_spec]
             as well as, according to dataset's state upon model
             creation,
@@ -209,15 +213,15 @@
             CLASSIFICATION_MULTI_CLASS : "MINIMIZE_LOG_LOSS" (default) -
             Minimize log loss.
 
             REGRESSION: "MINIMIZE_RMSE" (default) - Minimize
             root-mean-squared error (RMSE). "MINIMIZE_MAE" - Minimize
             mean-absolute error (MAE). "MINIMIZE_RMSLE" - Minimize
             root-mean-squared log error (RMSLE).
-        tables_model_column_info (Sequence[google.cloud.automl_v1beta1.types.TablesModelColumnInfo]):
+        tables_model_column_info (MutableSequence[google.cloud.automl_v1beta1.types.TablesModelColumnInfo]):
             Output only. Auxiliary information for each of the
             input_feature_column_specs with respect to this particular
             model.
         train_budget_milli_node_hours (int):
             Required. The train budget of creating this
             model, expressed in milli node hours i.e. 1,000
             value in this field means 1 node hour.
@@ -244,52 +248,56 @@
             Use the entire training budget. This disables
             the early stopping feature. By default, the
             early stopping feature is enabled, which means
             that AutoML Tables might stop training before
             the entire training budget has been used.
     """
 
-    optimization_objective_recall_value = proto.Field(
+    optimization_objective_recall_value: float = proto.Field(
         proto.FLOAT,
         number=17,
         oneof="additional_optimization_objective_config",
     )
-    optimization_objective_precision_value = proto.Field(
+    optimization_objective_precision_value: float = proto.Field(
         proto.FLOAT,
         number=18,
         oneof="additional_optimization_objective_config",
     )
-    target_column_spec = proto.Field(
+    target_column_spec: column_spec.ColumnSpec = proto.Field(
         proto.MESSAGE,
         number=2,
         message=column_spec.ColumnSpec,
     )
-    input_feature_column_specs = proto.RepeatedField(
+    input_feature_column_specs: MutableSequence[
+        column_spec.ColumnSpec
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=column_spec.ColumnSpec,
     )
-    optimization_objective = proto.Field(
+    optimization_objective: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    tables_model_column_info = proto.RepeatedField(
+    tables_model_column_info: MutableSequence[
+        "TablesModelColumnInfo"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message="TablesModelColumnInfo",
     )
-    train_budget_milli_node_hours = proto.Field(
+    train_budget_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=6,
     )
-    train_cost_milli_node_hours = proto.Field(
+    train_cost_milli_node_hours: int = proto.Field(
         proto.INT64,
         number=7,
     )
-    disable_early_stopping = proto.Field(
+    disable_early_stopping: bool = proto.Field(
         proto.BOOL,
         number=12,
     )
 
 
 class TablesAnnotation(proto.Message):
     r"""Contains annotation details specific to Tables.
@@ -315,15 +323,15 @@
             The value depends on the column's DataType:
 
             -  CATEGORY - the predicted (with the above confidence
                ``score``) CATEGORY value.
 
             -  FLOAT64 - the predicted (with above
                ``prediction_interval``) FLOAT64 value.
-        tables_model_column_info (Sequence[google.cloud.automl_v1beta1.types.TablesModelColumnInfo]):
+        tables_model_column_info (MutableSequence[google.cloud.automl_v1beta1.types.TablesModelColumnInfo]):
             Output only. Auxiliary information for each of the model's
 
             [input_feature_column_specs][google.cloud.automl.v1beta1.TablesModelMetadata.input_feature_column_specs]
             with respect to this particular prediction. If no other
             fields than
 
             [column_spec_name][google.cloud.automl.v1beta1.TablesModelColumnInfo.column_spec_name]
@@ -341,34 +349,36 @@
             importance is requested. For regression models,
             this holds the baseline prediction for the
             baseline example. For classification models,
             this holds the baseline prediction for the
             baseline example for the argmax class.
     """
 
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    prediction_interval = proto.Field(
+    prediction_interval: ranges.DoubleRange = proto.Field(
         proto.MESSAGE,
         number=4,
         message=ranges.DoubleRange,
     )
-    value = proto.Field(
+    value: struct_pb2.Value = proto.Field(
         proto.MESSAGE,
         number=2,
         message=struct_pb2.Value,
     )
-    tables_model_column_info = proto.RepeatedField(
+    tables_model_column_info: MutableSequence[
+        "TablesModelColumnInfo"
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="TablesModelColumnInfo",
     )
-    baseline_score = proto.Field(
+    baseline_score: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
 
 
 class TablesModelColumnInfo(proto.Message):
     r"""An information specific to given column and Tables Model, in
@@ -399,22 +409,22 @@
             prediction returned for the given row the value in this
             column was. Specifically, the feature importance specifies
             the marginal contribution that the feature made to the
             prediction score compared to the baseline score. These
             values are computed using the Sampled Shapley method.
     """
 
-    column_spec_name = proto.Field(
+    column_spec_name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    column_display_name = proto.Field(
+    column_display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    feature_importance = proto.Field(
+    feature_importance: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/temporal.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/temporal.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -37,20 +39,20 @@
             start.
         end_time_offset (google.protobuf.duration_pb2.Duration):
             End of the time segment (exclusive),
             represented as the duration since the example
             start.
     """
 
-    start_time_offset = proto.Field(
+    start_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    end_time_offset = proto.Field(
+    end_time_offset: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=2,
         message=duration_pb2.Duration,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import classification
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -35,15 +37,15 @@
     r"""Dataset metadata for classification.
 
     Attributes:
         classification_type (google.cloud.automl_v1beta1.types.ClassificationType):
             Required. Type of the classification problem.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=1,
         enum=classification.ClassificationType,
     )
 
 
 class TextClassificationModelMetadata(proto.Message):
@@ -51,15 +53,15 @@
 
     Attributes:
         classification_type (google.cloud.automl_v1beta1.types.ClassificationType):
             Output only. Classification type of the
             dataset used to train this model.
     """
 
-    classification_type = proto.Field(
+    classification_type: classification.ClassificationType = proto.Field(
         proto.ENUM,
         number=3,
         enum=classification.ClassificationType,
     )
 
 
 class TextExtractionDatasetMetadata(proto.Message):
@@ -76,15 +78,15 @@
             -  ``default``: Use to train a general text extraction
                model. Default value.
 
             -  ``health_care``: Use to train a text extraction model
                that is tuned for healthcare applications.
     """
 
-    model_hint = proto.Field(
+    model_hint: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TextSentimentDatasetMetadata(proto.Message):
     r"""Dataset metadata for text sentiment.
@@ -96,15 +98,15 @@
             range of sentiments that will be used is between 0 and
             sentiment_max (inclusive on both ends), and all the values
             in the range must be represented in the dataset before a
             model can be created. sentiment_max value must be between 1
             and 10 (inclusive).
     """
 
-    sentiment_max = proto.Field(
+    sentiment_max: int = proto.Field(
         proto.INT32,
         number=1,
     )
 
 
 class TextSentimentModelMetadata(proto.Message):
     r"""Model metadata that is specific to text sentiment."""
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text_extraction.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/text_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import text_segment as gca_text_segment
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -41,34 +43,34 @@
             This field is a member of `oneof`_ ``annotation``.
         score (float):
             Output only. A confidence estimate between
             0.0 and 1.0. A higher value means greater
             confidence in correctness of the annotation.
     """
 
-    text_segment = proto.Field(
+    text_segment: gca_text_segment.TextSegment = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="annotation",
         message=gca_text_segment.TextSegment,
     )
-    score = proto.Field(
+    score: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
 
 
 class TextExtractionEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for text extraction problems.
 
     Attributes:
         au_prc (float):
             Output only. The Area under precision recall
             curve metric.
-        confidence_metrics_entries (Sequence[google.cloud.automl_v1beta1.types.TextExtractionEvaluationMetrics.ConfidenceMetricsEntry]):
+        confidence_metrics_entries (MutableSequence[google.cloud.automl_v1beta1.types.TextExtractionEvaluationMetrics.ConfidenceMetricsEntry]):
             Output only. Metrics that have confidence
             thresholds. Precision-recall curve can be
             derived from it.
     """
 
     class ConfidenceMetricsEntry(proto.Message):
         r"""Metrics for a single confidence threshold.
@@ -86,36 +88,38 @@
                 Output only. Precision under the given
                 confidence threshold.
             f1_score (float):
                 Output only. The harmonic mean of recall and
                 precision.
         """
 
-        confidence_threshold = proto.Field(
+        confidence_threshold: float = proto.Field(
             proto.FLOAT,
             number=1,
         )
-        recall = proto.Field(
+        recall: float = proto.Field(
             proto.FLOAT,
             number=3,
         )
-        precision = proto.Field(
+        precision: float = proto.Field(
             proto.FLOAT,
             number=4,
         )
-        f1_score = proto.Field(
+        f1_score: float = proto.Field(
             proto.FLOAT,
             number=5,
         )
 
-    au_prc = proto.Field(
+    au_prc: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    confidence_metrics_entries = proto.RepeatedField(
+    confidence_metrics_entries: MutableSequence[
+        ConfidenceMetricsEntry
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=ConfidenceMetricsEntry,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/text_sentiment.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1/types/text_sentiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
-from google.cloud.automl_v1beta1.types import classification
+from google.cloud.automl_v1.types import classification
 
 
 __protobuf__ = proto.module(
-    package="google.cloud.automl.v1beta1",
+    package="google.cloud.automl.v1",
     manifest={
         "TextSentimentAnnotation",
         "TextSentimentEvaluationMetrics",
     },
 )
 
 
 class TextSentimentAnnotation(proto.Message):
     r"""Contains annotation details specific to text sentiment.
 
     Attributes:
         sentiment (int):
             Output only. The sentiment with the semantic, as given to
             the
-            [AutoMl.ImportData][google.cloud.automl.v1beta1.AutoMl.ImportData]
+            [AutoMl.ImportData][google.cloud.automl.v1.AutoMl.ImportData]
             when populating the dataset from which the model used for
             the prediction had been trained. The sentiment values are
             between 0 and
             Dataset.text_sentiment_dataset_metadata.sentiment_max
             (inclusive), with higher value meaning more positive
             sentiment. They are completely relative, i.e. 0 means least
             positive sentiment and sentiment_max means the most positive
@@ -46,15 +48,15 @@
             e.g. if train data had only negative sentiment, then
             sentiment_max, would be still negative (although least
             negative). The sentiment shouldn't be confused with "score"
             or "magnitude" from the previous Natural Language Sentiment
             Analysis API.
     """
 
-    sentiment = proto.Field(
+    sentiment: int = proto.Field(
         proto.INT32,
         number=1,
     )
 
 
 class TextSentimentEvaluationMetrics(proto.Message):
     r"""Model evaluation metrics for text sentiment problems.
@@ -79,57 +81,52 @@
             Output only. Linear weighted kappa. Only set
             for the overall model evaluation, not for
             evaluation of a single annotation spec.
         quadratic_kappa (float):
             Output only. Quadratic weighted kappa. Only
             set for the overall model evaluation, not for
             evaluation of a single annotation spec.
-        confusion_matrix (google.cloud.automl_v1beta1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
+        confusion_matrix (google.cloud.automl_v1.types.ClassificationEvaluationMetrics.ConfusionMatrix):
             Output only. Confusion matrix of the
             evaluation. Only set for the overall model
             evaluation, not for evaluation of a single
             annotation spec.
-        annotation_spec_id (Sequence[str]):
-            Output only. The annotation spec ids used for
-            this evaluation. Deprecated .
     """
 
-    precision = proto.Field(
+    precision: float = proto.Field(
         proto.FLOAT,
         number=1,
     )
-    recall = proto.Field(
+    recall: float = proto.Field(
         proto.FLOAT,
         number=2,
     )
-    f1_score = proto.Field(
+    f1_score: float = proto.Field(
         proto.FLOAT,
         number=3,
     )
-    mean_absolute_error = proto.Field(
+    mean_absolute_error: float = proto.Field(
         proto.FLOAT,
         number=4,
     )
-    mean_squared_error = proto.Field(
+    mean_squared_error: float = proto.Field(
         proto.FLOAT,
         number=5,
     )
-    linear_kappa = proto.Field(
+    linear_kappa: float = proto.Field(
         proto.FLOAT,
         number=6,
     )
-    quadratic_kappa = proto.Field(
+    quadratic_kappa: float = proto.Field(
         proto.FLOAT,
         number=7,
     )
-    confusion_matrix = proto.Field(
-        proto.MESSAGE,
-        number=8,
-        message=classification.ClassificationEvaluationMetrics.ConfusionMatrix,
-    )
-    annotation_spec_id = proto.RepeatedField(
-        proto.STRING,
-        number=9,
+    confusion_matrix: classification.ClassificationEvaluationMetrics.ConfusionMatrix = (
+        proto.Field(
+            proto.MESSAGE,
+            number=8,
+            message=classification.ClassificationEvaluationMetrics.ConfusionMatrix,
+        )
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/translation.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/translation.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.automl_v1beta1.types import data_items
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
@@ -37,19 +39,19 @@
             Required. The BCP-47 language code of the
             source language.
         target_language_code (str):
             Required. The BCP-47 language code of the
             target language.
     """
 
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class TranslationEvaluationMetrics(proto.Message):
     r"""Evaluation metrics for the dataset.
@@ -57,19 +59,19 @@
     Attributes:
         bleu_score (float):
             Output only. BLEU score.
         base_bleu_score (float):
             Output only. BLEU score for base model.
     """
 
-    bleu_score = proto.Field(
+    bleu_score: float = proto.Field(
         proto.DOUBLE,
         number=1,
     )
-    base_bleu_score = proto.Field(
+    base_bleu_score: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
 
 
 class TranslationModelMetadata(proto.Message):
     r"""Model metadata that is specific to translation.
@@ -85,37 +87,37 @@
             The source languge (The BCP-47 language code)
             that is used for training.
         target_language_code (str):
             Output only. The target languge (The BCP-47
             language code) that is used for training.
     """
 
-    base_model = proto.Field(
+    base_model: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    source_language_code = proto.Field(
+    source_language_code: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    target_language_code = proto.Field(
+    target_language_code: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class TranslationAnnotation(proto.Message):
     r"""Annotation details specific to translation.
 
     Attributes:
         translated_content (google.cloud.automl_v1beta1.types.TextSnippet):
             Output only . The translated content.
     """
 
-    translated_content = proto.Field(
+    translated_content: data_items.TextSnippet = proto.Field(
         proto.MESSAGE,
         number=1,
         message=data_items.TextSnippet,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-automl-2.8.3/google/cloud/automl_v1beta1/types/video.py` & `google-cloud-automl-2.9.0/google/cloud/automl_v1beta1/types/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.cloud.automl.v1beta1",
     manifest={
         "VideoClassificationDatasetMetadata",
```

### Comparing `google-cloud-automl-2.8.3/google_cloud_automl.egg-info/PKG-INFO` & `google-cloud-automl-2.9.0/google_cloud_automl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: google-cloud-automl
-Version: 2.8.3
-Summary: Cloud AutoML API client library
+Version: 2.9.0
+Summary: Google Cloud Automl API client library
 Home-page: https://github.com/googleapis/python-automl
 Author: Google LLC
-Author-email: googleapis-packages@oogle.com
+Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-cloud-automl-2.8.3/google_cloud_automl.egg-info/SOURCES.txt` & `google-cloud-automl-2.9.0/google_cloud_automl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/__init__.py
 google/cloud/automl/__init__.py
+google/cloud/automl/gapic_version.py
 google/cloud/automl/py.typed
 google/cloud/automl_v1/__init__.py
 google/cloud/automl_v1/gapic_metadata.json
+google/cloud/automl_v1/gapic_version.py
 google/cloud/automl_v1/py.typed
 google/cloud/automl_v1/services/__init__.py
 google/cloud/automl_v1/services/auto_ml/__init__.py
 google/cloud/automl_v1/services/auto_ml/async_client.py
 google/cloud/automl_v1/services/auto_ml/client.py
 google/cloud/automl_v1/services/auto_ml/pagers.py
 google/cloud/automl_v1/services/auto_ml/transports/__init__.py
@@ -43,14 +45,15 @@
 google/cloud/automl_v1/types/text.py
 google/cloud/automl_v1/types/text_extraction.py
 google/cloud/automl_v1/types/text_segment.py
 google/cloud/automl_v1/types/text_sentiment.py
 google/cloud/automl_v1/types/translation.py
 google/cloud/automl_v1beta1/__init__.py
 google/cloud/automl_v1beta1/gapic_metadata.json
+google/cloud/automl_v1beta1/gapic_version.py
 google/cloud/automl_v1beta1/py.typed
 google/cloud/automl_v1beta1/services/__init__.py
 google/cloud/automl_v1beta1/services/auto_ml/__init__.py
 google/cloud/automl_v1beta1/services/auto_ml/async_client.py
 google/cloud/automl_v1beta1/services/auto_ml/client.py
 google/cloud/automl_v1beta1/services/auto_ml/pagers.py
 google/cloud/automl_v1beta1/services/auto_ml/transports/__init__.py
```

### Comparing `google-cloud-automl-2.8.3/scripts/fixup_automl_v1_keywords.py` & `google-cloud-automl-2.9.0/scripts/fixup_automl_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/scripts/fixup_automl_v1beta1_keywords.py` & `google-cloud-automl-2.9.0/scripts/fixup_automl_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/setup.py` & `google-cloud-automl-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,55 @@
-# Copyright 2018 Google LLC
+# -*- coding: utf-8 -*-
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
+
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-automl"
-description = "Cloud AutoML API client library"
-version = "2.8.3"
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Automl API client library"
+
+version = {}
+with open(os.path.join(package_root, "google/cloud/automl/gapic_version.py")) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
 dependencies = [
-    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 extras = {
     "libcst": "libcst >= 0.2.5",
     "pandas": ["pandas>=1.0.5"],
     "storage": ["google-cloud-storage >=1.18.0, <3.0.0dev"],
 }
+url = "https://github.com/googleapis/python-automl"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -50,17 +65,17 @@
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
-    author_email="googleapis-packages@oogle.com",
+    author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-automl",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -68,18 +83,18 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
     extras_require=extras,
-    python_requires=">=3.7",
     scripts=[
         "scripts/fixup_automl_v1_keywords.py",
         "scripts/fixup_automl_v1beta1_keywords.py",
     ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-automl-2.8.3/tests/__init__.py` & `google-cloud-automl-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/system/gapic/v1beta1/test_system_tables_client_v1.py` & `google-cloud-automl-2.9.0/tests/system/gapic/v1beta1/test_system_tables_client_v1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/__init__.py` & `google-cloud-automl-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/__init__.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/__init__.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/test_auto_ml.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/test_auto_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from google.cloud.automl_v1.types import service
 from google.cloud.automl_v1.types import text
 from google.cloud.automl_v1.types import text_extraction
 from google.cloud.automl_v1.types import text_sentiment
 from google.cloud.automl_v1.types import translation
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
+from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
```

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1/test_prediction_service.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1/test_prediction_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/__init__.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/test_auto_ml.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/test_auto_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from google.cloud.automl_v1beta1.types import text
 from google.cloud.automl_v1beta1.types import text_extraction
 from google.cloud.automl_v1beta1.types import text_sentiment
 from google.cloud.automl_v1beta1.types import translation
 from google.cloud.automl_v1beta1.types import video
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
+from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
```

### Comparing `google-cloud-automl-2.8.3/tests/unit/gapic/automl_v1beta1/test_prediction_service.py` & `google-cloud-automl-2.9.0/tests/unit/gapic/automl_v1beta1/test_prediction_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/test_gcs_client_v1beta1.py` & `google-cloud-automl-2.9.0/tests/unit/test_gcs_client_v1beta1.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automl-2.8.3/tests/unit/test_tables_client_v1beta1.py` & `google-cloud-automl-2.9.0/tests/unit/test_tables_client_v1beta1.py`

 * *Files identical despite different names*

