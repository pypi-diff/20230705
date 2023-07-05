# Comparing `tmp/graphium-2.0.2.tar.gz` & `tmp/graphium-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphium-2.0.2.tar", last modified: Sat Jun 17 20:05:20 2023, max compression
+gzip compressed data, was "graphium-2.1.0.tar", last modified: Wed Jul  5 16:33:07 2023, max compression
```

## Comparing `graphium-2.0.2.tar` & `graphium-2.1.0.tar`

### file list

```diff
@@ -1,302 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.307239 graphium-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-17 20:01:04.000000 graphium-2.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-17 20:01:04.000000 graphium-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-17 20:01:04.000000 graphium-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-17 20:05:20.307239 graphium-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-17 20:01:04.000000 graphium-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-17 20:01:04.000000 graphium-2.0.2/cleanup_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.259239 graphium-2.0.2/docs/_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/docs/_assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/_assets/css/custom-graphium.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/_assets/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.config.md
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.data.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.features.md
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.ipu.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/docs/api/graphium.nn/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.nn/architectures.md
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.nn/encoders.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.nn/graphium.nn.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.nn/pyg_layers.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/api/graphium.visualization.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/baseline.md
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/cli_references.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/design.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.267239 graphium-2.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/images/datamodule.png
--rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/images/full_graph_network.png
--rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/pretrained_models.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.263239 graphium-2.0.2/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/docs/tutorials/feature_processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/feature_processing/timing_parallel.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/docs/tutorials/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/gnn/making_gnn_networks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/gnn/using_gnn_layers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/docs/tutorials/model_training/
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/model_training/config_ipu_tutorials.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    69215 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/model_training/ipu_training.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/model_training/ipu_training_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-06-17 20:01:04.000000 graphium-2.0.2/docs/tutorials/model_training/simple-molecular-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-17 20:01:04.000000 graphium-2.0.2/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/expts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/expts/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_gps_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_gpspp_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_mpnn_10M_b3lyp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_mpnn_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/configs/config_mpnn_pcqm4m.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.271239 graphium-2.0.2/expts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/data/micro_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/data/tiny_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/dataset_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/main_run_get_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/main_run_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/main_run_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/main_run_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.275239 graphium-2.0.2/expts/neurips2023_configs/
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_classifigression_l1000.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_large_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_large_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_large_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_large_mpnn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_luis_jama.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_small_gated_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_small_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_small_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_small_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/neurips2023_configs/config_small_mpnn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-17 20:01:04.000000 graphium-2.0.2/expts/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.275239 graphium-2.0.2/graphium/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.275239 graphium-2.0.2/graphium/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.275239 graphium-2.0.2/graphium/config/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/config_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/fake_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/config/zinc_default_multitask_pyg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/L1000/
--rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/QM9/
--rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/QM9/micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191171 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/QM9/micro_qm9.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/QM9/norm_micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)   106509 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26459 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/make_data_splits/
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/micro_ZINC/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/micro_ZINC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/micro_ZINC/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/multilevel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.279239 graphium-2.0.2/graphium/data/multitask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/multitask/tiny_ZINC_SA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/multitask/tiny_ZINC_logp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/multitask/tiny_ZINC_score.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/sdf2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.283239 graphium-2.0.2/graphium/data/single_atom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/single_atom_dataset/single_atom_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/smiles_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.283239 graphium-2.0.2/graphium/expts/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/expts/pyg_batching_sparse.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.283239 graphium-2.0.2/graphium/features/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/commute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    46861 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/nmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/periodic_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/test_new_pes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/features/transfer_pos_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.287239 graphium-2.0.2/graphium/ipu/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    36426 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_simple_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/ipu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/ipu/to_dense_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.287239 graphium-2.0.2/graphium/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.287239 graphium-2.0.2/graphium/nn/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/architectures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/architectures/encoder_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    73086 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/architectures/global_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/architectures/pyg_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/base_graph_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/base_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.287239 graphium-2.0.2/graphium/nn/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/bessel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/laplace_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/mlp_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/encoders/signnet_pos_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.291239 graphium-2.0.2/graphium/nn/pyg_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/dimenet_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/gated_gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/gin_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/gps_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/mpnn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/pna_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/pooling_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/pyg_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.291239 graphium-2.0.2/graphium/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/predictor_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/trainer/predictor_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.295239 graphium-2.0.2/graphium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/custom_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/moving_average_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/mup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/safe_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/utils/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.295239 graphium-2.0.2/graphium/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/visualization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-17 20:01:04.000000 graphium-2.0.2/graphium/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.275239 graphium-2.0.2/graphium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 20:05:20.000000 graphium-2.0.2/graphium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-17 20:01:04.000000 graphium-2.0.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.295239 graphium-2.0.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev-datamodule-invalidate-cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev-datamodule-ogb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev-datamodule.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev-pretrained.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev-training-loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/running-fingerprints-from-pretrained-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-17 20:01:04.000000 graphium-2.0.2/notebooks/running-model-from-config.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.295239 graphium-2.0.2/profiling/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-17 20:01:04.000000 graphium-2.0.2/profiling/configs_profiling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-17 20:01:04.000000 graphium-2.0.2/profiling/profile_mol_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-17 20:01:04.000000 graphium-2.0.2/profiling/profile_one_of_k_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-17 20:01:04.000000 graphium-2.0.2/profiling/profile_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-17 20:01:04.000000 graphium-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-17 20:01:04.000000 graphium-2.0.2/requirements_ipu.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.295239 graphium-2.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-17 20:01:04.000000 graphium-2.0.2/scripts/convert_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-17 20:01:04.000000 graphium-2.0.2/scripts/ipu_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-17 20:01:04.000000 graphium-2.0.2/scripts/ipu_venv.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:05:20.307239 graphium-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.303239 graphium-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/config_test_ipu_dataloader.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/converted_fake_multilevel_data.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:05:20.303239 graphium-2.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/config_micro_ZINC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC_corrupt.csv
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC_shard_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC_shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC_shard_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/micro_ZINC_shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/data/pcqm4mv2-2k.csv
--rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/fake_and_missing_multilevel_data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_base_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12591 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_mtl_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_multitask_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_mup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_pe_nodepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_pe_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_pe_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_pos_transfer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_positional_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_positional_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_pyg_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-17 20:01:04.000000 graphium-2.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.911317 graphium-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.863316 graphium-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.863316 graphium-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-05 16:28:36.000000 graphium-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-05 16:28:36.000000 graphium-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-05 16:28:36.000000 graphium-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-05 16:33:07.911317 graphium-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-05 16:28:36.000000 graphium-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-05 16:28:36.000000 graphium-2.1.0/cleanup_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.867316 graphium-2.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.859315 graphium-2.1.0/docs/_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.867316 graphium-2.1.0/docs/_assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/_assets/css/custom-graphium.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/_assets/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.867316 graphium-2.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.config.md
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.ipu.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.867316 graphium-2.1.0/docs/api/graphium.nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.nn/architectures.md
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.nn/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.nn/graphium.nn.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.nn/pyg_layers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/api/graphium.visualization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/baseline.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/cli_references.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/design.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.867316 graphium-2.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/images/datamodule.png
+-rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/images/full_graph_network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/pretrained_models.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.859315 graphium-2.1.0/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/docs/tutorials/feature_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/feature_processing/choosing_parallelization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/feature_processing/csv_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/feature_processing/timing_parallel.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/docs/tutorials/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/gnn/add_new_gnn_layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/gnn/making_gnn_networks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/gnn/using_gnn_layers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/docs/tutorials/model_training/
+-rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/model_training/running-multitask-ipu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-05 16:28:36.000000 graphium-2.1.0/docs/tutorials/model_training/simple-molecular-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-05 16:28:36.000000 graphium-2.1.0/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/expts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/expts/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_gps_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_gps_10M_pcqm4m_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_gpspp_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_mpnn_10M_b3lyp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_mpnn_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/configs/config_mpnn_pcqm4m.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.871316 graphium-2.1.0/expts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/data/micro_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/data/tiny_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/dataset_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/main_run_get_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/main_run_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/main_run_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/main_run_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_classifigression_l1000.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_large_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_large_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_large_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_large_mpnn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_luis_jama.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_small_gated_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_small_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_small_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_small_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/config_small_mpnn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/debug/config_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/single_task_gcn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/run_validation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-05 16:28:36.000000 graphium-2.1.0/expts/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.875316 graphium-2.1.0/graphium/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.879316 graphium-2.1.0/graphium/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.879316 graphium-2.1.0/graphium/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/config_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/fake_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/config/zinc_default_multitask_pyg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/L1000/
+-rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/QM9/
+-rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/QM9/micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/QM9/micro_qm9.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/QM9/norm_micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/make_data_splits/
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/micro_ZINC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/micro_ZINC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/micro_ZINC/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/multilevel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/multitask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/multitask/tiny_ZINC_SA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/multitask/tiny_ZINC_logp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/multitask/tiny_ZINC_score.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/sdf2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.883316 graphium-2.1.0/graphium/data/single_atom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/single_atom_dataset/single_atom_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/smiles_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.887316 graphium-2.1.0/graphium/expts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/expts/pyg_batching_sparse.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.887316 graphium-2.1.0/graphium/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/commute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/nmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/periodic_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/test_new_pes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/features/transfer_pos_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.887316 graphium-2.1.0/graphium/ipu/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_simple_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/ipu_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/ipu/to_dense_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.891316 graphium-2.1.0/graphium/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.891316 graphium-2.1.0/graphium/nn/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/architectures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/architectures/encoder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/architectures/global_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/architectures/pyg_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/base_graph_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/base_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.891316 graphium-2.1.0/graphium/nn/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/bessel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/laplace_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/mlp_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/encoders/signnet_pos_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.891316 graphium-2.1.0/graphium/nn/pyg_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/dimenet_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/gated_gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/gin_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/gps_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/mpnn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/pna_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/pooling_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/pyg_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.895316 graphium-2.1.0/graphium/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/predictor_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/trainer/predictor_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.895316 graphium-2.1.0/graphium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/custom_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/moving_average_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/safe_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/utils/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.895316 graphium-2.1.0/graphium/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/visualization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-05 16:28:36.000000 graphium-2.1.0/graphium/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.879316 graphium-2.1.0/graphium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 16:33:07.000000 graphium-2.1.0/graphium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 16:28:36.000000 graphium-2.1.0/lightning.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-05 16:28:36.000000 graphium-2.1.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.899316 graphium-2.1.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev-datamodule-invalidate-cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev-datamodule-ogb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev-datamodule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev-pretrained.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev-training-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/running-fingerprints-from-pretrained-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-05 16:28:36.000000 graphium-2.1.0/notebooks/running-model-from-config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.899316 graphium-2.1.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-05 16:28:36.000000 graphium-2.1.0/profiling/configs_profiling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-05 16:28:36.000000 graphium-2.1.0/profiling/profile_mol_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-05 16:28:36.000000 graphium-2.1.0/profiling/profile_one_of_k_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-05 16:28:36.000000 graphium-2.1.0/profiling/profile_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-05 16:28:36.000000 graphium-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-05 16:28:36.000000 graphium-2.1.0/requirements_ipu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.899316 graphium-2.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-05 16:28:36.000000 graphium-2.1.0/scripts/convert_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-05 16:28:36.000000 graphium-2.1.0/scripts/ipu_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-05 16:28:36.000000 graphium-2.1.0/scripts/ipu_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:33:07.911317 graphium-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.907317 graphium-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/config_test_ipu_dataloader.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/converted_fake_multilevel_data.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:33:07.907317 graphium-2.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/config_micro_ZINC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC_corrupt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC_shard_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC_shard_1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC_shard_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/micro_ZINC_shard_2.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/data/pcqm4mv2-2k.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/fake_and_missing_multilevel_data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_base_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_mtl_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_multitask_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_pe_nodepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_pe_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_pe_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_pos_transfer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_positional_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_positional_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_pyg_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-05 16:28:36.000000 graphium-2.1.0/tests/test_utils.py
```

### Comparing `graphium-2.0.2/.github/CODE_OF_CONDUCT.md` & `graphium-2.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/.github/workflows/code-check.yml` & `graphium-2.1.0/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/.github/workflows/doc.yml` & `graphium-2.1.0/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/.github/workflows/release.yml` & `graphium-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/.github/workflows/test.yml` & `graphium-2.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/.gitignore` & `graphium-2.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 out/
 saved_models/
 wandb/
 out/
 datacache/
 tests/temp_cache*
 predictions/
+draft/
 
 # Data and predictions
 graphium/data/ZINC_bench_gnn/
 graphium/data/BindingDB/
 graphium/data/mega-pubchem/
 graphium/data/cache/
 graphium/data/b3lyp/
```

### Comparing `graphium-2.0.2/LICENSE` & `graphium-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/PKG-INFO` & `graphium-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.0.2
+Version: 2.1.0
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,33 +27,38 @@
 
 <div align="center">
     <img src="docs/images/logo.png" height="200px">
     <h3>Scaling molecular GNNs to infinity</h3>
 </div>
 
 ---
-
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
 
+
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
 - ⮔ Read-to-use training loop based on [Pytorch Lightning](https://www.pytorchlightning.ai/).
 - 🔌 Have a new dataset? Graphium provides a simple plug-and-play interface. Change the path, the name of the columns to predict, the atomic featurization, and you’re ready to play!
 
 ## Documentation
 
 Visit https://graphium-docs.datamol.io/.
 
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
+
+You can try running Graphium on Graphcore IPUs for free on Gradient by clicking on the button above.
+
 ## Installation for developers
 
 ### For CPU and GPU developers
 
 Use [`mamba`](https://github.com/mamba-org/mamba):
 
 ```bash
@@ -68,22 +73,23 @@
 ### For IPU developers
 
 ```bash
 mkdir ~/.venv                               # Create the folder for the environment
 python3 -m venv ~/.venv/graphium_ipu        # Create the environment
 source ~/.venv/graphium_ipu/bin/activate    # Activate the environment
 
-# Installing the poptorch SDK. Make sure to change the path
+# Install the PopTorch wheel
 pip install PATH_TO_SDK/poptorch-3.2.0+109946_bb50ce43ab_ubuntu_20_04-cp38-cp38-linux_x86_64.whl
 
-# Activate poplar SDK.
+# Enable Poplar SDK (including Poplar and PopART)
 source PATH_TO_SDK/enable
 
 # Install the IPU specific and graphium requirements
 PACKAGE_NAME=pytorch pip install -r requirements_ipu.txt
+pip install -r lightning.txt
 
 # Install Graphium in dev mode
 pip install --no-deps -e .
 ```
 
 ## Training a model
```

### Comparing `graphium-2.0.2/README.md` & `graphium-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 <div align="center">
     <img src="docs/images/logo.png" height="200px">
     <h3>Scaling molecular GNNs to infinity</h3>
 </div>
 
 ---
-
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
 
+
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
 - ⮔ Read-to-use training loop based on [Pytorch Lightning](https://www.pytorchlightning.ai/).
 - 🔌 Have a new dataset? Graphium provides a simple plug-and-play interface. Change the path, the name of the columns to predict, the atomic featurization, and you’re ready to play!
 
 ## Documentation
 
 Visit https://graphium-docs.datamol.io/.
 
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
+
+You can try running Graphium on Graphcore IPUs for free on Gradient by clicking on the button above.
+
 ## Installation for developers
 
 ### For CPU and GPU developers
 
 Use [`mamba`](https://github.com/mamba-org/mamba):
 
 ```bash
@@ -41,22 +46,23 @@
 ### For IPU developers
 
 ```bash
 mkdir ~/.venv                               # Create the folder for the environment
 python3 -m venv ~/.venv/graphium_ipu        # Create the environment
 source ~/.venv/graphium_ipu/bin/activate    # Activate the environment
 
-# Installing the poptorch SDK. Make sure to change the path
+# Install the PopTorch wheel
 pip install PATH_TO_SDK/poptorch-3.2.0+109946_bb50ce43ab_ubuntu_20_04-cp38-cp38-linux_x86_64.whl
 
-# Activate poplar SDK.
+# Enable Poplar SDK (including Poplar and PopART)
 source PATH_TO_SDK/enable
 
 # Install the IPU specific and graphium requirements
 PACKAGE_NAME=pytorch pip install -r requirements_ipu.txt
+pip install -r lightning.txt
 
 # Install Graphium in dev mode
 pip install --no-deps -e .
 ```
 
 ## Training a model
```

### Comparing `graphium-2.0.2/docs/_assets/css/custom-graphium.css` & `graphium-2.1.0/docs/_assets/css/custom-graphium.css`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/_assets/css/custom.css` & `graphium-2.1.0/docs/_assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/api/graphium.features.md` & `graphium-2.1.0/docs/api/graphium.features.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/api/graphium.ipu.md` & `graphium-2.1.0/docs/api/graphium.ipu.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/api/graphium.nn/encoders.md` & `graphium-2.1.0/docs/api/graphium.nn/encoders.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/api/graphium.nn/pyg_layers.md` & `graphium-2.1.0/docs/api/graphium.nn/pyg_layers.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/api/graphium.utils.md` & `graphium-2.1.0/docs/api/graphium.utils.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/datasets.md` & `graphium-2.1.0/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/design.md` & `graphium-2.1.0/docs/design.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/images/datamodule.png` & `graphium-2.1.0/docs/images/datamodule.png`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/images/full_graph_network.png` & `graphium-2.1.0/docs/images/full_graph_network.png`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/images/logo.png` & `graphium-2.1.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/images/logo.svg` & `graphium-2.1.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/pretrained_models.md` & `graphium-2.1.0/docs/pretrained_models.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb` & `graphium-2.1.0/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981617647058824%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}}"}*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Add new positional encoding\n",
                 "\n",
                 "One of the main advantage of this library is the ability to easily incorporate novel positional encodings on the node, edge and graph level. The positional encodings are computed and feed into respective encoders and then the hidden embeddings from all pe encoders are pooled (according to if they are node, edge, or graph level) and then feed into the GNN layers as features. The designs allow any combination of positional encodings to be used by modifying the configuration file. For more details on the data processing part, please visit the [design page of the doc](https://graphium-docs.datamol.io/stable/design.html).\n",
                 "\n",
```

### Comparing `graphium-2.0.2/docs/tutorials/feature_processing/choosing_parallelization.ipynb` & `graphium-2.1.0/docs/tutorials/feature_processing/timing_parallel.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333333%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Timing parallel processing\\n')], delete: [0]}}}"}*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "0693c5c9",
             "metadata": {},
             "source": [
-                "# Choosing the right parallelization\n",
+                "# Timing parallel processing\n",
                 "\n",
                 "This tutorial is meant to help you benchmark different parallel processing methods for the processing of molecules into graphs. This will allow you to chose the one most suitable for your machine, since the benchmarks vary per machine.\n",
                 "\n",
                 "In general, we find that using `joblib` with the `loky` parallel processing and a batch size of `1000` is most beneficial. The logic is abstracted into `datamol.parallelized_with_batches`"
             ]
         },
         {
```

### Comparing `graphium-2.0.2/docs/tutorials/feature_processing/csv_to_parquet.ipynb` & `graphium-2.1.0/docs/tutorials/feature_processing/csv_to_parquet.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9298958333333334%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'source': {delete: [7, 5, 4, 2, 1, 0]}}, 1: "*

 * *            "{'execution_count': 2}, 2: {'execution_count': 2, 'outputs': {0: {'text': "*

 * *            "['/nethome/andyh/graphium/docs/tutorials/feature_processing\\r\\n']}}}, 3: "*

 * *            "{'outputs': []}, insert: [(4, OrderedDict([('cell_type', 'code'), ('execution_count', "*

 * *            "None), ('metadata', OrderedDict()), ('outputs', []), ('source', [])]))]}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3  […]*

```diff
@@ -1,91 +1,81 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import os\n",
-                "import pyarrow as pa\n",
-                "import pyarrow.parquet as pq\n",
                 "import pandas as pd\n",
-                "from google.cloud import storage\n",
-                "from io import StringIO\n",
                 "import graphium\n",
-                "import os\n",
                 "from os.path import dirname, abspath\n",
                 "\n",
                 "MAIN_DIR = dirname(dirname(abspath(graphium.__file__)))\n",
                 "\n",
                 "# TODO create funciton to read parquet, test from GCP storage (put it in path, should support gs and path, explore function from Pandas instead of parquet \"pq\")\n",
                 "def _csv_to_parquet(csv_path, parquet_path):\n",
                 "    df = pd.read_csv(csv_path)\n",
                 "    df.to_parquet(parquet_path)\n",
                 "\n",
                 "_csv_to_parquet(MAIN_DIR + '/graphium/data/QM9/micro_qm9.csv', MAIN_DIR + '/graphium/data/QM9/micro_qm9.parquet')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "    # TODO create funciton to specify if you read parquet or csv\n",
                 "    # TODO replace all location with call for _read_csv and make sure to read all files if path ends with \"*\"\n",
                 "    # def read_table:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "/home/oleksandr/code/graphium/docs/tutorials/basics\n"
+                        "/nethome/andyh/graphium/docs/tutorials/feature_processing\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pwd"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "'/home/oleksandr/code/graphium/graphium'"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import graphium\n",
                 "import os\n",
                 "from os.path import dirname, abspath\n",
                 "MAIN_DIR = dirname(dirname(abspath(graphium.__file__)))\n",
                 "os.chdir(MAIN_DIR) # No need for this file"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.8.10 ('graphium_ipu')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -93,15 +83,14 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.8.10"
         },
-        "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "b813b16c721ca8d9e65e6e6945a38a6ae48015ae799c455bab639da90d3bb278"
             }
         }
     },
     "nbformat": 4,
```

### Comparing `graphium-2.0.2/docs/tutorials/feature_processing/timing_parallel.ipynb` & `graphium-2.1.0/docs/tutorials/feature_processing/choosing_parallelization.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940157666618441%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Choosing the right parallelization\\n')], delete: "*

 * *            "[0]}, delete: ['attachments']}, 8: {'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'3e939cd3a24742038b804bbfd961377d'}}}}}, 10: {'execution_count': 6, 'outputs': {0: "*

 * *            "{'data': {'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'0187ede3dbd8429995511883319e246f'}}}, 1: {'data': "*

 * *            "{'applic […]*

```diff
@@ -1,16 +1,15 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "0693c5c9",
             "metadata": {},
             "source": [
-                "# Timing parallel processing\n",
+                "# Choosing the right parallelization\n",
                 "\n",
                 "This tutorial is meant to help you benchmark different parallel processing methods for the processing of molecules into graphs. This will allow you to chose the one most suitable for your machine, since the benchmarks vary per machine.\n",
                 "\n",
                 "In general, we find that using `joblib` with the `loky` parallel processing and a batch size of `1000` is most beneficial. The logic is abstracted into `datamol.parallelized_with_batches`"
             ]
         },
         {
@@ -135,15 +134,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "b2e528726a384b258d6ed3576bc0db1c",
+                            "model_id": "3e939cd3a24742038b804bbfd961377d",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/133885 [00:00<?, ?it/s]"
                         ]
                     },
@@ -181,66 +180,66 @@
             "metadata": {},
             "source": [
                 "### Batch"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "845a72d5-0b3f-4a21-8d7d-8312671e9924",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "85e79375f3e94d9abc435bdc8d28d2df",
+                            "model_id": "0187ede3dbd8429995511883319e246f",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/13388 [00:00<?, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "f5df65b3d2474b02aff1058e044f7dcf",
+                            "model_id": "fdd5ac6375b444359f6e8cef7b755b9b",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/1338 [00:00<?, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3a5170b0055e4971bd0ea5e7b6cdcbd8",
+                            "model_id": "c11c5894843a46848725d0c03fef9e02",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/133 [00:00<?, ?it/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "fa091db65b454db4bc824439645290ad",
+                            "model_id": "bd34e1a806604192bbd6f95ba6435b44",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "  0%|          | 0/13 [00:00<?, ?it/s]"
                         ]
                     },
@@ -282,15 +281,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "a9de4fa3630e4c9aa4d81cac4f10b4c8",
+                            "model_id": "928c2236948d4a109c79a6bc79bd4649",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "VBox(children=(HBox(children=(IntProgress(value=0, description='0.00%', max=558), Label(value='0 / 558'))), HB\u2026"
                         ]
                     },
@@ -364,89 +363,89 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>True</td>\n",
                             "      <td>1000.0</td>\n",
                             "      <td>loky_processes</td>\n",
-                            "      <td>0.014199</td>\n",
-                            "      <td>0.851930</td>\n",
+                            "      <td>0.015375</td>\n",
+                            "      <td>0.922496</td>\n",
                             "      <td>133885</td>\n",
-                            "      <td>0.000006</td>\n",
+                            "      <td>0.000007</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>True</td>\n",
                             "      <td>100.0</td>\n",
                             "      <td>loky_processes</td>\n",
-                            "      <td>0.037132</td>\n",
-                            "      <td>2.227947</td>\n",
+                            "      <td>0.037034</td>\n",
+                            "      <td>2.222021</td>\n",
                             "      <td>133885</td>\n",
                             "      <td>0.000017</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>True</td>\n",
                             "      <td>10000.0</td>\n",
                             "      <td>loky_processes</td>\n",
-                            "      <td>0.047438</td>\n",
-                            "      <td>2.846266</td>\n",
+                            "      <td>0.055083</td>\n",
+                            "      <td>3.304987</td>\n",
                             "      <td>133885</td>\n",
-                            "      <td>0.000021</td>\n",
+                            "      <td>0.000025</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>pandarallel</td>\n",
-                            "      <td>0.118230</td>\n",
-                            "      <td>7.093791</td>\n",
+                            "      <td>0.121338</td>\n",
+                            "      <td>7.280271</td>\n",
                             "      <td>133885</td>\n",
-                            "      <td>0.000053</td>\n",
+                            "      <td>0.000054</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>True</td>\n",
                             "      <td>10.0</td>\n",
                             "      <td>loky_processes</td>\n",
-                            "      <td>0.222177</td>\n",
-                            "      <td>13.330603</td>\n",
+                            "      <td>0.165935</td>\n",
+                            "      <td>9.956113</td>\n",
                             "      <td>133885</td>\n",
-                            "      <td>0.000100</td>\n",
+                            "      <td>0.000074</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>loky_processes</td>\n",
-                            "      <td>4.002346</td>\n",
-                            "      <td>240.140754</td>\n",
+                            "      <td>3.639053</td>\n",
+                            "      <td>218.343192</td>\n",
                             "      <td>133885</td>\n",
-                            "      <td>0.001794</td>\n",
+                            "      <td>0.001631</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   batch  batch_size       scheduler  duration_minutes  duration_seconds   \n",
-                            "3   True      1000.0  loky_processes          0.014199          0.851930  \\\n",
-                            "2   True       100.0  loky_processes          0.037132          2.227947   \n",
-                            "4   True     10000.0  loky_processes          0.047438          2.846266   \n",
-                            "5  False         NaN     pandarallel          0.118230          7.093791   \n",
-                            "1   True        10.0  loky_processes          0.222177         13.330603   \n",
-                            "0  False         NaN  loky_processes          4.002346        240.140754   \n",
+                            "   batch  batch_size       scheduler  duration_minutes  duration_seconds  \\\n",
+                            "3   True      1000.0  loky_processes          0.015375          0.922496   \n",
+                            "2   True       100.0  loky_processes          0.037034          2.222021   \n",
+                            "4   True     10000.0  loky_processes          0.055083          3.304987   \n",
+                            "5  False         NaN     pandarallel          0.121338          7.280271   \n",
+                            "1   True        10.0  loky_processes          0.165935          9.956113   \n",
+                            "0  False         NaN  loky_processes          3.639053        218.343192   \n",
                             "\n",
                             "   n_rows  duration_seconds_per_mol  \n",
-                            "3  133885                  0.000006  \n",
+                            "3  133885                  0.000007  \n",
                             "2  133885                  0.000017  \n",
-                            "4  133885                  0.000021  \n",
-                            "5  133885                  0.000053  \n",
-                            "1  133885                  0.000100  \n",
-                            "0  133885                  0.001794  "
+                            "4  133885                  0.000025  \n",
+                            "5  133885                  0.000054  \n",
+                            "1  133885                  0.000074  \n",
+                            "0  133885                  0.001631  "
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -472,15 +471,15 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "graphium_ipu",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
```

### Comparing `graphium-2.0.2/docs/tutorials/gnn/add_new_gnn_layers.ipynb` & `graphium-2.1.0/docs/tutorials/gnn/add_new_gnn_layers.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9652101224184845%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'One of the primary advantage of this library is the "*

 * *            'fact that GNN layers are independent from model architecture, thus allowing more '*

 * *            'flexibility with the code by easily swapping different layer types as '*

 * *            'hyper-parameters. However, this requires that the layers be implemented using the PyG '*

 * *            'library, and must be inherited from the class '*

 * *            '[`BaseGraphStructure`](https://graphium-docs.datamol.io/sta […]*

```diff
@@ -1,81 +1,86 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Creating GNN layers\n",
                 "\n",
-                "One of the primary advantage of the current library is the fact that GNN layers are independant from model architecture, thus allowing more flexibility with the code by easily swapping different layer types as hyper-parameters. However, this requires that the layers be implemented using the PyG library, and must be inherited from the class [`BaseGraphStructure`](https://graphium-docs.datamol.io/stable/api/graphium.nn/graphium.nn.html#graphium.nn.base_graph_layer.BaseGraphStructure), which standardizes the inputs, outputs and properties of the layers. Thus, the architecture can be handled independantly using the class [`FeedForwardPyg`](https://graphium-docs.datamol.io/stable/api/graphium.nn/architectures.html#graphium.nn.architectures.pyg_architectures.FeedForwardPyg) or other custom classes.\n",
+                "One of the primary advantage of this library is the fact that GNN layers are independent from model architecture, thus allowing more flexibility with the code by easily swapping different layer types as hyper-parameters. However, this requires that the layers be implemented using the PyG library, and must be inherited from the class [`BaseGraphStructure`](https://graphium-docs.datamol.io/stable/api/graphium.nn/graphium.nn.html#graphium.nn.base_graph_layer.BaseGraphStructure), which standardizes the inputs, outputs and properties of the layers. Thus, the architecture can be handled independantly using the class [`FeedForwardPyg`](https://graphium-docs.datamol.io/stable/api/graphium.nn/architectures.html#graphium.nn.architectures.pyg_architectures.FeedForwardPyg) or other custom classes.\n",
                 "\n",
                 "We will first start by a simple layer that does not use edges, to a more complex layer that uses edges.\n",
                 "\n",
                 "Since these examples are built on top of PyG, we recommend looking at their [Docs](https://pytorch-geometric.readthedocs.io/en/latest/) and [Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/get_started/introduction.html) for more info. "
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Table of content\n",
-                "1. [define test graph](#Define-synthetic-test-graph)\n",
-                "2. [create simple layer](#Creating-a-simple-layer)\n",
-                "3. [test simple layer](#Test-our-simple-layer)\n",
-                "4. [create complex layer](#Creating-a-complex-layer-with-edges)\n",
-                "5. [test complex layer](#Test-our-complex-layer) "
+                "1. [Define test graph](#Define-synthetic-test-graph)\n",
+                "2. [Create simple layer](#Creating-a-simple-layer)\n",
+                "3. [Test simple layer](#Test-our-simple-layer)\n",
+                "4. [Create complex layer](#Creating-a-complex-layer-with-edges)\n",
+                "5. [Test complex layer](#Test-our-complex-layer) "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 81,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "The autoreload extension is already loaded. To reload it, use:\n",
+                        "  %reload_ext autoreload\n"
+                    ]
+                }
+            ],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
                 "from torch import Tensor\n",
-                "import torch_geometric as pyg\n",
                 "from torch_geometric.data import Data, Batch\n",
                 "from torch_geometric.nn.conv import MessagePassing\n",
                 "from torch_scatter import scatter\n",
                 "from torch_geometric.typing import (\n",
-                "    Adj,\n",
                 "    OptPairTensor,\n",
-                "    OptTensor,\n",
-                "    Size,\n",
-                "    SparseTensor,\n",
+                "    OptTensor\n",
                 ")\n",
                 "\n",
-                "\n",
-                "\n",
                 "from copy import deepcopy\n",
                 "from typing import Callable, Union, Optional, List\n",
                 "from graphium.nn.base_graph_layer import BaseGraphStructure\n",
                 "from graphium.nn.base_layers import FCLayer\n",
                 "from graphium.utils.decorators import classproperty\n",
                 "\n",
-                "\n",
                 "_ = torch.manual_seed(42)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Define synthetic test graph\n",
                 "\n",
                 "We define below a small batched graph on which we can test the created layers. You can also use synthetic graphs to define unit tests "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 82,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "DataBatch(edge_index=[2, 7], feat=[7, 5], edge_feat=[7, 13], batch=[7], ptr=[3])\n"
@@ -86,38 +91,40 @@
                 "in_dim = 5          # Input node-feature dimensions\n",
                 "out_dim = 11        # Desired output node-feature dimensions\n",
                 "in_dim_edges = 13   # Input edge-feature dimensions\n",
                 "\n",
                 "\n",
                 "# Let's create 2 simple pyg graphs. \n",
                 "# start by specifying the edges with edge index\n",
-                "edge_idx1 = torch.stack([torch.tensor([0, 1, 2]), torch.tensor([1, 2, 3])])\n",
-                "edge_idx2 = torch.stack([torch.tensor([0, 0, 0, 1]), torch.tensor([0, 1, 2, 0])])\n",
+                "edge_idx1 = torch.tensor([[0, 1, 2],\n",
+                "                          [1, 2, 3]])\n",
+                "edge_idx2 = torch.tensor([[2, 0, 0, 1],\n",
+                "                          [0, 1, 2, 0]])\n",
                 "\n",
                 "# specify the node features, convention with variable x\n",
                 "x1 = torch.randn(edge_idx1.max() + 1, in_dim, dtype=torch.float32)\n",
                 "x2 = torch.randn(edge_idx2.max() + 1, in_dim, dtype=torch.float32)\n",
                 "\n",
                 "# specify the edge features in e\n",
                 "e1 = torch.randn(edge_idx1.shape[-1], in_dim_edges, dtype=torch.float32)\n",
                 "e2 = torch.randn(edge_idx2.shape[-1], in_dim_edges, dtype=torch.float32)\n",
                 "\n",
-                "\n",
                 "# make the pyg graph objects with our constructed features\n",
                 "g1 = Data(feat=x1, edge_index=edge_idx1, edge_feat=e1)\n",
                 "g2 = Data(feat=x2, edge_index=edge_idx2, edge_feat=e2)\n",
                 "\n",
                 "# put the two graphs into a Batch graph\n",
                 "bg = Batch.from_data_list([g1, g2])\n",
                 "\n",
                 "# The batched graph will show as a single graph with 7 nodes\n",
                 "print(bg)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a simple layer\n",
                 "\n",
                 "Here, we will show how to create a GNN layer that simples does a mean aggregation on the neighbouring features.\n",
                 "\n",
@@ -131,30 +138,30 @@
                 "- [`out_dim_factor`](https://graphium-docs.datamol.io/stable/api/graphium.nn/graphium.nn.html#graphium.nn.base_graph_layer.BaseGraphStructure.out_dim_factor): We want to return `1` since the output dimension does not depend on internal parameters.\n",
                 "\n",
                 "The example is given below"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 83,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#inherent from message passing class from pyg \n",
-                "#inherent from BaseGraphStructure\n",
+                "# inherit from message passing class from pyg \n",
+                "# inherit from BaseGraphStructure\n",
                 "# this example is also based of : https://pytorch-geometric.readthedocs.io/en/latest/_modules/torch_geometric/nn/conv/simple_conv.html#SimpleConv.forward\n",
                 "\n",
                 "class SimpleMeanLayer(MessagePassing, BaseGraphStructure):\n",
                 "    def __init__(self, \n",
                 "                 in_dim: int, \n",
                 "                 out_dim: int, \n",
                 "                 activation: Union[Callable, str] = \"relu\", \n",
                 "                 dropout: float = 0.0, \n",
                 "                 normalization: Union[str, Callable] = \"none\",\n",
-                "                 aggr: str = \"sum\",\n",
+                "                 aggr: str = \"mean\",\n",
                 "                ):\n",
                 "        r\"\"\"\n",
                 "        add documentation in the format shown here for this layer to be automatically added to the graphium api reference\n",
                 "        the type information will also be automatically shown in the doc\n",
                 "        \n",
                 "        Parameters:\n",
                 "\n",
@@ -174,18 +181,18 @@
                 "                Normalization to use. Choices:\n",
                 "\n",
                 "                - \"none\" or `None`: No normalization\n",
                 "                - \"batch_norm\": Batch normalization\n",
                 "                - \"layer_norm\": Layer normalization\n",
                 "                - `Callable`: Any callable function\n",
                 "            aggr:\n",
-                "                what aggregation to use\n",
+                "                what aggregation to use (\"add\", \"mean\" or \"max\")\n",
                 "        \"\"\"\n",
                 "        # Initialize the parent class\n",
-                "        MessagePassing.__init__(self, node_dim=0)\n",
+                "        MessagePassing.__init__(self, node_dim=0, aggr=aggr)\n",
                 "        BaseGraphStructure.__init__(self,\n",
                 "                                    in_dim=in_dim, \n",
                 "                                    out_dim=out_dim, \n",
                 "                                    activation=activation,\n",
                 "                                    dropout=dropout, \n",
                 "                                    normalization=normalization)\n",
                 "        \n",
@@ -203,33 +210,31 @@
                 "        similarly add documentation to the functions in the class\n",
                 "        \n",
                 "        Parameters:\n",
                 "            batch: pyg Batch graphs to pass through the layer\n",
                 "        Returns:\n",
                 "            batch: pyg Batch graphs\n",
                 "        \"\"\"\n",
-                "        # We first apply the mean aggregation\n",
                 "        \n",
                 "        x = batch.feat\n",
                 "        edge_index = batch.edge_index\n",
                 "        \n",
                 "        if isinstance(x, Tensor):\n",
                 "            x: OptPairTensor = (x, x)\n",
                 "\n",
                 "        # propagate_type: (x: OptPairTensor, edge_weight: OptTensor)\n",
-                "        h = self.propagate(edge_index, x=x)\n",
-                "        out = self.transform(h)\n",
-                "        out = self.apply_norm_activation_dropout(out,batch_idx=batch.batch)\n",
+                "        out = self.propagate(edge_index, x=x)\n",
+                "        out = self.transform(out)\n",
+                "        out = self.apply_norm_activation_dropout(out, batch_idx=batch.batch)\n",
                 "        batch.feat = out\n",
                 "        return batch\n",
                 "    \n",
-                "    def message_and_aggregate(self, \n",
-                "                              adj_t: SparseTensor,\n",
-                "                              x: OptPairTensor) -> Tensor:\n",
-                "        return spmm(adj_t, x[0], reduce=self.aggr)\n",
+                "    def message(self, x_j):\n",
+                "\n",
+                "        return x_j\n",
                 "\n",
                 "    # Finally, we define all the virtual properties according to how the class works with proper documentation of course\n",
                 "    @classproperty\n",
                 "    def layer_supports_edges(cls) -> bool:\n",
                 "        r\"\"\"\n",
                 "        Return a boolean specifying if the layer type supports edges or not.\n",
                 "\n",
@@ -272,25 +277,26 @@
                 "            int:\n",
                 "                Always ``1`` for the current class\n",
                 "        \"\"\"\n",
                 "        return 1"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Test our simple layer\n",
                 "\n",
                 "Now, we are ready to test the `SimpleMeanLayer` on our constructed graphs. Note that in this example, we **ignore** the edge features since they are not supported."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 84,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "torch.Size([7, 5])\n",
@@ -303,22 +309,22 @@
                 "print(graph.feat.shape)\n",
                 "\n",
                 "layer = SimpleMeanLayer(\n",
                 "            in_dim=in_dim, \n",
                 "            out_dim=out_dim, \n",
                 "            activation=\"relu\", \n",
                 "            dropout=.3, \n",
-                "            normalization=\"batch_norm\",\n",
-                "            aggr=\"sum\")\n",
+                "            normalization=\"batch_norm\")\n",
                 "\n",
                 "graph = layer(graph)\n",
                 "print(graph.feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating a complex layer with edges\n",
                 "\n",
                 "Here, we will show how to create a GNN layer that does a mean aggregation on the neighbouring features, concatenated to the edge features with their neighbours. In that case, only the node features will change, and the network will not update the edge features.\n",
                 "\n",
@@ -330,31 +336,31 @@
                 "- [`out_dim_factor`](https://graphium-docs.datamol.io/stable/api/graphium.nn/graphium.nn.html#graphium.nn.base_graph_layer.BaseGraphStructure.out_dim_factor): We want to return `1` since the output dimension does not depend on internal parameters.\n",
                 "\n",
                 "The example is given below"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 85,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#inherent from message passing class from pyg \n",
-                "#inherent from BaseGraphStructure\n",
+                "# inherent from message passing class from pyg \n",
+                "# inherent from BaseGraphStructure\n",
                 "# adapting example from graphium/nn/pyg_layers/png_pyg.py\n",
                 "\n",
                 "class ComplexMeanLayer(MessagePassing, BaseGraphStructure):\n",
                 "    def __init__(self, \n",
                 "                 in_dim: int, \n",
                 "                 out_dim: int, \n",
                 "                 in_dim_edges: int, \n",
                 "                 activation: Union[Callable, str] = \"relu\", \n",
                 "                 dropout: float = 0.0, \n",
                 "                 normalization: Union[str, Callable] = \"none\",\n",
-                "                 aggr: str = \"sum\",\n",
+                "                 aggr: str = \"mean\",\n",
                 "                ):\n",
                 "        r\"\"\"\n",
                 "        add documentation in the format shown here for this layer to be automatically added to the graphium api reference\n",
                 "        the type information will also be automatically shown in the doc\n",
                 "        \n",
                 "        Parameters:\n",
                 "\n",
@@ -377,30 +383,30 @@
                 "                Normalization to use. Choices:\n",
                 "\n",
                 "                - \"none\" or `None`: No normalization\n",
                 "                - \"batch_norm\": Batch normalization\n",
                 "                - \"layer_norm\": Layer normalization\n",
                 "                - `Callable`: Any callable function\n",
                 "            aggr:\n",
-                "                what aggregation to use\n",
+                "                what aggregation to use (\"add\", \"mean\" or \"max\")\n",
                 "        \"\"\"\n",
                 "        # Initialize the parent class\n",
-                "        MessagePassing.__init__(self, node_dim=0)\n",
+                "        MessagePassing.__init__(self, node_dim=0, aggr=aggr)\n",
                 "        BaseGraphStructure.__init__(self,\n",
                 "                                    in_dim=in_dim, \n",
                 "                                    out_dim=out_dim, \n",
                 "                                    activation=activation,\n",
                 "                                    dropout=dropout, \n",
                 "                                    normalization=normalization)\n",
                 "        \n",
                 "        self.aggr = aggr\n",
                 "        self._initialize_activation_dropout_norm()\n",
                 "        # Create the mlp layer \n",
                 "        # https://graphium-docs.datamol.io/stable/api/graphium.nn/graphium.nn.html#graphium.nn.base_layers.MLP\n",
-                "        self.transform = FCLayer(in_dim=(in_dim * 2 +in_dim_edges), out_dim=out_dim)\n",
+                "        self.transform = FCLayer(in_dim=(in_dim + in_dim_edges), out_dim=out_dim)\n",
                 "            \n",
                 "    # define the forward function \n",
                 "    def forward(self, \n",
                 "                batch: Union[Data, Batch],\n",
                 "               ) -> Union[Data, Batch]:\n",
                 "        r\"\"\"\n",
                 "        similarly add documentation to the functions in the class\n",
@@ -414,32 +420,32 @@
                 "        edge_index = batch.edge_index\n",
                 "        edge_feat = batch.edge_feat\n",
                 "        \n",
                 "        if isinstance(x, Tensor):\n",
                 "            x: OptPairTensor = (x, x)\n",
                 "\n",
                 "        # propagate_type: (x: OptPairTensor, edge_weight: OptTensor)\n",
-                "        h = self.propagate(edge_index, x=x, edge_feat=edge_feat, size=None)\n",
-                "        out = self.transform(h)\n",
-                "        out = self.apply_norm_activation_dropout(out,batch_idx=batch.batch)\n",
+                "        out = self.propagate(edge_index, x=x, edge_feat=edge_feat, size=None)\n",
+                "        out = self.transform(out)\n",
+                "        out = self.apply_norm_activation_dropout(out, batch_idx=batch.batch)\n",
                 "        batch.feat = out\n",
                 "        return batch\n",
                 "    \n",
-                "    def message(self, x_i: Tensor, x_j: Tensor, edge_feat: OptTensor) -> Tensor:\n",
+                "    def message(self, x_j: Tensor, edge_feat: OptTensor) -> Tensor:\n",
                 "        r\"\"\"\n",
                 "        message function\n",
                 "\n",
                 "        Parameters:\n",
                 "            x_i: node features\n",
                 "            x_j: neighbour node features\n",
                 "            edge_feat: edge features\n",
                 "        Returns:\n",
                 "            feat: the message\n",
                 "        \"\"\"\n",
-                "        feat = torch.cat([x_i, x_j, edge_feat], dim=-1)\n",
+                "        feat = torch.cat([x_j, edge_feat], dim=-1)\n",
                 "        return feat\n",
                 "    \n",
                 "    def aggregate(\n",
                 "        self,\n",
                 "        inputs: Tensor,\n",
                 "        index: Tensor,\n",
                 "        edge_index: Tensor,\n",
@@ -504,52 +510,61 @@
                 "            int:\n",
                 "                Always ``1`` for the current class\n",
                 "        \"\"\"\n",
                 "        return 1"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Test our complex layer \n",
                 "\n",
                 "Now, we are ready to test the `ComplexMeanLayer` on our constructed graphs. Note that in this example, we utilize the edge features and node features"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 86,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "torch.Size([7, 5])\n",
+                        "torch.Size([7, 13])\n",
                         "torch.Size([7, 11])\n"
                     ]
                 }
             ],
             "source": [
                 "graph = deepcopy(bg)\n",
                 "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)\n",
                 "\n",
                 "layer = ComplexMeanLayer(\n",
                 "            in_dim=in_dim, \n",
                 "            out_dim=out_dim, \n",
                 "            in_dim_edges=in_dim_edges,\n",
                 "            activation=\"relu\", \n",
                 "            dropout=.3, \n",
-                "            normalization=\"batch_norm\",\n",
-                "            aggr=\"sum\")\n",
+                "            normalization=\"batch_norm\")\n",
                 "\n",
                 "graph = layer(graph)\n",
                 "print(graph.feat.shape)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "interpreter": {
             "hash": "f4a99d018a205fcbcc0480c84566beaebcb91b08d0414b39a842df533e2a1d25"
         },
         "kernelspec": {
@@ -563,13 +578,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `graphium-2.0.2/docs/tutorials/gnn/using_gnn_layers.ipynb` & `graphium-2.1.0/docs/tutorials/gnn/using_gnn_layers.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9644013440603514%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'The current library implements multiple "*

 * *            'state-of-the-art graph neural networks. In this tutorial, you will learn how to use '*

 * *            'the **GCN**, **GIN**, **GINE**, **GPS**, **Gated-GCN** and **PNA** layers in a simple '*

 * *            "`forward` context.')], delete: [4, 2, 1]}, 'attachments': OrderedDict()}, 1: "*

 * *            "{'execution_count': 53, 'outputs': {0: {'name': 'stdout', 'text': ['The autoreload "*

 * *            "extension is already loa […]*

```diff
@@ -1,351 +1,395 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Using GNN layers\n",
                 "\n",
-                "The current library implements multiple state-of-the-art graph neural networks. In this tutorial, you will learn how to use the **GCN**, **GIN**, **Gated-GCN** and **PNA** layers in a simple `forward` context.\n",
-                "\n",
-                "Other layers such as **DGN** require additional positional encoding to work."
+                "The current library implements multiple state-of-the-art graph neural networks. In this tutorial, you will learn how to use the **GCN**, **GIN**, **GINE**, **GPS**, **Gated-GCN** and **PNA** layers in a simple `forward` context."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 53,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Using backend: pytorch\n"
+                        "The autoreload extension is already loaded. To reload it, use:\n",
+                        "  %reload_ext autoreload\n"
                     ]
                 }
             ],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "\n",
                 "import torch\n",
-                "import dgl\n",
+                "\n",
+                "import torch_geometric as pyg\n",
+                "from torch_geometric.data import Data, Batch\n",
+                "\n",
                 "from copy import deepcopy\n",
                 "\n",
-                "from graphium.nn.dgl_layers import (\n",
-                "    GCNLayer,\n",
-                "    GINLayer,\n",
-                "    GATLayer,\n",
-                "    GatedGCNLayer,\n",
-                "    PNAConvolutionalLayer,\n",
-                "    PNAMessagePassingLayer,\n",
+                "from graphium.nn.pyg_layers import (\n",
+                "    GCNConvPyg,\n",
+                "    GINConvPyg,\n",
+                "    GatedGCNPyg,\n",
+                "    GINEConvPyg,\n",
+                "    GPSLayerPyg,\n",
+                "    PNAMessagePassingPyg\n",
                 ")\n",
                 "\n",
                 "_ = torch.manual_seed(42)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We will first create some simple batched graphs that will be used accross the examples. Here, `bg` is a batch of 2 graphs containing random node features `bg.ndata[\"h\"]` and edge features `bg.edata[\"e\"]`."
+                "We will first create some simple batched graphs that will be used accross the examples. Here, `bg` is a batch containing 2 graphs with random node features."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 54,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Graph(num_nodes=7, num_edges=14,\n      ndata_schemes={'h': Scheme(shape=(5,), dtype=torch.float64)}\n      edata_schemes={'e': Scheme(shape=(13,), dtype=torch.float64)})\n"
+                        "DataBatch(edge_index=[2, 7], feat=[7, 5], edge_feat=[7, 13], batch=[7], ptr=[3])\n"
                     ]
                 }
             ],
             "source": [
                 "in_dim = 5          # Input node-feature dimensions\n",
-                "out_dim = 11        # Desired output node-feature dimensions\n",
                 "in_dim_edges = 13   # Input edge-feature dimensions\n",
+                "out_dim = 11        # Desired output node-feature dimensions\n",
+                "out_dim_edges = 15  # Desired output edge-feature dimensions\n",
+                "\n",
+                "\n",
+                "# Let's create 2 simple pyg graphs. \n",
+                "# start by specifying the edges with edge index\n",
+                "edge_idx1 = torch.tensor([[0, 1, 2],\n",
+                "                          [1, 2, 3]])\n",
+                "edge_idx2 = torch.tensor([[2, 0, 0, 1],\n",
+                "                          [0, 1, 2, 0]])\n",
+                "\n",
+                "# specify the node features, convention with variable x\n",
+                "x1 = torch.randn(edge_idx1.max() + 1, in_dim, dtype=torch.float32)\n",
+                "x2 = torch.randn(edge_idx2.max() + 1, in_dim, dtype=torch.float32)\n",
+                "\n",
+                "# specify the edge features in e\n",
+                "e1 = torch.randn(edge_idx1.shape[-1], in_dim_edges, dtype=torch.float32)\n",
+                "e2 = torch.randn(edge_idx2.shape[-1], in_dim_edges, dtype=torch.float32)\n",
+                "\n",
+                "# make the pyg graph objects with our constructed features\n",
+                "g1 = Data(feat=x1, edge_index=edge_idx1, edge_feat=e1)\n",
+                "g2 = Data(feat=x2, edge_index=edge_idx2, edge_feat=e2)\n",
                 "\n",
-                "# Let's create 2 simple graphs. Here the tensors represent the connectivity between nodes\n",
-                "g1 = dgl.graph((torch.tensor([0, 1, 2]), torch.tensor([1, 2, 3])))\n",
-                "g2 = dgl.graph((torch.tensor([0, 0, 0, 1]), torch.tensor([0, 1, 2, 0])))\n",
-                "\n",
-                "# We add some node features to the graphs\n",
-                "g1.ndata[\"h\"] = torch.rand(g1.num_nodes(), in_dim, dtype=float)\n",
-                "g2.ndata[\"h\"] = torch.rand(g2.num_nodes(), in_dim, dtype=float)\n",
-                "\n",
-                "# We also add some edge features to the graphs\n",
-                "g1.edata[\"e\"] = torch.rand(g1.num_edges(), in_dim_edges, dtype=float)\n",
-                "g2.edata[\"e\"] = torch.rand(g2.num_edges(), in_dim_edges, dtype=float)\n",
-                "\n",
-                "# Finally we batch the graphs in a way compatible with the DGL library\n",
-                "bg = dgl.batch([g1, g2])\n",
-                "bg = dgl.add_self_loop(bg)\n",
+                "# put the two graphs into a Batch graph\n",
+                "bg = Batch.from_data_list([g1, g2])\n",
                 "\n",
                 "# The batched graph will show as a single graph with 7 nodes\n",
-                "print(bg)\n"
+                "print(bg)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## GCN Layer\n",
                 "\n",
                 "To use the GCN layer from the *Kipf et al.* paper, the steps are very simple. We create the layer with the desired attributes, and apply it to the graph.\n",
                 "\n",
                 "<sub>Kipf, Thomas N., and Max Welling. \"Semi-supervised classification with graph convolutional networks.\" arXiv preprint arXiv:1609.02907 (2016).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 55,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GCNLayer(5 -> 11, activation=relu)\ntorch.Size([7, 5])\ntorch.Size([7, 11])\n"
+                        "torch.Size([7, 5])\n",
+                        "GCNConvPyg(5 -> 11, activation=relu)\n",
+                        "torch.Size([7, 11])\n"
                     ]
                 }
             ],
             "source": [
-                "# We first need to extract the node features from the graph.\n",
                 "# The GCN method doesn't support edge features, so we ignore them\n",
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
+                "print(graph.feat.shape)\n",
                 "\n",
                 "# We create the layer\n",
-                "layer = GCNLayer(\n",
+                "layer = GCNConvPyg(\n",
                 "            in_dim=in_dim, out_dim=out_dim, \n",
-                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
+                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
                 "\n",
                 "# We apply the forward loop on the node features\n",
-                "h_out = layer(graph, h_in)\n",
+                "graph = layer(graph)\n",
                 "\n",
                 "# 7 is the number of nodes, 5 number of input features and 11 number of output features\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)"
+                "print(graph.feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## GIN Layer\n",
                 "\n",
                 "To use the GIN layer from the *Xu et al.* paper, the steps are identical to GCN.\n",
                 "\n",
                 "<sub>Xu, Keyulu, et al. \"How powerful are graph neural networks?.\" arXiv preprint arXiv:1810.00826 (2018).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 56,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GINLayer(5 -> 11, activation=relu)\ntorch.Size([7, 5])\ntorch.Size([7, 11])\n"
+                        "torch.Size([7, 5])\n",
+                        "GINConvPyg(5 -> 11, activation=relu)\n",
+                        "torch.Size([7, 11])\n"
                     ]
                 }
             ],
             "source": [
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
-                "layer = GINLayer(\n",
+                "print(graph.feat.shape)\n",
+                "\n",
+                "# We create the layer\n",
+                "layer = GINConvPyg(\n",
                 "            in_dim=in_dim, out_dim=out_dim, \n",
-                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
-                "h_out = layer(graph, h_in)\n",
+                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
+                "\n",
+                "# We apply the forward loop on the node features\n",
+                "graph = layer(graph)\n",
                 "\n",
+                "# 7 is the number of nodes, 5 number of input features and 11 number of output features\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)"
+                "print(graph.feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## GAT Layer\n",
+                "## GINE Layer\n",
                 "\n",
-                "To use the GAT layer from the *Velickovic et al.* paper, the steps are identical to GCN, but the output dimension is multiplied by the number of heads.\n",
+                "To use the GINE layer from the *Hu et al.* paper, we also need to provide additional edge features as inputs.\n",
                 "\n",
-                "<sub>Velickovic, Petar, et al. \"Graph attention networks.\" arXiv preprint arXiv:1710.10903 (2017).</sub>"
+                "<sub>Hu, Weihua, et al. \"Strategies for Pre-training Graph Neural Networks.\" arXiv preprint arXiv:1905.12265 (2019).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 57,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GATLayer(5 -> 11 * 5, activation=elu)\ntorch.Size([7, 5])\ntorch.Size([7, 55])\n"
+                        "torch.Size([7, 5])\n",
+                        "torch.Size([7, 13])\n",
+                        "GINEConvPyg(5 -> 11, activation=relu)\n",
+                        "torch.Size([7, 11])\n"
                     ]
                 }
             ],
             "source": [
+                "# The GINE method uses edge features, so we have to pass the input dimension\n",
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
-                "layer = GATLayer(\n",
-                "            in_dim=in_dim, out_dim=out_dim, num_heads=5,\n",
-                "            activation=\"elu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
-                "h_out = layer(graph, h_in)\n",
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)\n",
+                "\n",
+                "# We create the layer\n",
+                "layer = GINEConvPyg(\n",
+                "            in_dim=in_dim, out_dim=out_dim,\n",
+                "            in_dim_edges=in_dim_edges,\n",
+                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
                 "\n",
+                "# We apply the forward loop on the node features\n",
+                "graph = layer(graph)\n",
+                "\n",
+                "# 7 is the number of nodes, 5 number of input features and 11 number of output features\n",
+                "# 7 is the number of edges, 13 number of input edge features\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)"
+                "print(graph.feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Gated-GCN Layer\n",
+                "## GPS Layer\n",
                 "\n",
-                "To use the Gated-GCN layer from the *Bresson et al.* paper, the steps are different since the layer requires edge features as inputs, and outputs new edge features.\n",
+                "To use the GPS layer from the *Ramp\u00e1\u0161ek et al.* paper, we also need to provide additional edge features as inputs. It is a hybrid approach using both a GNN and transformer in conjunction. Therefore, we further need to specify the GNN type and attention type used in the layer.\n",
                 "\n",
-                "<sub>Bresson, Xavier, and Thomas Laurent. \"Residual gated graph convnets.\" arXiv preprint arXiv:1711.07553 (2017).</sub>"
+                "<sub>Ramp\u00e1\u0161ek, Ladislav, et al. \"Recipe for a General, Powerful, Scalable Graph Transformer.\" arXiv preprint arXiv:2205.12454 (2022).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 58,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "GatedGCNLayer(5 -> 11, activation=relu)\ntorch.Size([7, 5])\ntorch.Size([7, 11])\ntorch.Size([14, 13])\ntorch.Size([14, 11])\n"
+                        "torch.Size([7, 5])\n",
+                        "torch.Size([7, 13])\n",
+                        "GPSLayerPyg(5 -> 11, activation=relu)\n",
+                        "torch.Size([7, 11])\n",
+                        "torch.Size([7, 13])\n"
                     ]
                 }
             ],
             "source": [
-                "# We first need to extract the node and edge features from the graph.\n",
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
-                "e_in = graph.edata[\"e\"]\n",
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)\n",
                 "\n",
                 "# We create the layer\n",
-                "layer = GatedGCNLayer(\n",
-                "        in_dim=in_dim, out_dim=out_dim, \n",
-                "        in_dim_edges=in_dim_edges, out_dim_edges=out_dim,\n",
-                "        activation=\"relu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
+                "layer = GPSLayerPyg(\n",
+                "            in_dim=in_dim, out_dim=out_dim,\n",
+                "            in_dim_edges=in_dim_edges,\n",
+                "            mpnn_type = \"pyg:gine\", attn_type = \"full-attention\",\n",
+                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
                 "\n",
                 "# We apply the forward loop on the node features\n",
-                "h_out, e_out = layer(graph, h_in, e_in)\n",
+                "graph = layer(graph)\n",
                 "\n",
                 "# 7 is the number of nodes, 5 number of input features and 11 number of output features\n",
-                "# 13 is the number of input edge features\n",
+                "# 7 is the number of edges, 13 number of input edge features\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)\n",
-                "print(e_in.shape)\n",
-                "print(e_out.shape)"
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# PNA\n",
-                "\n",
-                "PNA is a multi-aggregator method proposed by *Corso et al.*. It supports 2 types of aggregations, convolutional *PNA-conv* or message passing *PNA-msgpass*.\n",
-                "\n",
-                "<sub>PNA: Principal Neighbourhood Aggregation \n",
-                "Gabriele Corso, Luca Cavalleri, Dominique Beaini, Pietro Lio, Petar Velickovic\n",
-                "https://arxiv.org/abs/2004.05718</sub>\n",
+                "## Gated-GCN Layer\n",
                 "\n",
-                "## PNA-conv\n",
+                "To use the Gated-GCN layer from the *Bresson et al.* paper, the steps are different since the layer not only requires edge features as inputs, but also outputs new edge features. Therefore, we have to further specify the number of output edge features\n",
                 "\n",
-                "First, let's focus on the PNA-conv. In this case, it works exactly as the GCN and GIN methods. Although not presented in the example, PNA-conv also supports edge features by concatenating them to the node features during convolution."
+                "<sub>Bresson, Xavier, and Thomas Laurent. \"Residual gated graph convnets.\" arXiv preprint arXiv:1711.07553 (2017).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 59,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "PNAConvolutionalLayer(5 -> 11, activation=relu)\ntorch.Size([7, 5])\ntorch.Size([7, 11])\n"
+                        "torch.Size([7, 5])\n",
+                        "torch.Size([7, 13])\n",
+                        "GatedGCNPyg()\n",
+                        "torch.Size([7, 11])\n",
+                        "torch.Size([7, 15])\n"
                     ]
                 }
             ],
             "source": [
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)\n",
                 "\n",
-                "# We create the layer, and need to specify the aggregators and scalers\n",
-                "layer = PNAConvolutionalLayer(\n",
-                "    in_dim=in_dim, out_dim=out_dim, \n",
-                "    aggregators=[\"mean\", \"max\", \"min\", \"std\"],\n",
-                "    scalers=[\"identity\", \"amplification\", \"attenuation\"],\n",
-                "    activation=\"relu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
+                "# We create the layer\n",
+                "layer = GatedGCNPyg(\n",
+                "            in_dim=in_dim, out_dim=out_dim,\n",
+                "            in_dim_edges=in_dim_edges, out_dim_edges=out_dim_edges,\n",
+                "            activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
                 "\n",
-                "h_out = layer(graph, h_in)\n",
+                "# We apply the forward loop on the node features\n",
+                "graph = layer(graph)\n",
                 "\n",
+                "# 7 is the number of nodes, 5 number of input features and 11 number of output features\n",
+                "# 7 is the number of edges, 13 number of input edge features and 15 the the number of output edge features\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)"
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## PNA-msgpass\n",
+                "## PNA\n",
+                "\n",
+                "PNA is a multi-aggregator method proposed by *Corso et al.*. It supports 2 types of aggregations, convolutional *PNA-conv* or message passing *PNA-msgpass*. Here, we provide the typically more powerful *PNA-msgpass*. It supports edges as inputs, but doesn't output edges. Here, we need to further specify the aggregators and scalers specific to this layer.\n",
                 "\n",
-                "The PNA message passing is typically more powerful that the convolutional one, and it supports edges as inputs, but doesn't output edges. It's usage is very similar to the *PNA-conv*. Here, we also present the option to specify the edge dimensions and features."
+                "<sub>Corso, Gabriele, et al. \"Principal Neighbourhood Aggregation for Graph Nets.\"\n",
+                "arXiv preprint arXiv:2004.05718 (2020).</sub>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 60,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "PNAMessagePassingLayer(5 -> 11, activation=relu)\ntorch.Size([7, 5])\ntorch.Size([7, 11])\n"
+                        "torch.Size([7, 5])\n",
+                        "torch.Size([7, 13])\n",
+                        "PNAMessagePassingPyg()\n",
+                        "torch.Size([7, 11])\n"
                     ]
                 }
             ],
             "source": [
                 "graph = deepcopy(bg)\n",
-                "h_in = graph.ndata[\"h\"]\n",
-                "e_in = graph.edata[\"e\"]\n",
+                "print(graph.feat.shape)\n",
+                "print(graph.edge_feat.shape)\n",
                 "\n",
                 "# We create the layer, and need to specify the aggregators and scalers\n",
-                "layer = PNAMessagePassingLayer(\n",
-                "    in_dim=in_dim, out_dim=out_dim, in_dim_edges=in_dim_edges,\n",
+                "layer = PNAMessagePassingPyg(\n",
+                "    in_dim=in_dim, out_dim=out_dim,\n",
+                "    in_dim_edges=in_dim_edges,\n",
                 "    aggregators=[\"mean\", \"max\", \"min\", \"std\"],\n",
                 "    scalers=[\"identity\", \"amplification\", \"attenuation\"],\n",
-                "    activation=\"relu\", dropout=.3, normalization=\"batch_norm\").to(float)\n",
+                "    activation=\"relu\", dropout=.3, normalization=\"batch_norm\")\n",
                 "\n",
-                "h_out = layer(graph, h_in, e_in)\n",
+                "graph = layer(graph)\n",
                 "\n",
                 "print(layer)\n",
-                "print(h_in.shape)\n",
-                "print(h_out.shape)"
+                "print(graph.feat.shape)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -353,27 +397,27 @@
         }
     ],
     "metadata": {
         "interpreter": {
             "hash": "f4a99d018a205fcbcc0480c84566beaebcb91b08d0414b39a842df533e2a1d25"
         },
         "kernelspec": {
-            "display_name": "Python 3.8.8 64-bit ('graphium': conda)",
+            "display_name": "Python 3.8.8 64-bit ('goli': conda)",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.8"
+            "version": "3.10.12"
         },
         "orig_nbformat": 2
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `graphium-2.0.2/docs/tutorials/model_training/config_ipu_tutorials.yaml` & `graphium-2.1.0/tests/config_test_ipu_dataloader.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,131 @@
 # Testing the multitask pipeline with the QM9 dataset on IPU, by splitting it up into three tasks: homo, alpha and cv.
 constants:
-  name: &name tutorial_model
+  name: &name test_ipu #qm9_full
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
-  accelerator:
-    type: ipu  #cpu or ipu or gpu
 
+accelerator:
+  type: ipu  # cpu or ipu or gpu
+  config_override:
+    datamodule:
+      args:
+        ipu_dataloader_training_opts:
+          mode: async
+          max_num_nodes_per_graph: 20 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 60
+        ipu_dataloader_inference_opts:
+          mode: async
+          max_num_nodes_per_graph: 16 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 120
+        # Data handling-related
+        batch_size_training: 6
+        batch_size_inference: 6
+    trainer:
+      trainer:
+        precision: 16
+        accumulate_grad_batches: 4
+
+  ipu_config:
+    - deviceIterations(2)
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
       homo:
         df: null
-        df_path: &df_path https://storage.googleapis.com/graphium-public/datasets/QM9/norm_micro_qm9.csv
-        smiles_col: "smiles"
-        label_cols: ["homo", "lumo"]
+        df_path: &df_path https://storage.googleapis.com/datasets-public-research/PCQM4M/cxsmiles/pcqm4mv2-2k-lumo-alpha.csv
+        smiles_col: "cxsmiles"
+        label_cols: ["homo_lumo_gap", "lumo"]
         split_val: 0.2
         split_test: 0.2
-        split_seed: *seed
+        seed: *seed
         splits_path: null                 # This may not always be provided
         sample_size: null                 # This may not always be provided
         idx_col: null                     # This may not always be provided
         weights_col: null                 # This may not always be provided
         weights_type: null                # This may not always be provided
+        task_level: graph
       alpha:
         df: null
         df_path: *df_path
-        smiles_col: "smiles"
+        smiles_col: "cxsmiles"
         label_cols: ["alpha"]
         split_val: 0.2
         split_test: 0.2
-        split_seed: *seed
+        seed: *seed
         splits_path: null                 # This may not always be provided
         sample_size: null                 # This may not always be provided
         idx_col: null                     # This may not always be provided
         weights_col: null                 # This may not always be provided
         weights_type: null                # This may not always be provided
-      cv:
-        df: null
-        df_path: *df_path
-        smiles_col: "smiles"
-        label_cols: ["cv"]
-        split_val: 0.2
-        split_test: 0.2
-        split_seed: *seed
-        splits_path: null                 # This may not always be provided
-        sample_size: null                 # This may not always be provided
-        idx_col: null                     # This may not always be provided
-        weights_col: null                 # This may not always be provided
-        weights_type: null                # This may not always be provided
-
+        task_level: graph
     # Featurization
     prepare_dict_or_graph: pyg:graph
-    featurization_n_jobs: -1
+    featurization_n_jobs: 0
     featurization_progress: True
     featurization:
       atom_property_list_onehot: [atomic-number, valence]
       atom_property_list_float: [mass, electronegativity, in-ring]
       edge_property_list: [bond-type-onehot, stereo, in-ring]
+      conformer_property_list: [positions_3d]
       add_self_loop: False
       explicit_H: False
       use_bonds_weights: False
-      pos_encoding_as_features:
+      pos_encoding_as_features: # encoder dropout 0.18
         pos_types:
-          la_pos: &pos_enc  #use same name as pe_encoder
-            pos_type: laplacian_eigvec_eigval #laplacian_eigvec
-            num_pos: 3
+          node_laplacian_eigvec:
+            pos_type: laplacian_eigvec
+            pos_level: node
+            num_pos: 5
             normalization: "none"
             disconnected_comp: True
-          rw_pos: #use same name as pe_encoder
-            pos_type: rwse
-            ksteps: 16
-      # pos_encoding_as_directions: *pos_enc # Only for DGN or directional pooling
-
-    # Data handling-related
-    batch_size_training: 6
-    batch_size_inference: 6
-    # cache_data_path: null
+          node_laplacian_eigval:
+            pos_type: laplacian_eigval
+            pos_level: node
+            num_pos: 5
+            normalization: "none"
+            disconnected_comp: True
+          rw_return_probs:
+            pos_type: rw_return_probs
+            pos_level: node
+            ksteps: [4, 8]
+          edge_rw_transition_probs:
+            pos_type: rw_transition_probs
+            pos_level: edge
+            ksteps: [2, 4]
+          nodepair_rw_return_probs:
+            pos_type: rw_return_probs
+            pos_level: nodepair
+            ksteps: [4]
+          electrostatic:
+            pos_type: electrostatic
+            pos_level: node
+          edge_commute:
+            pos_type: commute
+            pos_level: edge
+          nodepair_graphormer:
+            pos_type: graphormer
+            pos_level: nodepair
 
     num_workers: -1
 
-    ipu_dataloader_training_opts:
-      max_num_nodes_per_graph: 12
-      max_num_edges_per_graph: 24
-
-    ipu_dataloader_inference_opts:
-      max_num_nodes_per_graph: 12
-      max_num_edges_per_graph: 24
-
 architecture:
   model_type: FullGraphMultiTaskNetwork
+  mup_base_path: null
+
   pre_nn:   # Set as null to avoid a pre-nn network
-    out_dim: 32
-    hidden_dims: 32
+    out_dim: 16
+    hidden_dims: 16
     depth: 1
     activation: relu
     last_activation: none
     dropout: &dropout 0.1
-    normalization: &normalization "none"
+    normalization: &normalization batch_norm
     last_normalization: *normalization
     residual_type: none
 
   pre_nn_edges:   # Set as null to avoid a pre-nn network
     out_dim: 16
     hidden_dims: 16
     depth: 1
@@ -110,191 +133,170 @@
     last_activation: none
     dropout: *dropout
     normalization: *normalization
     last_normalization: *normalization
     residual_type: none
 
   pe_encoders:
-    out_dim: 32
+    out_dim: &pe_out_dim 16
+    edge_out_dim: &edge_pe_out_dim 8
     pool: "sum" #"mean" "max"
     last_norm: None #"batch_norm", "layer_norm"
-    encoders: #la_pos |  rw_pos
-      la_pos:  # Set as null to avoid a pre-nn network
+    max_num_nodes_per_graph: 30
+    encoders:
+      emb_la_pos:
         encoder_type: "laplacian_pe"
         input_keys: ["laplacian_eigvec", "laplacian_eigval"]
+        output_keys: ["feat"]
         hidden_dim: 32
         model_type: 'DeepSet' #'Transformer' or 'DeepSet'
-        num_layers: 1
-        num_layers_post: 0 # Num. layers to apply after pooling
+        num_layers: 2
+        num_layers_post: 1 # Num. layers to apply after pooling
         dropout: 0.1
         first_normalization: "none" #"batch_norm" or "layer_norm"
-      rw_pos:
+      emb_rwse:
         encoder_type: "mlp"
         input_keys: ["rw_return_probs"]
-        output_keys: "node"
+        output_keys: ["feat"]
+        hidden_dim: 32
+        num_layers: 2
+        dropout: 0.1
+        normalization: "layer_norm" #"batch_norm" or "layer_norm"
+        first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
+      emb_electrostatic:
+        encoder_type: "mlp"
+        input_keys: ["electrostatic"]
+        output_keys: ["feat"]
         hidden_dim: 32
         num_layers: 1
         dropout: 0.1
-        normalization: "none" #"batch_norm" or "layer_norm"
-        first_normalization: "none" #"batch_norm" or "layer_norm"
-
+        normalization: "layer_norm" #"batch_norm" or "layer_norm"
+        first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
+      emb_edge_rwse:
+        encoder_type: "mlp"
+        input_keys: ["edge_rw_transition_probs"]
+        output_keys: ["edge_feat"]
+        hidden_dim: 32
+        num_layers: 1
+        dropout: 0.1
+        normalization: "layer_norm" #"batch_norm" or "layer_norm"
+      emb_edge_pes:
+        encoder_type: "cat_mlp"
+        input_keys: ["edge_rw_transition_probs", "edge_commute"]
+        output_keys: ["edge_feat"]
+        hidden_dim: 32
+        num_layers: 1
+        dropout: 0.1
+        normalization: "layer_norm" #"batch_norm" or "layer_norm"
+      gaussian_pos:
+        encoder_type: "gaussian_kernel"
+        input_keys: ["positions_3d"]
+        output_keys: ["feat", "nodepair_gaussian_bias_3d"]
+        num_heads: &num_heads 2
+        num_layers: 2
+        embed_dim: *pe_out_dim
+        use_input_keys_prefix: False
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: 32
-    hidden_dims: 32
-    depth: 3
+    out_dim: 8
+    hidden_dims: 16
+    depth: 2
     activation: relu
     last_activation: none
     dropout: *dropout
     normalization: *normalization
     last_normalization: *normalization
     residual_type: simple
-    pooling: [sum, mean, max]
     virtual_node: 'none'
     layer_type: 'pyg:gps' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
     layer_kwargs:  # Parameters for the model itself. You could define dropout_attn: 0.1
       mpnn_type: 'pyg:gine'
       mpnn_kwargs: null
         #out_dim_edges: 10
-      attn_type: "full-attention" #"none"
+      attn_type: "none" # "full-attention", "none"
       attn_kwargs: null
 
-
-      # out_dim_edges: 16
-      # aggregators: [mean, max]
-      # scalers: [identity, amplification, attenuation]
-      # num_heads: 3
-
   graph_output_nn:
-    out_dim: 32
-    hidden_dims: 32
-    depth: 1
-    activation: relu
-    last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: "none"
-    residual_type: none
+    graph:
+      pooling: [sum, mean, max]
+      out_dim: 8
+      hidden_dims: 8
+      depth: 1
+      activation: relu
+      last_activation: none
+      dropout: *dropout
+      normalization: *normalization
+      last_normalization: "none"
+      residual_type: none
 
   task_heads:
     homo:
       out_dim: 2
-      hidden_dims: 32
-      depth: 2                          # Not needed if we have hidden_dims
+      hidden_dims: 8
+      depth: 1                          # Not needed if we have hidden_dims
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
+      task_level: graph
     alpha:
       out_dim: 1
-      hidden_dims: 32
-      depth: 2                          # Not needed if we have hidden_dims
+      hidden_dims: 8
+      depth: 1                          # Not needed if we have hidden_dims
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
+      task_level: graph
     cv:
       out_dim: 1
-      hidden_dims: 32
+      hidden_dims: 8
       depth: 2                          # Not needed if we have hidden_dims
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
+      task_level: graph
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    homo: ["mae", "pearsonr"]
+    homo: ["mae"]
     alpha: ["mae"]
-    cv: ["mae", "pearsonr"]
   loss_fun:
     homo: mse_ipu
     alpha: mse_ipu
-    cv: mse_ipu
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-3
-    # weight_decay: 1.e-7
-  torch_scheduler_kwargs:
-    #module_type: ReduceLROnPlateau
-    #factor: 0.5
-    #patience: 7
-  scheduler_kwargs: null
-  #  monitor: &monitor loss/val
-  #  mode: min
-  #  frequency: 1
-  target_nan_mask: null # null: no mask, 0: 0 mask, ignore: ignore nan values from loss
-  flag_kwargs:
-    n_steps: 0 #1
-    alpha: 0.0 #0.01
+  target_nan_mask: null
 
 # Task-specific
 metrics:
   homo:
     - name: mae
-      metric: mae_ipu
-      target_nan_mask: null
-      multitask_handling: flatten
-      threshold_kwargs: null
-    - name: pearsonr
-      metric: pearsonr_ipu
+      metric: mae
       threshold_kwargs: null
       target_nan_mask: null
-      multitask_handling: mean-per-label
-    # - name: f1 > 0.5
-    #   metric: f1
-    #   target_to_int: True
-    #   num_classes: 2
-    #   average: micro
-    #   threshold_kwargs: &threshold_05
-    #     operator: greater
-    #     threshold: 0.5
-    #     th_on_preds: True
-    #     th_on_target: True
-    # - name: precision > 0.5
-    #   metric: precision
-    #   average: micro
-    #   threshold_kwargs: *threshold_05
-
   alpha:
     - name: mae
       metric: mae
       threshold_kwargs: null
-    - name: pearsonr
-      metric: pearsonr
-      threshold_kwargs: null
-
-  cv:
-    - name: mae
-      metric: mae
-      threshold_kwargs: null
-    - name: pearsonr
-      metric: pearsonr
-      threshold_kwargs: null
 
 trainer:
   logger:
     save_dir: logs/QM9
     name: *name
-  #early_stopping:
-  #  monitor: *monitor
-  #  min_delta: 0
-  #  patience: 10
-  #  mode: &mode min
   model_checkpoint:
     dirpath: models_checkpoints/QM9/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
     save_top_k: 1
     every_n_epochs: 1
   trainer:
-    precision: 16
-    max_epochs: 5
+    max_epochs: 2
     min_epochs: 1
```

### Comparing `graphium-2.0.2/docs/tutorials/model_training/simple-molecular-model.ipynb` & `graphium-2.1.0/docs/tutorials/model_training/simple-molecular-model.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992302135702535%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, '1. select a corresponding yaml file in the "*

 * *            '[expts/main_run_multitask.py](https://github.com/datamol-io/graphium/blob/master/expts/main_run_multitask.py) '*

 * *            'i.e. by `CONFIG_FILE = "expts/configs/config_gps_10M_pcqm4m_mod.yaml"`\\n\'), (10, '*

 * *            "'There are multiple examples of YAML files located in the folder "*

 * *            '`graphium/expts/configs` that one can refer to when training a new model. The file '*

 * *            '`config_gp […]*

```diff
@@ -6,23 +6,23 @@
             "source": [
                 "# Building and training a simple model from configurations\n",
                 "\n",
                 "This tutorial will walk you through how to use a configuration file to define all the parameters of a model and of the trainer. This tutorial focuses on training from SMILES data in a CSV format.\n",
                 "\n",
                 "The work flow of testing your code on the entire pipeline is as follows:\n",
                 "\n",
-                "1. select a corresponding yaml file in the [expts/main_run_multitask.py](https://github.com/datamol-io/graphium/blob/master/expts/main_run_multitask.py) i.e. by `CONFIG_FILE = \"expts/configs/config_gps_10M_pcqm4m.yaml\"`\n",
+                "1. select a corresponding yaml file in the [expts/main_run_multitask.py](https://github.com/datamol-io/graphium/blob/master/expts/main_run_multitask.py) i.e. by `CONFIG_FILE = \"expts/configs/config_gps_10M_pcqm4m_mod.yaml\"`\n",
                 "2. modify the yaml config file\n",
                 "3. `python expts/main_run_multitask.py`\n",
                 "\n",
-                "There are multiple examples of YAML files located in the folder `graphium/expts/configs` that one can refer to when training a new model. The file `config_gps_10M_pcqm4m.yaml` shows an example of running the GPS model on the pcqm4m dataset.\n",
+                "There are multiple examples of YAML files located in the folder `graphium/expts/configs` that one can refer to when training a new model. The file `config_gps_10M_pcqm4m_mod.yaml` shows an example of running the GPS model on the pcqm4m dataset.\n",
                 "\n",
                 "## Creating the yaml file\n",
                 "\n",
-                "The first step is to create a YAML file containing all the required configurations, with an example given at `graphium/expts/config_gps_10M_pcqm4m.yaml`. We will go through each part of the configurations."
+                "The first step is to create a YAML file containing all the required configurations, with an example given at `graphium/expts/config_gps_10M_pcqm4m_mod.yaml`. We will go through each part of the configurations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -53,15 +53,15 @@
                     "text": [
                         "Yaml file loaded\n"
                     ]
                 }
             ],
             "source": [
                 "# First, let's read the yaml configuration file\n",
-                "with open(\"../../../expts/configs/config_gps_10M_pcqm4m.yaml\", \"r\") as file:\n",
+                "with open(\"../../../expts/configs/config_gps_10M_pcqm4m_mod.yaml\", \"r\") as file:\n",
                 "    yaml_config = yaml.load(file, Loader=yaml.FullLoader)\n",
                 "\n",
                 "print(\"Yaml file loaded\")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -82,15 +82,15 @@
                     "output_type": "stream",
                     "text": [
                         "constants:\n",
                         "  name: pcqm4mv2_mpnn_4layer\n",
                         "  seed: 42\n",
                         "  raise_train_error: true\n",
                         "  accelerator:\n",
-                        "    type: cpu\n",
+                        "    type: gpu\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "print_config_with_key(yaml_config, \"constants\")"
             ]
@@ -117,25 +117,27 @@
                     "text": [
                         "datamodule:\n",
                         "  module_type: MultitaskFromSmilesDataModule\n",
                         "  args:\n",
                         "    task_specific_args:\n",
                         "      homolumo:\n",
                         "        df: null\n",
-                        "        df_path: graphium/data/PCQM4M/pcqm4mv2-20k.csv\n",
+                        "        task_level: graph\n",
+                        "        df_path: ~/scratch/data/graphium/data/PCQM4M/pcqm4mv2-20k.csv\n",
                         "        smiles_col: cxsmiles\n",
                         "        label_cols:\n",
                         "        - homo_lumo_gap\n",
                         "        split_val: 0.1\n",
                         "        split_test: 0.1\n",
                         "    prepare_dict_or_graph: pyg:graph\n",
                         "    featurization_n_jobs: 30\n",
                         "    featurization_progress: true\n",
                         "    featurization_backend: loky\n",
                         "    featurization:\n",
+                        "      mask_nan: 0\n",
                         "      atom_property_list_onehot:\n",
                         "      - atomic-number\n",
                         "      - group\n",
                         "      - period\n",
                         "      - total-valence\n",
                         "      atom_property_list_float:\n",
                         "      - degree\n",
@@ -150,22 +152,52 @@
                         "      conformer_property_list:\n",
                         "      - positions_3d\n",
                         "      add_self_loop: false\n",
                         "      explicit_H: false\n",
                         "      use_bonds_weights: false\n",
                         "      pos_encoding_as_features:\n",
                         "        pos_types:\n",
-                        "          la_pos:\n",
-                        "            pos_type: laplacian_eigvec_eigval\n",
+                        "          node_laplacian_eigvec:\n",
+                        "            pos_type: laplacian_eigvec\n",
+                        "            pos_level: node\n",
                         "            num_pos: 8\n",
                         "            normalization: none\n",
                         "            disconnected_comp: true\n",
-                        "          rw_pos:\n",
-                        "            pos_type: rwse\n",
-                        "            ksteps: 16\n",
+                        "          node_laplacian_eigval:\n",
+                        "            pos_type: laplacian_eigval\n",
+                        "            pos_level: node\n",
+                        "            num_pos: 8\n",
+                        "            normalization: none\n",
+                        "            disconnected_comp: true\n",
+                        "          rw_return_probs:\n",
+                        "            pos_type: rw_return_probs\n",
+                        "            pos_level: node\n",
+                        "            ksteps:\n",
+                        "            - 4\n",
+                        "            - 8\n",
+                        "          nodepair_rw_transition_probs:\n",
+                        "            pos_type: rw_transition_probs\n",
+                        "            pos_level: edge\n",
+                        "            ksteps:\n",
+                        "            - 2\n",
+                        "            - 4\n",
+                        "          nodepair_rw_return_probs:\n",
+                        "            pos_type: rw_return_probs\n",
+                        "            pos_level: nodepair\n",
+                        "            ksteps:\n",
+                        "            - 4\n",
+                        "          electrostatic:\n",
+                        "            pos_type: electrostatic\n",
+                        "            pos_level: node\n",
+                        "          edge_commute:\n",
+                        "            pos_type: commute\n",
+                        "            pos_level: edge\n",
+                        "          nodepair_graphormer:\n",
+                        "            pos_type: graphormer\n",
+                        "            pos_level: nodepair\n",
                         "    batch_size_training: 64\n",
                         "    batch_size_inference: 16\n",
                         "    num_workers: 0\n",
                         "    persistent_workers: false\n",
                         "\n"
                     ]
                 }
@@ -222,53 +254,84 @@
                         "    last_activation: none\n",
                         "    dropout: 0.1\n",
                         "    normalization: layer_norm\n",
                         "    last_normalization: layer_norm\n",
                         "    residual_type: none\n",
                         "  pe_encoders:\n",
                         "    out_dim: 32\n",
+                        "    edge_out_dim: 16\n",
                         "    pool: sum\n",
                         "    last_norm: None\n",
                         "    encoders:\n",
-                        "      la_pos:\n",
+                        "      emb_la_pos:\n",
                         "        encoder_type: laplacian_pe\n",
                         "        input_keys:\n",
-                        "        - eigvecs\n",
-                        "        - eigvals\n",
+                        "        - laplacian_eigvec\n",
+                        "        - laplacian_eigval\n",
                         "        output_keys:\n",
                         "        - feat\n",
-                        "        hidden_dim: 64\n",
-                        "        out_dim: 32\n",
+                        "        hidden_dim: 32\n",
                         "        model_type: DeepSet\n",
                         "        num_layers: 2\n",
                         "        num_layers_post: 1\n",
                         "        dropout: 0.1\n",
                         "        first_normalization: none\n",
-                        "      rw_pos:\n",
+                        "      emb_rwse:\n",
                         "        encoder_type: mlp\n",
                         "        input_keys:\n",
-                        "        - rwse\n",
+                        "        - rw_return_probs\n",
                         "        output_keys:\n",
                         "        - feat\n",
-                        "        hidden_dim: 64\n",
-                        "        out_dim: 32\n",
+                        "        hidden_dim: 32\n",
                         "        num_layers: 2\n",
                         "        dropout: 0.1\n",
                         "        normalization: layer_norm\n",
                         "        first_normalization: layer_norm\n",
+                        "      emb_electrostatic:\n",
+                        "        encoder_type: mlp\n",
+                        "        input_keys:\n",
+                        "        - electrostatic\n",
+                        "        output_keys:\n",
+                        "        - feat\n",
+                        "        hidden_dim: 32\n",
+                        "        num_layers: 1\n",
+                        "        dropout: 0.1\n",
+                        "        normalization: layer_norm\n",
+                        "        first_normalization: layer_norm\n",
+                        "      emb_edge_rwse:\n",
+                        "        encoder_type: mlp\n",
+                        "        input_keys:\n",
+                        "        - edge_rw_transition_probs\n",
+                        "        output_keys:\n",
+                        "        - edge_feat\n",
+                        "        hidden_dim: 32\n",
+                        "        num_layers: 1\n",
+                        "        dropout: 0.1\n",
+                        "        normalization: layer_norm\n",
+                        "      emb_edge_pes:\n",
+                        "        encoder_type: cat_mlp\n",
+                        "        input_keys:\n",
+                        "        - edge_rw_transition_probs\n",
+                        "        - edge_commute\n",
+                        "        output_keys:\n",
+                        "        - edge_feat\n",
+                        "        hidden_dim: 32\n",
+                        "        num_layers: 1\n",
+                        "        dropout: 0.1\n",
+                        "        normalization: layer_norm\n",
                         "      gaussian_pos:\n",
                         "        encoder_type: gaussian_kernel\n",
                         "        input_keys:\n",
                         "        - positions_3d\n",
                         "        output_keys:\n",
                         "        - feat\n",
                         "        - nodepair_gaussian_bias_3d\n",
                         "        num_heads: 2\n",
                         "        num_layers: 2\n",
-                        "        embed_dim: 16\n",
+                        "        embed_dim: 32\n",
                         "        use_input_keys_prefix: false\n",
                         "  gnn:\n",
                         "    out_dim: 32\n",
                         "    hidden_dims: 32\n",
                         "    depth: 4\n",
                         "    activation: gelu\n",
                         "    last_activation: none\n",
@@ -285,15 +348,17 @@
                         "      mpnn_type: pyg:mpnnplus\n",
                         "      mpnn_kwargs:\n",
                         "        in_dim: 32\n",
                         "        out_dim: 32\n",
                         "        in_dim_edges: 16\n",
                         "        out_dim_edges: 16\n",
                         "      attn_type: full-attention\n",
-                        "      attn_kwargs: null\n",
+                        "      attn_kwargs:\n",
+                        "        num_heads: 2\n",
+                        "      biased_attention_key: nodepair_gaussian_bias_3d\n",
                         "  post_nn: null\n",
                         "  task_heads:\n",
                         "    homolumo:\n",
                         "      out_dim: 1\n",
                         "      hidden_dims: 256\n",
                         "      depth: 2\n",
                         "      activation: relu\n",
@@ -336,15 +401,15 @@
                         "  loss_fun:\n",
                         "    homolumo: mse_ipu\n",
                         "  random_seed: 42\n",
                         "  optim_kwargs:\n",
                         "    lr: 0.0004\n",
                         "  torch_scheduler_kwargs:\n",
                         "    module_type: WarmUpLinearLR\n",
-                        "    max_num_epochs: 100\n",
+                        "    max_num_epochs: 5\n",
                         "    warmup_epochs: 10\n",
                         "    verbose: false\n",
                         "  scheduler_kwargs: null\n",
                         "  target_nan_mask: null\n",
                         "  flag_kwargs:\n",
                         "    n_steps: 0\n",
                         "    alpha: 0.0\n",
@@ -422,15 +487,15 @@
                         "  model_checkpoint:\n",
                         "    dirpath: models_checkpoints/PCMQv2/\n",
                         "    filename: pcqm4mv2_mpnn_4layer\n",
                         "    save_top_k: 1\n",
                         "    every_n_epochs: 100\n",
                         "  trainer:\n",
                         "    precision: 32\n",
-                        "    max_epochs: 100\n",
+                        "    max_epochs: 5\n",
                         "    min_epochs: 1\n",
                         "    accumulate_grad_batches: 2\n",
                         "    check_val_every_n_epoch: 20\n",
                         "\n"
                     ]
                 }
             ],
```

### Comparing `graphium-2.0.2/env.yml` & `graphium-2.1.0/env.yml`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 
   # scientific
   - numpy
   - scipy >=1.4
   - pandas >=1.0
   - scikit-learn
   - fastparquet
+  - sympy
 
   # viz
   - matplotlib >=3.0.1
   - seaborn
 
   # cloud IO
   - fsspec >=2021.6
   - s3fs >=2021.6
   - gcsfs >=2021.6
   - platformdirs
 
   # ML packages
   - cudatoolkit  # works also with CPU-only system.
   - pytorch >=1.10.2,<2.0
+  - tensorboard
+  - lightning >=2.0
   - torchvision
-  - pytorch-lightning >=1.9
   - torchmetrics >=0.7.0,<0.11
   - ogb
   - pytorch_geometric >=2.0  # Use `pyg` for Windows instead of `pytorch_geometric`
   - wandb
   - mup
   - pytorch_sparse >=0.6
   - pytorch_cluster >=1.5
@@ -60,7 +62,11 @@
   - mkdocs-material-extensions
   - mkdocstrings
   - mkdocstrings-python
   - mkdocs-jupyter
   - mkdocs-click
   - markdown-include
   - mike >=1.0.0
+
+  - pip
+  - pip:
+    - lightning-graphcore  # optional, for using IPUs only
```

### Comparing `graphium-2.0.2/expts/configs/config_gps_10M_pcqm4m.yaml` & `graphium-2.1.0/expts/configs/config_gps_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/configs/config_gps_10M_pcqm4m_mod.yaml` & `graphium-2.1.0/expts/configs/config_gps_10M_pcqm4m_mod.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/configs/config_gpspp_10M_pcqm4m.yaml` & `graphium-2.1.0/expts/configs/config_gpspp_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/configs/config_mpnn_10M_b3lyp.yaml` & `graphium-2.1.0/expts/configs/config_mpnn_10M_b3lyp.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/configs/config_mpnn_10M_pcqm4m.yaml` & `graphium-2.1.0/expts/configs/config_mpnn_10M_pcqm4m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         batch_size_training: 64
         batch_size_inference: 16
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 16
+        precision: 16-true
         accumulate_grad_batches: 4
 
   ipu_config:
     - deviceIterations(20) # IPU would require large batches to be ready for the model.
     - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
```

### Comparing `graphium-2.0.2/expts/configs/config_mpnn_pcqm4m.yaml` & `graphium-2.1.0/expts/configs/config_mpnn_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/data/micro_zinc_splits.csv` & `graphium-2.1.0/expts/data/micro_zinc_splits.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/dataset_benchmark.py` & `graphium-2.1.0/expts/dataset_benchmark.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/expts/main_run_get_fingerprints.py` & `graphium-2.1.0/expts/main_run_get_fingerprints.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from os.path import dirname, abspath
 import yaml
 import numpy as np
 import pandas as pd
 import torch
 import fsspec
-from pytorch_lightning.utilities.model_summary import ModelSummary
+from lightning.pytorch.utilities.model_summary import ModelSummary
 
 # Current project imports
 import graphium
 from graphium.config._loader import load_datamodule, load_trainer
 from graphium.utils.fs import mkdir
 from graphium.trainer.predictor import PredictorModule
```

### Comparing `graphium-2.0.2/expts/main_run_multitask.py` & `graphium-2.1.0/expts/main_run_multitask.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from os.path import dirname, abspath
 import yaml
 from copy import deepcopy
 from omegaconf import DictConfig
 import timeit
 from loguru import logger
 from datetime import datetime
-from pytorch_lightning.utilities.model_summary import ModelSummary
+from lightning.pytorch.utilities.model_summary import ModelSummary
 
 # Current project imports
 import graphium
 from graphium.config._loader import (
     load_datamodule,
     load_metrics,
     load_architecture,
     load_predictor,
     load_trainer,
     save_params_to_wandb,
     load_accelerator,
+    load_yaml_config,
 )
 from graphium.utils.safe_run import SafeRun
 from graphium.utils.command_line_utils import update_config, get_anchors_and_aliases
 
 
 # WandB
 import wandb
@@ -31,16 +32,17 @@
 # Set up the working directory
 MAIN_DIR = dirname(dirname(abspath(graphium.__file__)))
 
 # CONFIG_FILE = "expts/configs/config_mpnn_10M_b3lyp.yaml"
 # CONFIG_FILE = "expts/configs/config_mpnn_10M_pcqm4m.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_debug.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_mpnn.yaml"
-CONFIG_FILE = "expts/neurips2023_configs/config_large_gcn.yaml"
+CONFIG_FILE = "expts/neurips2023_configs/debug/config_small_gcn_debug.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_gin.yaml"
+# CONFIG_FILE = "expts/neurips2023_configs/config_large_gcn.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_gine.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_small_gcn.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_small_gin.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_small_gine.yaml"
 
 os.chdir(MAIN_DIR)
 
@@ -48,16 +50,15 @@
 def main(cfg: dict, run_name: str = "main", add_date_time: bool = True) -> None:
     st = timeit.default_timer()
 
     date_time_suffix = ""
     if add_date_time:
         date_time_suffix = datetime.now().strftime("%d.%m.%Y_%H.%M.%S")
 
-    cfg = deepcopy(cfg)
-    wandb.init(project=cfg["constants"]["name"], config=cfg)
+    wandb.init(entity="multitask-gnn", project=cfg["constants"]["name"], config=cfg)
 
     # Initialize the accelerator
     cfg, accelerator_type = load_accelerator(cfg)
 
     # Load and initialize the dataset
     datamodule = load_datamodule(cfg, accelerator_type)
 
@@ -79,14 +80,15 @@
     logger.info(predictor.model)
     logger.info(ModelSummary(predictor, max_depth=4))
 
     trainer = load_trainer(cfg, run_name, accelerator_type, date_time_suffix)
     save_params_to_wandb(trainer.logger, cfg, predictor, datamodule)
 
     # Determine the max num nodes and edges in training and validation
+    logger.info("About to set the max nodes etc.")
     predictor.set_max_nodes_edges_per_graph(datamodule, stages=["train", "val"])
 
     # Run the model training
     with SafeRun(name="TRAINING", raise_error=cfg["constants"]["raise_train_error"], verbose=True):
         trainer.fit(model=predictor, datamodule=datamodule)
 
     # Determine the max num nodes and edges in testing
@@ -104,17 +106,13 @@
     return trainer.callback_metrics
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--config", help="Path to the config file", default=None)
 
-    args, unknown = parser.parse_known_args()
-    # Optionally parse the config with the command line
+    args, unknown_args = parser.parse_known_args()
     if args.config is not None:
         CONFIG_FILE = args.config
+    cfg = load_yaml_config(CONFIG_FILE, MAIN_DIR, unknown_args)
 
-    with open(os.path.join(MAIN_DIR, CONFIG_FILE), "r") as f:
-        cfg = yaml.safe_load(f)
-        refs = get_anchors_and_aliases(CONFIG_FILE)
-        cfg = update_config(cfg, unknown, refs)
     main(cfg)
```

### Comparing `graphium-2.0.2/expts/main_run_predict.py` & `graphium-2.1.0/expts/main_run_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path import dirname, abspath
 import yaml
 from copy import deepcopy
 from omegaconf import DictConfig
 import numpy as np
 import pandas as pd
 import torch
-from pytorch_lightning.utilities.model_summary import ModelSummary
+from lightning.pytorch.utilities.model_summary import ModelSummary
 
 # Current project imports
 import graphium
 from graphium.config._loader import load_datamodule, load_trainer
 from graphium.utils.fs import mkdir
 from graphium.trainer.predictor import PredictorModule
```

### Comparing `graphium-2.0.2/expts/main_run_test.py` & `graphium-2.1.0/expts/main_run_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # General imports
 import os
 from os.path import dirname, abspath
 import yaml
 from copy import deepcopy
 from omegaconf import DictConfig
-from pytorch_lightning.utilities.model_summary import ModelSummary
+from lightning.pytorch.utilities.model_summary import ModelSummary
 
 # Current project imports
 import graphium
 from graphium.config._loader import load_datamodule, load_metrics, load_trainer
 
 from graphium.trainer.predictor import PredictorModule
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_classifigression_l1000.yaml` & `graphium-2.1.0/expts/neurips2023_configs/config_classifigression_l1000.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,15 @@
       target_to_int: True
       task: multiclass
       num_classes: 5
       top_k: 1
   l1000_mcf7: *classif_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_debug.yaml` & `graphium-2.1.0/expts/neurips2023_configs/debug/config_debug.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Testing the mpnn only model with the PCQMv2 dataset on IPU.
 constants:
   name: &name neurips2023_small_data_mpnn
-  seed: &seed 42
+  seed: &seed 999
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 # accelerator:
 #   type: ipu  # cpu or ipu or gpu
 #   config_override:
 #     datamodule:
 #       args:
@@ -248,14 +248,15 @@
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_large_gcn.yaml` & `graphium-2.1.0/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Testing the gcn model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_gcn
-  seed: &seed 42
+  name: &name neurips2023_large_data_gcn_debug
+  seed: &seed 100
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
@@ -14,27 +14,27 @@
           max_num_nodes_per_graph: 40 # train max nodes: 20, max_edges: 54
           max_num_edges_per_graph: 80
         ipu_dataloader_inference_opts:
           mode: async
           max_num_nodes_per_graph: 40 # valid max nodes: 51, max_edges: 118
           max_num_edges_per_graph: 80
         # Data handling-related
-        batch_size_training: 10
-        batch_size_inference: 10
+        batch_size_training: 20
+        batch_size_inference: 20
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 32
-        accumulate_grad_batches: 8
+        precision: 16
+        accumulate_grad_batches: 4
 
   ipu_config:
-    - deviceIterations(10) # IPU would require large batches to be ready for the model.
-    - replicationFactor(16)
+    - deviceIterations(2) # IPU would require large batches to be ready for the model.
+    - replicationFactor(4)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
 
 # accelerator:
@@ -56,65 +56,67 @@
       l1000_vcap:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
 
       l1000_mcf7:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
 
       pcba_1328:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCBA_1328_1564k.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCBA_1328_1564k.parquet
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: assayID-*  # assayID-* means all columns starting with "assayID-"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcba_1328_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcba_1328_random_splits.pt`
 
       pcqm4m_g25:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: graph_*  # graph_* means all columns starting with "graph_"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
       pcqm4m_n4:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: node_* # node_* means all columns starting with "node_"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: node
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         seed: *seed
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
@@ -199,15 +201,15 @@
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
     in_dim: 64 # or otherwise the correct value
-    out_dim: &gnn_dim 1024
+    out_dim: &gnn_dim 768
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
@@ -244,26 +246,26 @@
   task_heads:
     l1000_vcap:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
     l1000_mcf7:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
     pcba_1328:
       task_level: graph
       out_dim: 1328
@@ -302,93 +304,110 @@
 predictor:
   metrics_on_progress_bar:
     l1000_vcap: []
     l1000_mcf7: []
     pcba_1328: []
     pcqm4m_g25: []
     pcqm4m_n4: []
+  metrics_on_training_set:
+    l1000_vcap: []
+    l1000_mcf7: []
+    pcba_1328: []
+    pcqm4m_g25: []
+    pcqm4m_n4: [] 
   loss_fun:
-    l1000_vcap: hybrid_ce_ipu
-    l1000_mcf7: hybrid_ce_ipu
+    l1000_vcap:
+      name: hybrid_ce_ipu
+      n_brackets: 5
+    l1000_mcf7:
+      name: hybrid_ce_ipu
+      n_brackets: 5
     pcba_1328: bce_ipu
     pcqm4m_g25: mae_ipu
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 5.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
-    warmup_epochs: 10
+    max_num_epochs: &max_epochs 10
+    warmup_epochs: 5
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
   l1000_vcap: &classif_metrics
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
       num_classes: 5
       task: multiclass
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
+    - name: avpr
       metric: average_precision_ipu
       num_classes: 5
       task: multiclass
       target_to_int: True
       target_nan_mask: -1000
       ignore_index: -1000
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
   l1000_mcf7: *classif_metrics
   pcba_1328:
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
       task: binary
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
+    - name: avpr
       metric: average_precision_ipu
       task: binary
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
   pcqm4m_g25: &pcqm_metrics
     - name: mae
       metric: mae_ipu
       target_nan_mask: null
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
+    - name: r2
+      metric: r2_score_ipu
+      threshold_kwargs: null
+      target_nan_mask: null
+      multitask_handling: mean-per-label
   pcqm4m_n4: *pcqm_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-large/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large/
+    dirpath: models_checkpoints/neurips2023-large-gcn-debug/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    every_n_epochs: 5
+    save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
-    check_val_every_n_epoch: 20
+    check_val_every_n_epoch: 10
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_large_gin.yaml` & `graphium-2.1.0/expts/neurips2023_configs/config_large_gcn.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Testing the gin model with the PCQMv2 dataset on IPU.
+# Testing the gcn model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_large_data_gin
+  name: &name neurips2023_large_data_gcn
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 40 # train max nodes: 20, max_edges: 54
-          max_num_edges_per_graph: 80
+          max_num_nodes_per_graph: 60 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 40 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 80
+          max_num_nodes_per_graph: 60 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 100
         # Data handling-related
         batch_size_training: 10
         batch_size_inference: 10
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
@@ -93,36 +93,38 @@
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: graph_*  # graph_* means all columns starting with "graph_"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
       pcqm4m_n4:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: node_* # node_* means all columns starting with "node_"
         # sample_size: 2000 # use sample_size for test
         task_level: node
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         seed: *seed
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "../datacache/neurips2023-large/"
+    processed_graph_data_path: "/net/group/software-apps/datacache/neurips2023-large/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -199,25 +201,25 @@
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
     in_dim: 64 # or otherwise the correct value
-    out_dim: &gnn_dim 832
+    out_dim: &gnn_dim 768
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gcn' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
@@ -244,26 +246,26 @@
   task_heads:
     l1000_vcap:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
     l1000_mcf7:
       task_level: graph
       out_dim: 4890
       hidden_dims: 128
       depth: 2
       activation: none
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
     pcba_1328:
       task_level: graph
       out_dim: 1328
@@ -302,93 +304,104 @@
 predictor:
   metrics_on_progress_bar:
     l1000_vcap: []
     l1000_mcf7: []
     pcba_1328: []
     pcqm4m_g25: []
     pcqm4m_n4: []
+  metrics_on_training_set:
+    l1000_vcap: []
+    l1000_mcf7: []
+    pcba_1328: []
+    pcqm4m_g25: []
+    pcqm4m_n4: []
   loss_fun:
-    l1000_vcap: hybrid_ce_ipu
-    l1000_mcf7: hybrid_ce_ipu
+    l1000_vcap:
+      name: hybrid_ce_ipu
+      n_brackets: 5
+    l1000_mcf7:
+      name: hybrid_ce_ipu
+      n_brackets: 5
     pcba_1328: bce_ipu
     pcqm4m_g25: mae_ipu
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
+    max_num_epochs: &max_epochs 20
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
   l1000_vcap: &classif_metrics
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
       num_classes: 5
       task: multiclass
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
+    - name: avpr
       metric: average_precision_ipu
       num_classes: 5
       task: multiclass
       target_to_int: True
       target_nan_mask: -1000
       ignore_index: -1000
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
   l1000_mcf7: *classif_metrics
   pcba_1328:
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
       task: binary
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
+    - name: avpr
       metric: average_precision_ipu
       task: binary
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       threshold_kwargs: null
   pcqm4m_g25: &pcqm_metrics
     - name: mae
       metric: mae_ipu
       target_nan_mask: null
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
+    - name: r2
+      metric: r2_score_ipu
+      threshold_kwargs: null
+      target_nan_mask: null
+      multitask_handling: mean-per-label
   pcqm4m_n4: *pcqm_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-large/
     name: *name
     project: *name
-  #early_stopping:
-  #  monitor: *monitor
-  #  min_delta: 0
-  #  patience: 10
-  #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-large/
+    dirpath: models_checkpoints/neurips2023-large-gcn/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
     check_val_every_n_epoch: 20
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_luis_jama.yaml` & `graphium-2.1.0/expts/neurips2023_configs/config_luis_jama.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,15 @@
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
   pcqm20k_n4: *pcqm_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_small_gated_gcn.yaml` & `graphium-2.1.0/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Testing the gated_gcn model with the PCQMv2 dataset on IPU.
+# Testing the gcn model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_small_data_gated_gcn
-  seed: &seed 42
+  name: &name neurips2023_small_data_gcn
+  seed: &seed 3000
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # train max nodes: 20, max_edges: 54
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 44 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 80
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 100 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 200
         # Data handling-related
-        batch_size_training: 50
-        batch_size_inference: 50
+        batch_size_training: 5
+        batch_size_inference: 2
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
         precision: 16
         accumulate_grad_batches: 4
 
   ipu_config:
     - deviceIterations(5) # IPU would require large batches to be ready for the model.
-    - replicationFactor(8)
+    - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
 
 # accelerator:
@@ -61,14 +61,15 @@
         smiles_col: "smiles"
         label_cols: ["A", "B", "C", "mu", "alpha", "homo", "lumo", "gap", "r2", "zpve", "u0", "u298", "h298", "g298", "cv", "u0_atom", "u298_atom", "h298_atom", "g298_atom"]
         # sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/qm9_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
       tox21:
         df: null
         df_path: data/neurips2023/small-dataset/Tox21-7k-12-labels.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21-7k-12-labels.csv.gz
         # or set path as the URL directly
@@ -87,14 +88,15 @@
         smiles_col: "smiles"
         label_cols: ["SA", "logp", "score"]
         # sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/ZINC12k_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
@@ -141,29 +143,20 @@
   mup_base_path: null
   pre_nn:   # Set as null to avoid a pre-nn network
     out_dim: 64
     hidden_dims: 256
     depth: 2
     activation: relu
     last_activation: none
-    dropout: &dropout 0.18
+    dropout: &dropout 0.1
     normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
-  pre_nn_edges:   # Set as null to avoid a pre-nn network
-    out_dim: 32
-    hidden_dims: 128
-    depth: 2
-    activation: relu
-    last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: *normalization
-    residual_type: none
+  pre_nn_edges: null   # Set as null to avoid a pre-nn network
 
   pe_encoders:
     out_dim: 32
     pool: "sum" #"mean" "max"
     last_norm: None #"batch_norm", "layer_norm"
     encoders: #la_pos |  rw_pos
       la_pos:  # Set as null to avoid a pre-nn network
@@ -187,25 +180,26 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: &gnn_dim 64
+    in_dim: 64 # or otherwise the correct value
+    out_dim: &gnn_dim 128
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gated-gcn' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gcn' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
     layer_kwargs: null # Parameters for the model itself. You could define dropout_attn: 0.1
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
@@ -218,15 +212,15 @@
       last_normalization: "none"
       residual_type: none
 
   task_heads:
     qm9:
       task_level: graph
       out_dim: 19
-      hidden_dims: 128
+      hidden_dims: 256
       depth: 2
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
@@ -253,27 +247,27 @@
       last_normalization: "none"
       residual_type: none
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
     qm9: ["mae"]
-    tox21: ["auroc_flat"]
+    tox21: ["auroc"]
     zinc: ["mae"]
   loss_fun:
     qm9: mae_ipu
     tox21: bce_ipu
     zinc: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
+    max_num_epochs: &max_epochs 300
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
@@ -288,22 +282,29 @@
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
+    - name: r2_score
+      metric: r2_score_ipu
+      target_nan_mask: null
+      multitask_handling: mean-per-label
+      threshold_kwargs: null
   tox21:
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
-      multitask_handling: flatten
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
-      metric: averageprecision
-      multitask_handling: flatten
+    - name: avpr
+      metric: average_precision_ipu
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: f1 > 0.5
       metric: f1
       multitask_handling: flatten
       target_to_int: True
       num_classes: 2
       average: micro
@@ -316,25 +317,26 @@
       metric: precision
       multitask_handling: flatten
       average: micro
       threshold_kwargs: *threshold_05
   zinc: *qm9_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-small/
+    dirpath: models_checkpoints/neurips2023-small-gcn/
     filename: *name
     #monitor: *monitor
     #mode: *mode
     save_top_k: 1
     every_n_epochs: 100
   trainer:
     max_epochs: *max_epochs
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_small_gcn.yaml` & `graphium-2.1.0/expts/neurips2023_configs/config_small_gcn.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # train max nodes: 20, max_edges: 54
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 44 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 80
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 44 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 80
         # Data handling-related
         batch_size_training: 50
         batch_size_inference: 50
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
@@ -33,14 +33,25 @@
     - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
 
+# accelerator:
+#   type: cpu  # cpu or ipu or gpu
+#   config_override:
+#     datamodule:
+#       batch_size_training: 64
+#       batch_size_inference: 256
+#     trainer:
+#       trainer:
+#         precision: 32
+#         accumulate_grad_batches: 1
+
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
       qm9:
         df: null
@@ -50,14 +61,15 @@
         smiles_col: "smiles"
         label_cols: ["A", "B", "C", "mu", "alpha", "homo", "lumo", "gap", "r2", "zpve", "u0", "u298", "h298", "g298", "cv", "u0_atom", "u298_atom", "h298_atom", "g298_atom"]
         # sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/qm9_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
       tox21:
         df: null
         df_path: data/neurips2023/small-dataset/Tox21-7k-12-labels.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21-7k-12-labels.csv.gz
         # or set path as the URL directly
@@ -76,14 +88,15 @@
         smiles_col: "smiles"
         label_cols: ["SA", "logp", "score"]
         # sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/ZINC12k_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
@@ -168,15 +181,15 @@
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
     in_dim: 64 # or otherwise the correct value
-    out_dim: &gnn_dim 128
+    out_dim: &gnn_dim 96
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
@@ -234,15 +247,15 @@
       last_normalization: "none"
       residual_type: none
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
     qm9: ["mae"]
-    tox21: ["auroc_flat"]
+    tox21: ["auroc"]
     zinc: ["mae"]
   loss_fun:
     qm9: mae_ipu
     tox21: bce_ipu
     zinc: mae_ipu
   random_seed: *seed
   optim_kwargs:
@@ -269,55 +282,63 @@
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
+    - name: r2_score
+      metric: r2_score_ipu
+      target_nan_mask: null
+      multitask_handling: mean-per-label
+      threshold_kwargs: null
   tox21:
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
-      multitask_handling: flatten
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
-      metric: averageprecision
-      multitask_handling: flatten
+    - name: avpr
+      metric: average_precision_ipu
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: f1 > 0.5
       metric: f1
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       target_to_int: True
       num_classes: 2
       average: micro
       threshold_kwargs: &threshold_05
         operator: greater
         threshold: 0.5
         th_on_preds: True
         th_on_target: True
     - name: precision > 0.5
       metric: precision
-      multitask_handling: flatten
+      multitask_handling: mean-per-label
       average: micro
       threshold_kwargs: *threshold_05
   zinc: *qm9_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-small/
+    dirpath: models_checkpoints/neurips2023-small-gcn/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
     check_val_every_n_epoch: 20
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_small_gin.yaml` & `graphium-2.1.0/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Testing the gin model with the PCQMv2 dataset on IPU.
+# Testing the gcn model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_small_data_gin
+  name: &name neurips2023_small_data_gcn
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
@@ -22,75 +22,64 @@
         batch_size_inference: 50
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
         precision: 16
-        accumulate_grad_batches: 4
+        accumulate_grad_batches: 1
 
   ipu_config:
     - deviceIterations(5) # IPU would require large batches to be ready for the model.
-    - replicationFactor(16)
+    - replicationFactor(2)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
 
-# accelerator:
-#   type: cpu  # cpu or ipu or gpu
-#   config_override:
-#     datamodule:
-#       batch_size_training: 64
-#       batch_size_inference: 256
-#     trainer:
-#       trainer:
-#         precision: 32
-#         accumulate_grad_batches: 1
-
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
       qm9:
         df: null
         df_path: data/neurips2023/small-dataset/qm9.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9.csv.gz
         # or set path as the URL directly
         smiles_col: "smiles"
         label_cols: ["A", "B", "C", "mu", "alpha", "homo", "lumo", "gap", "r2", "zpve", "u0", "u298", "h298", "g298", "cv", "u0_atom", "u298_atom", "h298_atom", "g298_atom"]
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/qm9_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
           method: "normal"
 
       tox21:
         df: null
         df_path: data/neurips2023/small-dataset/Tox21-7k-12-labels.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21-7k-12-labels.csv.gz
         # or set path as the URL directly
         smiles_col: "smiles"
         label_cols: ["NR-AR", "NR-AR-LBD", "NR-AhR", "NR-Aromatase", "NR-ER", "NR-ER-LBD", "NR-PPAR-gamma", "SR-ARE", "SR-ATAD5", "SR-HSE", "SR-MMP", "SR-p53"]
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/Tox21_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21_random_splits.pt`
         seed: *seed
         task_level: graph
 
       zinc:
         df: null
         df_path: data/neurips2023/small-dataset/ZINC12k.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k.csv.gz
         # or set path as the URL directly
         smiles_col: "smiles"
         label_cols: ["SA", "logp", "score"]
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         splits_path: data/neurips2023/small-dataset/ZINC12k_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k_random_splits.pt`
         seed: *seed
         task_level: graph
         label_normalization:
           method: "normal"
 
     # Featurization
@@ -179,25 +168,25 @@
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
     in_dim: 64 # or otherwise the correct value
-    out_dim: &gnn_dim 64
+    out_dim: &gnn_dim 128
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gin' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+    layer_type: 'pyg:gcn' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
     layer_kwargs: null # Parameters for the model itself. You could define dropout_attn: 0.1
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
@@ -245,27 +234,27 @@
       last_normalization: "none"
       residual_type: none
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
     qm9: ["mae"]
-    tox21: ["auroc_flat"]
+    tox21: ["auroc"]
     zinc: ["mae"]
   loss_fun:
     qm9: mae_ipu
     tox21: bce_ipu
     zinc: mae_ipu
   random_seed: *seed
   optim_kwargs:
     lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
+    max_num_epochs: &max_epochs 20
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
@@ -281,21 +270,23 @@
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
   tox21:
-    - name: auroc_flat
+    - name: auroc
       metric: auroc_ipu
-      multitask_handling: flatten
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-    - name: avpr_flat
-      metric: averageprecision
-      multitask_handling: flatten
+    - name: avpr
+      metric: average_precision_ipu
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
     - name: f1 > 0.5
       metric: f1
       multitask_handling: flatten
       target_to_int: True
       num_classes: 2
       average: micro
@@ -308,27 +299,30 @@
       metric: precision
       multitask_handling: flatten
       average: micro
       threshold_kwargs: *threshold_05
   zinc: *qm9_metrics
 
 trainer:
+  seed: *seed
   logger:
     save_dir: logs/neurips2023-small/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-small/
+    dirpath: "models_checkpoints/neurips2023-small-gcn/"
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    # every_n_epochs: 4
+    save_last: True
+    # save_on_train_epoch_end: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
-    check_val_every_n_epoch: 20
+    check_val_every_n_epoch: 4
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_small_gine.yaml` & `graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Testing the gine model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_small_data_gine
+  name: &name neurips2023_large_data_gine_pcq
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # train max nodes: 20, max_edges: 54
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 30 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 24 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 30 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 100
         # Data handling-related
-        batch_size_training: 50
-        batch_size_inference: 50
+        batch_size_training: 10
+        batch_size_inference: 10
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 16
-        accumulate_grad_batches: 4
+        precision: 32
+        accumulate_grad_batches: 8
 
   ipu_config:
-    - deviceIterations(5) # IPU would require large batches to be ready for the model.
+    - deviceIterations(10) # IPU would require large batches to be ready for the model.
     - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
     - _Popart.set("defaultBufferingDepth", 128)
     - Precision.enableStochasticRounding(True)
 
@@ -49,60 +49,49 @@
 #         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
-      qm9:
+      pcqm4m_g25:
         df: null
-        df_path: data/neurips2023/small-dataset/qm9.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9.csv.gz
+        df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["A", "B", "C", "mu", "alpha", "homo", "lumo", "gap", "r2", "zpve", "u0", "u298", "h298", "g298", "cv", "u0_atom", "u298_atom", "h298_atom", "g298_atom"]
+        smiles_col: "ordered_smiles"
+        label_cols: graph_*  # graph_* means all columns starting with "graph_"
         # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/qm9_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9_random_splits.pt`
-        seed: *seed
         task_level: graph
+        splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
-      tox21:
-        df: null
-        df_path: data/neurips2023/small-dataset/Tox21-7k-12-labels.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21-7k-12-labels.csv.gz
-        # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["NR-AR", "NR-AR-LBD", "NR-AhR", "NR-Aromatase", "NR-ER", "NR-ER-LBD", "NR-PPAR-gamma", "SR-ARE", "SR-ATAD5", "SR-HSE", "SR-MMP", "SR-p53"]
-        # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/Tox21_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21_random_splits.pt`
-        seed: *seed
-        task_level: graph
-
-      zinc:
+      pcqm4m_n4:
         df: null
-        df_path: data/neurips2023/small-dataset/ZINC12k.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k.csv.gz
+        df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["SA", "logp", "score"]
+        smiles_col: "ordered_smiles"
+        label_cols: node_* # node_* means all columns starting with "node_"
         # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/ZINC12k_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k_random_splits.pt`
+        task_level: node
+        splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         seed: *seed
-        task_level: graph
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "../datacache/neurips2023-small/"
+    processed_graph_data_path: "../datacache/neurips2023-large/pcq/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -187,156 +176,137 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: &gnn_dim 64
+    out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
     layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
-    layer_kwargs: null # Parameters for the model itself. You could define dropout_attn: 0.1
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
       depth: 1
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
-
-  task_heads:
-    qm9:
-      task_level: graph
-      out_dim: 19
-      hidden_dims: 128
-      depth: 2
+    node:
+      pooling: [sum]
+      out_dim: *gnn_dim
+      hidden_dims: *gnn_dim
+      depth: 1
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
-    tox21:
+
+  task_heads:
+    pcqm4m_g25:
       task_level: graph
-      out_dim: 12
-      hidden_dims: 64
+      out_dim: 25
+      hidden_dims: 32
       depth: 2
       activation: relu
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
-    zinc:
-      task_level: graph
-      out_dim: 3
+    pcqm4m_n4:
+      task_level: node
+      out_dim: 4
       hidden_dims: 32
       depth: 2
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    qm9: ["mae"]
-    tox21: ["auroc_flat"]
-    zinc: ["mae"]
+    pcqm4m_g25: []
+    pcqm4m_n4: []
+  metrics_on_training_set:
+    pcqm4m_g25: []
+    pcqm4m_n4: []
   loss_fun:
-    qm9: mae_ipu
-    tox21: bce_ipu
-    zinc: mae_ipu
+    pcqm4m_g25: mae_ipu
+    pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
+    max_num_epochs: &max_epochs 20
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
-  qm9: &qm9_metrics
+  pcqm4m_g25: &pcqm_metrics
     - name: mae
       metric: mae_ipu
       target_nan_mask: null
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
-  tox21:
-    - name: auroc_flat
-      metric: auroc_ipu
-      multitask_handling: flatten
-      threshold_kwargs: null
-    - name: avpr_flat
-      metric: averageprecision
-      multitask_handling: flatten
+    - name: r2
+      metric: r2_score_ipu
       threshold_kwargs: null
-    - name: f1 > 0.5
-      metric: f1
-      multitask_handling: flatten
-      target_to_int: True
-      num_classes: 2
-      average: micro
-      threshold_kwargs: &threshold_05
-        operator: greater
-        threshold: 0.5
-        th_on_preds: True
-        th_on_target: True
-    - name: precision > 0.5
-      metric: precision
-      multitask_handling: flatten
-      average: micro
-      threshold_kwargs: *threshold_05
-  zinc: *qm9_metrics
+      target_nan_mask: null
+      multitask_handling: mean-per-label
+  pcqm4m_n4: *pcqm_metrics
 
 trainer:
+  seed: *seed
   logger:
-    save_dir: logs/neurips2023-small/
+    save_dir: logs/neurips2023-large/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-small/
+    dirpath: models_checkpoints/neurips2023-large-gine/pcq/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
     check_val_every_n_epoch: 20
```

### Comparing `graphium-2.0.2/expts/neurips2023_configs/config_small_mpnn.yaml` & `graphium-2.1.0/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,82 @@
-# Testing the mpnn only model with the PCQMv2 dataset on IPU.
+# Testing the gine model with the PCQMv2 dataset on IPU.
 constants:
-  name: &name neurips2023_small_data_mpnn
+  name: &name neurips2023_large_data_gine_g25
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
-# accelerator:
-#   type: ipu  # cpu or ipu or gpu
-#   config_override:
-#     datamodule:
-#       args:
-#         ipu_dataloader_training_opts:
-#           mode: async
-#           max_num_nodes_per_graph: 24 # train max nodes: 20, max_edges: 54
-#           max_num_edges_per_graph: 60
-#         ipu_dataloader_inference_opts:
-#           mode: async
-#           max_num_nodes_per_graph: 24 # valid max nodes: 51, max_edges: 118
-#           max_num_edges_per_graph: 60
-#         # Data handling-related
-#         batch_size_training: 50
-#         batch_size_inference: 50
-#     predictor:
-#       optim_kwargs:
-#         loss_scaling: 1024
-#     trainer:
-#       trainer:
-#         precision: 16
-#         accumulate_grad_batches: 4
-
-#   ipu_config:
-#     - deviceIterations(20) # IPU would require large batches to be ready for the model.
-#     - replicationFactor(8)
-#     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
-#     # - enableExecutableCaching("pop_compiler_cache")
-#     - TensorLocations.numIOTiles(128)
-#     - _Popart.set("defaultBufferingDepth", 128)
-#     - Precision.enableStochasticRounding(True)
-
 accelerator:
-  type: cpu  # cpu or ipu or gpu
+  type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
-      batch_size_training: 64
-      batch_size_inference: 256
+      args:
+        ipu_dataloader_training_opts:
+          mode: async
+          max_num_nodes_per_graph: 30 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 100
+        ipu_dataloader_inference_opts:
+          mode: async
+          max_num_nodes_per_graph: 30 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 100
+        # Data handling-related
+        batch_size_training: 10
+        batch_size_inference: 10
+    predictor:
+      optim_kwargs:
+        loss_scaling: 1024
     trainer:
       trainer:
         precision: 32
-        accumulate_grad_batches: 1
+        accumulate_grad_batches: 8
+
+  ipu_config:
+    - deviceIterations(10) # IPU would require large batches to be ready for the model.
+    - replicationFactor(16)
+    # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
+    # - enableExecutableCaching("pop_compiler_cache")
+    - TensorLocations.numIOTiles(128)
+    - _Popart.set("defaultBufferingDepth", 128)
+    - Precision.enableStochasticRounding(True)
+
+# accelerator:
+#   type: cpu  # cpu or ipu or gpu
+#   config_override:
+#     datamodule:
+#       batch_size_training: 64
+#       batch_size_inference: 256
+#     trainer:
+#       trainer:
+#         precision: 32
+#         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
   # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
-      qm9:
-        df: null
-        df_path: data/neurips2023/small-dataset/qm9.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9.csv.gz
-        # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["A", "B", "C", "mu", "alpha", "homo", "lumo", "gap", "r2", "zpve", "u0", "u298", "h298", "g298", "cv", "u0_atom", "u298_atom", "h298_atom", "g298_atom"]
-        # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/qm9_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/qm9_random_splits.pt`
-        seed: *seed
-        task_level: graph
-        label_normalization:
-          method: "normal"
-
-      tox21:
-        df: null
-        df_path: data/neurips2023/small-dataset/Tox21-7k-12-labels.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21-7k-12-labels.csv.gz
-        # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["NR-AR", "NR-AR-LBD", "NR-AhR", "NR-Aromatase", "NR-ER", "NR-ER-LBD", "NR-PPAR-gamma", "SR-ARE", "SR-ATAD5", "SR-HSE", "SR-MMP", "SR-p53"]
-        # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/Tox21_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/Tox21_random_splits.pt`
-        seed: *seed
-        task_level: graph
-
-      zinc:
+      pcqm4m_g25:
         df: null
-        df_path: data/neurips2023/small-dataset/ZINC12k.csv.gz
-        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k.csv.gz
+        df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
-        smiles_col: "smiles"
-        label_cols: ["SA", "logp", "score"]
+        smiles_col: "ordered_smiles"
+        label_cols: graph_*  # graph_* means all columns starting with "graph_"
         # sample_size: 2000 # use sample_size for test
-        splits_path: data/neurips2023/small-dataset/ZINC12k_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Small-dataset/ZINC12k_random_splits.pt`
-        seed: *seed
         task_level: graph
+        splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
+          normalize_val_test: True
           method: "normal"
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
-    processed_graph_data_path: "../datacache/neurips2023-small/"
+    processed_graph_data_path: "../datacache/neurips2023-large/g25/"
     featurization:
     # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
     # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
     # 'num_chiral_centers (not included yet)']
       atom_property_list_onehot: [atomic-number, group, period, total-valence]
       atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
       # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
@@ -187,35 +161,25 @@
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
 
 
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: &gnn_dim 64
+    out_dim: &gnn_dim 704
     hidden_dims: *gnn_dim
     depth: 4
     activation: gelu
     last_activation: none
     dropout: 0.1
     normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gps' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
-    layer_kwargs:  # Parameters for the model itself. You could define dropout_attn: 0.1
-      node_residual: false
-      mpnn_type: 'pyg:mpnnplus'
-      mpnn_kwargs:
-        in_dim: *gnn_dim
-        out_dim: *gnn_dim
-        in_dim_edges: 32
-        out_dim_edges: 32
-      attn_type: "none" # "full-attention", "none"
-      attn_kwargs: null
+    layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 
   graph_output_nn:
     graph:
       pooling: [sum]
       out_dim: *gnn_dim
       hidden_dims: *gnn_dim
@@ -224,128 +188,84 @@
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
   task_heads:
-    qm9:
-      task_level: graph
-      out_dim: 19
-      hidden_dims: 128
-      depth: 2
-      activation: relu
-      last_activation: none
-      dropout: *dropout
-      normalization: *normalization
-      last_normalization: "none"
-      residual_type: none
-    tox21:
-      task_level: graph
-      out_dim: 12
-      hidden_dims: 64
-      depth: 2
-      activation: relu
-      last_activation: sigmoid
-      dropout: *dropout
-      normalization: *normalization
-      last_normalization: "none"
-      residual_type: none
-    zinc:
+    pcqm4m_g25:
       task_level: graph
-      out_dim: 3
+      out_dim: 25
       hidden_dims: 32
       depth: 2
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    qm9: ["mae"]
-    tox21: ["auroc_flat"]
-    zinc: ["mae"]
+    pcqm4m_g25: []
+  metrics_on_training_set:
+    pcqm4m_g25: []
   loss_fun:
-    qm9: mae_ipu
-    tox21: bce_ipu
-    zinc: mae_ipu
+    pcqm4m_g25: mae_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 4.e-5 # warmup can be scheduled using torch_scheduler_kwargs
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
-    max_num_epochs: &max_epochs 100
+    max_num_epochs: &max_epochs 20
     warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
-  qm9: &qm9_metrics
+  pcqm4m_g25: &pcqm_metrics
     - name: mae
       metric: mae_ipu
       target_nan_mask: null
       multitask_handling: flatten
       threshold_kwargs: null
     - name: pearsonr
       metric: pearsonr_ipu
       threshold_kwargs: null
       target_nan_mask: null
       multitask_handling: mean-per-label
-  tox21:
-    - name: auroc_flat
-      metric: auroc_ipu
-      multitask_handling: flatten
+    - name: r2
+      metric: r2_score_ipu
       threshold_kwargs: null
-    - name: avpr_flat
-      metric: averageprecision
-      multitask_handling: flatten
-      threshold_kwargs: null
-    - name: f1 > 0.5
-      metric: f1
-      multitask_handling: flatten
-      target_to_int: True
-      num_classes: 2
-      average: micro
-      threshold_kwargs: &threshold_05
-        operator: greater
-        threshold: 0.5
-        th_on_preds: True
-        th_on_target: True
-    - name: precision > 0.5
-      metric: precision
-      multitask_handling: flatten
-      average: micro
-      threshold_kwargs: *threshold_05
-  zinc: *qm9_metrics
+      target_nan_mask: null
+      multitask_handling: mean-per-label
 
 trainer:
+  seed: *seed
   logger:
-    save_dir: logs/neurips2023-small/
+    save_dir: logs/neurips2023-large/
     name: *name
     project: *name
   #early_stopping:
   #  monitor: *monitor
   #  min_delta: 0
   #  patience: 10
   #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/neurips2023-small/
+    dirpath: models_checkpoints/neurips2023-large-gine/g25/
     filename: *name
-    #monitor: *monitor
-    #mode: *mode
-    save_top_k: 1
-    every_n_epochs: 100
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
     check_val_every_n_epoch: 20
```

### Comparing `graphium-2.0.2/expts/test_yaml.py` & `graphium-2.1.0/expts/test_yaml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/cli/data.py` & `graphium-2.1.0/graphium/cli/data.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/config/_loader.py` & `graphium-2.1.0/graphium/config/_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,60 +11,48 @@
 import warnings
 
 # Torch
 import torch
 import mup
 
 # Lightning
-from pytorch_lightning.callbacks import EarlyStopping, ModelCheckpoint
-from pytorch_lightning import Trainer
-from pytorch_lightning.loggers import WandbLogger, Logger
+from lightning import Trainer
+from lightning.pytorch.callbacks import EarlyStopping, ModelCheckpoint
+from lightning.pytorch.loggers import WandbLogger, Logger
 
 # Graphium
 from graphium.utils.mup import set_base_shapes
 from graphium.ipu.ipu_dataloader import IPUDataloaderOptions
 from graphium.trainer.metrics import MetricWrapper
 from graphium.nn.architectures import FullGraphMultiTaskNetwork
 from graphium.nn.utils import MupMixin
 from graphium.trainer.predictor import PredictorModule
 from graphium.utils.spaces import DATAMODULE_DICT
 from graphium.ipu.ipu_utils import import_poptorch, load_ipu_options
 from graphium.data.datamodule import MultitaskFromSmilesDataModule, BaseDataModule
-
-# Weights and Biases
-from pytorch_lightning import Trainer
+from graphium.utils.command_line_utils import update_config, get_anchors_and_aliases
 
 
 def get_accelerator(
     config_acc: Union[omegaconf.DictConfig, Dict[str, Any]],
 ) -> str:
     """
     Get the accelerator from the config file, and ensure that they are
-    consistant. For example, specifying `cpu` as the accelerators, but
-    `gpus>0` as a Trainer option will yield an error.
+    consistant.
     """
 
     # Get the accelerator type
     accelerator_type = config_acc["type"]
 
     # Get the GPU info
-    gpus = config_acc["config_override"].get("trainer", {}).get("trainer", {}).get("gpus", 0)
-    if gpus > 0:
-        assert (accelerator_type is None) or (accelerator_type == "gpu"), "Accelerator mismatch"
-        accelerator_type = "gpu"
-
     if (accelerator_type == "gpu") and (not torch.cuda.is_available()):
         logger.warning(f"GPUs selected, but will be ignored since no GPU are available on this device")
         accelerator_type = "cpu"
 
     # Get the IPU info
-    ipus = config_acc["config_override"].get("trainer", {}).get("trainer", {}).get("ipus", 0)
-    if ipus > 0:
-        assert (accelerator_type is None) or (accelerator_type == "ipu"), "Accelerator mismatch"
-        accelerator_type = "ipu"
     if accelerator_type == "ipu":
         poptorch = import_poptorch()
         if not poptorch.ipuHardwareIsAvailable():
             logger.warning(f"IPUs selected, but will be ignored since no IPU are available on this device")
             accelerator_type = "cpu"
 
     # Fall on cpu at the end
@@ -275,15 +263,15 @@
     model_class: Type[torch.nn.Module],
     model_kwargs: Dict[str, Any],
     metrics: Dict[str, MetricWrapper],
     accelerator_type: str,
     task_norms: Optional[Dict[Callable, Any]] = None,
 ) -> PredictorModule:
     """
-    Defining the predictor module, which handles the training logic from `pytorch_lightning.LighningModule`
+    Defining the predictor module, which handles the training logic from `lightning.LighningModule`
     Parameters:
         model_class: The torch Module containing the main forward function
         accelerator_type: The accelerator type, e.g. "cpu", "gpu", "ipu"
     Returns:
         predictor: The predictor module
     """
 
@@ -360,77 +348,67 @@
         date_time_suffix: The date and time of the current run. To be used for logging.
     Returns:
         trainer: the trainer module
     """
     cfg_trainer = deepcopy(config["trainer"])
 
     # Define the IPU plugin if required
-    strategy = None
+    strategy = "auto"
     if accelerator_type == "ipu":
         ipu_opts, ipu_inference_opts = _get_ipu_opts(config)
 
         training_opts, inference_opts = load_ipu_options(
             ipu_opts=ipu_opts,
             ipu_inference_opts=ipu_inference_opts,
             seed=config["constants"]["seed"],
             model_name=config["constants"]["name"],
             gradient_accumulation=config["trainer"]["trainer"].get("accumulate_grad_batches", None),
         )
 
-        from graphium.ipu.ipu_wrapper import DictIPUStrategy
+        from lightning_graphcore import IPUStrategy
 
-        strategy = DictIPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
+        strategy = IPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
 
-    # Set the number of gpus to 0 if no GPU is available
-    _ = cfg_trainer["trainer"].pop("accelerator", None)
-    gpus = cfg_trainer["trainer"].pop("gpus", None)
-    ipus = cfg_trainer["trainer"].pop("ipus", None)
-    if (accelerator_type == "gpu") and (gpus is None):
-        gpus = 1
-    if (accelerator_type == "ipu") and (ipus is None):
-        ipus = 1
-    if accelerator_type != "gpu":
-        gpus = 0
-    if accelerator_type != "ipu":
-        ipus = 0
+    # Get devices
+    devices = cfg_trainer["trainer"].pop("devices", 1)
+    if accelerator_type == "ipu":
+        devices = 1  # number of IPUs used is defined in the ipu options files
 
     # Remove the gradient accumulation from IPUs, since it's handled by the device
     if accelerator_type == "ipu":
         cfg_trainer["trainer"].pop("accumulate_grad_batches", None)
 
     # Define the early stopping parameters
     trainer_kwargs = {}
     callbacks = []
     if "early_stopping" in cfg_trainer.keys():
         callbacks.append(EarlyStopping(**cfg_trainer["early_stopping"]))
 
     # Define the early model checkpoing parameters
     if "model_checkpoint" in cfg_trainer.keys():
+        cfg_trainer["model_checkpoint"]["dirpath"] += str(cfg_trainer["seed"]) + "/"
         callbacks.append(ModelCheckpoint(**cfg_trainer["model_checkpoint"]))
 
     # Define the logger parameters
     logger = cfg_trainer.pop("logger", None)
     if logger is not None:
         name = logger.pop("name", run_name)
         if len(date_time_suffix) > 0:
             name += f"_{date_time_suffix}"
         trainer_kwargs["logger"] = WandbLogger(name=name, **logger)
 
     trainer_kwargs["callbacks"] = callbacks
-
     trainer = Trainer(
         detect_anomaly=True,
         strategy=strategy,
         accelerator=accelerator_type,
-        ipus=ipus,
-        gpus=gpus,
+        devices=devices,
         **cfg_trainer["trainer"],
         **trainer_kwargs,
     )
-
     return trainer
 
 
 def save_params_to_wandb(
     logger: Logger,
     config: Union[omegaconf.DictConfig, Dict[str, Any]],
     predictor: PredictorModule,
@@ -476,37 +454,99 @@
     config_override = config_acc.get("config_override", {})
     merge_dicts(config, config_override)
     accelerator_type = get_accelerator(config_acc)
 
     return config, accelerator_type
 
 
-def merge_dicts(dict_a: Dict[str, Any], dict_b: Dict[str, Any], previous_dict_path: str = "") -> None:
+def load_config_override(
+    config: Union[omegaconf.DictConfig, Dict[str, Any]], main_dir: Optional[Union[str, os.PathLike]] = None
+) -> Dict[str, Any]:
+    config = deepcopy(config)
+    config_override_path = config["constants"].get("config_override", None)
+    if config_override_path is not None:
+        if main_dir is not None:
+            config_override_path = os.path.join(main_dir, config_override_path)
+        with open(config_override_path, "r") as f:
+            cfg_override = yaml.safe_load(f)
+        config = merge_dicts(cfg_override, config, on_exist="overwrite")
+    return config
+
+
+def load_yaml_config(
+    config_path: Union[str, os.PathLike],
+    main_dir: Optional[Union[str, os.PathLike]] = None,
+    unknown_args=None,
+) -> Dict[str, Any]:
+    """
+    Load a YAML config file and return it as a dictionary.
+    Also returns the anchors `&` and aliases `*` of the YAML file.
+    Then, update the config with the unknown arguments.
+    Finally, update the config with the config override file specified in `constants.config_override`.
+
+    Parameters:
+        config_path: The path to the YAML config file
+        main_dir: The main directory of the project. If specified, the config override file will be loaded from this directory
+        unknown_args: The unknown arguments to update the config with, taken from `argparse.parse_known_args`
+
+    Returns:
+        config: The config dictionary
+
+    """
+    if main_dir is not None:
+        config_path = os.path.join(main_dir, config_path)
+
+    with open(config_path, "r") as f:
+        config = yaml.safe_load(f)
+        refs = get_anchors_and_aliases(config_path)
+        if unknown_args is not None:
+            config = update_config(config, unknown_args, refs)
+    config = load_config_override(config, main_dir)  # This goes here to avoid overriding the hparam search
+
+    return config
+
+
+def merge_dicts(
+    dict_a: Dict[str, Any], dict_b: Dict[str, Any], previous_dict_path: str = "", on_exist: str = "raise"
+) -> None:
     """
     Recursively merges dict_b into dict_a. If a key is missing from dict_a,
     it is added from dict_b. If a key exists in both, an error is raised.
     `dict_a` is modified in-place.
 
     Parameters:
         dict_a: The dictionary to merge into. Modified in-place.
         dict_b: The dictionary to merge from.
         previous_dict_path: The key path of the parent dictionary,
         used to track the recursive calls.
+        on_exist: What to do if a key already exists in dict_a. Options are "raise", "overwrite", "ignore".
 
     Raises:
         ValueError: If a key path already exists in dict_a.
 
     """
+    assert on_exist in [
+        "raise",
+        "overwrite",
+        "ignore",
+    ], f"on_exist must be one of ['raise', 'overwrite', 'ignore'], got {on_exist}"
+
     for key, value_b in dict_b.items():
         if key not in dict_a:
             dict_a[key] = value_b
         else:
             value_a = dict_a[key]
             if previous_dict_path == "":
                 previous_dict_path = key
             else:
                 previous_dict_path = f"{previous_dict_path}/{key}"
             if isinstance(value_a, dict) and isinstance(value_b, dict):
-                merge_dicts(value_a, value_b, previous_dict_path=previous_dict_path)
+                merge_dicts(value_a, value_b, previous_dict_path=previous_dict_path, on_exist=on_exist)
             else:
                 if value_a != value_b:
-                    raise ValueError(f"Dict path already exists: {previous_dict_path}")
+                    if on_exist == "raise":
+                        raise ValueError(f"Dict path already exists: {previous_dict_path}")
+                    elif on_exist == "overwrite":
+                        dict_a[key] = value_b
+                    elif on_exist == "ignore":
+                        pass
+    return dict_a
```

### Comparing `graphium-2.0.2/graphium/config/config_convert.py` & `graphium-2.1.0/graphium/config/config_convert.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml` & `graphium-2.1.0/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/config/fake_multilevel_multitask_pyg.yaml` & `graphium-2.1.0/graphium/config/fake_multilevel_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/config/zinc_default_multitask_pyg.yaml` & `graphium-2.1.0/graphium/config/zinc_default_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb` & `graphium-2.1.0/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/QM9/micro_qm9.csv` & `graphium-2.1.0/graphium/data/QM9/micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/QM9/micro_qm9.parquet` & `graphium-2.1.0/graphium/data/QM9/micro_qm9.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -11458,15 +11458,15 @@
 0002cc10: 0006 1918 0967 3239 385f 6174 6f6d 1502  .....g298_atom..
 0002cc20: 16dc 0f16 ee92 0116 8293 0126 a0f6 1526  ...........&...&
 0002cc30: 94f8 141c 1808 74c4 d38b 072d 69c0 1808  ......t....-i...
 0002cc40: f1fb 54e0 c2e2 a1c0 1600 2808 74c4 d38b  ..T.......(.t...
 0002cc50: 072d 69c0 1808 f1fb 54e0 c2e2 a1c0 0019  .-i.....T.......
 0002cc60: 2c15 0415 0015 0200 1500 1510 1502 0000  ,...............
 0002cc70: 0016 a0fd 1816 dc0f 2608 1692 ec15 1400  ........&.......
-0002cc80: 0019 2c18 0670 616e 6461 7318 be14 7b22  ..,..pandas...{"
+0002cc80: 0019 2c18 0670 616e 6461 7318 bf14 7b22  ..,..pandas...{"
 0002cc90: 696e 6465 785f 636f 6c75 6d6e 7322 3a20  index_columns": 
 0002cca0: 5b7b 226b 696e 6422 3a20 2272 616e 6765  [{"kind": "range
 0002ccb0: 222c 2022 6e61 6d65 223a 206e 756c 6c2c  ", "name": null,
 0002ccc0: 2022 7374 6172 7422 3a20 302c 2022 7374   "start": 0, "st
 0002ccd0: 6f70 223a 2031 3030 362c 2022 7374 6570  op": 1006, "step
 0002cce0: 223a 2031 7d5d 2c20 2263 6f6c 756d 6e5f  ": 1}], "column_
 0002ccf0: 696e 6465 7865 7322 3a20 5b7b 226e 616d  indexes": [{"nam
@@ -11620,330 +11620,330 @@
 0002d630: 6d22 2c20 2270 616e 6461 735f 7479 7065  m", "pandas_type
 0002d640: 223a 2022 666c 6f61 7436 3422 2c20 226e  ": "float64", "n
 0002d650: 756d 7079 5f74 7970 6522 3a20 2266 6c6f  umpy_type": "flo
 0002d660: 6174 3634 222c 2022 6d65 7461 6461 7461  at64", "metadata
 0002d670: 223a 206e 756c 6c7d 5d2c 2022 6372 6561  ": null}], "crea
 0002d680: 746f 7222 3a20 7b22 6c69 6272 6172 7922  tor": {"library"
 0002d690: 3a20 2270 7961 7272 6f77 222c 2022 7665  : "pyarrow", "ve
-0002d6a0: 7273 696f 6e22 3a20 2239 2e30 2e30 227d  rsion": "9.0.0"}
-0002d6b0: 2c20 2270 616e 6461 735f 7665 7273 696f  , "pandas_versio
-0002d6c0: 6e22 3a20 2231 2e34 2e33 227d 0018 0c41  n": "1.4.3"}...A
-0002d6d0: 5252 4f57 3a73 6368 656d 6118 f826 2f2f  RROW:schema..&//
-0002d6e0: 2f2f 2f35 414f 4141 4151 4141 4141 4141  ///5AOAAAQAAAAAA
-0002d6f0: 414b 4141 3441 4267 4146 4141 6741 4367  AKAA4ABgAFAAgACg
-0002d700: 4141 4141 4142 4241 4151 4141 4141 4141  AAAAABBAAQAAAAAA
-0002d710: 414b 4141 7741 4141 4145 4141 6741 4367  AKAAwAAAAEAAgACg
-0002d720: 4141 4148 514b 4141 4145 4141 4141 4151  AAAHQKAAAEAAAAAQ
-0002d730: 4141 4141 7741 4141 4149 4141 7741 4241  AAAAwAAAAIAAwABA
-0002d740: 4149 4141 6741 4141 4149 4141 4141 4541  AIAAgAAAAIAAAAEA
-0002d750: 4141 4141 5941 4141 4277 5957 356b 5958  AAAAYAAABwYW5kYX
-0002d760: 4d41 4144 344b 4141 4237 496d 6c75 5a47  MAAD4KAAB7ImluZG
-0002d770: 5634 5832 4e76 6248 5674 626e 4d69 4f69  V4X2NvbHVtbnMiOi
-0002d780: 4262 6579 4a72 6157 356b 496a 6f67 496e  BbeyJraW5kIjogIn
-0002d790: 4a68 626d 646c 4969 7767 496d 3568 6257  JhbmdlIiwgIm5hbW
-0002d7a0: 5569 4f69 4275 6457 7873 4c43 4169 6333  UiOiBudWxsLCAic3
-0002d7b0: 5268 636e 5169 4f69 4177 4c43 4169 6333  RhcnQiOiAwLCAic3
-0002d7c0: 5276 6343 4936 4944 4577 4d44 5973 4943  RvcCI6IDEwMDYsIC
-0002d7d0: 4a7a 6447 5677 496a 6f67 4d58 3164 4c43  JzdGVwIjogMX1dLC
-0002d7e0: 4169 5932 3973 6457 3175 5832 6c75 5a47  AiY29sdW1uX2luZG
-0002d7f0: 5634 5a58 4d69 4f69 4262 6579 4a75 5957  V4ZXMiOiBbeyJuYW
-0002d800: 316c 496a 6f67 626e 5673 6243 7767 496d  1lIjogbnVsbCwgIm
-0002d810: 5a70 5a57 786b 5832 3568 6257 5569 4f69  ZpZWxkX25hbWUiOi
-0002d820: 4275 6457 7873 4c43 4169 6347 4675 5a47  BudWxsLCAicGFuZG
-0002d830: 467a 5833 5235 6347 5569 4f69 4169 6457  FzX3R5cGUiOiAidW
-0002d840: 3570 5932 396b 5a53 4973 4943 4a75 6457  5pY29kZSIsICJudW
-0002d850: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-0002d860: 3969 616d 566a 6443 4973 4943 4a74 5a58  9iamVjdCIsICJtZX
-0002d870: 5268 5a47 4630 5953 4936 4948 7369 5a57  RhZGF0YSI6IHsiZW
-0002d880: 356a 6232 5270 626d 6369 4f69 4169 5656  5jb2RpbmciOiAiVV
-0002d890: 5247 4c54 6769 6658 3164 4c43 4169 5932  RGLTgifX1dLCAiY2
-0002d8a0: 3973 6457 3175 6379 4936 4946 7437 496d  9sdW1ucyI6IFt7Im
-0002d8b0: 3568 6257 5569 4f69 4169 6257 3973 5832  5hbWUiOiAibW9sX2
-0002d8c0: 6c6b 4969 7767 496d 5a70 5a57 786b 5832  lkIiwgImZpZWxkX2
-0002d8d0: 3568 6257 5569 4f69 4169 6257 3973 5832  5hbWUiOiAibW9sX2
-0002d8e0: 6c6b 4969 7767 496e 4268 626d 5268 6331  lkIiwgInBhbmRhc1
-0002d8f0: 3930 6558 426c 496a 6f67 496e 5675 6157  90eXBlIjogInVuaW
-0002d900: 4e76 5a47 5569 4c43 4169 626e 5674 6348  NvZGUiLCAibnVtcH
-0002d910: 6c66 6448 6c77 5a53 4936 4943 4a76 596d  lfdHlwZSI6ICJvYm
-0002d920: 706c 5933 5169 4c43 4169 6257 5630 5957  plY3QiLCAibWV0YW
-0002d930: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
-0002d940: 7767 6579 4a75 5957 316c 496a 6f67 496e  wgeyJuYW1lIjogIn
-0002d950: 4e74 6157 786c 6379 4973 4943 4a6d 6157  NtaWxlcyIsICJmaW
-0002d960: 5673 5a46 3975 5957 316c 496a 6f67 496e  VsZF9uYW1lIjogIn
-0002d970: 4e74 6157 786c 6379 4973 4943 4a77 5957  NtaWxlcyIsICJwYW
-0002d980: 356b 5958 4e66 6448 6c77 5a53 4936 4943  5kYXNfdHlwZSI6IC
-0002d990: 4a31 626d 6c6a 6232 526c 4969 7767 496d  J1bmljb2RlIiwgIm
-0002d9a0: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
-0002d9b0: 4169 6232 4a71 5a57 4e30 4969 7767 496d  Aib2JqZWN0IiwgIm
-0002d9c0: 316c 6447 466b 5958 5268 496a 6f67 626e  1ldGFkYXRhIjogbn
-0002d9d0: 5673 6248 3073 4948 7369 626d 4674 5a53  VsbH0sIHsibmFtZS
-0002d9e0: 4936 4943 4a42 4969 7767 496d 5a70 5a57  I6ICJBIiwgImZpZW
-0002d9f0: 786b 5832 3568 6257 5569 4f69 4169 5153  xkX25hbWUiOiAiQS
-0002da00: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
-0002da10: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
-0002da20: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-0002da30: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
-0002da40: 5132 4e43 4973 4943 4a74 5a58 5268 5a47  Q2NCIsICJtZXRhZG
-0002da50: 4630 5953 4936 4947 3531 6247 7839 4c43  F0YSI6IG51bGx9LC
-0002da60: 4237 496d 3568 6257 5569 4f69 4169 5169  B7Im5hbWUiOiAiQi
-0002da70: 4973 4943 4a6d 6157 5673 5a46 3975 5957  IsICJmaWVsZF9uYW
-0002da80: 316c 496a 6f67 496b 4969 4c43 4169 6347  1lIjogIkIiLCAicG
-0002da90: 4675 5a47 467a 5833 5235 6347 5569 4f69  FuZGFzX3R5cGUiOi
-0002daa0: 4169 5a6d 7876 5958 5132 4e43 4973 4943  AiZmxvYXQ2NCIsIC
-0002dab0: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
-0002dac0: 6f67 496d 5a73 6232 4630 4e6a 5169 4c43  ogImZsb2F0NjQiLC
-0002dad0: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
-0002dae0: 4275 6457 7873 6653 7767 6579 4a75 5957  BudWxsfSwgeyJuYW
-0002daf0: 316c 496a 6f67 496b 4d69 4c43 4169 5a6d  1lIjogIkMiLCAiZm
-0002db00: 6c6c 6247 5266 626d 4674 5a53 4936 4943  llbGRfbmFtZSI6IC
-0002db10: 4a44 4969 7767 496e 4268 626d 5268 6331  JDIiwgInBhbmRhc1
-0002db20: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
-0002db30: 4630 4e6a 5169 4c43 4169 626e 5674 6348  F0NjQiLCAibnVtcH
-0002db40: 6c66 6448 6c77 5a53 4936 4943 4a6d 6247  lfdHlwZSI6ICJmbG
-0002db50: 3968 6444 5930 4969 7767 496d 316c 6447  9hdDY0IiwgIm1ldG
-0002db60: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-0002db70: 3073 4948 7369 626d 4674 5a53 4936 4943  0sIHsibmFtZSI6IC
-0002db80: 4a74 6453 4973 4943 4a6d 6157 5673 5a46  JtdSIsICJmaWVsZF
-0002db90: 3975 5957 316c 496a 6f67 496d 3131 4969  9uYW1lIjogIm11Ii
-0002dba0: 7767 496e 4268 626d 5268 6331 3930 6558  wgInBhbmRhc190eX
-0002dbb0: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
-0002dbc0: 5169 4c43 4169 626e 5674 6348 6c66 6448  QiLCAibnVtcHlfdH
-0002dbd0: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
-0002dbe0: 5930 4969 7767 496d 316c 6447 466b 5958  Y0IiwgIm1ldGFkYX
-0002dbf0: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
-0002dc00: 7369 626d 4674 5a53 4936 4943 4a68 6248  sibmFtZSI6ICJhbH
-0002dc10: 426f 5953 4973 4943 4a6d 6157 5673 5a46  BoYSIsICJmaWVsZF
-0002dc20: 3975 5957 316c 496a 6f67 496d 4673 6347  9uYW1lIjogImFscG
-0002dc30: 6868 4969 7767 496e 4268 626d 5268 6331  hhIiwgInBhbmRhc1
-0002dc40: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
-0002dc50: 4630 4e6a 5169 4c43 4169 626e 5674 6348  F0NjQiLCAibnVtcH
-0002dc60: 6c66 6448 6c77 5a53 4936 4943 4a6d 6247  lfdHlwZSI6ICJmbG
-0002dc70: 3968 6444 5930 4969 7767 496d 316c 6447  9hdDY0IiwgIm1ldG
-0002dc80: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-0002dc90: 3073 4948 7369 626d 4674 5a53 4936 4943  0sIHsibmFtZSI6IC
-0002dca0: 4a6f 6232 3176 4969 7767 496d 5a70 5a57  Job21vIiwgImZpZW
-0002dcb0: 786b 5832 3568 6257 5569 4f69 4169 6147  xkX25hbWUiOiAiaG
-0002dcc0: 3974 6279 4973 4943 4a77 5957 356b 5958  9tbyIsICJwYW5kYX
-0002dcd0: 4e66 6448 6c77 5a53 4936 4943 4a6d 6247  NfdHlwZSI6ICJmbG
-0002dce0: 3968 6444 5930 4969 7767 496d 3531 6258  9hdDY0IiwgIm51bX
-0002dcf0: 4235 5833 5235 6347 5569 4f69 4169 5a6d  B5X3R5cGUiOiAiZm
-0002dd00: 7876 5958 5132 4e43 4973 4943 4a74 5a58  xvYXQ2NCIsICJtZX
-0002dd10: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
-0002dd20: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
-0002dd30: 4169 6248 5674 6279 4973 4943 4a6d 6157  AibHVtbyIsICJmaW
-0002dd40: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
-0002dd50: 7831 6257 3869 4c43 4169 6347 4675 5a47  x1bW8iLCAicGFuZG
-0002dd60: 467a 5833 5235 6347 5569 4f69 4169 5a6d  FzX3R5cGUiOiAiZm
-0002dd70: 7876 5958 5132 4e43 4973 4943 4a75 6457  xvYXQ2NCIsICJudW
-0002dd80: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-0002dd90: 5a73 6232 4630 4e6a 5169 4c43 4169 6257  Zsb2F0NjQiLCAibW
-0002dda0: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
-0002ddb0: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
-0002ddc0: 6f67 496d 6468 6343 4973 4943 4a6d 6157  ogImdhcCIsICJmaW
-0002ddd0: 5673 5a46 3975 5957 316c 496a 6f67 496d  VsZF9uYW1lIjogIm
-0002dde0: 6468 6343 4973 4943 4a77 5957 356b 5958  dhcCIsICJwYW5kYX
-0002ddf0: 4e66 6448 6c77 5a53 4936 4943 4a6d 6247  NfdHlwZSI6ICJmbG
-0002de00: 3968 6444 5930 4969 7767 496d 3531 6258  9hdDY0IiwgIm51bX
-0002de10: 4235 5833 5235 6347 5569 4f69 4169 5a6d  B5X3R5cGUiOiAiZm
-0002de20: 7876 5958 5132 4e43 4973 4943 4a74 5a58  xvYXQ2NCIsICJtZX
-0002de30: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
-0002de40: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
-0002de50: 4169 636a 4969 4c43 4169 5a6d 6c6c 6247  AicjIiLCAiZmllbG
-0002de60: 5266 626d 4674 5a53 4936 4943 4a79 4d69  RfbmFtZSI6ICJyMi
-0002de70: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
-0002de80: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
-0002de90: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-0002dea0: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
-0002deb0: 5132 4e43 4973 4943 4a74 5a58 5268 5a47  Q2NCIsICJtZXRhZG
-0002dec0: 4630 5953 4936 4947 3531 6247 7839 4c43  F0YSI6IG51bGx9LC
-0002ded0: 4237 496d 3568 6257 5569 4f69 4169 656e  B7Im5hbWUiOiAien
-0002dee0: 4232 5a53 4973 4943 4a6d 6157 5673 5a46  B2ZSIsICJmaWVsZF
-0002def0: 3975 5957 316c 496a 6f67 496e 7077 646d  9uYW1lIjogInpwdm
-0002df00: 5569 4c43 4169 6347 4675 5a47 467a 5833  UiLCAicGFuZGFzX3
-0002df10: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
-0002df20: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
-0002df30: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
-0002df40: 4630 4e6a 5169 4c43 4169 6257 5630 5957  F0NjQiLCAibWV0YW
-0002df50: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
-0002df60: 7767 6579 4a75 5957 316c 496a 6f67 496e  wgeyJuYW1lIjogIn
-0002df70: 5577 4969 7767 496d 5a70 5a57 786b 5832  UwIiwgImZpZWxkX2
-0002df80: 3568 6257 5569 4f69 4169 6454 4169 4c43  5hbWUiOiAidTAiLC
-0002df90: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-0002dfa0: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
-0002dfb0: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
-0002dfc0: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
-0002dfd0: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-0002dfe0: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-0002dff0: 4a75 5957 316c 496a 6f67 496e 5579 4f54  JuYW1lIjogInUyOT
-0002e000: 6769 4c43 4169 5a6d 6c6c 6247 5266 626d  giLCAiZmllbGRfbm
-0002e010: 4674 5a53 4936 4943 4a31 4d6a 6b34 4969  FtZSI6ICJ1Mjk4Ii
-0002e020: 7767 496e 4268 626d 5268 6331 3930 6558  wgInBhbmRhc190eX
-0002e030: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
-0002e040: 5169 4c43 4169 626e 5674 6348 6c66 6448  QiLCAibnVtcHlfdH
-0002e050: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
-0002e060: 5930 4969 7767 496d 316c 6447 466b 5958  Y0IiwgIm1ldGFkYX
-0002e070: 5268 496a 6f67 626e 5673 6248 3073 4948  RhIjogbnVsbH0sIH
-0002e080: 7369 626d 4674 5a53 4936 4943 4a6f 4d6a  sibmFtZSI6ICJoMj
-0002e090: 6b34 4969 7767 496d 5a70 5a57 786b 5832  k4IiwgImZpZWxkX2
-0002e0a0: 3568 6257 5569 4f69 4169 6144 4935 4f43  5hbWUiOiAiaDI5OC
-0002e0b0: 4973 4943 4a77 5957 356b 5958 4e66 6448  IsICJwYW5kYXNfdH
-0002e0c0: 6c77 5a53 4936 4943 4a6d 6247 3968 6444  lwZSI6ICJmbG9hdD
-0002e0d0: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
-0002e0e0: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
-0002e0f0: 5132 4e43 4973 4943 4a74 5a58 5268 5a47  Q2NCIsICJtZXRhZG
-0002e100: 4630 5953 4936 4947 3531 6247 7839 4c43  F0YSI6IG51bGx9LC
-0002e110: 4237 496d 3568 6257 5569 4f69 4169 5a7a  B7Im5hbWUiOiAiZz
-0002e120: 4935 4f43 4973 4943 4a6d 6157 5673 5a46  I5OCIsICJmaWVsZF
-0002e130: 3975 5957 316c 496a 6f67 496d 6379 4f54  9uYW1lIjogImcyOT
-0002e140: 6769 4c43 4169 6347 4675 5a47 467a 5833  giLCAicGFuZGFzX3
-0002e150: 5235 6347 5569 4f69 4169 5a6d 7876 5958  R5cGUiOiAiZmxvYX
-0002e160: 5132 4e43 4973 4943 4a75 6457 3177 6556  Q2NCIsICJudW1weV
-0002e170: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
-0002e180: 4630 4e6a 5169 4c43 4169 6257 5630 5957  F0NjQiLCAibWV0YW
-0002e190: 5268 6447 4569 4f69 4275 6457 7873 6653  RhdGEiOiBudWxsfS
-0002e1a0: 7767 6579 4a75 5957 316c 496a 6f67 496d  wgeyJuYW1lIjogIm
-0002e1b0: 4e32 4969 7767 496d 5a70 5a57 786b 5832  N2IiwgImZpZWxkX2
-0002e1c0: 3568 6257 5569 4f69 4169 5933 5969 4c43  5hbWUiOiAiY3YiLC
-0002e1d0: 4169 6347 4675 5a47 467a 5833 5235 6347  AicGFuZGFzX3R5cG
-0002e1e0: 5569 4f69 4169 5a6d 7876 5958 5132 4e43  UiOiAiZmxvYXQ2NC
-0002e1f0: 4973 4943 4a75 6457 3177 6556 3930 6558  IsICJudW1weV90eX
-0002e200: 426c 496a 6f67 496d 5a73 6232 4630 4e6a  BlIjogImZsb2F0Nj
-0002e210: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
-0002e220: 4569 4f69 4275 6457 7873 6653 7767 6579  EiOiBudWxsfSwgey
-0002e230: 4a75 5957 316c 496a 6f67 496e 5577 5832  JuYW1lIjogInUwX2
-0002e240: 4630 6232 3069 4c43 4169 5a6d 6c6c 6247  F0b20iLCAiZmllbG
-0002e250: 5266 626d 4674 5a53 4936 4943 4a31 4d46  RfbmFtZSI6ICJ1MF
-0002e260: 3968 6447 3974 4969 7767 496e 4268 626d  9hdG9tIiwgInBhbm
-0002e270: 5268 6331 3930 6558 426c 496a 6f67 496d  Rhc190eXBlIjogIm
-0002e280: 5a73 6232 4630 4e6a 5169 4c43 4169 626e  Zsb2F0NjQiLCAibn
-0002e290: 5674 6348 6c66 6448 6c77 5a53 4936 4943  VtcHlfdHlwZSI6IC
-0002e2a0: 4a6d 6247 3968 6444 5930 4969 7767 496d  JmbG9hdDY0IiwgIm
-0002e2b0: 316c 6447 466b 5958 5268 496a 6f67 626e  1ldGFkYXRhIjogbn
-0002e2c0: 5673 6248 3073 4948 7369 626d 4674 5a53  VsbH0sIHsibmFtZS
-0002e2d0: 4936 4943 4a31 4d6a 6b34 5832 4630 6232  I6ICJ1Mjk4X2F0b2
-0002e2e0: 3069 4c43 4169 5a6d 6c6c 6247 5266 626d  0iLCAiZmllbGRfbm
-0002e2f0: 4674 5a53 4936 4943 4a31 4d6a 6b34 5832  FtZSI6ICJ1Mjk4X2
-0002e300: 4630 6232 3069 4c43 4169 6347 4675 5a47  F0b20iLCAicGFuZG
-0002e310: 467a 5833 5235 6347 5569 4f69 4169 5a6d  FzX3R5cGUiOiAiZm
-0002e320: 7876 5958 5132 4e43 4973 4943 4a75 6457  xvYXQ2NCIsICJudW
-0002e330: 3177 6556 3930 6558 426c 496a 6f67 496d  1weV90eXBlIjogIm
-0002e340: 5a73 6232 4630 4e6a 5169 4c43 4169 6257  Zsb2F0NjQiLCAibW
-0002e350: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
-0002e360: 7873 6653 7767 6579 4a75 5957 316c 496a  xsfSwgeyJuYW1lIj
-0002e370: 6f67 496d 6779 4f54 6866 5958 5276 6253  ogImgyOThfYXRvbS
-0002e380: 4973 4943 4a6d 6157 5673 5a46 3975 5957  IsICJmaWVsZF9uYW
-0002e390: 316c 496a 6f67 496d 6779 4f54 6866 5958  1lIjogImgyOThfYX
-0002e3a0: 5276 6253 4973 4943 4a77 5957 356b 5958  RvbSIsICJwYW5kYX
-0002e3b0: 4e66 6448 6c77 5a53 4936 4943 4a6d 6247  NfdHlwZSI6ICJmbG
-0002e3c0: 3968 6444 5930 4969 7767 496d 3531 6258  9hdDY0IiwgIm51bX
-0002e3d0: 4235 5833 5235 6347 5569 4f69 4169 5a6d  B5X3R5cGUiOiAiZm
-0002e3e0: 7876 5958 5132 4e43 4973 4943 4a74 5a58  xvYXQ2NCIsICJtZX
-0002e3f0: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
-0002e400: 7839 4c43 4237 496d 3568 6257 5569 4f69  x9LCB7Im5hbWUiOi
-0002e410: 4169 5a7a 4935 4f46 3968 6447 3974 4969  AiZzI5OF9hdG9tIi
-0002e420: 7767 496d 5a70 5a57 786b 5832 3568 6257  wgImZpZWxkX25hbW
-0002e430: 5569 4f69 4169 5a7a 4935 4f46 3968 6447  UiOiAiZzI5OF9hdG
-0002e440: 3974 4969 7767 496e 4268 626d 5268 6331  9tIiwgInBhbmRhc1
-0002e450: 3930 6558 426c 496a 6f67 496d 5a73 6232  90eXBlIjogImZsb2
-0002e460: 4630 4e6a 5169 4c43 4169 626e 5674 6348  F0NjQiLCAibnVtcH
-0002e470: 6c66 6448 6c77 5a53 4936 4943 4a6d 6247  lfdHlwZSI6ICJmbG
-0002e480: 3968 6444 5930 4969 7767 496d 316c 6447  9hdDY0IiwgIm1ldG
-0002e490: 466b 5958 5268 496a 6f67 626e 5673 6248  FkYXRhIjogbnVsbH
-0002e4a0: 3164 4c43 4169 5933 4a6c 5958 5276 6369  1dLCAiY3JlYXRvci
-0002e4b0: 4936 4948 7369 6247 6c69 636d 4679 6553  I6IHsibGlicmFyeS
-0002e4c0: 4936 4943 4a77 6557 4679 636d 3933 4969  I6ICJweWFycm93Ii
-0002e4d0: 7767 496e 5a6c 636e 4e70 6232 3469 4f69  wgInZlcnNpb24iOi
-0002e4e0: 4169 4f53 3477 4c6a 4169 6653 7767 496e  AiOS4wLjAifSwgIn
-0002e4f0: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-0002e500: 3975 496a 6f67 496a 4575 4e43 347a 496e  9uIjogIjEuNC4zIn
-0002e510: 3041 4142 5541 4141 4441 4177 4141 6841  0AABUAAADAAwAAhA
-0002e520: 4d41 4146 5144 4141 416f 4177 4141 2f41  MAAFQDAAAoAwAA/A
-0002e530: 4941 414e 4143 4141 4367 4167 4141 6341  IAANACAACgAgAAcA
-0002e540: 4941 4145 4143 4141 4155 4167 4141 3641  IAAEACAAAUAgAA6A
-0002e550: 4541 414c 6742 4141 434d 4151 4141 5841  EAALgBAACMAQAAXA
-0002e560: 4541 4143 7742 4141 4438 4141 4141 3041  EAACwBAAD8AAAA0A
-0002e570: 4141 414b 4141 4141 4273 4141 4141 4f41  AAAKAAAABsAAAAOA
-0002e580: 4141 4141 5141 4141 436b 2f50 2f2f 4141  AAAAQAAACk/P//AA
-0002e590: 4142 4178 4141 4141 4163 4141 4141 4241  ABAxAAAAAcAAAABA
-0002e5a0: 4141 4141 4141 4141 414a 4141 4141 5a7a  AAAAAAAAAJAAAAZz
-0002e5b0: 4935 4f46 3968 6447 3974 4141 4141 4176  I5OF9hdG9tAAAAAv
-0002e5c0: 332f 2f77 4141 4167 4455 2f50 2f2f 4141  3//wAAAgDU/P//AA
-0002e5d0: 4142 4178 4141 4141 4163 4141 4141 4241  ABAxAAAAAcAAAABA
-0002e5e0: 4141 4141 4141 4141 414a 4141 4141 6144  AAAAAAAAAJAAAAaD
-0002e5f0: 4935 4f46 3968 6447 3974 4141 4141 4d76  I5OF9hdG9tAAAAMv
-0002e600: 332f 2f77 4141 4167 4145 2f66 2f2f 4141  3//wAAAgAE/f//AA
-0002e610: 4142 4178 4141 4141 4163 4141 4141 4241  ABAxAAAAAcAAAABA
-0002e620: 4141 4141 4141 4141 414a 4141 4141 6454  AAAAAAAAAJAAAAdT
-0002e630: 4935 4f46 3968 6447 3974 4141 4141 5976  I5OF9hdG9tAAAAYv
-0002e640: 332f 2f77 4141 4167 4130 2f66 2f2f 4141  3//wAAAgA0/f//AA
-0002e650: 4142 4178 4141 4141 4159 4141 4141 4241  ABAxAAAAAYAAAABA
-0002e660: 4141 4141 4141 4141 4148 4141 4141 6454  AAAAAAAAAHAAAAdT
-0002e670: 4266 5958 5276 6251 434f 2f66 2f2f 4141  BfYXRvbQCO/f//AA
-0002e680: 4143 4147 4439 2f2f 3841 4141 4544 4541  ACAGD9//8AAAEDEA
-0002e690: 4141 4142 5141 4141 4145 4141 4141 4141  AAABQAAAAEAAAAAA
-0002e6a0: 4141 4141 4941 4141 426a 6467 4141 7476  AAAAIAAABjdgAAtv
-0002e6b0: 332f 2f77 4141 4167 4349 2f66 2f2f 4141  3//wAAAgCI/f//AA
-0002e6c0: 4142 4178 4141 4141 4159 4141 4141 4241  ABAxAAAAAYAAAABA
-0002e6d0: 4141 4141 4141 4141 4145 4141 4141 5a7a  AAAAAAAAAEAAAAZz
-0002e6e0: 4935 4f41 4141 4141 4469 2f66 2f2f 4141  I5OAAAAADi/f//AA
-0002e6f0: 4143 414c 5439 2f2f 3841 4141 4544 4541  ACALT9//8AAAEDEA
-0002e700: 4141 4142 6741 4141 4145 4141 4141 4141  AAABgAAAAEAAAAAA
-0002e710: 4141 4141 5141 4141 426f 4d6a 6b34 4141  AAAAQAAABoMjk4AA
-0002e720: 4141 4141 372b 2f2f 3841 4141 4941 3450  AAAA7+//8AAAIA4P
-0002e730: 332f 2f77 4141 4151 4d51 4141 4141 4741  3//wAAAQMQAAAAGA
-0002e740: 4141 4141 5141 4141 4141 4141 4141 4241  AAAAQAAAAAAAAABA
-0002e750: 4141 4148 5579 4f54 6741 4141 4141 4f76  AAAHUyOTgAAAAAOv
-0002e760: 372f 2f77 4141 4167 414d 2f76 2f2f 4141  7//wAAAgAM/v//AA
-0002e770: 4142 4178 4141 4141 4155 4141 4141 4241  ABAxAAAAAUAAAABA
-0002e780: 4141 4141 4141 4141 4143 4141 4141 6454  AAAAAAAAACAAAAdT
-0002e790: 4141 4147 4c2b 2f2f 3841 4141 4941 4e50  AAAGL+//8AAAIANP
-0002e7a0: 372f 2f77 4141 4151 4d51 4141 4141 4741  7//wAAAQMQAAAAGA
-0002e7b0: 4141 4141 5141 4141 4141 4141 4141 4241  AAAAQAAAAAAAAABA
-0002e7c0: 4141 4148 7077 646d 5541 4141 4141 6a76  AAAHpwdmUAAAAAjv
-0002e7d0: 372f 2f77 4141 4167 4267 2f76 2f2f 4141  7//wAAAgBg/v//AA
-0002e7e0: 4142 4178 4141 4141 4155 4141 4141 4241  ABAxAAAAAUAAAABA
-0002e7f0: 4141 4141 4141 4141 4143 4141 4141 636a  AAAAAAAAACAAAAcj
-0002e800: 4941 414c 622b 2f2f 3841 4141 4941 6950  IAALb+//8AAAIAiP
-0002e810: 372f 2f77 4141 4151 4d51 4141 4141 4641  7//wAAAQMQAAAAFA
-0002e820: 4141 4141 5141 4141 4141 4141 4141 4177  AAAAQAAAAAAAAAAw
-0002e830: 4141 4147 6468 6341 4465 2f76 2f2f 4141  AAAGdhcADe/v//AA
-0002e840: 4143 414c 442b 2f2f 3841 4141 4544 4541  ACALD+//8AAAEDEA
-0002e850: 4141 4142 6741 4141 4145 4141 4141 4141  AAABgAAAAEAAAAAA
-0002e860: 4141 4141 5141 4141 4273 6457 3176 4141  AAAAQAAABsdW1vAA
-0002e870: 4141 4141 722f 2f2f 3841 4141 4941 3350  AAAAr///8AAAIA3P
-0002e880: 372f 2f77 4141 4151 4d51 4141 4141 4741  7//wAAAQMQAAAAGA
-0002e890: 4141 4141 5141 4141 4141 4141 4141 4241  AAAAQAAAAAAAAABA
-0002e8a0: 4141 4147 6876 6257 3841 4141 4141 4e76  AAAGhvbW8AAAAANv
-0002e8b0: 2f2f 2f77 4141 4167 4149 2f2f 2f2f 4141  ///wAAAgAI////AA
-0002e8c0: 4142 4178 4141 4141 4159 4141 4141 4241  ABAxAAAAAYAAAABA
-0002e8d0: 4141 4141 4141 4141 4146 4141 4141 5957  AAAAAAAAAFAAAAYW
-0002e8e0: 7877 6147 4541 4141 4269 2f2f 2f2f 4141  xwaGEAAABi////AA
-0002e8f0: 4143 4144 542f 2f2f 3841 4141 4544 4541  ACADT///8AAAEDEA
-0002e900: 4141 4142 5141 4141 4145 4141 4141 4141  AAABQAAAAEAAAAAA
-0002e910: 4141 4141 4941 4141 4274 6451 4141 6976  AAAAIAAABtdQAAiv
-0002e920: 2f2f 2f77 4141 4167 4263 2f2f 2f2f 4141  ///wAAAgBc////AA
-0002e930: 4142 4178 4141 4141 4155 4141 4141 4241  ABAxAAAAAUAAAABA
-0002e940: 4141 4141 4141 4141 4142 4141 4141 5177  AAAAAAAAABAAAAQw
-0002e950: 4141 414c 4c2f 2f2f 3841 4141 4941 6850  AAALL///8AAAIAhP
-0002e960: 2f2f 2f77 4141 4151 4d51 4141 4141 4641  ///wAAAQMQAAAAFA
-0002e970: 4141 4141 5141 4141 4141 4141 4141 4151  AAAAQAAAAAAAAAAQ
-0002e980: 4141 4145 4941 4141 4461 2f2f 2f2f 4141  AAAEIAAADa////AA
-0002e990: 4143 414b 7a2f 2f2f 3841 4141 4544 4541  ACAKz///8AAAEDEA
-0002e9a0: 4141 4142 6741 4141 4145 4141 4141 4141  AAABgAAAAEAAAAAA
-0002e9b0: 4141 4141 4541 4141 4242 4141 5941 4341  AAAAEAAABBAAYACA
-0002e9c0: 4147 4141 5941 4141 4141 4141 4941 3250  AGAAYAAAAAAAIA2P
-0002e9d0: 2f2f 2f77 4141 4151 5551 4141 4141 4741  ///wAAAQUQAAAAGA
-0002e9e0: 4141 4141 5141 4141 4141 4141 4141 4267  AAAAQAAAAAAAAABg
-0002e9f0: 4141 4148 4e74 6157 786c 6377 4141 7950  AAAHNtaWxlcwAAyP
-0002ea00: 2f2f 2f78 4141 4641 4149 4141 5941 4277  ///xAAFAAIAAYABw
-0002ea10: 414d 4141 4141 4541 4151 4141 4141 4141  AMAAAAEAAQAAAAAA
-0002ea20: 4142 4252 4141 4141 4163 4141 4141 4241  ABBRAAAAAcAAAABA
-0002ea30: 4141 4141 4141 4141 4147 4141 4141 6257  AAAAAAAAAGAAAAbW
-0002ea40: 3973 5832 6c6b 4141 4145 4141 5141 4241  9sX2lkAAAEAAQABA
-0002ea50: 4141 4141 3d3d 0018 1f70 6172 7175 6574  AAAA==...parquet
-0002ea60: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-0002ea70: 6f6e 2039 2e30 2e30 19fc 151c 0000 1c00  on 9.0.0........
-0002ea80: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
-0002ea90: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
-0002eaa0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
-0002eab0: 001c 0000 1c00 001c 0000 0085 2700 0050  ............'..P
-0002eac0: 4152 31                                  AR1
+0002d6a0: 7273 696f 6e22 3a20 2231 322e 302e 3122  rsion": "12.0.1"
+0002d6b0: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
+0002d6c0: 6f6e 223a 2022 322e 302e 3222 7d00 180c  on": "2.0.2"}...
+0002d6d0: 4152 524f 573a 7363 6865 6d61 18f8 262f  ARROW:schema..&/
+0002d6e0: 2f2f 2f2f 3541 4f41 4141 5141 4141 4141  ////5AOAAAQAAAAA
+0002d6f0: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
+0002d700: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
+0002d710: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
+0002d720: 6741 4141 4851 4b41 4141 4541 4141 4141  gAAAHQKAAAEAAAAA
+0002d730: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
+0002d740: 4141 4941 4167 4141 4141 4941 4141 4145  AAIAAgAAAAIAAAAE
+0002d750: 4141 4141 4159 4141 4142 7759 5735 6b59  AAAAAYAAABwYW5kY
+0002d760: 584d 4141 4438 4b41 4142 3749 6d6c 755a  XMAAD8KAAB7ImluZ
+0002d770: 4756 3458 324e 7662 4856 7462 6e4d 694f  GV4X2NvbHVtbnMiO
+0002d780: 6942 6265 794a 7261 5735 6b49 6a6f 6749  iBbeyJraW5kIjogI
+0002d790: 6e4a 6862 6d64 6c49 6977 6749 6d35 6862  nJhbmdlIiwgIm5hb
+0002d7a0: 5755 694f 6942 7564 5778 734c 4341 6963  WUiOiBudWxsLCAic
+0002d7b0: 3352 6863 6e51 694f 6941 774c 4341 6963  3RhcnQiOiAwLCAic
+0002d7c0: 3352 7663 4349 3649 4445 774d 4459 7349  3RvcCI6IDEwMDYsI
+0002d7d0: 434a 7a64 4756 7749 6a6f 674d 5831 644c  CJzdGVwIjogMX1dL
+0002d7e0: 4341 6959 3239 7364 5731 7558 326c 755a  CAiY29sdW1uX2luZ
+0002d7f0: 4756 345a 584d 694f 6942 6265 794a 7559  GV4ZXMiOiBbeyJuY
+0002d800: 5731 6c49 6a6f 6762 6e56 7362 4377 6749  W1lIjogbnVsbCwgI
+0002d810: 6d5a 705a 5778 6b58 3235 6862 5755 694f  mZpZWxkX25hbWUiO
+0002d820: 6942 7564 5778 734c 4341 6963 4746 755a  iBudWxsLCAicGFuZ
+0002d830: 4746 7a58 3352 3563 4755 694f 6941 6964  GFzX3R5cGUiOiAid
+0002d840: 5735 7059 3239 6b5a 5349 7349 434a 7564  W5pY29kZSIsICJud
+0002d850: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+0002d860: 6d39 6961 6d56 6a64 4349 7349 434a 745a  m9iamVjdCIsICJtZ
+0002d870: 5852 685a 4746 3059 5349 3649 4873 695a  XRhZGF0YSI6IHsiZ
+0002d880: 5735 6a62 3252 7062 6d63 694f 6941 6956  W5jb2RpbmciOiAiV
+0002d890: 5652 474c 5467 6966 5831 644c 4341 6959  VRGLTgifX1dLCAiY
+0002d8a0: 3239 7364 5731 7563 7949 3649 4674 3749  29sdW1ucyI6IFt7I
+0002d8b0: 6d35 6862 5755 694f 6941 6962 5739 7358  m5hbWUiOiAibW9sX
+0002d8c0: 326c 6b49 6977 6749 6d5a 705a 5778 6b58  2lkIiwgImZpZWxkX
+0002d8d0: 3235 6862 5755 694f 6941 6962 5739 7358  25hbWUiOiAibW9sX
+0002d8e0: 326c 6b49 6977 6749 6e42 6862 6d52 6863  2lkIiwgInBhbmRhc
+0002d8f0: 3139 3065 5842 6c49 6a6f 6749 6e56 7561  190eXBlIjogInVua
+0002d900: 574e 765a 4755 694c 4341 6962 6e56 7463  WNvZGUiLCAibnVtc
+0002d910: 486c 6664 486c 775a 5349 3649 434a 7659  HlfdHlwZSI6ICJvY
+0002d920: 6d70 6c59 3351 694c 4341 6962 5756 3059  mplY3QiLCAibWV0Y
+0002d930: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+0002d940: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+0002d950: 6e4e 7461 5778 6c63 7949 7349 434a 6d61  nNtaWxlcyIsICJma
+0002d960: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
+0002d970: 6e4e 7461 5778 6c63 7949 7349 434a 7759  nNtaWxlcyIsICJwY
+0002d980: 5735 6b59 584e 6664 486c 775a 5349 3649  W5kYXNfdHlwZSI6I
+0002d990: 434a 3162 6d6c 6a62 3252 6c49 6977 6749  CJ1bmljb2RlIiwgI
+0002d9a0: 6d35 3162 5842 3558 3352 3563 4755 694f  m51bXB5X3R5cGUiO
+0002d9b0: 6941 6962 324a 715a 574e 3049 6977 6749  iAib2JqZWN0IiwgI
+0002d9c0: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
+0002d9d0: 6e56 7362 4830 7349 4873 6962 6d46 745a  nVsbH0sIHsibmFtZ
+0002d9e0: 5349 3649 434a 4249 6977 6749 6d5a 705a  SI6ICJBIiwgImZpZ
+0002d9f0: 5778 6b58 3235 6862 5755 694f 6941 6951  WxkX25hbWUiOiAiQ
+0002da00: 5349 7349 434a 7759 5735 6b59 584e 6664  SIsICJwYW5kYXNfd
+0002da10: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+0002da20: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
+0002da30: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+0002da40: 5851 324e 4349 7349 434a 745a 5852 685a  XQ2NCIsICJtZXRhZ
+0002da50: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
+0002da60: 4342 3749 6d35 6862 5755 694f 6941 6951  CB7Im5hbWUiOiAiQ
+0002da70: 6949 7349 434a 6d61 5756 735a 4639 7559  iIsICJmaWVsZF9uY
+0002da80: 5731 6c49 6a6f 6749 6b49 694c 4341 6963  W1lIjogIkIiLCAic
+0002da90: 4746 755a 4746 7a58 3352 3563 4755 694f  GFuZGFzX3R5cGUiO
+0002daa0: 6941 695a 6d78 7659 5851 324e 4349 7349  iAiZmxvYXQ2NCIsI
+0002dab0: 434a 7564 5731 7765 5639 3065 5842 6c49  CJudW1weV90eXBlI
+0002dac0: 6a6f 6749 6d5a 7362 3246 304e 6a51 694c  jogImZsb2F0NjQiL
+0002dad0: 4341 6962 5756 3059 5752 6864 4745 694f  CAibWV0YWRhdGEiO
+0002dae0: 6942 7564 5778 7366 5377 6765 794a 7559  iBudWxsfSwgeyJuY
+0002daf0: 5731 6c49 6a6f 6749 6b4d 694c 4341 695a  W1lIjogIkMiLCAiZ
+0002db00: 6d6c 6c62 4752 6662 6d46 745a 5349 3649  mllbGRfbmFtZSI6I
+0002db10: 434a 4449 6977 6749 6e42 6862 6d52 6863  CJDIiwgInBhbmRhc
+0002db20: 3139 3065 5842 6c49 6a6f 6749 6d5a 7362  190eXBlIjogImZsb
+0002db30: 3246 304e 6a51 694c 4341 6962 6e56 7463  2F0NjQiLCAibnVtc
+0002db40: 486c 6664 486c 775a 5349 3649 434a 6d62  HlfdHlwZSI6ICJmb
+0002db50: 4739 6864 4459 3049 6977 6749 6d31 6c64  G9hdDY0IiwgIm1ld
+0002db60: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+0002db70: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+0002db80: 434a 7464 5349 7349 434a 6d61 5756 735a  CJtdSIsICJmaWVsZ
+0002db90: 4639 7559 5731 6c49 6a6f 6749 6d31 3149  F9uYW1lIjogIm11I
+0002dba0: 6977 6749 6e42 6862 6d52 6863 3139 3065  iwgInBhbmRhc190e
+0002dbb0: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+0002dbc0: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
+0002dbd0: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+0002dbe0: 4459 3049 6977 6749 6d31 6c64 4746 6b59  DY0IiwgIm1ldGFkY
+0002dbf0: 5852 6849 6a6f 6762 6e56 7362 4830 7349  XRhIjogbnVsbH0sI
+0002dc00: 4873 6962 6d46 745a 5349 3649 434a 6862  HsibmFtZSI6ICJhb
+0002dc10: 4842 6f59 5349 7349 434a 6d61 5756 735a  HBoYSIsICJmaWVsZ
+0002dc20: 4639 7559 5731 6c49 6a6f 6749 6d46 7363  F9uYW1lIjogImFsc
+0002dc30: 4768 6849 6977 6749 6e42 6862 6d52 6863  GhhIiwgInBhbmRhc
+0002dc40: 3139 3065 5842 6c49 6a6f 6749 6d5a 7362  190eXBlIjogImZsb
+0002dc50: 3246 304e 6a51 694c 4341 6962 6e56 7463  2F0NjQiLCAibnVtc
+0002dc60: 486c 6664 486c 775a 5349 3649 434a 6d62  HlfdHlwZSI6ICJmb
+0002dc70: 4739 6864 4459 3049 6977 6749 6d31 6c64  G9hdDY0IiwgIm1ld
+0002dc80: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+0002dc90: 4830 7349 4873 6962 6d46 745a 5349 3649  H0sIHsibmFtZSI6I
+0002dca0: 434a 6f62 3231 7649 6977 6749 6d5a 705a  CJob21vIiwgImZpZ
+0002dcb0: 5778 6b58 3235 6862 5755 694f 6941 6961  WxkX25hbWUiOiAia
+0002dcc0: 4739 7462 7949 7349 434a 7759 5735 6b59  G9tbyIsICJwYW5kY
+0002dcd0: 584e 6664 486c 775a 5349 3649 434a 6d62  XNfdHlwZSI6ICJmb
+0002dce0: 4739 6864 4459 3049 6977 6749 6d35 3162  G9hdDY0IiwgIm51b
+0002dcf0: 5842 3558 3352 3563 4755 694f 6941 695a  XB5X3R5cGUiOiAiZ
+0002dd00: 6d78 7659 5851 324e 4349 7349 434a 745a  mxvYXQ2NCIsICJtZ
+0002dd10: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
+0002dd20: 4778 394c 4342 3749 6d35 6862 5755 694f  Gx9LCB7Im5hbWUiO
+0002dd30: 6941 6962 4856 7462 7949 7349 434a 6d61  iAibHVtbyIsICJma
+0002dd40: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
+0002dd50: 6d78 3162 5738 694c 4341 6963 4746 755a  mx1bW8iLCAicGFuZ
+0002dd60: 4746 7a58 3352 3563 4755 694f 6941 695a  GFzX3R5cGUiOiAiZ
+0002dd70: 6d78 7659 5851 324e 4349 7349 434a 7564  mxvYXQ2NCIsICJud
+0002dd80: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+0002dd90: 6d5a 7362 3246 304e 6a51 694c 4341 6962  mZsb2F0NjQiLCAib
+0002dda0: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
+0002ddb0: 5778 7366 5377 6765 794a 7559 5731 6c49  WxsfSwgeyJuYW1lI
+0002ddc0: 6a6f 6749 6d64 6863 4349 7349 434a 6d61  jogImdhcCIsICJma
+0002ddd0: 5756 735a 4639 7559 5731 6c49 6a6f 6749  WVsZF9uYW1lIjogI
+0002dde0: 6d64 6863 4349 7349 434a 7759 5735 6b59  mdhcCIsICJwYW5kY
+0002ddf0: 584e 6664 486c 775a 5349 3649 434a 6d62  XNfdHlwZSI6ICJmb
+0002de00: 4739 6864 4459 3049 6977 6749 6d35 3162  G9hdDY0IiwgIm51b
+0002de10: 5842 3558 3352 3563 4755 694f 6941 695a  XB5X3R5cGUiOiAiZ
+0002de20: 6d78 7659 5851 324e 4349 7349 434a 745a  mxvYXQ2NCIsICJtZ
+0002de30: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
+0002de40: 4778 394c 4342 3749 6d35 6862 5755 694f  Gx9LCB7Im5hbWUiO
+0002de50: 6941 6963 6a49 694c 4341 695a 6d6c 6c62  iAicjIiLCAiZmllb
+0002de60: 4752 6662 6d46 745a 5349 3649 434a 794d  GRfbmFtZSI6ICJyM
+0002de70: 6949 7349 434a 7759 5735 6b59 584e 6664  iIsICJwYW5kYXNfd
+0002de80: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+0002de90: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
+0002dea0: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+0002deb0: 5851 324e 4349 7349 434a 745a 5852 685a  XQ2NCIsICJtZXRhZ
+0002dec0: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
+0002ded0: 4342 3749 6d35 6862 5755 694f 6941 6965  CB7Im5hbWUiOiAie
+0002dee0: 6e42 325a 5349 7349 434a 6d61 5756 735a  nB2ZSIsICJmaWVsZ
+0002def0: 4639 7559 5731 6c49 6a6f 6749 6e70 7764  F9uYW1lIjogInpwd
+0002df00: 6d55 694c 4341 6963 4746 755a 4746 7a58  mUiLCAicGFuZGFzX
+0002df10: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+0002df20: 5851 324e 4349 7349 434a 7564 5731 7765  XQ2NCIsICJudW1we
+0002df30: 5639 3065 5842 6c49 6a6f 6749 6d5a 7362  V90eXBlIjogImZsb
+0002df40: 3246 304e 6a51 694c 4341 6962 5756 3059  2F0NjQiLCAibWV0Y
+0002df50: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+0002df60: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+0002df70: 6e55 7749 6977 6749 6d5a 705a 5778 6b58  nUwIiwgImZpZWxkX
+0002df80: 3235 6862 5755 694f 6941 6964 5441 694c  25hbWUiOiAidTAiL
+0002df90: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
+0002dfa0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+0002dfb0: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
+0002dfc0: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+0002dfd0: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
+0002dfe0: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
+0002dff0: 794a 7559 5731 6c49 6a6f 6749 6e55 794f  yJuYW1lIjogInUyO
+0002e000: 5467 694c 4341 695a 6d6c 6c62 4752 6662  TgiLCAiZmllbGRfb
+0002e010: 6d46 745a 5349 3649 434a 314d 6a6b 3449  mFtZSI6ICJ1Mjk4I
+0002e020: 6977 6749 6e42 6862 6d52 6863 3139 3065  iwgInBhbmRhc190e
+0002e030: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+0002e040: 6a51 694c 4341 6962 6e56 7463 486c 6664  jQiLCAibnVtcHlfd
+0002e050: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+0002e060: 4459 3049 6977 6749 6d31 6c64 4746 6b59  DY0IiwgIm1ldGFkY
+0002e070: 5852 6849 6a6f 6762 6e56 7362 4830 7349  XRhIjogbnVsbH0sI
+0002e080: 4873 6962 6d46 745a 5349 3649 434a 6f4d  HsibmFtZSI6ICJoM
+0002e090: 6a6b 3449 6977 6749 6d5a 705a 5778 6b58  jk4IiwgImZpZWxkX
+0002e0a0: 3235 6862 5755 694f 6941 6961 4449 354f  25hbWUiOiAiaDI5O
+0002e0b0: 4349 7349 434a 7759 5735 6b59 584e 6664  CIsICJwYW5kYXNfd
+0002e0c0: 486c 775a 5349 3649 434a 6d62 4739 6864  HlwZSI6ICJmbG9hd
+0002e0d0: 4459 3049 6977 6749 6d35 3162 5842 3558  DY0IiwgIm51bXB5X
+0002e0e0: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+0002e0f0: 5851 324e 4349 7349 434a 745a 5852 685a  XQ2NCIsICJtZXRhZ
+0002e100: 4746 3059 5349 3649 4735 3162 4778 394c  GF0YSI6IG51bGx9L
+0002e110: 4342 3749 6d35 6862 5755 694f 6941 695a  CB7Im5hbWUiOiAiZ
+0002e120: 7a49 354f 4349 7349 434a 6d61 5756 735a  zI5OCIsICJmaWVsZ
+0002e130: 4639 7559 5731 6c49 6a6f 6749 6d63 794f  F9uYW1lIjogImcyO
+0002e140: 5467 694c 4341 6963 4746 755a 4746 7a58  TgiLCAicGFuZGFzX
+0002e150: 3352 3563 4755 694f 6941 695a 6d78 7659  3R5cGUiOiAiZmxvY
+0002e160: 5851 324e 4349 7349 434a 7564 5731 7765  XQ2NCIsICJudW1we
+0002e170: 5639 3065 5842 6c49 6a6f 6749 6d5a 7362  V90eXBlIjogImZsb
+0002e180: 3246 304e 6a51 694c 4341 6962 5756 3059  2F0NjQiLCAibWV0Y
+0002e190: 5752 6864 4745 694f 6942 7564 5778 7366  WRhdGEiOiBudWxsf
+0002e1a0: 5377 6765 794a 7559 5731 6c49 6a6f 6749  SwgeyJuYW1lIjogI
+0002e1b0: 6d4e 3249 6977 6749 6d5a 705a 5778 6b58  mN2IiwgImZpZWxkX
+0002e1c0: 3235 6862 5755 694f 6941 6959 3359 694c  25hbWUiOiAiY3YiL
+0002e1d0: 4341 6963 4746 755a 4746 7a58 3352 3563  CAicGFuZGFzX3R5c
+0002e1e0: 4755 694f 6941 695a 6d78 7659 5851 324e  GUiOiAiZmxvYXQ2N
+0002e1f0: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
+0002e200: 5842 6c49 6a6f 6749 6d5a 7362 3246 304e  XBlIjogImZsb2F0N
+0002e210: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
+0002e220: 4745 694f 6942 7564 5778 7366 5377 6765  GEiOiBudWxsfSwge
+0002e230: 794a 7559 5731 6c49 6a6f 6749 6e55 7758  yJuYW1lIjogInUwX
+0002e240: 3246 3062 3230 694c 4341 695a 6d6c 6c62  2F0b20iLCAiZmllb
+0002e250: 4752 6662 6d46 745a 5349 3649 434a 314d  GRfbmFtZSI6ICJ1M
+0002e260: 4639 6864 4739 7449 6977 6749 6e42 6862  F9hdG9tIiwgInBhb
+0002e270: 6d52 6863 3139 3065 5842 6c49 6a6f 6749  mRhc190eXBlIjogI
+0002e280: 6d5a 7362 3246 304e 6a51 694c 4341 6962  mZsb2F0NjQiLCAib
+0002e290: 6e56 7463 486c 6664 486c 775a 5349 3649  nVtcHlfdHlwZSI6I
+0002e2a0: 434a 6d62 4739 6864 4459 3049 6977 6749  CJmbG9hdDY0IiwgI
+0002e2b0: 6d31 6c64 4746 6b59 5852 6849 6a6f 6762  m1ldGFkYXRhIjogb
+0002e2c0: 6e56 7362 4830 7349 4873 6962 6d46 745a  nVsbH0sIHsibmFtZ
+0002e2d0: 5349 3649 434a 314d 6a6b 3458 3246 3062  SI6ICJ1Mjk4X2F0b
+0002e2e0: 3230 694c 4341 695a 6d6c 6c62 4752 6662  20iLCAiZmllbGRfb
+0002e2f0: 6d46 745a 5349 3649 434a 314d 6a6b 3458  mFtZSI6ICJ1Mjk4X
+0002e300: 3246 3062 3230 694c 4341 6963 4746 755a  2F0b20iLCAicGFuZ
+0002e310: 4746 7a58 3352 3563 4755 694f 6941 695a  GFzX3R5cGUiOiAiZ
+0002e320: 6d78 7659 5851 324e 4349 7349 434a 7564  mxvYXQ2NCIsICJud
+0002e330: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
+0002e340: 6d5a 7362 3246 304e 6a51 694c 4341 6962  mZsb2F0NjQiLCAib
+0002e350: 5756 3059 5752 6864 4745 694f 6942 7564  WV0YWRhdGEiOiBud
+0002e360: 5778 7366 5377 6765 794a 7559 5731 6c49  WxsfSwgeyJuYW1lI
+0002e370: 6a6f 6749 6d67 794f 5468 6659 5852 7662  jogImgyOThfYXRvb
+0002e380: 5349 7349 434a 6d61 5756 735a 4639 7559  SIsICJmaWVsZF9uY
+0002e390: 5731 6c49 6a6f 6749 6d67 794f 5468 6659  W1lIjogImgyOThfY
+0002e3a0: 5852 7662 5349 7349 434a 7759 5735 6b59  XRvbSIsICJwYW5kY
+0002e3b0: 584e 6664 486c 775a 5349 3649 434a 6d62  XNfdHlwZSI6ICJmb
+0002e3c0: 4739 6864 4459 3049 6977 6749 6d35 3162  G9hdDY0IiwgIm51b
+0002e3d0: 5842 3558 3352 3563 4755 694f 6941 695a  XB5X3R5cGUiOiAiZ
+0002e3e0: 6d78 7659 5851 324e 4349 7349 434a 745a  mxvYXQ2NCIsICJtZ
+0002e3f0: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
+0002e400: 4778 394c 4342 3749 6d35 6862 5755 694f  Gx9LCB7Im5hbWUiO
+0002e410: 6941 695a 7a49 354f 4639 6864 4739 7449  iAiZzI5OF9hdG9tI
+0002e420: 6977 6749 6d5a 705a 5778 6b58 3235 6862  iwgImZpZWxkX25hb
+0002e430: 5755 694f 6941 695a 7a49 354f 4639 6864  WUiOiAiZzI5OF9hd
+0002e440: 4739 7449 6977 6749 6e42 6862 6d52 6863  G9tIiwgInBhbmRhc
+0002e450: 3139 3065 5842 6c49 6a6f 6749 6d5a 7362  190eXBlIjogImZsb
+0002e460: 3246 304e 6a51 694c 4341 6962 6e56 7463  2F0NjQiLCAibnVtc
+0002e470: 486c 6664 486c 775a 5349 3649 434a 6d62  HlfdHlwZSI6ICJmb
+0002e480: 4739 6864 4459 3049 6977 6749 6d31 6c64  G9hdDY0IiwgIm1ld
+0002e490: 4746 6b59 5852 6849 6a6f 6762 6e56 7362  GFkYXRhIjogbnVsb
+0002e4a0: 4831 644c 4341 6959 334a 6c59 5852 7663  H1dLCAiY3JlYXRvc
+0002e4b0: 6949 3649 4873 6962 476c 6963 6d46 7965  iI6IHsibGlicmFye
+0002e4c0: 5349 3649 434a 7765 5746 7963 6d39 3349  SI6ICJweWFycm93I
+0002e4d0: 6977 6749 6e5a 6c63 6e4e 7062 3234 694f  iwgInZlcnNpb24iO
+0002e4e0: 6941 694d 5449 754d 4334 7849 6e30 7349  iAiMTIuMC4xIn0sI
+0002e4f0: 434a 7759 5735 6b59 584e 6664 6d56 7963  CJwYW5kYXNfdmVyc
+0002e500: 326c 7662 6949 3649 4349 794c 6a41 754d  2lvbiI6ICIyLjAuM
+0002e510: 694a 3941 4255 4141 4144 4141 7741 4168  iJ9ABUAAADAAwAAh
+0002e520: 414d 4141 4651 4441 4141 6f41 7741 412f  AMAAFQDAAAoAwAA/
+0002e530: 4149 4141 4e41 4341 4143 6741 6741 4163  AIAANACAACgAgAAc
+0002e540: 4149 4141 4541 4341 4141 5541 6741 4136  AIAAEACAAAUAgAA6
+0002e550: 4145 4141 4c67 4241 4143 4d41 5141 4158  AEAALgBAACMAQAAX
+0002e560: 4145 4141 4377 4241 4144 3841 4141 4130  AEAACwBAAD8AAAA0
+0002e570: 4141 4141 4b41 4141 4142 7341 4141 414f  AAAAKAAAABsAAAAO
+0002e580: 4141 4141 4151 4141 4143 6b2f 502f 2f41  AAAAAQAAACk/P//A
+0002e590: 4141 4241 7841 4141 4141 6341 4141 4142  AABAxAAAAAcAAAAB
+0002e5a0: 4141 4141 4141 4141 4141 4a41 4141 415a  AAAAAAAAAAJAAAAZ
+0002e5b0: 7a49 354f 4639 6864 4739 7441 4141 4141  zI5OF9hdG9tAAAAA
+0002e5c0: 7633 2f2f 7741 4141 6744 552f 502f 2f41  v3//wAAAgDU/P//A
+0002e5d0: 4141 4241 7841 4141 4141 6341 4141 4142  AABAxAAAAAcAAAAB
+0002e5e0: 4141 4141 4141 4141 4141 4a41 4141 4161  AAAAAAAAAAJAAAAa
+0002e5f0: 4449 354f 4639 6864 4739 7441 4141 414d  DI5OF9hdG9tAAAAM
+0002e600: 7633 2f2f 7741 4141 6741 452f 662f 2f41  v3//wAAAgAE/f//A
+0002e610: 4141 4241 7841 4141 4141 6341 4141 4142  AABAxAAAAAcAAAAB
+0002e620: 4141 4141 4141 4141 4141 4a41 4141 4164  AAAAAAAAAAJAAAAd
+0002e630: 5449 354f 4639 6864 4739 7441 4141 4159  TI5OF9hdG9tAAAAY
+0002e640: 7633 2f2f 7741 4141 6741 302f 662f 2f41  v3//wAAAgA0/f//A
+0002e650: 4141 4241 7841 4141 4141 5941 4141 4142  AABAxAAAAAYAAAAB
+0002e660: 4141 4141 4141 4141 4141 4841 4141 4164  AAAAAAAAAAHAAAAd
+0002e670: 5442 6659 5852 7662 5143 4f2f 662f 2f41  TBfYXRvbQCO/f//A
+0002e680: 4141 4341 4744 392f 2f38 4141 4145 4445  AACAGD9//8AAAEDE
+0002e690: 4141 4141 4251 4141 4141 4541 4141 4141  AAAABQAAAAEAAAAA
+0002e6a0: 4141 4141 4149 4141 4142 6a64 6741 4174  AAAAAIAAABjdgAAt
+0002e6b0: 7633 2f2f 7741 4141 6743 492f 662f 2f41  v3//wAAAgCI/f//A
+0002e6c0: 4141 4241 7841 4141 4141 5941 4141 4142  AABAxAAAAAYAAAAB
+0002e6d0: 4141 4141 4141 4141 4141 4541 4141 415a  AAAAAAAAAAEAAAAZ
+0002e6e0: 7a49 354f 4141 4141 4144 692f 662f 2f41  zI5OAAAAADi/f//A
+0002e6f0: 4141 4341 4c54 392f 2f38 4141 4145 4445  AACALT9//8AAAEDE
+0002e700: 4141 4141 4267 4141 4141 4541 4141 4141  AAAABgAAAAEAAAAA
+0002e710: 4141 4141 4151 4141 4142 6f4d 6a6b 3441  AAAAAQAAABoMjk4A
+0002e720: 4141 4141 4137 2b2f 2f38 4141 4149 4134  AAAAA7+//8AAAIA4
+0002e730: 5033 2f2f 7741 4141 514d 5141 4141 4147  P3//wAAAQMQAAAAG
+0002e740: 4141 4141 4151 4141 4141 4141 4141 4142  AAAAAQAAAAAAAAAB
+0002e750: 4141 4141 4855 794f 5467 4141 4141 414f  AAAAHUyOTgAAAAAO
+0002e760: 7637 2f2f 7741 4141 6741 4d2f 762f 2f41  v7//wAAAgAM/v//A
+0002e770: 4141 4241 7841 4141 4141 5541 4141 4142  AABAxAAAAAUAAAAB
+0002e780: 4141 4141 4141 4141 4141 4341 4141 4164  AAAAAAAAAACAAAAd
+0002e790: 5441 4141 474c 2b2f 2f38 4141 4149 414e  TAAAGL+//8AAAIAN
+0002e7a0: 5037 2f2f 7741 4141 514d 5141 4141 4147  P7//wAAAQMQAAAAG
+0002e7b0: 4141 4141 4151 4141 4141 4141 4141 4142  AAAAAQAAAAAAAAAB
+0002e7c0: 4141 4141 4870 7764 6d55 4141 4141 416a  AAAAHpwdmUAAAAAj
+0002e7d0: 7637 2f2f 7741 4141 6742 672f 762f 2f41  v7//wAAAgBg/v//A
+0002e7e0: 4141 4241 7841 4141 4141 5541 4141 4142  AABAxAAAAAUAAAAB
+0002e7f0: 4141 4141 4141 4141 4141 4341 4141 4163  AAAAAAAAAACAAAAc
+0002e800: 6a49 4141 4c62 2b2f 2f38 4141 4149 4169  jIAALb+//8AAAIAi
+0002e810: 5037 2f2f 7741 4141 514d 5141 4141 4146  P7//wAAAQMQAAAAF
+0002e820: 4141 4141 4151 4141 4141 4141 4141 4141  AAAAAQAAAAAAAAAA
+0002e830: 7741 4141 4764 6863 4144 652f 762f 2f41  wAAAGdhcADe/v//A
+0002e840: 4141 4341 4c44 2b2f 2f38 4141 4145 4445  AACALD+//8AAAEDE
+0002e850: 4141 4141 4267 4141 4141 4541 4141 4141  AAAABgAAAAEAAAAA
+0002e860: 4141 4141 4151 4141 4142 7364 5731 7641  AAAAAQAAABsdW1vA
+0002e870: 4141 4141 4172 2f2f 2f38 4141 4149 4133  AAAAAr///8AAAIA3
+0002e880: 5037 2f2f 7741 4141 514d 5141 4141 4147  P7//wAAAQMQAAAAG
+0002e890: 4141 4141 4151 4141 4141 4141 4141 4142  AAAAAQAAAAAAAAAB
+0002e8a0: 4141 4141 4768 7662 5738 4141 4141 414e  AAAAGhvbW8AAAAAN
+0002e8b0: 762f 2f2f 7741 4141 6741 492f 2f2f 2f41  v///wAAAgAI////A
+0002e8c0: 4141 4241 7841 4141 4141 5941 4141 4142  AABAxAAAAAYAAAAB
+0002e8d0: 4141 4141 4141 4141 4141 4641 4141 4159  AAAAAAAAAAFAAAAY
+0002e8e0: 5778 7761 4745 4141 4142 692f 2f2f 2f41  WxwaGEAAABi////A
+0002e8f0: 4141 4341 4454 2f2f 2f38 4141 4145 4445  AACADT///8AAAEDE
+0002e900: 4141 4141 4251 4141 4141 4541 4141 4141  AAAABQAAAAEAAAAA
+0002e910: 4141 4141 4149 4141 4142 7464 5141 4169  AAAAAIAAABtdQAAi
+0002e920: 762f 2f2f 7741 4141 6742 632f 2f2f 2f41  v///wAAAgBc////A
+0002e930: 4141 4241 7841 4141 4141 5541 4141 4142  AABAxAAAAAUAAAAB
+0002e940: 4141 4141 4141 4141 4141 4241 4141 4151  AAAAAAAAAABAAAAQ
+0002e950: 7741 4141 4c4c 2f2f 2f38 4141 4149 4168  wAAALL///8AAAIAh
+0002e960: 502f 2f2f 7741 4141 514d 5141 4141 4146  P///wAAAQMQAAAAF
+0002e970: 4141 4141 4151 4141 4141 4141 4141 4141  AAAAAQAAAAAAAAAA
+0002e980: 5141 4141 4549 4141 4144 612f 2f2f 2f41  QAAAEIAAADa////A
+0002e990: 4141 4341 4b7a 2f2f 2f38 4141 4145 4445  AACAKz///8AAAEDE
+0002e9a0: 4141 4141 4267 4141 4141 4541 4141 4141  AAAABgAAAAEAAAAA
+0002e9b0: 4141 4141 4145 4141 4142 4241 4159 4143  AAAAAEAAABBAAYAC
+0002e9c0: 4141 4741 4159 4141 4141 4141 4149 4132  AAGAAYAAAAAAAIA2
+0002e9d0: 502f 2f2f 7741 4141 5155 5141 4141 4147  P///wAAAQUQAAAAG
+0002e9e0: 4141 4141 4151 4141 4141 4141 4141 4142  AAAAAQAAAAAAAAAB
+0002e9f0: 6741 4141 484e 7461 5778 6c63 7741 4179  gAAAHNtaWxlcwAAy
+0002ea00: 502f 2f2f 7841 4146 4141 4941 4159 4142  P///xAAFAAIAAYAB
+0002ea10: 7741 4d41 4141 4145 4141 5141 4141 4141  wAMAAAAEAAQAAAAA
+0002ea20: 4141 4242 5241 4141 4141 6341 4141 4142  AABBRAAAAAcAAAAB
+0002ea30: 4141 4141 4141 4141 4141 4741 4141 4162  AAAAAAAAAAGAAAAb
+0002ea40: 5739 7358 326c 6b41 4141 4541 4151 4142  W9sX2lkAAAEAAQAB
+0002ea50: 4141 4141 413d 3d00 1820 7061 7271 7565  AAAAA==.. parque
+0002ea60: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
+0002ea70: 696f 6e20 3132 2e30 2e30 19fc 151c 0000  ion 12.0.0......
+0002ea80: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
+0002ea90: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
+0002eaa0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
+0002eab0: 1c00 001c 0000 1c00 001c 0000 0087 2700  ..............'.
+0002eac0: 0050 4152 31                             .PAR1
```

### Comparing `graphium-2.0.2/graphium/data/QM9/norm_micro_qm9.csv` & `graphium-2.1.0/graphium/data/QM9/norm_micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/README.md` & `graphium-2.1.0/graphium/data/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/collate.py` & `graphium-2.1.0/graphium/data/collate.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from torch.utils.data.dataloader import default_collate
 from typing import Union, List, Optional, Dict, Type, Any, Iterable
 from torch_geometric.data import Data, Batch
 
 from graphium.features import GraphDict, to_dense_array
 from graphium.utils.packing import fast_packing, get_pack_sizes, node_to_pack_indices_mask
 from loguru import logger
+from graphium.data.utils import get_keys
 
 
 def graphium_collate_fn(
     elements: Union[List[Any], Dict[str, List[Any]]],
     labels_size_dict: Optional[Dict[str, Any]] = None,
+    labels_dtype_dict: Optional[Dict[str, Any]] = None,
     mask_nan: Union[str, float, Type[None]] = "raise",
     do_not_collate_keys: List[str] = [],
     batch_size_per_pack: Optional[int] = None,
 ) -> Union[Any, Dict[str, Any]]:
     """This collate function is identical to the default
     pytorch collate function but add support for `pyg.data.Data` to batch graphs.
 
@@ -38,14 +40,19 @@
 
         labels_size_dict:
             (Note): This is an attribute of the `MultitaskDataset`.
             A dictionary of the form Dict[tasks, sizes] which has task names as keys
             and the size of the label tensor as value. The size of the tensor corresponds to how many
             labels/values there are to predict for that task.
 
+        labels_dtype_dict:
+            (Note): This is an attribute of the `MultitaskDataset`.
+            A dictionary of the form Dict[tasks, dtypes] which has task names as keys
+            and the dtype of the label tensor as value. This is necessary to ensure the missing labels are added with NaNs of the right dtype
+
         mask_nan:
             Deal with the NaN/Inf when calling the function `make_pyg_graph`.
             Some values become `Inf` when changing data type. This allows to deal
             with that.
 
             - "raise": Raise an error when there is a nan or inf in the featurization
             - "warn": Raise a warning when there is a nan or inf in the featurization
@@ -68,15 +75,15 @@
     elem = elements[0]
     if isinstance(elem, Mapping):
         batch = {}
         for key in elem:
             # Multitask setting: We have to pad the missing labels
             if key == "labels":
                 labels = [d[key] for d in elements]
-                batch[key] = collate_labels(labels, labels_size_dict)
+                batch[key] = collate_labels(labels, labels_size_dict, labels_dtype_dict)
 
             # If the features are a dictionary containing GraphDict elements,
             # Convert to pyg graphs and use the pyg batching.
             elif isinstance(elem[key], GraphDict):
                 pyg_graphs = [d[key].make_pyg_graph(mask_nan=mask_nan) for d in elements]
                 batch[key] = collage_pyg_graph(pyg_graphs)
 
@@ -120,15 +127,15 @@
     num_nodes_list = []
     for pyg_graph in pyg_graphs:
         num_nodes_list.append(pyg_graph["num_nodes"])
     max_num_nodes_per_graph = max(num_nodes_list)
 
     pyg_batch = []
     for pyg_graph in pyg_graphs:
-        for pyg_key in pyg_graph.keys:
+        for pyg_key in get_keys(pyg_graph):
             tensor = pyg_graph[pyg_key]
 
             # Convert numpy/scipy to Pytorch
             if isinstance(tensor, (ndarray, spmatrix)):
                 tensor = torch.as_tensor(to_dense_array(tensor, tensor.dtype))
 
             # pad nodepair-level positional encodings
@@ -188,15 +195,15 @@
     Convert all numpy types to torch
 
     Parameters:
         pyg_labels: Iterable of PyG label Data objects
     """
     pyg_batch = []
     for pyg_label in pyg_labels:
-        for pyg_key in set(pyg_label.keys) - set(["x", "edge_index"]):
+        for pyg_key in set(get_keys(pyg_label)) - set(["x", "edge_index"]):
             tensor = pyg_label[pyg_key]
             # Convert numpy/scipy to Pytorch
             if isinstance(tensor, (ndarray, spmatrix)):
                 tensor = torch.as_tensor(to_dense_array(tensor, tensor.dtype))
 
             pyg_label[pyg_key] = tensor
 
@@ -219,42 +226,48 @@
         raise NotImplementedError()
     return [num_labels] + label_size
 
 
 def collate_labels(
     labels: List[Data],
     labels_size_dict: Optional[Dict[str, Any]] = None,
+    labels_dtype_dict: Optional[Dict[str, Any]] = None,
 ):
     """Collate labels for multitask learning.
 
     Parameters:
         labels: List of labels
         labels_size_dict: Dict of the form Dict[tasks, sizes] which has task names as keys
             and the size of the label tensor as value. The size of the tensor corresponds to how many
             labels/values there are to predict for that task.
+        labels_dtype_dict:
+            (Note): This is an attribute of the `MultitaskDataset`.
+            A dictionary of the form Dict[tasks, dtypes] which has task names as keys
+            and the dtype of the label tensor as value. This is necessary to ensure the missing labels are added with NaNs of the right dtype
 
     Returns:
         A dictionary of the form Dict[tasks, labels] where tasks is the name of the task and labels
         is a tensor of shape (batch_size, *labels_size_dict[task]).
     """
     if labels_size_dict is not None:
         for this_label in labels:
             for task in labels_size_dict.keys():
                 labels_size_dict[task] = list(labels_size_dict[task])
                 if len(labels_size_dict[task]) >= 2:
                     labels_size_dict[task] = labels_size_dict[task][1:]
                 elif not task.startswith("graph_"):
                     labels_size_dict[task] = [1]
-
-            empty_task_labels = set(labels_size_dict.keys()) - set(this_label.keys)
+            label_keys_set = set(get_keys(this_label))
+            empty_task_labels = set(labels_size_dict.keys()) - label_keys_set
             for task in empty_task_labels:
                 labels_size_dict[task] = get_expected_label_size(this_label, task, labels_size_dict[task])
-                this_label[task] = torch.full([*labels_size_dict[task]], torch.nan)
+                dtype = labels_dtype_dict[task]
+                this_label[task] = torch.full([*labels_size_dict[task]], torch.nan, dtype=dtype)
 
-            for task in set(this_label.keys) - set(["x", "edge_index"]) - empty_task_labels:
+            for task in label_keys_set - set(["x", "edge_index"]) - empty_task_labels:
                 labels_size_dict[task] = get_expected_label_size(this_label, task, labels_size_dict[task])
 
                 if not isinstance(this_label[task], (torch.Tensor)):
                     this_label[task] = torch.as_tensor(this_label[task])
 
                 # Ensure explicit task dimension also for single task labels
                 if len(this_label[task].shape) == 1:
```

### Comparing `graphium-2.0.2/graphium/data/datamodule.py` & `graphium-2.1.0/graphium/data/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 from functools import partial
 import importlib.resources
 import zipfile
 from copy import deepcopy
 import time
 import gc
 from rdkit import Chem
+import re
+from graphium.data.utils import get_keys
 
 from loguru import logger
 import fsspec
 import omegaconf
 
 import pandas as pd
 import numpy as np
 import datamol as dm
 from tqdm import tqdm
 import os.path as osp
 from fastparquet import ParquetFile
 
 from sklearn.model_selection import train_test_split
 
-import pytorch_lightning as pl
-from pytorch_lightning.trainer.states import RunningStage
+import lightning
+from lightning.pytorch.trainer.states import RunningStage
 
 import torch
 from torch_geometric.data import Data
 from torch.utils.data.dataloader import DataLoader, Dataset
 from torch.utils.data import Subset
 
 from graphium.utils import fs
@@ -76,15 +78,15 @@
         "download_name": "pcqm4m-v2",
         "url": "https://dgl-data.s3-accelerate.amazonaws.com/dataset/OGB-LSC/pcqm4m-v2.zip",  # TODO: Allow PyG
         "version": 2,
     }
 )
 
 
-class BaseDataModule(pl.LightningDataModule):
+class BaseDataModule(lightning.LightningDataModule):
     def __init__(
         self,
         batch_size_training: int = 16,
         batch_size_inference: int = 16,
         batch_size_per_pack: Optional[int] = None,
         num_workers: int = 0,
         pin_memory: bool = True,
@@ -436,15 +438,15 @@
             path: path to the file to read
             kwargs: keyword arguments for pd.read_csv or pd.read_parquet
         Returns:
             pd.DataFrame: the panda dataframe storing molecules
         """
         files = self._glob(path)
         if len(files) == 0:
-            raise FileNotFoundError("No such file or directory `{path}`")
+            raise FileNotFoundError(f"No such file or directory `{path}`")
 
         if len(files) > 1:
             files = tqdm(sorted(files), desc=f"Reading files at `{path}`")
         dfs = []
         for file in files:
             file_type = self._get_data_file_type(file)
             if file_type == "parquet":
@@ -546,30 +548,33 @@
             stages = allowed_stages
         for stage in stages:
             assert stage in allowed_stages, f"stage value `{stage}` not allowed."
 
         max_num_nodes = 0
         # Max number of nodes in the training dataset
         if (self.train_ds is not None) and ("train" in stages):
+            logger.info("Max num nodes being calcuated train")
             max_num_nodes = max(max_num_nodes, self.train_ds.max_num_nodes_per_graph)
 
         # Max number of nodes in the validation dataset
         if (
             (self.val_ds is not None)
             and ("val" in stages)
             and (self.val_ds.max_num_nodes_per_graph is not None)
         ):
+            logger.info("Max num nodes being calcuated val")
             max_num_nodes = max(max_num_nodes, self.val_ds.max_num_nodes_per_graph)
 
         # Max number of nodes in the test dataset
         if (
             (self.test_ds is not None)
             and ("test" in stages)
             and (self.test_ds.max_num_nodes_per_graph is not None)
         ):
+            logger.info("Max num nodes being calcuated test")
             max_num_nodes = max(max_num_nodes, self.test_ds.max_num_nodes_per_graph)
 
         # Max number of nodes in the predict dataset
         if (
             (self.predict_ds is not None)
             and ("predict" in stages)
             and (self.predict_ds.max_num_nodes_per_graph is not None)
@@ -914,14 +919,24 @@
             - Extract the smiles, labels from the dataframe
         - In the previous step, we were also able to get the unique smiles, which we use to compute the features
         - For each single-task dataframe and associated data (smiles, labels, etc.):
             - Filter out the data corresponding to molecules which failed featurization.
             - Create a corresponding SingletaskDataset
             - Split the SingletaskDataset according to the task-specific splits for train, val and test
         """
+
+        def has_atoms_after_h_removal(smiles):
+            # Remove all 'H' characters from the SMILES
+            smiles_without_h = re.sub("H", "", smiles)
+            # Check if any letters are remaining in the modified string
+            has_atoms = bool(re.search("[a-zA-Z]", smiles_without_h))
+            if has_atoms == False:
+                logger.info(f"Removed Hydrogen molecule: {smiles}")
+            return has_atoms
+
         if self._data_is_prepared:
             logger.info("Data is already prepared. Skipping the preparation")
             return
 
         if self.load_from_file:
             if self._ready_to_load_all_from_file():
                 self.get_label_statistics(self.processed_graph_data_path, self.data_hash, dataset=None)
@@ -978,14 +993,20 @@
         for task, df in task_df.items():
             # Subsample all the dataframes
             sample_size = self.task_dataset_processing_params[task].sample_size
             df = self._sub_sample_df(df, sample_size, self.task_dataset_processing_params[task].seed)
 
             logger.info(f"Prepare single-task dataset for task '{task}' with {len(df)} data points.")
 
+            logger.info("Filtering the molecules for Hydrogen")
+            logger.info(f"Looking at column {df.columns[0]}")
+            # Filter the DataFrame based on the function
+            # need this for pcba dataset
+            # df = df[df[df.columns[0]].apply(lambda x: has_atoms_after_h_removal(x))]
+            logger.info("Filtering done")
             # Extract smiles, labels, extras
             args = self.task_dataset_processing_params[task]
             smiles, labels, sample_idx, extras = self._extract_smiles_labels(
                 df,
                 task_level=args.task_level,
                 smiles_col=args.smiles_col,
                 label_cols=args.label_cols,
@@ -1117,14 +1138,15 @@
         Parameters:
             stage (str): Either 'fit', 'test', or None.
         """
 
         # Can possibly get rid of setup because a single dataset will have molecules exclusively in train, val or test
         # Produce the label sizes to update the collate function
         labels_size = {}
+        labels_dtype = {}
         if stage == "fit" or stage is None:
             if self.load_from_file:
                 processed_train_data_path = self._path_to_load_from_file("train")
                 assert self._data_ready_at_path(
                     processed_train_data_path
                 ), "Loading from file + setup() called but training data not ready"
                 processed_val_data_path = self._path_to_load_from_file("val")
@@ -1139,33 +1161,41 @@
             self.val_ds = self._make_multitask_dataset("val", save_smiles_and_ids=save_smiles_and_ids)
             logger.info(self.train_ds)
             logger.info(self.val_ds)
             labels_size.update(
                 self.train_ds.labels_size
             )  # Make sure that all task label sizes are contained in here. Maybe do the update outside these if statements.
             labels_size.update(self.val_ds.labels_size)
+            labels_dtype.update(self.train_ds.labels_dtype)
+            labels_dtype.update(self.val_ds.labels_dtype)
 
         if stage == "test" or stage is None:
             if self.load_from_file:
                 processed_test_data_path = self._path_to_load_from_file("test")
                 assert self._data_ready_at_path(
                     processed_test_data_path
                 ), "Loading from file + setup() called but test data not ready"
             else:
                 processed_test_data_path = None
             self.test_ds = self._make_multitask_dataset("test", save_smiles_and_ids=save_smiles_and_ids)
             logger.info(self.test_ds)
 
             labels_size.update(self.test_ds.labels_size)
+            labels_dtype.update(self.test_ds.labels_dtype)
 
         default_labels_size_dict = self.collate_fn.keywords.get("labels_size_dict", None)
 
         if default_labels_size_dict is None:
             self.collate_fn.keywords["labels_size_dict"] = labels_size
 
+        default_labels_dtype_dict = self.collate_fn.keywords.get("labels_dtype_dict", None)
+
+        if default_labels_dtype_dict is None:
+            self.collate_fn.keywords["labels_dtype_dict"] = labels_dtype
+
     def _make_multitask_dataset(
         self,
         stage: Literal["train", "val", "test"],
         save_smiles_and_ids: bool,
         load_from_file: Optional[bool] = None,
     ) -> Datasets.MultitaskDataset:
         """
@@ -1216,19 +1246,21 @@
             about=about,
             save_smiles_and_ids=save_smiles_and_ids,
             data_path=self._path_to_load_from_file(stage) if load_from_file else None,
             load_from_file=load_from_file,
             files_ready=files_ready,
         )  # type: ignore
 
+        # calculate statistics for the train split and used for all splits normalization
         if stage == "train":
             self.get_label_statistics(
                 self.processed_graph_data_path, self.data_hash, multitask_dataset, train=True
             )
-            self.normalize_label(multitask_dataset)
+        if not load_from_file:
+            self.normalize_label(multitask_dataset, stage)
 
         return multitask_dataset
 
     def _ready_to_load_all_from_file(self) -> bool:
         """
         Check if the data for all stages is ready to be loaded from files
         """
@@ -1330,28 +1362,32 @@
             if self.task_norms and train and not os.path.isfile(filename):
                 self.calculate_statistics(dataset, train=train)
                 torch.save(self.task_norms, filename, pickle_protocol=4)
             # if any of the above three condition does not satisfy, we load from file.
             else:
                 self.task_norms = torch.load(filename)
 
-    def normalize_label(self, dataset: Datasets.MultitaskDataset) -> Datasets.MultitaskDataset:
+    def normalize_label(self, dataset: Datasets.MultitaskDataset, stage) -> Datasets.MultitaskDataset:
         """
         Normalize the labels in the dataset using the statistics in `self.task_norms`.
 
         Parameters:
             dataset: the dataset to normalize the labels from
 
         Returns:
             the dataset with normalized labels
         """
         for task in dataset.labels_size.keys():
-            for i in range(len(dataset)):
-                if task in dataset[i]["labels"]:
-                    dataset[i]["labels"][task] = self.task_norms[task].normalize(dataset[i]["labels"][task])
+            # we normalize the dataset if (it is train split) or (it is val/test splits and normalize_val_test is set to true)
+            if (stage == "train") or (stage in ["val", "test"] and self.task_norms[task].normalize_val_test):
+                for i in range(len(dataset)):
+                    if task in dataset[i]["labels"]:
+                        dataset[i]["labels"][task] = self.task_norms[task].normalize(
+                            dataset[i]["labels"][task]
+                        )
         return dataset
 
     def save_featurized_data(self, dataset: Datasets.MultitaskDataset, processed_data_path):
         os.makedirs(processed_data_path)  # In case the len(dataset) is 0
         for i in range(0, len(dataset), 1000):
             os.makedirs(os.path.join(processed_data_path, format(i // 1000, "04d")), exist_ok=True)
         process_params = [(index, datum, processed_data_path) for index, datum in enumerate(dataset)]
@@ -1627,16 +1663,15 @@
 
         graph = self.get_fake_graph()
         if isinstance(graph, (GraphDict)):
             graph = graph.data
 
         # get list of all keys corresponding to positional encoding
         pe_dim_dict = {}
-        g_keys = graph.keys
-
+        g_keys = get_keys(graph)
         # ignore the normal keys for node feat and edge feat etc.
         for key in g_keys:
             prop = graph.get(key, None)
             if hasattr(prop, "shape"):
                 pe_dim_dict[key] = prop.shape[-1]
         return pe_dim_dict
```

### Comparing `graphium-2.0.2/graphium/data/dataset.py` & `graphium-2.1.0/graphium/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
             else:
                 self.mol_ids, self.smiles, self.labels = self.merge(datasets)
             # Set mol_ids and smiles to None to save memory as they are not needed.
             if not save_smiles_and_ids:
                 self.mol_ids = None
                 self.smiles = None
             self.labels_size = self.set_label_size_dict(datasets)
+            self.labels_dtype = self.set_label_dtype_dict(datasets)
             self.dataset_length = len(self.labels)
             self._num_nodes_list = None
             self._num_edges_list = None
             if self.features is not None:
                 self._num_nodes_list = get_num_nodes_per_graph(self.features)
                 self._num_edges_list = get_num_edges_per_graph(self.features)
             if self.load_from_file:
@@ -215,14 +216,15 @@
         """
         Save everything other than features/labels
         """
         attrs_to_save = [
             "mol_ids",
             "smiles",
             "labels_size",
+            "labels_dtype",
             "dataset_length",
             "_num_nodes_list",
             "_num_edges_list",
         ]
         attrs = {attr: getattr(self, attr) for attr in attrs_to_save}
 
         path = os.path.join(directory, "multitask_metadata.pkl")
@@ -233,21 +235,31 @@
         """
         Load everything other than features/labels
         """
         attrs_to_load = [
             "mol_ids",
             "smiles",
             "labels_size",
+            "labels_dtype",
             "dataset_length",
             "_num_nodes_list",
             "_num_edges_list",
         ]
         path = os.path.join(self.data_path, "multitask_metadata.pkl")
         attrs = torch.load(path)
 
+        if not set(attrs_to_load).issubset(set(attrs.keys())):
+            raise ValueError(
+                f"The metadata in the cache at {self.data_path} does not contain the right information. "
+                f"This may be because the cache was prepared using an earlier version of Graphium. "
+                f"You can try deleting the cache and running the data preparation again. "
+                f"\nMetadata keys found: {attrs.keys()}"
+                f"\nMetadata keys required: {attrs_to_load}"
+            )
+
         for attr, value in attrs.items():
             setattr(self, attr, value)
 
     def __len__(self):
         r"""
         Returns the number of molecules
         """
@@ -350,34 +362,37 @@
     @property
     def mean_num_edges_per_graph(self):
         """Average number of edges per graph"""
         if len(self) == 0:
             return
         return self.num_edges_total / self.num_graphs_total
 
-    @lru_cache(maxsize=16)
     def __getitem__(self, idx):
         r"""
         get the data for at the specified index
         Parameters:
             idx: The index of the data to retrieve
         Returns:
             A dictionary containing the data for the specified index with keys "mol_ids", "smiles", "labels", and "features"
         """
         datum = {}
         if self.load_from_file:
             data_dict = self.load_graph_from_index(idx)
             datum["features"] = data_dict["graph_with_features"]
-            # these type changes are temporary for ipu dtype match
-            if hasattr(data_dict["labels"], "graph_pcba_1328"):
-                data_dict["labels"].graph_pcba_1328 = data_dict["labels"].graph_pcba_1328.astype(np.float32)
-            if hasattr(data_dict["labels"], "graph_pcqm4m_g25"):
-                data_dict["labels"].graph_pcqm4m_g25 = data_dict["labels"].graph_pcqm4m_g25.astype(np.float32)
-            if hasattr(data_dict["labels"], "node_pcqm4m_n4"):
-                data_dict["labels"].node_pcqm4m_n4 = data_dict["labels"].node_pcqm4m_n4.astype(np.float32)
+            # these type changes are necessary for label dtype match of the largmix
+            # if hasattr(data_dict["labels"], "graph_l1000_vcap"):
+            #     data_dict["labels"].graph_l1000_vcap = data_dict["labels"].graph_l1000_vcap.astype(np.float32)
+            # if hasattr(data_dict["labels"], "graph_l1000_mcf7"):
+            #     data_dict["labels"].graph_l1000_mcf7 = data_dict["labels"].graph_l1000_mcf7.astype(np.float32)
+            # if hasattr(data_dict["labels"], "graph_pcba_1328"):
+            #     data_dict["labels"].graph_pcba_1328 = data_dict["labels"].graph_pcba_1328.astype(np.float32)
+            # if hasattr(data_dict["labels"], "graph_pcqm4m_g25"):
+            #     data_dict["labels"].graph_pcqm4m_g25 = data_dict["labels"].graph_pcqm4m_g25.astype(np.float32)
+            # if hasattr(data_dict["labels"], "node_pcqm4m_n4"):
+            #     data_dict["labels"].node_pcqm4m_n4 = data_dict["labels"].node_pcqm4m_n4.astype(np.float32)
             datum["labels"] = data_dict["labels"]
             if "smiles" in data_dict.keys():
                 datum["smiles"] = data_dict["smiles"]
         else:
             if self.mol_ids is not None:
                 datum["mol_ids"] = self.mol_ids[idx]
 
@@ -505,39 +520,62 @@
 
         return all_lists
 
     def _get_inv_of_mol_ids(self, all_mol_ids):
         mol_ids, inv = np.unique(all_mol_ids, return_inverse=True)
         return mol_ids, inv
 
+    def _find_valid_label(self, task, ds):
+        r"""
+        For a given dataset, find a genuine label for that dataset
+        """
+        valid_label = None
+        for i in range(len(ds)):
+            if ds[i] is not None:
+                valid_label = ds[i]["labels"]
+                break
+
+        if valid_label is None:
+            raise ValueError(f"Dataset for task {task} has no valid labels.")
+
+        return valid_label
+
     def set_label_size_dict(self, datasets: Dict[str, SingleTaskDataset]):
         r"""
         This gives the number of labels to predict for a given task.
         """
         task_labels_size = {}
         for task, ds in datasets.items():
             if len(ds) == 0:
                 continue
 
-            valid_label = None
-            for i in range(len(ds)):
-                if ds[i] is not None:
-                    valid_label = ds[i]["labels"]
-                    break
-
-            if valid_label is None:
-                raise ValueError(f"Dataset for task {task} has no valid labels.")
+            valid_label = self._find_valid_label(task, ds)
 
             # Assume for a fixed task, the label dimension is the same across data points
             torch_label = torch.as_tensor(valid_label)
 
             # First dimension is graph-specific
             task_labels_size[task] = torch_label.size()
         return task_labels_size
 
+    def set_label_dtype_dict(self, datasets: Dict[str, SingleTaskDataset]):
+        r"""
+        Gets correct dtype for a given label
+        """
+        task_labels_dtype = {}
+        for task, ds in datasets.items():
+            if len(ds) == 0:
+                continue
+
+            valid_label = self._find_valid_label(task, ds)
+
+            torch_label = torch.as_tensor(valid_label)
+            task_labels_dtype[task] = torch_label.dtype
+        return task_labels_dtype
+
     def __repr__(self) -> str:
         """
         summarizes the dataset in a string
         Returns:
             A string representation of the dataset.
         """
         if len(self) == 0:
@@ -612,14 +650,15 @@
             self.mol_ids, self.smiles, self.labels = self.merge(datasets)
             if self.indexing_same_elem is False:
                 self.mol_ids, self.smiles, self.labels, _ = self.deepcopy_mol(
                     self.mol_ids, self.smiles, self.labels
                 )
 
         self.labels_size = self.set_label_size_dict(datasets)
+        self.labels_dtype = self.set_label_dtype_dict(datasets)
         self.features = self.features
 
     def _get_inv_of_mol_ids(self, all_mol_ids):
         # The generated data is a single molecule duplicated
         mol_ids = np.array(all_mol_ids)
         inv = [_ for _ in range(len(mol_ids) // self.num_datasets)] * self.num_datasets
         mol_ids = np.unique(inv)
```

### Comparing `graphium-2.0.2/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb` & `graphium-2.1.0/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb` & `graphium-2.1.0/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/micro_ZINC/micro_ZINC.csv` & `graphium-2.1.0/graphium/data/micro_ZINC/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/multilevel_utils.py` & `graphium-2.1.0/graphium/data/multilevel_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def unpack_column(data: pd.Series):
         return data.apply(unpack)
 
     def merge_columns(data: pd.Series):
         data = data.to_list()
         data = [np.array([np.nan]) if not isinstance(d, np.ndarray) and math.isnan(d) else d for d in data]
         padded_data = itertools.zip_longest(*data, fillvalue=np.nan)
-        data = np.stack(padded_data, 1).T
+        data = np.stack(list(padded_data), 1).T
         return data
 
     unpacked_df: pd.DataFrame = df[label_cols].apply(unpack_column)
     output = unpacked_df.apply(merge_columns, axis="columns").to_list()
 
     if task_level == "graph":
         return np.concatenate(output)
```

### Comparing `graphium-2.0.2/graphium/data/multitask/tiny_ZINC_SA.csv` & `graphium-2.1.0/graphium/data/multitask/tiny_ZINC_SA.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/multitask/tiny_ZINC_logp.csv` & `graphium-2.1.0/graphium/data/multitask/tiny_ZINC_logp.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/multitask/tiny_ZINC_score.csv` & `graphium-2.1.0/graphium/data/multitask/tiny_ZINC_score.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/normalization.py` & `graphium-2.1.0/graphium/data/normalization.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class LabelNormalization:
     def __init__(
         self,
         method: Optional[str] = None,
         min_clipping: Optional[int] = None,
         max_clipping: Optional[int] = None,
+        normalize_val_test: Optional[bool] = False,
         verbose: Optional[bool] = True,
     ):
         """
         Parameters:
         method: str
             Normalization method. Supports the following values:
             - `None` (default): No normalization applied
@@ -31,14 +32,15 @@
             For example, if `max_clipping` is 2, all values above 2 will be clipped to 2.
             This is applied before the normalization.
         """
 
         self.method = method
         self.min_clipping = min_clipping
         self.max_clipping = max_clipping
+        self.normalize_val_test = normalize_val_test
         self.verbose = verbose
         self.data_max = None
         self.data_min = None
         self.data_mean = None
         self.data_std = None
 
     def calculate_statistics(self, array):
```

### Comparing `graphium-2.0.2/graphium/data/sdf2csv.py` & `graphium-2.1.0/graphium/data/sdf2csv.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/smiles_transform.py` & `graphium-2.1.0/graphium/data/smiles_transform.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/data/utils.py` & `graphium-2.1.0/graphium/data/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,7 +94,14 @@
 
     if extract_zip:
         # Set the destination path to the folder
         # NOTE(hadim): this is a bit fragile.
         dataset_path_destination = dataset_path_destination.split(".")[0]
 
     return dataset_path_destination
+
+
+def get_keys(pyg_data):
+    if isinstance(type(pyg_data).keys, property):
+        return pyg_data.keys
+    else:
+        return pyg_data.keys()
```

### Comparing `graphium-2.0.2/graphium/expts/pyg_batching_sparse.ipynb` & `graphium-2.1.0/graphium/expts/pyg_batching_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/README.md` & `graphium-2.1.0/graphium/features/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/commute.py` & `graphium-2.1.0/graphium/features/commute.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/electrostatic.py` & `graphium-2.1.0/graphium/features/electrostatic.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/featurizer.py` & `graphium-2.1.0/graphium/features/featurizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,14 +882,22 @@
         #     assert key.startswith("edge_"), f"Edge features must start with 'edge_' but got {key}"
         default_dic.update(dic)
         default_dic.update(data)
         # default_dic.update(ndata)
         # default_dic.update(edata)
         super().__init__(default_dic)
 
+    @property
+    def keys(self):
+        return list(super().keys())
+
+    @property
+    def values(self):
+        return list(super().self.values())
+
     def make_pyg_graph(self, **kwargs) -> Data:
         """
         Convert the current dictionary of parameters, containing an adjacency matrix with node/edge data
         into a `pyg.data.Data` of torch Tensors.
 
         `**kwargs` can be used to overwrite any parameter from the current dictionary. See `GraphDict.__init__`
         for a list of parameters
```

### Comparing `graphium-2.0.2/graphium/features/graphormer.py` & `graphium-2.1.0/graphium/features/graphormer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/nmp.py` & `graphium-2.1.0/graphium/features/nmp.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/periodic_table.csv` & `graphium-2.1.0/graphium/features/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/positional_encoding.py` & `graphium-2.1.0/graphium/features/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/properties.py` & `graphium-2.1.0/graphium/features/properties.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/rw.py` & `graphium-2.1.0/graphium/features/rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/spectral.py` & `graphium-2.1.0/graphium/features/spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/test_new_pes.ipynb` & `graphium-2.1.0/graphium/features/test_new_pes.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/features/transfer_pos_level.py` & `graphium-2.1.0/graphium/features/transfer_pos_level.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/ipu/ipu_dataloader.py` & `graphium-2.1.0/graphium/ipu/ipu_dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from loguru import logger
 from torch import Tensor
 
 import torch
 from torch_geometric.data import Data, Batch, Dataset
 from torch_geometric.transforms import BaseTransform
 
+from graphium.data.utils import get_keys
 from graphium.ipu.ipu_utils import import_poptorch
 from graphium.utils.packing import (
     fast_packing,
     hybrid_packing,
     get_pack_sizes,
     node_to_pack_indices_mask,
     estimate_max_pack_node_size,
@@ -151,17 +152,17 @@
             local_batch["features"] = transform(local_batch["features"])
             local_batch["labels"] = transform(local_batch["labels"])
             all_batches.append(local_batch)
 
         out_batch = {}
 
         # Stack tensors in the first dimension to allow IPUs to differentiate between local and global graph
+        all_keys = get_keys(all_batches[0]["labels"])
         out_batch["labels"] = {
-            key: torch.stack([this_batch["labels"][key] for this_batch in all_batches], 0)
-            for key in all_batches[0]["labels"].keys
+            key: torch.stack([this_batch["labels"][key] for this_batch in all_batches], 0) for key in all_keys
         }
         out_graphs = [this_batch["features"] for this_batch in all_batches]
         stacked_features = deepcopy(out_graphs[0])
         for key, val in out_graphs[0].items():
             if isinstance(val, torch.Tensor):
                 stacked_features[key] = torch.stack([this_graph[key] for this_graph in out_graphs], dim=0)
```

### Comparing `graphium-2.0.2/graphium/ipu/ipu_losses.py` & `graphium-2.1.0/graphium/ipu/ipu_losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -103,14 +103,25 @@
         factor2 = torch.where(num_real_targets > 0, 0, 1)
         loss = factor1 * loss * nan_targets.numel() / (num_real_targets + factor2)
 
         return loss
 
 
 class HybridCELossIPU(HybridCELoss):
+    def __init__(
+        self,
+        n_brackets,
+    ) -> None:
+        """
+        Parameters:
+            n_brackets: the number of brackets that will be used to group the regression targets.
+                Expected to have the same size as the number of classes in the transformed regression task.
+        """
+        super().__init__(n_brackets=n_brackets)
+
     def forward(self, input: Tensor, target: Tensor) -> Tensor:
         """
         Parameters:
             input: (batch_size x n_classes) tensor of logits predicted for each bracket.
             target: (batch_size) or (batch_size, 1) tensor of target brackets in {0, 1, ..., self.n_brackets}.
         """
```

### Comparing `graphium-2.0.2/graphium/ipu/ipu_metrics.py` & `graphium-2.1.0/graphium/ipu/ipu_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     return score
 
 
 def average_precision_ipu(
     preds: Tensor,
     target: Tensor,
     num_classes: Optional[int] = None,
-    task: Optional[str] = "multiclass",
+    task: Optional[Literal["binary", "multiclass", "multilabel"]] = None,
     ignore_index: Optional[int] = None,
     pos_label: Optional[int] = None,
     average: Optional[str] = "macro",
     sample_weights: Optional[Sequence] = None,
 ):
     """
     A modified version of the `torchmetrics.functional.average_precision` that can ignore NaNs
```

### Comparing `graphium-2.0.2/graphium/ipu/ipu_simple_lightning.py` & `graphium-2.1.0/graphium/ipu/ipu_simple_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2021 Graphcore Ltd. All rights reserved.
-import pytorch_lightning as pl
-from pytorch_lightning.strategies import IPUStrategy
-from pytorch_lightning.loggers import WandbLogger
+import lightning
+from lightning_graphcore import IPUStrategy
+from lightning.pytorch.loggers import WandbLogger
 
 import torch
 from torch import nn
 
 import torchvision
 import torchvision.transforms as transforms
 
@@ -56,15 +56,15 @@
     def forward(self, x):
         return self.the_network(x)
 
 
 # This class shows a minimal lightning example. This example uses our own
 # SimpleTorchModel which is a basic 2 conv, 2 FC torch network. It can be
 # found in simple_torch_model.py.
-class SimpleLightning(pl.LightningModule):
+class SimpleLightning(lightning.LightningModule):
     def __init__(self, in_dim, hidden_dim, kernel_size, num_classes, on_ipu):
         super().__init__()
         self.model = SimpleTorchModel(
             in_dim=in_dim, hidden_dim=hidden_dim, kernel_size=kernel_size, num_classes=num_classes
         )
         self.on_ipu = on_ipu
 
@@ -140,15 +140,15 @@
 
         # Set the seeds
         training_opts.randomSeed(SEED)
         inference_opts.randomSeed(SEED)
         ipus = 1
         strategy = IPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
 
-    trainer = pl.Trainer(
+    trainer = lightning.Trainer(
         logger=WandbLogger(),
         ipus=ipus,
         max_epochs=3,
         log_every_n_steps=1,
         plugins=plugins,
     )
```

### Comparing `graphium-2.0.2/graphium/ipu/ipu_utils.py` & `graphium-2.1.0/graphium/ipu/ipu_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,17 @@
         The poptorch module
 
     """
     try:
         import poptorch
 
         return poptorch
-    except ImportError:
+    except ImportError as e:
         if raise_error:
-            raise ImportError(
-                "You must install poptorch and have IPU hardware. Check the GraphCore support https://www.graphcore.ai/support"
-            )
+            raise e
         return
 
 
 def is_running_on_ipu() -> bool:
     """
     Returns whether the current module is running on ipu.
     Needs to be used in the `forward` or `backward` pass.
```

### Comparing `graphium-2.0.2/graphium/ipu/ipu_wrapper.py` & `graphium-2.1.0/graphium/ipu/ipu_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 from typing import Dict, Any, Optional, Callable, Union, Type, Tuple, Iterable
 
 from torch_geometric.data import Batch
 from torch import Tensor
-from pytorch_lightning.strategies import IPUStrategy
-from pytorch_lightning.utilities.types import STEP_OUTPUT
-from pytorch_lightning.trainer.states import RunningStage
+from lightning_graphcore import IPUStrategy
+from lightning.pytorch.utilities.types import STEP_OUTPUT
+from lightning.pytorch.trainer.states import RunningStage
 
 from graphium.trainer.predictor import PredictorModule
 from graphium.ipu.ipu_utils import import_poptorch
 
 import torch
 from torch_geometric.data import Data, Batch
 from torch_geometric.data.data import BaseData
 from loguru import logger
 import functools
 import collections
+from graphium.data.utils import get_keys
 
 poptorch = import_poptorch()
 
 
-class DictIPUStrategy(IPUStrategy):
-    def _step(self, stage: RunningStage, *args: Any, **kwargs: Any) -> STEP_OUTPUT:
-        args = self._prepare_input(args)
-        args = args[0]
-        poptorch_model = self.poptorch_models[stage]
-        self.lightning_module._running_torchscript = True
-        out = poptorch_model(**args)
-        self.lightning_module._running_torchscript = False
-        return out
-
-
 class PyGArgsParser(poptorch.ICustomArgParser):
     """
     This class is responsible for converting a PyG Batch from and to
     a tensor of tuples. This allows PyG Batch to be used as inputs to
     IPU programs. Copied from poppyg repo, in the future import from
     the repo directly.
     """
 
     @staticmethod
     def sortedTensorKeys(struct: BaseData) -> Iterable[str]:
         """
         Find all the keys that map to a tensor value in struct. The keys
         are returned in sorted order.
         """
-        all_keys = sorted(struct.keys)
+        all_keys = sorted(get_keys(struct))
 
         def isTensor(k: str) -> bool:
             return isinstance(struct[k], torch.Tensor)
 
         return filter(isTensor, all_keys)
 
     def yieldTensors(self, struct: BaseData):
@@ -64,15 +54,15 @@
         original_structure. This new instance will be initialized with tensors
         from the provided iterator and uses the same sorted keys from the
         yieldTensors() implementation.
         """
         tensor_keys = self.sortedTensorKeys(original_structure)
         kwargs = {k: next(tensor_iterator) for k in tensor_keys}
 
-        for k in original_structure.keys:
+        for k in get_keys(original_structure):
             if k not in kwargs:
                 # copy non-tensor properties to the new instance
                 kwargs[k] = original_structure[k]
 
         cls = original_structure.__class__
 
         if issubclass(cls, Batch):
@@ -110,56 +100,60 @@
         )
 
     def on_train_batch_end(self, outputs, batch, batch_idx):
         outputs = self.convert_from_fp16(outputs)
         outputs["loss"] = outputs["loss"].mean()
         super().on_train_batch_end(outputs, batch, batch_idx)
 
-    def training_step(self, features, labels) -> Dict[str, Any]:
+    def training_step(self, batch, batch_idx) -> Dict[str, Any]:
+        features, labels = batch["features"], batch["labels"]
         features, labels = self.squeeze_input_dims(features, labels)
         dict_input = {"features": features, "labels": labels}
         step_dict = super().training_step(dict_input, to_cpu=False)
 
         loss = step_dict.pop("loss")
         step_dict["loss"] = self.poptorch.identity_loss(loss, reduction="mean")
         return step_dict
 
-    def validation_step(self, features, labels) -> Dict[str, Any]:
+    def validation_step(self, batch, batch_idx) -> Dict[str, Any]:
+        features, labels = batch["features"], batch["labels"]
         features, labels = self.squeeze_input_dims(features, labels)
         dict_input = {"features": features, "labels": labels}
         step_dict = super().validation_step(dict_input, to_cpu=False)
 
         return step_dict
 
-    def test_step(self, features, labels) -> Dict[str, Any]:
+    def test_step(self, batch, batch_idx) -> Dict[str, Any]:
         # Build a dictionary from the tuples
+        features, labels = batch["features"], batch["labels"]
         features, labels = self.squeeze_input_dims(features, labels)
         dict_input = {"features": features, "labels": labels}
         step_dict = super().test_step(dict_input, to_cpu=False)
 
         return step_dict
 
     def predict_step(self, **inputs) -> Dict[str, Any]:
         # Build a dictionary from the tuples
         dict_input = inputs
         step_dict = super().predict_step(dict_input, to_cpu=False)
 
         return step_dict
 
-    def validation_epoch_end(self, outputs: Dict[str, Any]):
+    def on_validation_batch_end(self, outputs: Any, batch: Any, batch_idx: int) -> None:
+        # convert data that will be tracked
         outputs = self.convert_from_fp16(outputs)
-        super().validation_epoch_end(outputs)
+        super().on_validation_batch_end(outputs, batch, batch_idx)
 
-    def evaluation_epoch_end(self, outputs: Dict[str, Any]):
+    def evaluation_epoch_end(self, outputs: Any):
         outputs = self.convert_from_fp16(outputs)
         super().evaluation_epoch_end(outputs)
 
-    def test_epoch_end(self, outputs: Dict[str, Any]):
+    def on_test_batch_end(self, outputs: Any, batch: Any, batch_idx: int) -> None:
         outputs = self.convert_from_fp16(outputs)
-        super().test_epoch_end(outputs)
+        super().on_test_batch_end(outputs, batch, batch_idx)
 
     def configure_optimizers(self, impl=None):
         if impl is None:
             dtype = self.precision_to_dtype(self.trainer.precision)
             impl = functools.partial(
                 self.poptorch.optim.Adam,
                 accum_type=dtype,
@@ -207,15 +201,15 @@
                 if isinstance(val, torch.Tensor) and (val.is_floating_point()):
                     feats[key] = val.to(dtype=dtype)
         else:
             raise ValueError(f"Unsupported feats type `{type(feats)}` : {feats}")
         return feats
 
     def precision_to_dtype(self, precision):
-        return torch.half if precision in (16, "16") else torch.float
+        return torch.half if precision == "16-true" else torch.float
 
     def get_num_graphs(self, data: Batch):
         """
         IPU specific method to compute the number of graphs in a Batch,
         that considers gradient accumulation, multiple IPUs and multiple
         device iterations. Essential to estimate throughput in graphs/s.
         """
```

### Comparing `graphium-2.0.2/graphium/ipu/to_dense_batch.py` & `graphium-2.1.0/graphium/ipu/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/README.md` & `graphium-2.1.0/graphium/nn/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/architectures/encoder_manager.py` & `graphium-2.1.0/graphium/nn/architectures/encoder_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import inspect
 from copy import deepcopy
 
 # Torch imports
 from torch import Tensor, nn
 import torch
 
+from graphium.data.utils import get_keys
 from graphium.nn.encoders import (
     laplace_pos_encoder,
     mlp_encoder,
     signnet_pos_encoder,
     gaussian_kernel_pos_encoder,
 )
 
@@ -165,15 +166,15 @@
         # Apply the positional encoders
         pe_pooled = self.forward_positional_encoding(g)
 
         # Add the processed positional encodings to the graphs.
         # If the key is already present, concatenate the pe_pooled to the pre-existing feature.
         for pe_key, this_pe in pe_pooled.items():
             feat = this_pe
-            if pe_key in g.keys:
+            if pe_key in get_keys(g):
                 feat = torch.cat((feat, g[pe_key]), dim=-1)
             g[pe_key] = feat
         return g
 
     def forward_positional_encoding(self, g: Batch) -> Dict[str, Tensor]:
         """
         Forward pass for the positional encodings (PE),
```

### Comparing `graphium-2.0.2/graphium/nn/architectures/global_architectures.py` & `graphium-2.1.0/graphium/nn/architectures/global_architectures.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # Torch imports
 from torch import Tensor, nn
 import torch
 from torch_geometric.data import Data
 
 # graphium imports
+from graphium.data.utils import get_keys
 from graphium.nn.base_layers import FCLayer, get_activation, get_norm
 from graphium.nn.architectures.encoder_manager import EncoderManager
 from graphium.nn.pyg_layers import VirtualNodePyg, parse_pooling_layer_pyg
 from graphium.nn.base_graph_layer import BaseGraphModule, BaseGraphStructure
 from graphium.nn.residual_connections import (
     ResidualConnectionBase,
     ResidualConnectionWeighted,
@@ -1148,15 +1149,16 @@
         """
 
         # Apply the positional encoders
         g = self.encoder_manager(g)
 
         g["feat"] = g["feat"]
         e = None
-        if "edge_feat" in g.keys:
+
+        if "edge_feat" in get_keys(g):
             g["edge_feat"] = g["edge_feat"]
 
         # Run the pre-processing network on node features
         if self.pre_nn is not None:
             g["feat"] = self.pre_nn.forward(g["feat"])
 
         # Run the pre-processing network on edge features
```

### Comparing `graphium-2.0.2/graphium/nn/architectures/pyg_architectures.py` & `graphium-2.1.0/graphium/nn/architectures/pyg_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/base_graph_layer.py` & `graphium-2.1.0/graphium/nn/base_graph_layer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/base_layers.py` & `graphium-2.1.0/graphium/nn/base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/README.md` & `graphium-2.1.0/graphium/nn/encoders/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/base_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/bessel_pos_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/bessel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/gaussian_kernel_pos_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/gaussian_kernel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/laplace_pos_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/laplace_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/mlp_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/mlp_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/encoders/signnet_pos_encoder.py` & `graphium-2.1.0/graphium/nn/encoders/signnet_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/README.md` & `graphium-2.1.0/graphium/nn/pyg_layers/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/dimenet_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/dimenet_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/gated_gcn_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/gated_gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/gcn_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/gin_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/gin_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/gps_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/gps_pyg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from graphium.nn.pyg_layers import (
     GatedGCNPyg,
     GINConvPyg,
     GINEConvPyg,
     PNAMessagePassingPyg,
     MPNNPlusPyg,
 )
+from graphium.data.utils import get_keys
 from graphium.utils.decorators import classproperty
 from graphium.ipu.to_dense_batch import (
     to_dense_batch,
     to_sparse_batch,
     to_packed_dense_batch,
     to_sparse_batch_from_packed,
 )
@@ -285,15 +286,16 @@
             attn_layer = attn_class(biased_attention_key, **attn_kwargs)
         return attn_layer
 
     def _use_packing(self, batch: Batch) -> bool:
         """
         Check if we should use packing for the batch of graphs.
         """
-        return "pack_from_node_idx" in batch.keys and "pack_attn_mask" in batch.keys
+        batch_keys = get_keys(batch)
+        return "pack_from_node_idx" in batch_keys and "pack_attn_mask" in batch_keys
 
     def _to_dense_batch(
         self,
         h: Tensor,
         batch: Batch,
         batch_size: Optional[int] = None,
         max_num_nodes_per_graph: Optional[int] = None,
```

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/mpnn_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/mpnn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/pna_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/pna_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/pooling_pyg.py` & `graphium-2.1.0/graphium/nn/pyg_layers/pooling_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/pyg_layers/utils.py` & `graphium-2.1.0/graphium/nn/pyg_layers/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/residual_connections.py` & `graphium-2.1.0/graphium/nn/residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/nn/utils.py` & `graphium-2.1.0/graphium/nn/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/trainer/losses.py` & `graphium-2.1.0/graphium/trainer/losses.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,23 +46,28 @@
             )
 
         if alpha < 0 or alpha > 1:
             raise ValueError(f"Expected alpha to be in the [0, 1] range, received {alpha}.")
 
         self.brackets = Tensor(range(n_brackets))
         self.alpha = alpha
+        self.softmax = torch.nn.Softmax(dim=1)
 
     def forward(self, input: Tensor, target: Tensor) -> Tensor:
         """
         Parameters:
             input: (batch_size x n_classes) tensor of logits predicted for each bracket.
             target: (batch_size) or (batch_size, 1) tensor of target brackets in {0, 1, ..., self.n_brackets}.
         """
 
         target = target.flatten()
-
-        regression_input = torch.inner(input, self.brackets.to(input.device))
+        # regression loss needs normalized logits to probability as input to do inner product with self.brackets
+        # we apply softmax on the raw logits first
+        softmax_input = self.softmax(input)
+        # [batch_size, n_classes] * [n_classes] ([0, 1, 2...n_brakets-1]) -> [batch_size]
+        regression_input = torch.inner(softmax_input, self.brackets.to(input.device))
         regression_loss = self.regression_loss(regression_input, target.float(), reduction=self.reduction)
 
+        # cross_entropy loss needs raw logits as input
         ce_loss = F.cross_entropy(input, target.long(), weight=self.weight, reduction=self.reduction)
 
         return self.alpha * ce_loss + (1 - self.alpha) * regression_loss
```

### Comparing `graphium-2.0.2/graphium/trainer/metrics.py` & `graphium-2.1.0/graphium/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/trainer/predictor.py` & `graphium-2.1.0/graphium/trainer/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import numpy as np
 from copy import deepcopy
 import time
 from loguru import logger
 
 import torch
 from torch import nn, Tensor
-import pytorch_lightning as pl
+import lightning
 from torch_geometric.data import Data, Batch
 from mup.optim import MuAdam
 
 from graphium.config.config_convert import recursive_config_reformating
 from graphium.trainer.predictor_options import EvalOptions, FlagOptions, ModelOptions, OptimOptions
 from graphium.trainer.predictor_summaries import TaskSummaries
 from graphium.data.datamodule import BaseDataModule
 from graphium.utils.moving_average_tracker import MovingAverageTracker
 
 GRAPHIUM_PRETRAINED_MODELS = {
     "graphium-zinc-micro-dummy-test": "gcs://graphium-public/pretrained-models/graphium-zinc-micro-dummy-test/model.ckpt"
 }
 
 
-class PredictorModule(pl.LightningModule):
+class PredictorModule(lightning.LightningModule):
     def __init__(
         self,
         model_class: Type[nn.Module],
         model_kwargs: Dict[str, Any],
         loss_fun: Dict[str, Union[str, Callable]],
         random_seed: int = 42,
         optim_kwargs: Optional[Dict[str, Any]] = None,
@@ -154,14 +154,16 @@
 
         # This helps avoid a bug when saving hparams to yaml with different dict or str formats
         self._set_hparams(recursive_config_reformating(self.hparams))
 
         # throughput estimation
         self.mean_val_time_tracker = MovingAverageTracker()
         self.mean_val_tput_tracker = MovingAverageTracker()
+        self.validation_step_outputs = []
+        self.test_step_outputs = []
         self.epoch_start_time = None
 
     def forward(
         self, inputs: Dict
     ) -> Dict[str, Union[Tensor, Dict[str, Tensor], Dict[str, Dict[str, Tensor]]]]:
         r"""
         Returns the result of `self.model.forward(*inputs)` on the inputs.
@@ -307,18 +309,22 @@
                 task_level=self.model_kwargs["task_heads_kwargs"][key]["task_level"], task=key
             ): value
             for key, value in preds.items()
         }
         # preds = {k: preds[ii] for ii, k in enumerate(targets_dict.keys())}
         for task, pred in preds.items():
             task_specific_norm = self.task_norms[task] if self.task_norms is not None else None
-            if step_name != "train":
+            if hasattr(task_specific_norm, "normalize_val_test"):
+                normalize_val_test = task_specific_norm.normalize_val_test
+            else:
+                normalize_val_test = False
+            if step_name != "train" and not normalize_val_test:
                 # apply denormalization for val and test predictions for correct loss and metrics evaluation
-                # targets for val and test were not normalized
-                # train loss will stay as the normalized version
+                # if normalize_val_test is not true, only train loss will stay as the normalized version
+                # if normalize_val_test is true, no denormalization is applied, all losses and metrics are normalized version
                 preds[task] = task_specific_norm.denormalize(pred)
             targets_dict[task] = targets_dict[task].to(dtype=pred.dtype)
         weights = batch.get("weights", None)
 
         loss, task_losses = self.compute_loss(
             preds=preds,
             targets=targets_dict,
@@ -327,17 +333,22 @@
             target_nan_mask=self.target_nan_mask,
             multitask_handling=self.multitask_handling,
         )
 
         device = "cpu" if to_cpu else None
         for task in preds:
             task_specific_norm = self.task_norms[task] if self.task_norms is not None else None
-            if step_name == "train":
-                # apply denormalization for targets and predictions for the evaluation of metrics (excluding loss)
-                # train loss will stay as the normalized version
+            if hasattr(task_specific_norm, "normalize_val_test"):
+                normalize_val_test = task_specific_norm.normalize_val_test
+            else:
+                normalize_val_test = False
+            if step_name == "train" and not normalize_val_test:
+                # apply denormalization for targets and predictions for the evaluation of training metrics (excluding loss)
+                # if normalize_val_test is not true, train loss will stay as the normalized version
+                # if normalize_val_test is true, no denormalization is applied, all losses and metrics are normalized version
                 preds[task] = task_specific_norm.denormalize(preds[task])
                 targets_dict[task] = task_specific_norm.denormalize(targets_dict[task])
             preds[task] = preds[task].detach().to(device=device)
             targets_dict[task] = targets_dict[task].detach().to(device=device)
         if weights is not None:
             weights = weights.detach().to(device=device)
 
@@ -444,21 +455,26 @@
             task_losses=outputs["task_losses"],
             n_epochs=self.current_epoch,
         )
         metrics_logs = self.task_epoch_summary.get_metrics_logs()  # Dict[task, metric_logs]
         metrics_logs["_global"]["grad_norm"] = self.get_gradient_norm()
         outputs.update(metrics_logs)  # Dict[task, metric_logs]. Concatenate them?
 
-        concatenated_metrics_logs = self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
+        concatenated_metrics_logs = {}  # self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
         concatenated_metrics_logs["loss"] = outputs["loss"]
         outputs["grad_norm"] = self.get_gradient_norm()
         concatenated_metrics_logs["train/grad_norm"] = outputs["grad_norm"]
         concatenated_metrics_logs["train/batch_time"] = train_batch_time
         concatenated_metrics_logs["train/batch_tput"] = tput
 
+        for key in concatenated_metrics_logs:
+            if isinstance(concatenated_metrics_logs[key], torch.Tensor):
+                if concatenated_metrics_logs[key].numel() > 1:
+                    concatenated_metrics_logs[key] = concatenated_metrics_logs[key].mean()
+
         if self.logger is not None:
             self.logger.log_metrics(
                 concatenated_metrics_logs, step=self.global_step
             )  # This is a pytorch lightning function call
 
     def training_step(self, batch: Dict[str, Tensor], to_cpu: bool = True) -> Dict[str, Any]:
         step_dict = None
@@ -532,55 +548,54 @@
         if self.epoch_start_time is None:
             logger.warning("epoch timer not initialized")
         else:
             epoch_time = time.time() - self.epoch_start_time
             self.epoch_start_time = None
             self.log("epoch_time", torch.tensor(epoch_time))
 
-    def training_epoch_end(self, outputs: Dict):
-        """
-        Nothing happens at the end of the training epoch.
-        It serves no purpose to do a general step for the training,
-        but it can explode the RAM when using a large dataset.
-        """
-        pass
-
     def on_validation_epoch_start(self) -> None:
         self.mean_val_time_tracker.reset()
         self.mean_val_tput_tracker.reset()
         return super().on_validation_epoch_start()
 
-    def on_validation_batch_start(self, batch: Any, batch_idx: int, dataloader_idx: int) -> None:
+    def on_validation_batch_start(self, batch: Any, batch_idx: int) -> None:
         self.validation_batch_start_time = time.time()
-        return super().on_validation_batch_start(batch, batch_idx, dataloader_idx)
+        return super().on_validation_batch_start(batch, batch_idx)
 
-    def on_validation_batch_end(self, outputs, batch: Any, batch_idx: int, dataloader_idx: int) -> None:
+    def on_validation_batch_end(self, outputs: Any, batch: Any, batch_idx: int) -> None:
         val_batch_time = time.time() - self.validation_batch_start_time
+        self.validation_step_outputs.append(outputs)
         self.mean_val_time_tracker.update(val_batch_time)
         num_graphs = self.get_num_graphs(batch["features"])
         self.mean_val_tput_tracker.update(num_graphs / val_batch_time)
-        return super().on_validation_batch_end(outputs, batch, batch_idx, dataloader_idx)
+        return super().on_validation_batch_end(outputs, batch, batch_idx)
 
-    def validation_epoch_end(self, outputs: Dict[str, Any]):
-        metrics_logs = self._general_epoch_end(outputs=outputs, step_name="val")
+    def on_validation_epoch_end(self) -> None:
+        metrics_logs = self._general_epoch_end(outputs=self.validation_step_outputs, step_name="val")
+        self.validation_step_outputs.clear()
         concatenated_metrics_logs = self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
-        concatenated_metrics_logs["val/mean_time"] = self.mean_val_time_tracker.mean_value
+        concatenated_metrics_logs["val/mean_time"] = torch.tensor(self.mean_val_time_tracker.mean_value)
         concatenated_metrics_logs["val/mean_tput"] = self.mean_val_tput_tracker.mean_value
 
-        lr = self.optimizers().param_groups[0]["lr"]
-        concatenated_metrics_logs["lr"] = lr
-        concatenated_metrics_logs["n_epochs"] = self.current_epoch
+        if hasattr(self.optimizers(), "param_groups"):
+            lr = self.optimizers().param_groups[0]["lr"]
+            concatenated_metrics_logs["lr"] = torch.tensor(lr)
+        concatenated_metrics_logs["n_epochs"] = torch.tensor(self.current_epoch, dtype=torch.float32)
         self.log_dict(concatenated_metrics_logs)
 
         # Save yaml file with the per-task metrics summaries
         full_dict = {}
         full_dict.update(self.task_epoch_summary.get_dict_summary())
 
-    def test_epoch_end(self, outputs: Dict[str, Any]):
-        metrics_logs = self._general_epoch_end(outputs=outputs, step_name="test")
+    def on_test_batch_end(self, outputs: Any, batch: Any, batch_idx: int) -> None:
+        self.test_step_outputs.append(outputs)
+
+    def on_test_epoch_end(self) -> None:
+        metrics_logs = self._general_epoch_end(outputs=self.test_step_outputs, step_name="test")
+        self.test_step_outputs.clear()
         concatenated_metrics_logs = self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
 
         self.log_dict(concatenated_metrics_logs)
 
         # Save yaml file with the per-task metrics summaries
         full_dict = {}
         full_dict.update(self.task_epoch_summary.get_dict_summary())
```

### Comparing `graphium-2.0.2/graphium/trainer/predictor_options.py` & `graphium-2.1.0/graphium/trainer/predictor_options.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/trainer/predictor_summaries.py` & `graphium-2.1.0/graphium/trainer/predictor_summaries.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/arg_checker.py` & `graphium-2.1.0/graphium/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/command_line_utils.py` & `graphium-2.1.0/graphium/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/custom_lr.py` & `graphium-2.1.0/graphium/utils/custom_lr.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/dict_tensor.py` & `graphium-2.1.0/graphium/utils/dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/fs.py` & `graphium-2.1.0/graphium/utils/fs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/mup.py` & `graphium-2.1.0/graphium/utils/mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/packing.py` & `graphium-2.1.0/graphium/utils/packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/read_file.py` & `graphium-2.1.0/graphium/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/safe_run.py` & `graphium-2.1.0/graphium/utils/safe_run.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/spaces.py` & `graphium-2.1.0/graphium/utils/spaces.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/utils/tensor.py` & `graphium-2.1.0/graphium/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium/visualization/vis_utils.py` & `graphium-2.1.0/graphium/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/graphium.egg-info/PKG-INFO` & `graphium-2.1.0/graphium.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.0.2
+Version: 2.1.0
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,33 +27,38 @@
 
 <div align="center">
     <img src="docs/images/logo.png" height="200px">
     <h3>Scaling molecular GNNs to infinity</h3>
 </div>
 
 ---
-
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
 
+
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
 - ⮔ Read-to-use training loop based on [Pytorch Lightning](https://www.pytorchlightning.ai/).
 - 🔌 Have a new dataset? Graphium provides a simple plug-and-play interface. Change the path, the name of the columns to predict, the atomic featurization, and you’re ready to play!
 
 ## Documentation
 
 Visit https://graphium-docs.datamol.io/.
 
+[![Run on Gradient](https://assets.paperspace.io/img/gradient-badge.svg)](https://ipu.dev/sdGggS)
+
+You can try running Graphium on Graphcore IPUs for free on Gradient by clicking on the button above.
+
 ## Installation for developers
 
 ### For CPU and GPU developers
 
 Use [`mamba`](https://github.com/mamba-org/mamba):
 
 ```bash
@@ -68,22 +73,23 @@
 ### For IPU developers
 
 ```bash
 mkdir ~/.venv                               # Create the folder for the environment
 python3 -m venv ~/.venv/graphium_ipu        # Create the environment
 source ~/.venv/graphium_ipu/bin/activate    # Activate the environment
 
-# Installing the poptorch SDK. Make sure to change the path
+# Install the PopTorch wheel
 pip install PATH_TO_SDK/poptorch-3.2.0+109946_bb50ce43ab_ubuntu_20_04-cp38-cp38-linux_x86_64.whl
 
-# Activate poplar SDK.
+# Enable Poplar SDK (including Poplar and PopART)
 source PATH_TO_SDK/enable
 
 # Install the IPU specific and graphium requirements
 PACKAGE_NAME=pytorch pip install -r requirements_ipu.txt
+pip install -r lightning.txt
 
 # Install Graphium in dev mode
 pip install --no-deps -e .
 ```
 
 ## Training a model
```

### Comparing `graphium-2.0.2/graphium.egg-info/SOURCES.txt` & `graphium-2.1.0/graphium.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 LICENSE
 README.md
 cleanup_files.sh
 env.yml
+lightning.txt
 mkdocs.yml
 pyproject.toml
 requirements_ipu.txt
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/code-check.yml
@@ -41,44 +42,63 @@
 docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
 docs/tutorials/feature_processing/choosing_parallelization.ipynb
 docs/tutorials/feature_processing/csv_to_parquet.ipynb
 docs/tutorials/feature_processing/timing_parallel.ipynb
 docs/tutorials/gnn/add_new_gnn_layers.ipynb
 docs/tutorials/gnn/making_gnn_networks.ipynb
 docs/tutorials/gnn/using_gnn_layers.ipynb
-docs/tutorials/model_training/config_ipu_tutorials.yaml
-docs/tutorials/model_training/ipu_training.ipynb
-docs/tutorials/model_training/ipu_training_demo.py
+docs/tutorials/model_training/running-multitask-ipu.ipynb
 docs/tutorials/model_training/simple-molecular-model.ipynb
 expts/dataset_benchmark.py
 expts/main_run_get_fingerprints.py
 expts/main_run_multitask.py
 expts/main_run_predict.py
 expts/main_run_test.py
+expts/run_validation_test.py
 expts/test_yaml.py
 expts/configs/config_gps_10M_pcqm4m.yaml
 expts/configs/config_gps_10M_pcqm4m_mod.yaml
 expts/configs/config_gpspp_10M_pcqm4m.yaml
 expts/configs/config_mpnn_10M_b3lyp.yaml
 expts/configs/config_mpnn_10M_pcqm4m.yaml
 expts/configs/config_mpnn_pcqm4m.yaml
 expts/data/micro_zinc_splits.csv
 expts/data/tiny_zinc_splits.csv
 expts/neurips2023_configs/config_classifigression_l1000.yaml
-expts/neurips2023_configs/config_debug.yaml
 expts/neurips2023_configs/config_large_gcn.yaml
 expts/neurips2023_configs/config_large_gin.yaml
 expts/neurips2023_configs/config_large_gine.yaml
 expts/neurips2023_configs/config_large_mpnn.yaml
 expts/neurips2023_configs/config_luis_jama.yaml
 expts/neurips2023_configs/config_small_gated_gcn.yaml
 expts/neurips2023_configs/config_small_gcn.yaml
 expts/neurips2023_configs/config_small_gin.yaml
 expts/neurips2023_configs/config_small_gine.yaml
 expts/neurips2023_configs/config_small_mpnn.yaml
+expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
+expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
+expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
+expts/neurips2023_configs/debug/config_debug.yaml
+expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
+expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
+expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
+expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
+expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
+expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
+expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
 graphium/__init__.py
 graphium/_version.py
 graphium.egg-info/PKG-INFO
 graphium.egg-info/SOURCES.txt
 graphium.egg-info/dependency_links.txt
 graphium.egg-info/entry_points.txt
 graphium.egg-info/requires.txt
```

### Comparing `graphium-2.0.2/mkdocs.yml` & `graphium-2.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/notebooks/dev-datamodule-invalidate-cache.ipynb` & `graphium-2.1.0/notebooks/dev-datamodule-invalidate-cache.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998015873015873%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(8, 'import lightning\\n')], delete: [8]}}}"}*

```diff
@@ -18,15 +18,15 @@
                 "%autoreload 2\n",
                 "\n",
                 "import pathlib\n",
                 "import functools\n",
                 "import tempfile\n",
                 "\n",
                 "import numpy as np\n",
-                "import pytorch_lightning as pl\n",
+                "import lightning\n",
                 "import torch\n",
                 "import datamol as dm\n",
                 "\n",
                 "import graphium"
             ]
         },
         {
```

### Comparing `graphium-2.0.2/notebooks/dev-datamodule-ogb.ipynb` & `graphium-2.1.0/notebooks/dev-datamodule-ogb.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958984375%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'source': {insert: [(10, 'import "*

 * *            "lightning\\n')], delete: [10]}}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```yaml\n",
                 "data:\n",
                 "  module_type: \"GraphOGBDataModule\"\n",
                 "  args:\n",
@@ -45,15 +46,15 @@
                 "import pathlib\n",
                 "import functools\n",
                 "import tempfile\n",
                 "import importlib\n",
                 "\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
-                "import pytorch_lightning as pl\n",
+                "import lightning\n",
                 "import torch\n",
                 "import datamol as dm\n",
                 "\n",
                 "import graphium"
             ]
         },
         {
```

### Comparing `graphium-2.0.2/notebooks/dev-datamodule.ipynb` & `graphium-2.1.0/notebooks/dev-datamodule.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944940476190476%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(8, 'import lightning\\n')], delete: [8]}}, 4: "*

 * *            "{'attachments': OrderedDict()}}"}*

```diff
@@ -20,15 +20,15 @@
                 "%autoreload 2\n",
                 "\n",
                 "import pathlib\n",
                 "import functools\n",
                 "import tempfile\n",
                 "\n",
                 "import numpy as np\n",
-                "import pytorch_lightning as pl\n",
+                "import lightning\n",
                 "import torch\n",
                 "import datamol as dm\n",
                 "\n",
                 "import graphium"
             ]
         },
         {
@@ -173,14 +173,15 @@
                 "dl = dm.train_dataloader()\n",
                 "it = iter(dl)\n",
                 "batch = next(it)\n",
                 "batch"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "---\n",
                 "\n",
                 "## Launch a training\n",
                 "\n",
```

### Comparing `graphium-2.0.2/notebooks/dev-pretrained.ipynb` & `graphium-2.1.0/notebooks/dev-pretrained.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949926900584796%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(11, 'import lightning\\n')], delete: [11]}}, 1: "*

 * *            "{'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, 11: "*

 * *            "{'attachments': OrderedDict()}}"}*

```diff
@@ -21,23 +21,24 @@
                 "import functools\n",
                 "import tempfile\n",
                 "import yaml\n",
                 "\n",
                 "from loguru import logger\n",
                 "\n",
                 "import numpy as np\n",
-                "import pytorch_lightning as pl\n",
+                "import lightning\n",
                 "import torch\n",
                 "import datamol as dm\n",
                 "import pandas as pd\n",
                 "\n",
                 "import graphium"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Training"
             ]
         },
         {
@@ -208,14 +209,15 @@
             ],
             "source": [
                 "# Training\n",
                 "trainer.fit(model=predictor, datamodule=datamodule)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Load pretrained (hard coded path)"
             ]
         },
         {
@@ -315,14 +317,15 @@
                 "predictor = graphium.trainer.predictor.PredictorModule.load_from_checkpoint(model_path)\n",
                 "\n",
                 "# Inference\n",
                 "results = trainer.predict(predictor, datamodule=datamodule, return_predictions=True)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Load pretrained (from graphium available models)"
             ]
         },
         {
```

### Comparing `graphium-2.0.2/notebooks/dev-training-loop.ipynb` & `graphium-2.1.0/notebooks/dev-training-loop.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/notebooks/dev.ipynb` & `graphium-2.1.0/notebooks/dev.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(11, 'import lightning\\n')], delete: [11]}}}"}*

```diff
@@ -21,15 +21,15 @@
                 "import functools\n",
                 "import tempfile\n",
                 "import yaml\n",
                 "\n",
                 "from loguru import logger\n",
                 "\n",
                 "import numpy as np\n",
-                "import pytorch_lightning as pl\n",
+                "import lightning\n",
                 "import torch\n",
                 "import datamol as dm\n",
                 "import pandas as pd\n",
                 "\n",
                 "import graphium"
             ]
         },
```

### Comparing `graphium-2.0.2/notebooks/running-fingerprints-from-pretrained-model.ipynb` & `graphium-2.1.0/notebooks/running-fingerprints-from-pretrained-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/notebooks/running-model-from-config.ipynb` & `graphium-2.1.0/notebooks/running-model-from-config.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/profiling/configs_profiling.yaml` & `graphium-2.1.0/profiling/configs_profiling.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/profiling/profile_mol_to_graph.py` & `graphium-2.1.0/profiling/profile_mol_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/profiling/profile_predictor.py` & `graphium-2.1.0/profiling/profile_predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from graphium.config._loader import (
     load_datamodule,
     load_metrics,
     load_trainer,
     load_predictor,
     load_architecture,
 )
-from pytorch_lightning import Trainer
+from lightning import Trainer
 
 
 def main():
     CONFIG_PATH = "expts/config_micro-PCBA.yaml"
     # DATA_PATH = "https://storage.googleapis.com/graphium-public/datasets/graphium-zinc-bench-gnn/smiles_score.csv.gz"
 
     with fsspec.open(CONFIG_PATH, "r") as f:
```

### Comparing `graphium-2.0.2/pyproject.toml` & `graphium-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "seaborn",
     # cloud IO
     "fsspec >=2021.6",
     "s3fs >=2021.6",
     "gcsfs >=2021.6",
     "platformdirs",
     # ML packages
-    "pytorch-lightning >=1.9",
+    "pytorch-lightning >=2.0",
     "torchmetrics >=0.7.0,<0.11",
     "ogb",
     "torch-geometric >=2.0",
     "wandb",
     "mup",
     "torch_sparse >=0.6",
     "torch_cluster >=1.5",
```

### Comparing `graphium-2.0.2/scripts/convert_yml.py` & `graphium-2.1.0/scripts/convert_yml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/scripts/ipu_venv.sh` & `graphium-2.1.0/scripts/ipu_venv.sh`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/config_test_ipu_dataloader.yaml` & `graphium-2.1.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,300 +1,255 @@
-# Testing the multitask pipeline with the QM9 dataset on IPU, by splitting it up into three tasks: homo, alpha and cv.
+# Testing the gcn model
 constants:
-  name: &name test_ipu #qm9_full
+  name: &name neurips2023_large_data_gcn_pcba
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 20 # train max nodes: 20, max_edges: 54
-          max_num_edges_per_graph: 60
+          max_num_nodes_per_graph: 60 # train max nodes: 20, max_edges: 54
+          max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 16 # valid max nodes: 51, max_edges: 118
-          max_num_edges_per_graph: 120
+          max_num_nodes_per_graph: 200 # valid max nodes: 51, max_edges: 118
+          max_num_edges_per_graph: 400
         # Data handling-related
-        batch_size_training: 6
-        batch_size_inference: 6
+        batch_size_training: 10
+        batch_size_inference: 2
+    predictor:
+      optim_kwargs:
+        loss_scaling: 1024
     trainer:
       trainer:
-        precision: 16
-        accumulate_grad_batches: 4
+        precision: 32
+        accumulate_grad_batches: 8
 
   ipu_config:
-    - deviceIterations(2)
+    - deviceIterations(10) # IPU would require large batches to be ready for the model.
+    - replicationFactor(16)
+    # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
+    # - enableExecutableCaching("pop_compiler_cache")
+    - TensorLocations.numIOTiles(128)
+    - _Popart.set("defaultBufferingDepth", 128)
+    - Precision.enableStochasticRounding(True)
+
+# accelerator:
+#   type: cpu  # cpu or ipu or gpu
+#   config_override:
+#     datamodule:
+#       batch_size_training: 64
+#       batch_size_inference: 256
+#     trainer:
+#       trainer:
+#         precision: 32
+#         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
+  # module_type: "FakeDataModule"  # Option to use generated data
   args: # Matches that in the test_multitask_datamodule.py case.
     task_specific_args:   # To be replaced by a new class "DatasetParams"
-      homo:
+      pcba_1328:
         df: null
-        df_path: &df_path https://storage.googleapis.com/datasets-public-research/PCQM4M/cxsmiles/pcqm4mv2-2k-lumo-alpha.csv
-        smiles_col: "cxsmiles"
-        label_cols: ["homo_lumo_gap", "lumo"]
-        split_val: 0.2
-        split_test: 0.2
-        seed: *seed
-        splits_path: null                 # This may not always be provided
-        sample_size: null                 # This may not always be provided
-        idx_col: null                     # This may not always be provided
-        weights_col: null                 # This may not always be provided
-        weights_type: null                # This may not always be provided
-      alpha:
-        df: null
-        df_path: *df_path
-        smiles_col: "cxsmiles"
-        label_cols: ["alpha"]
-        split_val: 0.2
-        split_test: 0.2
-        seed: *seed
-        splits_path: null                 # This may not always be provided
-        sample_size: null                 # This may not always be provided
-        idx_col: null                     # This may not always be provided
-        weights_col: null                 # This may not always be provided
-        weights_type: null                # This may not always be provided
+        df_path: graphium/data/neurips2023/large-dataset/PCBA_1328_1564k.parquet
+        # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCBA_1328_1564k.parquet
+        # or set path as the URL directly
+        smiles_col: "SMILES"
+        label_cols: assayID-*  # assayID-* means all columns starting with "assayID-"
+        # sample_size: 2000 # use sample_size for test
+        task_level: graph
+        splits_path: graphium/data/neurips2023/large-dataset/pcba_1328_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcba_1328_random_splits.pt`
+
     # Featurization
     prepare_dict_or_graph: pyg:graph
-    featurization_n_jobs: 0
+    featurization_n_jobs: 30
     featurization_progress: True
+    featurization_backend: "loky"
+    processed_graph_data_path: "../datacache/neurips2023-large/pcba/"
     featurization:
-      atom_property_list_onehot: [atomic-number, valence]
-      atom_property_list_float: [mass, electronegativity, in-ring]
+    # OGB: ['atomic_num', 'degree', 'possible_formal_charge', 'possible_numH' (total-valence),
+    # 'possible_number_radical_e', 'possible_is_aromatic', 'possible_is_in_ring',
+    # 'num_chiral_centers (not included yet)']
+      atom_property_list_onehot: [atomic-number, group, period, total-valence]
+      atom_property_list_float: [degree, formal-charge, radical-electron, aromatic, in-ring]
+      # OGB: ['possible_bond_type', 'possible_bond_stereo', 'possible_is_in_ring']
       edge_property_list: [bond-type-onehot, stereo, in-ring]
-      conformer_property_list: [positions_3d]
       add_self_loop: False
-      explicit_H: False
+      explicit_H: False # if H is included
       use_bonds_weights: False
       pos_encoding_as_features: # encoder dropout 0.18
         pos_types:
-          node_laplacian_eigvec:
+          lap_eigvec:
+            pos_level: node
             pos_type: laplacian_eigvec
+            num_pos: 8
+            normalization: "none" # nomrlization already applied on the eigen vectors
+            disconnected_comp: True # if eigen values/vector for disconnected graph are included
+          lap_eigval:
             pos_level: node
-            num_pos: 5
-            normalization: "none"
-            disconnected_comp: True
-          node_laplacian_eigval:
             pos_type: laplacian_eigval
+            num_pos: 8
+            normalization: "none" # nomrlization already applied on the eigen vectors
+            disconnected_comp: True # if eigen values/vector for disconnected graph are included
+          rw_pos: # use same name as pe_encoder
             pos_level: node
-            num_pos: 5
-            normalization: "none"
-            disconnected_comp: True
-          rw_return_probs:
             pos_type: rw_return_probs
-            pos_level: node
-            ksteps: [4, 8]
-          edge_rw_transition_probs:
-            pos_type: rw_transition_probs
-            pos_level: edge
-            ksteps: [2, 4]
-          nodepair_rw_return_probs:
-            pos_type: rw_return_probs
-            pos_level: nodepair
-            ksteps: [4]
-          electrostatic:
-            pos_type: electrostatic
-            pos_level: node
-          edge_commute:
-            pos_type: commute
-            pos_level: edge
-          nodepair_graphormer:
-            pos_type: graphormer
-            pos_level: nodepair
+            ksteps: 16
+
+    # cache_data_path: .
+    num_workers: 30 # -1 to use all
+    persistent_workers: False # if use persistent worker at the start of each epoch.
+    # Using persistent_workers false might make the start of each epoch very long.
+    featurization_backend: "loky"
 
-    num_workers: -1
 
 architecture:
   model_type: FullGraphMultiTaskNetwork
   mup_base_path: null
-
   pre_nn:   # Set as null to avoid a pre-nn network
-    out_dim: 16
-    hidden_dims: 16
-    depth: 1
+    out_dim: 64
+    hidden_dims: 256
+    depth: 2
     activation: relu
     last_activation: none
-    dropout: &dropout 0.1
-    normalization: &normalization batch_norm
+    dropout: &dropout 0.18
+    normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
-  pre_nn_edges:   # Set as null to avoid a pre-nn network
-    out_dim: 16
-    hidden_dims: 16
-    depth: 1
-    activation: relu
-    last_activation: none
-    dropout: *dropout
-    normalization: *normalization
-    last_normalization: *normalization
-    residual_type: none
+  pre_nn_edges: null
 
   pe_encoders:
-    out_dim: &pe_out_dim 16
-    edge_out_dim: &edge_pe_out_dim 8
+    out_dim: 32
     pool: "sum" #"mean" "max"
     last_norm: None #"batch_norm", "layer_norm"
-    max_num_nodes_per_graph: 30
-    encoders:
-      emb_la_pos:
+    encoders: #la_pos |  rw_pos
+      la_pos:  # Set as null to avoid a pre-nn network
         encoder_type: "laplacian_pe"
         input_keys: ["laplacian_eigvec", "laplacian_eigval"]
         output_keys: ["feat"]
-        hidden_dim: 32
+        hidden_dim: 64
+        out_dim: 32
         model_type: 'DeepSet' #'Transformer' or 'DeepSet'
         num_layers: 2
         num_layers_post: 1 # Num. layers to apply after pooling
         dropout: 0.1
         first_normalization: "none" #"batch_norm" or "layer_norm"
-      emb_rwse:
+      rw_pos:
         encoder_type: "mlp"
         input_keys: ["rw_return_probs"]
         output_keys: ["feat"]
-        hidden_dim: 32
+        hidden_dim: 64
+        out_dim: 32
         num_layers: 2
         dropout: 0.1
         normalization: "layer_norm" #"batch_norm" or "layer_norm"
         first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
-      emb_electrostatic:
-        encoder_type: "mlp"
-        input_keys: ["electrostatic"]
-        output_keys: ["feat"]
-        hidden_dim: 32
-        num_layers: 1
-        dropout: 0.1
-        normalization: "layer_norm" #"batch_norm" or "layer_norm"
-        first_normalization: "layer_norm" #"batch_norm" or "layer_norm"
-      emb_edge_rwse:
-        encoder_type: "mlp"
-        input_keys: ["edge_rw_transition_probs"]
-        output_keys: ["edge_feat"]
-        hidden_dim: 32
-        num_layers: 1
-        dropout: 0.1
-        normalization: "layer_norm" #"batch_norm" or "layer_norm"
-      emb_edge_pes:
-        encoder_type: "cat_mlp"
-        input_keys: ["edge_rw_transition_probs", "edge_commute"]
-        output_keys: ["edge_feat"]
-        hidden_dim: 32
-        num_layers: 1
-        dropout: 0.1
-        normalization: "layer_norm" #"batch_norm" or "layer_norm"
-      gaussian_pos:
-        encoder_type: "gaussian_kernel"
-        input_keys: ["positions_3d"]
-        output_keys: ["feat", "nodepair_gaussian_bias_3d"]
-        num_heads: &num_heads 2
-        num_layers: 2
-        embed_dim: *pe_out_dim
-        use_input_keys_prefix: False
+
+
 
   gnn:  # Set as null to avoid a post-nn network
-    out_dim: 8
-    hidden_dims: 16
-    depth: 2
-    activation: relu
+    in_dim: 64 # or otherwise the correct value
+    out_dim: &gnn_dim 768
+    hidden_dims: *gnn_dim
+    depth: 4
+    activation: gelu
     last_activation: none
-    dropout: *dropout
-    normalization: *normalization
+    dropout: 0.1
+    normalization: "layer_norm"
     last_normalization: *normalization
     residual_type: simple
     virtual_node: 'none'
-    layer_type: 'pyg:gps' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
-    layer_kwargs:  # Parameters for the model itself. You could define dropout_attn: 0.1
-      mpnn_type: 'pyg:gine'
-      mpnn_kwargs: null
-        #out_dim_edges: 10
-      attn_type: "none" # "full-attention", "none"
-      attn_kwargs: null
+    layer_type: 'pyg:gcn' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
+
 
   graph_output_nn:
     graph:
-      pooling: [sum, mean, max]
-      out_dim: 8
-      hidden_dims: 8
+      pooling: [sum]
+      out_dim: *gnn_dim
+      hidden_dims: *gnn_dim
       depth: 1
       activation: relu
       last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
 
   task_heads:
-    homo:
-      out_dim: 2
-      hidden_dims: 8
-      depth: 1                          # Not needed if we have hidden_dims
-      activation: relu
-      last_activation: none
-      dropout: *dropout
-      normalization: *normalization
-      last_normalization: "none"
-      residual_type: none
+    pcba_1328:
       task_level: graph
-    alpha:
-      out_dim: 1
-      hidden_dims: 8
-      depth: 1                          # Not needed if we have hidden_dims
+      out_dim: 1328
+      hidden_dims: 64
+      depth: 2
       activation: relu
-      last_activation: none
+      last_activation: sigmoid
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
-      task_level: graph
-    cv:
-      out_dim: 1
-      hidden_dims: 8
-      depth: 2                          # Not needed if we have hidden_dims
-      activation: relu
-      last_activation: none
-      dropout: *dropout
-      normalization: *normalization
-      last_normalization: "none"
-      residual_type: none
-      task_level: graph
 
 #Task-specific
 predictor:
   metrics_on_progress_bar:
-    homo: ["mae"]
-    alpha: ["mae"]
+    pcba_1328: []
+  metrics_on_training_set:
+    pcba_1328: []
   loss_fun:
-    homo: mse_ipu
-    alpha: mse_ipu
+    pcba_1328: bce_ipu
   random_seed: *seed
   optim_kwargs:
-    lr: 1.e-3
-  target_nan_mask: null
+    lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
+    # weight_decay: 1.e-7
+  torch_scheduler_kwargs:
+    module_type: WarmUpLinearLR
+    max_num_epochs: &max_epochs 20
+    warmup_epochs: 10
+    verbose: False
+  scheduler_kwargs:
+  #  monitor: &monitor qm9/mae/train
+  #  mode: min
+  #  frequency: 1
+  target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
+  multitask_handling: flatten # flatten, mean-per-label
 
 # Task-specific
 metrics:
-  homo:
-    - name: mae
-      metric: mae
+  pcba_1328:
+    - name: auroc
+      metric: auroc_ipu
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
-      target_nan_mask: null
-  alpha:
-    - name: mae
-      metric: mae
+    - name: avpr
+      metric: average_precision_ipu
+      task: binary
+      multitask_handling: mean-per-label
       threshold_kwargs: null
 
 trainer:
+  seed: *seed
   logger:
-    save_dir: logs/QM9
+    save_dir: logs/neurips2023-large/
     name: *name
+    project: *name
+  #early_stopping:
+  #  monitor: *monitor
+  #  min_delta: 0
+  #  patience: 10
+  #  mode: &mode min
   model_checkpoint:
-    dirpath: models_checkpoints/QM9/
+    dirpath: models_checkpoints/neurips2023-large-gcn/pcba/
     filename: *name
-    save_top_k: 1
-    every_n_epochs: 1
+    # monitor: *monitor
+    # mode: *mode
+    # save_top_k: 1
+    save_last: True
   trainer:
-    max_epochs: 2
+    max_epochs: *max_epochs
     min_epochs: 1
+    check_val_every_n_epoch: 20
```

### Comparing `graphium-2.0.2/tests/converted_fake_multilevel_data.parquet` & `graphium-2.1.0/tests/converted_fake_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/config_micro_ZINC.yaml` & `graphium-2.1.0/tests/data/config_micro_ZINC.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC.csv` & `graphium-2.1.0/tests/data/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC_corrupt.csv` & `graphium-2.1.0/tests/data/micro_ZINC_corrupt.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC_shard_1.csv` & `graphium-2.1.0/tests/data/micro_ZINC_shard_1.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC_shard_1.parquet` & `graphium-2.1.0/tests/data/micro_ZINC_shard_1.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC_shard_2.csv` & `graphium-2.1.0/tests/data/micro_ZINC_shard_2.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/micro_ZINC_shard_2.parquet` & `graphium-2.1.0/tests/data/micro_ZINC_shard_2.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/data/pcqm4mv2-2k.csv` & `graphium-2.1.0/tests/data/pcqm4mv2-2k.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/fake_and_missing_multilevel_data.parquet` & `graphium-2.1.0/tests/fake_and_missing_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_architectures.py` & `graphium-2.1.0/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_attention.py` & `graphium-2.1.0/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_base_layers.py` & `graphium-2.1.0/tests/test_base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_collate.py` & `graphium-2.1.0/tests/test_collate.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,37 +17,49 @@
         labels_size_dict = {
             "graph_label1": [1],
             "graph_label2": [3],
             "node_label2": [5],
             "edge_label3": [5, 2],
             "node_label4": [5, 1],
         }
+        labels_dtype_dict = {
+            "graph_label1": torch.float32,
+            "graph_label2": torch.float16,
+            "node_label2": torch.float32,
+            "edge_label3": torch.float32,
+            "node_label4": torch.float32,
+        }
         fake_label = {
             "graph_label1": torch.FloatTensor([1]),
-            "graph_label2": torch.FloatTensor([1, 2, 3]),
+            "graph_label2": torch.HalfTensor([1, 2, 3]),
             "node_label2": torch.FloatTensor([1, 2, 3, 4, 5]),
             "edge_label3": torch.FloatTensor([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]),
             "node_label4": torch.FloatTensor([[1], [2], [3], [4], [5]]),
         }
         fake_labels = []
         num_labels = 10
         for i in range(num_labels):
             pyg_labels = Data(x=torch.empty(5, 0), edge_index=torch.empty(2, 5))
             for key, val in fake_label.items():
                 pyg_labels[key] = val + 17 * 2
             fake_labels.append(pyg_labels)
 
-        # Collate labels and check for the right shapes
-        collated_labels = collate_labels(deepcopy(fake_labels), deepcopy(labels_size_dict))
+        # Collate labels and check for the right shapes and dtypes
+        collated_labels = collate_labels(
+            deepcopy(fake_labels), deepcopy(labels_size_dict), deepcopy(labels_dtype_dict)
+        )
         self.assertEqual(collated_labels["graph_label1"].shape, torch.Size([num_labels, 1]))  # , 1
         self.assertEqual(collated_labels["graph_label2"].shape, torch.Size([num_labels, 3]))  # , 1
         self.assertEqual(collated_labels["node_label2"].shape, torch.Size([num_labels * 5, 1]))  # , 5
         self.assertEqual(collated_labels["edge_label3"].shape, torch.Size([num_labels * 5, 2]))  # , 5, 2
         self.assertEqual(collated_labels["node_label4"].shape, torch.Size([num_labels * 5, 1]))  # , 5, 1
 
+        self.assertEqual(collated_labels["graph_label1"].dtype, torch.float32)
+        self.assertEqual(collated_labels["graph_label2"].dtype, torch.float16)
+
         # Check that the values are correct
         graph_label1_true = deepcopy(torch.stack([this_label["graph_label1"] for this_label in fake_labels]))
         graph_label2_true = deepcopy(torch.stack([this_label["graph_label2"] for this_label in fake_labels]))
         label2_true = deepcopy(torch.stack([this_label["node_label2"] for this_label in fake_labels]))
         label3_true = deepcopy(torch.stack([this_label["edge_label3"] for this_label in fake_labels]))
         label4_true = deepcopy(torch.stack([this_label["node_label4"] for this_label in fake_labels]))
 
@@ -85,15 +97,17 @@
         labels_size_dict = {
             "graph_label1": [1],
             "graph_label2": [3],
             "node_label2": [5],
             "edge_label3": [5, 2],
             "node_label4": [5, 1],
         }
-        collated_labels = collate_labels(deepcopy(fake_labels), deepcopy(labels_size_dict))
+        collated_labels = collate_labels(
+            deepcopy(fake_labels), deepcopy(labels_size_dict), deepcopy(labels_dtype_dict)
+        )
         self.assertEqual(collated_labels["graph_label1"].shape, torch.Size([num_labels, 1]))  # , 1
         self.assertEqual(collated_labels["graph_label2"].shape, torch.Size([num_labels, 3]))  # , 1
         self.assertEqual(collated_labels["node_label2"].shape, torch.Size([num_labels * 5, 1]))  # , 5
         self.assertEqual(collated_labels["edge_label3"].shape, torch.Size([num_labels * 5, 2]))  # , 5, 2
         self.assertEqual(collated_labels["node_label4"].shape, torch.Size([num_labels * 5, 1]))  # , 5, 1
 
         # Check that the values are correct when some labels are missing
@@ -107,17 +121,17 @@
             collated_labels["edge_label3"].numpy(), label3_true.flatten(0, 1).numpy()
         )
         np.testing.assert_array_equal(
             collated_labels["node_label4"].numpy(), label4_true.flatten(0, 1).numpy()
         )
         # Now test the `graphium_collate_fn` function when only labels are given
         fake_labels2 = [{"labels": this_label} for this_label in fake_labels]
-        collated_labels = graphium_collate_fn(deepcopy(fake_labels2), labels_size_dict=labels_size_dict)[
-            "labels"
-        ]
+        collated_labels = graphium_collate_fn(
+            deepcopy(fake_labels2), labels_size_dict=labels_size_dict, labels_dtype_dict=labels_dtype_dict
+        )["labels"]
         self.assertEqual(collated_labels["graph_label1"].shape, torch.Size([num_labels, 1]))
         self.assertEqual(collated_labels["graph_label2"].shape, torch.Size([num_labels, 3]))
         self.assertEqual(collated_labels["node_label2"].shape, torch.Size([num_labels * 5, 1]))  # , 5
         self.assertEqual(collated_labels["edge_label3"].shape, torch.Size([num_labels * 5, 2]))  # , 5, 2
         self.assertEqual(collated_labels["node_label4"].shape, torch.Size([num_labels * 5, 1]))  # , 5, 1
 
         # Check that the values are correct when some labels are missing
```

### Comparing `graphium-2.0.2/tests/test_data_utils.py` & `graphium-2.1.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_datamodule.py` & `graphium-2.1.0/tests/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_dataset.py` & `graphium-2.1.0/tests/test_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest as ut
 
 from graphium.data import load_micro_zinc
 from graphium.data.dataset import SingleTaskDataset, MultitaskDataset
 from graphium.data.smiles_transform import smiles_to_unique_mol_ids
+from graphium.data.utils import get_keys
 
 
 class Test_Multitask_Dataset(ut.TestCase):
     # Then we can choose different rows and columns for the tests as we see fit.
     # Remember tests are supposed to be FAST, and reading from the file system multiple times slows things down.
 
     # Make sure that the inputs to single task datasets are always lists!
@@ -133,27 +134,27 @@
             # Search for that molecule in the multitask dataset
             mol_ids = smiles_to_unique_mol_ids([smiles])
             mol_id = mol_ids[0]
             found_idx = -1
             for i, id in enumerate(multitask_microzinc.mol_ids):
                 if mol_id == id:
                     found_idx = i
-
+            multitask_microzinc_labels = get_keys(multitask_microzinc.labels[found_idx])
             if task == "SA":
                 self.assertEqual(label_SA, multitask_microzinc.labels[found_idx]["SA"])
-                self.assertFalse("score" in multitask_microzinc.labels[found_idx].keys)
-                self.assertFalse("logp" in multitask_microzinc.labels[found_idx].keys)
+                self.assertFalse("score" in multitask_microzinc_labels)
+                self.assertFalse("logp" in multitask_microzinc_labels)
             elif task == "logp":
                 self.assertEqual(label_logp, multitask_microzinc.labels[found_idx]["logp"])
-                self.assertFalse("score" in multitask_microzinc.labels[found_idx].keys)
-                self.assertFalse("SA" in multitask_microzinc.labels[found_idx].keys)
+                self.assertFalse("score" in multitask_microzinc_labels)
+                self.assertFalse("SA" in multitask_microzinc_labels)
             elif task == "score":
                 self.assertEqual(label_score, multitask_microzinc.labels[found_idx]["score"])
-                self.assertFalse("SA" in multitask_microzinc.labels[found_idx].keys)
-                self.assertFalse("logp" in multitask_microzinc.labels[found_idx].keys)
+                self.assertFalse("SA" in multitask_microzinc_labels)
+                self.assertFalse("logp" in multitask_microzinc_labels)
 
     def test_multitask_dataset_case_3(self):
         """Case: Different tasks, but with semi-intersection (some smiles unique per task, some intersect)
         - Check that the total dataset has as much smiles as the unique number of smiles.
         - Check that for each task, you retrieve the same smiles as expected from the initial DF
         """
         df_micro_zinc = load_micro_zinc()  # Has about 1000 molecules
```

### Comparing `graphium-2.0.2/tests/test_dict_tensor.py` & `graphium-2.1.0/tests/test_dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_featurizer.py` & `graphium-2.1.0/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_ipu_dataloader.py` & `graphium-2.1.0/tests/test_ipu_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # General imports
 import yaml
 import unittest as ut
 import numpy as np
 from copy import deepcopy
 from warnings import warn
-from pytorch_lightning import Trainer, LightningModule
-from pytorch_lightning.strategies import IPUStrategy
+from lightning import Trainer, LightningModule
+from lightning_graphcore import IPUStrategy
 from functools import partial
 
 import torch
 from torch.utils.data.dataloader import default_collate
 
 # Current library imports
 from graphium.config._loader import load_datamodule, load_metrics, load_architecture, load_accelerator
@@ -155,15 +155,16 @@
         strategy = IPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
         trainer = Trainer(
             logger=False,
             enable_checkpointing=False,
             max_epochs=2,
             strategy=strategy,
             num_sanity_val_steps=0,
-            ipus=1,
+            accelerator="ipu",
+            devices=1,
         )
         trainer.fit(model=model, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader)
 
     def test_poptorch_graphium_deviceiterations_gradient_accumulation(self):
         """
         Test the device-iterations and gradient accumulation in a way
         that is very similar to the Graphium code
@@ -235,41 +236,27 @@
                 assert (
                     this_shape == true_shape
                 ), f"Shape of the feature 0 is `{this_shape}` but should be {true_shape}. {msg}"
 
             def get_progress_bar_dict(self):
                 return {}
 
-            def on_train_batch_end(self, *args, **kwargs):
-                return
-
-            def on_validation_batch_end(self, *args, **kwargs):
-                return
-
-            def validation_epoch_end(self, *args, **kwargs):
-                return
-
-            def on_train_epoch_end(self) -> None:
-                return
-
             def configure_optimizers(self):
                 return torch.optim.Adam(self.parameters(), lr=1e-3)
 
             def squeeze_input_dims(self, features, labels):
                 for key, tensor in features:
                     if isinstance(tensor, torch.Tensor):
                         features[key] = features[key].squeeze(0)
 
                 for key in labels:
                     labels[key] = labels[key].squeeze(0)
 
                 return features, labels
 
-        from graphium.ipu.ipu_wrapper import DictIPUStrategy
-
         gradient_accumulation = 3
         device_iterations = 5
         batch_size = 7
 
         # Initialize the batch info and poptorch options
         opts = poptorch.Options()
         opts.deviceIterations(device_iterations)
@@ -302,15 +289,15 @@
             edge_batch_size=edge_factor * batch_size,
             in_dims=datamodule.in_dims,
             model_class=model_class,
             model_kwargs=model_kwargs,
             metrics=metrics,
             **cfg["predictor"],
         )
-        strategy = DictIPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
+        strategy = IPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
         trainer = Trainer(
             logger=False, enable_checkpointing=False, max_epochs=2, strategy=strategy, num_sanity_val_steps=0
         )
         trainer.fit(model=predictor, datamodule=datamodule)
 
 
 if __name__ == "__main__":
```

### Comparing `graphium-2.0.2/tests/test_ipu_losses.py` & `graphium-2.1.0/tests/test_ipu_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_ipu_metrics.py` & `graphium-2.1.0/tests/test_ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_loaders.py` & `graphium-2.1.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_losses.py` & `graphium-2.1.0/tests/test_losses.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,61 +15,65 @@
     return eval_options.parse_loss_fun(loss_fun)
 
 
 class test_HybridCELoss(ut.TestCase):
     input = torch.Tensor([[0.1, 0.1, 0.3, 0.5, 0.0], [0.1, 0.0, 0.7, 0.2, 0.0]])
     target = torch.Tensor([3, 0]).long()
     brackets = torch.Tensor([0, 1, 2, 3, 4])
-    regression_input = torch.Tensor([2.2, 2.0])  # inner product of input and brackets
+    regression_input = torch.Tensor([2.0537, 2.0017])  # inner product of input and brackets
     regression_target = torch.Tensor([3, 0]).float()
 
     def test_pure_ce_loss(self):
         loss = HybridCELoss(n_brackets=len(self.brackets), alpha=1.0, reduction="none")
-
         assert torch.allclose(
             loss(self.input, self.target),
             F.cross_entropy(self.input, self.target, reduction="none"),
         )
         assert loss(self.input, self.target).shape == (2,)
 
     def test_pure_mae_loss(self):
         loss = HybridCELoss(
             n_brackets=len(self.brackets),
             alpha=0.0,
             regression_loss="mae",
             reduction="none",
         )
-
         assert torch.allclose(
             loss(self.input, self.target),
             F.l1_loss(self.regression_input, self.regression_target, reduction="none"),
+            rtol=1e-04,
+            atol=1e-07,
         )
         assert loss(self.input, self.target).shape == (2,)
 
     def test_pure_mse_loss(self):
         loss = HybridCELoss(
             n_brackets=len(self.brackets),
             alpha=0.0,
             regression_loss="mse",
             reduction="none",
         )
 
         assert torch.allclose(
             loss(self.input, self.target),
             F.mse_loss(self.regression_input, self.regression_target, reduction="none"),
+            rtol=1e-04,
+            atol=1e-07,
         )
         assert loss(self.input, self.target).shape == (2,)
 
     def test_hybrid_loss(self):
         loss = HybridCELoss(n_brackets=len(self.brackets), alpha=0.5, regression_loss="mse")
 
         ce_loss = F.cross_entropy(self.input, self.target)
         mse_loss = F.mse_loss(self.regression_input, self.regression_target)
 
-        assert torch.allclose(loss(self.input, self.target), 0.5 * ce_loss + 0.5 * mse_loss)
+        assert torch.allclose(
+            loss(self.input, self.target), 0.5 * ce_loss + 0.5 * mse_loss, rtol=1e-04, atol=1e-07
+        )
         assert loss(self.input, self.target).shape == torch.Size([])
 
     def test_loss_parser(self):
         # HybridCE cannot be parsed from a string because it requires specifying n_brackets
         loss_fun = "hybrid_ce"
         self.assertRaises(TypeError, _parse, loss_fun=loss_fun)
```

### Comparing `graphium-2.0.2/tests/test_metrics.py` & `graphium-2.1.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_mtl_architecture.py` & `graphium-2.1.0/tests/test_mtl_architecture.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_multitask_datamodule.py` & `graphium-2.1.0/tests/test_multitask_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_mup.py` & `graphium-2.1.0/tests/test_mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_packing.py` & `graphium-2.1.0/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_pe_nodepair.py` & `graphium-2.1.0/tests/test_pe_nodepair.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_pe_rw.py` & `graphium-2.1.0/tests/test_pe_rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_pe_spectral.py` & `graphium-2.1.0/tests/test_pe_spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_pos_transfer_funcs.py` & `graphium-2.1.0/tests/test_pos_transfer_funcs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_positional_encoders.py` & `graphium-2.1.0/tests/test_positional_encoders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_positional_encodings.py` & `graphium-2.1.0/tests/test_positional_encodings.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_predictor.py` & `graphium-2.1.0/tests/test_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_pyg_layers.py` & `graphium-2.1.0/tests/test_pyg_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_residual_connections.py` & `graphium-2.1.0/tests/test_residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.0.2/tests/test_utils.py` & `graphium-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

